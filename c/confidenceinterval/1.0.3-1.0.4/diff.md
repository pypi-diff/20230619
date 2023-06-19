# Comparing `tmp/confidenceinterval-1.0.3.tar.gz` & `tmp/confidenceinterval-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confidenceinterval-1.0.3.tar", last modified: Sun Jun 11 08:34:43 2023, max compression
+gzip compressed data, was "confidenceinterval-1.0.4.tar", last modified: Mon Jun 19 03:09:16 2023, max compression
```

## Comparing `confidenceinterval-1.0.3.tar` & `confidenceinterval-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-06-11 08:34:43.958030 confidenceinterval-1.0.3/
--rw-r--r--   0 gildenbj   (501) staff       (20)     1072 2023-03-11 16:10:01.000000 confidenceinterval-1.0.3/LICENSE
--rw-r--r--   0 gildenbj   (501) staff       (20)       48 2023-04-19 15:52:18.000000 confidenceinterval-1.0.3/MANIFEST.in
--rw-r--r--   0 gildenbj   (501) staff       (20)     8165 2023-06-11 08:34:43.958216 confidenceinterval-1.0.3/PKG-INFO
--rw-r--r--   0 gildenbj   (501) staff       (20)     7626 2023-06-11 04:08:57.000000 confidenceinterval-1.0.3/README.md
-drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-06-11 08:34:43.955500 confidenceinterval-1.0.3/confidenceinterval/
--rw-r--r--   0 gildenbj   (501) staff       (20)      365 2023-06-10 10:27:57.000000 confidenceinterval-1.0.3/confidenceinterval/__init__.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     1666 2023-06-10 11:51:15.000000 confidenceinterval-1.0.3/confidenceinterval/auc.py
--rw-r--r--   0 gildenbj   (501) staff       (20)    17608 2023-06-11 08:32:15.000000 confidenceinterval-1.0.3/confidenceinterval/binary_metrics.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     1422 2023-06-11 08:33:05.000000 confidenceinterval-1.0.3/confidenceinterval/bootstrap.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     7130 2023-03-11 16:36:30.000000 confidenceinterval-1.0.3/confidenceinterval/delong.py
--rw-r--r--   0 gildenbj   (501) staff       (20)    25708 2023-06-11 08:34:03.000000 confidenceinterval-1.0.3/confidenceinterval/takahashi_methods.py
--rw-r--r--   0 gildenbj   (501) staff       (20)      895 2023-03-11 15:07:46.000000 confidenceinterval-1.0.3/confidenceinterval/utils.py
-drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-06-11 08:34:43.957631 confidenceinterval-1.0.3/confidenceinterval.egg-info/
--rw-r--r--   0 gildenbj   (501) staff       (20)     8165 2023-06-11 08:34:43.000000 confidenceinterval-1.0.3/confidenceinterval.egg-info/PKG-INFO
--rw-r--r--   0 gildenbj   (501) staff       (20)      497 2023-06-11 08:34:43.000000 confidenceinterval-1.0.3/confidenceinterval.egg-info/SOURCES.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)        1 2023-06-11 08:34:43.000000 confidenceinterval-1.0.3/confidenceinterval.egg-info/dependency_links.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)       55 2023-06-11 08:34:43.000000 confidenceinterval-1.0.3/confidenceinterval.egg-info/requires.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)       19 2023-06-11 08:34:43.000000 confidenceinterval-1.0.3/confidenceinterval.egg-info/top_level.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)       54 2023-06-11 08:34:14.000000 confidenceinterval-1.0.3/requirements.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)      613 2023-06-11 08:34:43.958819 confidenceinterval-1.0.3/setup.cfg
--rw-r--r--   0 gildenbj   (501) staff       (20)      870 2023-06-11 08:30:40.000000 confidenceinterval-1.0.3/setup.py
+drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-06-19 03:09:16.522462 confidenceinterval-1.0.4/
+-rw-r--r--   0 gildenbj   (501) staff       (20)     1072 2023-03-11 16:10:01.000000 confidenceinterval-1.0.4/LICENSE
+-rw-r--r--   0 gildenbj   (501) staff       (20)       48 2023-04-19 15:52:18.000000 confidenceinterval-1.0.4/MANIFEST.in
+-rw-r--r--   0 gildenbj   (501) staff       (20)     8342 2023-06-19 03:09:16.522757 confidenceinterval-1.0.4/PKG-INFO
+-rw-r--r--   0 gildenbj   (501) staff       (20)     7803 2023-06-11 14:36:31.000000 confidenceinterval-1.0.4/README.md
+drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-06-19 03:09:16.519086 confidenceinterval-1.0.4/confidenceinterval/
+-rw-r--r--   0 gildenbj   (501) staff       (20)      365 2023-06-10 10:27:57.000000 confidenceinterval-1.0.4/confidenceinterval/__init__.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)     1666 2023-06-19 03:07:55.000000 confidenceinterval-1.0.4/confidenceinterval/auc.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)    17421 2023-06-19 03:08:08.000000 confidenceinterval-1.0.4/confidenceinterval/binary_metrics.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)     1422 2023-06-19 03:07:30.000000 confidenceinterval-1.0.4/confidenceinterval/bootstrap.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)     7130 2023-03-11 16:36:30.000000 confidenceinterval-1.0.4/confidenceinterval/delong.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)    25596 2023-06-19 03:05:50.000000 confidenceinterval-1.0.4/confidenceinterval/takahashi_methods.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)      895 2023-06-19 03:08:07.000000 confidenceinterval-1.0.4/confidenceinterval/utils.py
+drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-06-19 03:09:16.521907 confidenceinterval-1.0.4/confidenceinterval.egg-info/
+-rw-r--r--   0 gildenbj   (501) staff       (20)     8342 2023-06-19 03:09:16.000000 confidenceinterval-1.0.4/confidenceinterval.egg-info/PKG-INFO
+-rw-r--r--   0 gildenbj   (501) staff       (20)      497 2023-06-19 03:09:16.000000 confidenceinterval-1.0.4/confidenceinterval.egg-info/SOURCES.txt
+-rw-r--r--   0 gildenbj   (501) staff       (20)        1 2023-06-19 03:09:16.000000 confidenceinterval-1.0.4/confidenceinterval.egg-info/dependency_links.txt
+-rw-r--r--   0 gildenbj   (501) staff       (20)       37 2023-06-19 03:09:16.000000 confidenceinterval-1.0.4/confidenceinterval.egg-info/requires.txt
+-rw-r--r--   0 gildenbj   (501) staff       (20)       19 2023-06-19 03:09:16.000000 confidenceinterval-1.0.4/confidenceinterval.egg-info/top_level.txt
+-rw-r--r--   0 gildenbj   (501) staff       (20)       36 2023-06-19 03:07:49.000000 confidenceinterval-1.0.4/requirements.txt
+-rw-r--r--   0 gildenbj   (501) staff       (20)      613 2023-06-19 03:09:16.523705 confidenceinterval-1.0.4/setup.cfg
+-rw-r--r--   0 gildenbj   (501) staff       (20)      870 2023-06-19 03:09:13.000000 confidenceinterval-1.0.4/setup.py
```

### Comparing `confidenceinterval-1.0.3/LICENSE` & `confidenceinterval-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.3/PKG-INFO` & `confidenceinterval-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: confidenceinterval
-Version: 1.0.3
+Version: 1.0.4
 Summary: Confidence Intervals in python
 Home-page: https://github.com/jacobgil/confidenceinterval
 Author: Jacob Gildenblat
 Author-email: jacob.gildenblat@gmail.com
 Project-URL: Bug Tracker, https://github.com/jacobgil/confidenceinterval/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # The long missing python library for confidence intervals
+![logo](logo.png)
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![Build Status](https://github.com/jacobgil/confidenceinterval/workflows/Tests/badge.svg)
 [![Downloads](https://static.pepy.tech/personalized-badge/confidenceinterval?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=Monthly%20Downloads)](https://pepy.tech/project/confidenceinterval)
 [![Downloads](https://static.pepy.tech/personalized-badge/confidenceinterval?period=total&units=international_system&left_color=black&right_color=blue&left_text=Total%20Downloads)](https://pepy.tech/project/confidenceinterval)
 
 `pip install confidenceinterval`
@@ -57,16 +58,28 @@
                                 ppv_score,
                                 npv_score,
                                 tpr_score,
                                 fpr_score,
                                 tnr_score
 from confidenceinterval.bootstrap import bootstrap_ci
 
-# Example usage:
-auc, ci = roc_auc_score(y_true, y_pred, confidence_level=0.95, method='bootstrap_bca', n_resamples=5000)
+
+# Analytic CI:
+auc, ci = roc_auc_score(y_true,
+                        y_pred,
+                        confidence_level=0.95)
+# Bootstrap CI:
+auc, ci = roc_auc_score(y_true,
+                        y_pred,
+                        confidence_level=0.95,
+                        method='bootstrap_bca',
+                        n_resamples=5000)
+
+
+
 ```
 
 ## All methods do an analytical computation by default, but can do bootsrapping instead
 By default all the methods return an analytical computation of the confidence interval (CI).
 
 For a bootstrap computation of the CI for any of the methods belonw, just specify method='bootstrap_bca', or method='bootstrap_percentile' or method='bootstrap_basic'.
 These are different ways of doing the bootstrapping, but method='bootstrap_bca' is the generalibly reccomended method.
@@ -74,29 +87,27 @@
 You can also pass the number of bootstrap resamples (n_resamples), and a random generator for controling the reproducability:
 
 ```python
 random_state = np.random.default_rng()
 n_resamples=9999
 ```
 
-## Support for binary, macro and micro averagin for F1, Precision and Recall.
+## Support for binary, macro and micro averaging for F1, Precision and Recall.
 ```python
 from confidence interval import precision_score, recall_score, f1_score
 binary_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='binary')
 macro_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='macro')
 micro_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='micro')
 bootstrap_binary_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='binary', method='bootstrap_bca', n_resamples=5000)
 
 ```
 
-These methods also accept average='micro' or average='macro', or 'binary'.
-
 The analytical computation here is using the (amazing) 2022 paper of Takahashi et al (reference below).
-
-The paper derived recall and precision only for micro. We derive the recall and precision confidence intervals for macro F1 as well using the delta method.
+The paper derived recall and precision only for micro averaging.
+We derive the recall and precision confidence intervals for macro F1 as well using the delta method.
 
 
 ## ROC AUC
 ```python
 from confidence interval import roc_auc_score
 ```
 The analytical computation here is a fast implementation of the DeLong method.
```

### Comparing `confidenceinterval-1.0.3/README.md` & `confidenceinterval-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # The long missing python library for confidence intervals
+![logo](logo.png)
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![Build Status](https://github.com/jacobgil/confidenceinterval/workflows/Tests/badge.svg)
 [![Downloads](https://static.pepy.tech/personalized-badge/confidenceinterval?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=Monthly%20Downloads)](https://pepy.tech/project/confidenceinterval)
 [![Downloads](https://static.pepy.tech/personalized-badge/confidenceinterval?period=total&units=international_system&left_color=black&right_color=blue&left_text=Total%20Downloads)](https://pepy.tech/project/confidenceinterval)
 
 `pip install confidenceinterval`
@@ -42,16 +43,28 @@
                                 ppv_score,
                                 npv_score,
                                 tpr_score,
                                 fpr_score,
                                 tnr_score
 from confidenceinterval.bootstrap import bootstrap_ci
 
-# Example usage:
-auc, ci = roc_auc_score(y_true, y_pred, confidence_level=0.95, method='bootstrap_bca', n_resamples=5000)
+
+# Analytic CI:
+auc, ci = roc_auc_score(y_true,
+                        y_pred,
+                        confidence_level=0.95)
+# Bootstrap CI:
+auc, ci = roc_auc_score(y_true,
+                        y_pred,
+                        confidence_level=0.95,
+                        method='bootstrap_bca',
+                        n_resamples=5000)
+
+
+
 ```
 
 ## All methods do an analytical computation by default, but can do bootsrapping instead
 By default all the methods return an analytical computation of the confidence interval (CI).
 
 For a bootstrap computation of the CI for any of the methods belonw, just specify method='bootstrap_bca', or method='bootstrap_percentile' or method='bootstrap_basic'.
 These are different ways of doing the bootstrapping, but method='bootstrap_bca' is the generalibly reccomended method.
@@ -59,29 +72,27 @@
 You can also pass the number of bootstrap resamples (n_resamples), and a random generator for controling the reproducability:
 
 ```python
 random_state = np.random.default_rng()
 n_resamples=9999
 ```
 
-## Support for binary, macro and micro averagin for F1, Precision and Recall.
+## Support for binary, macro and micro averaging for F1, Precision and Recall.
 ```python
 from confidence interval import precision_score, recall_score, f1_score
 binary_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='binary')
 macro_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='macro')
 micro_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='micro')
 bootstrap_binary_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='binary', method='bootstrap_bca', n_resamples=5000)
 
 ```
 
-These methods also accept average='micro' or average='macro', or 'binary'.
-
 The analytical computation here is using the (amazing) 2022 paper of Takahashi et al (reference below).
-
-The paper derived recall and precision only for micro. We derive the recall and precision confidence intervals for macro F1 as well using the delta method.
+The paper derived recall and precision only for micro averaging.
+We derive the recall and precision confidence intervals for macro F1 as well using the delta method.
 
 
 ## ROC AUC
 ```python
 from confidence interval import roc_auc_score
 ```
 The analytical computation here is a fast implementation of the DeLong method.
```

### Comparing `confidenceinterval-1.0.3/confidenceinterval/auc.py` & `confidenceinterval-1.0.4/confidenceinterval/auc.py`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.3/confidenceinterval/binary_metrics.py` & `confidenceinterval-1.0.4/confidenceinterval/binary_metrics.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """ Confidence intervals for common binary metrics."""
 
 from ast import Call
 import statsmodels
 from statsmodels.stats.proportion import proportion_confint
 from typing import List, Callable, Tuple, Union, Optional
-from typing_extensions import Unpack
 from functools import partial
 import numpy as np
 from confidenceinterval.utils import get_positive_negative_counts
 from confidenceinterval.bootstrap import bootstrap_ci, bootstrap_methods, BootstrapParams
 
 proportion_conf_methods: List[str] = [
     'wilson',
@@ -109,15 +108,15 @@
 
 
 def accuracy_score(y_true: List[int],
                    y_pred: List[int],
                    confidence_level: float = 0.95,
                    method: str = 'wilson',
                    compute_ci: bool = True,
-                   **kwargs: Unpack[BootstrapParams]) -> Union[float, Tuple[float, Tuple[float, float]]]:
+                   **kwargs) -> Union[float, Tuple[float, Tuple[float, float]]]:
     """
         Compute the accuracy score and optionally the confidence interval.
         Parameters
         ----------
         y_true : List[int]
             The grount truth labels.
         y_pred : List[int]
@@ -184,15 +183,15 @@
 
 
 def ppv_score(y_true: List[int],
               y_pred: List[int],
               confidence_level: float = 0.95,
               method: str = 'wilson',
               compute_ci: bool = True,
-              **kwargs: Unpack[BootstrapParams]) -> Union[float, Tuple[float, Tuple[float, float]]]:
+              **kwargs) -> Union[float, Tuple[float, Tuple[float, float]]]:
     if method in bootstrap_methods:
         return ppv_score_bootstrap(
             y_true, y_pred, confidence_level, method, **kwargs)
     else:
         return ppv_score_binomial_ci(
             y_true, y_pred, confidence_level, method, compute_ci)
 
@@ -239,15 +238,15 @@
 
 
 def npv_score(y_true: List[int],
               y_pred: List[int],
               confidence_level: float = 0.95,
               method: str = 'wilson',
               compute_ci: bool = True,
-              **kwargs: Unpack[BootstrapParams]) -> Union[float, Tuple[float, Tuple[float, float]]]:
+              **kwargs) -> Union[float, Tuple[float, Tuple[float, float]]]:
     if method in bootstrap_methods:
         return npv_score_bootstrap(
             y_true, y_pred, confidence_level, method, **kwargs)
     else:
         return npv_score_binomial_ci(
             y_true, y_pred, confidence_level, method, compute_ci)
 
@@ -294,15 +293,15 @@
 
 
 def tpr_score(y_true: List[int],
               y_pred: List[int],
               confidence_level: float = 0.95,
               method: str = 'wilson',
               compute_ci: bool = True,
-              **kwargs: Unpack[BootstrapParams]) -> Union[float, Tuple[float, Tuple[float, float]]]:
+              **kwargs) -> Union[float, Tuple[float, Tuple[float, float]]]:
     if method in bootstrap_methods:
         return tpr_score_bootstrap(
             y_true, y_pred, confidence_level, method, **kwargs)
     else:
         return tpr_score_binomial_ci(
             y_true, y_pred, confidence_level, method, compute_ci=compute_ci)
 
@@ -349,15 +348,15 @@
 
 
 def fpr_score(y_true: List[int],
               y_pred: List[int],
               confidence_level: float = 0.95,
               method: str = 'wilson',
               compute_ci: bool = True,
-              **kwargs: Unpack[BootstrapParams]) -> Union[float, Tuple[float, Tuple[float, float]]]:
+              **kwargs) -> Union[float, Tuple[float, Tuple[float, float]]]:
     if method in bootstrap_methods:
         return fpr_score_bootstrap(
             y_true=y_true, y_pred=y_pred, confidence_level=confidence_level, method=method, **kwargs)
     else:
         return fpr_score_binomial_ci(
             y_true=y_true, y_pred=y_pred, confidence_level=confidence_level, method=method, compute_ci=compute_ci)
 
@@ -404,14 +403,14 @@
 
 
 def tnr_score(y_true: List[int],
               y_pred: List[int],
               confidence_level: float = 0.95,
               method: str = 'wilson',
               compute_ci: bool = True,
-              **kwargs: Unpack[BootstrapParams]) -> Union[float, Tuple[float, Tuple[float, float]]]:
+              **kwargs) -> Union[float, Tuple[float, Tuple[float, float]]]:
     if method in bootstrap_methods:
         return tnr_score_bootstrap(
             y_true=y_true, y_pred=y_pred, confidence_level=confidence_level, method=method, **kwargs)
     else:
         return tnr_score_binomial_ci(
             y_true=y_true, y_pred=y_pred, confidence_level=confidence_level, method=method, compute_ci=compute_ci)
```

### Comparing `confidenceinterval-1.0.3/confidenceinterval/bootstrap.py` & `confidenceinterval-1.0.4/confidenceinterval/bootstrap.py`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.3/confidenceinterval/delong.py` & `confidenceinterval-1.0.4/confidenceinterval/delong.py`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.3/confidenceinterval/takahashi_methods.py` & `confidenceinterval-1.0.4/confidenceinterval/takahashi_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """ Confidence intervals for the F1, precision and recall scores, based on the Takahashi paper.
     https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8936911/#APP1
 """
 
 from typing import List, Callable, Tuple, Union, Optional
-from typing_extensions import Unpack
 
 from functools import partial
 import numpy as np
 from scipy.stats import norm
 from confidenceinterval.utils import get_positive_negative_counts
 from confidenceinterval.bootstrap import bootstrap_ci, bootstrap_methods, BootstrapParams
 from confidenceinterval.binary_metrics import tpr_score, ppv_score
@@ -159,15 +158,15 @@
 
 def precision_score(y_true: List[int],
                     y_pred: List[int],
                     confidence_level: float = 0.95,
                     average: str = 'micro',
                     method: str = 'takahashi',
                     compute_ci: bool = True,
-                    **kwargs: Unpack[BootstrapParams]) -> Union[float, Tuple[float, Tuple[float, float]]]:
+                    **kwargs) -> Union[float, Tuple[float, Tuple[float, float]]]:
     """Return the precision score. Supports micro/binary precision methods.
 
     Parameters
     ----------
     y_true : List[int]
         The ground truth labels.
     y_pred : List[int]
@@ -342,15 +341,15 @@
 
 def recall_score(y_true: List[int],
                  y_pred: List[int],
                  confidence_level: float = 0.95,
                  average: str = 'micro',
                  method: str = 'takahashi',
                  compute_ci: bool = True,
-                 **kwargs: Unpack[BootstrapParams]) -> Union[float, Tuple[float, Tuple[float, float]]]:
+                 **kwargs) -> Union[float, Tuple[float, Tuple[float, float]]]:
     """Return the precision score. Supports micro/binary precision methods.
 
     Parameters
     ----------
     y_true : List[int]
         The ground truth labels.
     y_pred : List[int]
@@ -568,15 +567,15 @@
 
 def f1_score(y_true: List[int],
              y_pred: List[int],
              confidence_level: float = 0.95,
              average: str = 'micro',
              method: str = 'takahashi',
              compute_ci: bool = True,
-             **kwargs: Unpack[BootstrapParams]) -> Union[float, Tuple[float, Tuple[float, float]]]:
+             **kwargs) -> Union[float, Tuple[float, Tuple[float, float]]]:
     """Compute the F1 score and optionally the confidence interval.
     For non bootstrapping methods, the micro and macro F1 averaging modes, this following the method described in the paper:
     https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8936911/
     For the binary F1 averaging mode, the confidence interval is computed using a derivation made by us in the spirit of the paper above,
     using the delta method and the derivatives of F1 score with respect to the 2x2 confusion matrix parameters.
 
     Parameters
```

### Comparing `confidenceinterval-1.0.3/confidenceinterval/utils.py` & `confidenceinterval-1.0.4/confidenceinterval/utils.py`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.3/confidenceinterval.egg-info/PKG-INFO` & `confidenceinterval-1.0.4/confidenceinterval.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: confidenceinterval
-Version: 1.0.3
+Version: 1.0.4
 Summary: Confidence Intervals in python
 Home-page: https://github.com/jacobgil/confidenceinterval
 Author: Jacob Gildenblat
 Author-email: jacob.gildenblat@gmail.com
 Project-URL: Bug Tracker, https://github.com/jacobgil/confidenceinterval/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # The long missing python library for confidence intervals
+![logo](logo.png)
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![Build Status](https://github.com/jacobgil/confidenceinterval/workflows/Tests/badge.svg)
 [![Downloads](https://static.pepy.tech/personalized-badge/confidenceinterval?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=Monthly%20Downloads)](https://pepy.tech/project/confidenceinterval)
 [![Downloads](https://static.pepy.tech/personalized-badge/confidenceinterval?period=total&units=international_system&left_color=black&right_color=blue&left_text=Total%20Downloads)](https://pepy.tech/project/confidenceinterval)
 
 `pip install confidenceinterval`
@@ -57,16 +58,28 @@
                                 ppv_score,
                                 npv_score,
                                 tpr_score,
                                 fpr_score,
                                 tnr_score
 from confidenceinterval.bootstrap import bootstrap_ci
 
-# Example usage:
-auc, ci = roc_auc_score(y_true, y_pred, confidence_level=0.95, method='bootstrap_bca', n_resamples=5000)
+
+# Analytic CI:
+auc, ci = roc_auc_score(y_true,
+                        y_pred,
+                        confidence_level=0.95)
+# Bootstrap CI:
+auc, ci = roc_auc_score(y_true,
+                        y_pred,
+                        confidence_level=0.95,
+                        method='bootstrap_bca',
+                        n_resamples=5000)
+
+
+
 ```
 
 ## All methods do an analytical computation by default, but can do bootsrapping instead
 By default all the methods return an analytical computation of the confidence interval (CI).
 
 For a bootstrap computation of the CI for any of the methods belonw, just specify method='bootstrap_bca', or method='bootstrap_percentile' or method='bootstrap_basic'.
 These are different ways of doing the bootstrapping, but method='bootstrap_bca' is the generalibly reccomended method.
@@ -74,29 +87,27 @@
 You can also pass the number of bootstrap resamples (n_resamples), and a random generator for controling the reproducability:
 
 ```python
 random_state = np.random.default_rng()
 n_resamples=9999
 ```
 
-## Support for binary, macro and micro averagin for F1, Precision and Recall.
+## Support for binary, macro and micro averaging for F1, Precision and Recall.
 ```python
 from confidence interval import precision_score, recall_score, f1_score
 binary_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='binary')
 macro_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='macro')
 micro_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='micro')
 bootstrap_binary_f1, ci = f1_score(y_true, y_pred, confidence_interval=0.95, average='binary', method='bootstrap_bca', n_resamples=5000)
 
 ```
 
-These methods also accept average='micro' or average='macro', or 'binary'.
-
 The analytical computation here is using the (amazing) 2022 paper of Takahashi et al (reference below).
-
-The paper derived recall and precision only for micro. We derive the recall and precision confidence intervals for macro F1 as well using the delta method.
+The paper derived recall and precision only for micro averaging.
+We derive the recall and precision confidence intervals for macro F1 as well using the delta method.
 
 
 ## ROC AUC
 ```python
 from confidence interval import roc_auc_score
 ```
 The analytical computation here is a fast implementation of the DeLong method.
```

### Comparing `confidenceinterval-1.0.3/setup.cfg` & `confidenceinterval-1.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.3/setup.py` & `confidenceinterval-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.readlines()
 
 setuptools.setup(
     name='confidenceinterval',
-    version='1.0.3',
+    version='1.0.4',
     author='Jacob Gildenblat',
     author_email='jacob.gildenblat@gmail.com',
     description='Confidence Intervals in python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/jacobgil/confidenceinterval',
     project_urls={
```

