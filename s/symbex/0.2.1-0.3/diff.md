# Comparing `tmp/symbex-0.2.1.tar.gz` & `tmp/symbex-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbex-0.2.1.tar", last modified: Mon Jun 19 08:04:12 2023, max compression
+gzip compressed data, was "symbex-0.3.tar", last modified: Mon Jun 19 14:01:34 2023, max compression
```

## Comparing `symbex-0.2.1.tar` & `symbex-0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:04:12.887510 symbex-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 08:03:56.000000 symbex-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-06-19 08:04:12.887510 symbex-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-19 08:03:56.000000 symbex-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 08:04:12.887510 symbex-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-19 08:03:56.000000 symbex-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:04:12.883510 symbex-0.2.1/symbex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:03:56.000000 symbex-0.2.1/symbex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-19 08:03:56.000000 symbex-0.2.1/symbex/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-19 08:03:56.000000 symbex-0.2.1/symbex/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-19 08:03:56.000000 symbex-0.2.1/symbex/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:04:12.883510 symbex-0.2.1/symbex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-06-19 08:04:12.000000 symbex-0.2.1/symbex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-19 08:04:12.000000 symbex-0.2.1/symbex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:04:12.000000 symbex-0.2.1/symbex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 08:04:12.000000 symbex-0.2.1/symbex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-19 08:04:12.000000 symbex-0.2.1/symbex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 08:04:12.000000 symbex-0.2.1/symbex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:04:12.883510 symbex-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-19 08:03:56.000000 symbex-0.2.1/tests/test_symbex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:01:34.079884 symbex-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 14:01:19.000000 symbex-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-06-19 14:01:34.079884 symbex-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-06-19 14:01:19.000000 symbex-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 14:01:34.079884 symbex-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-19 14:01:19.000000 symbex-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:01:34.075884 symbex-0.3/symbex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:01:19.000000 symbex-0.3/symbex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-19 14:01:19.000000 symbex-0.3/symbex/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-19 14:01:19.000000 symbex-0.3/symbex/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-06-19 14:01:19.000000 symbex-0.3/symbex/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:01:34.075884 symbex-0.3/symbex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-06-19 14:01:34.000000 symbex-0.3/symbex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-19 14:01:34.000000 symbex-0.3/symbex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 14:01:34.000000 symbex-0.3/symbex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 14:01:34.000000 symbex-0.3/symbex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 14:01:34.000000 symbex-0.3/symbex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 14:01:34.000000 symbex-0.3/symbex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:01:34.079884 symbex-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-06-19 14:01:19.000000 symbex-0.3/tests/test_symbex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-19 14:01:19.000000 symbex-0.3/tests/test_symbols.py
```

### Comparing `symbex-0.2.1/LICENSE` & `symbex-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `symbex-0.2.1/README.md` & `symbex-0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -26,14 +26,28 @@
 ```bash
 symbex my_function MyClass
 ```
 Wildcards are supported - to search for every `test_` function run this (note the single quotes to avoid the shell interpreting the `*` as a wildcard):
 ```bash
 symbex 'test_*'
 ```
+To search for methods within classes, use `class.method` notation:
+```bash
+symbex Entry.get_absolute_url
+```
+Wildcards are supported here as well:
+```bash
+symbex 'Entry.*'
+symbex '*.get_absolute_url'
+symbex '*.get_*'
+```
+Or to view every method of every class:
+```bash
+symbex '*.*'
+```
 To search within a specific file, pass that file using the `-f` option. You can pass this more than once to search multiple files.
 
 ```bash
 symbex MyClass -f my_file.py
 ```
 To search within a specific directory and all of its subdirectories, use the `-d` option:
 ```bash
@@ -43,16 +57,15 @@
 ```
 # Syntax error in path/badcode.py: expected ':' (<unknown>, line 1)
 ```
 Pass `--silent` to suppress these warnings:
 ```bash
 symbex MyClass --silent
 ```
-
-## Example output
+### Example output
 
 In a fresh checkout of [Datasette](https://github.com/simonw/datasette) I ran this command:
 
 ```bash
 symbex MessagesDebugView get_long_description
 ```
 Here's the output of the command:
@@ -73,14 +86,58 @@
             await datasette.render_template(
                 "patterns.html",
                 request=request,
                 view_name="patterns",
             )
         )
 ```
+### Just the signatures
+
+The `-s/--signatures` option will list just the signatures of the functions and classes, for example:
+```bash
+symbex -s -d symbex
+```
+
+<!-- [[[cog
+import cog
+from click.testing import CliRunner
+import pathlib
+from symbex.cli import cli
+
+path = pathlib.Path("symbex").resolve()
+runner = CliRunner()
+result = runner.invoke(cli, ["-s", "-d", str(path)])
+# Need a consistent sort order
+chunks = result.stdout.strip().split("\n\n")
+chunks.sort()
+cog.out(
+    "```\n{}\n```\n".format("\n\n".join(chunks))
+)
+]]] -->
+```
+# File: symbex/cli.py Line: 37
+def cli(symbols, files, directories, signatures, silent)
+
+# File: symbex/lib.py Line: 150
+def class_definition(class_def)
+
+# File: symbex/lib.py Line: 32
+def code_for_node(code: str, node: AST, class_name: str, signatures: bool)
+
+# File: symbex/lib.py Line: 63
+def match(name: str, symbols) -> bool
+
+# File: symbex/lib.py Line: 8
+def find_symbol_nodes(code: str, symbols)
+
+# File: symbex/lib.py Line: 88
+def function_definition(function_node: AST)
+```
+<!-- [[[end]]] -->
+This can be combined with other options, or you can run `symbex -s` to see every symbol in the current directory and its subdirectories.
 
 ## Using with LLM
 
 This tool is primarily designed to be used with [LLM](https://llm.datasette.io/), a CLI tool for working with Large Language Models.
 
 `symbex` makes it easy to grab a specific class or function and pass it to the `llm` command.
```

### Comparing `symbex-0.2.1/setup.py` & `symbex-0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.2.1"
+VERSION = "0.3"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -28,10 +28,10 @@
     version=VERSION,
     packages=["symbex"],
     entry_points="""
         [console_scripts]
         symbex=symbex.cli:cli
     """,
     install_requires=["click"],
-    extras_require={"test": ["pytest", "pytest-icdiff"]},
+    extras_require={"test": ["pytest", "pytest-icdiff", "cogapp"]},
     python_requires=">=3.8",
 )
```

### Comparing `symbex-0.2.1/symbex/cli.py` & `symbex-0.3/symbex/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,56 +20,84 @@
     "-d",
     "--directory",
     type=click.Path(file_okay=False, dir_okay=True, resolve_path=True),
     multiple=True,
     help="Directories to search",
 )
 @click.option(
+    "-s",
+    "--signatures",
+    is_flag=True,
+    help="Show just function and class signatures",
+)
+@click.option(
     "--silent",
     is_flag=True,
     help="Silently ignore Python files with parse errors",
 )
-def cli(symbols, files, directories, silent):
+def cli(symbols, files, directories, signatures, silent):
     """
     Find symbols in Python code and print the code for them.
 
     Example usage:
 
     \b
         # Search current directory and subdirectories
         symbex my_function MyClass
     \b
         # Search using a wildcard
         symbex 'test_*'
+
+    \b
+        # Find a specific class method
+        symbex 'MyClass.my_method'
+
+    \b
+        # Find class methods using wildcards
+        symbex '*View.handle_*'
+
     \b
         # Search a specific file
         symbex MyClass -f my_file.py
     \b
         # Search within a specific directory and its subdirectories
         symbex Database -d ~/projects/datasette
 
+    \b
+        # View signatures for all symbols in current directory and subdirectories
+        symbex -s
+
+    \b
+        # View signatures for all test functions
+        symbex 'test_*' -s
     """
+    if signatures and not symbols:
+        symbols = ["*"]
     if not files and not directories:
         directories = ["."]
     files = [pathlib.Path(f) for f in files]
     for directory in directories:
         files.extend(pathlib.Path(directory).rglob("*.py"))
     pwd = pathlib.Path(".").resolve()
     for file in files:
         code = file.read_text("utf-8") if hasattr(file, "read_text") else file.read()
         try:
             nodes = find_symbol_nodes(code, symbols)
         except SyntaxError as ex:
             if not silent:
                 click.secho(f"# Syntax error in {file}: {ex}", err=True, fg="yellow")
             continue
-        for node in nodes:
+        for node, class_name in nodes:
             # If file is within pwd, print relative path
             # else print absolute path
             if pwd in file.resolve().parents:
                 path = file.resolve().relative_to(pwd)
             else:
                 path = file.resolve()
-            snippet, line_no = code_for_node(code, node)
-            print("# File:", path, "Line:", line_no)
+            snippet, line_no = code_for_node(code, node, class_name, signatures)
+            bits = ["# File:", path]
+            if class_name:
+                bits.extend(["Class:", class_name])
+            bits.extend(["Line:", line_no])
+            print(*bits)
             print(snippet)
             print()
```

