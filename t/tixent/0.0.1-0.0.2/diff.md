# Comparing `tmp/tixent-0.0.1.tar.gz` & `tmp/tixent-0.0.2.tar.gz`

## Comparing `tixent-0.0.1.tar` & `tixent-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tixent-0.0.1/tixent/__init__.py
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 tixent-0.0.1/tixent/_core.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 tixent-0.0.1/tixent/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tixent-0.0.1/tixent/py.typed
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 tixent-0.0.1/tixent/types.py
--rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 tixent-0.0.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tixent-0.0.1/LICENSE
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 tixent-0.0.1/README.md
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 tixent-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5216 2020-02-02 00:00:00.000000 tixent-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 tixent-0.0.2/tixent/__init__.py
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 tixent-0.0.2/tixent/_core.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 tixent-0.0.2/tixent/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tixent-0.0.2/tixent/py.typed
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 tixent-0.0.2/tixent/types.py
+-rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 tixent-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tixent-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 tixent-0.0.2/README.md
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 tixent-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5216 2020-02-02 00:00:00.000000 tixent-0.0.2/PKG-INFO
```

### Comparing `tixent-0.0.1/tixent/_core.py` & `tixent-0.0.2/tixent/_core.py`

 * *Files identical despite different names*

### Comparing `tixent-0.0.1/.gitignore` & `tixent-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tixent-0.0.1/LICENSE` & `tixent-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tixent-0.0.1/README.md` & `tixent-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tixent-0.0.1/pyproject.toml` & `tixent-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -81,26 +81,26 @@
 detached = true
 python = "3.11"
 
 [tool.hatch.envs.lint.scripts]
 check = [
   "black --check --diff {args:.}",
   "isort --check {args:.}",
-  "docformatter {args:--check .}",
+  "docformatter --check {args:.}",
   "ruff {args:.}",
   "typing",
 ]
 format = [
   "black {args:.}",
   "isort {args:.}",
-  "docformatter {args:--in-place .}",
+  "docformatter --in-place {args:.}",
   "ruff --fix {args:.}",
   "typing",
 ]
-typing = "mypy --install-types --non-interactive {args:src tests}"
+typing = "mypy {args:src tests}"
 
 [tool.coverage.run]
 branch = true
 omit = ["src/tixent/types.py"]
 parallel = true
 source_pkgs = ["tixent"]
 
@@ -130,14 +130,16 @@
 [tool.isort]
 include_trailing_comma = true
 line_length = 88
 multi_line_output = 3
 profile = "black"
 
 [tool.mypy]
+install_types = true
+non_interactive = true
 strict = true
 
 [tool.ruff]
 ignore = [
   "D200",
   "D205",
   "ANN",
```

### Comparing `tixent-0.0.1/PKG-INFO` & `tixent-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tixent
-Version: 0.0.1
+Version: 0.0.2
 Summary: A text splitting tool
 Project-URL: Documentation, https://github.com/sincekmori/tixent#readme
 Project-URL: Issues, https://github.com/sincekmori/tixent/issues
 Project-URL: Source, https://github.com/sincekmori/tixent
 Author-email: Shinsuke Mori <sincekmori@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

