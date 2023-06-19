# Comparing `tmp/aqsconverters-0.1.0.tar.gz` & `tmp/aqsconverters-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqsconverters-0.1.0.tar", last modified: Wed Feb 15 12:14:42 2023, max compression
+gzip compressed data, was "aqsconverters-0.1.1.tar", last modified: Mon Jun 19 10:14:59 2023, max compression
```

## Comparing `aqsconverters-0.1.0.tar` & `aqsconverters-0.1.1.tar`

### file list

```diff
@@ -1,44 +1,32 @@
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2023-02-15 12:14:42.697862 aqsconverters-0.1.0/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       25 2022-09-21 14:21:30.000000 aqsconverters-0.1.0/.gitignore
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1517 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/LICENSE
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      155 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/MANIFEST.in
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      988 2023-02-15 12:14:42.697862 aqsconverters-0.1.0/PKG-INFO
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       37 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/README.md
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        6 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/VERSION
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2023-02-15 12:14:42.693862 aqsconverters-0.1.0/aqschema_converters.egg-info/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      983 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/aqschema_converters.egg-info/PKG-INFO
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      580 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/aqschema_converters.egg-info/SOURCES.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        1 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/aqschema_converters.egg-info/dependency_links.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        1 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/aqschema_converters.egg-info/not-zip-safe
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       29 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/aqschema_converters.egg-info/requires.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       20 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/aqschema_converters.egg-info/top_level.txt
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2023-02-15 12:14:42.693862 aqsconverters-0.1.0/aqsconverters/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      799 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/aqsconverters/__init__.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    10214 2022-09-21 14:21:30.000000 aqsconverters-0.1.0/aqsconverters/aq.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     5407 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/aqsconverters/common.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      552 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/aqsconverters/decorators.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1317 2022-09-21 14:21:30.000000 aqsconverters-0.1.0/aqsconverters/io.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     5722 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/aqsconverters/keras.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    10490 2023-02-15 12:14:22.000000 aqsconverters-0.1.0/aqsconverters/models.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1827 2022-09-21 14:21:30.000000 aqsconverters-0.1.0/aqsconverters/owl.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1734 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/aqsconverters/session.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     3813 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/aqsconverters/sklearn.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     3630 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/aqsconverters/xgboost.py
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2023-02-15 12:14:42.697862 aqsconverters-0.1.0/aqsconverters.egg-info/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      988 2023-02-15 12:14:42.000000 aqsconverters-0.1.0/aqsconverters.egg-info/PKG-INFO
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      967 2023-02-15 12:14:42.000000 aqsconverters-0.1.0/aqsconverters.egg-info/SOURCES.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        1 2023-02-15 12:14:42.000000 aqsconverters-0.1.0/aqsconverters.egg-info/dependency_links.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        1 2022-09-19 09:18:54.000000 aqsconverters-0.1.0/aqsconverters.egg-info/not-zip-safe
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       29 2023-02-15 12:14:42.000000 aqsconverters-0.1.0/aqsconverters.egg-info/requires.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       20 2023-02-15 12:14:42.000000 aqsconverters-0.1.0/aqsconverters.egg-info/top_level.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        0 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/conftest.py
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2023-02-15 12:14:42.697862 aqsconverters-0.1.0/dist/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    11308 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/dist/aqschema-converters-0.1.0.tar.gz
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    14663 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/dist/aqschema_converters-0.1.0-py3-none-any.whl
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       38 2023-02-15 12:14:42.697862 aqsconverters-0.1.0/setup.cfg
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1320 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/setup.py
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2023-02-15 12:14:42.697862 aqsconverters-0.1.0/tests/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       13 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/tests/__init__.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      791 2022-09-21 14:21:30.000000 aqsconverters-0.1.0/tests/test_aq.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1378 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/tests/test_keras.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     3491 2021-11-02 09:54:02.000000 aqsconverters-0.1.0/tests/test_model.py
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-06-19 10:14:59.762407 aqsconverters-0.1.1/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     1517 2021-11-03 10:50:08.000000 aqsconverters-0.1.1/LICENSE
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      155 2021-11-03 10:50:08.000000 aqsconverters-0.1.1/MANIFEST.in
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      959 2023-06-19 10:14:59.762407 aqsconverters-0.1.1/PKG-INFO
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)       37 2021-11-03 10:50:08.000000 aqsconverters-0.1.1/README.md
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        6 2023-06-19 10:12:37.000000 aqsconverters-0.1.1/VERSION
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-06-19 10:14:59.758407 aqsconverters-0.1.1/aqsconverters/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        0 2023-06-14 13:37:26.000000 aqsconverters-0.1.1/aqsconverters/__init__.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    10093 2023-06-15 10:18:45.000000 aqsconverters-0.1.1/aqsconverters/aq.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     5407 2021-11-03 10:50:08.000000 aqsconverters-0.1.1/aqsconverters/common.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      552 2021-11-03 10:50:08.000000 aqsconverters-0.1.1/aqsconverters/decorators.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      828 2023-06-15 09:22:40.000000 aqsconverters-0.1.1/aqsconverters/io.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     5722 2021-11-03 10:50:08.000000 aqsconverters-0.1.1/aqsconverters/keras.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    10490 2023-06-14 11:22:18.000000 aqsconverters-0.1.1/aqsconverters/models.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     1827 2023-06-14 11:22:18.000000 aqsconverters-0.1.1/aqsconverters/owl.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     1734 2021-11-03 10:50:08.000000 aqsconverters-0.1.1/aqsconverters/session.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     3813 2021-11-03 10:50:08.000000 aqsconverters-0.1.1/aqsconverters/sklearn.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     3630 2021-11-03 10:50:08.000000 aqsconverters-0.1.1/aqsconverters/xgboost.py
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-06-19 10:14:59.762407 aqsconverters-0.1.1/aqsconverters.egg-info/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      959 2023-06-19 10:14:59.000000 aqsconverters-0.1.1/aqsconverters.egg-info/PKG-INFO
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      602 2023-06-19 10:14:59.000000 aqsconverters-0.1.1/aqsconverters.egg-info/SOURCES.txt
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        1 2023-06-19 10:14:59.000000 aqsconverters-0.1.1/aqsconverters.egg-info/dependency_links.txt
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        1 2021-11-03 10:50:36.000000 aqsconverters-0.1.1/aqsconverters.egg-info/not-zip-safe
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)       29 2023-06-19 10:14:59.000000 aqsconverters-0.1.1/aqsconverters.egg-info/requires.txt
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)       20 2023-06-19 10:14:59.000000 aqsconverters-0.1.1/aqsconverters.egg-info/top_level.txt
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)       38 2023-06-19 10:14:59.762407 aqsconverters-0.1.1/setup.cfg
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     1320 2021-11-03 10:50:08.000000 aqsconverters-0.1.1/setup.py
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-06-19 10:14:59.762407 aqsconverters-0.1.1/tests/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)       13 2021-11-03 10:50:08.000000 aqsconverters-0.1.1/tests/__init__.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      791 2023-06-14 11:22:18.000000 aqsconverters-0.1.1/tests/test_aq.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     1378 2021-11-03 10:50:08.000000 aqsconverters-0.1.1/tests/test_keras.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     3491 2021-11-03 10:50:08.000000 aqsconverters-0.1.1/tests/test_model.py
```

### Comparing `aqsconverters-0.1.0/LICENSE` & `aqsconverters-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aqsconverters-0.1.0/PKG-INFO` & `aqsconverters-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: aqsconverters
-Version: 0.1.0
+Version: 0.1.1
 Summary: AQSchema Converter
-Home-page: UNKNOWN
 Author: Volodymyr Savchenko, Gabriele Barni
 Author-email: volodymyr.savchenko@unige.ch
 License: BSD 3.0
 Keywords: AQSchema
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -19,10 +18,7 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 4 - Beta
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `aqsconverters-0.1.0/aqschema_converters.egg-info/PKG-INFO` & `aqsconverters-0.1.1/aqsconverters.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-Metadata-Version: 1.1
-Name: aqschema-converters
-Version: 0.1.0
+Metadata-Version: 2.1
+Name: aqsconverters
+Version: 0.1.1
 Summary: AQSchema Converter
-Home-page: UNKNOWN
 Author: Volodymyr Savchenko, Gabriele Barni
 Author-email: volodymyr.savchenko@unige.ch
 License: BSD 3.0
-Description: UNKNOWN
 Keywords: AQSchema
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -19,7 +17,8 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 4 - Beta
+License-File: LICENSE
```

### Comparing `aqsconverters-0.1.0/aqsconverters/aq.py` & `aqsconverters-0.1.1/aqsconverters/aq.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,16 @@
     Position,
     Angle,
     Pixels,
     ImageBand,
     Run,
     RunSchema,
 )
-from .common import fn_args_as_params, mls_add_param
-from .io import log_renku_aqs
-from distutils.version import LooseVersion
+from .io import log_aqs_annotation
 from uuid import uuid1
-import random
-import json
 
 
 def standardize_types(v):
     if isinstance(v, np.ndarray):
         return [normalize_float(x) for x in v.tolist()]
     elif isinstance(v, float):
         return normalize_float(v)
@@ -197,18 +193,18 @@
 
         # extra stuff for debug
         run.aq_module_name = aq_module_name
         run.aq_query_type = aq_query_type
         run.aq_args = args
         run.aq_kwargs = kwargs
 
-        log_renku_aqs(
-            RunSchema().dumps(run), str(run_id),
-            force=True,
-            run=run
+        log_aqs_annotation(
+            RunSchema().dumps(run),
+            str(run_id),
+            force=True
         )        
 
     # aq hook
     def aqs_query_object(self, *args, **kwargs):
         produce_annotation(self, 'query_object', *args, **kwargs)
 
         return object.__getattribute__(self, 'query_object')(*args, **kwargs)
```

### Comparing `aqsconverters-0.1.0/aqsconverters/common.py` & `aqsconverters-0.1.1/aqsconverters/common.py`

 * *Files identical despite different names*

### Comparing `aqsconverters-0.1.0/aqsconverters/decorators.py` & `aqsconverters-0.1.1/aqsconverters/decorators.py`

 * *Files identical despite different names*

### Comparing `aqsconverters-0.1.0/aqsconverters/keras.py` & `aqsconverters-0.1.1/aqsconverters/keras.py`

 * *Files identical despite different names*

### Comparing `aqsconverters-0.1.0/aqsconverters/models.py` & `aqsconverters-0.1.1/aqsconverters/models.py`

 * *Files identical despite different names*

### Comparing `aqsconverters-0.1.0/aqsconverters/owl.py` & `aqsconverters-0.1.1/aqsconverters/owl.py`

 * *Files identical despite different names*

### Comparing `aqsconverters-0.1.0/aqsconverters/session.py` & `aqsconverters-0.1.1/aqsconverters/session.py`

 * *Files identical despite different names*

### Comparing `aqsconverters-0.1.0/aqsconverters/sklearn.py` & `aqsconverters-0.1.1/aqsconverters/sklearn.py`

 * *Files identical despite different names*

### Comparing `aqsconverters-0.1.0/aqsconverters/xgboost.py` & `aqsconverters-0.1.1/aqsconverters/xgboost.py`

 * *Files identical despite different names*

### Comparing `aqsconverters-0.1.0/setup.py` & `aqsconverters-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `aqsconverters-0.1.0/tests/test_aq.py` & `aqsconverters-0.1.1/tests/test_aq.py`

 * *Files identical despite different names*

### Comparing `aqsconverters-0.1.0/tests/test_keras.py` & `aqsconverters-0.1.1/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `aqsconverters-0.1.0/tests/test_model.py` & `aqsconverters-0.1.1/tests/test_model.py`

 * *Files identical despite different names*

