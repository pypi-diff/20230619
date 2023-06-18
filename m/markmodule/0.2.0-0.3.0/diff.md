# Comparing `tmp/markmodule-0.2.0.tar.gz` & `tmp/markmodule-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markmodule-0.2.0.tar", max compression
+gzip compressed data, was "markmodule-0.3.0.tar", max compression
```

## Comparing `markmodule-0.2.0.tar` & `markmodule-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-06-18 17:44:37.980431 markmodule-0.2.0/LICENSE
--rw-r--r--   0        0        0     1795 2023-06-18 17:44:37.980431 markmodule-0.2.0/README.md
--rw-r--r--   0        0        0      172 2023-06-18 17:44:37.980431 markmodule-0.2.0/markmodule/__init__.py
--rw-r--r--   0        0        0      200 2023-06-18 17:44:37.980431 markmodule-0.2.0/markmodule/class_source.py
--rw-r--r--   0        0        0     2062 2023-06-18 17:44:37.980431 markmodule-0.2.0/markmodule/import_string.py
--rw-r--r--   0        0        0     3822 2023-06-18 17:44:37.980431 markmodule-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3408 1970-01-01 00:00:00.000000 markmodule-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-18 23:29:11.624553 markmodule-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2030 2023-06-18 23:29:11.624553 markmodule-0.3.0/README.md
+-rw-r--r--   0        0        0      318 2023-06-18 23:29:11.624553 markmodule-0.3.0/markmodule/__init__.py
+-rw-r--r--   0        0        0      200 2023-06-18 23:29:11.624553 markmodule-0.3.0/markmodule/class_source.py
+-rw-r--r--   0        0        0     2879 2023-06-18 23:29:11.624553 markmodule-0.3.0/markmodule/generate_pyi.py
+-rw-r--r--   0        0        0     2244 2023-06-18 23:29:11.624553 markmodule-0.3.0/markmodule/import_string.py
+-rw-r--r--   0        0        0     2063 2023-06-18 23:29:11.624553 markmodule-0.3.0/markmodule/md_importer.py
+-rw-r--r--   0        0        0      966 2023-06-18 23:29:11.624553 markmodule-0.3.0/markmodule/string_loader.py
+-rw-r--r--   0        0        0     3700 2023-06-18 23:29:11.628553 markmodule-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3617 1970-01-01 00:00:00.000000 markmodule-0.3.0/PKG-INFO
```

### Comparing `markmodule-0.2.0/LICENSE` & `markmodule-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `markmodule-0.2.0/README.md` & `markmodule-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 # markmodule
 Import python from markdown files.
 
-## Markdown is a hammer, everything is a nail
-
-You can use markdown:
-
-- as a place to put module code, [markmodule](https://pypi.org/project/markmodule), this library
-
-The do-everything-with-markdown ecosystem is surprisingly robust.
-- as a Makefile alternative, [mask](https://github.com/jacobdeichert/mask)
-- as a place to put scripts, eg python's [markdown-exec](https://pypi.org/project/markdown-exec/), or ruby's [markdown_exec](https://github.com/fareedst/markdown_exec)
-- as a place to put unit tests, [pytest-markdown-docs](https://pypi.org/project/pytest-markdown-docs/),  [pytest-codeblocks](https://pypi.org/project/pytest_codeblocks/), and [pytest-markdown](https://pypi.org/project/pytest-markdown/)
-- as a string template, [proof-of-concept gist](https://gist.github.com/facelessuser/53fa4d93f27c252fda813b5e0ba7325c)
-
 ## Usage
 
-In a file named `hello_module.md`m define a function. I'm escaping the fence, use a real three tick fence.
+In a file named `hello_module.md` define a function. I'm escaping the fence, use a real three-tick fence.
 
 ```markdown
 Here is a function
 
 ``(`)python
-def some_function(args: str) -> str:
-    """This is a function that does something."""
-    return "Hello World" + args
-``(`)
+def hello() -> str:
+    return "Hello"
+``(`) 
+```
 
-And some more documentation 
+Generate a type stub and import using the usual syntax. `generate_side_by_side_pyi` will write a `.pyi` file to the file system and enable IDEs type hinting to work.
+
+```python
+import sys
+import markmodule
+markmodule.generate_side_by_side_pyi("hello_module")
+sys.meta_path.append(markmodule.MdFinder())
+import hello_module
+print(hello_module.hello())
 ```
 
-Import. Your IDE will not recognize the module, but it will work at runtime.
+Import with path to file.
 ```python
 import markmodule
 markmodule.import_md("hello_module.md")
 import hello_module
-
-print(hello_module.some_function("yo!"))
+print(hello_module.hello())
 ```
 
+## Markdown is a hammer, everything is a nail
+
+You can use markdown:
+
+- as a place to put module code, [markmodule](https://pypi.org/project/markmodule), this library
+
+The do-everything-with-markdown ecosystem is surprisingly robust.
+- as a Makefile alternative, [mask](https://github.com/jacobdeichert/mask)
+- as a place to put scripts, eg python's [markdown-exec](https://pypi.org/project/markdown-exec/), or ruby's [markdown_exec](https://github.com/fareedst/markdown_exec)
+- as a place to put unit tests, [pytest-markdown-docs](https://pypi.org/project/pytest-markdown-docs/),  [pytest-codeblocks](https://pypi.org/project/pytest_codeblocks/), and [pytest-markdown](https://pypi.org/project/pytest-markdown/)
+- as a string template, [proof-of-concept gist](https://gist.github.com/facelessuser/53fa4d93f27c252fda813b5e0ba7325c)
+
+
 ## Change Log
 
 - 0.1.0 - Basic idea.
 - 0.2.0 - Updates to readme
-- 
+- 0.3.0 - Generates pyi and you can use `import` syntax 
+
 ## Documentation
 
 - [Contributing](https://github.com/matthewdeanmartin/markmoduel/blob/main/docs/contributing.md)
 - [TODO](https://github.com/matthewdeanmartin/markmoduel/blob/main/docs/TODO.md)
 - [Related StackOverflow Links](https://github.com/matthewdeanmartin/markmoduel/blob/main/docs/stackoverflow.md)
-
-
```

### Comparing `markmodule-0.2.0/markmodule/import_string.py` & `markmodule-0.3.0/markmodule/import_string.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,39 +19,43 @@
     with open(path, encoding="utf-8") as file:
         string_value = file.read()
         import_markdown_string(string_value, path.stem)
 
 
 def import_markdown_string(string_value: str, module_name: str) -> None:
     """Import markdown as a string."""
-    parser = mistune.create_markdown(renderer="ast")
+    code_string = parse_code_out_of_markdown(string_value)
+
+    if not code_string:
+        raise TypeError("Can't find source code in markdown file")
+    import_code_string(code_string, module_name)
+
 
+def parse_code_out_of_markdown(string_value: str) -> str:
+    """Get python code out of markdown"""
+    parser = mistune.create_markdown(renderer="ast")
     if mistune.__version__.startswith("3"):
         result, _block_state = parser.parse(string_value)
     else:
         result = parser.parse(string_value)
-
     code_string = ""
     for token in result:
         if token["type"] == "blank_line":
             continue
         if mistune.__version__.startswith("3."):
             if token["type"] == "block_code" and token.get("attrs", {}).get("info") in (
                 "python",
                 "python3",
                 "py",
             ):
                 code_string += token["raw"]
         else:
             if token["type"] == "block_code" and token["info"] == "python":
                 code_string += token["text"]
-
-    if not code_string:
-        raise TypeError("Can't find source code in markdown file")
-    import_code_string(code_string, module_name)
+    return code_string
 
 
 def import_code_string(code_string: str, module_name: str) -> None:
     """Import a code string as a module using function. See md_module_support to import
     using `import` syntax."""
     spec = importlib.util.spec_from_loader(module_name, loader=None)
     if not spec:
```

### Comparing `markmodule-0.2.0/pyproject.toml` & `markmodule-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "markmodule"
-version = "0.2.0"
+version = "0.3.0"
 description = "Import python code in markdown as module"
 authors = ["Matthew Martin <matthewdeanmartin@gmail.com>"]
 keywords = ["markdown",]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -33,26 +33,20 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/matthewdeanmartin/markmodule/issues"
 "Change Log" = "https://github.com/matthewdeanmartin/markmodule/blob/main/CHANGES.md"
 
 [tool.poetry.dependencies]
 # DOM parser
 mistune = "<3.0.0"
-# support more types to table
-tabulate = "*"
-# image/binary support
-pillow = "*"
+mypy = "*"
 # 3.8/3/9 support
 typing-extensions = { version = ">=4.0.0, <5.0", python = "<=3.9" }
 
 [tool.poetry.dev-dependencies]
-# alternate formatter
 mdformat = "*"
-#marko = "*"
-#mistletoe = "*"
 pytest = "*"
 vermin = "*"
 hypothesis = {extras = ["cli"], version = "*"}
 pre-commit = "*"
 mypy = "*"
 
 [tool.black]
```

### Comparing `markmodule-0.2.0/PKG-INFO` & `markmodule-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markmodule
-Version: 0.2.0
+Version: 0.3.0
 Summary: Import python code in markdown as module
 Home-page: https://github.com/matthewdeanmartin/markmodule
 License: MIT
 Keywords: markdown
 Author: Matthew Martin
 Author-email: matthewdeanmartin@gmail.com
 Classifier: Development Status :: 3 - Alpha
@@ -21,69 +21,75 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: mistune (<3.0.0)
-Requires-Dist: pillow
-Requires-Dist: tabulate
+Requires-Dist: mypy
 Requires-Dist: typing-extensions (>=4.0.0,<5.0) ; python_full_version <= "3.9.0"
 Project-URL: Bug Tracker, https://github.com/matthewdeanmartin/markmodule/issues
 Project-URL: Change Log, https://github.com/matthewdeanmartin/markmodule/blob/main/CHANGES.md
 Project-URL: Documentation, https://github.com/matthewdeanmartin/markmodule
 Project-URL: Repository, https://github.com/matthewdeanmartin/markmodule
 Description-Content-Type: text/markdown
 
 # markmodule
 Import python from markdown files.
 
-## Markdown is a hammer, everything is a nail
-
-You can use markdown:
-
-- as a place to put module code, [markmodule](https://pypi.org/project/markmodule), this library
-
-The do-everything-with-markdown ecosystem is surprisingly robust.
-- as a Makefile alternative, [mask](https://github.com/jacobdeichert/mask)
-- as a place to put scripts, eg python's [markdown-exec](https://pypi.org/project/markdown-exec/), or ruby's [markdown_exec](https://github.com/fareedst/markdown_exec)
-- as a place to put unit tests, [pytest-markdown-docs](https://pypi.org/project/pytest-markdown-docs/),  [pytest-codeblocks](https://pypi.org/project/pytest_codeblocks/), and [pytest-markdown](https://pypi.org/project/pytest-markdown/)
-- as a string template, [proof-of-concept gist](https://gist.github.com/facelessuser/53fa4d93f27c252fda813b5e0ba7325c)
-
 ## Usage
 
-In a file named `hello_module.md`m define a function. I'm escaping the fence, use a real three tick fence.
+In a file named `hello_module.md` define a function. I'm escaping the fence, use a real three-tick fence.
 
 ```markdown
 Here is a function
 
 ``(`)python
-def some_function(args: str) -> str:
-    """This is a function that does something."""
-    return "Hello World" + args
-``(`)
+def hello() -> str:
+    return "Hello"
+``(`) 
+```
 
-And some more documentation 
+Generate a type stub and import using the usual syntax. `generate_side_by_side_pyi` will write a `.pyi` file to the file system and enable IDEs type hinting to work.
+
+```python
+import sys
+import markmodule
+markmodule.generate_side_by_side_pyi("hello_module")
+sys.meta_path.append(markmodule.MdFinder())
+import hello_module
+print(hello_module.hello())
 ```
 
-Import. Your IDE will not recognize the module, but it will work at runtime.
+Import with path to file.
 ```python
 import markmodule
 markmodule.import_md("hello_module.md")
 import hello_module
-
-print(hello_module.some_function("yo!"))
+print(hello_module.hello())
 ```
 
+## Markdown is a hammer, everything is a nail
+
+You can use markdown:
+
+- as a place to put module code, [markmodule](https://pypi.org/project/markmodule), this library
+
+The do-everything-with-markdown ecosystem is surprisingly robust.
+- as a Makefile alternative, [mask](https://github.com/jacobdeichert/mask)
+- as a place to put scripts, eg python's [markdown-exec](https://pypi.org/project/markdown-exec/), or ruby's [markdown_exec](https://github.com/fareedst/markdown_exec)
+- as a place to put unit tests, [pytest-markdown-docs](https://pypi.org/project/pytest-markdown-docs/),  [pytest-codeblocks](https://pypi.org/project/pytest_codeblocks/), and [pytest-markdown](https://pypi.org/project/pytest-markdown/)
+- as a string template, [proof-of-concept gist](https://gist.github.com/facelessuser/53fa4d93f27c252fda813b5e0ba7325c)
+
+
 ## Change Log
 
 - 0.1.0 - Basic idea.
 - 0.2.0 - Updates to readme
-- 
+- 0.3.0 - Generates pyi and you can use `import` syntax 
+
 ## Documentation
 
 - [Contributing](https://github.com/matthewdeanmartin/markmoduel/blob/main/docs/contributing.md)
 - [TODO](https://github.com/matthewdeanmartin/markmoduel/blob/main/docs/TODO.md)
 - [Related StackOverflow Links](https://github.com/matthewdeanmartin/markmoduel/blob/main/docs/stackoverflow.md)
 
-
-
```

