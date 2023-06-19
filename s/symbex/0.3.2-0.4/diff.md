# Comparing `tmp/symbex-0.3.2.tar.gz` & `tmp/symbex-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbex-0.3.2.tar", last modified: Mon Jun 19 15:52:56 2023, max compression
+gzip compressed data, was "symbex-0.4.tar", last modified: Mon Jun 19 18:08:06 2023, max compression
```

## Comparing `symbex-0.3.2.tar` & `symbex-0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:56.290764 symbex-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 15:52:39.000000 symbex-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-19 15:52:56.286764 symbex-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-06-19 15:52:39.000000 symbex-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 15:52:56.290764 symbex-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-19 15:52:39.000000 symbex-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:56.286764 symbex-0.3.2/symbex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:39.000000 symbex-0.3.2/symbex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-19 15:52:39.000000 symbex-0.3.2/symbex/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-19 15:52:39.000000 symbex-0.3.2/symbex/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-06-19 15:52:39.000000 symbex-0.3.2/symbex/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:56.286764 symbex-0.3.2/symbex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-19 15:52:56.000000 symbex-0.3.2/symbex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-19 15:52:56.000000 symbex-0.3.2/symbex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:52:56.000000 symbex-0.3.2/symbex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 15:52:56.000000 symbex-0.3.2/symbex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 15:52:56.000000 symbex-0.3.2/symbex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 15:52:56.000000 symbex-0.3.2/symbex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:56.286764 symbex-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-19 15:52:39.000000 symbex-0.3.2/tests/test_symbex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-19 15:52:39.000000 symbex-0.3.2/tests/test_symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:08:06.508515 symbex-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 18:07:51.000000 symbex-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-06-19 18:08:06.508515 symbex-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-06-19 18:07:51.000000 symbex-0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 18:08:06.508515 symbex-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-19 18:07:51.000000 symbex-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:08:06.508515 symbex-0.4/symbex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 18:07:51.000000 symbex-0.4/symbex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-19 18:07:51.000000 symbex-0.4/symbex/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-19 18:07:51.000000 symbex-0.4/symbex/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-06-19 18:07:51.000000 symbex-0.4/symbex/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:08:06.508515 symbex-0.4/symbex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-06-19 18:08:06.000000 symbex-0.4/symbex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-19 18:08:06.000000 symbex-0.4/symbex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 18:08:06.000000 symbex-0.4/symbex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 18:08:06.000000 symbex-0.4/symbex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 18:08:06.000000 symbex-0.4/symbex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 18:08:06.000000 symbex-0.4/symbex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:08:06.508515 symbex-0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-19 18:07:51.000000 symbex-0.4/tests/test_symbex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-19 18:07:51.000000 symbex-0.4/tests/test_symbols.py
```

### Comparing `symbex-0.3.2/LICENSE` & `symbex-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `symbex-0.3.2/PKG-INFO` & `symbex-0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: symbex
-Version: 0.3.2
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
 
@@ -128,27 +113,33 @@
     "```\n{}\n```\n".format("\n\n".join(chunks))
 )
 ]]] -->
 ```
 # File: symbex/cli.py Line: 37
 def cli(symbols, files, directories, signatures, silent)
 
-# File: symbex/lib.py Line: 161
+# File: symbex/lib.py Line: 10
+def find_symbol_nodes(code: str, filename: str, symbols: Iterable[str]) -> List[Tuple[(AST, Optional[str])]]
+
+# File: symbex/lib.py Line: 158
 def class_definition(class_def)
 
-# File: symbex/lib.py Line: 32
-def code_for_node(code: str, node: AST, class_name: str, signatures: bool)
+# File: symbex/lib.py Line: 192
+def annotation_definition(annotation: AST) -> str
+
+# File: symbex/lib.py Line: 210
+def read_file(path)
 
-# File: symbex/lib.py Line: 63
-def match(name: str, symbols) -> bool
+# File: symbex/lib.py Line: 34
+def code_for_node(code: str, node: AST, class_name: str, signatures: bool) -> Tuple[(str, int)]
 
-# File: symbex/lib.py Line: 8
-def find_symbol_nodes(code: str, symbols)
+# File: symbex/lib.py Line: 65
+def match(name: str, symbols: Iterable[str]) -> bool
 
-# File: symbex/lib.py Line: 88
+# File: symbex/lib.py Line: 90
 def function_definition(function_node: AST)
 ```
 <!-- [[[end]]] -->
 This can be combined with other options, or you can run `symbex -s` to see every symbol in the current directory and its subdirectories.
 
 ## Using with LLM
 
@@ -161,14 +152,18 @@
 ```bash
 symbex Response | llm --system 'Explain this code, succinctly'
 ```
 And got back this:
 
 > This code defines a custom `Response` class with methods for returning HTTP responses. It includes methods for setting cookies, returning HTML, text, and JSON responses, and redirecting to a different URL. The `asgi_send` method sends the response to the client using the ASGI (Asynchronous Server Gateway Interface) protocol.
 
+## Similar tools
+
+- [pyastgrep](https://github.com/spookylukey/pyastgrep) by Luke Plant offers advanced capabilities for viewing and searching through Python ASTs using XPath.
+- [cq](https://github.com/fullstackio/cq) is a tool thet lets you "extract code snippets using CSS-like selectors", built using [Tree-sitter](https://tree-sitter.github.io/tree-sitter/) and primarily targetting JavaScript and TypeScript.
 
 ## Development
 
 To contribute to this tool, first checkout the code. Then create a new virtual environment:
 ```bash
 cd symbex
 python -m venv venv
@@ -178,7 +173,26 @@
 ```bash
 pip install -e '.[test]'
 ```
 To run the tests:
 ```bash
 pytest
 ```
+### just
+
+You can also install [just](https://github.com/casey/just) and use it to run the tests and linters like this:
+
+```bash
+just
+```
+Or to list commands:
+```bash
+just -l
+```
+```
+Available recipes:
+    black         # Apply Black
+    cog           # Rebuild docs with cog
+    default       # Run tests and linters
+    lint          # Run linters
+    test *options # Run pytest with supplied options
+```
```

### Comparing `symbex-0.3.2/README.md` & `symbex-0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: symbex
+Version: 0.4
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
 
@@ -113,27 +128,33 @@
     "```\n{}\n```\n".format("\n\n".join(chunks))
 )
 ]]] -->
 ```
 # File: symbex/cli.py Line: 37
 def cli(symbols, files, directories, signatures, silent)
 
-# File: symbex/lib.py Line: 161
+# File: symbex/lib.py Line: 10
+def find_symbol_nodes(code: str, filename: str, symbols: Iterable[str]) -> List[Tuple[(AST, Optional[str])]]
+
+# File: symbex/lib.py Line: 158
 def class_definition(class_def)
 
-# File: symbex/lib.py Line: 32
-def code_for_node(code: str, node: AST, class_name: str, signatures: bool)
+# File: symbex/lib.py Line: 192
+def annotation_definition(annotation: AST) -> str
+
+# File: symbex/lib.py Line: 210
+def read_file(path)
 
-# File: symbex/lib.py Line: 63
-def match(name: str, symbols) -> bool
+# File: symbex/lib.py Line: 34
+def code_for_node(code: str, node: AST, class_name: str, signatures: bool) -> Tuple[(str, int)]
 
-# File: symbex/lib.py Line: 8
-def find_symbol_nodes(code: str, symbols)
+# File: symbex/lib.py Line: 65
+def match(name: str, symbols: Iterable[str]) -> bool
 
-# File: symbex/lib.py Line: 88
+# File: symbex/lib.py Line: 90
 def function_definition(function_node: AST)
 ```
 <!-- [[[end]]] -->
 This can be combined with other options, or you can run `symbex -s` to see every symbol in the current directory and its subdirectories.
 
 ## Using with LLM
 
@@ -146,14 +167,18 @@
 ```bash
 symbex Response | llm --system 'Explain this code, succinctly'
 ```
 And got back this:
 
 > This code defines a custom `Response` class with methods for returning HTTP responses. It includes methods for setting cookies, returning HTML, text, and JSON responses, and redirecting to a different URL. The `asgi_send` method sends the response to the client using the ASGI (Asynchronous Server Gateway Interface) protocol.
 
+## Similar tools
+
+- [pyastgrep](https://github.com/spookylukey/pyastgrep) by Luke Plant offers advanced capabilities for viewing and searching through Python ASTs using XPath.
+- [cq](https://github.com/fullstackio/cq) is a tool thet lets you "extract code snippets using CSS-like selectors", built using [Tree-sitter](https://tree-sitter.github.io/tree-sitter/) and primarily targetting JavaScript and TypeScript.
 
 ## Development
 
 To contribute to this tool, first checkout the code. Then create a new virtual environment:
 ```bash
 cd symbex
 python -m venv venv
@@ -163,7 +188,26 @@
 ```bash
 pip install -e '.[test]'
 ```
 To run the tests:
 ```bash
 pytest
 ```
+### just
+
+You can also install [just](https://github.com/casey/just) and use it to run the tests and linters like this:
+
+```bash
+just
+```
+Or to list commands:
+```bash
+just -l
+```
+```
+Available recipes:
+    black         # Apply Black
+    cog           # Rebuild docs with cog
+    default       # Run tests and linters
+    lint          # Run linters
+    test *options # Run pytest with supplied options
+```
```

### Comparing `symbex-0.3.2/setup.py` & `symbex-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.3.2"
+VERSION = "0.4"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `symbex-0.3.2/symbex/cli.py` & `symbex-0.4/symbex/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import click
 import pathlib
 
-from .lib import code_for_node, find_symbol_nodes
+from .lib import code_for_node, find_symbol_nodes, read_file
 
 
 @click.command()
 @click.version_option()
 @click.argument("symbols", nargs=-1)
 @click.option(
     "files",
@@ -66,26 +66,35 @@
         # View signatures for all symbols in current directory and subdirectories
         symbex -s
 
     \b
         # View signatures for all test functions
         symbex 'test_*' -s
     """
+    if not symbols and not signatures:
+        ctx = click.get_current_context()
+        click.echo(ctx.get_help())
+        ctx.exit()
     if signatures and not symbols:
         symbols = ["*"]
     if not files and not directories:
         directories = ["."]
-    files = [pathlib.Path(f) for f in files]
-    for directory in directories:
-        files.extend(pathlib.Path(directory).rglob("*.py"))
+
+    def iterate_files():
+        yield from (pathlib.Path(f) for f in files)
+        for directory in directories:
+            for path in pathlib.Path(directory).rglob("*.py"):
+                if path.is_file():
+                    yield path
+
     pwd = pathlib.Path(".").resolve()
-    for file in files:
-        code = file.read_text("utf-8") if hasattr(file, "read_text") else file.read()
+    for file in iterate_files():
+        code = read_file(file)
         try:
-            nodes = find_symbol_nodes(code, symbols)
+            nodes = find_symbol_nodes(code, str(file), symbols)
         except SyntaxError as ex:
             if not silent:
                 click.secho(f"# Syntax error in {file}: {ex}", err=True, fg="yellow")
             continue
         for node, class_name in nodes:
             # If file is within pwd, print relative path
             # else print absolute path
```

### Comparing `symbex-0.3.2/symbex/lib.py` & `symbex-0.4/symbex/lib.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import fnmatch
+import ast
 from ast import literal_eval, parse, AST, AsyncFunctionDef, FunctionDef, ClassDef
+import codecs
 from itertools import zip_longest
-import textwrap
+import re
 from typing import Iterable, List, Optional, Tuple
 
 
 def find_symbol_nodes(
-    code: str, symbols: Iterable[str]
+    code: str, filename: str, symbols: Iterable[str]
 ) -> List[Tuple[AST, Optional[str]]]:
     "Returns ast Nodes matching symbols"
     # list of (AST, None-or-class-name)
     matches = []
     module = parse(code)
     for node in module.body:
         if not isinstance(node, (ClassDef, FunctionDef, AsyncFunctionDef)):
@@ -121,18 +123,17 @@
     arguments = []
 
     for i, (arg, default) in enumerate(zip_longest(all_args, defaults)):
         if position_of_slash and i == position_of_slash:
             arguments.append("/")
         if position_of_star and i == position_of_star:
             arguments.append("*")
-        if getattr(arg.annotation, "id", None):
-            arg_str = f"{arg.arg}: {arg.annotation.id}"
-        else:
-            arg_str = arg.arg
+        arg_str = arg.arg
+        if arg.annotation:
+            arg_str += f": {annotation_definition(arg.annotation)}"
 
         if default:
             arg_str = f"{arg_str}={default}"
 
         arguments.append(arg_str)
 
     if function_node.args.vararg:
@@ -141,19 +142,15 @@
     if function_node.args.kwarg:
         arguments.append(f"**{function_node.args.kwarg.arg}")
 
     arguments_str = ", ".join(arguments)
 
     return_annotation = ""
     if function_node.returns:
-        if hasattr(function_node.returns, "id"):
-            return_annotation = f" -> {function_node.returns.id}"
-        elif function_node.returns.value is None:
-            # None shows as returns.value is None
-            return_annotation = " -> None"
+        return_annotation = f" -> {annotation_definition(function_node.returns)}"
 
     def_ = "def "
     if isinstance(function_node, AsyncFunctionDef):
         def_ = "async def "
 
     return f"{def_}{function_name}({arguments_str}){return_annotation}"
 
@@ -186,7 +183,50 @@
 
     if signature:
         signature = f"({signature})"
 
     class_definition = f"class {class_def.name}{signature}"
 
     return class_definition
+
+
+def annotation_definition(annotation: AST) -> str:
+    if annotation is None:
+        return ""
+    elif isinstance(annotation, ast.Name):
+        return annotation.id
+    elif isinstance(annotation, ast.Subscript):
+        value = annotation_definition(annotation.value)
+        slice = annotation_definition(annotation.slice)
+        return f"{value}[{slice}]"
+    elif isinstance(annotation, ast.Index):
+        return annotation_definition(annotation.value)
+    elif isinstance(annotation, ast.Tuple):
+        elements = ", ".join(annotation_definition(e) for e in annotation.elts)
+        return f"({elements})"
+    else:
+        return "?"
+
+
+def read_file(path):
+    encoding_pattern = r"^[ \t\f]*#.*?coding[:=][ \t]*([-_.a-zA-Z0-9]+)"
+    default_encoding = "utf-8"
+
+    with open(path, "r", encoding=default_encoding, errors="ignore") as f:
+        first_512_bytes = f.read(512)
+        first_two_lines = "\n".join(first_512_bytes.split("\n")[:2])
+
+        match = re.search(encoding_pattern, first_two_lines, re.MULTILINE)
+        if match:
+            encoding = match.group(1)
+        else:
+            encoding = default_encoding
+
+    try:
+        with codecs.open(path, "r", encoding=encoding) as f:
+            content = f.read()
+    except LookupError:
+        # If the detected encoding is not valid, try again with utf-8
+        with codecs.open(path, "r", encoding=default_encoding) as f:
+            content = f.read()
+
+    return content
```

### Comparing `symbex-0.3.2/symbex.egg-info/PKG-INFO` & `symbex-0.4/symbex.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbex
-Version: 0.3.2
+Version: 0.4
 Summary: Find the Python code for specified symbols
 Home-page: https://github.com/simonw/symbex
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/symbex/issues
 Project-URL: CI, https://github.com/simonw/symbex/actions
 Project-URL: Changelog, https://github.com/simonw/symbex/releases
@@ -128,27 +128,33 @@
     "```\n{}\n```\n".format("\n\n".join(chunks))
 )
 ]]] -->
 ```
 # File: symbex/cli.py Line: 37
 def cli(symbols, files, directories, signatures, silent)
 
-# File: symbex/lib.py Line: 161
+# File: symbex/lib.py Line: 10
+def find_symbol_nodes(code: str, filename: str, symbols: Iterable[str]) -> List[Tuple[(AST, Optional[str])]]
+
+# File: symbex/lib.py Line: 158
 def class_definition(class_def)
 
-# File: symbex/lib.py Line: 32
-def code_for_node(code: str, node: AST, class_name: str, signatures: bool)
+# File: symbex/lib.py Line: 192
+def annotation_definition(annotation: AST) -> str
+
+# File: symbex/lib.py Line: 210
+def read_file(path)
 
-# File: symbex/lib.py Line: 63
-def match(name: str, symbols) -> bool
+# File: symbex/lib.py Line: 34
+def code_for_node(code: str, node: AST, class_name: str, signatures: bool) -> Tuple[(str, int)]
 
-# File: symbex/lib.py Line: 8
-def find_symbol_nodes(code: str, symbols)
+# File: symbex/lib.py Line: 65
+def match(name: str, symbols: Iterable[str]) -> bool
 
-# File: symbex/lib.py Line: 88
+# File: symbex/lib.py Line: 90
 def function_definition(function_node: AST)
 ```
 <!-- [[[end]]] -->
 This can be combined with other options, or you can run `symbex -s` to see every symbol in the current directory and its subdirectories.
 
 ## Using with LLM
 
@@ -161,14 +167,18 @@
 ```bash
 symbex Response | llm --system 'Explain this code, succinctly'
 ```
 And got back this:
 
 > This code defines a custom `Response` class with methods for returning HTTP responses. It includes methods for setting cookies, returning HTML, text, and JSON responses, and redirecting to a different URL. The `asgi_send` method sends the response to the client using the ASGI (Asynchronous Server Gateway Interface) protocol.
 
+## Similar tools
+
+- [pyastgrep](https://github.com/spookylukey/pyastgrep) by Luke Plant offers advanced capabilities for viewing and searching through Python ASTs using XPath.
+- [cq](https://github.com/fullstackio/cq) is a tool thet lets you "extract code snippets using CSS-like selectors", built using [Tree-sitter](https://tree-sitter.github.io/tree-sitter/) and primarily targetting JavaScript and TypeScript.
 
 ## Development
 
 To contribute to this tool, first checkout the code. Then create a new virtual environment:
 ```bash
 cd symbex
 python -m venv venv
@@ -178,7 +188,26 @@
 ```bash
 pip install -e '.[test]'
 ```
 To run the tests:
 ```bash
 pytest
 ```
+### just
+
+You can also install [just](https://github.com/casey/just) and use it to run the tests and linters like this:
+
+```bash
+just
+```
+Or to list commands:
+```bash
+just -l
+```
+```
+Available recipes:
+    black         # Apply Black
+    cog           # Rebuild docs with cog
+    default       # Run tests and linters
+    lint          # Run linters
+    test *options # Run pytest with supplied options
+```
```

### Comparing `symbex-0.3.2/tests/test_symbex.py` & `symbex-0.4/tests/test_symbex.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 import pathlib
 import pytest
 import textwrap
 from click.testing import CliRunner
 
 from symbex.cli import cli
+from symbex.lib import read_file
+
+
+def test_no_args_shows_help():
+    runner = CliRunner()
+    result = runner.invoke(cli, catch_exceptions=False)
+    assert result.exit_code == 0
+    assert "Usage: cli [OPTIONS]" in result.stdout
 
 
 @pytest.fixture
 def directory_full_of_code(tmpdir):
     for path, content in (
         ("foo.py", "def foo1():\n    pass\n\n@decorated\ndef foo2():\n    pass\n\n"),
         ("bar.py", "class BarClass:\n    pass\n\n"),
-        ("nested/baz.py", 'def baz(delimiter=", ", type=str):\n    pass\n\n'),
-        ("nested/error.py", "def baz_error()" + "bug:\n    pass\n\n"),
+        ("nested.py/baz.py", 'def baz(delimiter=", ", type=str):\n    pass\n\n'),
+        ("nested.py/error.py", "def baz_error()" + "bug:\n    pass\n\n"),
         (
             "methods.py",
             textwrap.dedent(
                 """
         class MyClass:
             def __init__(self, a):
                 self.a = a
@@ -56,29 +64,29 @@
         ),
         (
             ["BarClass", "--silent"],
             "# File: bar.py Line: 1\nclass BarClass:\n    pass\n\n",
         ),
         (
             ["baz", "--silent"],
-            '# File: nested/baz.py Line: 1\ndef baz(delimiter=", ", type=str):\n    pass\n\n',
+            '# File: nested.py/baz.py Line: 1\ndef baz(delimiter=", ", type=str):\n    pass\n\n',
         ),
         (
             ["async_func", "--silent"],
             "# File: async.py Line: 1\nasync def async_func(a, b, c):\n    pass\n\n",
         ),
         # The -f option
         (
-            ["baz", "-f", "nested/baz.py", "--silent"],
-            '# File: nested/baz.py Line: 1\ndef baz(delimiter=", ", type=str):\n    pass\n\n',
+            ["baz", "-f", "nested.py/baz.py", "--silent"],
+            '# File: nested.py/baz.py Line: 1\ndef baz(delimiter=", ", type=str):\n    pass\n\n',
         ),
         # The -d option
         (
-            ["baz", "-d", "nested", "--silent"],
-            '# File: nested/baz.py Line: 1\ndef baz(delimiter=", ", type=str):\n    pass\n\n',
+            ["baz", "-d", "nested.py", "--silent"],
+            '# File: nested.py/baz.py Line: 1\ndef baz(delimiter=", ", type=str):\n    pass\n\n',
         ),
         # Classes
         (
             ["MyClass", "--silent"],
             "# File: methods.py Line: 2\n"
             "class MyClass:\n"
             "    def __init__(self, a):\n"
@@ -142,15 +150,15 @@
             "\n"
             "# File: foo.py Line: 5\n"
             "def foo2()",
         ),
         (["BarClass", "--silent"], "# File: bar.py Line: 1\n" "class BarClass"),
         (
             ["baz", "--silent"],
-            ("# File: nested/baz.py Line: 1\n" 'def baz(delimiter=", ", type=str)'),
+            ("# File: nested.py/baz.py Line: 1\n" 'def baz(delimiter=", ", type=str)'),
         ),
     ),
 )
 def test_symbex_symbols(directory_full_of_code, monkeypatch, args, expected):
     runner = CliRunner()
     monkeypatch.chdir(directory_full_of_code)
     result = runner.invoke(cli, args + ["-s"], catch_exceptions=False)
@@ -162,14 +170,31 @@
 def test_errors(directory_full_of_code, monkeypatch):
     # Test without --silent to see errors
     runner = CliRunner(mix_stderr=False)
     monkeypatch.chdir(directory_full_of_code)
     result = runner.invoke(cli, ["baz"], catch_exceptions=False)
     assert result.exit_code == 0
     expected = (
-        "# File: nested/baz.py Line: 1\n"
+        "# File: nested.py/baz.py Line: 1\n"
         'def baz(delimiter=", ", type=str):\n'
         "    pass\n\n"
     )
     assert result.stdout == expected
     # This differs between different Python versions
-    assert result.stderr.startswith("# Syntax error in nested/error.py:")
+    assert result.stderr.startswith("# Syntax error in nested.py/error.py:")
+
+
+def test_read_file_with_encoding(tmpdir):
+    # https://github.com/simonw/symbex/issues/18#issuecomment-1597546242
+    path = tmpdir / "encoded.py"
+    path.write_binary(
+        b"# coding: iso-8859-5\n# (Unlikely to be the default encoding for most testers.)\n"
+        b"# \xb1\xb6\xff\xe0\xe1\xe2\xe3\xe4\xe5\xe6\xe7\xe8\xe9\xea\xeb\xec\xed\xee\xef <- Cyrillic characters\n"
+        b'u = "\xae\xe2\xf0\xc4"\n'
+    )
+    text = read_file(path)
+    assert text == (
+        "# coding: iso-8859-5\n"
+        "# (Unlikely to be the default encoding for most testers.)\n"
+        "# БЖџрстуфхцчшщъыьэюя <- Cyrillic characters\n"
+        'u = "Ўт№Ф"\n'
+    )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `symbex-0.3.2/tests/test_symbols.py` & `symbex-0.4/tests/test_symbols.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,14 +28,22 @@
         ("func_positional_only_args", "def func_positional_only_args(a, /, b, c)"),
         ("func_keyword_only_args", "def func_keyword_only_args(a, *, b, c)"),
         ("func_type_annotations", "def func_type_annotations(a: int, b: str) -> bool"),
         ("ClassNoBase", "class ClassNoBase"),
         ("ClassSingleBase", "class ClassSingleBase(int)"),
         ("ClassMultipleBase", "class ClassMultipleBase(int, str)"),
         ("ClassWithMeta", "class ClassWithMeta(metaclass=type)"),
+        (
+            "function_with_non_pep_0484_annotation",
+            "def function_with_non_pep_0484_annotation(x: ?, xx: ?, yy: ?, y: ?, zz: float) -> ?",
+        ),
+        (
+            "complex_annotations",
+            "complex_annotations(code: str, symbols: Iterable[str]) -> List[Tuple[(AST, Optional[str])]]",
+        ),
     ),
 )
 def test_symbols(name, expected, symbols_text):
     # For error reporting try and find the relevant bit
     likely_line = [
         line
         for line in symbols_text.split("\n")
```

