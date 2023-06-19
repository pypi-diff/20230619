# Comparing `tmp/prostate-nomograms-0.0.6.tar.gz` & `tmp/prostate-nomograms-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prostate-nomograms-0.0.6.tar", last modified: Mon Jun 19 15:19:49 2023, max compression
+gzip compressed data, was "prostate-nomograms-0.0.7.tar", last modified: Mon Jun 19 16:08:08 2023, max compression
```

## Comparing `prostate-nomograms-0.0.6.tar` & `prostate-nomograms-0.0.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 15:19:49.928906 prostate-nomograms-0.0.6/
--rw-rw-rw-   0        0        0    11549 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     3858 2023-06-19 15:19:49.927906 prostate-nomograms-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3248 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 15:19:49.884771 prostate-nomograms-0.0.6/examples/
--rw-rw-rw-   0        0        0        0 2023-05-03 22:40:34.000000 prostate-nomograms-0.0.6/examples/__init__.py
--rw-rw-rw-   0        0        0      150 2023-05-06 03:41:30.000000 prostate-nomograms-0.0.6/examples/env_examples.py
--rw-rw-rw-   0        0        0     3569 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/examples/ex01-mskcc.py
--rw-rw-rw-   0        0        0     4129 2023-06-17 14:21:21.000000 prostate-nomograms-0.0.6/examples/ex02-capra.py
--rw-rw-rw-   0        0        0     4210 2023-06-17 14:21:21.000000 prostate-nomograms-0.0.6/examples/ex03-custom.py
-drwxrwxrwx   0        0        0        0 2023-06-19 15:19:49.889589 prostate-nomograms-0.0.6/prostate_nomograms/
--rw-rw-rw-   0        0        0      465 2023-06-19 15:17:01.000000 prostate-nomograms-0.0.6/prostate_nomograms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 15:19:49.897087 prostate-nomograms-0.0.6/prostate_nomograms/capra/
--rw-rw-rw-   0        0        0       34 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/capra/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 15:19:49.903732 prostate-nomograms-0.0.6/prostate_nomograms/capra/base/
--rw-rw-rw-   0        0        0      106 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/capra/base/__init__.py
--rw-rw-rw-   0        0        0     1336 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/capra/base/logistic_regression.py
--rw-rw-rw-   0        0        0     2273 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/capra/base/survival_regression.py
--rw-rw-rw-   0        0        0    12184 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/capra/capra.py
-drwxrwxrwx   0        0        0        0 2023-06-19 15:19:49.907891 prostate-nomograms-0.0.6/prostate_nomograms/custom/
--rw-rw-rw-   0        0        0       36 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/custom/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 15:19:49.914048 prostate-nomograms-0.0.6/prostate_nomograms/custom/base/
--rw-rw-rw-   0        0        0      106 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/custom/base/__init__.py
--rw-rw-rw-   0        0        0     1282 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/custom/base/logistic_regression.py
--rw-rw-rw-   0        0        0     2192 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/custom/base/survival_regression.py
--rw-rw-rw-   0        0        0     7179 2023-06-17 14:21:21.000000 prostate-nomograms-0.0.6/prostate_nomograms/custom/custom.py
--rw-rw-rw-   0        0        0     1162 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/enum.py
-drwxrwxrwx   0        0        0        0 2023-06-19 15:19:49.917561 prostate-nomograms-0.0.6/prostate_nomograms/mskcc/
--rw-rw-rw-   0        0        0       86 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/mskcc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 15:19:49.927906 prostate-nomograms-0.0.6/prostate_nomograms/mskcc/base/
--rw-rw-rw-   0        0        0       26 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/mskcc/base/__init__.py
--rw-rw-rw-   0        0        0     9792 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/mskcc/base/logistic_regression.py
--rw-rw-rw-   0        0        0    10577 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/mskcc/base/model.py
--rw-rw-rw-   0        0        0     2533 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/mskcc/base/survival_regression.py
--rw-rw-rw-   0        0        0     5490 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/mskcc/base/web_table_scraper.py
--rw-rw-rw-   0        0        0     2841 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.6/prostate_nomograms/mskcc/pre_radical_prostatectomy_nomogram.py
-drwxrwxrwx   0        0        0        0 2023-06-19 15:19:49.893063 prostate-nomograms-0.0.6/prostate_nomograms.egg-info/
--rw-rw-rw-   0        0        0     3858 2023-06-19 15:19:49.000000 prostate-nomograms-0.0.6/prostate_nomograms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1191 2023-06-19 15:19:49.000000 prostate-nomograms-0.0.6/prostate_nomograms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 15:19:49.000000 prostate-nomograms-0.0.6/prostate_nomograms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-06-19 15:19:49.000000 prostate-nomograms-0.0.6/prostate_nomograms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-06-19 15:19:49.000000 prostate-nomograms-0.0.6/prostate_nomograms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 15:19:49.928906 prostate-nomograms-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-06-19 15:16:49.000000 prostate-nomograms-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:08:08.117614 prostate-nomograms-0.0.7/
+-rw-rw-rw-   0        0        0    11549 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3858 2023-06-19 16:08:08.116523 prostate-nomograms-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3248 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 16:08:08.092025 prostate-nomograms-0.0.7/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-03 22:40:34.000000 prostate-nomograms-0.0.7/examples/__init__.py
+-rw-rw-rw-   0        0        0      150 2023-05-06 03:41:30.000000 prostate-nomograms-0.0.7/examples/env_examples.py
+-rw-rw-rw-   0        0        0     3569 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/examples/ex01-mskcc.py
+-rw-rw-rw-   0        0        0     4129 2023-06-17 14:21:21.000000 prostate-nomograms-0.0.7/examples/ex02-capra.py
+-rw-rw-rw-   0        0        0     4210 2023-06-17 14:21:21.000000 prostate-nomograms-0.0.7/examples/ex03-custom.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:08:08.095659 prostate-nomograms-0.0.7/prostate_nomograms/
+-rw-rw-rw-   0        0        0      465 2023-06-19 16:07:22.000000 prostate-nomograms-0.0.7/prostate_nomograms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:08:08.100658 prostate-nomograms-0.0.7/prostate_nomograms/capra/
+-rw-rw-rw-   0        0        0       34 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/capra/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:08:08.105830 prostate-nomograms-0.0.7/prostate_nomograms/capra/base/
+-rw-rw-rw-   0        0        0      106 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/capra/base/__init__.py
+-rw-rw-rw-   0        0        0     1353 2023-06-19 16:06:39.000000 prostate-nomograms-0.0.7/prostate_nomograms/capra/base/logistic_regression.py
+-rw-rw-rw-   0        0        0     2273 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/capra/base/survival_regression.py
+-rw-rw-rw-   0        0        0    12184 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/capra/capra.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:08:08.106845 prostate-nomograms-0.0.7/prostate_nomograms/custom/
+-rw-rw-rw-   0        0        0       36 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/custom/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:08:08.110319 prostate-nomograms-0.0.7/prostate_nomograms/custom/base/
+-rw-rw-rw-   0        0        0      106 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/custom/base/__init__.py
+-rw-rw-rw-   0        0        0     1299 2023-06-19 16:06:39.000000 prostate-nomograms-0.0.7/prostate_nomograms/custom/base/logistic_regression.py
+-rw-rw-rw-   0        0        0     2192 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/custom/base/survival_regression.py
+-rw-rw-rw-   0        0        0     7179 2023-06-17 14:21:21.000000 prostate-nomograms-0.0.7/prostate_nomograms/custom/custom.py
+-rw-rw-rw-   0        0        0     1162 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/enum.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:08:08.111806 prostate-nomograms-0.0.7/prostate_nomograms/mskcc/
+-rw-rw-rw-   0        0        0       86 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/mskcc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:08:08.115355 prostate-nomograms-0.0.7/prostate_nomograms/mskcc/base/
+-rw-rw-rw-   0        0        0       26 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/mskcc/base/__init__.py
+-rw-rw-rw-   0        0        0     9792 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/mskcc/base/logistic_regression.py
+-rw-rw-rw-   0        0        0    10577 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/mskcc/base/model.py
+-rw-rw-rw-   0        0        0     2533 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/mskcc/base/survival_regression.py
+-rw-rw-rw-   0        0        0     5490 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/mskcc/base/web_table_scraper.py
+-rw-rw-rw-   0        0        0     2841 2023-06-17 14:00:00.000000 prostate-nomograms-0.0.7/prostate_nomograms/mskcc/pre_radical_prostatectomy_nomogram.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:08:08.099666 prostate-nomograms-0.0.7/prostate_nomograms.egg-info/
+-rw-rw-rw-   0        0        0     3858 2023-06-19 16:08:08.000000 prostate-nomograms-0.0.7/prostate_nomograms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1191 2023-06-19 16:08:08.000000 prostate-nomograms-0.0.7/prostate_nomograms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 16:08:08.000000 prostate-nomograms-0.0.7/prostate_nomograms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-06-19 16:08:08.000000 prostate-nomograms-0.0.7/prostate_nomograms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-06-19 16:08:08.000000 prostate-nomograms-0.0.7/prostate_nomograms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 16:08:08.117614 prostate-nomograms-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2023-06-19 16:07:22.000000 prostate-nomograms-0.0.7/setup.py
```

### Comparing `prostate-nomograms-0.0.6/LICENSE` & `prostate-nomograms-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.6/PKG-INFO` & `prostate-nomograms-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prostate-nomograms
-Version: 0.0.6
+Version: 0.0.7
 Summary: Prediction tools based on existing prostate cancer nomograms.
 Home-page: https://github.com/MaxenceLarose/prostate-nomograms
 Author: Maxence Larose
 Author-email: maxence.larose.1@ulaval.ca
 License: Apache License 2.0
 Keywords: cancer medical nomogram prediction prostate python3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prostate-nomograms-0.0.6/README.md` & `prostate-nomograms-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.6/examples/ex01-mskcc.py` & `prostate-nomograms-0.0.7/examples/ex01-mskcc.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.6/examples/ex02-capra.py` & `prostate-nomograms-0.0.7/examples/ex02-capra.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.6/examples/ex03-custom.py` & `prostate-nomograms-0.0.7/examples/ex03-custom.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.6/prostate_nomograms/capra/base/logistic_regression.py` & `prostate-nomograms-0.0.7/prostate_nomograms/capra/base/logistic_regression.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         Logistic regression.
 
         Parameters
         ----------
         random_state : int
             The random state.
         """
-        self.classifier = SklearnLogisticRegression(class_weight="balanced", random_state=random_state)
+        self.classifier = SklearnLogisticRegression(class_weight="balanced", random_state=random_state, max_iter=10_000)
 
     def fit(
             self,
             capra_score: np.ndarray,
             target: np.ndarray
     ):
         """
```

### Comparing `prostate-nomograms-0.0.6/prostate_nomograms/capra/base/survival_regression.py` & `prostate-nomograms-0.0.7/prostate_nomograms/capra/base/survival_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.6/prostate_nomograms/capra/capra.py` & `prostate-nomograms-0.0.7/prostate_nomograms/capra/capra.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.6/prostate_nomograms/custom/base/logistic_regression.py` & `prostate-nomograms-0.0.7/prostate_nomograms/custom/base/logistic_regression.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         Logistic regression.
 
         Parameters
         ----------
         random_state : int
             The random state.
         """
-        self.classifier = SklearnLogisticRegression(class_weight="balanced", random_state=random_state)
+        self.classifier = SklearnLogisticRegression(class_weight="balanced", random_state=random_state, max_iter=10_000)
 
     def fit(
             self,
             features: np.ndarray,
             target: np.ndarray
     ):
         """
```

### Comparing `prostate-nomograms-0.0.6/prostate_nomograms/custom/base/survival_regression.py` & `prostate-nomograms-0.0.7/prostate_nomograms/custom/base/survival_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.6/prostate_nomograms/custom/custom.py` & `prostate-nomograms-0.0.7/prostate_nomograms/custom/custom.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.6/prostate_nomograms/enum.py` & `prostate-nomograms-0.0.7/prostate_nomograms/enum.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.6/prostate_nomograms/mskcc/base/logistic_regression.py` & `prostate-nomograms-0.0.7/prostate_nomograms/mskcc/base/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.6/prostate_nomograms/mskcc/base/model.py` & `prostate-nomograms-0.0.7/prostate_nomograms/mskcc/base/model.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.6/prostate_nomograms/mskcc/base/survival_regression.py` & `prostate-nomograms-0.0.7/prostate_nomograms/mskcc/base/survival_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.6/prostate_nomograms/mskcc/base/web_table_scraper.py` & `prostate-nomograms-0.0.7/prostate_nomograms/mskcc/base/web_table_scraper.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.6/prostate_nomograms/mskcc/pre_radical_prostatectomy_nomogram.py` & `prostate-nomograms-0.0.7/prostate_nomograms/mskcc/pre_radical_prostatectomy_nomogram.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.6/prostate_nomograms.egg-info/PKG-INFO` & `prostate-nomograms-0.0.7/prostate_nomograms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prostate-nomograms
-Version: 0.0.6
+Version: 0.0.7
 Summary: Prediction tools based on existing prostate cancer nomograms.
 Home-page: https://github.com/MaxenceLarose/prostate-nomograms
 Author: Maxence Larose
 Author-email: maxence.larose.1@ulaval.ca
 License: Apache License 2.0
 Keywords: cancer medical nomogram prediction prostate python3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prostate-nomograms-0.0.6/prostate_nomograms.egg-info/SOURCES.txt` & `prostate-nomograms-0.0.7/prostate_nomograms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.6/setup.py` & `prostate-nomograms-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="prostate-nomograms",
-    version="0.0.6",
+    version="0.0.7",
     author="Maxence Larose",
     author_email="maxence.larose.1@ulaval.ca",
     description="Prediction tools based on existing prostate cancer nomograms.",
     long_description=open('README.md', "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/MaxenceLarose/prostate-nomograms",
     license="Apache License 2.0",
```

