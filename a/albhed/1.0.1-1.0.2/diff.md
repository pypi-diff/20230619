# Comparing `tmp/albhed-1.0.1.tar.gz` & `tmp/albhed-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "albhed-1.0.1.tar", max compression
+gzip compressed data, was "albhed-1.0.2.tar", max compression
```

## Comparing `albhed-1.0.1.tar` & `albhed-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1072 2023-06-19 18:06:45.392511 albhed-1.0.1/LICENSE
--rw-r--r--   0        0        0      217 2023-06-19 18:06:45.404321 albhed-1.0.1/README.md
--rw-r--r--   0        0        0      316 2023-06-19 18:06:45.392697 albhed-1.0.1/albhed/__init__.py
--rw-r--r--   0        0        0      586 2023-06-19 18:07:42.605562 albhed-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 albhed-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-19 18:22:17.319166 albhed-1.0.2/LICENSE
+-rw-r--r--   0        0        0      217 2023-06-19 18:22:17.319166 albhed-1.0.2/README.md
+-rw-r--r--   0        0        0      316 2023-06-19 18:22:17.319166 albhed-1.0.2/albhed/__init__.py
+-rw-r--r--   0        0        0      681 2023-06-19 18:22:32.731371 albhed-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 albhed-1.0.2/PKG-INFO
```

### Comparing `albhed-1.0.1/LICENSE` & `albhed-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `albhed-1.0.1/pyproject.toml` & `albhed-1.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "albhed"
-version = "1.0.1"
+version = "1.0.2"
 description = "Converts ASCII into Al Bhed"
 authors = ["Chris Pressland <mail@cpressland.io>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 albhed = "albhed.__init__:cli"
 
@@ -25,10 +25,13 @@
 [tool.isort]
 line_length = 88
 profile = "black"
 
 [tool.ruff]
 line-length = 88
 
+[tool.poetry-dynamic-versioning]
+enable = false
+
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `albhed-1.0.1/PKG-INFO` & `albhed-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albhed
-Version: 1.0.1
+Version: 1.0.2
 Summary: Converts ASCII into Al Bhed
 Author: Chris Pressland
 Author-email: mail@cpressland.io
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

