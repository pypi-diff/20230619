# Comparing `tmp/prostate-nomograms-0.0.7.tar.gz` & `tmp/prostate-nomograms-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prostate-nomograms-0.0.7.tar", last modified: Mon Jun 19 16:08:08 2023, max compression
+gzip compressed data, was "prostate-nomograms-0.0.8.tar", last modified: Mon Jun 19 17:05:43 2023, max compression
```

## Comparing `prostate-nomograms-0.0.7.tar` & `prostate-nomograms-0.0.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 16:08:08.117614 prostate-nomograms-0.0.7/
--rw-rw-rw-   0        0        0    11549 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     3858 2023-06-19 16:08:08.116523 prostate-nomograms-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3248 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 16:08:08.092025 prostate-nomograms-0.0.7/examples/
--rw-rw-rw-   0        0        0        0 2023-05-03 22:40:34.000000 prostate-nomograms-0.0.7/examples/__init__.py
--rw-rw-rw-   0        0        0      150 2023-05-06 03:41:30.000000 prostate-nomograms-0.0.7/examples/env_examples.py
--rw-rw-rw-   0        0        0     3569 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/examples/ex01-mskcc.py
--rw-rw-rw-   0        0        0     4129 2023-06-17 14:21:21.000000 prostate-nomograms-0.0.7/examples/ex02-capra.py
--rw-rw-rw-   0        0        0     4210 2023-06-17 14:21:21.000000 prostate-nomograms-0.0.7/examples/ex03-custom.py
-drwxrwxrwx   0        0        0        0 2023-06-19 16:08:08.095659 prostate-nomograms-0.0.7/prostate_nomograms/
--rw-rw-rw-   0        0        0      465 2023-06-19 16:07:22.000000 prostate-nomograms-0.0.7/prostate_nomograms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 16:08:08.100658 prostate-nomograms-0.0.7/prostate_nomograms/capra/
--rw-rw-rw-   0        0        0       34 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/capra/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 16:08:08.105830 prostate-nomograms-0.0.7/prostate_nomograms/capra/base/
--rw-rw-rw-   0        0        0      106 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/capra/base/__init__.py
--rw-rw-rw-   0        0        0     1353 2023-06-19 16:06:39.000000 prostate-nomograms-0.0.7/prostate_nomograms/capra/base/logistic_regression.py
--rw-rw-rw-   0        0        0     2273 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/capra/base/survival_regression.py
--rw-rw-rw-   0        0        0    12184 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/capra/capra.py
-drwxrwxrwx   0        0        0        0 2023-06-19 16:08:08.106845 prostate-nomograms-0.0.7/prostate_nomograms/custom/
--rw-rw-rw-   0        0        0       36 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/custom/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 16:08:08.110319 prostate-nomograms-0.0.7/prostate_nomograms/custom/base/
--rw-rw-rw-   0        0        0      106 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/custom/base/__init__.py
--rw-rw-rw-   0        0        0     1299 2023-06-19 16:06:39.000000 prostate-nomograms-0.0.7/prostate_nomograms/custom/base/logistic_regression.py
--rw-rw-rw-   0        0        0     2192 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/custom/base/survival_regression.py
--rw-rw-rw-   0        0        0     7179 2023-06-17 14:21:21.000000 prostate-nomograms-0.0.7/prostate_nomograms/custom/custom.py
--rw-rw-rw-   0        0        0     1162 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/enum.py
-drwxrwxrwx   0        0        0        0 2023-06-19 16:08:08.111806 prostate-nomograms-0.0.7/prostate_nomograms/mskcc/
--rw-rw-rw-   0        0        0       86 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/mskcc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 16:08:08.115355 prostate-nomograms-0.0.7/prostate_nomograms/mskcc/base/
--rw-rw-rw-   0        0        0       26 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/mskcc/base/__init__.py
--rw-rw-rw-   0        0        0     9792 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/mskcc/base/logistic_regression.py
--rw-rw-rw-   0        0        0    10577 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/mskcc/base/model.py
--rw-rw-rw-   0        0        0     2533 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/mskcc/base/survival_regression.py
--rw-rw-rw-   0        0        0     5490 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/mskcc/base/web_table_scraper.py
--rw-rw-rw-   0        0        0     2841 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/mskcc/pre_radical_prostatectomy_nomogram.py
-drwxrwxrwx   0        0        0        0 2023-06-19 16:08:08.099666 prostate-nomograms-0.0.7/prostate_nomograms.egg-info/
--rw-rw-rw-   0        0        0     3858 2023-06-19 16:08:08.000000 prostate-nomograms-0.0.7/prostate_nomograms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1191 2023-06-19 16:08:08.000000 prostate-nomograms-0.0.7/prostate_nomograms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 16:08:08.000000 prostate-nomograms-0.0.7/prostate_nomograms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-06-19 16:08:08.000000 prostate-nomograms-0.0.7/prostate_nomograms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-06-19 16:08:08.000000 prostate-nomograms-0.0.7/prostate_nomograms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 16:08:08.117614 prostate-nomograms-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-06-19 16:07:22.000000 prostate-nomograms-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:05:43.361402 prostate-nomograms-0.0.8/
+-rw-rw-rw-   0        0        0    11549 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     3858 2023-06-19 17:05:43.361402 prostate-nomograms-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3248 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 17:05:43.336913 prostate-nomograms-0.0.8/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-03 22:40:34.000000 prostate-nomograms-0.0.8/examples/__init__.py
+-rw-rw-rw-   0        0        0      150 2023-05-06 03:41:30.000000 prostate-nomograms-0.0.8/examples/env_examples.py
+-rw-rw-rw-   0        0        0     3569 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.8/examples/ex01-mskcc.py
+-rw-rw-rw-   0        0        0     4129 2023-06-17 14:21:21.000000 prostate-nomograms-0.0.8/examples/ex02-capra.py
+-rw-rw-rw-   0        0        0     4210 2023-06-17 14:21:21.000000 prostate-nomograms-0.0.8/examples/ex03-custom.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:05:43.339921 prostate-nomograms-0.0.8/prostate_nomograms/
+-rw-rw-rw-   0        0        0      465 2023-06-19 17:05:08.000000 prostate-nomograms-0.0.8/prostate_nomograms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:05:43.347655 prostate-nomograms-0.0.8/prostate_nomograms/capra/
+-rw-rw-rw-   0        0        0       34 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.8/prostate_nomograms/capra/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:05:43.350658 prostate-nomograms-0.0.8/prostate_nomograms/capra/base/
+-rw-rw-rw-   0        0        0      106 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.8/prostate_nomograms/capra/base/__init__.py
+-rw-rw-rw-   0        0        0     1353 2023-06-19 16:06:39.000000 prostate-nomograms-0.0.8/prostate_nomograms/capra/base/logistic_regression.py
+-rw-rw-rw-   0        0        0     2273 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.8/prostate_nomograms/capra/base/survival_regression.py
+-rw-rw-rw-   0        0        0    12184 2023-06-19 17:03:14.000000 prostate-nomograms-0.0.8/prostate_nomograms/capra/capra.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:05:43.352654 prostate-nomograms-0.0.8/prostate_nomograms/custom/
+-rw-rw-rw-   0        0        0       36 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.8/prostate_nomograms/custom/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:05:43.355032 prostate-nomograms-0.0.8/prostate_nomograms/custom/base/
+-rw-rw-rw-   0        0        0      106 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.8/prostate_nomograms/custom/base/__init__.py
+-rw-rw-rw-   0        0        0     1299 2023-06-19 16:06:39.000000 prostate-nomograms-0.0.8/prostate_nomograms/custom/base/logistic_regression.py
+-rw-rw-rw-   0        0        0     2192 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.8/prostate_nomograms/custom/base/survival_regression.py
+-rw-rw-rw-   0        0        0     7439 2023-06-19 17:03:05.000000 prostate-nomograms-0.0.8/prostate_nomograms/custom/custom.py
+-rw-rw-rw-   0        0        0     1162 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.8/prostate_nomograms/enum.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:05:43.357032 prostate-nomograms-0.0.8/prostate_nomograms/mskcc/
+-rw-rw-rw-   0        0        0       86 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.8/prostate_nomograms/mskcc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:05:43.360417 prostate-nomograms-0.0.8/prostate_nomograms/mskcc/base/
+-rw-rw-rw-   0        0        0       26 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.8/prostate_nomograms/mskcc/base/__init__.py
+-rw-rw-rw-   0        0        0     9792 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.8/prostate_nomograms/mskcc/base/logistic_regression.py
+-rw-rw-rw-   0        0        0    10577 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.8/prostate_nomograms/mskcc/base/model.py
+-rw-rw-rw-   0        0        0     2533 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.8/prostate_nomograms/mskcc/base/survival_regression.py
+-rw-rw-rw-   0        0        0     5490 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.8/prostate_nomograms/mskcc/base/web_table_scraper.py
+-rw-rw-rw-   0        0        0     2841 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.8/prostate_nomograms/mskcc/pre_radical_prostatectomy_nomogram.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:05:43.344574 prostate-nomograms-0.0.8/prostate_nomograms.egg-info/
+-rw-rw-rw-   0        0        0     3858 2023-06-19 17:05:43.000000 prostate-nomograms-0.0.8/prostate_nomograms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1191 2023-06-19 17:05:43.000000 prostate-nomograms-0.0.8/prostate_nomograms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 17:05:43.000000 prostate-nomograms-0.0.8/prostate_nomograms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-06-19 17:05:43.000000 prostate-nomograms-0.0.8/prostate_nomograms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-06-19 17:05:43.000000 prostate-nomograms-0.0.8/prostate_nomograms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 17:05:43.361402 prostate-nomograms-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2023-06-19 17:05:08.000000 prostate-nomograms-0.0.8/setup.py
```

### Comparing `prostate-nomograms-0.0.7/LICENSE` & `prostate-nomograms-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.7/PKG-INFO` & `prostate-nomograms-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prostate-nomograms
-Version: 0.0.7
+Version: 0.0.8
 Summary: Prediction tools based on existing prostate cancer nomograms.
 Home-page: https://github.com/MaxenceLarose/prostate-nomograms
 Author: Maxence Larose
 Author-email: maxence.larose.1@ulaval.ca
 License: Apache License 2.0
 Keywords: cancer medical nomogram prediction prostate python3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prostate-nomograms-0.0.7/README.md` & `prostate-nomograms-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.7/examples/ex01-mskcc.py` & `prostate-nomograms-0.0.8/examples/ex01-mskcc.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.7/examples/ex02-capra.py` & `prostate-nomograms-0.0.8/examples/ex02-capra.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.7/examples/ex03-custom.py` & `prostate-nomograms-0.0.8/examples/ex03-custom.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.7/prostate_nomograms/capra/base/logistic_regression.py` & `prostate-nomograms-0.0.8/prostate_nomograms/capra/base/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.7/prostate_nomograms/capra/base/survival_regression.py` & `prostate-nomograms-0.0.8/prostate_nomograms/capra/base/survival_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.7/prostate_nomograms/capra/capra.py` & `prostate-nomograms-0.0.8/prostate_nomograms/capra/capra.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.7/prostate_nomograms/custom/base/logistic_regression.py` & `prostate-nomograms-0.0.8/prostate_nomograms/custom/base/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.7/prostate_nomograms/custom/base/survival_regression.py` & `prostate-nomograms-0.0.8/prostate_nomograms/custom/base/survival_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.7/prostate_nomograms/custom/custom.py` & `prostate-nomograms-0.0.8/prostate_nomograms/custom/custom.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import List, Optional, Union
 
 import pandas as pd
 import numpy as np
+from sklearn.preprocessing import StandardScaler
 
 from ..enum import ClassificationOutcome, SurvivalOutcome
 from .base import LogisticRegression, SurvivalRegression
 
 
 class CustomNomogram:
     """
@@ -46,15 +47,17 @@
         else:
             raise ValueError(f"Invalid outcome: {outcome}")
 
         self.target_column_name = target_column_name
         self.event_indicator_column_name = event_indicator_column_name
         self.event_time_column_name = event_time_column_name
         self.features_column_names = features_column_names
+
         self._is_fitted = False
+        self._scaler = StandardScaler()
 
         if self.model_type == "survival":
             assert self.event_indicator_column_name is not None, (
                 "Event indicator column name must be specified for survival models."
             )
             assert self.event_time_column_name is not None, (
                 "Event time column name must be specified for survival models."
@@ -138,14 +141,15 @@
 
         Parameters
         ----------
         dataset : pd.DataFrame
             Dataframe containing the data of the patients.
         """
         features = self.get_features(dataset)
+        features = self._scaler.fit_transform(features)
         if self.model_type == "survival":
             self.regressor.fit(
                 features,
                 np.array(dataset[self.event_indicator_column_name], dtype=bool),
                 np.array(dataset[self.event_time_column_name], dtype=float)
             )
         else:
@@ -175,14 +179,15 @@
         -------
         predictions : numpy.ndarray
             The predictions.
         """
         assert self._is_fitted, "Model must be fitted first."
 
         features = self.get_features(dataframe)
+        features = self._scaler.transform(features)
         if self.model_type == "survival":
             if number_of_months is None:
                 raise ValueError("Number of months must be given.")
             else:
                 return self.regressor.get_predicted_survival_probability(features, number_of_months)
         elif self.model_type == "logistic":
             return self.regressor.get_predicted_probability(features)
@@ -204,12 +209,13 @@
         Returns
         -------
         predictions : numpy.ndarray
             The predictions.
         """
         if self.model_type == "survival":
             features = self.get_features(dataframe)
+            features = self._scaler.transform(features)
             return self.regressor.get_predicted_risk(features)
         elif self.model_type == "logistic":
             raise ValueError("Logistic models don't have risk predictions.")
         else:
             raise ValueError(f"Model type {self.model_type} doesn't exist.")
```

### Comparing `prostate-nomograms-0.0.7/prostate_nomograms/enum.py` & `prostate-nomograms-0.0.8/prostate_nomograms/enum.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.7/prostate_nomograms/mskcc/base/logistic_regression.py` & `prostate-nomograms-0.0.8/prostate_nomograms/mskcc/base/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.7/prostate_nomograms/mskcc/base/model.py` & `prostate-nomograms-0.0.8/prostate_nomograms/mskcc/base/model.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.7/prostate_nomograms/mskcc/base/survival_regression.py` & `prostate-nomograms-0.0.8/prostate_nomograms/mskcc/base/survival_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.7/prostate_nomograms/mskcc/base/web_table_scraper.py` & `prostate-nomograms-0.0.8/prostate_nomograms/mskcc/base/web_table_scraper.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.7/prostate_nomograms/mskcc/pre_radical_prostatectomy_nomogram.py` & `prostate-nomograms-0.0.8/prostate_nomograms/mskcc/pre_radical_prostatectomy_nomogram.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.7/prostate_nomograms.egg-info/PKG-INFO` & `prostate-nomograms-0.0.8/prostate_nomograms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prostate-nomograms
-Version: 0.0.7
+Version: 0.0.8
 Summary: Prediction tools based on existing prostate cancer nomograms.
 Home-page: https://github.com/MaxenceLarose/prostate-nomograms
 Author: Maxence Larose
 Author-email: maxence.larose.1@ulaval.ca
 License: Apache License 2.0
 Keywords: cancer medical nomogram prediction prostate python3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prostate-nomograms-0.0.7/prostate_nomograms.egg-info/SOURCES.txt` & `prostate-nomograms-0.0.8/prostate_nomograms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.7/setup.py` & `prostate-nomograms-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="prostate-nomograms",
-    version="0.0.7",
+    version="0.0.8",
     author="Maxence Larose",
     author_email="maxence.larose.1@ulaval.ca",
     description="Prediction tools based on existing prostate cancer nomograms.",
     long_description=open('README.md', "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/MaxenceLarose/prostate-nomograms",
     license="Apache License 2.0",
```

