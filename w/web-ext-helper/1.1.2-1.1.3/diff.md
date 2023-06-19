# Comparing `tmp/web_ext_helper-1.1.2.tar.gz` & `tmp/web_ext_helper-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_ext_helper-1.1.2.tar", max compression
+gzip compressed data, was "web_ext_helper-1.1.3.tar", max compression
```

## Comparing `web_ext_helper-1.1.2.tar` & `web_ext_helper-1.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.1.2/LICENSE
--rw-r--r--   0        0        0      654 2023-06-19 16:47:38.633075 web_ext_helper-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1754 2023-06-17 20:34:00.666577 web_ext_helper-1.1.2/README.md
--rw-r--r--   0        0        0      262 2023-06-18 17:57:02.181036 web_ext_helper-1.1.2/web_ext_helper/classes.py
--rw-r--r--   0        0        0      613 2023-06-18 17:49:15.766872 web_ext_helper-1.1.2/web_ext_helper/functions.py
--rw-r--r--   0        0        0    18980 2023-06-19 16:48:12.024304 web_ext_helper-1.1.2/web_ext_helper/web_ext_helper.py
--rw-r--r--   0        0        0     2325 1970-01-01 00:00:00.000000 web_ext_helper-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.1.3/LICENSE
+-rw-r--r--   0        0        0      654 2023-06-19 16:49:56.278302 web_ext_helper-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1754 2023-06-17 20:34:00.666577 web_ext_helper-1.1.3/README.md
+-rw-r--r--   0        0        0      262 2023-06-18 17:57:02.181036 web_ext_helper-1.1.3/web_ext_helper/classes.py
+-rw-r--r--   0        0        0      613 2023-06-18 17:49:15.766872 web_ext_helper-1.1.3/web_ext_helper/functions.py
+-rw-r--r--   0        0        0    18433 2023-06-19 16:49:48.739408 web_ext_helper-1.1.3/web_ext_helper/web_ext_helper.py
+-rw-r--r--   0        0        0     2325 1970-01-01 00:00:00.000000 web_ext_helper-1.1.3/PKG-INFO
```

### Comparing `web_ext_helper-1.1.2/LICENSE` & `web_ext_helper-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.1.2/pyproject.toml` & `web_ext_helper-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web-ext-helper"
-version = "1.1.2"
+version = "1.1.3"
 description = "A simple cli tool that helps you building your web extensions."
 authors = ["AppSolves <appsolves@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "web_ext_helper"}]
 
 [tool.poetry.dependencies]
```

### Comparing `web_ext_helper-1.1.2/README.md` & `web_ext_helper-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.1.2/web_ext_helper/functions.py` & `web_ext_helper-1.1.3/web_ext_helper/functions.py`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.1.2/web_ext_helper/web_ext_helper.py` & `web_ext_helper-1.1.3/web_ext_helper/web_ext_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__ext_version__ = "1.1.2"
+__ext_version__ = "1.1.3"
 
 import os
 import json
 import shutil
 import typer
 import zipfile
 import rich.progress
@@ -47,33 +47,14 @@
 @app.command(help="Show the version of the extension", name="version")
 def __version__():
     typer.echo(
         f"{bcolors.OKGREEN}Current {bcolors.OKCYAN}web-ext-helper{bcolors.OKGREEN} version: {bcolors.PURPLE}{__ext_version__}{bcolors.ENDC}"
     )
 
 
-@app.command(help="Update the extension", name="update")
-def __update__():
-    typer.echo(
-        f"{bcolors.OKGREEN}Updating {bcolors.OKCYAN}web-ext-helper{bcolors.OKGREEN}...{bcolors.ENDC}"
-    )
-    try:
-        sp.Popen(
-            [
-                "pip",
-                "install",
-                "web-ext-helper",
-                "--upgrade",
-            ],
-        )
-    except sp.CalledProcessError as e:
-        typer.echo(f"{bcolors.FAIL}{e.stderr.decode()}{bcolors.ENDC}", err=True)
-        raise typer.Exit(1)
-
-
 @app.command(help="Build the extension from the files in the src folder", name="build")
 def __build__(
     compress: bool = typer.Option(
         True, "--compress", "-co", help="Compress the output"
     ),
     clean: bool = typer.Option(False, "--clean", "-cl", help="Clean the build folder"),
 ):
```

### Comparing `web_ext_helper-1.1.2/PKG-INFO` & `web_ext_helper-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ext-helper
-Version: 1.1.2
+Version: 1.1.3
 Summary: A simple cli tool that helps you building your web extensions.
 License: GPL-3.0-or-later
 Author: AppSolves
 Author-email: appsolves@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

