# Comparing `tmp/revChatGPT-6.3.3.tar.gz` & `tmp/revChatGPT-6.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.3.3.tar", last modified: Sat Jun 17 02:23:23 2023, max compression
+gzip compressed data, was "revChatGPT-6.3.4.tar", last modified: Mon Jun 19 08:42:43 2023, max compression
```

## Comparing `revChatGPT-6.3.3.tar` & `revChatGPT-6.3.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:23:23.733875 revChatGPT-6.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-17 02:22:55.000000 revChatGPT-6.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-17 02:23:23.733875 revChatGPT-6.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-17 02:23:23.000000 revChatGPT-6.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-17 02:23:23.733875 revChatGPT-6.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-17 02:22:55.000000 revChatGPT-6.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:23:23.729875 revChatGPT-6.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:23:23.733875 revChatGPT-6.3.3/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    58838 2023-06-17 02:22:55.000000 revChatGPT-6.3.3/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23492 2023-06-17 02:22:55.000000 revChatGPT-6.3.3/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-17 02:22:55.000000 revChatGPT-6.3.3/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-17 02:22:55.000000 revChatGPT-6.3.3/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:23:23.733875 revChatGPT-6.3.3/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-17 02:22:55.000000 revChatGPT-6.3.3/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-17 02:22:55.000000 revChatGPT-6.3.3/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-17 02:22:55.000000 revChatGPT-6.3.3/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:23:23.733875 revChatGPT-6.3.3/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-17 02:23:23.000000 revChatGPT-6.3.3/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-17 02:23:23.000000 revChatGPT-6.3.3/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 02:23:23.000000 revChatGPT-6.3.3/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 02:23:23.000000 revChatGPT-6.3.3/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-17 02:23:23.000000 revChatGPT-6.3.3/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:23:23.733875 revChatGPT-6.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-17 02:22:55.000000 revChatGPT-6.3.3/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:42:43.618160 revChatGPT-6.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-19 08:42:14.000000 revChatGPT-6.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-19 08:42:43.618160 revChatGPT-6.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-19 08:42:43.000000 revChatGPT-6.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-19 08:42:43.618160 revChatGPT-6.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-19 08:42:14.000000 revChatGPT-6.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:42:43.614160 revChatGPT-6.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:42:43.618160 revChatGPT-6.3.4/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    58973 2023-06-19 08:42:14.000000 revChatGPT-6.3.4/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23492 2023-06-19 08:42:14.000000 revChatGPT-6.3.4/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-19 08:42:14.000000 revChatGPT-6.3.4/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-19 08:42:14.000000 revChatGPT-6.3.4/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:42:43.618160 revChatGPT-6.3.4/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-19 08:42:14.000000 revChatGPT-6.3.4/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-19 08:42:14.000000 revChatGPT-6.3.4/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-19 08:42:14.000000 revChatGPT-6.3.4/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:42:43.618160 revChatGPT-6.3.4/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-19 08:42:43.000000 revChatGPT-6.3.4/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-19 08:42:43.000000 revChatGPT-6.3.4/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:42:43.000000 revChatGPT-6.3.4/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-19 08:42:43.000000 revChatGPT-6.3.4/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-19 08:42:43.000000 revChatGPT-6.3.4/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:42:43.618160 revChatGPT-6.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-19 08:42:14.000000 revChatGPT-6.3.4/tests/test_recipient.py
```

### Comparing `revChatGPT-6.3.3/LICENSE` & `revChatGPT-6.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.3/PKG-INFO` & `revChatGPT-6.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.3.3
+Version: 6.3.4
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.3.3/README.md` & `revChatGPT-6.3.4/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.3/setup.py` & `revChatGPT-6.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="6.3.3",
+    version="6.3.4",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
@@ -33,14 +33,15 @@
         "requests[socks]",
         "httpx[socks]",
         "async_tio",
         "prompt-toolkit",
         "tiktoken>=0.3.0",
         "openai",
         "curl_cffi",
+        "rich",
     ],
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Intended Audience :: Developers",
         "Intended Audience :: End Users/Desktop",
         "Natural Language :: English",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `revChatGPT-6.3.3/src/revChatGPT/V1.py` & `revChatGPT-6.3.4/src/revChatGPT/V1.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 from typing import NoReturn
 
 import httpx
 import requests
 from httpx import AsyncClient
 from OpenAIAuth import Auth0 as Authenticator
 
+from rich.live import Live
+from rich.markdown import Markdown
+
 from . import __version__
 from . import typings as t
 from .utils import create_completer
 from .utils import create_session
 from .utils import get_input
 
 
@@ -199,17 +202,21 @@
 
         if self.config.get("plugin_ids", []):
             for plugin in self.config.get("plugin_ids"):
                 self.install_plugin(plugin)
         if self.config.get("unverified_plugin_domains", []):
             for domain in self.config.get("unverified_plugin_domains"):
                 if self.config.get("plugin_ids"):
-                    self.config["plugin_ids"].append(self.get_unverified_plugin(domain,install=True).get("id"))
+                    self.config["plugin_ids"].append(
+                        self.get_unverified_plugin(domain, install=True).get("id")
+                    )
                 else:
-                    self.config["plugin_ids"] = [self.get_unverified_plugin(domain,install=True).get("id")]
+                    self.config["plugin_ids"] = [
+                        self.get_unverified_plugin(domain, install=True).get("id")
+                    ]
 
     @logger(is_timed=True)
     def __check_credentials(self) -> None:
         """Check login info and perform login
 
         Any one of the following is sufficient for login. Multiple login info can be provided at the same time and they will be used in the order listed below.
             - access_token
@@ -1537,23 +1544,21 @@
             if prompt.startswith("!") and handle_commands(prompt):
                 continue
 
             print()
             print(f"{bcolors.OKGREEN + bcolors.BOLD}Chatbot: {bcolors.ENDC}")
             if chatbot.config.get("model") == "gpt-4-browsing":
                 print("Browsing takes a while, please wait...")
-            prev_text = ""
-            for data in chatbot.ask(prompt=prompt, auto_continue=True):
-                if data["recipient"] != "all":
-                    continue
-                result = data
-                message = data["message"][len(prev_text) :]
-                print(message, end="", flush=True)
-                prev_text = data["message"]
-            print(bcolors.ENDC)
+            with Live(Markdown(""), auto_refresh=False) as live:
+                for data in chatbot.ask(prompt=prompt, auto_continue=True):
+                    if data["recipient"] != "all":
+                        continue
+                    result = data
+                    message = data["message"]
+                    live.update(Markdown(message), refresh=True)
             print()
 
             if result.get("citations", False):
                 print(
                     f"{bcolors.WARNING + bcolors.BOLD}Citations: {bcolors.ENDC}",
                 )
                 for citation in result["citations"]:
```

### Comparing `revChatGPT-6.3.3/src/revChatGPT/V3.py` & `revChatGPT-6.3.4/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.3/src/revChatGPT/__init__.py` & `revChatGPT-6.3.4/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.3/src/revChatGPT/__main__.py` & `revChatGPT-6.3.4/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.3/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.3.4/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.3/src/revChatGPT/typings.py` & `revChatGPT-6.3.4/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.3/src/revChatGPT/utils.py` & `revChatGPT-6.3.4/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.3/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.3.4/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.3.3
+Version: 6.3.4
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.3.3/tests/test_recipient.py` & `revChatGPT-6.3.4/tests/test_recipient.py`

 * *Files identical despite different names*

