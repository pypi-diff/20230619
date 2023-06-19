# Comparing `tmp/webdriver_kaifuku-22.6.28.0.tar.gz` & `tmp/webdriver_kaifuku-23.6.19.0.tar.gz`

## Comparing `webdriver_kaifuku-22.6.28.0.tar` & `webdriver_kaifuku-23.6.19.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 webdriver_kaifuku-22.6.28.0/LICENSE
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 webdriver_kaifuku-22.6.28.0/README.md
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 webdriver_kaifuku-22.6.28.0/pyproject.toml
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 webdriver_kaifuku-22.6.28.0/src/webdriver_kaifuku/__init__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 webdriver_kaifuku-22.6.28.0/src/webdriver_kaifuku/tries.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 webdriver_kaifuku-22.6.28.0/.gitignore
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 webdriver_kaifuku-22.6.28.0/PKG-INFO
+-rw-r--r--   0        0        0     8855 2020-02-02 00:00:00.000000 webdriver_kaifuku-23.6.19.0/src/webdriver_kaifuku/__init__.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 webdriver_kaifuku-23.6.19.0/src/webdriver_kaifuku/tries.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 webdriver_kaifuku-23.6.19.0/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 webdriver_kaifuku-23.6.19.0/LICENSE
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 webdriver_kaifuku-23.6.19.0/README.md
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 webdriver_kaifuku-23.6.19.0/pyproject.toml
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 webdriver_kaifuku-23.6.19.0/PKG-INFO
```

### Comparing `webdriver_kaifuku-22.6.28.0/LICENSE` & `webdriver_kaifuku-23.6.19.0/LICENSE`

 * *Files identical despite different names*

### Comparing `webdriver_kaifuku-22.6.28.0/README.md` & `webdriver_kaifuku-23.6.19.0/README.md`

 * *Files identical despite different names*

### Comparing `webdriver_kaifuku-22.6.28.0/pyproject.toml` & `webdriver_kaifuku-23.6.19.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -39,8 +39,10 @@
 include = ["/src"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["/src/webdriver_kaifuku"]
 
 [tool.hatch.version]
 raw-options.version_scheme = "calver-by-date"
+# re-enable after fixing https://github.com/pypa/setuptools_scm/issues/768
+# raw-options.normalize = false
 source = "vcs"
```

### Comparing `webdriver_kaifuku-22.6.28.0/src/webdriver_kaifuku/__init__.py` & `webdriver_kaifuku-23.6.19.0/src/webdriver_kaifuku/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,24 +23,52 @@
 
 THIRTY_SECONDS = 30
 
 BROWSER_ERRORS = URLError, WebDriverException
 TRUSTED_WEB_DRIVERS = [webdriver.Firefox, webdriver.Chrome, webdriver.Remote]
 
 
-def _get_browser_name(webdriver_kwargs: dict) -> str:
+def _get_browser_name(webdriver_kwargs: dict, webdriver_name: str) -> str:
     """
-    Extract the name of the browser from the desired capabilities
+    Extract the name of the browser from the browser config
     """
-    name = webdriver_kwargs.get("desired_capabilities", {}).get("browserName")
+    if webdriver_name.lower() == "remote":
+        name_from_options = (
+            webdriver_kwargs["options"].to_capabilities().get("browserName")
+            if "options" in webdriver_kwargs
+            else None
+        )
+        name_from_desired_capabilities = webdriver_kwargs.get("desired_capabilities", {}).get(
+            "browserName"
+        )
+        name = name_from_options or name_from_desired_capabilities
+    else:
+        name = webdriver_name
     if name:
         return name.lower()
     raise ValueError("No browser name specified")
 
 
+def _remove_deprecated_items(browser_conf: dict) -> dict:
+    """
+    Remove deprecated items from browser config
+    """
+    deprecated_items = ["perfLoggingPrefs", "marionette"]
+    opts = browser_conf.get("webdriver_options", {})
+    if opts and "desired_capabilities" in opts:
+        for i in deprecated_items:
+            if i in opts["desired_capabilities"]:
+                log.warning(
+                    f"'{i}' capability has been deprecated in Selenium 4.10. "
+                    f"Remove it from your browser config"
+                )
+                del browser_conf["webdriver_options"]["desired_capabilities"][i]
+    return browser_conf
+
+
 @define(auto_attribs=True)
 class BrowserFactory:
     ALLOWED_KWARGS: ClassVar[list[str]] = ["command_executor", "options", "keep_alive"]
     webdriver_class: type
     webdriver_kwargs: dict
 
     def processed_browser_args(self):
@@ -74,37 +102,48 @@
 @define(auto_attribs=True)
 class BrowserManager:
     browser_factory: BrowserFactory
     browser: WebDriver | None = field(default=None, init=False)
 
     @staticmethod
     def _config_options_for_remote_chrome(browser_conf: dict) -> webdriver.ChromeOptions:
-        opts = webdriver.ChromeOptions()
-        desired_capabilities = browser_conf.get("webdriver_options", {}).get(
-            "desired_capabilities", {}
-        )
-        desired_capabilities_chrome_options = desired_capabilities.pop("chromeOptions", {})
-        chrome_args = desired_capabilities_chrome_options.get("args", [])
-        for arg in chrome_args:
-            if arg not in opts.arguments:
-                opts.add_argument(arg)
+        opts = browser_conf.get("webdriver_options", {}).get("options", webdriver.ChromeOptions())
+        chrome_options = browser_conf.get("webdriver_options", {}).get("desired_capabilities", {})
+        additional_chrome_opts = chrome_options.pop("chromeOptions", {})
+
+        chrome_args = additional_chrome_opts.get("args", [])
+        if chrome_args:
+            for arg in chrome_args:
+                if arg not in opts.arguments:
+                    opts.add_argument(arg)
         opts.add_argument("--no-sandbox")
         if "proxy_url" in browser_conf:
             opts.add_argument(f"--proxy-server={browser_conf['proxy_url']}")
-        for key, value in desired_capabilities.items():
+        for key, value in chrome_options.items():
             opts.set_capability(key, value)
         return opts
 
     @staticmethod
     def _config_options_for_remote_firefox(browser_conf: dict) -> webdriver.FirefoxOptions:
-        opts = webdriver.FirefoxOptions()
-        desired_capabilities = browser_conf.get("webdriver_options", {}).get(
-            "desired_capabilities", {}
-        )
-        for key, value in desired_capabilities.items():
+        opts = browser_conf.get("webdriver_options", {}).get("options", webdriver.FirefoxOptions())
+        firefox_options = browser_conf.get("webdriver_options", {}).get("desired_capabilities", {})
+        additional_firefox_opts = firefox_options.pop("firefoxOptions", {})
+
+        firefox_args = additional_firefox_opts.get("args", [])
+        if firefox_args:
+            for arg in firefox_args:
+                if arg not in opts.arguments:
+                    opts.add_argument(arg)
+
+        firefox_prefs = additional_firefox_opts.get("prefs", {})
+        for pref, value in firefox_prefs.items():
+            if pref not in opts.arguments:
+                opts.set_preference(pref, value)
+
+        for key, value in firefox_options.items():
             opts.set_capability(key, value)
         if "proxy_url" in browser_conf:
             opts.set_capability(
                 "proxy",
                 {
                     "proxyType": "MANUAL",
                     "httpProxy": browser_conf["proxy_url"],
@@ -112,34 +151,36 @@
                 },
             )
         return opts
 
     @classmethod
     def from_conf(cls, browser_conf: dict) -> BrowserManager:
         browser_conf = copy(browser_conf)
+        browser_conf = _remove_deprecated_items(browser_conf)
+
         log.debug(browser_conf)
-        webdriver_name = browser_conf.get("webdriver", "Firefox").title()
+        webdriver_name = browser_conf.get("webdriver", "Chrome").title()
         webdriver_class = getattr(webdriver, webdriver_name)
 
         if webdriver_class not in TRUSTED_WEB_DRIVERS:
             log.warning(f"Untrusted webdriver {webdriver_name}, may cause failure.")
 
         webdriver_kwargs = browser_conf.get("webdriver_options", {})
-        browser_name = _get_browser_name(webdriver_kwargs)
+        browser_name = _get_browser_name(webdriver_kwargs, webdriver_name)
 
         if "proxy_url" in browser_conf:
             parsed_url = urlparse(browser_conf["proxy_url"])
             proxy_netloc = parsed_url.netloc or parsed_url.path
             browser_conf["proxy_url"] = proxy_netloc
-        if browser_name == "chrome":
+        if browser_name == "chrome" and webdriver_class == webdriver.Remote:
             webdriver_kwargs["options"] = cls._config_options_for_remote_chrome(browser_conf)
-        if browser_name == "firefox":
+        if browser_name == "firefox" and webdriver_class == webdriver.Remote:
             webdriver_kwargs["options"] = cls._config_options_for_remote_firefox(browser_conf)
 
-        if webdriver_class == webdriver.Remote and "command_executor" in browser_conf:
+        if webdriver_class in TRUSTED_WEB_DRIVERS and "command_executor" in browser_conf:
             webdriver_kwargs["command_executor"] = browser_conf["command_executor"]
         return cls(BrowserFactory(webdriver_class, webdriver_kwargs))
 
     @property
     def is_alive(self) -> bool:
         log.debug("alive check")
         if self.browser is None:
```

### Comparing `webdriver_kaifuku-22.6.28.0/src/webdriver_kaifuku/tries.py` & `webdriver_kaifuku-23.6.19.0/src/webdriver_kaifuku/tries.py`

 * *Files identical despite different names*

### Comparing `webdriver_kaifuku-22.6.28.0/.gitignore` & `webdriver_kaifuku-23.6.19.0/.gitignore`

 * *Files identical despite different names*

### Comparing `webdriver_kaifuku-22.6.28.0/PKG-INFO` & `webdriver_kaifuku-23.6.19.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
-Name: webdriver-kaifuku
-Version: 22.6.28.0
+Name: webdriver_kaifuku
+Version: 23.6.19.0
 Summary: Restartable webdriver instances
 Project-URL: repository, https://github.com/RonnyPfannschmidt/webdriver_kaifuku
+License-File: LICENSE
 Keywords: selenium
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8
 Requires-Dist: attrs
 Requires-Dist: requests
 Requires-Dist: selenium>=4.0.0
 Provides-Extra: test
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: webdriver-kaifuku Version: 22.6.28.0 Summary:
+Metadata-Version: 2.1 Name: webdriver_kaifuku Version: 23.6.19.0 Summary:
 Restartable webdriver instances Project-URL: repository, https://github.com/
-RonnyPfannschmidt/webdriver_kaifuku Keywords: selenium Classifier: License ::
-OSI Approved :: Mozilla Public License 2.0 (MPL 2.0) Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.10 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Topic :: Software Development :: Quality
-Assurance Classifier: Topic :: Software Development :: Testing Requires-Python:
->=3.8 Requires-Dist: attrs Requires-Dist: requests Requires-Dist:
-selenium>=4.0.0 Provides-Extra: test Requires-Dist: pytest; extra == 'test'
-Requires-Dist: wait-for; extra == 'test' Description-Content-Type: text/
-markdown
+RonnyPfannschmidt/webdriver_kaifuku License-File: LICENSE Keywords: selenium
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
+Software Development :: Quality Assurance Classifier: Topic :: Software
+Development :: Testing Requires-Python: >=3.8 Requires-Dist: attrs Requires-
+Dist: requests Requires-Dist: selenium>=4.0.0 Provides-Extra: test Requires-
+Dist: pytest; extra == 'test' Requires-Dist: wait-for; extra == 'test'
+Description-Content-Type: text/markdown
                         ****** webdriver_kaifuku ******
                    **** Restartable webdriver instances ****
   [Python_Versions] [PyPI_version] [https://codecov.io/gh/RonnyPfannschmidt/
   webdriver_kaifuku/branch/master/graph/badge.svg] [github_actions] [License]
 The library provides restartable webdriver instances. ### Usage: It support
 both `local` and `remote` webdriver. Some basic examples are- - Local Browser
 Make sure `webdriver` is already installed on your local machine. ```python
```

