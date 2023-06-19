# Comparing `tmp/py_madvr-1.4.2.tar.gz` & `tmp/py_madvr-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr-1.4.2.tar", last modified: Mon Jun 19 16:10:06 2023, max compression
+gzip compressed data, was "py_madvr-1.4.3.tar", last modified: Mon Jun 19 17:17:45 2023, max compression
```

## Comparing `py_madvr-1.4.2.tar` & `py_madvr-1.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:10:06.774314 py_madvr-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-19 16:09:55.000000 py_madvr-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-19 16:10:06.774314 py_madvr-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-19 16:09:55.000000 py_madvr-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:10:06.770314 py_madvr-1.4.2/madvr/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-19 16:09:55.000000 py_madvr-1.4.2/madvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-19 16:09:55.000000 py_madvr-1.4.2/madvr/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-19 16:09:55.000000 py_madvr-1.4.2/madvr/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-06-19 16:09:55.000000 py_madvr-1.4.2/madvr/madvr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:10:06.770314 py_madvr-1.4.2/py_madvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-19 16:10:06.000000 py_madvr-1.4.2/py_madvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-19 16:10:06.000000 py_madvr-1.4.2/py_madvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:10:06.000000 py_madvr-1.4.2/py_madvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 16:10:06.000000 py_madvr-1.4.2/py_madvr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 16:10:06.774314 py_madvr-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-19 16:09:55.000000 py_madvr-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:10:06.774314 py_madvr-1.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:09:55.000000 py_madvr-1.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-19 16:09:55.000000 py_madvr-1.4.2/tests/testMadVR.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:17:45.661504 py_madvr-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-19 17:17:34.000000 py_madvr-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-19 17:17:45.661504 py_madvr-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-19 17:17:34.000000 py_madvr-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:17:45.661504 py_madvr-1.4.3/madvr/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-19 17:17:34.000000 py_madvr-1.4.3/madvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-19 17:17:34.000000 py_madvr-1.4.3/madvr/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-19 17:17:34.000000 py_madvr-1.4.3/madvr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-06-19 17:17:34.000000 py_madvr-1.4.3/madvr/madvr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:17:45.661504 py_madvr-1.4.3/py_madvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-19 17:17:45.000000 py_madvr-1.4.3/py_madvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-19 17:17:45.000000 py_madvr-1.4.3/py_madvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 17:17:45.000000 py_madvr-1.4.3/py_madvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 17:17:45.000000 py_madvr-1.4.3/py_madvr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 17:17:45.661504 py_madvr-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-19 17:17:34.000000 py_madvr-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:17:45.661504 py_madvr-1.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 17:17:34.000000 py_madvr-1.4.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-19 17:17:34.000000 py_madvr-1.4.3/tests/testMadVR.py
```

### Comparing `py_madvr-1.4.2/LICENSE` & `py_madvr-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr-1.4.2/PKG-INFO` & `py_madvr-1.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr
-Version: 1.4.2
+Version: 1.4.3
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.4.2/madvr/commands.py` & `py_madvr-1.4.3/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr-1.4.2/madvr/madvr.py` & `py_madvr-1.4.3/madvr/madvr.py`

 * *Files identical despite different names*

### Comparing `py_madvr-1.4.2/py_madvr.egg-info/PKG-INFO` & `py_madvr-1.4.3/py_madvr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-madvr
-Version: 1.4.2
+Version: 1.4.3
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.4.2/setup.py` & `py_madvr-1.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr",
-    version="1.4.2",
+    version="1.4.3",
     author="iloveicedgreentea",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr-1.4.2/tests/testMadVR.py` & `py_madvr-1.4.3/tests/testMadVR.py`

 * *Files identical despite different names*

