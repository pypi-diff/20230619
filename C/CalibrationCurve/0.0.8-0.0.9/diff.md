# Comparing `tmp/CalibrationCurve-0.0.8.tar.gz` & `tmp/CalibrationCurve-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CalibrationCurve-0.0.8.tar", last modified: Mon Jun 19 08:50:45 2023, max compression
+gzip compressed data, was "CalibrationCurve-0.0.9.tar", last modified: Mon Jun 19 09:00:48 2023, max compression
```

## Comparing `CalibrationCurve-0.0.8.tar` & `CalibrationCurve-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-19 08:50:45.332981 CalibrationCurve-0.0.8/
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-19 08:50:45.332981 CalibrationCurve-0.0.8/CalibrationCurve/
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       22 2023-06-19 08:50:42.000000 CalibrationCurve-0.0.8/CalibrationCurve/__init__.py
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     3423 2023-06-19 08:50:42.000000 CalibrationCurve-0.0.8/CalibrationCurve/_modidx.py
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     3189 2023-06-19 08:50:42.000000 CalibrationCurve-0.0.8/CalibrationCurve/core.py
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-19 08:50:45.332981 CalibrationCurve-0.0.8/CalibrationCurve.egg-info/
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1090 2023-06-19 08:50:45.000000 CalibrationCurve-0.0.8/CalibrationCurve.egg-info/PKG-INFO
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      414 2023-06-19 08:50:45.000000 CalibrationCurve-0.0.8/CalibrationCurve.egg-info/SOURCES.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-19 08:50:45.000000 CalibrationCurve-0.0.8/CalibrationCurve.egg-info/dependency_links.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       54 2023-06-19 08:50:45.000000 CalibrationCurve-0.0.8/CalibrationCurve.egg-info/entry_points.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-12 05:51:02.000000 CalibrationCurve-0.0.8/CalibrationCurve.egg-info/not-zip-safe
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       66 2023-06-19 08:50:45.000000 CalibrationCurve-0.0.8/CalibrationCurve.egg-info/requires.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       17 2023-06-19 08:50:45.000000 CalibrationCurve-0.0.8/CalibrationCurve.egg-info/top_level.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)    11357 2023-06-12 05:47:40.000000 CalibrationCurve-0.0.8/LICENSE
--rw-rw-r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      111 2023-04-27 10:12:58.000000 CalibrationCurve-0.0.8/MANIFEST.in
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1090 2023-06-19 08:50:45.332981 CalibrationCurve-0.0.8/PKG-INFO
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      225 2023-06-19 08:49:07.000000 CalibrationCurve-0.0.8/README.md
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1002 2023-06-19 08:50:42.000000 CalibrationCurve-0.0.8/settings.ini
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       38 2023-06-19 08:50:45.332981 CalibrationCurve-0.0.8/setup.cfg
--rw-rw-r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2596 2023-04-27 10:12:58.000000 CalibrationCurve-0.0.8/setup.py
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-19 09:00:48.502841 CalibrationCurve-0.0.9/
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-19 09:00:48.502841 CalibrationCurve-0.0.9/CalibrationCurve/
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       22 2023-06-19 09:00:21.000000 CalibrationCurve-0.0.9/CalibrationCurve/__init__.py
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     3423 2023-06-19 09:00:21.000000 CalibrationCurve-0.0.9/CalibrationCurve/_modidx.py
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     3413 2023-06-19 09:00:21.000000 CalibrationCurve-0.0.9/CalibrationCurve/core.py
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-19 09:00:48.502841 CalibrationCurve-0.0.9/CalibrationCurve.egg-info/
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1090 2023-06-19 09:00:48.000000 CalibrationCurve-0.0.9/CalibrationCurve.egg-info/PKG-INFO
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      414 2023-06-19 09:00:48.000000 CalibrationCurve-0.0.9/CalibrationCurve.egg-info/SOURCES.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-19 09:00:48.000000 CalibrationCurve-0.0.9/CalibrationCurve.egg-info/dependency_links.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       54 2023-06-19 09:00:48.000000 CalibrationCurve-0.0.9/CalibrationCurve.egg-info/entry_points.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-12 05:51:02.000000 CalibrationCurve-0.0.9/CalibrationCurve.egg-info/not-zip-safe
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       66 2023-06-19 09:00:48.000000 CalibrationCurve-0.0.9/CalibrationCurve.egg-info/requires.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       17 2023-06-19 09:00:48.000000 CalibrationCurve-0.0.9/CalibrationCurve.egg-info/top_level.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)    11357 2023-06-12 05:47:40.000000 CalibrationCurve-0.0.9/LICENSE
+-rw-rw-r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      111 2023-04-27 10:12:58.000000 CalibrationCurve-0.0.9/MANIFEST.in
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1090 2023-06-19 09:00:48.502841 CalibrationCurve-0.0.9/PKG-INFO
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      225 2023-06-19 08:49:07.000000 CalibrationCurve-0.0.9/README.md
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1002 2023-06-19 09:00:21.000000 CalibrationCurve-0.0.9/settings.ini
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       38 2023-06-19 09:00:48.502841 CalibrationCurve-0.0.9/setup.cfg
+-rw-rw-r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2596 2023-04-27 10:12:58.000000 CalibrationCurve-0.0.9/setup.py
```

### Comparing `CalibrationCurve-0.0.8/CalibrationCurve/_modidx.py` & `CalibrationCurve-0.0.9/CalibrationCurve/_modidx.py`

 * *Files identical despite different names*

### Comparing `CalibrationCurve-0.0.8/CalibrationCurve/core.py` & `CalibrationCurve-0.0.9/CalibrationCurve/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% auto 0
 __all__ = ['CalibrationModel']
 
+# %% ../nbs/00_core.ipynb 3
+import pandas as pd
+import scipy as sp
+import matplotlib.pyplot as plt
+import numpy as np
+import seaborn as sns
+from dataclasses import dataclass
+# from scipy.stats import t
+import typing
+
+
 # %% ../nbs/00_core.ipynb 6
 class CalibrationModel:
 
     def __init__(self, x, y, test_replicates):
       
         self.x = x
         self.y = y
@@ -16,15 +27,15 @@
         self.std_err = None
         self.test_replicates = test_replicates
         self.cal_line_points = self.x.shape[0]
         self.df_resid = self.cal_line_points - 2
 
     def fit_ols(self):
 
-        self.slope, self.intercept, self.r_squared, self.std_err, _ = scipy.stats.linregress(self.x, self.y)
+        self.slope, self.intercept, self.r_squared, self.std_err, _ = sp.stats.linregress(self.x, self.y)
     
     def calculate_fitted_values(self):
         
         self.fitted_values = self.slope * self.x + self.intercept
 
    
     def inverse_prediction(self, unknown):
@@ -40,15 +51,15 @@
         self.calculate_fitted_values()
         return np.sum((self.fitted_values - self.y) **2)
     
     def calculate_syx(self):
         return np.sqrt((self.calculate_sse())/(len(self.x)-2))
 
     def get_t_value(self,alpha):
-        return t.ppf(1 - alpha/2, self.df_resid)
+        return sp.stats.t.ppf(1 - alpha/2, self.df_resid)
 
     def calculate_uncertainty(self):
         return self.calculate_sxhat() * self.get_t_value(0.05)
     
     def calculate_sxhat(self):
         return (self.calculate_syx() / self.slope) * np.sqrt( 1/ self.test_replicates + 1 / self.cal_line_points)
```

### Comparing `CalibrationCurve-0.0.8/CalibrationCurve.egg-info/PKG-INFO` & `CalibrationCurve-0.0.9/CalibrationCurve.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalibrationCurve
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of functions that streamline the process of creating calibration curves using Python.
 Home-page: https://github.com/Rhys-McAlister/CalibrationCurve
 Author: Rhys McAlister
 Author-email: mcalisterrhys@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CalibrationCurve-0.0.8/LICENSE` & `CalibrationCurve-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `CalibrationCurve-0.0.8/PKG-INFO` & `CalibrationCurve-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalibrationCurve
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of functions that streamline the process of creating calibration curves using Python.
 Home-page: https://github.com/Rhys-McAlister/CalibrationCurve
 Author: Rhys McAlister
 Author-email: mcalisterrhys@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CalibrationCurve-0.0.8/settings.ini` & `CalibrationCurve-0.0.9/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = CalibrationCurve
 lib_name = CalibrationCurve
-version = 0.0.8
+version = 0.0.9
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = CalibrationCurve
 nbs_path = nbs
 recursive = True
```

### Comparing `CalibrationCurve-0.0.8/setup.py` & `CalibrationCurve-0.0.9/setup.py`

 * *Files identical despite different names*

