# Comparing `tmp/genos-0.1.8.tar.gz` & `tmp/genos-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/genos-0.1.8.tar", last modified: Wed Apr 13 06:34:38 2022, max compression
+gzip compressed data, was "dist/genos-0.1.9.tar", last modified: Wed Apr 13 07:14:35 2022, max compression
```

## Comparing `genos-0.1.8.tar` & `genos-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 aldurino  (1000) aldurino  (1000)        0 2022-04-13 06:34:38.000000 genos-0.1.8/
--rw-rw-r--   0 aldurino  (1000) aldurino  (1000)     1062 2022-04-13 06:12:36.000000 genos-0.1.8/LICENSE
--rw-rw-r--   0 aldurino  (1000) aldurino  (1000)    14174 2022-04-13 06:34:38.000000 genos-0.1.8/PKG-INFO
--rw-rw-r--   0 aldurino  (1000) aldurino  (1000)    13365 2022-04-13 06:12:36.000000 genos-0.1.8/README.md
--rw-rw-r--   0 aldurino  (1000) aldurino  (1000)      584 2022-04-13 06:12:36.000000 genos-0.1.8/pyproject.toml
--rw-rw-r--   0 aldurino  (1000) aldurino  (1000)      433 2022-04-13 06:34:38.000000 genos-0.1.8/setup.cfg
--rw-rw-r--   0 aldurino  (1000) aldurino  (1000)     1894 2022-04-13 06:12:36.000000 genos-0.1.8/setup.py
-drwxrwxr-x   0 aldurino  (1000) aldurino  (1000)        0 2022-04-13 06:34:38.000000 genos-0.1.8/src/
-drwxrwxr-x   0 aldurino  (1000) aldurino  (1000)        0 2022-04-13 06:34:38.000000 genos-0.1.8/src/genos/
--rw-rw-r--   0 aldurino  (1000) aldurino  (1000)      175 2022-04-13 06:12:36.000000 genos-0.1.8/src/genos/__init__.py
-drwxrwxr-x   0 aldurino  (1000) aldurino  (1000)        0 2022-04-13 06:34:38.000000 genos-0.1.8/src/genos/examples/
--rw-rw-r--   0 aldurino  (1000) aldurino  (1000)      461 2022-04-13 06:12:36.000000 genos-0.1.8/src/genos/examples/__init__.py
--rw-rw-r--   0 aldurino  (1000) aldurino  (1000)     1919 2022-04-13 06:12:36.000000 genos-0.1.8/src/genos/examples/complex_examples.py
--rw-rw-r--   0 aldurino  (1000) aldurino  (1000)      692 2022-04-13 06:12:36.000000 genos-0.1.8/src/genos/examples/simple_examples.py
--rw-rw-r--   0 aldurino  (1000) aldurino  (1000)    12977 2022-04-13 06:12:36.000000 genos-0.1.8/src/genos/instantiate.py
--rw-rw-r--   0 aldurino  (1000) aldurino  (1000)       18 2022-04-13 06:19:25.000000 genos-0.1.8/src/genos/version.py
-drwxrwxr-x   0 aldurino  (1000) aldurino  (1000)        0 2022-04-13 06:34:38.000000 genos-0.1.8/src/genos.egg-info/
--rw-rw-r--   0 aldurino  (1000) aldurino  (1000)    14174 2022-04-13 06:34:38.000000 genos-0.1.8/src/genos.egg-info/PKG-INFO
--rw-rw-r--   0 aldurino  (1000) aldurino  (1000)      391 2022-04-13 06:34:38.000000 genos-0.1.8/src/genos.egg-info/SOURCES.txt
--rw-rw-r--   0 aldurino  (1000) aldurino  (1000)        1 2022-04-13 06:34:38.000000 genos-0.1.8/src/genos.egg-info/dependency_links.txt
--rw-rw-r--   0 aldurino  (1000) aldurino  (1000)       17 2022-04-13 06:34:38.000000 genos-0.1.8/src/genos.egg-info/requires.txt
--rw-rw-r--   0 aldurino  (1000) aldurino  (1000)        6 2022-04-13 06:34:38.000000 genos-0.1.8/src/genos.egg-info/top_level.txt
+drwxrwxr-x   0 aldurino  (1000) aldurino  (1000)        0 2022-04-13 07:14:35.000000 genos-0.1.9/
+-rw-rw-r--   0 aldurino  (1000) aldurino  (1000)     1062 2022-04-13 06:12:36.000000 genos-0.1.9/LICENSE
+-rw-rw-r--   0 aldurino  (1000) aldurino  (1000)    14174 2022-04-13 07:14:35.000000 genos-0.1.9/PKG-INFO
+-rw-rw-r--   0 aldurino  (1000) aldurino  (1000)    13365 2022-04-13 06:12:36.000000 genos-0.1.9/README.md
+-rw-rw-r--   0 aldurino  (1000) aldurino  (1000)      585 2022-04-13 06:52:03.000000 genos-0.1.9/pyproject.toml
+-rw-rw-r--   0 aldurino  (1000) aldurino  (1000)      433 2022-04-13 07:14:35.000000 genos-0.1.9/setup.cfg
+-rw-rw-r--   0 aldurino  (1000) aldurino  (1000)     1894 2022-04-13 06:12:36.000000 genos-0.1.9/setup.py
+drwxrwxr-x   0 aldurino  (1000) aldurino  (1000)        0 2022-04-13 07:14:35.000000 genos-0.1.9/src/
+drwxrwxr-x   0 aldurino  (1000) aldurino  (1000)        0 2022-04-13 07:14:35.000000 genos-0.1.9/src/genos/
+-rw-rw-r--   0 aldurino  (1000) aldurino  (1000)      175 2022-04-13 06:12:36.000000 genos-0.1.9/src/genos/__init__.py
+drwxrwxr-x   0 aldurino  (1000) aldurino  (1000)        0 2022-04-13 07:14:35.000000 genos-0.1.9/src/genos/examples/
+-rw-rw-r--   0 aldurino  (1000) aldurino  (1000)      461 2022-04-13 06:12:36.000000 genos-0.1.9/src/genos/examples/__init__.py
+-rw-rw-r--   0 aldurino  (1000) aldurino  (1000)     1919 2022-04-13 06:12:36.000000 genos-0.1.9/src/genos/examples/complex_examples.py
+-rw-rw-r--   0 aldurino  (1000) aldurino  (1000)      692 2022-04-13 06:12:36.000000 genos-0.1.9/src/genos/examples/simple_examples.py
+-rw-rw-r--   0 aldurino  (1000) aldurino  (1000)    12977 2022-04-13 06:12:36.000000 genos-0.1.9/src/genos/instantiate.py
+-rw-rw-r--   0 aldurino  (1000) aldurino  (1000)       18 2022-04-13 07:13:45.000000 genos-0.1.9/src/genos/version.py
+drwxrwxr-x   0 aldurino  (1000) aldurino  (1000)        0 2022-04-13 07:14:35.000000 genos-0.1.9/src/genos.egg-info/
+-rw-rw-r--   0 aldurino  (1000) aldurino  (1000)    14174 2022-04-13 07:14:35.000000 genos-0.1.9/src/genos.egg-info/PKG-INFO
+-rw-rw-r--   0 aldurino  (1000) aldurino  (1000)      391 2022-04-13 07:14:35.000000 genos-0.1.9/src/genos.egg-info/SOURCES.txt
+-rw-rw-r--   0 aldurino  (1000) aldurino  (1000)        1 2022-04-13 07:14:35.000000 genos-0.1.9/src/genos.egg-info/dependency_links.txt
+-rw-rw-r--   0 aldurino  (1000) aldurino  (1000)       17 2022-04-13 07:14:35.000000 genos-0.1.9/src/genos.egg-info/requires.txt
+-rw-rw-r--   0 aldurino  (1000) aldurino  (1000)        6 2022-04-13 07:14:35.000000 genos-0.1.9/src/genos.egg-info/top_level.txt
```

### Comparing `genos-0.1.8/LICENSE` & `genos-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `genos-0.1.8/PKG-INFO` & `genos-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genos
-Version: 0.1.8
+Version: 0.1.9
 Summary: Instantiate objects and call functions using dictionary configs in Python using Genos.
 Home-page: https://github.com/Neural-Space/genos
 Author: Kushal Jain
 Author-email: kushal@neuralspace.ai
 License: MIT
 Keywords: instantiation,objects,recursive instantiation,functio call,config instantiate
 Platform: UNKNOWN
```

### Comparing `genos-0.1.8/README.md` & `genos-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `genos-0.1.8/pyproject.toml` & `genos-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 version = "0.1.0"
 description = "Instantiate objects and call functions using dictionary configs in Python using Genos."
 authors = ["Ayushman Dash <ayushman@neuralspace.ai>"]
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
-omegaconf = "^2.0.4"
+omegaconf = ">=2.1.0"
 
 [tool.poetry.dev-dependencies]
 isort = "^4.3.21"
 flake8 = "^3.7.9"
 pytest = "^5.4.1"
 coverage = "^5.1"
 requirements-parser = "^0.2.0"
```

### Comparing `genos-0.1.8/setup.py` & `genos-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `genos-0.1.8/src/genos/examples/complex_examples.py` & `genos-0.1.9/src/genos/examples/complex_examples.py`

 * *Files identical despite different names*

### Comparing `genos-0.1.8/src/genos/examples/simple_examples.py` & `genos-0.1.9/src/genos/examples/simple_examples.py`

 * *Files identical despite different names*

### Comparing `genos-0.1.8/src/genos/instantiate.py` & `genos-0.1.9/src/genos/instantiate.py`

 * *Files identical despite different names*

### Comparing `genos-0.1.8/src/genos.egg-info/PKG-INFO` & `genos-0.1.9/src/genos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genos
-Version: 0.1.8
+Version: 0.1.9
 Summary: Instantiate objects and call functions using dictionary configs in Python using Genos.
 Home-page: https://github.com/Neural-Space/genos
 Author: Kushal Jain
 Author-email: kushal@neuralspace.ai
 License: MIT
 Keywords: instantiation,objects,recursive instantiation,functio call,config instantiate
 Platform: UNKNOWN
```

