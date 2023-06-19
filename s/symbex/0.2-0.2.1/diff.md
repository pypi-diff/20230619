# Comparing `tmp/symbex-0.2.tar.gz` & `tmp/symbex-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbex-0.2.tar", last modified: Sun Jun 18 21:21:46 2023, max compression
+gzip compressed data, was "symbex-0.2.1.tar", last modified: Mon Jun 19 08:04:12 2023, max compression
```

## Comparing `symbex-0.2.tar` & `symbex-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:21:46.505070 symbex-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-18 21:21:31.000000 symbex-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-18 21:21:46.505070 symbex-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-18 21:21:31.000000 symbex-0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 21:21:46.505070 symbex-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-18 21:21:31.000000 symbex-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:21:46.505070 symbex-0.2/symbex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:21:31.000000 symbex-0.2/symbex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 21:21:31.000000 symbex-0.2/symbex/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-18 21:21:31.000000 symbex-0.2/symbex/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-18 21:21:31.000000 symbex-0.2/symbex/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:21:46.505070 symbex-0.2/symbex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-18 21:21:46.000000 symbex-0.2/symbex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-18 21:21:46.000000 symbex-0.2/symbex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 21:21:46.000000 symbex-0.2/symbex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-18 21:21:46.000000 symbex-0.2/symbex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-18 21:21:46.000000 symbex-0.2/symbex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-18 21:21:46.000000 symbex-0.2/symbex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:21:46.505070 symbex-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-18 21:21:31.000000 symbex-0.2/tests/test_symbex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:04:12.887510 symbex-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 08:03:56.000000 symbex-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-06-19 08:04:12.887510 symbex-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-19 08:03:56.000000 symbex-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 08:04:12.887510 symbex-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-19 08:03:56.000000 symbex-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:04:12.883510 symbex-0.2.1/symbex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:03:56.000000 symbex-0.2.1/symbex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-19 08:03:56.000000 symbex-0.2.1/symbex/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-19 08:03:56.000000 symbex-0.2.1/symbex/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-19 08:03:56.000000 symbex-0.2.1/symbex/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:04:12.883510 symbex-0.2.1/symbex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-06-19 08:04:12.000000 symbex-0.2.1/symbex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-19 08:04:12.000000 symbex-0.2.1/symbex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:04:12.000000 symbex-0.2.1/symbex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 08:04:12.000000 symbex-0.2.1/symbex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-19 08:04:12.000000 symbex-0.2.1/symbex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 08:04:12.000000 symbex-0.2.1/symbex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:04:12.883510 symbex-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-19 08:03:56.000000 symbex-0.2.1/tests/test_symbex.py
```

### Comparing `symbex-0.2/LICENSE` & `symbex-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `symbex-0.2/PKG-INFO` & `symbex-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbex
-Version: 0.2
+Version: 0.2.1
 Summary: Find the Python code for specified symbols
 Home-page: https://github.com/simonw/symbex
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/symbex/issues
 Project-URL: CI, https://github.com/simonw/symbex/actions
 Project-URL: Changelog, https://github.com/simonw/symbex/releases
@@ -50,14 +50,22 @@
 ```bash
 symbex MyClass -f my_file.py
 ```
 To search within a specific directory and all of its subdirectories, use the `-d` option:
 ```bash
 symbex Database -d ~/projects/datasette
 ```
+If `symbex` encounters any Python code that it cannot parse, it will print a warning message and continue searching:
+```
+# Syntax error in path/badcode.py: expected ':' (<unknown>, line 1)
+```
+Pass `--silent` to suppress these warnings:
+```bash
+symbex MyClass --silent
+```
 
 ## Example output
 
 In a fresh checkout of [Datasette](https://github.com/simonw/datasette) I ran this command:
 
 ```bash
 symbex MessagesDebugView get_long_description
```

### Comparing `symbex-0.2/README.md` & `symbex-0.2.1/symbex.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: symbex
+Version: 0.2.1
+Summary: Find the Python code for specified symbols
+Home-page: https://github.com/simonw/symbex
+Author: Simon Willison
+License: Apache License, Version 2.0
+Project-URL: Issues, https://github.com/simonw/symbex/issues
+Project-URL: CI, https://github.com/simonw/symbex/actions
+Project-URL: Changelog, https://github.com/simonw/symbex/releases
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # symbex
 
 [![PyPI](https://img.shields.io/pypi/v/symbex.svg)](https://pypi.org/project/symbex/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/symbex?include_prereleases&label=changelog)](https://github.com/simonw/symbex/releases)
 [![Tests](https://github.com/simonw/symbex/workflows/Test/badge.svg)](https://github.com/simonw/symbex/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/symbex/blob/master/LICENSE)
 
@@ -35,14 +50,22 @@
 ```bash
 symbex MyClass -f my_file.py
 ```
 To search within a specific directory and all of its subdirectories, use the `-d` option:
 ```bash
 symbex Database -d ~/projects/datasette
 ```
+If `symbex` encounters any Python code that it cannot parse, it will print a warning message and continue searching:
+```
+# Syntax error in path/badcode.py: expected ':' (<unknown>, line 1)
+```
+Pass `--silent` to suppress these warnings:
+```bash
+symbex MyClass --silent
+```
 
 ## Example output
 
 In a fresh checkout of [Datasette](https://github.com/simonw/datasette) I ran this command:
 
 ```bash
 symbex MessagesDebugView get_long_description
```

### Comparing `symbex-0.2/setup.py` & `symbex-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.2"
+VERSION = "0.2.1"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `symbex-0.2/symbex/cli.py` & `symbex-0.2.1/symbex/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,25 +4,35 @@
 from .lib import code_for_node, find_symbol_nodes
 
 
 @click.command()
 @click.version_option()
 @click.argument("symbols", nargs=-1)
 @click.option(
-    "files", "-f", "--file", type=click.File("r"), multiple=True, help="Files to search"
+    "files",
+    "-f",
+    "--file",
+    type=click.Path(file_okay=True, dir_okay=False),
+    multiple=True,
+    help="Files to search",
 )
 @click.option(
     "directories",
     "-d",
     "--directory",
     type=click.Path(file_okay=False, dir_okay=True, resolve_path=True),
     multiple=True,
     help="Directories to search",
 )
-def cli(symbols, files, directories):
+@click.option(
+    "--silent",
+    is_flag=True,
+    help="Silently ignore Python files with parse errors",
+)
+def cli(symbols, files, directories, silent):
     """
     Find symbols in Python code and print the code for them.
 
     Example usage:
 
     \b
         # Search current directory and subdirectories
@@ -36,21 +46,26 @@
     \b
         # Search within a specific directory and its subdirectories
         symbex Database -d ~/projects/datasette
 
     """
     if not files and not directories:
         directories = ["."]
-    files = list(files)
+    files = [pathlib.Path(f) for f in files]
     for directory in directories:
         files.extend(pathlib.Path(directory).rglob("*.py"))
     pwd = pathlib.Path(".").resolve()
     for file in files:
         code = file.read_text("utf-8") if hasattr(file, "read_text") else file.read()
-        nodes = find_symbol_nodes(code, symbols)
+        try:
+            nodes = find_symbol_nodes(code, symbols)
+        except SyntaxError as ex:
+            if not silent:
+                click.secho(f"# Syntax error in {file}: {ex}", err=True, fg="yellow")
+            continue
         for node in nodes:
             # If file is within pwd, print relative path
             # else print absolute path
             if pwd in file.resolve().parents:
                 path = file.resolve().relative_to(pwd)
             else:
                 path = file.resolve()
```

### Comparing `symbex-0.2/symbex/lib.py` & `symbex-0.2.1/symbex/lib.py`

 * *Files identical despite different names*

### Comparing `symbex-0.2/symbex.egg-info/PKG-INFO` & `symbex-0.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: symbex
-Version: 0.2
-Summary: Find the Python code for specified symbols
-Home-page: https://github.com/simonw/symbex
-Author: Simon Willison
-License: Apache License, Version 2.0
-Project-URL: Issues, https://github.com/simonw/symbex/issues
-Project-URL: CI, https://github.com/simonw/symbex/actions
-Project-URL: Changelog, https://github.com/simonw/symbex/releases
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # symbex
 
 [![PyPI](https://img.shields.io/pypi/v/symbex.svg)](https://pypi.org/project/symbex/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/symbex?include_prereleases&label=changelog)](https://github.com/simonw/symbex/releases)
 [![Tests](https://github.com/simonw/symbex/workflows/Test/badge.svg)](https://github.com/simonw/symbex/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/symbex/blob/master/LICENSE)
 
@@ -50,14 +35,22 @@
 ```bash
 symbex MyClass -f my_file.py
 ```
 To search within a specific directory and all of its subdirectories, use the `-d` option:
 ```bash
 symbex Database -d ~/projects/datasette
 ```
+If `symbex` encounters any Python code that it cannot parse, it will print a warning message and continue searching:
+```
+# Syntax error in path/badcode.py: expected ':' (<unknown>, line 1)
+```
+Pass `--silent` to suppress these warnings:
+```bash
+symbex MyClass --silent
+```
 
 ## Example output
 
 In a fresh checkout of [Datasette](https://github.com/simonw/datasette) I ran this command:
 
 ```bash
 symbex MessagesDebugView get_long_description
```

