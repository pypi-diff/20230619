# Comparing `tmp/web_ext_helper-1.1.3.tar.gz` & `tmp/web_ext_helper-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_ext_helper-1.1.3.tar", max compression
+gzip compressed data, was "web_ext_helper-1.1.4.tar", max compression
```

## Comparing `web_ext_helper-1.1.3.tar` & `web_ext_helper-1.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.1.3/LICENSE
--rw-r--r--   0        0        0      654 2023-06-19 16:49:56.278302 web_ext_helper-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1754 2023-06-17 20:34:00.666577 web_ext_helper-1.1.3/README.md
--rw-r--r--   0        0        0      262 2023-06-18 17:57:02.181036 web_ext_helper-1.1.3/web_ext_helper/classes.py
--rw-r--r--   0        0        0      613 2023-06-18 17:49:15.766872 web_ext_helper-1.1.3/web_ext_helper/functions.py
--rw-r--r--   0        0        0    18433 2023-06-19 16:49:48.739408 web_ext_helper-1.1.3/web_ext_helper/web_ext_helper.py
--rw-r--r--   0        0        0     2325 1970-01-01 00:00:00.000000 web_ext_helper-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.1.4/LICENSE
+-rw-r--r--   0        0        0      654 2023-06-19 17:30:04.196280 web_ext_helper-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1871 2023-06-19 17:29:34.258602 web_ext_helper-1.1.4/README.md
+-rw-r--r--   0        0        0      262 2023-06-18 17:57:02.181036 web_ext_helper-1.1.4/web_ext_helper/classes.py
+-rw-r--r--   0        0        0      613 2023-06-18 17:49:15.766872 web_ext_helper-1.1.4/web_ext_helper/functions.py
+-rw-r--r--   0        0        0    18433 2023-06-19 17:29:54.980463 web_ext_helper-1.1.4/web_ext_helper/web_ext_helper.py
+-rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 web_ext_helper-1.1.4/PKG-INFO
```

### Comparing `web_ext_helper-1.1.3/LICENSE` & `web_ext_helper-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.1.3/pyproject.toml` & `web_ext_helper-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web-ext-helper"
-version = "1.1.3"
+version = "1.1.4"
 description = "A simple cli tool that helps you building your web extensions."
 authors = ["AppSolves <appsolves@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "web_ext_helper"}]
 
 [tool.poetry.dependencies]
```

### Comparing `web_ext_helper-1.1.3/README.md` & `web_ext_helper-1.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [Web Extension Helper](https://www.appsolves.dev/python-packages/web-extension-helper) is a command-line tool that simplifies the process of building web extensions. It provides a convenient interface to streamline the development and packaging of your web extensions.
 
 ## Features
 
 - Easily scaffold a new web extension project.
 - Automate common tasks like bundling and minification.
-- Simplify the process of publishing your web extension.
+- Simplify the process of building and publishing your web extension.
 
 ## Installation
 
 Web Extension Helper can be installed via pip:
 
 ```shell
 pip install web-ext-helper
@@ -24,14 +24,20 @@
 
 To use Web Extension Helper, run the web-ext-helper command followed by the desired action. Here are some examples:
 
 ```shell
 * Build the web extension
 web-ext-helper build
 
+* Sign the web extension
+web-ext-helper sign
+
+* Publish the web extension
+web-ext-helper publish
+
 * Create a new manifest.json file
 web-ext-helper manifest --create
 
 * View the current manifest.json file
 web-ext-helper manifest
 
 * View the help menu
```

### Comparing `web_ext_helper-1.1.3/web_ext_helper/functions.py` & `web_ext_helper-1.1.4/web_ext_helper/functions.py`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.1.3/web_ext_helper/web_ext_helper.py` & `web_ext_helper-1.1.4/web_ext_helper/web_ext_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__ext_version__ = "1.1.3"
+__ext_version__ = "1.1.4"
 
 import os
 import json
 import shutil
 import typer
 import zipfile
 import rich.progress
```

### Comparing `web_ext_helper-1.1.3/PKG-INFO` & `web_ext_helper-1.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ext-helper
-Version: 1.1.3
+Version: 1.1.4
 Summary: A simple cli tool that helps you building your web extensions.
 License: GPL-3.0-or-later
 Author: AppSolves
 Author-email: appsolves@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 
 [Web Extension Helper](https://www.appsolves.dev/python-packages/web-extension-helper) is a command-line tool that simplifies the process of building web extensions. It provides a convenient interface to streamline the development and packaging of your web extensions.
 
 ## Features
 
 - Easily scaffold a new web extension project.
 - Automate common tasks like bundling and minification.
-- Simplify the process of publishing your web extension.
+- Simplify the process of building and publishing your web extension.
 
 ## Installation
 
 Web Extension Helper can be installed via pip:
 
 ```shell
 pip install web-ext-helper
@@ -41,14 +41,20 @@
 
 To use Web Extension Helper, run the web-ext-helper command followed by the desired action. Here are some examples:
 
 ```shell
 * Build the web extension
 web-ext-helper build
 
+* Sign the web extension
+web-ext-helper sign
+
+* Publish the web extension
+web-ext-helper publish
+
 * Create a new manifest.json file
 web-ext-helper manifest --create
 
 * View the current manifest.json file
 web-ext-helper manifest
 
 * View the help menu
```

