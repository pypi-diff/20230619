# Comparing `tmp/bild-0.0.4.tar.gz` & `tmp/bild-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/simongh/gitlibs/bild/dist/tmp3c1htdwf/bild-0.0.4.tar", last modified: Fri Nov  4 01:24:44 2022, max compression
+gzip compressed data, was "/home/simongh/gitlibs/bild/dist/.tmp-k03riomj/bild-0.0.5.tar", last modified: Mon Jun 19 19:28:13 2023, max compression
```

## Comparing `bild-0.0.4.tar` & `bild-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxrwxr-x   0 simongh   (8090) simongh   (8090)        0 2022-11-04 01:24:44.000000 bild-0.0.4/
--rw-rw-r--   0 simongh   (8090) simongh   (8090)     1074 2022-08-27 01:59:25.000000 bild-0.0.4/LICENSE
--rw-rw-r--   0 simongh   (8090) simongh   (8090)     2503 2022-11-04 01:24:44.000000 bild-0.0.4/PKG-INFO
--rw-rw-r--   0 simongh   (8090) simongh   (8090)      657 2022-08-31 23:30:46.000000 bild-0.0.4/README.md
-drwxrwxr-x   0 simongh   (8090) simongh   (8090)        0 2022-11-04 01:24:44.000000 bild-0.0.4/bild/
--rw-rw-r--   0 simongh   (8090) simongh   (8090)      587 2022-10-27 03:06:47.000000 bild-0.0.4/bild/__init__.py
--rw-rw-r--   0 simongh   (8090) simongh   (8090)    36002 2022-11-04 01:14:32.000000 bild-0.0.4/bild/amis.py
--rw-rw-r--   0 simongh   (8090) simongh   (8090)    10347 2022-10-28 14:40:56.000000 bild-0.0.4/bild/core.py
--rw-rw-r--   0 simongh   (8090) simongh   (8090)      248 2022-11-04 01:14:32.000000 bild-0.0.4/bild/cython_imports.py
--rw-rw-r--   0 simongh   (8090) simongh   (8090)    19911 2022-11-04 00:02:16.000000 bild-0.0.4/bild/models.py
--rw-rw-r--   0 simongh   (8090) simongh   (8090)     3762 2022-08-25 18:36:07.000000 bild-0.0.4/bild/postproc.py
-drwxrwxr-x   0 simongh   (8090) simongh   (8090)        0 2022-11-04 01:24:44.000000 bild-0.0.4/bild/src/
--rw-rw-r--   0 simongh   (8090) simongh   (8090)  1006234 2022-11-04 01:15:34.000000 bild-0.0.4/bild/src/MSRouse_logL.c
--rw-rw-r--   0 simongh   (8090) simongh   (8090)     3584 2022-11-04 00:02:16.000000 bild-0.0.4/bild/src/MSRouse_logL_py.py
--rw-rw-r--   0 simongh   (8090) simongh   (8090)     3424 2022-08-25 18:43:11.000000 bild-0.0.4/bild/stats.py
--rw-rw-r--   0 simongh   (8090) simongh   (8090)     5517 2022-08-25 18:36:07.000000 bild-0.0.4/bild/util.py
-drwxrwxr-x   0 simongh   (8090) simongh   (8090)        0 2022-11-04 01:24:44.000000 bild-0.0.4/bild.egg-info/
--rw-rw-r--   0 simongh   (8090) simongh   (8090)     2503 2022-11-04 01:24:44.000000 bild-0.0.4/bild.egg-info/PKG-INFO
--rw-rw-r--   0 simongh   (8090) simongh   (8090)      384 2022-11-04 01:24:44.000000 bild-0.0.4/bild.egg-info/SOURCES.txt
--rw-rw-r--   0 simongh   (8090) simongh   (8090)        1 2022-11-04 01:24:44.000000 bild-0.0.4/bild.egg-info/dependency_links.txt
--rw-rw-r--   0 simongh   (8090) simongh   (8090)        1 2022-11-03 23:56:18.000000 bild-0.0.4/bild.egg-info/not-zip-safe
--rw-rw-r--   0 simongh   (8090) simongh   (8090)       53 2022-11-04 01:24:44.000000 bild-0.0.4/bild.egg-info/requires.txt
--rw-rw-r--   0 simongh   (8090) simongh   (8090)        5 2022-11-04 01:24:44.000000 bild-0.0.4/bild.egg-info/top_level.txt
--rw-rw-r--   0 simongh   (8090) simongh   (8090)      818 2022-11-04 01:24:26.000000 bild-0.0.4/pyproject.toml
--rw-rw-r--   0 simongh   (8090) simongh   (8090)       38 2022-11-04 01:24:44.000000 bild-0.0.4/setup.cfg
--rw-rw-r--   0 simongh   (8090) simongh   (8090)     2005 2022-11-04 00:02:16.000000 bild-0.0.4/setup.py
+drwxrwxr-x   0 simongh   (8090) simongh   (8090)        0 2023-06-19 19:28:13.000000 bild-0.0.5/
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)     1074 2022-08-27 01:59:25.000000 bild-0.0.5/LICENSE
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)     2503 2023-06-19 19:28:13.000000 bild-0.0.5/PKG-INFO
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)      657 2022-08-31 23:30:46.000000 bild-0.0.5/README.md
+drwxrwxr-x   0 simongh   (8090) simongh   (8090)        0 2023-06-19 19:28:13.000000 bild-0.0.5/bild/
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)      587 2022-10-27 03:06:47.000000 bild-0.0.5/bild/__init__.py
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)    36002 2022-11-04 01:14:32.000000 bild-0.0.5/bild/amis.py
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)    10347 2022-10-28 14:40:56.000000 bild-0.0.5/bild/core.py
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)      248 2022-11-04 01:14:32.000000 bild-0.0.5/bild/cython_imports.py
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)    19911 2022-11-04 00:02:16.000000 bild-0.0.5/bild/models.py
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)     3762 2022-08-25 18:36:07.000000 bild-0.0.5/bild/postproc.py
+drwxrwxr-x   0 simongh   (8090) simongh   (8090)        0 2023-06-19 19:28:13.000000 bild-0.0.5/bild/src/
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)  1006234 2022-11-04 01:15:34.000000 bild-0.0.5/bild/src/MSRouse_logL.c
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)     3584 2022-11-04 00:02:16.000000 bild-0.0.5/bild/src/MSRouse_logL_py.py
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)     3424 2022-08-25 18:43:11.000000 bild-0.0.5/bild/stats.py
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)     5517 2022-08-25 18:36:07.000000 bild-0.0.5/bild/util.py
+drwxrwxr-x   0 simongh   (8090) simongh   (8090)        0 2023-06-19 19:28:13.000000 bild-0.0.5/bild.egg-info/
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)     2503 2023-06-19 19:28:13.000000 bild-0.0.5/bild.egg-info/PKG-INFO
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)      422 2023-06-19 19:28:13.000000 bild-0.0.5/bild.egg-info/SOURCES.txt
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)        1 2023-06-19 19:28:13.000000 bild-0.0.5/bild.egg-info/dependency_links.txt
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)        1 2022-11-03 23:56:18.000000 bild-0.0.5/bild.egg-info/not-zip-safe
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)       53 2023-06-19 19:28:13.000000 bild-0.0.5/bild.egg-info/requires.txt
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)        5 2023-06-19 19:28:13.000000 bild-0.0.5/bild.egg-info/top_level.txt
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)      818 2023-06-19 19:25:49.000000 bild-0.0.5/pyproject.toml
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)       38 2023-06-19 19:28:13.000000 bild-0.0.5/setup.cfg
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)     2005 2022-11-04 00:02:16.000000 bild-0.0.5/setup.py
+drwxrwxr-x   0 simongh   (8090) simongh   (8090)        0 2023-06-19 19:28:13.000000 bild-0.0.5/tests/
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)     8718 2023-06-19 18:16:24.000000 bild-0.0.5/tests/test_amis.py
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)    10549 2023-06-19 18:16:24.000000 bild-0.0.5/tests/test_bild.py
```

### Comparing `bild-0.0.4/LICENSE` & `bild-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bild-0.0.4/PKG-INFO` & `bild-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bild
-Version: 0.0.4
+Version: 0.0.5
 Summary: Bayesian Inference of Looping Dynamics
 Author-email: Simon Grosse-Holz <sgh256@mit.edu>
 License: MIT License
         
         Copyright (c) 2022 Simon Grosse-Holz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bild-0.0.4/README.md` & `bild-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bild-0.0.4/bild/__init__.py` & `bild-0.0.5/bild/__init__.py`

 * *Files identical despite different names*

### Comparing `bild-0.0.4/bild/amis.py` & `bild-0.0.5/bild/amis.py`

 * *Files identical despite different names*

### Comparing `bild-0.0.4/bild/core.py` & `bild-0.0.5/bild/core.py`

 * *Files identical despite different names*

### Comparing `bild-0.0.4/bild/models.py` & `bild-0.0.5/bild/models.py`

 * *Files identical despite different names*

### Comparing `bild-0.0.4/bild/postproc.py` & `bild-0.0.5/bild/postproc.py`

 * *Files identical despite different names*

### Comparing `bild-0.0.4/bild/src/MSRouse_logL.c` & `bild-0.0.5/bild/src/MSRouse_logL.c`

 * *Files identical despite different names*

### Comparing `bild-0.0.4/bild/src/MSRouse_logL_py.py` & `bild-0.0.5/bild/src/MSRouse_logL_py.py`

 * *Files identical despite different names*

### Comparing `bild-0.0.4/bild/stats.py` & `bild-0.0.5/bild/stats.py`

 * *Files identical despite different names*

### Comparing `bild-0.0.4/bild/util.py` & `bild-0.0.5/bild/util.py`

 * *Files identical despite different names*

### Comparing `bild-0.0.4/bild.egg-info/PKG-INFO` & `bild-0.0.5/bild.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bild
-Version: 0.0.4
+Version: 0.0.5
 Summary: Bayesian Inference of Looping Dynamics
 Author-email: Simon Grosse-Holz <sgh256@mit.edu>
 License: MIT License
         
         Copyright (c) 2022 Simon Grosse-Holz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bild-0.0.4/pyproject.toml` & `bild-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel", "numpy>=1.20"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bild"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Simon Grosse-Holz", email="sgh256@mit.edu" }
 ]
 description = "Bayesian Inference of Looping Dynamics"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `bild-0.0.4/setup.py` & `bild-0.0.5/setup.py`

 * *Files identical despite different names*

