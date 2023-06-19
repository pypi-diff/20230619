# Comparing `tmp/htruc-1.0.7.tar.gz` & `tmp/htruc-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htruc-1.0.7.tar", last modified: Mon Jun 19 08:23:14 2023, max compression
+gzip compressed data, was "htruc-1.0.8.tar", last modified: Mon Jun 19 08:44:24 2023, max compression
```

## Comparing `htruc-1.0.7.tar` & `htruc-1.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-06-19 08:23:14.347750 htruc-1.0.7/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    16725 2023-06-19 07:16:39.000000 htruc-1.0.7/LICENSE.md
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1874 2023-06-19 08:23:14.347750 htruc-1.0.7/PKG-INFO
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1191 2022-06-20 10:01:21.000000 htruc-1.0.7/README.md
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-06-19 08:23:14.347750 htruc-1.0.7/htruc/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2021-09-23 12:36:36.000000 htruc-1.0.7/htruc/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    11474 2023-06-19 07:36:30.000000 htruc-1.0.7/htruc/catalog.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     8939 2023-06-19 08:19:51.000000 htruc-1.0.7/htruc/cli.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-06-19 08:23:14.347750 htruc-1.0.7/htruc/repos/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      118 2022-06-21 08:16:17.000000 htruc-1.0.7/htruc/repos/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      492 2022-02-04 15:30:28.000000 htruc-1.0.7/htruc/repos/_generic.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2537 2023-06-19 07:58:45.000000 htruc-1.0.7/htruc/repos/_github.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-06-19 08:23:14.347750 htruc-1.0.7/htruc/schemas/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1220 2022-06-20 10:01:21.000000 htruc-1.0.7/htruc/schemas/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1021 2022-06-20 10:01:21.000000 htruc-1.0.7/htruc/schemas/upgrade_path.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      130 2022-06-20 10:01:21.000000 htruc-1.0.7/htruc/types.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2390 2023-06-19 08:19:31.000000 htruc-1.0.7/htruc/utils.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2882 2023-06-19 07:59:20.000000 htruc-1.0.7/htruc/validator.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-06-19 08:23:14.347750 htruc-1.0.7/htruc.egg-info/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1874 2023-06-19 08:23:14.000000 htruc-1.0.7/htruc.egg-info/PKG-INFO
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      429 2023-06-19 08:23:14.000000 htruc-1.0.7/htruc.egg-info/SOURCES.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2023-06-19 08:23:14.000000 htruc-1.0.7/htruc.egg-info/dependency_links.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       41 2023-06-19 08:23:14.000000 htruc-1.0.7/htruc.egg-info/entry_points.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      176 2023-06-19 08:23:14.000000 htruc-1.0.7/htruc.egg-info/requires.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        6 2023-06-19 08:23:14.000000 htruc-1.0.7/htruc.egg-info/top_level.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       38 2023-06-19 08:23:14.347750 htruc-1.0.7/setup.cfg
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3799 2023-06-19 07:41:49.000000 htruc-1.0.7/setup.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-06-19 08:44:24.724958 htruc-1.0.8/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    16725 2023-06-19 07:16:39.000000 htruc-1.0.8/LICENSE.md
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1874 2023-06-19 08:44:24.724958 htruc-1.0.8/PKG-INFO
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1191 2022-06-20 10:01:21.000000 htruc-1.0.8/README.md
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-06-19 08:44:24.724958 htruc-1.0.8/htruc/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2021-09-23 12:36:36.000000 htruc-1.0.8/htruc/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    11544 2023-06-19 08:29:18.000000 htruc-1.0.8/htruc/catalog.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     8939 2023-06-19 08:19:51.000000 htruc-1.0.8/htruc/cli.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-06-19 08:44:24.724958 htruc-1.0.8/htruc/repos/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      118 2022-06-21 08:16:17.000000 htruc-1.0.8/htruc/repos/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      492 2022-02-04 15:30:28.000000 htruc-1.0.8/htruc/repos/_generic.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2537 2023-06-19 07:58:45.000000 htruc-1.0.8/htruc/repos/_github.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-06-19 08:44:24.724958 htruc-1.0.8/htruc/schemas/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1220 2022-06-20 10:01:21.000000 htruc-1.0.8/htruc/schemas/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1021 2022-06-20 10:01:21.000000 htruc-1.0.8/htruc/schemas/upgrade_path.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      130 2022-06-20 10:01:21.000000 htruc-1.0.8/htruc/types.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2390 2023-06-19 08:19:31.000000 htruc-1.0.8/htruc/utils.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2882 2023-06-19 07:59:20.000000 htruc-1.0.8/htruc/validator.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-06-19 08:44:24.724958 htruc-1.0.8/htruc.egg-info/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1874 2023-06-19 08:44:24.000000 htruc-1.0.8/htruc.egg-info/PKG-INFO
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      429 2023-06-19 08:44:24.000000 htruc-1.0.8/htruc.egg-info/SOURCES.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2023-06-19 08:44:24.000000 htruc-1.0.8/htruc.egg-info/dependency_links.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       41 2023-06-19 08:44:24.000000 htruc-1.0.8/htruc.egg-info/entry_points.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      176 2023-06-19 08:44:24.000000 htruc-1.0.8/htruc.egg-info/requires.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        6 2023-06-19 08:44:24.000000 htruc-1.0.8/htruc.egg-info/top_level.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       38 2023-06-19 08:44:24.724958 htruc-1.0.8/setup.cfg
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     3799 2023-06-19 08:29:31.000000 htruc-1.0.8/setup.py
```

### Comparing `htruc-1.0.7/LICENSE.md` & `htruc-1.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `htruc-1.0.7/PKG-INFO` & `htruc-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htruc
-Version: 1.0.7
+Version: 1.0.8
 Summary: HTRUC, a toolkit for HTR-United cataloging
 Home-page: https://github.com/htr-united/htrvc
 Author: Thibault Clérice
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `htruc-1.0.7/README.md` & `htruc-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `htruc-1.0.7/htruc/catalog.py` & `htruc-1.0.8/htruc/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,16 @@
 
 def clever_catalog_update(catalog1: Dict, catalog2: Dict) -> Dict:
     for repository in catalog2:
         if repository in catalog1:
             for key in ["characters", "volume"]:
                 if key in catalog2[repository]:
                     catalog1[repository][key] = catalog2[repository][key]
+        else:
+            catalog1[repository] = catalog2[repository]
     return catalog1
 
 
 def get_all_catalogs(
     access_token: Optional[str] = None,
     local_directory: Optional[str] = None,
     get_distant: bool = True,
```

### Comparing `htruc-1.0.7/htruc/cli.py` & `htruc-1.0.8/htruc/cli.py`

 * *Files identical despite different names*

### Comparing `htruc-1.0.7/htruc/repos/_github.py` & `htruc-1.0.8/htruc/repos/_github.py`

 * *Files identical despite different names*

### Comparing `htruc-1.0.7/htruc/schemas/__init__.py` & `htruc-1.0.8/htruc/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `htruc-1.0.7/htruc/schemas/upgrade_path.py` & `htruc-1.0.8/htruc/schemas/upgrade_path.py`

 * *Files identical despite different names*

### Comparing `htruc-1.0.7/htruc/utils.py` & `htruc-1.0.8/htruc/utils.py`

 * *Files identical despite different names*

### Comparing `htruc-1.0.7/htruc/validator.py` & `htruc-1.0.8/htruc/validator.py`

 * *Files identical despite different names*

### Comparing `htruc-1.0.7/htruc.egg-info/PKG-INFO` & `htruc-1.0.8/htruc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htruc
-Version: 1.0.7
+Version: 1.0.8
 Summary: HTRUC, a toolkit for HTR-United cataloging
 Home-page: https://github.com/htr-united/htrvc
 Author: Thibault Clérice
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `htruc-1.0.7/setup.py` & `htruc-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # Package meta-data.
 NAME = 'htruc'
 DESCRIPTION = 'HTRUC, a toolkit for HTR-United cataloging'
 URL = 'https://github.com/htr-united/htrvc'
 AUTHOR = 'Thibault Clérice'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = "1.0.7"
+VERSION = "1.0.8"
 
 # What packages are required for this module to be executed?
 
 with open(os.path.join(here, 'requirements.txt')) as f:
     REQUIRED = f.read().splitlines()
 
 # What packages are optional?
```

