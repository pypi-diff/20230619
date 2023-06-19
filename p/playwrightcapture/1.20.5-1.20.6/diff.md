# Comparing `tmp/playwrightcapture-1.20.5.tar.gz` & `tmp/playwrightcapture-1.20.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.20.5.tar", max compression
+gzip compressed data, was "playwrightcapture-1.20.6.tar", max compression
```

## Comparing `playwrightcapture-1.20.5.tar` & `playwrightcapture-1.20.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.20.5/LICENSE
--rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.20.5/README.md
--rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.20.5/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    36844 2023-06-15 16:17:17.999029 playwrightcapture-1.20.5/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.20.5/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     1734 2023-06-06 09:15:52.098307 playwrightcapture-1.20.5/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.20.5/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1828 2023-06-15 16:20:12.123618 playwrightcapture-1.20.5/pyproject.toml
--rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 playwrightcapture-1.20.5/PKG-INFO
+-rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.20.6/LICENSE
+-rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.20.6/README.md
+-rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.20.6/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    36868 2023-06-19 09:52:41.331440 playwrightcapture-1.20.6/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.20.6/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     1734 2023-06-06 09:15:52.098307 playwrightcapture-1.20.6/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.20.6/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1828 2023-06-19 14:49:16.933781 playwrightcapture-1.20.6/pyproject.toml
+-rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 playwrightcapture-1.20.6/PKG-INFO
```

### Comparing `playwrightcapture-1.20.5/LICENSE` & `playwrightcapture-1.20.6/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.5/README.md` & `playwrightcapture-1.20.6/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.5/playwrightcapture/capture.py` & `playwrightcapture-1.20.6/playwrightcapture/capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -671,15 +671,15 @@
                 # unable to sanitize
                 self.logger.warning(f'Unable to sanitize link: "{href}" - {e}')
 
         return sorted(urls)
 
     async def _recaptcha_solver(self, page: Page) -> bool:
         try:
-            framename = await page.locator("//iframe[@title='reCAPTCHA']").get_attribute("name")
+            framename = await page.locator("//iframe[@title='reCAPTCHA']").first.get_attribute("name")
             if not framename:
                 return False
         except PlaywrightTimeoutError as e:
             self.logger.info(f'Captcha not ready: {e}')
             return False
 
         recaptcha_init_frame = page.frame(name=framename)
@@ -694,23 +694,23 @@
                 return False
         except PlaywrightTimeoutError as e:
             self.logger.info(f'Checkbox never ready: {e}')
             return False
 
         await page.wait_for_timeout(random.randint(3, 6) * 1000)
         try:
-            if await recaptcha_init_frame.locator("//span[@id='recaptcha-anchor']").is_checked(timeout=5000):  # solved already
+            if await recaptcha_init_frame.locator("//span[@id='recaptcha-anchor']").first.is_checked(timeout=5000):  # solved already
                 return True
         except PlaywrightTimeoutError:
             self.logger.info('Need to solve the captcha.')
 
         possible_urls = ['https://google.com/recaptcha/api2/bframe?', 'https://google.com/recaptcha/enterprise/bframe?']
         for url in possible_urls:
             try:
-                recaptcha_testframename = await page.locator(f"//iframe[contains(@src,'{url}')]").get_attribute("name")
+                recaptcha_testframename = await page.locator(f"//iframe[contains(@src,'{url}')]").first.get_attribute("name")
                 if recaptcha_testframename:
                     self.logger.debug(f'Got iframe with {url}')
                     break
             except PlaywrightTimeoutError:
                 self.logger.debug(f'Unable to get iframe with {url}')
                 continue
         else:
@@ -742,15 +742,15 @@
                     audio = recognizer.record(source)
                 text = recognizer.recognize_google(audio)
             await main_frame.get_by_role("textbox", name="Enter what you hear").fill(text)
             await main_frame.get_by_role("button", name="Verify").click()
             await self._safe_wait(page)
             await page.wait_for_timeout(random.randint(3, 6) * 1000)
             try:
-                if await recaptcha_init_frame.locator("//span[@id='recaptcha-anchor']").is_checked(timeout=5000):
+                if await recaptcha_init_frame.locator("//span[@id='recaptcha-anchor']").first.is_checked(timeout=5000):
                     self.logger.info('Captcha solved successfully')
                     return True
                 elif await main_frame.get_by_role("textbox", name="Enter what you hear").is_editable(timeout=5000):
                     self.logger.info('Unable to find checkbox, needs to solve more captchas')
             except PlaywrightTimeoutError as e:
                 self.logger.info(f'Unexpected timeout: {e}')
```

### Comparing `playwrightcapture-1.20.5/playwrightcapture/helpers.py` & `playwrightcapture-1.20.6/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.5/pyproject.toml` & `playwrightcapture-1.20.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.20.5"
+version = "1.20.6"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
```

### Comparing `playwrightcapture-1.20.5/PKG-INFO` & `playwrightcapture-1.20.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwrightcapture
-Version: 1.20.5
+Version: 1.20.6
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
```

