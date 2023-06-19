# Comparing `tmp/exmol-3.0.2.tar.gz` & `tmp/exmol-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exmol-3.0.2.tar", last modified: Mon Mar 13 11:06:44 2023, max compression
+gzip compressed data, was "exmol-3.0.3.tar", last modified: Mon Jun 19 20:56:16 2023, max compression
```

## Comparing `exmol-3.0.2.tar` & `exmol-3.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 11:06:44.962741 exmol-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-13 11:02:24.000000 exmol-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-13 11:02:24.000000 exmol-3.0.2/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-03-13 11:06:44.962741 exmol-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-03-13 11:02:24.000000 exmol-3.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 11:06:44.942742 exmol-3.0.2/exmol/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-13 11:02:24.000000 exmol-3.0.2/exmol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-13 11:02:24.000000 exmol-3.0.2/exmol/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    54787 2023-03-13 11:02:24.000000 exmol-3.0.2/exmol/exmol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 11:06:44.962741 exmol-3.0.2/exmol/lime_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-03-13 11:02:24.000000 exmol-3.0.2/exmol/lime_data/MACCSkeys.txt
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-13 11:02:24.000000 exmol-3.0.2/exmol/lime_data/atom_pols.txt
--rw-r--r--   0 runner    (1001) docker     (123) 23010050 2023-03-13 11:02:25.000000 exmol-3.0.2/exmol/lime_data/keys.pb
--rw-r--r--   0 runner    (1001) docker     (123)    27944 2023-03-13 11:02:25.000000 exmol-3.0.2/exmol/lime_data/smarts.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-03-13 11:02:25.000000 exmol-3.0.2/exmol/plot_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 11:06:44.962741 exmol-3.0.2/exmol/stoned/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-13 11:02:25.000000 exmol-3.0.2/exmol/stoned/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21841 2023-03-13 11:02:25.000000 exmol-3.0.2/exmol/stoned/stoned.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-13 11:02:25.000000 exmol-3.0.2/exmol/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 11:06:44.942742 exmol-3.0.2/exmol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-03-13 11:06:44.000000 exmol-3.0.2/exmol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-13 11:06:44.000000 exmol-3.0.2/exmol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 11:06:44.000000 exmol-3.0.2/exmol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-13 11:06:44.000000 exmol-3.0.2/exmol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-13 11:06:44.000000 exmol-3.0.2/exmol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 11:06:44.962741 exmol-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-03-13 11:02:25.000000 exmol-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 11:06:44.962741 exmol-3.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-03-13 11:02:25.000000 exmol-3.0.2/tests/test_exmol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-03-13 11:02:25.000000 exmol-3.0.2/tests/test_svg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:56:16.128290 exmol-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-19 20:51:27.000000 exmol-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-19 20:51:27.000000 exmol-3.0.3/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-06-19 20:56:16.128290 exmol-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-06-19 20:51:27.000000 exmol-3.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:56:16.100289 exmol-3.0.3/exmol/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-19 20:51:27.000000 exmol-3.0.3/exmol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-19 20:51:27.000000 exmol-3.0.3/exmol/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54787 2023-06-19 20:51:27.000000 exmol-3.0.3/exmol/exmol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:56:16.128290 exmol-3.0.3/exmol/lime_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-06-19 20:51:27.000000 exmol-3.0.3/exmol/lime_data/MACCSkeys.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-19 20:51:27.000000 exmol-3.0.3/exmol/lime_data/atom_pols.txt
+-rw-r--r--   0 runner    (1001) docker     (123) 23010050 2023-06-19 20:51:27.000000 exmol-3.0.3/exmol/lime_data/keys.pb
+-rw-r--r--   0 runner    (1001) docker     (123)    27944 2023-06-19 20:51:27.000000 exmol-3.0.3/exmol/lime_data/smarts.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-06-19 20:51:27.000000 exmol-3.0.3/exmol/plot_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:56:16.128290 exmol-3.0.3/exmol/stoned/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-19 20:51:27.000000 exmol-3.0.3/exmol/stoned/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21841 2023-06-19 20:51:27.000000 exmol-3.0.3/exmol/stoned/stoned.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-19 20:51:27.000000 exmol-3.0.3/exmol/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:56:16.104289 exmol-3.0.3/exmol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-06-19 20:56:16.000000 exmol-3.0.3/exmol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-19 20:56:16.000000 exmol-3.0.3/exmol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:56:16.000000 exmol-3.0.3/exmol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-19 20:56:16.000000 exmol-3.0.3/exmol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 20:56:16.000000 exmol-3.0.3/exmol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 20:56:16.128290 exmol-3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-19 20:51:28.000000 exmol-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:56:16.128290 exmol-3.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-06-19 20:51:28.000000 exmol-3.0.3/tests/test_exmol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-19 20:51:28.000000 exmol-3.0.3/tests/test_svg.py
```

### Comparing `exmol-3.0.2/LICENSE` & `exmol-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `exmol-3.0.2/PKG-INFO` & `exmol-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exmol
-Version: 3.0.2
+Version: 3.0.3
 Summary: Counterfactual generation with STONED SELFIES
 Home-page: https://ur-whitelab.github.io/exmol/
 Author: Aditi Seshadri, Geemi Wellawatte, Andrew White
 Author-email: andrew.white@rochester.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `exmol-3.0.2/README.md` & `exmol-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `exmol-3.0.2/exmol/data.py` & `exmol-3.0.3/exmol/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dataclasses import dataclass, asdict
+from dataclasses import dataclass, asdict, field
 from typing import Optional
 import numpy as np  # type: ignore
 
 
 @dataclass
 class Descriptors:
     """Molecular descriptors"""
@@ -30,15 +30,15 @@
     #: Tanimoto similarity relative to base
     similarity: float
     #: Output of model function
     yhat: float
     #: Index relative to other examples
     index: int
     #: PCA projected position from similarity
-    position: np.ndarray = np.array(None)
+    position: np.ndarray = field(default_factory=lambda: np.array(None))
     #: True if base
     is_origin: bool = False
     #: Index of cluster, can be -1 for no cluster
     cluster: int = 0
     #: Label for this example
     label: str = None  # type: ignore
     #: Descriptors for this example
```

### Comparing `exmol-3.0.2/exmol/exmol.py` & `exmol-3.0.3/exmol/exmol.py`

 * *Files identical despite different names*

### Comparing `exmol-3.0.2/exmol/lime_data/MACCSkeys.txt` & `exmol-3.0.3/exmol/lime_data/MACCSkeys.txt`

 * *Files identical despite different names*

### Comparing `exmol-3.0.2/exmol/lime_data/atom_pols.txt` & `exmol-3.0.3/exmol/lime_data/atom_pols.txt`

 * *Files identical despite different names*

### Comparing `exmol-3.0.2/exmol/lime_data/keys.pb` & `exmol-3.0.3/exmol/lime_data/keys.pb`

 * *Files identical despite different names*

### Comparing `exmol-3.0.2/exmol/lime_data/smarts.txt` & `exmol-3.0.3/exmol/lime_data/smarts.txt`

 * *Files identical despite different names*

### Comparing `exmol-3.0.2/exmol/plot_utils.py` & `exmol-3.0.3/exmol/plot_utils.py`

 * *Files identical despite different names*

### Comparing `exmol-3.0.2/exmol/stoned/stoned.py` & `exmol-3.0.3/exmol/stoned/stoned.py`

 * *Files identical despite different names*

### Comparing `exmol-3.0.2/exmol.egg-info/PKG-INFO` & `exmol-3.0.3/exmol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exmol
-Version: 3.0.2
+Version: 3.0.3
 Summary: Counterfactual generation with STONED SELFIES
 Home-page: https://ur-whitelab.github.io/exmol/
 Author: Aditi Seshadri, Geemi Wellawatte, Andrew White
 Author-email: andrew.white@rochester.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `exmol-3.0.2/setup.py` & `exmol-3.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `exmol-3.0.2/tests/test_exmol.py` & `exmol-3.0.3/tests/test_exmol.py`

 * *Files identical despite different names*

### Comparing `exmol-3.0.2/tests/test_svg.py` & `exmol-3.0.3/tests/test_svg.py`

 * *Files identical despite different names*

