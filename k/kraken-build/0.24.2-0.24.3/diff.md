# Comparing `tmp/kraken_build-0.24.2.tar.gz` & `tmp/kraken_build-0.24.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken_build-0.24.2.tar", max compression
+gzip compressed data, was "kraken_build-0.24.3.tar", max compression
```

## Comparing `kraken_build-0.24.2.tar` & `kraken_build-0.24.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      998 2023-05-19 09:06:18.694605 kraken_build-0.24.2/LICENSE
--rw-r--r--   0        0        0      178 2023-05-19 09:06:18.694605 kraken_build-0.24.2/README.md
--rw-r--r--   0        0        0      698 2023-06-17 22:02:33.441081 kraken_build-0.24.2/pyproject.toml
--rw-r--r--   0        0        0       23 2023-06-17 22:02:33.441081 kraken_build-0.24.2/src/kraken/build/__init__.py
--rw-r--r--   0        0        0     1036 1970-01-01 00:00:00.000000 kraken_build-0.24.2/PKG-INFO
+-rw-r--r--   0        0        0      998 2023-06-19 15:04:27.268759 kraken_build-0.24.3/LICENSE
+-rw-r--r--   0        0        0      178 2023-06-19 15:04:27.268965 kraken_build-0.24.3/README.md
+-rw-r--r--   0        0        0      698 2023-06-19 15:05:59.419534 kraken_build-0.24.3/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-06-19 15:05:59.419726 kraken_build-0.24.3/src/kraken/build/__init__.py
+-rw-r--r--   0        0        0     1036 1970-01-01 00:00:00.000000 kraken_build-0.24.3/PKG-INFO
```

### Comparing `kraken_build-0.24.2/LICENSE` & `kraken_build-0.24.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kraken_build-0.24.2/pyproject.toml` & `kraken_build-0.24.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kraken-build"
-version = "0.24.2"
+version = "0.24.3"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "kraken/build", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `kraken_build-0.24.2/PKG-INFO` & `kraken_build-0.24.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kraken-build
-Version: 0.24.2
+Version: 0.24.3
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

