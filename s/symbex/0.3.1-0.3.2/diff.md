# Comparing `tmp/symbex-0.3.1.tar.gz` & `tmp/symbex-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbex-0.3.1.tar", last modified: Mon Jun 19 14:28:38 2023, max compression
+gzip compressed data, was "symbex-0.3.2.tar", last modified: Mon Jun 19 15:52:56 2023, max compression
```

## Comparing `symbex-0.3.1.tar` & `symbex-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:28:38.180785 symbex-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 14:28:22.000000 symbex-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-19 14:28:38.180785 symbex-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-06-19 14:28:22.000000 symbex-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 14:28:38.180785 symbex-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-19 14:28:22.000000 symbex-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:28:38.180785 symbex-0.3.1/symbex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:28:22.000000 symbex-0.3.1/symbex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-19 14:28:22.000000 symbex-0.3.1/symbex/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-19 14:28:22.000000 symbex-0.3.1/symbex/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-06-19 14:28:22.000000 symbex-0.3.1/symbex/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:28:38.180785 symbex-0.3.1/symbex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-19 14:28:38.000000 symbex-0.3.1/symbex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-19 14:28:38.000000 symbex-0.3.1/symbex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 14:28:38.000000 symbex-0.3.1/symbex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 14:28:38.000000 symbex-0.3.1/symbex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 14:28:38.000000 symbex-0.3.1/symbex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 14:28:38.000000 symbex-0.3.1/symbex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:28:38.180785 symbex-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-06-19 14:28:22.000000 symbex-0.3.1/tests/test_symbex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-19 14:28:22.000000 symbex-0.3.1/tests/test_symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:56.290764 symbex-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 15:52:39.000000 symbex-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-19 15:52:56.286764 symbex-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-06-19 15:52:39.000000 symbex-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 15:52:56.290764 symbex-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-19 15:52:39.000000 symbex-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:56.286764 symbex-0.3.2/symbex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:39.000000 symbex-0.3.2/symbex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-19 15:52:39.000000 symbex-0.3.2/symbex/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-19 15:52:39.000000 symbex-0.3.2/symbex/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-06-19 15:52:39.000000 symbex-0.3.2/symbex/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:56.286764 symbex-0.3.2/symbex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-19 15:52:56.000000 symbex-0.3.2/symbex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-19 15:52:56.000000 symbex-0.3.2/symbex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:52:56.000000 symbex-0.3.2/symbex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 15:52:56.000000 symbex-0.3.2/symbex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 15:52:56.000000 symbex-0.3.2/symbex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 15:52:56.000000 symbex-0.3.2/symbex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:56.286764 symbex-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-19 15:52:39.000000 symbex-0.3.2/tests/test_symbex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-19 15:52:39.000000 symbex-0.3.2/tests/test_symbols.py
```

### Comparing `symbex-0.3.1/LICENSE` & `symbex-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `symbex-0.3.1/PKG-INFO` & `symbex-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbex
-Version: 0.3.1
+Version: 0.3.2
 Summary: Find the Python code for specified symbols
 Home-page: https://github.com/simonw/symbex
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/symbex/issues
 Project-URL: CI, https://github.com/simonw/symbex/actions
 Project-URL: Changelog, https://github.com/simonw/symbex/releases
@@ -128,15 +128,15 @@
     "```\n{}\n```\n".format("\n\n".join(chunks))
 )
 ]]] -->
 ```
 # File: symbex/cli.py Line: 37
 def cli(symbols, files, directories, signatures, silent)
 
-# File: symbex/lib.py Line: 150
+# File: symbex/lib.py Line: 161
 def class_definition(class_def)
 
 # File: symbex/lib.py Line: 32
 def code_for_node(code: str, node: AST, class_name: str, signatures: bool)
 
 # File: symbex/lib.py Line: 63
 def match(name: str, symbols) -> bool
```

### Comparing `symbex-0.3.1/README.md` & `symbex-0.3.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     "```\n{}\n```\n".format("\n\n".join(chunks))
 )
 ]]] -->
 ```
 # File: symbex/cli.py Line: 37
 def cli(symbols, files, directories, signatures, silent)
 
-# File: symbex/lib.py Line: 150
+# File: symbex/lib.py Line: 161
 def class_definition(class_def)
 
 # File: symbex/lib.py Line: 32
 def code_for_node(code: str, node: AST, class_name: str, signatures: bool)
 
 # File: symbex/lib.py Line: 63
 def match(name: str, symbols) -> bool
```

### Comparing `symbex-0.3.1/setup.py` & `symbex-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.3.1"
+VERSION = "0.3.2"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `symbex-0.3.1/symbex/cli.py` & `symbex-0.3.2/symbex/cli.py`

 * *Files identical despite different names*

### Comparing `symbex-0.3.1/symbex/lib.py` & `symbex-0.3.2/symbex/lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,15 +105,22 @@
     position_of_star = len(all_args) - len(function_node.args.kwonlyargs)
 
     # function_node.args.defaults may have defaults
     # corresponding to function_node.args.args - but
     # if defaults has 2 and args has 3 then those
     # defaults correspond to the last two args
     defaults = [None] * (len(all_args) - len(function_node.args.defaults))
-    defaults.extend(literal_eval(default) for default in function_node.args.defaults)
+    for default in function_node.args.defaults:
+        try:
+            value = literal_eval(default)
+            if isinstance(value, str):
+                value = f'"{value}"'
+        except ValueError:
+            value = getattr(default, "id", "...")
+        defaults.append(value)
 
     arguments = []
 
     for i, (arg, default) in enumerate(zip_longest(all_args, defaults)):
         if position_of_slash and i == position_of_slash:
             arguments.append("/")
         if position_of_star and i == position_of_star:
```

### Comparing `symbex-0.3.1/symbex.egg-info/PKG-INFO` & `symbex-0.3.2/symbex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbex
-Version: 0.3.1
+Version: 0.3.2
 Summary: Find the Python code for specified symbols
 Home-page: https://github.com/simonw/symbex
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/symbex/issues
 Project-URL: CI, https://github.com/simonw/symbex/actions
 Project-URL: Changelog, https://github.com/simonw/symbex/releases
@@ -128,15 +128,15 @@
     "```\n{}\n```\n".format("\n\n".join(chunks))
 )
 ]]] -->
 ```
 # File: symbex/cli.py Line: 37
 def cli(symbols, files, directories, signatures, silent)
 
-# File: symbex/lib.py Line: 150
+# File: symbex/lib.py Line: 161
 def class_definition(class_def)
 
 # File: symbex/lib.py Line: 32
 def code_for_node(code: str, node: AST, class_name: str, signatures: bool)
 
 # File: symbex/lib.py Line: 63
 def match(name: str, symbols) -> bool
```

### Comparing `symbex-0.3.1/tests/test_symbex.py` & `symbex-0.3.2/tests/test_symbex.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 @pytest.fixture
 def directory_full_of_code(tmpdir):
     for path, content in (
         ("foo.py", "def foo1():\n    pass\n\n@decorated\ndef foo2():\n    pass\n\n"),
         ("bar.py", "class BarClass:\n    pass\n\n"),
-        ("nested/baz.py", "def baz():\n    pass\n\n"),
+        ("nested/baz.py", 'def baz(delimiter=", ", type=str):\n    pass\n\n'),
         ("nested/error.py", "def baz_error()" + "bug:\n    pass\n\n"),
         (
             "methods.py",
             textwrap.dedent(
                 """
         class MyClass:
             def __init__(self, a):
@@ -56,29 +56,29 @@
         ),
         (
             ["BarClass", "--silent"],
             "# File: bar.py Line: 1\nclass BarClass:\n    pass\n\n",
         ),
         (
             ["baz", "--silent"],
-            "# File: nested/baz.py Line: 1\ndef baz():\n    pass\n\n",
+            '# File: nested/baz.py Line: 1\ndef baz(delimiter=", ", type=str):\n    pass\n\n',
         ),
         (
             ["async_func", "--silent"],
             "# File: async.py Line: 1\nasync def async_func(a, b, c):\n    pass\n\n",
         ),
         # The -f option
         (
             ["baz", "-f", "nested/baz.py", "--silent"],
-            "# File: nested/baz.py Line: 1\ndef baz():\n    pass\n\n",
+            '# File: nested/baz.py Line: 1\ndef baz(delimiter=", ", type=str):\n    pass\n\n',
         ),
         # The -d option
         (
             ["baz", "-d", "nested", "--silent"],
-            "# File: nested/baz.py Line: 1\ndef baz():\n    pass\n\n",
+            '# File: nested/baz.py Line: 1\ndef baz(delimiter=", ", type=str):\n    pass\n\n',
         ),
         # Classes
         (
             ["MyClass", "--silent"],
             "# File: methods.py Line: 2\n"
             "class MyClass:\n"
             "    def __init__(self, a):\n"
@@ -140,15 +140,18 @@
             "# File: foo.py Line: 1\n"
             "def foo1()\n"
             "\n"
             "# File: foo.py Line: 5\n"
             "def foo2()",
         ),
         (["BarClass", "--silent"], "# File: bar.py Line: 1\n" "class BarClass"),
-        (["baz", "--silent"], ("# File: nested/baz.py Line: 1\n" "def baz()")),
+        (
+            ["baz", "--silent"],
+            ("# File: nested/baz.py Line: 1\n" 'def baz(delimiter=", ", type=str)'),
+        ),
     ),
 )
 def test_symbex_symbols(directory_full_of_code, monkeypatch, args, expected):
     runner = CliRunner()
     monkeypatch.chdir(directory_full_of_code)
     result = runner.invoke(cli, args + ["-s"], catch_exceptions=False)
     assert result.exit_code == 0
@@ -158,12 +161,15 @@
 
 def test_errors(directory_full_of_code, monkeypatch):
     # Test without --silent to see errors
     runner = CliRunner(mix_stderr=False)
     monkeypatch.chdir(directory_full_of_code)
     result = runner.invoke(cli, ["baz"], catch_exceptions=False)
     assert result.exit_code == 0
-    assert result.stdout == (
-        "# File: nested/baz.py Line: 1\n" "def baz():\n" "    pass\n\n"
+    expected = (
+        "# File: nested/baz.py Line: 1\n"
+        'def baz(delimiter=", ", type=str):\n'
+        "    pass\n\n"
     )
+    assert result.stdout == expected
     # This differs between different Python versions
     assert result.stderr.startswith("# Syntax error in nested/error.py:")
```

### Comparing `symbex-0.3.1/tests/test_symbols.py` & `symbex-0.3.2/tests/test_symbols.py`

 * *Files identical despite different names*

