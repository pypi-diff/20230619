# Comparing `tmp/web_ext_helper-1.0.8.tar.gz` & `tmp/web_ext_helper-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_ext_helper-1.0.8.tar", max compression
+gzip compressed data, was "web_ext_helper-1.0.9.tar", max compression
```

## Comparing `web_ext_helper-1.0.8.tar` & `web_ext_helper-1.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.0.8/LICENSE
--rw-r--r--   0        0        0      654 2023-06-19 16:21:17.751282 web_ext_helper-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     1754 2023-06-17 20:34:00.666577 web_ext_helper-1.0.8/README.md
--rw-r--r--   0        0        0      262 2023-06-18 17:57:02.181036 web_ext_helper-1.0.8/web_ext_helper/classes.py
--rw-r--r--   0        0        0      613 2023-06-18 17:49:15.766872 web_ext_helper-1.0.8/web_ext_helper/functions.py
--rw-r--r--   0        0        0    18142 2023-06-19 16:21:10.777540 web_ext_helper-1.0.8/web_ext_helper/web_ext_helper.py
--rw-r--r--   0        0        0     2325 1970-01-01 00:00:00.000000 web_ext_helper-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.0.9/LICENSE
+-rw-r--r--   0        0        0      654 2023-06-19 16:37:34.325806 web_ext_helper-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1754 2023-06-17 20:34:00.666577 web_ext_helper-1.0.9/README.md
+-rw-r--r--   0        0        0      262 2023-06-18 17:57:02.181036 web_ext_helper-1.0.9/web_ext_helper/classes.py
+-rw-r--r--   0        0        0      613 2023-06-18 17:49:15.766872 web_ext_helper-1.0.9/web_ext_helper/functions.py
+-rw-r--r--   0        0        0    18920 2023-06-19 16:42:37.757384 web_ext_helper-1.0.9/web_ext_helper/web_ext_helper.py
+-rw-r--r--   0        0        0     2325 1970-01-01 00:00:00.000000 web_ext_helper-1.0.9/PKG-INFO
```

### Comparing `web_ext_helper-1.0.8/LICENSE` & `web_ext_helper-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.0.8/pyproject.toml` & `web_ext_helper-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web-ext-helper"
-version = "1.0.8"
+version = "1.0.9"
 description = "A simple cli tool that helps you building your web extensions."
 authors = ["AppSolves <appsolves@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "web_ext_helper"}]
 
 [tool.poetry.dependencies]
```

### Comparing `web_ext_helper-1.0.8/README.md` & `web_ext_helper-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.0.8/web_ext_helper/functions.py` & `web_ext_helper-1.0.9/web_ext_helper/functions.py`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.0.8/web_ext_helper/web_ext_helper.py` & `web_ext_helper-1.0.9/web_ext_helper/web_ext_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__ext_version__ = "1.0.9"
+
 import os
 import json
 import shutil
 import typer
 import zipfile
 import rich.progress
 import requests as req
@@ -38,14 +40,39 @@
     manifest_name_lower = manifest_data["name"].lower()
     manifest_version = manifest_data["version"]
 except FileNotFoundError:
     manifest_name_lower = None
     manifest_version = None
 
 
+@app.command(help="Show the version of the extension", name="version")
+def __version__():
+    typer.echo(
+        f"{bcolors.OKCYAN}Current web-ext-helper version: {bcolors.OKGREEN}{__ext_version__}{bcolors.ENDC}"
+    )
+
+
+@app.command(help="Update the extension", name="update")
+def __update__():
+    typer.echo(f"{bcolors.OKCYAN}Updating web-ext-helper...{bcolors.ENDC}")
+    try:
+        sp.run(
+            [
+                "pip",
+                "install",
+                "web-ext-helper",
+                "--upgrade",
+            ],
+            check=True,
+        )
+    except sp.CalledProcessError as e:
+        typer.echo(f"{bcolors.FAIL}{e.stderr.decode()}{bcolors.ENDC}", err=True)
+        raise typer.Exit(1)
+
+
 @app.command(help="Build the extension from the files in the src folder", name="build")
 def __build__(
     compress: bool = typer.Option(
         True, "--compress", "-co", help="Compress the output"
     ),
     clean: bool = typer.Option(False, "--clean", "-cl", help="Clean the build folder"),
 ):
```

### Comparing `web_ext_helper-1.0.8/PKG-INFO` & `web_ext_helper-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ext-helper
-Version: 1.0.8
+Version: 1.0.9
 Summary: A simple cli tool that helps you building your web extensions.
 License: GPL-3.0-or-later
 Author: AppSolves
 Author-email: appsolves@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

