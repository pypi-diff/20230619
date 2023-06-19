# Comparing `tmp/fuzzy_magic-1.0.tar.gz` & `tmp/fuzzy_magic-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzy_magic-1.0.tar", last modified: Tue Jun 13 10:17:29 2023, max compression
+gzip compressed data, was "fuzzy_magic-1.0.1.tar", last modified: Mon Jun 19 11:07:20 2023, max compression
```

## Comparing `fuzzy_magic-1.0.tar` & `fuzzy_magic-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 plopez    (1000) plopez    (1000)        0 2023-06-13 10:17:29.348330 fuzzy_magic-1.0/
--rw-r--r--   0 plopez    (1000) plopez    (1000)     1068 2023-06-13 07:43:46.000000 fuzzy_magic-1.0/LICENSE.txt
--rw-r--r--   0 plopez    (1000) plopez    (1000)     1243 2023-06-13 10:17:29.348330 fuzzy_magic-1.0/PKG-INFO
--rw-r--r--   0 plopez    (1000) plopez    (1000)      739 2023-05-26 12:52:15.000000 fuzzy_magic-1.0/README.md
--rw-r--r--   0 plopez    (1000) plopez    (1000)      574 2023-06-13 10:16:23.000000 fuzzy_magic-1.0/pyproject.toml
--rw-r--r--   0 plopez    (1000) plopez    (1000)       38 2023-06-13 10:17:29.348330 fuzzy_magic-1.0/setup.cfg
--rw-r--r--   0 plopez    (1000) plopez    (1000)      730 2023-06-13 10:17:15.000000 fuzzy_magic-1.0/setup.py
-drwxr-xr-x   0 plopez    (1000) plopez    (1000)        0 2023-06-13 10:17:29.337497 fuzzy_magic-1.0/src/
-drwxr-xr-x   0 plopez    (1000) plopez    (1000)        0 2023-06-13 10:17:29.337497 fuzzy_magic-1.0/src/fuzzy_magic.egg-info/
--rw-r--r--   0 plopez    (1000) plopez    (1000)     1243 2023-06-13 10:17:29.000000 fuzzy_magic-1.0/src/fuzzy_magic.egg-info/PKG-INFO
--rw-r--r--   0 plopez    (1000) plopez    (1000)      302 2023-06-13 10:17:29.000000 fuzzy_magic-1.0/src/fuzzy_magic.egg-info/SOURCES.txt
--rw-r--r--   0 plopez    (1000) plopez    (1000)        1 2023-06-13 10:17:29.000000 fuzzy_magic-1.0/src/fuzzy_magic.egg-info/dependency_links.txt
--rw-r--r--   0 plopez    (1000) plopez    (1000)       30 2023-06-13 10:17:29.000000 fuzzy_magic-1.0/src/fuzzy_magic.egg-info/requires.txt
--rw-r--r--   0 plopez    (1000) plopez    (1000)        1 2023-06-13 10:17:29.000000 fuzzy_magic-1.0/src/fuzzy_magic.egg-info/top_level.txt
-drwxr-xr-x   0 plopez    (1000) plopez    (1000)        0 2023-06-13 10:17:29.348330 fuzzy_magic-1.0/test/
--rw-r--r--   0 plopez    (1000) plopez    (1000)     1386 2023-05-26 12:52:15.000000 fuzzy_magic-1.0/test/test_fuzzy.py
--rw-r--r--   0 plopez    (1000) plopez    (1000)      519 2023-05-18 15:36:42.000000 fuzzy_magic-1.0/test/test_memberships.py
--rw-r--r--   0 plopez    (1000) plopez    (1000)     3034 2023-05-18 15:30:36.000000 fuzzy_magic-1.0/test/test_rules.py
+drwxr-xr-x   0 plopez    (1000) plopez    (1000)        0 2023-06-19 11:07:20.253837 fuzzy_magic-1.0.1/
+-rw-r--r--   0 plopez    (1000) plopez    (1000)     1068 2023-06-13 07:43:46.000000 fuzzy_magic-1.0.1/LICENSE.txt
+-rw-r--r--   0 plopez    (1000) plopez    (1000)     1245 2023-06-19 11:07:20.253837 fuzzy_magic-1.0.1/PKG-INFO
+-rw-r--r--   0 plopez    (1000) plopez    (1000)      739 2023-05-26 12:52:15.000000 fuzzy_magic-1.0.1/README.md
+-rw-r--r--   0 plopez    (1000) plopez    (1000)      576 2023-06-19 11:07:18.000000 fuzzy_magic-1.0.1/pyproject.toml
+-rw-r--r--   0 plopez    (1000) plopez    (1000)       38 2023-06-19 11:07:20.253837 fuzzy_magic-1.0.1/setup.cfg
+-rw-r--r--   0 plopez    (1000) plopez    (1000)      781 2023-06-19 11:01:03.000000 fuzzy_magic-1.0.1/setup.py
+drwxr-xr-x   0 plopez    (1000) plopez    (1000)        0 2023-06-19 11:07:20.243837 fuzzy_magic-1.0.1/src/
+drwxr-xr-x   0 plopez    (1000) plopez    (1000)        0 2023-06-19 11:07:20.253837 fuzzy_magic-1.0.1/src/fuzzy_magic.egg-info/
+-rw-r--r--   0 plopez    (1000) plopez    (1000)     1245 2023-06-19 11:07:20.000000 fuzzy_magic-1.0.1/src/fuzzy_magic.egg-info/PKG-INFO
+-rw-r--r--   0 plopez    (1000) plopez    (1000)      302 2023-06-19 11:07:20.000000 fuzzy_magic-1.0.1/src/fuzzy_magic.egg-info/SOURCES.txt
+-rw-r--r--   0 plopez    (1000) plopez    (1000)        1 2023-06-19 11:07:20.000000 fuzzy_magic-1.0.1/src/fuzzy_magic.egg-info/dependency_links.txt
+-rw-r--r--   0 plopez    (1000) plopez    (1000)       30 2023-06-19 11:07:20.000000 fuzzy_magic-1.0.1/src/fuzzy_magic.egg-info/requires.txt
+-rw-r--r--   0 plopez    (1000) plopez    (1000)        1 2023-06-19 11:07:20.000000 fuzzy_magic-1.0.1/src/fuzzy_magic.egg-info/top_level.txt
+drwxr-xr-x   0 plopez    (1000) plopez    (1000)        0 2023-06-19 11:07:20.253837 fuzzy_magic-1.0.1/test/
+-rw-r--r--   0 plopez    (1000) plopez    (1000)     1386 2023-05-26 12:52:15.000000 fuzzy_magic-1.0.1/test/test_fuzzy.py
+-rw-r--r--   0 plopez    (1000) plopez    (1000)      519 2023-05-18 15:36:42.000000 fuzzy_magic-1.0.1/test/test_memberships.py
+-rw-r--r--   0 plopez    (1000) plopez    (1000)     3034 2023-05-18 15:30:36.000000 fuzzy_magic-1.0.1/test/test_rules.py
```

### Comparing `fuzzy_magic-1.0/LICENSE.txt` & `fuzzy_magic-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fuzzy_magic-1.0/PKG-INFO` & `fuzzy_magic-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzy_magic
-Version: 1.0
+Version: 1.0.1
 Summary: A Fuzzy Logic library to create Mamdani Fuzzy Systems the easiest way possible
 Home-page: https://github.com/EXUS-AI-Labs/ailabs-fuzzylogic
 Author: Pedro López
 Author-email: Pedro López <p.lopez@exus.ai>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fuzzy_magic-1.0/README.md` & `fuzzy_magic-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fuzzy_magic-1.0/pyproject.toml` & `fuzzy_magic-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","numpy==1.23.5","simpful==2.10.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fuzzy_magic"
-version = "1.0"
+version = "1.0.1"
 authors = [
   { name="Pedro López", email="p.lopez@exus.ai" },
 ]
 description = "A Fuzzy Logic library to create Mamdani Fuzzy Systems the easiest way possible"
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies=["numpy==1.23.5","simpful==2.10.0"]
```

### Comparing `fuzzy_magic-1.0/setup.py` & `fuzzy_magic-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "fuzzy_magic",
-    version = "1.0",
+    version = "1.0.1",
     author = "Pedro López",
     author_email = "p.lopez@exus.ai",
     url = "https://github.com/EXUS-AI-Labs/ailabs-fuzzylogic",
     description = "A Fuzzy Logic library to create Mamdani Fuzzy Systems the easiest way possible",
     long_description = long_description,
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
+        "Intended Audience :: Science/Research",
     ],
     package_dir = {"": "src"},
     packages = setuptools.find_packages(where="src"),
     python_requires = ">=3.6"
 )
```

### Comparing `fuzzy_magic-1.0/src/fuzzy_magic.egg-info/PKG-INFO` & `fuzzy_magic-1.0.1/src/fuzzy_magic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzy-magic
-Version: 1.0
+Version: 1.0.1
 Summary: A Fuzzy Logic library to create Mamdani Fuzzy Systems the easiest way possible
 Home-page: https://github.com/EXUS-AI-Labs/ailabs-fuzzylogic
 Author: Pedro López
 Author-email: Pedro López <p.lopez@exus.ai>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fuzzy_magic-1.0/test/test_fuzzy.py` & `fuzzy_magic-1.0.1/test/test_fuzzy.py`

 * *Files identical despite different names*

### Comparing `fuzzy_magic-1.0/test/test_memberships.py` & `fuzzy_magic-1.0.1/test/test_memberships.py`

 * *Files identical despite different names*

### Comparing `fuzzy_magic-1.0/test/test_rules.py` & `fuzzy_magic-1.0.1/test/test_rules.py`

 * *Files identical despite different names*

