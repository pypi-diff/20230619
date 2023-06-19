# Comparing `tmp/orange3-fca-addon-0.0.2.tar.gz` & `tmp/orange3-fca-addon-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orange3-fca-addon-0.0.2.tar", last modified: Mon Jun 19 13:34:50 2023, max compression
+gzip compressed data, was "orange3-fca-addon-0.0.3.tar", last modified: Mon Jun 19 13:43:48 2023, max compression
```

## Comparing `orange3-fca-addon-0.0.2.tar` & `orange3-fca-addon-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 shisus    (1000) shisus    (1000)        0 2023-06-19 13:34:50.003073 orange3-fca-addon-0.0.2/
--rw-rw-r--   0 shisus    (1000) shisus    (1000)    35146 2023-06-16 07:46:48.000000 orange3-fca-addon-0.0.2/LICENSE
--rw-rw-r--   0 shisus    (1000) shisus    (1000)    42509 2023-06-19 13:34:50.003073 orange3-fca-addon-0.0.2/PKG-INFO
--rw-rw-r--   0 shisus    (1000) shisus    (1000)      841 2023-06-19 11:48:28.000000 orange3-fca-addon-0.0.2/README.md
-drwxrwxr-x   0 shisus    (1000) shisus    (1000)        0 2023-06-19 13:34:50.003073 orange3-fca-addon-0.0.2/orange3_fca_addon.egg-info/
--rw-rw-r--   0 shisus    (1000) shisus    (1000)    42509 2023-06-19 13:34:49.000000 orange3-fca-addon-0.0.2/orange3_fca_addon.egg-info/PKG-INFO
--rw-rw-r--   0 shisus    (1000) shisus    (1000)      315 2023-06-19 13:34:49.000000 orange3-fca-addon-0.0.2/orange3_fca_addon.egg-info/SOURCES.txt
--rw-rw-r--   0 shisus    (1000) shisus    (1000)        1 2023-06-19 13:34:49.000000 orange3-fca-addon-0.0.2/orange3_fca_addon.egg-info/dependency_links.txt
--rw-rw-r--   0 shisus    (1000) shisus    (1000)      134 2023-06-19 13:34:49.000000 orange3-fca-addon-0.0.2/orange3_fca_addon.egg-info/entry_points.txt
--rw-rw-r--   0 shisus    (1000) shisus    (1000)       68 2023-06-19 13:34:49.000000 orange3-fca-addon-0.0.2/orange3_fca_addon.egg-info/requires.txt
--rw-rw-r--   0 shisus    (1000) shisus    (1000)       14 2023-06-19 13:34:49.000000 orange3-fca-addon-0.0.2/orange3_fca_addon.egg-info/top_level.txt
-drwxrwxr-x   0 shisus    (1000) shisus    (1000)        0 2023-06-19 13:34:50.003073 orange3-fca-addon-0.0.2/orangecontrib/
--rw-rw-r--   0 shisus    (1000) shisus    (1000)        0 2023-06-16 10:09:19.000000 orange3-fca-addon-0.0.2/orangecontrib/__init__.py
--rw-rw-r--   0 shisus    (1000) shisus    (1000)     1258 2023-06-19 13:34:35.000000 orange3-fca-addon-0.0.2/pyproject.toml
--rw-rw-r--   0 shisus    (1000) shisus    (1000)       38 2023-06-19 13:34:50.003073 orange3-fca-addon-0.0.2/setup.cfg
--rw-rw-r--   0 shisus    (1000) shisus    (1000)     1018 2023-06-19 13:22:42.000000 orange3-fca-addon-0.0.2/setup.py
+drwxrwxr-x   0 shisus    (1000) shisus    (1000)        0 2023-06-19 13:43:48.755089 orange3-fca-addon-0.0.3/
+-rw-rw-r--   0 shisus    (1000) shisus    (1000)    35146 2023-06-16 07:46:48.000000 orange3-fca-addon-0.0.3/LICENSE
+-rw-rw-r--   0 shisus    (1000) shisus    (1000)    42502 2023-06-19 13:43:48.755089 orange3-fca-addon-0.0.3/PKG-INFO
+-rw-rw-r--   0 shisus    (1000) shisus    (1000)      841 2023-06-19 11:48:28.000000 orange3-fca-addon-0.0.3/README.md
+drwxrwxr-x   0 shisus    (1000) shisus    (1000)        0 2023-06-19 13:43:48.755089 orange3-fca-addon-0.0.3/orange3_fca_addon.egg-info/
+-rw-rw-r--   0 shisus    (1000) shisus    (1000)    42502 2023-06-19 13:43:48.000000 orange3-fca-addon-0.0.3/orange3_fca_addon.egg-info/PKG-INFO
+-rw-rw-r--   0 shisus    (1000) shisus    (1000)      315 2023-06-19 13:43:48.000000 orange3-fca-addon-0.0.3/orange3_fca_addon.egg-info/SOURCES.txt
+-rw-rw-r--   0 shisus    (1000) shisus    (1000)        1 2023-06-19 13:43:48.000000 orange3-fca-addon-0.0.3/orange3_fca_addon.egg-info/dependency_links.txt
+-rw-rw-r--   0 shisus    (1000) shisus    (1000)      134 2023-06-19 13:43:48.000000 orange3-fca-addon-0.0.3/orange3_fca_addon.egg-info/entry_points.txt
+-rw-rw-r--   0 shisus    (1000) shisus    (1000)       68 2023-06-19 13:43:48.000000 orange3-fca-addon-0.0.3/orange3_fca_addon.egg-info/requires.txt
+-rw-rw-r--   0 shisus    (1000) shisus    (1000)       14 2023-06-19 13:43:48.000000 orange3-fca-addon-0.0.3/orange3_fca_addon.egg-info/top_level.txt
+drwxrwxr-x   0 shisus    (1000) shisus    (1000)        0 2023-06-19 13:43:48.755089 orange3-fca-addon-0.0.3/orangecontrib/
+-rw-rw-r--   0 shisus    (1000) shisus    (1000)        0 2023-06-16 10:09:19.000000 orange3-fca-addon-0.0.3/orangecontrib/__init__.py
+-rw-rw-r--   0 shisus    (1000) shisus    (1000)     1250 2023-06-19 13:43:37.000000 orange3-fca-addon-0.0.3/pyproject.toml
+-rw-rw-r--   0 shisus    (1000) shisus    (1000)       38 2023-06-19 13:43:48.755089 orange3-fca-addon-0.0.3/setup.cfg
+-rw-rw-r--   0 shisus    (1000) shisus    (1000)     1018 2023-06-19 13:22:42.000000 orange3-fca-addon-0.0.3/setup.py
```

### Comparing `orange3-fca-addon-0.0.2/LICENSE` & `orange3-fca-addon-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `orange3-fca-addon-0.0.2/PKG-INFO` & `orange3-fca-addon-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orange3-fca-addon
-Version: 0.0.2
+Version: 0.0.3
 Summary: Orange FCA add-on for Orange data mining software package.
 Author-email: jesus laime <laimejesu@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -689,15 +689,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
-Requires-Python: <=3.10,>=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Orange-FCA
 
 This repository contains an add-on for the Orange Datamining Framework which extends the functionality with multiple Formal Concept Analysis widgets.
```

### Comparing `orange3-fca-addon-0.0.2/README.md` & `orange3-fca-addon-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `orange3-fca-addon-0.0.2/orange3_fca_addon.egg-info/PKG-INFO` & `orange3-fca-addon-0.0.3/orange3_fca_addon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orange3-fca-addon
-Version: 0.0.2
+Version: 0.0.3
 Summary: Orange FCA add-on for Orange data mining software package.
 Author-email: jesus laime <laimejesu@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -689,15 +689,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
-Requires-Python: <=3.10,>=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Orange-FCA
 
 This repository contains an add-on for the Orange Datamining Framework which extends the functionality with multiple Formal Concept Analysis widgets.
```

### Comparing `orange3-fca-addon-0.0.2/pyproject.toml` & `orange3-fca-addon-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "orange3-fca-addon"
-version = "0.0.2"
+version = "0.0.3"
 description = "Orange FCA add-on for Orange data mining software package."
 authors = [
   {name = "jesus laime", email = "laimejesu@gmail.com"},
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
-requires-python = ">=3.7, <=3.10"
+requires-python = ">=3.7"
 keywords= ["orange3 add-on"]
 classifiers = [
   "Development Status :: 1 - Planning",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
```

### Comparing `orange3-fca-addon-0.0.2/setup.py` & `orange3-fca-addon-0.0.3/setup.py`

 * *Files identical despite different names*

