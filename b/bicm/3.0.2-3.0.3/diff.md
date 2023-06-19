# Comparing `tmp/bicm-3.0.2.tar.gz` & `tmp/bicm-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bicm-3.0.2.tar", last modified: Mon Jun 19 13:32:58 2023, max compression
+gzip compressed data, was "bicm-3.0.3.tar", last modified: Mon Jun 19 13:37:57 2023, max compression
```

## Comparing `bicm-3.0.2.tar` & `bicm-3.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-06-19 13:32:58.725112 bicm-3.0.2/
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     1068 2023-01-04 08:23:41.000000 bicm-3.0.2/LICENSE.txt
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     4602 2023-06-19 13:32:58.725112 bicm-3.0.2/PKG-INFO
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     3928 2023-04-20 13:13:38.000000 bicm-3.0.2/README.md
-drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-06-19 13:32:58.725112 bicm-3.0.2/bicm/
--rw-rw-r--   0 matteo    (1000) matteo    (1000)      471 2023-06-19 13:30:20.000000 bicm-3.0.2/bicm/__init__.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)    73882 2023-06-19 13:21:15.000000 bicm-3.0.2/bicm/graph_classes.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)    40970 2023-04-20 08:23:16.000000 bicm-3.0.2/bicm/models_functions.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)    11883 2023-04-20 08:31:25.000000 bicm-3.0.2/bicm/network_functions.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     6409 2023-01-04 08:23:41.000000 bicm-3.0.2/bicm/poibin.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     9439 2023-04-06 09:27:43.000000 bicm-3.0.2/bicm/solver_functions.py
-drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-06-19 13:32:58.725112 bicm-3.0.2/bicm.egg-info/
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     4602 2023-06-19 13:32:58.000000 bicm-3.0.2/bicm.egg-info/PKG-INFO
--rw-rw-r--   0 matteo    (1000) matteo    (1000)      415 2023-06-19 13:32:58.000000 bicm-3.0.2/bicm.egg-info/SOURCES.txt
--rw-rw-r--   0 matteo    (1000) matteo    (1000)        1 2023-06-19 13:32:58.000000 bicm-3.0.2/bicm.egg-info/dependency_links.txt
--rw-rw-r--   0 matteo    (1000) matteo    (1000)       50 2023-06-19 13:32:58.000000 bicm-3.0.2/bicm.egg-info/requires.txt
--rw-rw-r--   0 matteo    (1000) matteo    (1000)       11 2023-06-19 13:32:58.000000 bicm-3.0.2/bicm.egg-info/top_level.txt
--rw-rw-r--   0 matteo    (1000) matteo    (1000)       38 2023-06-19 13:32:58.725112 bicm-3.0.2/setup.cfg
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     1042 2023-06-19 13:30:11.000000 bicm-3.0.2/setup.py
-drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-06-19 13:32:58.725112 bicm-3.0.2/tests/
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     9480 2023-01-04 08:23:41.000000 bicm-3.0.2/tests/BiCM_test.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)        0 2023-01-04 08:23:41.000000 bicm-3.0.2/tests/__init__.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     1804 2023-01-08 16:20:56.000000 bicm-3.0.2/tests/biwcm_c.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     2378 2023-01-08 16:20:56.000000 bicm-3.0.2/tests/biwcm_d.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     7224 2023-01-08 16:20:57.000000 bicm-3.0.2/tests/biwcm_main.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)      462 2023-01-04 18:33:41.000000 bicm-3.0.2/tests/delta_converter.py
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-06-19 13:37:57.934579 bicm-3.0.3/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     1068 2023-01-04 08:23:41.000000 bicm-3.0.3/LICENSE.txt
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     4602 2023-06-19 13:37:57.934579 bicm-3.0.3/PKG-INFO
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     3928 2023-04-20 13:13:38.000000 bicm-3.0.3/README.md
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-06-19 13:37:57.930579 bicm-3.0.3/bicm/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)      471 2023-06-19 13:36:24.000000 bicm-3.0.3/bicm/__init__.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)    73882 2023-06-19 13:21:15.000000 bicm-3.0.3/bicm/graph_classes.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)    40970 2023-04-20 08:23:16.000000 bicm-3.0.3/bicm/models_functions.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)    11883 2023-04-20 08:31:25.000000 bicm-3.0.3/bicm/network_functions.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     6409 2023-01-04 08:23:41.000000 bicm-3.0.3/bicm/poibin.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     9439 2023-04-06 09:27:43.000000 bicm-3.0.3/bicm/solver_functions.py
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-06-19 13:37:57.930579 bicm-3.0.3/bicm.egg-info/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     4602 2023-06-19 13:37:57.000000 bicm-3.0.3/bicm.egg-info/PKG-INFO
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)      415 2023-06-19 13:37:57.000000 bicm-3.0.3/bicm.egg-info/SOURCES.txt
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)        1 2023-06-19 13:37:57.000000 bicm-3.0.3/bicm.egg-info/dependency_links.txt
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)       50 2023-06-19 13:37:57.000000 bicm-3.0.3/bicm.egg-info/requires.txt
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)       11 2023-06-19 13:37:57.000000 bicm-3.0.3/bicm.egg-info/top_level.txt
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)       38 2023-06-19 13:37:57.934579 bicm-3.0.3/setup.cfg
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     1042 2023-06-19 13:36:22.000000 bicm-3.0.3/setup.py
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-06-19 13:37:57.934579 bicm-3.0.3/tests/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     9480 2023-01-04 08:23:41.000000 bicm-3.0.3/tests/BiCM_test.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)        0 2023-01-04 08:23:41.000000 bicm-3.0.3/tests/__init__.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     1804 2023-01-08 16:20:56.000000 bicm-3.0.3/tests/biwcm_c.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     2378 2023-01-08 16:20:56.000000 bicm-3.0.3/tests/biwcm_d.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     7224 2023-01-08 16:20:57.000000 bicm-3.0.3/tests/biwcm_main.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)      462 2023-01-04 18:33:41.000000 bicm-3.0.3/tests/delta_converter.py
```

### Comparing `bicm-3.0.2/LICENSE.txt` & `bicm-3.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bicm-3.0.2/PKG-INFO` & `bicm-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bicm
-Version: 3.0.2
+Version: 3.0.3
 Summary: Package for bipartite configuration model
 Home-page: https://github.com/mat701/BiCM
 Author: Matteo Bruno
 Author-email: matteobruno180@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bicm-3.0.2/README.md` & `bicm-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bicm-3.0.2/bicm/graph_classes.py` & `bicm-3.0.3/bicm/graph_classes.py`

 * *Files identical despite different names*

### Comparing `bicm-3.0.2/bicm/models_functions.py` & `bicm-3.0.3/bicm/models_functions.py`

 * *Files identical despite different names*

### Comparing `bicm-3.0.2/bicm/network_functions.py` & `bicm-3.0.3/bicm/network_functions.py`

 * *Files identical despite different names*

### Comparing `bicm-3.0.2/bicm/poibin.py` & `bicm-3.0.3/bicm/poibin.py`

 * *Files identical despite different names*

### Comparing `bicm-3.0.2/bicm/solver_functions.py` & `bicm-3.0.3/bicm/solver_functions.py`

 * *Files identical despite different names*

### Comparing `bicm-3.0.2/bicm.egg-info/PKG-INFO` & `bicm-3.0.3/bicm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bicm
-Version: 3.0.2
+Version: 3.0.3
 Summary: Package for bipartite configuration model
 Home-page: https://github.com/mat701/BiCM
 Author: Matteo Bruno
 Author-email: matteobruno180@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bicm-3.0.2/setup.py` & `bicm-3.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="bicm",
-    version="3.0.2",
+    version="3.0.3",
     author="Matteo Bruno",
     author_email="matteobruno180@gmail.com",
     description="Package for bipartite configuration model",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mat701/BiCM",
     packages=setuptools.find_packages(),
```

### Comparing `bicm-3.0.2/tests/BiCM_test.py` & `bicm-3.0.3/tests/BiCM_test.py`

 * *Files identical despite different names*

### Comparing `bicm-3.0.2/tests/biwcm_c.py` & `bicm-3.0.3/tests/biwcm_c.py`

 * *Files identical despite different names*

### Comparing `bicm-3.0.2/tests/biwcm_d.py` & `bicm-3.0.3/tests/biwcm_d.py`

 * *Files identical despite different names*

### Comparing `bicm-3.0.2/tests/biwcm_main.py` & `bicm-3.0.3/tests/biwcm_main.py`

 * *Files identical despite different names*

