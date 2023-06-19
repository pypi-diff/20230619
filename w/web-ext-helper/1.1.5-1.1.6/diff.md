# Comparing `tmp/web_ext_helper-1.1.5.tar.gz` & `tmp/web_ext_helper-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_ext_helper-1.1.5.tar", max compression
+gzip compressed data, was "web_ext_helper-1.1.6.tar", max compression
```

## Comparing `web_ext_helper-1.1.5.tar` & `web_ext_helper-1.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.1.5/LICENSE
--rw-r--r--   0        0        0      654 2023-06-19 17:37:33.886377 web_ext_helper-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1871 2023-06-19 17:29:34.258602 web_ext_helper-1.1.5/README.md
--rw-r--r--   0        0        0      262 2023-06-18 17:57:02.181036 web_ext_helper-1.1.5/web_ext_helper/classes.py
--rw-r--r--   0        0        0      613 2023-06-18 17:49:15.766872 web_ext_helper-1.1.5/web_ext_helper/functions.py
--rw-r--r--   0        0        0    18478 2023-06-19 17:37:27.898020 web_ext_helper-1.1.5/web_ext_helper/web_ext_helper.py
--rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 web_ext_helper-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.1.6/LICENSE
+-rw-r--r--   0        0        0      654 2023-06-19 17:41:14.311771 web_ext_helper-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1871 2023-06-19 17:29:34.258602 web_ext_helper-1.1.6/README.md
+-rw-r--r--   0        0        0      262 2023-06-18 17:57:02.181036 web_ext_helper-1.1.6/web_ext_helper/classes.py
+-rw-r--r--   0        0        0      613 2023-06-18 17:49:15.766872 web_ext_helper-1.1.6/web_ext_helper/functions.py
+-rw-r--r--   0        0        0    18518 2023-06-19 17:40:52.404327 web_ext_helper-1.1.6/web_ext_helper/web_ext_helper.py
+-rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 web_ext_helper-1.1.6/PKG-INFO
```

### Comparing `web_ext_helper-1.1.5/LICENSE` & `web_ext_helper-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.1.5/pyproject.toml` & `web_ext_helper-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web-ext-helper"
-version = "1.1.5"
+version = "1.1.6"
 description = "A simple cli tool that helps you building your web extensions."
 authors = ["AppSolves <appsolves@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "web_ext_helper"}]
 
 [tool.poetry.dependencies]
```

### Comparing `web_ext_helper-1.1.5/README.md` & `web_ext_helper-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.1.5/web_ext_helper/functions.py` & `web_ext_helper-1.1.6/web_ext_helper/functions.py`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.1.5/web_ext_helper/web_ext_helper.py` & `web_ext_helper-1.1.6/web_ext_helper/web_ext_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__ext_version__ = "1.1.5"
+__ext_version__ = "1.1.6"
 
 import os
 import json
 import shutil
 import typer
 import zipfile
 import rich.progress
@@ -522,14 +522,16 @@
 
         with open("src/manifest.json", "w") as manifest_file:
             json.dump(manifest, manifest_file, indent=2)
 
         with open("src/background.js", "w") as background_file:
             background_file.write("")
 
-        typer.echo(f"{bcolors.OKGREEN}Created src/manifest.json{bcolors.ENDC}")
+        typer.echo(
+            f"{bcolors.OKGREEN}Created {bcolors.OKCYAN}src/manifest.json{bcolors.ENDC}"
+        )
 
     ask_for_input(False, None, None, None, None, None, None, None, None)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `web_ext_helper-1.1.5/PKG-INFO` & `web_ext_helper-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ext-helper
-Version: 1.1.5
+Version: 1.1.6
 Summary: A simple cli tool that helps you building your web extensions.
 License: GPL-3.0-or-later
 Author: AppSolves
 Author-email: appsolves@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

