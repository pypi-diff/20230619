# Comparing `tmp/adapt-0.4.2.tar.gz` & `tmp/adapt-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adapt-0.4.2.tar", last modified: Sat Sep 17 16:48:39 2022, max compression
+gzip compressed data, was "dist\adapt-0.4.3.tar", last modified: Mon Jun 19 06:52:40 2023, max compression
```

## Comparing `adapt-0.4.2.tar` & `adapt-0.4.3.tar`

### file list

```diff
@@ -1,54 +1,67 @@
-drwxrwxrwx   0        0        0        0 2022-09-17 16:48:39.794599 adapt-0.4.2/
--rw-rw-rw-   0        0        0     1316 2022-09-17 16:47:35.000000 adapt-0.4.2/LICENSE.txt
--rw-rw-rw-   0        0        0    16691 2022-09-17 16:48:39.797751 adapt-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0    16320 2022-09-17 16:47:35.000000 adapt-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2022-09-17 16:48:38.783822 adapt-0.4.2/adapt/
--rw-rw-rw-   0        0        0      396 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/__init__.py
--rw-rw-rw-   0        0        0    17573 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/_tree_utils.py
--rw-rw-rw-   0        0        0    62268 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/base.py
-drwxrwxrwx   0        0        0        0 2022-09-17 16:48:39.309967 adapt-0.4.2/adapt/feature_based/
--rw-rw-rw-   0        0        0      530 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/feature_based/__init__.py
--rw-rw-rw-   0        0        0    12245 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/feature_based/_adda.py
--rw-rw-rw-   0        0        0     7140 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/feature_based/_ccsa.py
--rw-rw-rw-   0        0        0    15741 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/feature_based/_cdan.py
--rw-rw-rw-   0        0        0     6059 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/feature_based/_coral.py
--rw-rw-rw-   0        0        0     6998 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/feature_based/_dann.py
--rw-rw-rw-   0        0        0     7581 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/feature_based/_deepcoral.py
--rw-rw-rw-   0        0        0     8375 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/feature_based/_fa.py
--rw-rw-rw-   0        0        0     8934 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/feature_based/_fmmd.py
--rw-rw-rw-   0        0        0    10994 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/feature_based/_mcd.py
--rw-rw-rw-   0        0        0     7970 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/feature_based/_mdd.py
--rw-rw-rw-   0        0        0     8557 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/feature_based/_pred.py
--rw-rw-rw-   0        0        0     4040 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/feature_based/_sa.py
--rw-rw-rw-   0        0        0     4970 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/feature_based/_tca.py
--rw-rw-rw-   0        0        0     7868 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/feature_based/_wdgrl.py
-drwxrwxrwx   0        0        0        0 2022-09-17 16:48:39.653206 adapt-0.4.2/adapt/instance_based/
--rw-rw-rw-   0        0        0      638 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/instance_based/__init__.py
--rw-rw-rw-   0        0        0     4063 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/instance_based/_balancedweighting.py
--rw-rw-rw-   0        0        0     7067 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/instance_based/_iwc.py
--rw-rw-rw-   0        0        0    13824 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/instance_based/_iwn.py
--rw-rw-rw-   0        0        0    20081 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/instance_based/_kliep.py
--rw-rw-rw-   0        0        0     8943 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/instance_based/_kmm.py
--rw-rw-rw-   0        0        0     4911 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/instance_based/_ldm.py
--rw-rw-rw-   0        0        0     6097 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/instance_based/_nearestneighborsweighting.py
--rw-rw-rw-   0        0        0    14518 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/instance_based/_rulsif.py
--rw-rw-rw-   0        0        0    37799 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/instance_based/_tradaboost.py
--rw-rw-rw-   0        0        0    13936 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/instance_based/_ulsif.py
--rw-rw-rw-   0        0        0     9429 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/instance_based/_wann.py
--rw-rw-rw-   0        0        0    18343 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/metrics.py
-drwxrwxrwx   0        0        0        0 2022-09-17 16:48:39.788805 adapt-0.4.2/adapt/parameter_based/
--rw-rw-rw-   0        0        0      520 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/parameter_based/__init__.py
--rw-rw-rw-   0        0        0     7887 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/parameter_based/_finetuning.py
--rw-rw-rw-   0        0        0     5458 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/parameter_based/_linint.py
--rw-rw-rw-   0        0        0    16272 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/parameter_based/_regular.py
--rw-rw-rw-   0        0        0    54504 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/parameter_based/_transfer_tree.py
--rw-rw-rw-   0        0        0    21435 2022-09-17 16:47:35.000000 adapt-0.4.2/adapt/utils.py
-drwxrwxrwx   0        0        0        0 2022-09-17 16:48:38.891424 adapt-0.4.2/adapt.egg-info/
--rw-rw-rw-   0        0        0    16691 2022-09-17 16:48:37.000000 adapt-0.4.2/adapt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1316 2022-09-17 16:48:37.000000 adapt-0.4.2/adapt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-17 16:48:37.000000 adapt-0.4.2/adapt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-17 16:48:37.000000 adapt-0.4.2/adapt.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       69 2022-09-17 16:48:37.000000 adapt-0.4.2/adapt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-09-17 16:48:37.000000 adapt-0.4.2/adapt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-09-17 16:48:39.803243 adapt-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0      747 2022-09-17 16:47:36.000000 adapt-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:40.000000 adapt-0.4.3/
+-rw-rw-rw-   0        0        0    18980 2023-06-19 06:52:40.000000 adapt-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0    16323 2023-06-19 06:51:47.000000 adapt-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:39.000000 adapt-0.4.3/adapt/
+-rw-rw-rw-   0        0        0      396 2022-01-19 21:14:19.000000 adapt-0.4.3/adapt/__init__.py
+-rw-rw-rw-   0        0        0    17573 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/_tree_utils.py
+-rw-rw-rw-   0        0        0    62346 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/base.py
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:39.000000 adapt-0.4.3/adapt/feature_based/
+-rw-rw-rw-   0        0        0      530 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/feature_based/__init__.py
+-rw-rw-rw-   0        0        0    12245 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/feature_based/_adda.py
+-rw-rw-rw-   0        0        0     7140 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/feature_based/_ccsa.py
+-rw-rw-rw-   0        0        0    15741 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/feature_based/_cdan.py
+-rw-rw-rw-   0        0        0     6059 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/feature_based/_coral.py
+-rw-rw-rw-   0        0        0     6998 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/feature_based/_dann.py
+-rw-rw-rw-   0        0        0     7581 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/feature_based/_deepcoral.py
+-rw-rw-rw-   0        0        0     8423 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/feature_based/_fa.py
+-rw-rw-rw-   0        0        0     8934 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/feature_based/_fmmd.py
+-rw-rw-rw-   0        0        0    10994 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/feature_based/_mcd.py
+-rw-rw-rw-   0        0        0     7970 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/feature_based/_mdd.py
+-rw-rw-rw-   0        0        0     8557 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/feature_based/_pred.py
+-rw-rw-rw-   0        0        0     4040 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/feature_based/_sa.py
+-rw-rw-rw-   0        0        0     4970 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/feature_based/_tca.py
+-rw-rw-rw-   0        0        0     7868 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/feature_based/_wdgrl.py
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:40.000000 adapt-0.4.3/adapt/instance_based/
+-rw-rw-rw-   0        0        0      638 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/instance_based/__init__.py
+-rw-rw-rw-   0        0        0     4063 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/instance_based/_balancedweighting.py
+-rw-rw-rw-   0        0        0     7067 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/instance_based/_iwc.py
+-rw-rw-rw-   0        0        0    13824 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/instance_based/_iwn.py
+-rw-rw-rw-   0        0        0    20091 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/instance_based/_kliep.py
+-rw-rw-rw-   0        0        0     8943 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/instance_based/_kmm.py
+-rw-rw-rw-   0        0        0     4911 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/instance_based/_ldm.py
+-rw-rw-rw-   0        0        0     6097 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/instance_based/_nearestneighborsweighting.py
+-rw-rw-rw-   0        0        0    14518 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/instance_based/_rulsif.py
+-rw-rw-rw-   0        0        0    37799 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/instance_based/_tradaboost.py
+-rw-rw-rw-   0        0        0    13936 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/instance_based/_ulsif.py
+-rw-rw-rw-   0        0        0     9429 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/instance_based/_wann.py
+-rw-rw-rw-   0        0        0    18343 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/metrics.py
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:40.000000 adapt-0.4.3/adapt/parameter_based/
+-rw-rw-rw-   0        0        0      750 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/parameter_based/__init__.py
+-rw-rw-rw-   0        0        0     7887 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/parameter_based/_finetuning.py
+-rw-rw-rw-   0        0        0     5458 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/parameter_based/_linint.py
+-rw-rw-rw-   0        0        0    23282 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/parameter_based/_regular.py
+-rw-rw-rw-   0        0        0    70563 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/parameter_based/_transfer_tree.py
+-rw-rw-rw-   0        0        0    21435 2023-06-19 06:51:47.000000 adapt-0.4.3/adapt/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:39.000000 adapt-0.4.3/adapt.egg-info/
+-rw-rw-rw-   0        0        0    18980 2023-06-19 06:52:38.000000 adapt-0.4.3/adapt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1560 2023-06-19 06:52:38.000000 adapt-0.4.3/adapt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 06:52:38.000000 adapt-0.4.3/adapt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-11-27 15:00:12.000000 adapt-0.4.3/adapt.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       71 2023-06-19 06:52:38.000000 adapt-0.4.3/adapt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 06:52:38.000000 adapt-0.4.3/adapt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-19 06:52:40.000000 adapt-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      749 2023-06-19 06:51:48.000000 adapt-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:40.000000 adapt-0.4.3/tests/
+-rw-rw-rw-   0        0        0       36 2021-11-26 11:25:15.000000 adapt-0.4.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     3223 2023-06-19 06:51:48.000000 adapt-0.4.3/tests/test_adda.py
+-rw-rw-rw-   0        0        0     4049 2023-06-19 06:51:48.000000 adapt-0.4.3/tests/test_cdan.py
+-rw-rw-rw-   0        0        0     3049 2023-06-19 06:51:48.000000 adapt-0.4.3/tests/test_coral.py
+-rw-rw-rw-   0        0        0     4597 2023-06-19 06:51:48.000000 adapt-0.4.3/tests/test_dann.py
+-rw-rw-rw-   0        0        0     5776 2023-06-19 06:51:48.000000 adapt-0.4.3/tests/test_kliep.py
+-rw-rw-rw-   0        0        0     2327 2023-06-19 06:51:48.000000 adapt-0.4.3/tests/test_kmm.py
+-rw-rw-rw-   0        0        0     2846 2023-06-19 06:51:48.000000 adapt-0.4.3/tests/test_mcd.py
+-rw-rw-rw-   0        0        0     3475 2023-06-19 06:51:48.000000 adapt-0.4.3/tests/test_mdd.py
+-rw-rw-rw-   0        0        0     8306 2023-06-19 06:51:48.000000 adapt-0.4.3/tests/test_regular.py
+-rw-rw-rw-   0        0        0     7858 2023-06-19 06:51:48.000000 adapt-0.4.3/tests/test_tradaboost.py
+-rw-rw-rw-   0        0        0    16636 2023-06-19 06:51:48.000000 adapt-0.4.3/tests/test_utils.py
+-rw-rw-rw-   0        0        0     2922 2023-06-19 06:51:48.000000 adapt-0.4.3/tests/test_wdgrl.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `adapt-0.4.2/PKG-INFO` & `adapt-0.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: adapt
-Version: 0.4.2
-Summary: Awesome Domain Adaptation Python Toolbox for Tensorflow and Scikit-learn
-Home-page: https://github.com/adapt-python/adapt.git
-Author: Antoine de Mathelin
-Author-email: antoine.demat@gmail.com
-License: BSD-2
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # ADAPT
 
 [![PyPI version](https://badge.fury.io/py/adapt.svg)](https://pypi.org/project/adapt)
 [![Build Status](https://github.com/adapt-python/adapt/workflows/build/badge.svg)](https://github.com/adapt-python/adapt/actions)
 [![Python Version](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8|%203.9-blue)](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8|%203.9-blue)
 [![Codecov Status](https://codecov.io/gh/adapt-python/adapt/branch/master/graph/badge.svg?token=IWQXMYGY2Q)](https://codecov.io/gh/adapt-python/adapt)
 
@@ -93,15 +81,15 @@
 
 Finally import the module in your python scripts with:
 
 ```python
 import adapt
 ```
 
-A simple example of usage is given in the [Qick-Start](#Quick-Start) below.
+A simple example of usage is given in the [Quick-Start](#Quick-Start) below.
 
 
 ## ADAPT Guideline
 
 The transfer learning methods implemented in ADAPT can be seen as scikit-learn "Meta-estimators" or tensorflow "Custom Model":
 
 <table>
@@ -165,32 +153,32 @@
 </td>
 </tr>
 </table>
 
 
 As you can see, the main difference between ADAPT models and scikit-learn and tensorflow objects is the two arguments `Xt, yt` which refer to the target data. Indeed, in classical machine learning, one assumes that the fitted model is applied on data distributed according to the training distribution. This is why, in this setting, one performs cross-validation and splits uniformly the training set to evaluate a model.
 
-In the transfer learning framework, however, one assumes that the target data (on which the model will be used at the end) are not distributed like the source training data. Moreover, one assumes that the target distribution can be estimated and compared to the training distribution. Either because a small sample of labeled target data `Xt, yt` is avalaible or because a large sample of unlabeled target data `Xt` is at one's disposal.
+In the transfer learning framework, however, one assumes that the target data (on which the model will be used at the end) are not distributed like the source training data. Moreover, one assumes that the target distribution can be estimated and compared to the training distribution. Either because a small sample of labeled target data `Xt, yt` is available or because a large sample of unlabeled target data `Xt` is at one's disposal.
 
 Thus, the transfer learning models from the ADAPT library can be seen as machine learning models that are fitted with a specific target in mind. This target is different but somewhat related to the training data. This is generally achieved by a transformation of the input features (see [feature-based transfer](https://adapt-python.github.io/adapt/contents.html#adapt-feature-based-feature-based-methods)) or by importance weighting (see [instance-based transfer](https://adapt-python.github.io/adapt/contents.html#adapt-instance-based)). In some cases, the training data are no more available but one aims at fine-tuning a pre-trained source model on a new target dataset (see [parameter-based transfer](https://adapt-python.github.io/adapt/contents.html#adapt-parameter-based)).
 
 
 ## Navigate into ADAPT
 
 The ADAPT library proposes numerous transfer algorithms and it can be hard to know which algorithm is best suited for a particular problem. If you do not know which algorithm to choose, this [flowchart](https://adapt-python.github.io/adapt/map.html) may help you:
 
 [<img src="https://github.com/adapt-python/adapt/raw/master/src_docs/_static/images/thumbnai_flowchart.PNG" width=30%>](https://adapt-python.github.io/adapt/map.html)
 
 
 ## Quick Start
 
-Here is a simple usage example of the ADAPT library. This is a simulation of a 1D sample bias problem with binary classfication task. The source input data are distributed according to a Gaussian distribution centered in -1 with standard deviation of 2. The target data are drawn from Gaussian distribution centered in 1 with standard deviation of 2. The output labels are equal to 1 in the interval [-1, 1] and 0 elsewhere. We apply the transfer method [KMM](https://adapt-python.github.io/adapt/generated/adapt.instance_based.KMM.html) which is an unsupervised instance-based algortihm.
+Here is a simple usage example of the ADAPT library. This is a simulation of a 1D sample bias problem with binary classification task. The source input data are distributed according to a Gaussian distribution centered in -1 with standard deviation of 2. The target data are drawn from Gaussian distribution centered in 1 with standard deviation of 2. The output labels are equal to 1 in the interval [-1, 1] and 0 elsewhere. We apply the transfer method [KMM](https://adapt-python.github.io/adapt/generated/adapt.instance_based.KMM.html) which is an unsupervised instance-based algorithm.
 
 ```python
-# Import standard librairies
+# Import standard libraries
 import numpy as np
 from sklearn.linear_model import LogisticRegression
 
 # Import KMM method form adapt.instance_based module
 from adapt.instance_based import KMM
 
 np.random.seed(0)
@@ -240,15 +228,15 @@
 
 ### Feature-based methods
 
 <img src="https://raw.githubusercontent.com/adapt-python/adapt/a490a5c4cefb80d6222bc831a8cc25b2f65221ce/docs/_static/images/feature_based.png">
 
 - [FA](https://adapt-python.github.io/adapt/generated/adapt.feature_based.FA.html) (*Frustratingly Easy Domain Adaptation*) [[paper]](https://arxiv.org/pdf/0907.1815.pdf)
 - [SA](https://adapt-python.github.io/adapt/generated/adapt.feature_based.SA.html) (*Subspace Alignment*) [[paper]](https://arxiv.org/abs/1409.5241)
-- [fMMD](https://adapt-python.github.io/adapt/generated/adapt.feature_based.SA.html) (*feature Selection with MMD*) [[paper]](https://www.cs.cmu.edu/afs/cs/Web/People/jgc/publication/Feature%20Selection%20for%20Transfer%20Learning.pdf)
+- [fMMD](https://adapt-python.github.io/adapt/generated/adapt.feature_based.fMMD.html) (*feature Selection with MMD*) [[paper]](https://www.cs.cmu.edu/afs/cs/Web/People/jgc/publication/Feature%20Selection%20for%20Transfer%20Learning.pdf)
 - [DANN](https://adapt-python.github.io/adapt/generated/adapt.feature_based.DANN.html) (*Discriminative Adversarial Neural Network*) [[paper]](https://jmlr.org/papers/volume17/15-239/15-239.pdf)
 - [ADDA](https://adapt-python.github.io/adapt/generated/adapt.feature_based.ADDA.html) (*Adversarial Discriminative Domain Adaptation*) [[paper]](https://arxiv.org/pdf/1702.05464.pdf)
 - [CORAL](https://adapt-python.github.io/adapt/generated/adapt.feature_based.CORAL.html) (*CORrelation ALignment*) [[paper]](https://arxiv.org/pdf/1511.05547.pdf)
 - [DeepCORAL](https://adapt-python.github.io/adapt/generated/adapt.feature_based.DeepCORAL.html) (*Deep CORrelation ALignment*) [[paper]](https://arxiv.org/pdf/1607.01719.pdf)
 - [MCD](https://adapt-python.github.io/adapt/generated/adapt.feature_based.MCD.html) (*Maximum Classifier Discrepancy*) [[paper]](https://arxiv.org/pdf/1712.02560.pdf)
 - [MDD](https://adapt-python.github.io/adapt/generated/adapt.feature_based.MDD.html) (*Margin Disparity Discrepancy*) [[paper]](https://arxiv.org/pdf/1904.05801.pdf)
 - [WDGRL](https://adapt-python.github.io/adapt/generated/adapt.feature_based.WDGRL.html) (*Wasserstein Distance Guided Representation Learning*) [[paper]](https://arxiv.org/pdf/1707.01217.pdf)
@@ -257,15 +245,15 @@
 
 ### Instance-based methods
 
 <img src="https://raw.githubusercontent.com/adapt-python/adapt/a490a5c4cefb80d6222bc831a8cc25b2f65221ce/docs/_static/images/instance_based.png">
 
 - [LDM](https://adapt-python.github.io/adapt/generated/adapt.instance_based.LDM.html) (*Linear Discrepancy Minimization*) [[paper]](https://arxiv.org/pdf/0902.3430.pdf)
 - [KMM](https://adapt-python.github.io/adapt/generated/adapt.instance_based.KMM.html) (*Kernel Mean Matching*) [[paper]](https://proceedings.neurips.cc/paper/2006/file/a2186aa7c086b46ad4e8bf81e2a3a19b-Paper.pdf)
-- [KLIEP](https://adapt-python.github.io/adapt/generated/adapt.instance_based.KLIEP.html) (*Kullbackâ€“Leibler Importance Estimation Procedure*) [[paper]](https://proceedings.neurips.cc/paper/2007/file/be83ab3ecd0db773eb2dc1b0a17836a1-Paper.pdf)
+- [KLIEP](https://adapt-python.github.io/adapt/generated/adapt.instance_based.KLIEP.html) (*Kullback–Leibler Importance Estimation Procedure*) [[paper]](https://proceedings.neurips.cc/paper/2007/file/be83ab3ecd0db773eb2dc1b0a17836a1-Paper.pdf)
 - [TrAdaBoost](https://adapt-python.github.io/adapt/generated/adapt.instance_based.TrAdaBoost.html) (*Transfer AdaBoost*) [[paper]](https://cse.hkust.edu.hk/~qyang/Docs/2007/tradaboost.pdf)
 - [TrAdaBoostR2](https://adapt-python.github.io/adapt/generated/adapt.instance_based.TrAdaBoostR2.html) (*Transfer AdaBoost for Regression*) [[paper]](https://www.cs.utexas.edu/~dpardoe/papers/ICML10.pdf)
 - [TwoStageTrAdaBoostR2](https://adapt-python.github.io/adapt/generated/adapt.instance_based.TwoStageTrAdaBoostR2.html) (*Two Stage Transfer AdaBoost for Regression*) [[paper]](https://www.cs.utexas.edu/~dpardoe/papers/ICML10.pdf)
 - [NearestNeighborsWeighting](https://adapt-python.github.io/adapt/generated/adapt.instance_based.NearestNeighborsWeighting.html) (*Nearest Neighbors Weighting*) [[paper]](https://arxiv.org/pdf/2102.02291.pdf)
 - [WANN](https://adapt-python.github.io/adapt/generated/adapt.instance_based.WANN.html) (*Weighting Adversarial Neural Network*) [[paper]](https://arxiv.org/pdf/2006.08251.pdf)
 
 ### Parameter-based methods
@@ -294,9 +282,7 @@
 ```
 
 ## Acknowledgement
 
 This work has been funded by Michelin and the Industrial Data Analytics and Machine Learning chair from ENS Paris-Saclay, Borelli center.
 
 [<img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/michelin.png" width=200px alt="Michelin">](https://www.michelin.com/) [<img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/idaml.jpg" width=200px alt="IDAML">](https://centreborelli.ens-paris-saclay.fr/fr/chaire-idaml) [<img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/borelli.jpg" alt="Centre Borelli" width=150px>](https://centreborelli.ens-paris-saclay.fr/fr)
-
-
```

#### html2text {}

```diff
@@ -1,29 +1,24 @@
-Metadata-Version: 2.1 Name: adapt Version: 0.4.2 Summary: Awesome Domain
-Adaptation Python Toolbox for Tensorflow and Scikit-learn Home-page: https://
-github.com/adapt-python/adapt.git Author: Antoine de Mathelin Author-email:
-antoine.demat@gmail.com License: BSD-2 Platform: UNKNOWN Description-Content-
-Type: text/markdown License-File: LICENSE.txt # ADAPT [![PyPI version](https://
-badge.fury.io/py/adapt.svg)](https://pypi.org/project/adapt) [![Build Status]
-(https://github.com/adapt-python/adapt/workflows/build/badge.svg)](https://
-github.com/adapt-python/adapt/actions) [![Python Version](https://
-img.shields.io/badge/python-3.6%20|%203.7%20|%203.8|%203.9-blue)](https://
-img.shields.io/badge/python-3.6%20|%203.7%20|%203.8|%203.9-blue) [![Codecov
-Status](https://codecov.io/gh/adapt-python/adapt/branch/master/graph/
-badge.svg?token=IWQXMYGY2Q)](https://codecov.io/gh/adapt-python/adapt)
-**A**wesome **D**omain **A**daptation **P**ython **T**oolbox --- ADAPT is an
-open source library providing numerous tools to perform Transfer Learning and
-Domain Adaptation. The purpose of the ADAPT library is to facilitate the access
-to transfer learning algorithms for a large public, including industrial
-players. ADAPT is specifically designed for [Scikit-learn](https://scikit-
-learn.org/stable/) and [Tensorflow](https://www.tensorflow.org/) users with a
-"user-friendly" approach. All objects in ADAPT implement the ***fit***,
-***predict*** and ***score*** methods like any scikit-learn object. A very
-detailed documentation with several examples is provided: :arrow_right:
-[Documentation](https://adapt-python.github.io/adapt/)
+# ADAPT [![PyPI version](https://badge.fury.io/py/adapt.svg)](https://pypi.org/
+project/adapt) [![Build Status](https://github.com/adapt-python/adapt/
+workflows/build/badge.svg)](https://github.com/adapt-python/adapt/actions) [!
+[Python Version](https://img.shields.io/badge/python-
+3.6%20|%203.7%20|%203.8|%203.9-blue)](https://img.shields.io/badge/python-
+3.6%20|%203.7%20|%203.8|%203.9-blue) [![Codecov Status](https://codecov.io/gh/
+adapt-python/adapt/branch/master/graph/badge.svg?token=IWQXMYGY2Q)](https://
+codecov.io/gh/adapt-python/adapt) **A**wesome **D**omain **A**daptation
+**P**ython **T**oolbox --- ADAPT is an open source library providing numerous
+tools to perform Transfer Learning and Domain Adaptation. The purpose of the
+ADAPT library is to facilitate the access to transfer learning algorithms for a
+large public, including industrial players. ADAPT is specifically designed for
+[Scikit-learn](https://scikit-learn.org/stable/) and [Tensorflow](https://
+www.tensorflow.org/) users with a "user-friendly" approach. All objects in
+ADAPT implement the ***fit***, ***predict*** and ***score*** methods like any
+scikit-learn object. A very detailed documentation with several examples is
+provided: :arrow_right: [Documentation](https://adapt-python.github.io/adapt/)
 
 Sample_bias_correction_                   Model-based_Transfer_
 
 [https://github.com/adapt-python/adapt/   [https://github.com/adapt-python/adapt/
 raw/                                      raw/
 41c13055facc0733faf49c4e3979709e82be10e5/ 41c13055facc0733faf49c4e3979709e82be10e5/
 docs/_static/images/                      docs/_static/images/finetuned.png]
@@ -39,17 +34,17 @@
 ## Installation and Usage This package is available on [Pypi](https://pypi.org/
 project/adapt) and can be installed with the following command line: ``` pip
 install adapt ``` The following dependencies are required and will be installed
 with the library: - `numpy` - `scipy` - `tensorflow` (>= 2.0) - `scikit-learn`
 - `cvxopt` If for some reason, these packages failed to install, you can do it
 manually with: ``` pip install numpy scipy tensorflow scikit-learn cvxopt ```
 Finally import the module in your python scripts with: ```python import adapt
-``` A simple example of usage is given in the [Qick-Start](#Quick-Start) below.
-## ADAPT Guideline The transfer learning methods implemented in ADAPT can be
-seen as scikit-learn "Meta-estimators" or tensorflow "Custom Model":
+``` A simple example of usage is given in the [Quick-Start](#Quick-Start)
+below. ## ADAPT Guideline The transfer learning methods implemented in ADAPT
+can be seen as scikit-learn "Meta-estimators" or tensorflow "Custom Model":
 
 Adapt Estimator            Deep Adapt Estimator       Scikit-learn Meta-
                                                       Estimator
 ```python AdaptEstimator   ```python
 ( estimator = """A scikit- DeepAdaptEstimator         ```python
 learn estimator (like      ( encoder = "A Tensorflow  SklearnMetaEstimator
 Ridge(alpha=1.) for        Model (if required)", task ( base_estimator = """A
@@ -71,15 +66,15 @@
 is applied on data distributed according to the training distribution. This is
 why, in this setting, one performs cross-validation and splits uniformly the
 training set to evaluate a model. In the transfer learning framework, however,
 one assumes that the target data (on which the model will be used at the end)
 are not distributed like the source training data. Moreover, one assumes that
 the target distribution can be estimated and compared to the training
 distribution. Either because a small sample of labeled target data `Xt, yt` is
-avalaible or because a large sample of unlabeled target data `Xt` is at one's
+available or because a large sample of unlabeled target data `Xt` is at one's
 disposal. Thus, the transfer learning models from the ADAPT library can be seen
 as machine learning models that are fitted with a specific target in mind. This
 target is different but somewhat related to the training data. This is
 generally achieved by a transformation of the input features (see [feature-
 based transfer](https://adapt-python.github.io/adapt/contents.html#adapt-
 feature-based-feature-based-methods)) or by importance weighting (see
 [instance-based transfer](https://adapt-python.github.io/adapt/
@@ -90,21 +85,21 @@
 library proposes numerous transfer algorithms and it can be hard to know which
 algorithm is best suited for a particular problem. If you do not know which
 algorithm to choose, this [flowchart](https://adapt-python.github.io/adapt/
 map.html) may help you: [[https://github.com/adapt-python/adapt/raw/master/
 src_docs/_static/images/thumbnai_flowchart.PNG]](https://adapt-
 python.github.io/adapt/map.html) ## Quick Start Here is a simple usage example
 of the ADAPT library. This is a simulation of a 1D sample bias problem with
-binary classfication task. The source input data are distributed according to a
-Gaussian distribution centered in -1 with standard deviation of 2. The target
+binary classification task. The source input data are distributed according to
+a Gaussian distribution centered in -1 with standard deviation of 2. The target
 data are drawn from Gaussian distribution centered in 1 with standard deviation
 of 2. The output labels are equal to 1 in the interval [-1, 1] and 0 elsewhere.
 We apply the transfer method [KMM](https://adapt-python.github.io/adapt/
 generated/adapt.instance_based.KMM.html) which is an unsupervised instance-
-based algortihm. ```python # Import standard librairies import numpy as np from
+based algorithm. ```python # Import standard libraries import numpy as np from
 sklearn.linear_model import LogisticRegression # Import KMM method form
 adapt.instance_based module from adapt.instance_based import KMM np.random.seed
 (0) # Create source dataset (Xs ~ N(-1, 2)) # ys = 1 for ys in [-1, 1] else, ys
 = 0 Xs = np.random.randn(1000, 1)*2-1 ys = (Xs[:, 0] > -1.) & (Xs[:, 0] < 1.) #
 Create target dataset (Xt ~ N(1, 2)), yt ~ ys Xt = np.random.randn(1000, 1)*2+1
 yt = (Xt[:, 0] > -1.) & (Xt[:, 0] < 1.) # Instantiate and fit a source only
 model for comparison src_only = LogisticRegression(penalty="none") src_only.fit
@@ -125,15 +120,15 @@
 methods: ### Feature-based methods [https://raw.githubusercontent.com/adapt-
 python/adapt/a490a5c4cefb80d6222bc831a8cc25b2f65221ce/docs/_static/images/
 feature_based.png] - [FA](https://adapt-python.github.io/adapt/generated/
 adapt.feature_based.FA.html) (*Frustratingly Easy Domain Adaptation*) [[paper]]
 (https://arxiv.org/pdf/0907.1815.pdf) - [SA](https://adapt-python.github.io/
 adapt/generated/adapt.feature_based.SA.html) (*Subspace Alignment*) [[paper]]
 (https://arxiv.org/abs/1409.5241) - [fMMD](https://adapt-python.github.io/
-adapt/generated/adapt.feature_based.SA.html) (*feature Selection with MMD*) [
+adapt/generated/adapt.feature_based.fMMD.html) (*feature Selection with MMD*) [
 [paper]](https://www.cs.cmu.edu/afs/cs/Web/People/jgc/publication/
 Feature%20Selection%20for%20Transfer%20Learning.pdf) - [DANN](https://adapt-
 python.github.io/adapt/generated/adapt.feature_based.DANN.html)
 (*Discriminative Adversarial Neural Network*) [[paper]](https://jmlr.org/
 papers/volume17/15-239/15-239.pdf) - [ADDA](https://adapt-python.github.io/
 adapt/generated/adapt.feature_based.ADDA.html) (*Adversarial Discriminative
 Domain Adaptation*) [[paper]](https://arxiv.org/pdf/1702.05464.pdf) - [CORAL]
@@ -159,15 +154,15 @@
 instance_based.png] - [LDM](https://adapt-python.github.io/adapt/generated/
 adapt.instance_based.LDM.html) (*Linear Discrepancy Minimization*) [[paper]]
 (https://arxiv.org/pdf/0902.3430.pdf) - [KMM](https://adapt-python.github.io/
 adapt/generated/adapt.instance_based.KMM.html) (*Kernel Mean Matching*) [
 [paper]](https://proceedings.neurips.cc/paper/2006/file/
 a2186aa7c086b46ad4e8bf81e2a3a19b-Paper.pdf) - [KLIEP](https://adapt-
 python.github.io/adapt/generated/adapt.instance_based.KLIEP.html)
-(*KullbackÃ¢â¬âLeibler Importance Estimation Procedure*) [[paper]](https://
+(*KullbackâLeibler Importance Estimation Procedure*) [[paper]](https://
 proceedings.neurips.cc/paper/2007/file/be83ab3ecd0db773eb2dc1b0a17836a1-
 Paper.pdf) - [TrAdaBoost](https://adapt-python.github.io/adapt/generated/
 adapt.instance_based.TrAdaBoost.html) (*Transfer AdaBoost*) [[paper]](https://
 cse.hkust.edu.hk/~qyang/Docs/2007/tradaboost.pdf) - [TrAdaBoostR2](https://
 adapt-python.github.io/adapt/generated/adapt.instance_based.TrAdaBoostR2.html)
 (*Transfer AdaBoost for Regression*) [[paper]](https://www.cs.utexas.edu/
 ~dpardoe/papers/ICML10.pdf) - [TwoStageTrAdaBoostR2](https://adapt-
```

### Comparing `adapt-0.4.2/README.md` & `adapt-0.4.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,288 +1,299 @@
-# ADAPT
-
-[![PyPI version](https://badge.fury.io/py/adapt.svg)](https://pypi.org/project/adapt)
-[![Build Status](https://github.com/adapt-python/adapt/workflows/build/badge.svg)](https://github.com/adapt-python/adapt/actions)
-[![Python Version](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8|%203.9-blue)](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8|%203.9-blue)
-[![Codecov Status](https://codecov.io/gh/adapt-python/adapt/branch/master/graph/badge.svg?token=IWQXMYGY2Q)](https://codecov.io/gh/adapt-python/adapt)
-
-**A**wesome **D**omain **A**daptation **P**ython **T**oolbox
-
----
-
-ADAPT is an open source library providing numerous tools to perform Transfer Learning and Domain Adaptation.
-
-The purpose of the ADAPT library is to facilitate the access to transfer learning algorithms for a large public, including industrial players. ADAPT is specifically designed for [Scikit-learn](https://scikit-learn.org/stable/) and [Tensorflow](https://www.tensorflow.org/) users with a "user-friendly" approach. All objects in ADAPT implement the ***fit***, ***predict*** and ***score*** methods like any scikit-learn object. A very detailed documentation with several examples is provided:
-
-:arrow_right: [Documentation](https://adapt-python.github.io/adapt/)
-
-<table>
-  <tr valign="top">
-    <td width="50%" >
-        <a href="https://adapt-python.github.io/adapt/examples/Sample_bias_example.html">
-            <br>
-            <b>Sample bias correction</b>
-            <br>
-            <br>
-            <img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/sample_bias_corr_img.png">
-        </a>
-    </td>
-    <td width="50%">
-        <a href="https://adapt-python.github.io/adapt/examples/Flowers_example.html">
-            <br>
-            <b>Model-based Transfer</b>
-            <br>
-            <br>
-            <img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/finetuned.png">
-        </a>
-    </td>
-  </tr>
-  <tr valign="top">
-    <td width="50%">
-        <a href="https://adapt-python.github.io/adapt/examples/Office_example.html">
-            <br>
-            <b>Deep Domain Adaptation</b>
-            <br>
-            <br>
-            <img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/office_item.png">
-        </a>
-    </td>
-    <td width="50%">
-        <a href="https://adapt-python.github.io/adapt/examples/Multi_fidelity.html">
-            <br>
-            <b>Multi-Fidelity Transfer</b>
-            <br>
-            <br>
-            <img src="https://raw.githubusercontent.com/adapt-python/adapt/a490a5c4cefb80d6222bc831a8cc25b2f65221ce/docs/_static/images/multifidelity_setup.png">
-        </a>
-    </td>
-  </tr>
-</table>
-
-## Installation and Usage
-
-This package is available on [Pypi](https://pypi.org/project/adapt) and can be installed with the following command line: 
-
-```
-pip install adapt
-```
-
-The following dependencies are required and will be installed with the library:
-- `numpy`
-- `scipy`
-- `tensorflow` (>= 2.0)
-- `scikit-learn`
-- `cvxopt`
-
-If for some reason, these packages failed to install, you can do it manually with:
-
-```
-pip install numpy scipy tensorflow scikit-learn cvxopt
-```
-
-Finally import the module in your python scripts with:
-
-```python
-import adapt
-```
-
-A simple example of usage is given in the [Qick-Start](#Quick-Start) below.
-
-
-## ADAPT Guideline
-
-The transfer learning methods implemented in ADAPT can be seen as scikit-learn "Meta-estimators" or tensorflow "Custom Model":
-
-<table>
-<tr valign="top">
-<td width="33%" >
-<br>
-<b>Adapt Estimator</b>
-<br>
-<br>
-	
-```python
-AdaptEstimator(
-	estimator = """A scikit-learn estimator
-	            (like Ridge(alpha=1.) for example)
-		    or a Tensorflow Model""",
-	Xt = "The target input features",
-	yt = "The target output labels (if any)",
-	**params = "Hyper-parameters of the AdaptEstimator"
-)
-```
-	
-<td width="33%">
-<br>
-<b>Deep Adapt Estimator</b>
-<br>
-<br>
-
-	
-```python
-DeepAdaptEstimator(
-	encoder = "A Tensorflow Model (if required)",
-	task = "A Tensorflow Model (if required)",
-	discriminator = "A Tensorflow Model (if required)",
-	Xt = "The target input features",
-	yt = "The target output labels (if any)",
-	**params = """Hyper-parameters of the DeepAdaptEstimator and
-		      the compile and fit params (optimizer, epochs...)"""
-)
-```
-	
-
-</td>
-	
-	
-</td>
-<td width="33%">
-<br>
-<b>Scikit-learn Meta-Estimator</b>
-<br>
-<br>
-	
-```python
-SklearnMetaEstimator(
-	base_estimator = """A scikit-learn estimator
-			 (like Ridge(alpha=1.) for example)""",
-	**params = "Hyper-parameters of the SklearnMetaEstimator"
-)
-```
-	
-
-</td>
-</tr>
-</table>
-
-
-As you can see, the main difference between ADAPT models and scikit-learn and tensorflow objects is the two arguments `Xt, yt` which refer to the target data. Indeed, in classical machine learning, one assumes that the fitted model is applied on data distributed according to the training distribution. This is why, in this setting, one performs cross-validation and splits uniformly the training set to evaluate a model.
-
-In the transfer learning framework, however, one assumes that the target data (on which the model will be used at the end) are not distributed like the source training data. Moreover, one assumes that the target distribution can be estimated and compared to the training distribution. Either because a small sample of labeled target data `Xt, yt` is avalaible or because a large sample of unlabeled target data `Xt` is at one's disposal.
-
-Thus, the transfer learning models from the ADAPT library can be seen as machine learning models that are fitted with a specific target in mind. This target is different but somewhat related to the training data. This is generally achieved by a transformation of the input features (see [feature-based transfer](https://adapt-python.github.io/adapt/contents.html#adapt-feature-based-feature-based-methods)) or by importance weighting (see [instance-based transfer](https://adapt-python.github.io/adapt/contents.html#adapt-instance-based)). In some cases, the training data are no more available but one aims at fine-tuning a pre-trained source model on a new target dataset (see [parameter-based transfer](https://adapt-python.github.io/adapt/contents.html#adapt-parameter-based)).
-
-
-## Navigate into ADAPT
-
-The ADAPT library proposes numerous transfer algorithms and it can be hard to know which algorithm is best suited for a particular problem. If you do not know which algorithm to choose, this [flowchart](https://adapt-python.github.io/adapt/map.html) may help you:
-
-[<img src="https://github.com/adapt-python/adapt/raw/master/src_docs/_static/images/thumbnai_flowchart.PNG" width=30%>](https://adapt-python.github.io/adapt/map.html)
-
-
-## Quick Start
-
-Here is a simple usage example of the ADAPT library. This is a simulation of a 1D sample bias problem with binary classfication task. The source input data are distributed according to a Gaussian distribution centered in -1 with standard deviation of 2. The target data are drawn from Gaussian distribution centered in 1 with standard deviation of 2. The output labels are equal to 1 in the interval [-1, 1] and 0 elsewhere. We apply the transfer method [KMM](https://adapt-python.github.io/adapt/generated/adapt.instance_based.KMM.html) which is an unsupervised instance-based algortihm.
-
-```python
-# Import standard librairies
-import numpy as np
-from sklearn.linear_model import LogisticRegression
-
-# Import KMM method form adapt.instance_based module
-from adapt.instance_based import KMM
-
-np.random.seed(0)
-
-# Create source dataset (Xs ~ N(-1, 2))
-# ys = 1 for ys in [-1, 1] else, ys = 0
-Xs = np.random.randn(1000, 1)*2-1
-ys = (Xs[:, 0] > -1.) & (Xs[:, 0] < 1.)
-
-# Create target dataset (Xt ~ N(1, 2)), yt ~ ys
-Xt = np.random.randn(1000, 1)*2+1
-yt = (Xt[:, 0] > -1.) & (Xt[:, 0] < 1.)
-
-# Instantiate and fit a source only model for comparison
-src_only = LogisticRegression(penalty="none")
-src_only.fit(Xs, ys)
-
-# Instantiate a KMM model : estimator and target input
-# data Xt are given as parameters with the kernel parameters
-adapt_model = KMM(
-    estimator=LogisticRegression(penalty="none"), 
-    Xt=Xt,
-    kernel="rbf",  # Gaussian kernel
-    gamma=1.,     # Bandwidth of the kernel
-    verbose=0,
-    random_state=0
-)
-
-# Fit the model.
-adapt_model.fit(Xs, ys);
-
-# Get the score on target data
-adapt_model.score(Xt, yt)
-```
-```python
->>> 0.574
-```
-
-| <img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/results_qs.png"> | 
-|:--:| 
-| **Quick-Start Plotting Results**. *The dotted and dashed lines are respectively the class separation of the "source only" and KMM models. Note that the predicted positive class is on the right of the dotted line for the "source only" model but on the left of the dashed line for KMM. (The code for plotting the Figure is available [here](https://adapt-python.github.io/adapt/examples/Quick_start.html))* |
-
-
-## Contents
-
-ADAPT package is divided in three sub-modules containing the following domain adaptation methods:
-
-### Feature-based methods
-
-<img src="https://raw.githubusercontent.com/adapt-python/adapt/a490a5c4cefb80d6222bc831a8cc25b2f65221ce/docs/_static/images/feature_based.png">
-
-- [FA](https://adapt-python.github.io/adapt/generated/adapt.feature_based.FA.html) (*Frustratingly Easy Domain Adaptation*) [[paper]](https://arxiv.org/pdf/0907.1815.pdf)
-- [SA](https://adapt-python.github.io/adapt/generated/adapt.feature_based.SA.html) (*Subspace Alignment*) [[paper]](https://arxiv.org/abs/1409.5241)
-- [fMMD](https://adapt-python.github.io/adapt/generated/adapt.feature_based.SA.html) (*feature Selection with MMD*) [[paper]](https://www.cs.cmu.edu/afs/cs/Web/People/jgc/publication/Feature%20Selection%20for%20Transfer%20Learning.pdf)
-- [DANN](https://adapt-python.github.io/adapt/generated/adapt.feature_based.DANN.html) (*Discriminative Adversarial Neural Network*) [[paper]](https://jmlr.org/papers/volume17/15-239/15-239.pdf)
-- [ADDA](https://adapt-python.github.io/adapt/generated/adapt.feature_based.ADDA.html) (*Adversarial Discriminative Domain Adaptation*) [[paper]](https://arxiv.org/pdf/1702.05464.pdf)
-- [CORAL](https://adapt-python.github.io/adapt/generated/adapt.feature_based.CORAL.html) (*CORrelation ALignment*) [[paper]](https://arxiv.org/pdf/1511.05547.pdf)
-- [DeepCORAL](https://adapt-python.github.io/adapt/generated/adapt.feature_based.DeepCORAL.html) (*Deep CORrelation ALignment*) [[paper]](https://arxiv.org/pdf/1607.01719.pdf)
-- [MCD](https://adapt-python.github.io/adapt/generated/adapt.feature_based.MCD.html) (*Maximum Classifier Discrepancy*) [[paper]](https://arxiv.org/pdf/1712.02560.pdf)
-- [MDD](https://adapt-python.github.io/adapt/generated/adapt.feature_based.MDD.html) (*Margin Disparity Discrepancy*) [[paper]](https://arxiv.org/pdf/1904.05801.pdf)
-- [WDGRL](https://adapt-python.github.io/adapt/generated/adapt.feature_based.WDGRL.html) (*Wasserstein Distance Guided Representation Learning*) [[paper]](https://arxiv.org/pdf/1707.01217.pdf)
-- [CDAN](https://adapt-python.github.io/adapt/generated/adapt.feature_based.CDAN.html) (*Conditional Adversarial Domain Adaptation*) [[paper]](https://arxiv.org/pdf/1705.10667.pdf)
-- [CCSA](https://adapt-python.github.io/adapt/generated/adapt.feature_based.CCSA.html) (*Classification and Contrastive Semantic Alignment*) [[paper]](https://arxiv.org/abs/1709.10190)
-
-### Instance-based methods
-
-<img src="https://raw.githubusercontent.com/adapt-python/adapt/a490a5c4cefb80d6222bc831a8cc25b2f65221ce/docs/_static/images/instance_based.png">
-
-- [LDM](https://adapt-python.github.io/adapt/generated/adapt.instance_based.LDM.html) (*Linear Discrepancy Minimization*) [[paper]](https://arxiv.org/pdf/0902.3430.pdf)
-- [KMM](https://adapt-python.github.io/adapt/generated/adapt.instance_based.KMM.html) (*Kernel Mean Matching*) [[paper]](https://proceedings.neurips.cc/paper/2006/file/a2186aa7c086b46ad4e8bf81e2a3a19b-Paper.pdf)
-- [KLIEP](https://adapt-python.github.io/adapt/generated/adapt.instance_based.KLIEP.html) (*Kullback–Leibler Importance Estimation Procedure*) [[paper]](https://proceedings.neurips.cc/paper/2007/file/be83ab3ecd0db773eb2dc1b0a17836a1-Paper.pdf)
-- [TrAdaBoost](https://adapt-python.github.io/adapt/generated/adapt.instance_based.TrAdaBoost.html) (*Transfer AdaBoost*) [[paper]](https://cse.hkust.edu.hk/~qyang/Docs/2007/tradaboost.pdf)
-- [TrAdaBoostR2](https://adapt-python.github.io/adapt/generated/adapt.instance_based.TrAdaBoostR2.html) (*Transfer AdaBoost for Regression*) [[paper]](https://www.cs.utexas.edu/~dpardoe/papers/ICML10.pdf)
-- [TwoStageTrAdaBoostR2](https://adapt-python.github.io/adapt/generated/adapt.instance_based.TwoStageTrAdaBoostR2.html) (*Two Stage Transfer AdaBoost for Regression*) [[paper]](https://www.cs.utexas.edu/~dpardoe/papers/ICML10.pdf)
-- [NearestNeighborsWeighting](https://adapt-python.github.io/adapt/generated/adapt.instance_based.NearestNeighborsWeighting.html) (*Nearest Neighbors Weighting*) [[paper]](https://arxiv.org/pdf/2102.02291.pdf)
-- [WANN](https://adapt-python.github.io/adapt/generated/adapt.instance_based.WANN.html) (*Weighting Adversarial Neural Network*) [[paper]](https://arxiv.org/pdf/2006.08251.pdf)
-
-### Parameter-based methods
-
-<img src="https://raw.githubusercontent.com/adapt-python/adapt/a490a5c4cefb80d6222bc831a8cc25b2f65221ce/docs/_static/images/parameter_based.png">
-
-- [RegularTransferLR](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.RegularTransferLR.html) (*Regular Transfer with Linear Regression*) [[paper]](https://www.microsoft.com/en-us/research/wp-content/uploads/2004/07/2004-chelba-emnlp.pdf)
-- [RegularTransferLC](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.RegularTransferLC.html) (*Regular Transfer with Linear Classification*) [[paper]](https://www.microsoft.com/en-us/research/wp-content/uploads/2004/07/2004-chelba-emnlp.pdf)
-- [RegularTransferNN](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.RegularTransferNN.html) (*Regular Transfer with Neural Network*) [[paper]](https://hal.inria.fr/hal-00911179v1/document)
-- [FineTuning](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.FineTuning.html) (*Fine-Tuning*) [[paper]](https://hal.inria.fr/hal-00911179v1/document)
-- [TransferTreeClassifier](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.TransferTreeClassifier.html) (*Transfer Tree Classifier*) [[paper]](https://ieeexplore.ieee.org/document/8995296)
-- [TransferTreeForest](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.TransferTreeForest.html) (*Transfer Tree Forest*) [[paper]](https://ieeexplore.ieee.org/document/8995296)
-
-
-## Reference
-
-If you use this library in your research, please cite ADAPT using the following reference: https://arxiv.org/pdf/2107.03049.pdf
-
-```
-@article{de2021adapt,
-	  title={ADAPT: Awesome Domain Adaptation Python Toolbox},
-	  author={de Mathelin, Antoine and Deheeger, Fran{\c{c}}ois and Richard, Guillaume and Mougeot, Mathilde and Vayatis, Nicolas},
-	  journal={arXiv preprint arXiv:2107.03049},
-	  year={2021}
-	}
-```
-
-## Acknowledgement
-
-This work has been funded by Michelin and the Industrial Data Analytics and Machine Learning chair from ENS Paris-Saclay, Borelli center.
-
-[<img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/michelin.png" width=200px alt="Michelin">](https://www.michelin.com/) [<img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/idaml.jpg" width=200px alt="IDAML">](https://centreborelli.ens-paris-saclay.fr/fr/chaire-idaml) [<img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/borelli.jpg" alt="Centre Borelli" width=150px>](https://centreborelli.ens-paris-saclay.fr/fr)
+Metadata-Version: 2.1
+Name: adapt
+Version: 0.4.3
+Summary: Awesome Domain Adaptation Python Toolbox for Tensorflow and Scikit-learn
+Home-page: https://github.com/adapt-python/adapt.git
+Author: Antoine de Mathelin
+Author-email: antoine.demat@gmail.com
+License: BSD-2
+Description: # ADAPT
+        
+        [![PyPI version](https://badge.fury.io/py/adapt.svg)](https://pypi.org/project/adapt)
+        [![Build Status](https://github.com/adapt-python/adapt/workflows/build/badge.svg)](https://github.com/adapt-python/adapt/actions)
+        [![Python Version](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8|%203.9-blue)](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8|%203.9-blue)
+        [![Codecov Status](https://codecov.io/gh/adapt-python/adapt/branch/master/graph/badge.svg?token=IWQXMYGY2Q)](https://codecov.io/gh/adapt-python/adapt)
+        
+        **A**wesome **D**omain **A**daptation **P**ython **T**oolbox
+        
+        ---
+        
+        ADAPT is an open source library providing numerous tools to perform Transfer Learning and Domain Adaptation.
+        
+        The purpose of the ADAPT library is to facilitate the access to transfer learning algorithms for a large public, including industrial players. ADAPT is specifically designed for [Scikit-learn](https://scikit-learn.org/stable/) and [Tensorflow](https://www.tensorflow.org/) users with a "user-friendly" approach. All objects in ADAPT implement the ***fit***, ***predict*** and ***score*** methods like any scikit-learn object. A very detailed documentation with several examples is provided:
+        
+        :arrow_right: [Documentation](https://adapt-python.github.io/adapt/)
+        
+        <table>
+          <tr valign="top">
+            <td width="50%" >
+                <a href="https://adapt-python.github.io/adapt/examples/Sample_bias_example.html">
+                    <br>
+                    <b>Sample bias correction</b>
+                    <br>
+                    <br>
+                    <img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/sample_bias_corr_img.png">
+                </a>
+            </td>
+            <td width="50%">
+                <a href="https://adapt-python.github.io/adapt/examples/Flowers_example.html">
+                    <br>
+                    <b>Model-based Transfer</b>
+                    <br>
+                    <br>
+                    <img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/finetuned.png">
+                </a>
+            </td>
+          </tr>
+          <tr valign="top">
+            <td width="50%">
+                <a href="https://adapt-python.github.io/adapt/examples/Office_example.html">
+                    <br>
+                    <b>Deep Domain Adaptation</b>
+                    <br>
+                    <br>
+                    <img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/office_item.png">
+                </a>
+            </td>
+            <td width="50%">
+                <a href="https://adapt-python.github.io/adapt/examples/Multi_fidelity.html">
+                    <br>
+                    <b>Multi-Fidelity Transfer</b>
+                    <br>
+                    <br>
+                    <img src="https://raw.githubusercontent.com/adapt-python/adapt/a490a5c4cefb80d6222bc831a8cc25b2f65221ce/docs/_static/images/multifidelity_setup.png">
+                </a>
+            </td>
+          </tr>
+        </table>
+        
+        ## Installation and Usage
+        
+        This package is available on [Pypi](https://pypi.org/project/adapt) and can be installed with the following command line: 
+        
+        ```
+        pip install adapt
+        ```
+        
+        The following dependencies are required and will be installed with the library:
+        - `numpy`
+        - `scipy`
+        - `tensorflow` (>= 2.0)
+        - `scikit-learn`
+        - `cvxopt`
+        
+        If for some reason, these packages failed to install, you can do it manually with:
+        
+        ```
+        pip install numpy scipy tensorflow scikit-learn cvxopt
+        ```
+        
+        Finally import the module in your python scripts with:
+        
+        ```python
+        import adapt
+        ```
+        
+        A simple example of usage is given in the [Quick-Start](#Quick-Start) below.
+        
+        
+        ## ADAPT Guideline
+        
+        The transfer learning methods implemented in ADAPT can be seen as scikit-learn "Meta-estimators" or tensorflow "Custom Model":
+        
+        <table>
+        <tr valign="top">
+        <td width="33%" >
+        <br>
+        <b>Adapt Estimator</b>
+        <br>
+        <br>
+        	
+        ```python
+        AdaptEstimator(
+        	estimator = """A scikit-learn estimator
+        	            (like Ridge(alpha=1.) for example)
+        		    or a Tensorflow Model""",
+        	Xt = "The target input features",
+        	yt = "The target output labels (if any)",
+        	**params = "Hyper-parameters of the AdaptEstimator"
+        )
+        ```
+        	
+        <td width="33%">
+        <br>
+        <b>Deep Adapt Estimator</b>
+        <br>
+        <br>
+        
+        	
+        ```python
+        DeepAdaptEstimator(
+        	encoder = "A Tensorflow Model (if required)",
+        	task = "A Tensorflow Model (if required)",
+        	discriminator = "A Tensorflow Model (if required)",
+        	Xt = "The target input features",
+        	yt = "The target output labels (if any)",
+        	**params = """Hyper-parameters of the DeepAdaptEstimator and
+        		      the compile and fit params (optimizer, epochs...)"""
+        )
+        ```
+        	
+        
+        </td>
+        	
+        	
+        </td>
+        <td width="33%">
+        <br>
+        <b>Scikit-learn Meta-Estimator</b>
+        <br>
+        <br>
+        	
+        ```python
+        SklearnMetaEstimator(
+        	base_estimator = """A scikit-learn estimator
+        			 (like Ridge(alpha=1.) for example)""",
+        	**params = "Hyper-parameters of the SklearnMetaEstimator"
+        )
+        ```
+        	
+        
+        </td>
+        </tr>
+        </table>
+        
+        
+        As you can see, the main difference between ADAPT models and scikit-learn and tensorflow objects is the two arguments `Xt, yt` which refer to the target data. Indeed, in classical machine learning, one assumes that the fitted model is applied on data distributed according to the training distribution. This is why, in this setting, one performs cross-validation and splits uniformly the training set to evaluate a model.
+        
+        In the transfer learning framework, however, one assumes that the target data (on which the model will be used at the end) are not distributed like the source training data. Moreover, one assumes that the target distribution can be estimated and compared to the training distribution. Either because a small sample of labeled target data `Xt, yt` is available or because a large sample of unlabeled target data `Xt` is at one's disposal.
+        
+        Thus, the transfer learning models from the ADAPT library can be seen as machine learning models that are fitted with a specific target in mind. This target is different but somewhat related to the training data. This is generally achieved by a transformation of the input features (see [feature-based transfer](https://adapt-python.github.io/adapt/contents.html#adapt-feature-based-feature-based-methods)) or by importance weighting (see [instance-based transfer](https://adapt-python.github.io/adapt/contents.html#adapt-instance-based)). In some cases, the training data are no more available but one aims at fine-tuning a pre-trained source model on a new target dataset (see [parameter-based transfer](https://adapt-python.github.io/adapt/contents.html#adapt-parameter-based)).
+        
+        
+        ## Navigate into ADAPT
+        
+        The ADAPT library proposes numerous transfer algorithms and it can be hard to know which algorithm is best suited for a particular problem. If you do not know which algorithm to choose, this [flowchart](https://adapt-python.github.io/adapt/map.html) may help you:
+        
+        [<img src="https://github.com/adapt-python/adapt/raw/master/src_docs/_static/images/thumbnai_flowchart.PNG" width=30%>](https://adapt-python.github.io/adapt/map.html)
+        
+        
+        ## Quick Start
+        
+        Here is a simple usage example of the ADAPT library. This is a simulation of a 1D sample bias problem with binary classification task. The source input data are distributed according to a Gaussian distribution centered in -1 with standard deviation of 2. The target data are drawn from Gaussian distribution centered in 1 with standard deviation of 2. The output labels are equal to 1 in the interval [-1, 1] and 0 elsewhere. We apply the transfer method [KMM](https://adapt-python.github.io/adapt/generated/adapt.instance_based.KMM.html) which is an unsupervised instance-based algorithm.
+        
+        ```python
+        # Import standard libraries
+        import numpy as np
+        from sklearn.linear_model import LogisticRegression
+        
+        # Import KMM method form adapt.instance_based module
+        from adapt.instance_based import KMM
+        
+        np.random.seed(0)
+        
+        # Create source dataset (Xs ~ N(-1, 2))
+        # ys = 1 for ys in [-1, 1] else, ys = 0
+        Xs = np.random.randn(1000, 1)*2-1
+        ys = (Xs[:, 0] > -1.) & (Xs[:, 0] < 1.)
+        
+        # Create target dataset (Xt ~ N(1, 2)), yt ~ ys
+        Xt = np.random.randn(1000, 1)*2+1
+        yt = (Xt[:, 0] > -1.) & (Xt[:, 0] < 1.)
+        
+        # Instantiate and fit a source only model for comparison
+        src_only = LogisticRegression(penalty="none")
+        src_only.fit(Xs, ys)
+        
+        # Instantiate a KMM model : estimator and target input
+        # data Xt are given as parameters with the kernel parameters
+        adapt_model = KMM(
+            estimator=LogisticRegression(penalty="none"), 
+            Xt=Xt,
+            kernel="rbf",  # Gaussian kernel
+            gamma=1.,     # Bandwidth of the kernel
+            verbose=0,
+            random_state=0
+        )
+        
+        # Fit the model.
+        adapt_model.fit(Xs, ys);
+        
+        # Get the score on target data
+        adapt_model.score(Xt, yt)
+        ```
+        ```python
+        >>> 0.574
+        ```
+        
+        | <img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/results_qs.png"> | 
+        |:--:| 
+        | **Quick-Start Plotting Results**. *The dotted and dashed lines are respectively the class separation of the "source only" and KMM models. Note that the predicted positive class is on the right of the dotted line for the "source only" model but on the left of the dashed line for KMM. (The code for plotting the Figure is available [here](https://adapt-python.github.io/adapt/examples/Quick_start.html))* |
+        
+        
+        ## Contents
+        
+        ADAPT package is divided in three sub-modules containing the following domain adaptation methods:
+        
+        ### Feature-based methods
+        
+        <img src="https://raw.githubusercontent.com/adapt-python/adapt/a490a5c4cefb80d6222bc831a8cc25b2f65221ce/docs/_static/images/feature_based.png">
+        
+        - [FA](https://adapt-python.github.io/adapt/generated/adapt.feature_based.FA.html) (*Frustratingly Easy Domain Adaptation*) [[paper]](https://arxiv.org/pdf/0907.1815.pdf)
+        - [SA](https://adapt-python.github.io/adapt/generated/adapt.feature_based.SA.html) (*Subspace Alignment*) [[paper]](https://arxiv.org/abs/1409.5241)
+        - [fMMD](https://adapt-python.github.io/adapt/generated/adapt.feature_based.fMMD.html) (*feature Selection with MMD*) [[paper]](https://www.cs.cmu.edu/afs/cs/Web/People/jgc/publication/Feature%20Selection%20for%20Transfer%20Learning.pdf)
+        - [DANN](https://adapt-python.github.io/adapt/generated/adapt.feature_based.DANN.html) (*Discriminative Adversarial Neural Network*) [[paper]](https://jmlr.org/papers/volume17/15-239/15-239.pdf)
+        - [ADDA](https://adapt-python.github.io/adapt/generated/adapt.feature_based.ADDA.html) (*Adversarial Discriminative Domain Adaptation*) [[paper]](https://arxiv.org/pdf/1702.05464.pdf)
+        - [CORAL](https://adapt-python.github.io/adapt/generated/adapt.feature_based.CORAL.html) (*CORrelation ALignment*) [[paper]](https://arxiv.org/pdf/1511.05547.pdf)
+        - [DeepCORAL](https://adapt-python.github.io/adapt/generated/adapt.feature_based.DeepCORAL.html) (*Deep CORrelation ALignment*) [[paper]](https://arxiv.org/pdf/1607.01719.pdf)
+        - [MCD](https://adapt-python.github.io/adapt/generated/adapt.feature_based.MCD.html) (*Maximum Classifier Discrepancy*) [[paper]](https://arxiv.org/pdf/1712.02560.pdf)
+        - [MDD](https://adapt-python.github.io/adapt/generated/adapt.feature_based.MDD.html) (*Margin Disparity Discrepancy*) [[paper]](https://arxiv.org/pdf/1904.05801.pdf)
+        - [WDGRL](https://adapt-python.github.io/adapt/generated/adapt.feature_based.WDGRL.html) (*Wasserstein Distance Guided Representation Learning*) [[paper]](https://arxiv.org/pdf/1707.01217.pdf)
+        - [CDAN](https://adapt-python.github.io/adapt/generated/adapt.feature_based.CDAN.html) (*Conditional Adversarial Domain Adaptation*) [[paper]](https://arxiv.org/pdf/1705.10667.pdf)
+        - [CCSA](https://adapt-python.github.io/adapt/generated/adapt.feature_based.CCSA.html) (*Classification and Contrastive Semantic Alignment*) [[paper]](https://arxiv.org/abs/1709.10190)
+        
+        ### Instance-based methods
+        
+        <img src="https://raw.githubusercontent.com/adapt-python/adapt/a490a5c4cefb80d6222bc831a8cc25b2f65221ce/docs/_static/images/instance_based.png">
+        
+        - [LDM](https://adapt-python.github.io/adapt/generated/adapt.instance_based.LDM.html) (*Linear Discrepancy Minimization*) [[paper]](https://arxiv.org/pdf/0902.3430.pdf)
+        - [KMM](https://adapt-python.github.io/adapt/generated/adapt.instance_based.KMM.html) (*Kernel Mean Matching*) [[paper]](https://proceedings.neurips.cc/paper/2006/file/a2186aa7c086b46ad4e8bf81e2a3a19b-Paper.pdf)
+        - [KLIEP](https://adapt-python.github.io/adapt/generated/adapt.instance_based.KLIEP.html) (*Kullbackâ€“Leibler Importance Estimation Procedure*) [[paper]](https://proceedings.neurips.cc/paper/2007/file/be83ab3ecd0db773eb2dc1b0a17836a1-Paper.pdf)
+        - [TrAdaBoost](https://adapt-python.github.io/adapt/generated/adapt.instance_based.TrAdaBoost.html) (*Transfer AdaBoost*) [[paper]](https://cse.hkust.edu.hk/~qyang/Docs/2007/tradaboost.pdf)
+        - [TrAdaBoostR2](https://adapt-python.github.io/adapt/generated/adapt.instance_based.TrAdaBoostR2.html) (*Transfer AdaBoost for Regression*) [[paper]](https://www.cs.utexas.edu/~dpardoe/papers/ICML10.pdf)
+        - [TwoStageTrAdaBoostR2](https://adapt-python.github.io/adapt/generated/adapt.instance_based.TwoStageTrAdaBoostR2.html) (*Two Stage Transfer AdaBoost for Regression*) [[paper]](https://www.cs.utexas.edu/~dpardoe/papers/ICML10.pdf)
+        - [NearestNeighborsWeighting](https://adapt-python.github.io/adapt/generated/adapt.instance_based.NearestNeighborsWeighting.html) (*Nearest Neighbors Weighting*) [[paper]](https://arxiv.org/pdf/2102.02291.pdf)
+        - [WANN](https://adapt-python.github.io/adapt/generated/adapt.instance_based.WANN.html) (*Weighting Adversarial Neural Network*) [[paper]](https://arxiv.org/pdf/2006.08251.pdf)
+        
+        ### Parameter-based methods
+        
+        <img src="https://raw.githubusercontent.com/adapt-python/adapt/a490a5c4cefb80d6222bc831a8cc25b2f65221ce/docs/_static/images/parameter_based.png">
+        
+        - [RegularTransferLR](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.RegularTransferLR.html) (*Regular Transfer with Linear Regression*) [[paper]](https://www.microsoft.com/en-us/research/wp-content/uploads/2004/07/2004-chelba-emnlp.pdf)
+        - [RegularTransferLC](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.RegularTransferLC.html) (*Regular Transfer with Linear Classification*) [[paper]](https://www.microsoft.com/en-us/research/wp-content/uploads/2004/07/2004-chelba-emnlp.pdf)
+        - [RegularTransferNN](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.RegularTransferNN.html) (*Regular Transfer with Neural Network*) [[paper]](https://hal.inria.fr/hal-00911179v1/document)
+        - [FineTuning](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.FineTuning.html) (*Fine-Tuning*) [[paper]](https://hal.inria.fr/hal-00911179v1/document)
+        - [TransferTreeClassifier](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.TransferTreeClassifier.html) (*Transfer Tree Classifier*) [[paper]](https://ieeexplore.ieee.org/document/8995296)
+        - [TransferTreeForest](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.TransferTreeForest.html) (*Transfer Tree Forest*) [[paper]](https://ieeexplore.ieee.org/document/8995296)
+        
+        
+        ## Reference
+        
+        If you use this library in your research, please cite ADAPT using the following reference: https://arxiv.org/pdf/2107.03049.pdf
+        
+        ```
+        @article{de2021adapt,
+        	  title={ADAPT: Awesome Domain Adaptation Python Toolbox},
+        	  author={de Mathelin, Antoine and Deheeger, Fran{\c{c}}ois and Richard, Guillaume and Mougeot, Mathilde and Vayatis, Nicolas},
+        	  journal={arXiv preprint arXiv:2107.03049},
+        	  year={2021}
+        	}
+        ```
+        
+        ## Acknowledgement
+        
+        This work has been funded by Michelin and the Industrial Data Analytics and Machine Learning chair from ENS Paris-Saclay, Borelli center.
+        
+        [<img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/michelin.png" width=200px alt="Michelin">](https://www.michelin.com/) [<img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/idaml.jpg" width=200px alt="IDAML">](https://centreborelli.ens-paris-saclay.fr/fr/chaire-idaml) [<img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/borelli.jpg" alt="Centre Borelli" width=150px>](https://centreborelli.ens-paris-saclay.fr/fr)
+        
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,24 +1,28 @@
-# ADAPT [![PyPI version](https://badge.fury.io/py/adapt.svg)](https://pypi.org/
-project/adapt) [![Build Status](https://github.com/adapt-python/adapt/
-workflows/build/badge.svg)](https://github.com/adapt-python/adapt/actions) [!
-[Python Version](https://img.shields.io/badge/python-
-3.6%20|%203.7%20|%203.8|%203.9-blue)](https://img.shields.io/badge/python-
-3.6%20|%203.7%20|%203.8|%203.9-blue) [![Codecov Status](https://codecov.io/gh/
-adapt-python/adapt/branch/master/graph/badge.svg?token=IWQXMYGY2Q)](https://
-codecov.io/gh/adapt-python/adapt) **A**wesome **D**omain **A**daptation
-**P**ython **T**oolbox --- ADAPT is an open source library providing numerous
-tools to perform Transfer Learning and Domain Adaptation. The purpose of the
-ADAPT library is to facilitate the access to transfer learning algorithms for a
-large public, including industrial players. ADAPT is specifically designed for
-[Scikit-learn](https://scikit-learn.org/stable/) and [Tensorflow](https://
-www.tensorflow.org/) users with a "user-friendly" approach. All objects in
-ADAPT implement the ***fit***, ***predict*** and ***score*** methods like any
-scikit-learn object. A very detailed documentation with several examples is
-provided: :arrow_right: [Documentation](https://adapt-python.github.io/adapt/)
+Metadata-Version: 2.1 Name: adapt Version: 0.4.3 Summary: Awesome Domain
+Adaptation Python Toolbox for Tensorflow and Scikit-learn Home-page: https://
+github.com/adapt-python/adapt.git Author: Antoine de Mathelin Author-email:
+antoine.demat@gmail.com License: BSD-2 Description: # ADAPT [![PyPI version]
+(https://badge.fury.io/py/adapt.svg)](https://pypi.org/project/adapt) [![Build
+Status](https://github.com/adapt-python/adapt/workflows/build/badge.svg)]
+(https://github.com/adapt-python/adapt/actions) [![Python Version](https://
+img.shields.io/badge/python-3.6%20|%203.7%20|%203.8|%203.9-blue)](https://
+img.shields.io/badge/python-3.6%20|%203.7%20|%203.8|%203.9-blue) [![Codecov
+Status](https://codecov.io/gh/adapt-python/adapt/branch/master/graph/
+badge.svg?token=IWQXMYGY2Q)](https://codecov.io/gh/adapt-python/adapt)
+**A**wesome **D**omain **A**daptation **P**ython **T**oolbox --- ADAPT is an
+open source library providing numerous tools to perform Transfer Learning and
+Domain Adaptation. The purpose of the ADAPT library is to facilitate the access
+to transfer learning algorithms for a large public, including industrial
+players. ADAPT is specifically designed for [Scikit-learn](https://scikit-
+learn.org/stable/) and [Tensorflow](https://www.tensorflow.org/) users with a
+"user-friendly" approach. All objects in ADAPT implement the ***fit***,
+***predict*** and ***score*** methods like any scikit-learn object. A very
+detailed documentation with several examples is provided: :arrow_right:
+[Documentation](https://adapt-python.github.io/adapt/)
 
 Sample_bias_correction_                   Model-based_Transfer_
 
 [https://github.com/adapt-python/adapt/   [https://github.com/adapt-python/adapt/
 raw/                                      raw/
 41c13055facc0733faf49c4e3979709e82be10e5/ 41c13055facc0733faf49c4e3979709e82be10e5/
 docs/_static/images/                      docs/_static/images/finetuned.png]
@@ -34,17 +38,17 @@
 ## Installation and Usage This package is available on [Pypi](https://pypi.org/
 project/adapt) and can be installed with the following command line: ``` pip
 install adapt ``` The following dependencies are required and will be installed
 with the library: - `numpy` - `scipy` - `tensorflow` (>= 2.0) - `scikit-learn`
 - `cvxopt` If for some reason, these packages failed to install, you can do it
 manually with: ``` pip install numpy scipy tensorflow scikit-learn cvxopt ```
 Finally import the module in your python scripts with: ```python import adapt
-``` A simple example of usage is given in the [Qick-Start](#Quick-Start) below.
-## ADAPT Guideline The transfer learning methods implemented in ADAPT can be
-seen as scikit-learn "Meta-estimators" or tensorflow "Custom Model":
+``` A simple example of usage is given in the [Quick-Start](#Quick-Start)
+below. ## ADAPT Guideline The transfer learning methods implemented in ADAPT
+can be seen as scikit-learn "Meta-estimators" or tensorflow "Custom Model":
 
 Adapt Estimator            Deep Adapt Estimator       Scikit-learn Meta-
                                                       Estimator
 ```python AdaptEstimator   ```python
 ( estimator = """A scikit- DeepAdaptEstimator         ```python
 learn estimator (like      ( encoder = "A Tensorflow  SklearnMetaEstimator
 Ridge(alpha=1.) for        Model (if required)", task ( base_estimator = """A
@@ -66,15 +70,15 @@
 is applied on data distributed according to the training distribution. This is
 why, in this setting, one performs cross-validation and splits uniformly the
 training set to evaluate a model. In the transfer learning framework, however,
 one assumes that the target data (on which the model will be used at the end)
 are not distributed like the source training data. Moreover, one assumes that
 the target distribution can be estimated and compared to the training
 distribution. Either because a small sample of labeled target data `Xt, yt` is
-avalaible or because a large sample of unlabeled target data `Xt` is at one's
+available or because a large sample of unlabeled target data `Xt` is at one's
 disposal. Thus, the transfer learning models from the ADAPT library can be seen
 as machine learning models that are fitted with a specific target in mind. This
 target is different but somewhat related to the training data. This is
 generally achieved by a transformation of the input features (see [feature-
 based transfer](https://adapt-python.github.io/adapt/contents.html#adapt-
 feature-based-feature-based-methods)) or by importance weighting (see
 [instance-based transfer](https://adapt-python.github.io/adapt/
@@ -85,21 +89,21 @@
 library proposes numerous transfer algorithms and it can be hard to know which
 algorithm is best suited for a particular problem. If you do not know which
 algorithm to choose, this [flowchart](https://adapt-python.github.io/adapt/
 map.html) may help you: [[https://github.com/adapt-python/adapt/raw/master/
 src_docs/_static/images/thumbnai_flowchart.PNG]](https://adapt-
 python.github.io/adapt/map.html) ## Quick Start Here is a simple usage example
 of the ADAPT library. This is a simulation of a 1D sample bias problem with
-binary classfication task. The source input data are distributed according to a
-Gaussian distribution centered in -1 with standard deviation of 2. The target
+binary classification task. The source input data are distributed according to
+a Gaussian distribution centered in -1 with standard deviation of 2. The target
 data are drawn from Gaussian distribution centered in 1 with standard deviation
 of 2. The output labels are equal to 1 in the interval [-1, 1] and 0 elsewhere.
 We apply the transfer method [KMM](https://adapt-python.github.io/adapt/
 generated/adapt.instance_based.KMM.html) which is an unsupervised instance-
-based algortihm. ```python # Import standard librairies import numpy as np from
+based algorithm. ```python # Import standard libraries import numpy as np from
 sklearn.linear_model import LogisticRegression # Import KMM method form
 adapt.instance_based module from adapt.instance_based import KMM np.random.seed
 (0) # Create source dataset (Xs ~ N(-1, 2)) # ys = 1 for ys in [-1, 1] else, ys
 = 0 Xs = np.random.randn(1000, 1)*2-1 ys = (Xs[:, 0] > -1.) & (Xs[:, 0] < 1.) #
 Create target dataset (Xt ~ N(1, 2)), yt ~ ys Xt = np.random.randn(1000, 1)*2+1
 yt = (Xt[:, 0] > -1.) & (Xt[:, 0] < 1.) # Instantiate and fit a source only
 model for comparison src_only = LogisticRegression(penalty="none") src_only.fit
@@ -120,15 +124,15 @@
 methods: ### Feature-based methods [https://raw.githubusercontent.com/adapt-
 python/adapt/a490a5c4cefb80d6222bc831a8cc25b2f65221ce/docs/_static/images/
 feature_based.png] - [FA](https://adapt-python.github.io/adapt/generated/
 adapt.feature_based.FA.html) (*Frustratingly Easy Domain Adaptation*) [[paper]]
 (https://arxiv.org/pdf/0907.1815.pdf) - [SA](https://adapt-python.github.io/
 adapt/generated/adapt.feature_based.SA.html) (*Subspace Alignment*) [[paper]]
 (https://arxiv.org/abs/1409.5241) - [fMMD](https://adapt-python.github.io/
-adapt/generated/adapt.feature_based.SA.html) (*feature Selection with MMD*) [
+adapt/generated/adapt.feature_based.fMMD.html) (*feature Selection with MMD*) [
 [paper]](https://www.cs.cmu.edu/afs/cs/Web/People/jgc/publication/
 Feature%20Selection%20for%20Transfer%20Learning.pdf) - [DANN](https://adapt-
 python.github.io/adapt/generated/adapt.feature_based.DANN.html)
 (*Discriminative Adversarial Neural Network*) [[paper]](https://jmlr.org/
 papers/volume17/15-239/15-239.pdf) - [ADDA](https://adapt-python.github.io/
 adapt/generated/adapt.feature_based.ADDA.html) (*Adversarial Discriminative
 Domain Adaptation*) [[paper]](https://arxiv.org/pdf/1702.05464.pdf) - [CORAL]
@@ -154,15 +158,15 @@
 instance_based.png] - [LDM](https://adapt-python.github.io/adapt/generated/
 adapt.instance_based.LDM.html) (*Linear Discrepancy Minimization*) [[paper]]
 (https://arxiv.org/pdf/0902.3430.pdf) - [KMM](https://adapt-python.github.io/
 adapt/generated/adapt.instance_based.KMM.html) (*Kernel Mean Matching*) [
 [paper]](https://proceedings.neurips.cc/paper/2006/file/
 a2186aa7c086b46ad4e8bf81e2a3a19b-Paper.pdf) - [KLIEP](https://adapt-
 python.github.io/adapt/generated/adapt.instance_based.KLIEP.html)
-(*KullbackâLeibler Importance Estimation Procedure*) [[paper]](https://
+(*KullbackÃ¢â¬âLeibler Importance Estimation Procedure*) [[paper]](https://
 proceedings.neurips.cc/paper/2007/file/be83ab3ecd0db773eb2dc1b0a17836a1-
 Paper.pdf) - [TrAdaBoost](https://adapt-python.github.io/adapt/generated/
 adapt.instance_based.TrAdaBoost.html) (*Transfer AdaBoost*) [[paper]](https://
 cse.hkust.edu.hk/~qyang/Docs/2007/tradaboost.pdf) - [TrAdaBoostR2](https://
 adapt-python.github.io/adapt/generated/adapt.instance_based.TrAdaBoostR2.html)
 (*Transfer AdaBoost for Regression*) [[paper]](https://www.cs.utexas.edu/
 ~dpardoe/papers/ICML10.pdf) - [TwoStageTrAdaBoostR2](https://adapt-
@@ -201,8 +205,9 @@
 Awesome Domain Adaptation Python Toolbox}, author={de Mathelin, Antoine and
 Deheeger, Fran{\c{c}}ois and Richard, Guillaume and Mougeot, Mathilde and
 Vayatis, Nicolas}, journal={arXiv preprint arXiv:2107.03049}, year={2021} } ```
 ## Acknowledgement This work has been funded by Michelin and the Industrial
 Data Analytics and Machine Learning chair from ENS Paris-Saclay, Borelli
 center. [[Michelin]](https://www.michelin.com/) [[IDAML]](https://
 centreborelli.ens-paris-saclay.fr/fr/chaire-idaml) [[Centre Borelli]](https://
-centreborelli.ens-paris-saclay.fr/fr)
+centreborelli.ens-paris-saclay.fr/fr) Platform: UNKNOWN Description-Content-
+Type: text/markdown
```

### Comparing `adapt-0.4.2/adapt/_tree_utils.py` & `adapt-0.4.3/adapt/_tree_utils.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/base.py` & `adapt-0.4.3/adapt/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 import tensorflow as tf
 from sklearn.base import BaseEstimator
 from sklearn.utils import check_array
 from sklearn.metrics.pairwise import KERNEL_PARAMS
 from sklearn.exceptions import NotFittedError
 from tensorflow.keras import Model
 from tensorflow.keras.wrappers.scikit_learn import KerasClassifier, KerasRegressor
+try:
+    from tensorflow.keras.optimizers.legacy import RMSprop
+except:
+    from tensorflow.keras.optimizers import RMSprop
+
 
 from adapt.utils import (check_estimator,
                          check_network,
                          check_arrays,
                          set_random_seed,
                          check_sample_weight,
                          accuracy,
@@ -791,15 +796,14 @@
             legal_params += list(KERNEL_PARAMS[kernel])
         legal_params = set(legal_params)
         legal_params.discard("self")
         return legal_params
 
 
     def __getstate__(self):
-        print("getting")
         dict_ = {k: v for k, v in self.__dict__.items()}
         if "estimator_" in dict_:
             if isinstance(dict_["estimator_"], Model):
                 dict_["estimator_"] = self._get_config_keras_model(
                 dict_["estimator_"]
                 )
         if "estimators_" in dict_:
@@ -813,15 +817,14 @@
                 dict_["estimator"] = self._get_config_keras_model(
                 dict_["estimator"]
                 )
         return dict_
 
 
     def __setstate__(self, dict_):
-        print("setting")
         if "estimator_" in dict_:
             if isinstance(dict_["estimator_"], dict):
                 dict_["estimator_"] = self._from_config_keras_model(
                     dict_["estimator_"]
                 )
         if "estimators_" in dict_:
             for i in range(len(dict_["estimators_"])):
@@ -1306,15 +1309,15 @@
         )
         compile_params = {k: v for k, v in compile_params.items() if v is not None}
         
         compile_params = self._filter_params(super().compile, compile_params)
         
         if ((not "optimizer" in compile_params) or 
             (compile_params["optimizer"] is None)):
-            compile_params["optimizer"] = "rmsprop"
+            compile_params["optimizer"] = RMSprop()
         else:
             if optimizer is None:
                 if not isinstance(compile_params["optimizer"], str):
                     optim_params = self._filter_params(
                         compile_params["optimizer"].__init__)
                     if len(optim_params) > 0:
                         kwargs = compile_params["optimizer"].get_config()
```

### Comparing `adapt-0.4.2/adapt/feature_based/__init__.py` & `adapt-0.4.3/adapt/feature_based/__init__.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/feature_based/_adda.py` & `adapt-0.4.3/adapt/feature_based/_adda.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/feature_based/_ccsa.py` & `adapt-0.4.3/adapt/feature_based/_ccsa.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/feature_based/_cdan.py` & `adapt-0.4.3/adapt/feature_based/_cdan.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/feature_based/_coral.py` & `adapt-0.4.3/adapt/feature_based/_coral.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/feature_based/_dann.py` & `adapt-0.4.3/adapt/feature_based/_dann.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/feature_based/_deepcoral.py` & `adapt-0.4.3/adapt/feature_based/_deepcoral.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/feature_based/_fa.py` & `adapt-0.4.3/adapt/feature_based/_fa.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,17 +88,17 @@
     References
     ----------
     .. [1] `[1] <https://arxiv.org/pdf/0907.1815\
 .pdf>`_ Daume III, H. "Frustratingly easy domain adaptation". In ACL, 2007.
 
     Notes
     -----
-    FA can be used for multi-source DA by giving list of source data
-    for arguments Xs, ys of fit method : Xs = [Xs1, Xs2, ...],
-    ys = [ys1, ys2, ...]
+    FA can be used for multi-source DA by using the ``domains`` argument
+    in the ``fit`` or ``fit_transform`` method. An example is given
+    `[here] <https://github.com/adapt-python/adapt/issues/86>`_
     """
     def __init__(self,
                  estimator=None,
                  Xt=None,
                  yt=None,
                  copy=True,
                  verbose=1,
```

### Comparing `adapt-0.4.2/adapt/feature_based/_fmmd.py` & `adapt-0.4.3/adapt/feature_based/_fmmd.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/feature_based/_mcd.py` & `adapt-0.4.3/adapt/feature_based/_mcd.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/feature_based/_mdd.py` & `adapt-0.4.3/adapt/feature_based/_mdd.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/feature_based/_pred.py` & `adapt-0.4.3/adapt/feature_based/_pred.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/feature_based/_sa.py` & `adapt-0.4.3/adapt/feature_based/_sa.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/feature_based/_tca.py` & `adapt-0.4.3/adapt/feature_based/_tca.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/feature_based/_wdgrl.py` & `adapt-0.4.3/adapt/feature_based/_wdgrl.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/instance_based/__init__.py` & `adapt-0.4.3/adapt/instance_based/__init__.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/instance_based/_balancedweighting.py` & `adapt-0.4.3/adapt/instance_based/_balancedweighting.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/instance_based/_iwc.py` & `adapt-0.4.3/adapt/instance_based/_iwc.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/instance_based/_iwn.py` & `adapt-0.4.3/adapt/instance_based/_iwn.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/instance_based/_kliep.py` & `adapt-0.4.3/adapt/instance_based/_kliep.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,15 +217,15 @@
                  estimator=None,
                  Xt=None,
                  kernel="rbf",
                  sigmas=None,
                  max_centers=100,
                  cv=5,
                  algo="FW",
-                 lr=np.logspace(-3,1,5),
+                 lr=[0.001, 0.01, 0.1, 1.0, 10.0],
                  tol=1e-6,
                  max_iter=2000,
                  copy=True,
                  verbose=1,
                  random_state=None,
                  **params):
```

### Comparing `adapt-0.4.2/adapt/instance_based/_kmm.py` & `adapt-0.4.3/adapt/instance_based/_kmm.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/instance_based/_ldm.py` & `adapt-0.4.3/adapt/instance_based/_ldm.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/instance_based/_nearestneighborsweighting.py` & `adapt-0.4.3/adapt/instance_based/_nearestneighborsweighting.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/instance_based/_rulsif.py` & `adapt-0.4.3/adapt/instance_based/_rulsif.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/instance_based/_tradaboost.py` & `adapt-0.4.3/adapt/instance_based/_tradaboost.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/instance_based/_ulsif.py` & `adapt-0.4.3/adapt/instance_based/_ulsif.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/instance_based/_wann.py` & `adapt-0.4.3/adapt/instance_based/_wann.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/metrics.py` & `adapt-0.4.3/adapt/metrics.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/parameter_based/__init__.py` & `adapt-0.4.3/adapt/parameter_based/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 """
 Parameter-Based Methods Module
 """
 
-from ._regular import RegularTransferLR, RegularTransferLC, RegularTransferNN
+from ._regular import RegularTransferLR, RegularTransferLC, RegularTransferNN, RegularTransferGP
 from ._finetuning import FineTuning
 from ._transfer_tree import TransferTreeClassifier
 from ._transfer_tree import TransferForestClassifier
+from ._transfer_tree import TransferTreeSelector
+from ._transfer_tree import TransferForestSelector
 from ._linint import LinInt
 
 __all__ = ["RegularTransferLR",
            "RegularTransferLC",
            "RegularTransferNN",
+           "RegularTransferGP",
            "FineTuning",
            "TransferTreeClassifier",
            "TransferForestClassifier",
-           "LinInt"]
+           "TransferTreeSelector",
+           "TransferForestSelector",
+           "LinInt"]
```

### Comparing `adapt-0.4.2/adapt/parameter_based/_finetuning.py` & `adapt-0.4.3/adapt/parameter_based/_finetuning.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/parameter_based/_linint.py` & `adapt-0.4.3/adapt/parameter_based/_linint.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt/parameter_based/_regular.py` & `adapt-0.4.3/adapt/parameter_based/_regular.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Regular Transfer
 """
 
 import numpy as np
 from sklearn.preprocessing import LabelBinarizer
 from scipy.sparse.linalg import lsqr
+from sklearn.gaussian_process import GaussianProcessRegressor, GaussianProcessClassifier
+from sklearn.linear_model import LinearRegression
 import tensorflow as tf
 from tensorflow.keras import Sequential
 from tensorflow.keras.layers import Flatten, Dense
 
 from adapt.base import BaseAdaptEstimator, BaseAdaptDeep, make_insert_doc
 from adapt.utils import (check_arrays,
                          set_random_seed,
@@ -182,15 +184,16 @@
             self.coef_ = beta_tgt[:, 1:]
             self.intercept_ = beta_tgt[:, 0]
         else:
             self.coef_ = beta_tgt
             
         if yt_ndim_below_one_:
             self.coef_ = self.coef_.reshape(-1)
-            self.intercept_ = self.intercept_[0]
+            if self.estimator_.fit_intercept:
+                self.intercept_ = self.intercept_[0]
             
         self.estimator_.coef_ = self.coef_
         if self.estimator_.fit_intercept:
             self.estimator_.intercept_ = self.intercept_
         return self
 
     
@@ -263,15 +266,19 @@
     ### TODO reshape yt for multiclass.
     
     def fit(self, Xt=None, yt=None, **fit_params):       
         Xt, yt = self._get_target_data(Xt, yt)
         Xt, yt = check_arrays(Xt, yt)
         
         _label_binarizer = LabelBinarizer(pos_label=1, neg_label=-1)
-        yt = _label_binarizer.fit_transform(yt)
+        _label_binarizer.fit(self.estimator.classes_)
+        yt = _label_binarizer.transform(yt)
+        
+        print(yt.shape)
+        
         return super().fit(Xt, yt, **fit_params)
 
 
 @make_insert_doc(["task"], supervised=True)
 class RegularTransferNN(BaseAdaptDeep):
     """
     Regular Transfer with Neural Network
@@ -463,8 +470,181 @@
         return X
     
     
     def predict_disc(self, X):
         """
         Not used.
         """     
-        pass
+        pass
+    
+    
+@make_insert_doc(supervised=True)
+class RegularTransferGP(BaseAdaptEstimator):
+    """
+    Regular Transfer with Gaussian Process
+    
+    RegularTransferGP is a parameter-based domain adaptation method.
+    
+    The method is based on the assumption that a good target estimator
+    can be obtained by adapting the parameters of a pre-trained source
+    estimator using a few labeled target data.
+    
+    The approach consist in fitting the `alpha` coeficients of a
+    Gaussian Process estimator on target data according to an
+    objective function regularized by the euclidean distance between
+    the source and target `alpha`:
+    
+    .. math::
+    
+        \\alpha_T = \\underset{\\alpha \in \\mathbb{R}^n}{\\text{argmin}}
+        \\, ||K_{TS} \\alpha - y_T||^2 + \\lambda ||\\alpha - \\alpha_S||^2
+        
+    Where:
+    
+    - :math:`\\alpha_T` are the target model coeficients.
+    - :math:`\\alpha_S = \\underset{\\alpha \\in \\mathbb{R}^n}{\\text{argmin}}
+      \\, ||K_{SS} \\alpha - y_S||^2` are the source model coeficients.
+    - :math:`y_S, y_T` are respectively the source and
+      the target labels.
+    - :math:`K_{SS}` is the pariwise kernel distance matrix between source
+      input data.
+    - :math:`K_{TS}` is the pariwise kernel distance matrix between target
+      and source input data.
+    - :math:`n` is the number of source data in :math:`X_S`
+    - :math:`\\lambda` is a trade-off parameter. The larger :math:`\\lambda`
+      the closer the target model will be from the source model.
+    
+    The ``estimator`` given to ``RegularTransferGP`` should be from classes
+    ``sklearn.gaussian_process.GaussianProcessRegressor`` or 
+    ``sklearn.gaussian_process.GaussianProcessClassifier``
+    
+    Parameters
+    ----------
+    lambda_ : float (default=1.0)
+        Trade-Off parameter. For large ``lambda_``, the
+        target model will be similar to the source model.
+
+    Attributes
+    ----------
+    estimator_ : Same class as estimator
+        Fitted Estimator.
+        
+    Examples
+    --------
+    >>> from sklearn.gaussian_process import GaussianProcessRegressor
+    >>> from sklearn.gaussian_process.kernels import Matern, WhiteKernel
+    >>> from adapt.utils import make_regression_da
+    >>> from adapt.parameter_based import RegularTransferGP
+    >>> Xs, ys, Xt, yt = make_regression_da()
+    >>> kernel = Matern() + WhiteKernel()
+    >>> src_model = GaussianProcessRegressor(kernel)
+    >>> src_model.fit(Xs, ys)
+    >>> print(src_model.score(Xt, yt))
+    -2.3409379221035382
+    >>> tgt_model = RegularTransferGP(src_model, lambda_=1.)
+    >>> tgt_model.fit(Xt[:3], yt[:3])
+    >>> tgt_model.score(Xt, yt)
+    -0.21947435769240653
+        
+    See also
+    --------
+    RegularTransferLR, RegularTransferNN
+
+    References
+    ----------
+    .. [1] `[1] <https://www.microsoft.com/en-us/research/wp-\
+content/uploads/2004/07/2004-chelba-emnlp.pdf>`_ C. Chelba and \
+A. Acero. "Adaptation of maximum entropy classifier: Little data \
+can help a lot". In EMNLP, 2004.
+    """
+    
+    def __init__(self,
+             estimator=None,
+             Xt=None,
+             yt=None,
+             lambda_=1.,
+             copy=True,
+             verbose=1,
+             random_state=None,
+             **params):
+                
+        if not hasattr(estimator, "kernel_"):
+            raise ValueError("`estimator` argument has no ``kernel_`` attribute, "
+                             "please call `fit` on `estimator` or use "
+                             "another estimator as `GaussianProcessRegressor` or "
+                             "`GaussianProcessClassifier`.")
+            
+        estimator = check_fitted_estimator(estimator)
+
+        names = self._get_param_names()
+        kwargs = {k: v for k, v in locals().items() if k in names}
+        kwargs.update(params)
+        super().__init__(**kwargs)
+
+    
+    def fit(self, Xt=None, yt=None, **fit_params):
+        """
+        Fit RegularTransferGP.
+
+        Parameters
+        ----------
+        Xt : numpy array (default=None)
+            Target input data.
+
+        yt : numpy array (default=None)
+            Target output data.
+
+        fit_params : key, value arguments
+            Not used. Here for sklearn compatibility.
+
+        Returns
+        -------
+        self : returns an instance of self
+        """
+        Xt, yt = self._get_target_data(Xt, yt)
+        Xt, yt = check_arrays(Xt, yt)
+        set_random_seed(self.random_state)
+        
+        self.estimator_ = check_estimator(self.estimator,
+                                          copy=self.copy,
+                                          force_copy=True)
+        
+        if isinstance(self.estimator, GaussianProcessRegressor):
+            src_linear_model = LinearRegression(fit_intercept=False)
+            src_linear_model.coef_ = self.estimator_.alpha_.transpose()
+
+            Kt = self.estimator_.kernel_(Xt, self.estimator_.X_train_)
+            tgt_linear_model = RegularTransferLR(src_linear_model, lambda_=self.lambda_)
+            
+            tgt_linear_model.fit(Kt, yt)
+            
+            self.estimator_.alpha_ = np.copy(tgt_linear_model.coef_).transpose()
+        
+        elif isinstance(self.estimator, GaussianProcessClassifier):
+            
+            if hasattr(self.estimator_.base_estimator_, "estimators_"):
+                for i in range(len(self.estimator_.base_estimator_.estimators_)):
+                    c = self.estimator_.classes_[i]
+                    if sum(yt == c) > 0:
+                        yt_c = np.zeros(yt.shape[0])
+                        yt_c[yt == c] = 1
+                        self.estimator_.base_estimator_.estimators_[i] = self._fit_one_vs_one_classifier(
+                        self.estimator_.base_estimator_.estimators_[i], Xt, yt_c)
+                
+            else:
+                self.estimator_.base_estimator_ = self._fit_one_vs_one_classifier(
+                self.estimator_.base_estimator_, Xt, yt)
+        return self
+    
+    
+    def _fit_one_vs_one_classifier(self, estimator, Xt, yt):
+        src_linear_model = LinearRegression(fit_intercept=False)
+        src_linear_model.coef_ = (estimator.y_train_ - estimator.pi_)
+        src_linear_model.classes_ = estimator.classes_
+        Kt = estimator.kernel_(Xt, estimator.X_train_)
+        
+        tgt_linear_model = RegularTransferLC(src_linear_model, lambda_=self.lambda_)
+
+        tgt_linear_model.fit(Kt, yt)
+
+        estimator.pi_ = (estimator.y_train_ - np.copy(tgt_linear_model.coef_).ravel())
+        return estimator
```

### Comparing `adapt-0.4.2/adapt/parameter_based/_transfer_tree.py` & `adapt-0.4.3/adapt/parameter_based/_transfer_tree.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #from adapt.utils import (check_arrays,set_random_seed,check_estimator)
 import copy
 import numpy as np
-from sklearn.tree import DecisionTreeClassifier
-from sklearn.ensemble import RandomForestClassifier
+from sklearn.tree import DecisionTreeClassifier, DecisionTreeRegressor
+from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
+from sklearn.metrics import roc_auc_score as _auc_
 
 from adapt.base import BaseAdaptEstimator, make_insert_doc
 from adapt.utils import check_arrays, set_random_seed, check_estimator, check_fitted_estimator
 
 import adapt._tree_utils as ut
 
 
@@ -140,32 +141,36 @@
         -------
         self : returns an instance of self
         """
         Xt, yt = self._get_target_data(Xt, yt)
         Xt, yt = check_arrays(Xt, yt)
         set_random_seed(self.random_state)
 
-        self._modify_tree(self.estimator_, Xt, yt)
+        self._modify_tree(self.estimator_, Xt, yt, **fit_params)
         
         return self
 
     
-    def _modify_tree(self, dtree, X, y):
+    def _modify_tree(self, dtree, X, y, **fit_params):
         
         # Aiguillage
-        if self.algo == "" or self.algo == "relabel":
-            return self._relab(X, y)
+        if self.algo == "src" or self.algo == "source":
+            return 0
+        elif self.algo == "tgt" or self.algo == "trgt" or self.algo == "target":
+            return self._retrain(X,y, **fit_params)
+        elif self.algo == "" or self.algo == "relab" or self.algo == "relabel":
+            return self._relab(X, y, **fit_params)
         elif self.algo == "ser":
-            return self._ser(X, y)
+            return self._ser(X, y, **fit_params)
         
         elif self.algo == "strut":
-            return self._strut(X, y)
+            return self._strut(X, y, **fit_params)
         
         elif hasattr(self.algo, "__call__"):
-            return self.algo(dtree, X, y)
+            return self.algo(dtree, X, y, **fit_params)
 
     ### @@@ ###
 
     ###########
     
     def _compute_params(self,node=0):
         #Tree_ = self.estimator_.tree_
@@ -452,15 +457,20 @@
         if phi != -2:
         #if it is not a leaf
             coh,non_coherent_sense = ut.coherent_new_split(phi,th,rule)
                         
             if not coh:
                 if Translate :
                     if auto_drift:
-                        b_infs,b_sups = ut.bounds_rule(rule,self.estimator_.n_features_)
+                        try:
+                            n_feat = self.estimator_.n_features_
+                        except:
+                            n_feat = self.estimator_.n_features_in_
+                        b_infs,b_sups = ut.bounds_rule(rule, n_feat)
+
                         if non_coherent_sense == -1:
                             if b_sups[phi] == np.inf:
                                 self.updateSplit(node,phi,th+D_MARGIN)
                             else:
                                 self.updateSplit(node,phi,( b_infs[phi] + b_sups[phi] )/2)
                         if non_coherent_sense == 1:
                             if b_infs[phi] == -np.inf:
@@ -494,25 +504,66 @@
             return node
             
     ### @@@ ###
     
     ###########
 
     def updateSplit(self,node,feature,threshold):
+        """
+        Update the (feature,threshold) split for a given node.
+        
+        Parameters
+        ----------
+        node : int
+            Node to update.
+            
+        feature : int
+            New node feature.
+            
+        threshold : float
+            New node threshold.
+        
+        """
         return self._update_split(node,feature,threshold)
         
     def updateValue(self,node,values):
+        """
+        Update class values for a given node.
+        
+        Parameters
+        ----------
+        node : int
+            Node to update.
+            
+        values : numpy array of float
+            Class values to affect at node.
+        
+        """
         #Tree_ = self.estimator_.tree_
         self.estimator_.tree_.value[node] = values
         self.estimator_.tree_.impurity[node] = ut.GINI(values)
         self.estimator_.tree_.n_node_samples[node] = np.sum(values)
         self.estimator_.tree_.weighted_n_node_samples[node] = np.sum(values)
         return node
     
     def swap_subtrees(self,node1,node2):
+        """
+        Swap respective sub-trees between two given nodes.
+        
+        Each node must not be a sub-node of the other.
+        Update the (feature,threshold) split for a given node.
+        
+        Parameters
+        ----------
+        node1 : int
+            Node to swap.
+            
+        node2 : int
+            Node to swap.            
+        """
         #Check sub-nodes :
         if node1 == node2:
             print('Warning : same node given twice.')
             return 0
         
         if node2 in ut.sub_nodes(self.estimator_.tree_, node1)[1:]:
             print('Error : node2 is a sub-node of node1.')
@@ -545,27 +596,62 @@
         
         self.estimator_.tree_.max_depth = max(d1,d2)
         self.estimator_.max_depth = self.estimator_.tree_.max_depth
         
         return 1
         
     def prune(self,node,include_node=False,lr=0,leaf_value=None):
+        """
+        Pruning the corresponding sub-tree at a given node.
+        
+        If `include_node` is `False`, replaces the node by a leaf (with values `leaf_values` if provided).
+        If `include_node` is `True`, prunes the left (`lr=-1`) or (`lr=1`) child sub-tree and
+        replaces the given node by the other sub-tree.
+        
+        Parameters
+        ----------
+        node : int
+            Node to prune.
+            
+        include_node : boolean (default=False)
+            Type of pruning to apply.
+        
+        lr : float
+            Direction of pruning if `include_node` is `True`.
+            Must be either -1 (left) or 1 (right) in this case.
+            
+        leaf_value : numpy array of float (default=None)
+            If `include_node` is `False`, affects these values to the created leaf.          
+        """
         if include_node:
             n = self._cut_left_right(node,lr)
         else:
             n = self._cut_leaf(node,leaf_value=leaf_value)
         return n
 
     def extend(self,node,subtree):
+        """
+        Extend the underlying decision tree estimator by a sub-tree at a given node.
+        
+        Parameters
+        ----------
+        node : int
+            Node to update.
+            
+        subtree : DecisionTreeClassifier.        
+        """
         n = self._extend(node,subtree)
         return n
 
     ### @@@ ###
 
     ###########
+    
+    def _retrain(self,X_target, Y_target):
+        self.estimator_.fit(X_target, Y_target)
 
 
     def _relab(self, X_target_node, Y_target_node, node=0):
         
         #Tree_ = self.estimator_.tree_
         classes_ = self.estimator_.classes_
         
@@ -592,15 +678,34 @@
 
 
     def _ser(self,X_target_node,y_target_node,node=0,original_ser=True,
              no_red_on_cl=False,cl_no_red=None, no_ext_on_cl=False, cl_no_ext=None,ext_cond=None,
              leaf_loss_quantify=False,leaf_loss_threshold=None,coeffs=[1,1],root_source_values=None,Nkmin=None,max_depth=None):
         
         #Tree_ = self.estimator_.tree_
+        if (no_red_on_cl or no_ext_on_cl ) and node == 0:
+            if Nkmin is None:
+                if no_ext_on_cl:
+                    Nkmin = sum(y_target_node == cl_no_ext )
+                if no_red_on_cl:
+                    Nkmin = sum(y_target_node == cl_no_red )
+            if root_source_values is None:
+                root_source_values = ut.get_node_distribution(self.estimator_, 0).reshape(-1)
+
 
+            if coeffs is None or list(coeffs) == [1,1]:        
+                props_s = root_source_values
+                props_s = props_s / sum(props_s)
+                props_t = np.zeros(props_s.size)
+                
+                for k in range(props_s.size):
+                    props_t[k] = np.sum(y_target_node == k) / y_target_node.size
+                    
+                coeffs = np.divide(props_t, props_s)
+                
         source_values = self.estimator_.tree_.value[node].copy()
         #node_source_label = np.argmax(source_values)
         maj_class = np.argmax(self.estimator_.tree_.value[node, :].copy())
 
         if cl_no_red is None:
             old_size_cl_no_red = 0
         else:
@@ -609,16 +714,17 @@
         # Situation où il y a des restrictions sur plusieurs classes ?
         if no_red_on_cl is not None or no_ext_on_cl is not None :
             if no_ext_on_cl:
                 cl = cl_no_ext[0]
             if no_red_on_cl:
                 cl = cl_no_red[0]
 
-        if leaf_loss_quantify and ((no_red_on_cl  or  no_ext_on_cl) and maj_class == cl) and  self.estimator_.tree_.feature[node] == -2 :
-            
+        if (leaf_loss_quantify is True ) and ((no_red_on_cl  or  no_ext_on_cl) and maj_class == cl) and  self.estimator_.tree_.feature[node] == -2 :
+            if Nkmin is None:
+                Nkmin = sum(y_target_node == cl_no_red )
             ps_rf = self.estimator_.tree_.value[node,0,:]/sum(self.estimator_.tree_.value[node,0,:])
             p1_in_l = self.estimator_.tree_.value[node,0,cl]/root_source_values[cl]
             
             cond_homog_unreached = np.power(1 - p1_in_l,Nkmin) > leaf_loss_threshold
             cond_homog_min_label = np.argmax(np.multiply(coeffs,ps_rf)) == cl
             
         val = np.zeros((self.estimator_.n_outputs_, self.estimator_.n_classes_))
@@ -804,52 +910,75 @@
             
 
     def _strut(self,X_target_node,Y_target_node,node=0,no_prune_on_cl=False,cl_no_prune=None,adapt_prop=False,
           coeffs=[1, 1],use_divergence=True,measure_default_IG=True,min_drift=None,max_drift=None,no_prune_with_translation=True,
           leaf_loss_quantify=False,leaf_loss_threshold=None,root_source_values=None,Nkmin=None):
                 
 #        Tree_ = self.estimator_.tree_
-        
+
+        if (no_prune_on_cl or leaf_loss_quantify or adapt_prop) and node == 0:
+
+            if Nkmin is None:
+                Nkmin = sum(Y_target_node == cl_no_prune )
+            if root_source_values is None:
+                root_source_values = ut.get_node_distribution(self.estimator_, 0).reshape(-1)
+
+            if coeffs is None or list(coeffs) == [1,1]:        
+                props_s = root_source_values
+                props_s = props_s / sum(props_s)
+                props_t = np.zeros(props_s.size)
+                
+                for k in range(props_s.size):
+                    props_t[k] = np.sum(Y_target_node == k) / Y_target_node.size
+                    
+                coeffs = np.divide(props_t, props_s)
+            
         feature_ = self.estimator_.tree_.feature[node]
         classes_ = self.estimator_.classes_
         threshold_ = self.estimator_.tree_.threshold[node]
             
         old_threshold = threshold_.copy()
         maj_class = np.argmax(self.estimator_.tree_.value[node, :].copy())
         
         if min_drift is None or max_drift is None:
-            min_drift = np.zeros(self.estimator_.n_features_)
-            max_drift = np.zeros(self.estimator_.n_features_)
+            try:
+                n_feat = self.estimator_.n_features_
+            except:
+                n_feat = self.estimator_.n_features_in_
+            min_drift = np.zeros(n_feat)
+            max_drift = np.zeros(n_feat)
 
         current_class_distribution = ut.compute_class_distribution(classes_, Y_target_node)
         is_reached = (Y_target_node.size > 0)
         no_min_instance_targ = False
         
         if no_prune_on_cl:
             no_min_instance_targ = (sum(current_class_distribution[cl_no_prune]) == 0 )
             is_instance_cl_no_prune = np.sum(self.estimator_.tree_.value[node, :,cl_no_prune].astype(int))
 
         # If it is a leaf :
         if self.estimator_.tree_.feature[node] == -2:
             """ When to apply UpdateValue """
             if leaf_loss_quantify and (no_prune_on_cl and maj_class == cl_no_prune) :
-                
+
                 ps_rf = self.estimator_.tree_.value[node,0,:]/sum(self.estimator_.tree_.value[node,0,:])
                 p1_in_l = self.estimator_.tree_.value[node,0,cl_no_prune]/root_source_values[cl_no_prune]
                 cond1 = np.power(1 - p1_in_l,Nkmin) > leaf_loss_threshold
                 cond2 = np.argmax(np.multiply(coeffs,ps_rf)) == cl_no_prune
                 
             if no_min_instance_targ and no_prune_on_cl and is_instance_cl_no_prune:
                 if leaf_loss_quantify and (no_prune_on_cl and maj_class == cl_no_prune) and not(cond1 and cond2):
                     self.updateValue(node,current_class_distribution)
                     return node
                 else:
                     return node
             else:
-                self.estimator_.tree_.value[node] = current_class_distribution
+                #self.estimator_.tree_.value[node] = current_class_distribution
+                """ UpdateValue """
+                self.updateValue(node,current_class_distribution)
                 return node
 
         # Only one class remaining in target :
         if (current_class_distribution > 0).sum() == 1:
             """ When to apply Pruning and how if not """
             if no_min_instance_targ and no_prune_on_cl and is_instance_cl_no_prune :
                 bool_subleaf_noprune = True
@@ -1015,21 +1144,133 @@
                           min_drift=min_drift.copy(),max_drift=max_drift.copy(),no_prune_with_translation=no_prune_with_translation,
                           leaf_loss_quantify=leaf_loss_quantify,leaf_loss_threshold=leaf_loss_threshold,root_source_values=root_source_values,Nkmin=Nkmin)
 
             node = self.parents[node_r]
               
         return node
 
+        
+class TransferTreeSelector(BaseAdaptEstimator):
+    """
+    TransferTreeSelector : Run several decision tree transfer algorithms on a target dataset and select the best one.
+    """
+    def __init__(self,
+                 estimator=None,
+                 Xt=None,
+                 yt=None,
+                 algorithms=list(),
+                 list_alg_args=list(),
+                 data_size_per_class=None,
+                 root_source_values=None,
+                 coeffs=[1,1],
+                 copy=True,
+                 verbose=1,
+                 random_state=None,
+                 **params):
+               
+        if not hasattr(estimator, "tree_"):
+            raise ValueError("`estimator` argument has no ``tree_`` attribute, "
+                                "please call `fit` on `estimator` or use "
+                                "another estimator as `DecisionTreeClassifier`.")
+        
+        estimator = check_fitted_estimator(estimator)
+        
+        super().__init__(estimator=estimator,
+                         Xt=Xt,
+                         yt=yt,
+                         copy=copy,
+                         verbose=verbose,                       
+                         **params)
 
+        
+        if len(algorithms) == 0:
+            print('Warning : empty list of methods. Default are Source and Target models.')
+            self.algorithms = ['src','trgt']
+            self.list_alg_args = [{},{}]
+        else:
+            self.algorithms = algorithms
+            self.list_alg_args = list_alg_args
+            
+        if len(self.list_alg_args) == 0 and len(self.algorithms) != 0 :
+            self.list_alg_args = list(np.repeat({},len(self.algorithms)))
+        
+        self.n_methods = len(self.algorithms)
+        self.scores = np.zeros(self.n_methods)
+        
+        self.best_score = 0
+        self.best_index = -1
+        
+        self.data_size_per_class = data_size_per_class
+        self.root_source_values = root_source_values
+        self.coeffs = coeffs
+        
+        self.transferred_models = list()
+        
+        for algo in self.algorithms:
 
+            self.transferred_models.append(TransferTreeClassifier(estimator=self.estimator,Xt=self.Xt,yt=self.yt,algo=algo,copy=self.copy))
+            
+      
+    def fit(self, Xt=None, yt=None, **fit_params):
 
+        Xt, yt = self._get_target_data(Xt, yt)
+        Xt, yt = check_arrays(Xt, yt)
+        set_random_seed(self.random_state)
+        
+        for k,algo in enumerate(self.algorithms):
+            kwargs = self.list_alg_args[k]
+            
+            if 'Nkmin' not in kwargs.keys():
+                if 'cl_no_red' in kwargs.keys():
+                    cl = kwargs['cl_no_red']
+                    self.Nkmin = self.data_size_per_class[cl]
+                    kwargs['Nkmin'] = self.Nkmin
+                elif 'cl_no_prune' in kwargs.keys():
+                    cl = kwargs['cl_no_prune']
+                    self.Nkmin = self.data_size_per_class[cl]
+                    kwargs['Nkmin'] = self.Nkmin
+                elif 'cl_no_ext' in kwargs.keys():
+                    cl = kwargs['cl_no_ext']
+                    self.Nkmin = self.data_size_per_class[cl]
+                    kwargs['Nkmin'] = self.Nkmin
+            if ('leaf_loss_quantify' in kwargs.keys() and kwargs['leaf_loss_quantify']) or ('adapt_prop' in kwargs.keys() and kwargs['adapt_prop']):
+                kwargs['root_source_values'] = self.root_source_values
+                kwargs['coeffs'] = self.coeffs
+
+            
+            #self.transferred_models[k].fit(Xt=Xt, yt=yt,Nkmin=self.Nkmin,root_source_values=self.root_source_values,coeffs=self.coeffs,**kwargs,**fit_params)
+            self.transferred_models[k].fit(Xt=Xt, yt=yt,**kwargs,**fit_params)
+            
+    def select(self,Xtest=None,ytest=None,score_type="auc"):
+
+        Xtest, ytest = self._get_target_data(Xtest, ytest)
+        Xtest, ytest = check_arrays(Xtest, ytest)
+        set_random_seed(self.random_state)
+        
+        for k in range(len(self.algorithms)):
+            if score_type == "auc":
+                self.scores[k] = _auc_(ytest,self.transferred_models[k].estimator_.predict_proba(Xtest)[:,1]) 
+            else:
+                self.scores[k] = self.transferred_models[k].score(Xtest,ytest) 
+        
+        self.best_score = np.amax(self.scores)
+        self.best_index = np.argmax(self.scores)
+        self.best_method = self.algorithms[self.best_index]
+        
+        return self.best_score, self.best_index
+    
 class TransferForestClassifier(BaseAdaptEstimator):
     """
     TransferForestClassifier: Modify a source Random Forest on a target dataset.
     
+    Random forest classifier structure for model-based transfer algorithms.
+    
+    This includes several algorithms : leaves relabeling according to target data, SER and STRUT algorithms
+    and various variants for target class imbalance situations.
+    
     Parameters
     ----------    
     estimator : sklearn RandomForestClassifier (default=None)
         Source random forest classifier.
         
     Xt : numpy array (default=None)
         Target input data.
@@ -1077,15 +1318,15 @@
 
     def __init__(self,
                  estimator=None,
                  Xt=None,
                  yt=None,
                  algo="",
                  bootstrap=False,
-                 cpy=True,
+                 copy=True,
                  verbose=1,
                  random_state=None,
                  **params):
         
         if not isinstance(estimator, RandomForestClassifier):
             raise ValueError("`estimator` argument must be a ``RandomForestClassifier`` instance, got %s."%str(type(estimator)))
 
@@ -1117,26 +1358,29 @@
             self.estimators_[i] = TransferTreeClassifier(estimator = self.estimator_.estimators_[i], algo = self.algo)
 
 
     ### @@@ ###
 
     ###########
     
-    def _modify_rf(self, rf, X, y):
+    def _modify_rf(self, rf, X, y, **fit_params):
         # Aiguillage
+        if self.algo == "src" or self.algo == "source":
+            return 0
+        elif self.algo == "tgt" or self.algo == "trgt" or self.algo == "target":
+            return self._retrain(X,y, **fit_params)
         if self.algo == "" or self.algo == "relabel":
-            bootstrap = self.bootstrap
-            return self._relab_rf(X, y, bootstrap=bootstrap)
+            return self._relab_rf(X, y, **fit_params)
         elif self.algo == "ser":
-            return self._ser_rf(X, y)        
+            return self._ser_rf(X, y, **fit_params)        
         elif self.algo == "strut":
-            return self._strut_rf(X, y)
+            return self._strut_rf(X, y, **fit_params)
         
         elif hasattr(self.algo, "__call__"):
-            return self.algo(rf, X, y)
+            return self.algo(rf, X, y, **fit_params)
 
     def fit(self, Xt=None, yt=None, **fit_params):
         """
         Fit TransferTreeClassifier.
 
         Parameters
         ----------
@@ -1154,45 +1398,57 @@
         self : returns an instance of self
         """
 
         Xt, yt = self._get_target_data(Xt, yt)
         Xt, yt = check_arrays(Xt, yt)
         set_random_seed(self.random_state)
             
-        self._modify_rf(self.estimator_, Xt, yt)
+        self._modify_rf(self.estimator_, Xt, yt, **fit_params)
         
         return self
+    
+    def _copy_rf(self):
+        rf_out = copy.deepcopy(self.estimator)
+        for k in range(self.rf_size):
+            rf_out.estimators_[k] = self.estimators_[k].estimator_
+        self.estimator_ = rf_out
 
-    def _relab_rf(self, X_target_node, Y_target_node,bootstrap=False):
+    def _copy_dt(self):
+        for k in range(self.rf_size):
+            self.estimators_[k].estimator_ = self.estimator_.estimators_[k]
+        
+    def _retrain(self,X_target, Y_target):
+        self.estimator_.fit(X_target, Y_target)
+        self._copy_dt()
         
-        rf_out = copy.deepcopy(self.estimator)
+    def _relab_rf(self, X_target_node, Y_target_node):
         
-        if bootstrap :             
+        rf_out = copy.deepcopy(self.estimator)
+        if self.bootstrap :             
             inds,oob_inds = ut._bootstrap_(Y_target_node.size,class_wise=True,y=Y_target_node)
             for k in range(self.rf_size):
                 X_target_node_bootstrap = X_target_node[inds]
                 Y_target_node_bootstrap = Y_target_node[inds]
                 self.estimators_[k]._relab(X_target_node_bootstrap, Y_target_node_bootstrap, node=0)
                 rf_out.estimators_[k] = self.estimators_[k].estimator_
         else:            
             for k in range(self.rf_size):
                 self.estimators_[k]._relab(X_target_node, Y_target_node, node=0)
                 rf_out.estimators_[k] = self.estimators_[k].estimator_
-        
-        
+                
         self.estimator_ = rf_out
-
+        self._copy_dt()
+        self._copy_rf()
         return self.estimator_
     
     def _ser_rf(self,X_target,y_target,original_ser=True,
              no_red_on_cl=False,cl_no_red=None, no_ext_on_cl=False, cl_no_ext=None,ext_cond=None,
              leaf_loss_quantify=False,leaf_loss_threshold=None,coeffs=[1,1],root_source_values=None,Nkmin=None,max_depth=None):
         
         rf_out = copy.deepcopy(self.estimator)
-        
         for i in range(self.rf_size):
             root_source_values = None
             coeffs = None
             Nkmin = None
             if  leaf_loss_quantify :    
                 Nkmin = sum(y_target == cl_no_red )
                 root_source_values = ut.get_node_distribution(self.estimator_.estimators_[i], 0).reshape(-1)
@@ -1213,25 +1469,25 @@
             self.estimators_[i]._ser(X_target[inds],y_target[inds],node=0,original_ser=original_ser,
                             no_red_on_cl=no_red_on_cl,cl_no_red=cl_no_red,no_ext_on_cl=no_ext_on_cl, cl_no_ext=cl_no_ext,ext_cond=ext_cond,
                             leaf_loss_quantify=leaf_loss_quantify,leaf_loss_threshold=leaf_loss_threshold,coeffs=coeffs,root_source_values=root_source_values,
                             Nkmin=Nkmin,max_depth=max_depth)
             
             rf_out.estimators_[i] = self.estimators_[i].estimator_
             
-
         self.estimator_ = rf_out
+        self._copy_dt()
+        self._copy_rf()
         
         return self.estimator_
     
     def _strut_rf(self,X_target,y_target,no_prune_on_cl=False,cl_no_prune=None,adapt_prop=False,
           coeffs=[1, 1],use_divergence=True,measure_default_IG=True,min_drift=None,max_drift=None,no_prune_with_translation=True,
           leaf_loss_quantify=False,leaf_loss_threshold=None,root_source_values=None,Nkmin=None):
                     
         rf_out = copy.deepcopy(self.estimator)
-        
         for i in range(self.rf_size):
     
             if adapt_prop or leaf_loss_quantify:
             
                 Nkmin = sum(y_target == cl_no_prune )
                 root_source_values = ut.get_node_distribution(self.estimator_.estimators_[i], 0).reshape(-1)
             
@@ -1251,30 +1507,166 @@
                       no_prune_on_cl=no_prune_on_cl,
                       cl_no_prune=cl_no_prune,
                       adapt_prop=adapt_prop,                  
                       coeffs=coeffs,
                       use_divergence=use_divergence,
                       measure_default_IG=measure_default_IG,no_prune_with_translation=no_prune_with_translation,
                       leaf_loss_quantify=leaf_loss_quantify,leaf_loss_threshold=leaf_loss_threshold, 
-                      root_source_values=root_source_values,Nkmin=Nkmin)                
-                rf_out.estimators_[i] = self.estimators_[i].estimator_
+                      root_source_values=root_source_values,Nkmin=Nkmin)      
+
                 
             else:
                 self.estimators_[i]._strut(
                       X_target,
                       y_target,
                       node=0,
                       no_prune_on_cl=no_prune_on_cl,
                       cl_no_prune=cl_no_prune,               
                       use_divergence=use_divergence,
                       measure_default_IG=measure_default_IG,no_prune_with_translation=no_prune_with_translation,
                       root_source_values=root_source_values,Nkmin=Nkmin) 
-                rf_out.estimators_[i] = self.estimators_[i].estimator_
+                
+            rf_out.estimators_[i] = self.estimators_[i].estimator_
                 
         self.estimator_ = rf_out
+        self._copy_dt()
+        self._copy_rf()
         
-        return self.estimator_
+        return self.estimator_      
+       
+
+
+        
+class TransferForestSelector(BaseAdaptEstimator):
+    """
+    TransferForestSelector : Run several decision tree transfer algorithms on a target dataset and select the best one for each tree of the random forest.
+    
+    """
+    def __init__(self,
+                 estimator=None,
+                 Xt=None,
+                 yt=None,
+                 algorithms=list(),
+                 list_alg_args=list(),
+                 bootstrap=True,
+                 copy=True,
+                 verbose=1,
+                 random_state=None,
+                 **params):
+        
+        if not isinstance(estimator, RandomForestClassifier):
+            raise ValueError("`estimator` argument must be a ``RandomForestClassifier`` instance, got %s."%str(type(estimator)))
 
+        if not hasattr(estimator, "estimators_"):
+            raise ValueError("`estimator` argument has no ``estimators_`` attribute, "
+                                "please call `fit` on `estimator`.")
+        
+        estimator = check_fitted_estimator(estimator)
+        
+        super().__init__(estimator=estimator,
+                         Xt=Xt,
+                         yt=yt,
+                         copy=copy,
+                         verbose=verbose,
+                         random_state=random_state,                       
+                         bootstrap=bootstrap,
+                         **params)
+        
+
+        self.estimator_ = check_estimator(self.estimator,
+                                          copy=self.copy,
+                                          force_copy=True)
+                
+        
+        self.rf_size = self.estimator_.n_estimators
+
+        
+        if len(algorithms) == 0:
+            print('Warning : empty list of methods. Default are Source and Target models.')
+            self.algorithms = ['src','trgt']
+            self.list_alg_args = [{},{}]
+        else:
+            self.algorithms = algorithms
+            self.list_alg_args = list_alg_args
             
+        if len(self.list_alg_args) == 0 and len(self.algorithms) != 0 :
+            self.list_alg_args = list(np.repeat({},len(self.algorithms)))
             
 
+        self.n_methods = len(self.algorithms)
+        self.scores = np.zeros(self.n_methods)
+        
+        self.best_score = 0
+        self.best_index = -1
+        
+        self.transferred_models = list()
+        
+        for algo in self.algorithms:
+            self.transferred_models.append(TransferForestClassifier(estimator=self.estimator,Xt=self.Xt,yt=self.yt,algo=algo,bootstrap=self.bootstrap,copy=self.copy))
+            
+        self.STRF_model = TransferForestClassifier(estimator=self.estimator,Xt=self.Xt,yt=self.yt,algo=algo,bootstrap=self.bootstrap,copy=self.copy)
+        self.STRF_indexes = np.zeros(self.rf_size)
+
+                
+    def model_selection(self, Xt=None, yt=None, score_type = "auc", oob_ = False, **fit_params):
+
+        Xt, yt = self._get_target_data(Xt, yt)
+        Xt, yt = check_arrays(Xt, yt)
+        set_random_seed(self.random_state)
+        
+        rf_out = copy.deepcopy(self.estimator)
+
+
+        for k in range(self.rf_size):
+
+            # For imbalance adaptation:
+            data_size_per_class = np.zeros(rf_out.n_classes_)
+            props_t = np.zeros(rf_out.n_classes_)
+            
+            for cl in range(rf_out.n_classes_):
+                data_size_per_class[cl] = sum(yt == cl )
+            props_t = data_size_per_class / yt.size
+            
+            root_source_values = ut.get_node_distribution(rf_out.estimators_[k], 0).reshape(-1)
+
+            props_s = root_source_values
+            props_s = props_s / sum(props_s)     
+            coeffs = np.divide(props_t, props_s)
+
+            TTS = TransferTreeSelector(estimator=self.estimator_.estimators_[k],algorithms=self.algorithms,
+                                       list_alg_args=self.list_alg_args,
+                                       data_size_per_class=data_size_per_class,
+                                       root_source_values=root_source_values,coeffs=coeffs)
+            
+            if self.bootstrap:
+                inds, oob_inds = ut._bootstrap_(yt.size,class_wise=True,y=yt)
+                TTS.fit(Xt[inds],yt[inds],**fit_params)         
+                
+                if len(set(yt[oob_inds])) == 1:
+                    print('Warning: Only one class in OOB samples.')
+                    oob_ = False
+                if oob_:
+                    score, index = TTS.select(Xtest=Xt[oob_inds],ytest=yt[oob_inds],score_type=score_type)
+                else:
+                    score, index = TTS.select(Xtest=Xt[inds],ytest=yt[inds],score_type=score_type)
+            else:
+                TTS.fit(Xt,yt,**fit_params)                
+                score, index = TTS.select(Xtest=Xt,ytest=yt,score_type=score_type)                 
+
+            self.STRF_indexes[k] = index
+            
+            self.STRF_model.estimators_[k] = TTS.transferred_models[index]
+            
+            for j,m in enumerate(self.transferred_models):
+                #rf_out_alg = copy.deepcopy(rf_out)
+                m.estimators_[k] = TTS.transferred_models[j]
+                m.estimator_.estimators_[k] = TTS.transferred_models[j].estimator_
+                #m.estimator_ = rf_out_alg
+                
+            rf_out.estimators_[k] = TTS.transferred_models[index].estimator_
+        
+        self.STRF_model.estimator_ = rf_out
+        self.estimator_ = rf_out
+        
+        return self.STRF_indexes
+
```

### Comparing `adapt-0.4.2/adapt/utils.py` & `adapt-0.4.3/adapt/utils.py`

 * *Files identical despite different names*

### Comparing `adapt-0.4.2/adapt.egg-info/PKG-INFO` & `adapt-0.4.3/adapt.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,302 +1,299 @@
 Metadata-Version: 2.1
 Name: adapt
-Version: 0.4.2
+Version: 0.4.3
 Summary: Awesome Domain Adaptation Python Toolbox for Tensorflow and Scikit-learn
 Home-page: https://github.com/adapt-python/adapt.git
 Author: Antoine de Mathelin
 Author-email: antoine.demat@gmail.com
 License: BSD-2
+Description: # ADAPT
+        
+        [![PyPI version](https://badge.fury.io/py/adapt.svg)](https://pypi.org/project/adapt)
+        [![Build Status](https://github.com/adapt-python/adapt/workflows/build/badge.svg)](https://github.com/adapt-python/adapt/actions)
+        [![Python Version](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8|%203.9-blue)](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8|%203.9-blue)
+        [![Codecov Status](https://codecov.io/gh/adapt-python/adapt/branch/master/graph/badge.svg?token=IWQXMYGY2Q)](https://codecov.io/gh/adapt-python/adapt)
+        
+        **A**wesome **D**omain **A**daptation **P**ython **T**oolbox
+        
+        ---
+        
+        ADAPT is an open source library providing numerous tools to perform Transfer Learning and Domain Adaptation.
+        
+        The purpose of the ADAPT library is to facilitate the access to transfer learning algorithms for a large public, including industrial players. ADAPT is specifically designed for [Scikit-learn](https://scikit-learn.org/stable/) and [Tensorflow](https://www.tensorflow.org/) users with a "user-friendly" approach. All objects in ADAPT implement the ***fit***, ***predict*** and ***score*** methods like any scikit-learn object. A very detailed documentation with several examples is provided:
+        
+        :arrow_right: [Documentation](https://adapt-python.github.io/adapt/)
+        
+        <table>
+          <tr valign="top">
+            <td width="50%" >
+                <a href="https://adapt-python.github.io/adapt/examples/Sample_bias_example.html">
+                    <br>
+                    <b>Sample bias correction</b>
+                    <br>
+                    <br>
+                    <img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/sample_bias_corr_img.png">
+                </a>
+            </td>
+            <td width="50%">
+                <a href="https://adapt-python.github.io/adapt/examples/Flowers_example.html">
+                    <br>
+                    <b>Model-based Transfer</b>
+                    <br>
+                    <br>
+                    <img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/finetuned.png">
+                </a>
+            </td>
+          </tr>
+          <tr valign="top">
+            <td width="50%">
+                <a href="https://adapt-python.github.io/adapt/examples/Office_example.html">
+                    <br>
+                    <b>Deep Domain Adaptation</b>
+                    <br>
+                    <br>
+                    <img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/office_item.png">
+                </a>
+            </td>
+            <td width="50%">
+                <a href="https://adapt-python.github.io/adapt/examples/Multi_fidelity.html">
+                    <br>
+                    <b>Multi-Fidelity Transfer</b>
+                    <br>
+                    <br>
+                    <img src="https://raw.githubusercontent.com/adapt-python/adapt/a490a5c4cefb80d6222bc831a8cc25b2f65221ce/docs/_static/images/multifidelity_setup.png">
+                </a>
+            </td>
+          </tr>
+        </table>
+        
+        ## Installation and Usage
+        
+        This package is available on [Pypi](https://pypi.org/project/adapt) and can be installed with the following command line: 
+        
+        ```
+        pip install adapt
+        ```
+        
+        The following dependencies are required and will be installed with the library:
+        - `numpy`
+        - `scipy`
+        - `tensorflow` (>= 2.0)
+        - `scikit-learn`
+        - `cvxopt`
+        
+        If for some reason, these packages failed to install, you can do it manually with:
+        
+        ```
+        pip install numpy scipy tensorflow scikit-learn cvxopt
+        ```
+        
+        Finally import the module in your python scripts with:
+        
+        ```python
+        import adapt
+        ```
+        
+        A simple example of usage is given in the [Quick-Start](#Quick-Start) below.
+        
+        
+        ## ADAPT Guideline
+        
+        The transfer learning methods implemented in ADAPT can be seen as scikit-learn "Meta-estimators" or tensorflow "Custom Model":
+        
+        <table>
+        <tr valign="top">
+        <td width="33%" >
+        <br>
+        <b>Adapt Estimator</b>
+        <br>
+        <br>
+        	
+        ```python
+        AdaptEstimator(
+        	estimator = """A scikit-learn estimator
+        	            (like Ridge(alpha=1.) for example)
+        		    or a Tensorflow Model""",
+        	Xt = "The target input features",
+        	yt = "The target output labels (if any)",
+        	**params = "Hyper-parameters of the AdaptEstimator"
+        )
+        ```
+        	
+        <td width="33%">
+        <br>
+        <b>Deep Adapt Estimator</b>
+        <br>
+        <br>
+        
+        	
+        ```python
+        DeepAdaptEstimator(
+        	encoder = "A Tensorflow Model (if required)",
+        	task = "A Tensorflow Model (if required)",
+        	discriminator = "A Tensorflow Model (if required)",
+        	Xt = "The target input features",
+        	yt = "The target output labels (if any)",
+        	**params = """Hyper-parameters of the DeepAdaptEstimator and
+        		      the compile and fit params (optimizer, epochs...)"""
+        )
+        ```
+        	
+        
+        </td>
+        	
+        	
+        </td>
+        <td width="33%">
+        <br>
+        <b>Scikit-learn Meta-Estimator</b>
+        <br>
+        <br>
+        	
+        ```python
+        SklearnMetaEstimator(
+        	base_estimator = """A scikit-learn estimator
+        			 (like Ridge(alpha=1.) for example)""",
+        	**params = "Hyper-parameters of the SklearnMetaEstimator"
+        )
+        ```
+        	
+        
+        </td>
+        </tr>
+        </table>
+        
+        
+        As you can see, the main difference between ADAPT models and scikit-learn and tensorflow objects is the two arguments `Xt, yt` which refer to the target data. Indeed, in classical machine learning, one assumes that the fitted model is applied on data distributed according to the training distribution. This is why, in this setting, one performs cross-validation and splits uniformly the training set to evaluate a model.
+        
+        In the transfer learning framework, however, one assumes that the target data (on which the model will be used at the end) are not distributed like the source training data. Moreover, one assumes that the target distribution can be estimated and compared to the training distribution. Either because a small sample of labeled target data `Xt, yt` is available or because a large sample of unlabeled target data `Xt` is at one's disposal.
+        
+        Thus, the transfer learning models from the ADAPT library can be seen as machine learning models that are fitted with a specific target in mind. This target is different but somewhat related to the training data. This is generally achieved by a transformation of the input features (see [feature-based transfer](https://adapt-python.github.io/adapt/contents.html#adapt-feature-based-feature-based-methods)) or by importance weighting (see [instance-based transfer](https://adapt-python.github.io/adapt/contents.html#adapt-instance-based)). In some cases, the training data are no more available but one aims at fine-tuning a pre-trained source model on a new target dataset (see [parameter-based transfer](https://adapt-python.github.io/adapt/contents.html#adapt-parameter-based)).
+        
+        
+        ## Navigate into ADAPT
+        
+        The ADAPT library proposes numerous transfer algorithms and it can be hard to know which algorithm is best suited for a particular problem. If you do not know which algorithm to choose, this [flowchart](https://adapt-python.github.io/adapt/map.html) may help you:
+        
+        [<img src="https://github.com/adapt-python/adapt/raw/master/src_docs/_static/images/thumbnai_flowchart.PNG" width=30%>](https://adapt-python.github.io/adapt/map.html)
+        
+        
+        ## Quick Start
+        
+        Here is a simple usage example of the ADAPT library. This is a simulation of a 1D sample bias problem with binary classification task. The source input data are distributed according to a Gaussian distribution centered in -1 with standard deviation of 2. The target data are drawn from Gaussian distribution centered in 1 with standard deviation of 2. The output labels are equal to 1 in the interval [-1, 1] and 0 elsewhere. We apply the transfer method [KMM](https://adapt-python.github.io/adapt/generated/adapt.instance_based.KMM.html) which is an unsupervised instance-based algorithm.
+        
+        ```python
+        # Import standard libraries
+        import numpy as np
+        from sklearn.linear_model import LogisticRegression
+        
+        # Import KMM method form adapt.instance_based module
+        from adapt.instance_based import KMM
+        
+        np.random.seed(0)
+        
+        # Create source dataset (Xs ~ N(-1, 2))
+        # ys = 1 for ys in [-1, 1] else, ys = 0
+        Xs = np.random.randn(1000, 1)*2-1
+        ys = (Xs[:, 0] > -1.) & (Xs[:, 0] < 1.)
+        
+        # Create target dataset (Xt ~ N(1, 2)), yt ~ ys
+        Xt = np.random.randn(1000, 1)*2+1
+        yt = (Xt[:, 0] > -1.) & (Xt[:, 0] < 1.)
+        
+        # Instantiate and fit a source only model for comparison
+        src_only = LogisticRegression(penalty="none")
+        src_only.fit(Xs, ys)
+        
+        # Instantiate a KMM model : estimator and target input
+        # data Xt are given as parameters with the kernel parameters
+        adapt_model = KMM(
+            estimator=LogisticRegression(penalty="none"), 
+            Xt=Xt,
+            kernel="rbf",  # Gaussian kernel
+            gamma=1.,     # Bandwidth of the kernel
+            verbose=0,
+            random_state=0
+        )
+        
+        # Fit the model.
+        adapt_model.fit(Xs, ys);
+        
+        # Get the score on target data
+        adapt_model.score(Xt, yt)
+        ```
+        ```python
+        >>> 0.574
+        ```
+        
+        | <img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/results_qs.png"> | 
+        |:--:| 
+        | **Quick-Start Plotting Results**. *The dotted and dashed lines are respectively the class separation of the "source only" and KMM models. Note that the predicted positive class is on the right of the dotted line for the "source only" model but on the left of the dashed line for KMM. (The code for plotting the Figure is available [here](https://adapt-python.github.io/adapt/examples/Quick_start.html))* |
+        
+        
+        ## Contents
+        
+        ADAPT package is divided in three sub-modules containing the following domain adaptation methods:
+        
+        ### Feature-based methods
+        
+        <img src="https://raw.githubusercontent.com/adapt-python/adapt/a490a5c4cefb80d6222bc831a8cc25b2f65221ce/docs/_static/images/feature_based.png">
+        
+        - [FA](https://adapt-python.github.io/adapt/generated/adapt.feature_based.FA.html) (*Frustratingly Easy Domain Adaptation*) [[paper]](https://arxiv.org/pdf/0907.1815.pdf)
+        - [SA](https://adapt-python.github.io/adapt/generated/adapt.feature_based.SA.html) (*Subspace Alignment*) [[paper]](https://arxiv.org/abs/1409.5241)
+        - [fMMD](https://adapt-python.github.io/adapt/generated/adapt.feature_based.fMMD.html) (*feature Selection with MMD*) [[paper]](https://www.cs.cmu.edu/afs/cs/Web/People/jgc/publication/Feature%20Selection%20for%20Transfer%20Learning.pdf)
+        - [DANN](https://adapt-python.github.io/adapt/generated/adapt.feature_based.DANN.html) (*Discriminative Adversarial Neural Network*) [[paper]](https://jmlr.org/papers/volume17/15-239/15-239.pdf)
+        - [ADDA](https://adapt-python.github.io/adapt/generated/adapt.feature_based.ADDA.html) (*Adversarial Discriminative Domain Adaptation*) [[paper]](https://arxiv.org/pdf/1702.05464.pdf)
+        - [CORAL](https://adapt-python.github.io/adapt/generated/adapt.feature_based.CORAL.html) (*CORrelation ALignment*) [[paper]](https://arxiv.org/pdf/1511.05547.pdf)
+        - [DeepCORAL](https://adapt-python.github.io/adapt/generated/adapt.feature_based.DeepCORAL.html) (*Deep CORrelation ALignment*) [[paper]](https://arxiv.org/pdf/1607.01719.pdf)
+        - [MCD](https://adapt-python.github.io/adapt/generated/adapt.feature_based.MCD.html) (*Maximum Classifier Discrepancy*) [[paper]](https://arxiv.org/pdf/1712.02560.pdf)
+        - [MDD](https://adapt-python.github.io/adapt/generated/adapt.feature_based.MDD.html) (*Margin Disparity Discrepancy*) [[paper]](https://arxiv.org/pdf/1904.05801.pdf)
+        - [WDGRL](https://adapt-python.github.io/adapt/generated/adapt.feature_based.WDGRL.html) (*Wasserstein Distance Guided Representation Learning*) [[paper]](https://arxiv.org/pdf/1707.01217.pdf)
+        - [CDAN](https://adapt-python.github.io/adapt/generated/adapt.feature_based.CDAN.html) (*Conditional Adversarial Domain Adaptation*) [[paper]](https://arxiv.org/pdf/1705.10667.pdf)
+        - [CCSA](https://adapt-python.github.io/adapt/generated/adapt.feature_based.CCSA.html) (*Classification and Contrastive Semantic Alignment*) [[paper]](https://arxiv.org/abs/1709.10190)
+        
+        ### Instance-based methods
+        
+        <img src="https://raw.githubusercontent.com/adapt-python/adapt/a490a5c4cefb80d6222bc831a8cc25b2f65221ce/docs/_static/images/instance_based.png">
+        
+        - [LDM](https://adapt-python.github.io/adapt/generated/adapt.instance_based.LDM.html) (*Linear Discrepancy Minimization*) [[paper]](https://arxiv.org/pdf/0902.3430.pdf)
+        - [KMM](https://adapt-python.github.io/adapt/generated/adapt.instance_based.KMM.html) (*Kernel Mean Matching*) [[paper]](https://proceedings.neurips.cc/paper/2006/file/a2186aa7c086b46ad4e8bf81e2a3a19b-Paper.pdf)
+        - [KLIEP](https://adapt-python.github.io/adapt/generated/adapt.instance_based.KLIEP.html) (*Kullbackâ€“Leibler Importance Estimation Procedure*) [[paper]](https://proceedings.neurips.cc/paper/2007/file/be83ab3ecd0db773eb2dc1b0a17836a1-Paper.pdf)
+        - [TrAdaBoost](https://adapt-python.github.io/adapt/generated/adapt.instance_based.TrAdaBoost.html) (*Transfer AdaBoost*) [[paper]](https://cse.hkust.edu.hk/~qyang/Docs/2007/tradaboost.pdf)
+        - [TrAdaBoostR2](https://adapt-python.github.io/adapt/generated/adapt.instance_based.TrAdaBoostR2.html) (*Transfer AdaBoost for Regression*) [[paper]](https://www.cs.utexas.edu/~dpardoe/papers/ICML10.pdf)
+        - [TwoStageTrAdaBoostR2](https://adapt-python.github.io/adapt/generated/adapt.instance_based.TwoStageTrAdaBoostR2.html) (*Two Stage Transfer AdaBoost for Regression*) [[paper]](https://www.cs.utexas.edu/~dpardoe/papers/ICML10.pdf)
+        - [NearestNeighborsWeighting](https://adapt-python.github.io/adapt/generated/adapt.instance_based.NearestNeighborsWeighting.html) (*Nearest Neighbors Weighting*) [[paper]](https://arxiv.org/pdf/2102.02291.pdf)
+        - [WANN](https://adapt-python.github.io/adapt/generated/adapt.instance_based.WANN.html) (*Weighting Adversarial Neural Network*) [[paper]](https://arxiv.org/pdf/2006.08251.pdf)
+        
+        ### Parameter-based methods
+        
+        <img src="https://raw.githubusercontent.com/adapt-python/adapt/a490a5c4cefb80d6222bc831a8cc25b2f65221ce/docs/_static/images/parameter_based.png">
+        
+        - [RegularTransferLR](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.RegularTransferLR.html) (*Regular Transfer with Linear Regression*) [[paper]](https://www.microsoft.com/en-us/research/wp-content/uploads/2004/07/2004-chelba-emnlp.pdf)
+        - [RegularTransferLC](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.RegularTransferLC.html) (*Regular Transfer with Linear Classification*) [[paper]](https://www.microsoft.com/en-us/research/wp-content/uploads/2004/07/2004-chelba-emnlp.pdf)
+        - [RegularTransferNN](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.RegularTransferNN.html) (*Regular Transfer with Neural Network*) [[paper]](https://hal.inria.fr/hal-00911179v1/document)
+        - [FineTuning](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.FineTuning.html) (*Fine-Tuning*) [[paper]](https://hal.inria.fr/hal-00911179v1/document)
+        - [TransferTreeClassifier](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.TransferTreeClassifier.html) (*Transfer Tree Classifier*) [[paper]](https://ieeexplore.ieee.org/document/8995296)
+        - [TransferTreeForest](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.TransferTreeForest.html) (*Transfer Tree Forest*) [[paper]](https://ieeexplore.ieee.org/document/8995296)
+        
+        
+        ## Reference
+        
+        If you use this library in your research, please cite ADAPT using the following reference: https://arxiv.org/pdf/2107.03049.pdf
+        
+        ```
+        @article{de2021adapt,
+        	  title={ADAPT: Awesome Domain Adaptation Python Toolbox},
+        	  author={de Mathelin, Antoine and Deheeger, Fran{\c{c}}ois and Richard, Guillaume and Mougeot, Mathilde and Vayatis, Nicolas},
+        	  journal={arXiv preprint arXiv:2107.03049},
+        	  year={2021}
+        	}
+        ```
+        
+        ## Acknowledgement
+        
+        This work has been funded by Michelin and the Industrial Data Analytics and Machine Learning chair from ENS Paris-Saclay, Borelli center.
+        
+        [<img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/michelin.png" width=200px alt="Michelin">](https://www.michelin.com/) [<img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/idaml.jpg" width=200px alt="IDAML">](https://centreborelli.ens-paris-saclay.fr/fr/chaire-idaml) [<img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/borelli.jpg" alt="Centre Borelli" width=150px>](https://centreborelli.ens-paris-saclay.fr/fr)
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# ADAPT
-
-[![PyPI version](https://badge.fury.io/py/adapt.svg)](https://pypi.org/project/adapt)
-[![Build Status](https://github.com/adapt-python/adapt/workflows/build/badge.svg)](https://github.com/adapt-python/adapt/actions)
-[![Python Version](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8|%203.9-blue)](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8|%203.9-blue)
-[![Codecov Status](https://codecov.io/gh/adapt-python/adapt/branch/master/graph/badge.svg?token=IWQXMYGY2Q)](https://codecov.io/gh/adapt-python/adapt)
-
-**A**wesome **D**omain **A**daptation **P**ython **T**oolbox
-
----
-
-ADAPT is an open source library providing numerous tools to perform Transfer Learning and Domain Adaptation.
-
-The purpose of the ADAPT library is to facilitate the access to transfer learning algorithms for a large public, including industrial players. ADAPT is specifically designed for [Scikit-learn](https://scikit-learn.org/stable/) and [Tensorflow](https://www.tensorflow.org/) users with a "user-friendly" approach. All objects in ADAPT implement the ***fit***, ***predict*** and ***score*** methods like any scikit-learn object. A very detailed documentation with several examples is provided:
-
-:arrow_right: [Documentation](https://adapt-python.github.io/adapt/)
-
-<table>
-  <tr valign="top">
-    <td width="50%" >
-        <a href="https://adapt-python.github.io/adapt/examples/Sample_bias_example.html">
-            <br>
-            <b>Sample bias correction</b>
-            <br>
-            <br>
-            <img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/sample_bias_corr_img.png">
-        </a>
-    </td>
-    <td width="50%">
-        <a href="https://adapt-python.github.io/adapt/examples/Flowers_example.html">
-            <br>
-            <b>Model-based Transfer</b>
-            <br>
-            <br>
-            <img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/finetuned.png">
-        </a>
-    </td>
-  </tr>
-  <tr valign="top">
-    <td width="50%">
-        <a href="https://adapt-python.github.io/adapt/examples/Office_example.html">
-            <br>
-            <b>Deep Domain Adaptation</b>
-            <br>
-            <br>
-            <img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/office_item.png">
-        </a>
-    </td>
-    <td width="50%">
-        <a href="https://adapt-python.github.io/adapt/examples/Multi_fidelity.html">
-            <br>
-            <b>Multi-Fidelity Transfer</b>
-            <br>
-            <br>
-            <img src="https://raw.githubusercontent.com/adapt-python/adapt/a490a5c4cefb80d6222bc831a8cc25b2f65221ce/docs/_static/images/multifidelity_setup.png">
-        </a>
-    </td>
-  </tr>
-</table>
-
-## Installation and Usage
-
-This package is available on [Pypi](https://pypi.org/project/adapt) and can be installed with the following command line: 
-
-```
-pip install adapt
-```
-
-The following dependencies are required and will be installed with the library:
-- `numpy`
-- `scipy`
-- `tensorflow` (>= 2.0)
-- `scikit-learn`
-- `cvxopt`
-
-If for some reason, these packages failed to install, you can do it manually with:
-
-```
-pip install numpy scipy tensorflow scikit-learn cvxopt
-```
-
-Finally import the module in your python scripts with:
-
-```python
-import adapt
-```
-
-A simple example of usage is given in the [Qick-Start](#Quick-Start) below.
-
-
-## ADAPT Guideline
-
-The transfer learning methods implemented in ADAPT can be seen as scikit-learn "Meta-estimators" or tensorflow "Custom Model":
-
-<table>
-<tr valign="top">
-<td width="33%" >
-<br>
-<b>Adapt Estimator</b>
-<br>
-<br>
-	
-```python
-AdaptEstimator(
-	estimator = """A scikit-learn estimator
-	            (like Ridge(alpha=1.) for example)
-		    or a Tensorflow Model""",
-	Xt = "The target input features",
-	yt = "The target output labels (if any)",
-	**params = "Hyper-parameters of the AdaptEstimator"
-)
-```
-	
-<td width="33%">
-<br>
-<b>Deep Adapt Estimator</b>
-<br>
-<br>
-
-	
-```python
-DeepAdaptEstimator(
-	encoder = "A Tensorflow Model (if required)",
-	task = "A Tensorflow Model (if required)",
-	discriminator = "A Tensorflow Model (if required)",
-	Xt = "The target input features",
-	yt = "The target output labels (if any)",
-	**params = """Hyper-parameters of the DeepAdaptEstimator and
-		      the compile and fit params (optimizer, epochs...)"""
-)
-```
-	
-
-</td>
-	
-	
-</td>
-<td width="33%">
-<br>
-<b>Scikit-learn Meta-Estimator</b>
-<br>
-<br>
-	
-```python
-SklearnMetaEstimator(
-	base_estimator = """A scikit-learn estimator
-			 (like Ridge(alpha=1.) for example)""",
-	**params = "Hyper-parameters of the SklearnMetaEstimator"
-)
-```
-	
-
-</td>
-</tr>
-</table>
-
-
-As you can see, the main difference between ADAPT models and scikit-learn and tensorflow objects is the two arguments `Xt, yt` which refer to the target data. Indeed, in classical machine learning, one assumes that the fitted model is applied on data distributed according to the training distribution. This is why, in this setting, one performs cross-validation and splits uniformly the training set to evaluate a model.
-
-In the transfer learning framework, however, one assumes that the target data (on which the model will be used at the end) are not distributed like the source training data. Moreover, one assumes that the target distribution can be estimated and compared to the training distribution. Either because a small sample of labeled target data `Xt, yt` is avalaible or because a large sample of unlabeled target data `Xt` is at one's disposal.
-
-Thus, the transfer learning models from the ADAPT library can be seen as machine learning models that are fitted with a specific target in mind. This target is different but somewhat related to the training data. This is generally achieved by a transformation of the input features (see [feature-based transfer](https://adapt-python.github.io/adapt/contents.html#adapt-feature-based-feature-based-methods)) or by importance weighting (see [instance-based transfer](https://adapt-python.github.io/adapt/contents.html#adapt-instance-based)). In some cases, the training data are no more available but one aims at fine-tuning a pre-trained source model on a new target dataset (see [parameter-based transfer](https://adapt-python.github.io/adapt/contents.html#adapt-parameter-based)).
-
-
-## Navigate into ADAPT
-
-The ADAPT library proposes numerous transfer algorithms and it can be hard to know which algorithm is best suited for a particular problem. If you do not know which algorithm to choose, this [flowchart](https://adapt-python.github.io/adapt/map.html) may help you:
-
-[<img src="https://github.com/adapt-python/adapt/raw/master/src_docs/_static/images/thumbnai_flowchart.PNG" width=30%>](https://adapt-python.github.io/adapt/map.html)
-
-
-## Quick Start
-
-Here is a simple usage example of the ADAPT library. This is a simulation of a 1D sample bias problem with binary classfication task. The source input data are distributed according to a Gaussian distribution centered in -1 with standard deviation of 2. The target data are drawn from Gaussian distribution centered in 1 with standard deviation of 2. The output labels are equal to 1 in the interval [-1, 1] and 0 elsewhere. We apply the transfer method [KMM](https://adapt-python.github.io/adapt/generated/adapt.instance_based.KMM.html) which is an unsupervised instance-based algortihm.
-
-```python
-# Import standard librairies
-import numpy as np
-from sklearn.linear_model import LogisticRegression
-
-# Import KMM method form adapt.instance_based module
-from adapt.instance_based import KMM
-
-np.random.seed(0)
-
-# Create source dataset (Xs ~ N(-1, 2))
-# ys = 1 for ys in [-1, 1] else, ys = 0
-Xs = np.random.randn(1000, 1)*2-1
-ys = (Xs[:, 0] > -1.) & (Xs[:, 0] < 1.)
-
-# Create target dataset (Xt ~ N(1, 2)), yt ~ ys
-Xt = np.random.randn(1000, 1)*2+1
-yt = (Xt[:, 0] > -1.) & (Xt[:, 0] < 1.)
-
-# Instantiate and fit a source only model for comparison
-src_only = LogisticRegression(penalty="none")
-src_only.fit(Xs, ys)
-
-# Instantiate a KMM model : estimator and target input
-# data Xt are given as parameters with the kernel parameters
-adapt_model = KMM(
-    estimator=LogisticRegression(penalty="none"), 
-    Xt=Xt,
-    kernel="rbf",  # Gaussian kernel
-    gamma=1.,     # Bandwidth of the kernel
-    verbose=0,
-    random_state=0
-)
-
-# Fit the model.
-adapt_model.fit(Xs, ys);
-
-# Get the score on target data
-adapt_model.score(Xt, yt)
-```
-```python
->>> 0.574
-```
-
-| <img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/results_qs.png"> | 
-|:--:| 
-| **Quick-Start Plotting Results**. *The dotted and dashed lines are respectively the class separation of the "source only" and KMM models. Note that the predicted positive class is on the right of the dotted line for the "source only" model but on the left of the dashed line for KMM. (The code for plotting the Figure is available [here](https://adapt-python.github.io/adapt/examples/Quick_start.html))* |
-
-
-## Contents
-
-ADAPT package is divided in three sub-modules containing the following domain adaptation methods:
-
-### Feature-based methods
-
-<img src="https://raw.githubusercontent.com/adapt-python/adapt/a490a5c4cefb80d6222bc831a8cc25b2f65221ce/docs/_static/images/feature_based.png">
-
-- [FA](https://adapt-python.github.io/adapt/generated/adapt.feature_based.FA.html) (*Frustratingly Easy Domain Adaptation*) [[paper]](https://arxiv.org/pdf/0907.1815.pdf)
-- [SA](https://adapt-python.github.io/adapt/generated/adapt.feature_based.SA.html) (*Subspace Alignment*) [[paper]](https://arxiv.org/abs/1409.5241)
-- [fMMD](https://adapt-python.github.io/adapt/generated/adapt.feature_based.SA.html) (*feature Selection with MMD*) [[paper]](https://www.cs.cmu.edu/afs/cs/Web/People/jgc/publication/Feature%20Selection%20for%20Transfer%20Learning.pdf)
-- [DANN](https://adapt-python.github.io/adapt/generated/adapt.feature_based.DANN.html) (*Discriminative Adversarial Neural Network*) [[paper]](https://jmlr.org/papers/volume17/15-239/15-239.pdf)
-- [ADDA](https://adapt-python.github.io/adapt/generated/adapt.feature_based.ADDA.html) (*Adversarial Discriminative Domain Adaptation*) [[paper]](https://arxiv.org/pdf/1702.05464.pdf)
-- [CORAL](https://adapt-python.github.io/adapt/generated/adapt.feature_based.CORAL.html) (*CORrelation ALignment*) [[paper]](https://arxiv.org/pdf/1511.05547.pdf)
-- [DeepCORAL](https://adapt-python.github.io/adapt/generated/adapt.feature_based.DeepCORAL.html) (*Deep CORrelation ALignment*) [[paper]](https://arxiv.org/pdf/1607.01719.pdf)
-- [MCD](https://adapt-python.github.io/adapt/generated/adapt.feature_based.MCD.html) (*Maximum Classifier Discrepancy*) [[paper]](https://arxiv.org/pdf/1712.02560.pdf)
-- [MDD](https://adapt-python.github.io/adapt/generated/adapt.feature_based.MDD.html) (*Margin Disparity Discrepancy*) [[paper]](https://arxiv.org/pdf/1904.05801.pdf)
-- [WDGRL](https://adapt-python.github.io/adapt/generated/adapt.feature_based.WDGRL.html) (*Wasserstein Distance Guided Representation Learning*) [[paper]](https://arxiv.org/pdf/1707.01217.pdf)
-- [CDAN](https://adapt-python.github.io/adapt/generated/adapt.feature_based.CDAN.html) (*Conditional Adversarial Domain Adaptation*) [[paper]](https://arxiv.org/pdf/1705.10667.pdf)
-- [CCSA](https://adapt-python.github.io/adapt/generated/adapt.feature_based.CCSA.html) (*Classification and Contrastive Semantic Alignment*) [[paper]](https://arxiv.org/abs/1709.10190)
-
-### Instance-based methods
-
-<img src="https://raw.githubusercontent.com/adapt-python/adapt/a490a5c4cefb80d6222bc831a8cc25b2f65221ce/docs/_static/images/instance_based.png">
-
-- [LDM](https://adapt-python.github.io/adapt/generated/adapt.instance_based.LDM.html) (*Linear Discrepancy Minimization*) [[paper]](https://arxiv.org/pdf/0902.3430.pdf)
-- [KMM](https://adapt-python.github.io/adapt/generated/adapt.instance_based.KMM.html) (*Kernel Mean Matching*) [[paper]](https://proceedings.neurips.cc/paper/2006/file/a2186aa7c086b46ad4e8bf81e2a3a19b-Paper.pdf)
-- [KLIEP](https://adapt-python.github.io/adapt/generated/adapt.instance_based.KLIEP.html) (*Kullbackâ€“Leibler Importance Estimation Procedure*) [[paper]](https://proceedings.neurips.cc/paper/2007/file/be83ab3ecd0db773eb2dc1b0a17836a1-Paper.pdf)
-- [TrAdaBoost](https://adapt-python.github.io/adapt/generated/adapt.instance_based.TrAdaBoost.html) (*Transfer AdaBoost*) [[paper]](https://cse.hkust.edu.hk/~qyang/Docs/2007/tradaboost.pdf)
-- [TrAdaBoostR2](https://adapt-python.github.io/adapt/generated/adapt.instance_based.TrAdaBoostR2.html) (*Transfer AdaBoost for Regression*) [[paper]](https://www.cs.utexas.edu/~dpardoe/papers/ICML10.pdf)
-- [TwoStageTrAdaBoostR2](https://adapt-python.github.io/adapt/generated/adapt.instance_based.TwoStageTrAdaBoostR2.html) (*Two Stage Transfer AdaBoost for Regression*) [[paper]](https://www.cs.utexas.edu/~dpardoe/papers/ICML10.pdf)
-- [NearestNeighborsWeighting](https://adapt-python.github.io/adapt/generated/adapt.instance_based.NearestNeighborsWeighting.html) (*Nearest Neighbors Weighting*) [[paper]](https://arxiv.org/pdf/2102.02291.pdf)
-- [WANN](https://adapt-python.github.io/adapt/generated/adapt.instance_based.WANN.html) (*Weighting Adversarial Neural Network*) [[paper]](https://arxiv.org/pdf/2006.08251.pdf)
-
-### Parameter-based methods
-
-<img src="https://raw.githubusercontent.com/adapt-python/adapt/a490a5c4cefb80d6222bc831a8cc25b2f65221ce/docs/_static/images/parameter_based.png">
-
-- [RegularTransferLR](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.RegularTransferLR.html) (*Regular Transfer with Linear Regression*) [[paper]](https://www.microsoft.com/en-us/research/wp-content/uploads/2004/07/2004-chelba-emnlp.pdf)
-- [RegularTransferLC](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.RegularTransferLC.html) (*Regular Transfer with Linear Classification*) [[paper]](https://www.microsoft.com/en-us/research/wp-content/uploads/2004/07/2004-chelba-emnlp.pdf)
-- [RegularTransferNN](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.RegularTransferNN.html) (*Regular Transfer with Neural Network*) [[paper]](https://hal.inria.fr/hal-00911179v1/document)
-- [FineTuning](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.FineTuning.html) (*Fine-Tuning*) [[paper]](https://hal.inria.fr/hal-00911179v1/document)
-- [TransferTreeClassifier](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.TransferTreeClassifier.html) (*Transfer Tree Classifier*) [[paper]](https://ieeexplore.ieee.org/document/8995296)
-- [TransferTreeForest](https://adapt-python.github.io/adapt/generated/adapt.parameter_based.TransferTreeForest.html) (*Transfer Tree Forest*) [[paper]](https://ieeexplore.ieee.org/document/8995296)
-
-
-## Reference
-
-If you use this library in your research, please cite ADAPT using the following reference: https://arxiv.org/pdf/2107.03049.pdf
-
-```
-@article{de2021adapt,
-	  title={ADAPT: Awesome Domain Adaptation Python Toolbox},
-	  author={de Mathelin, Antoine and Deheeger, Fran{\c{c}}ois and Richard, Guillaume and Mougeot, Mathilde and Vayatis, Nicolas},
-	  journal={arXiv preprint arXiv:2107.03049},
-	  year={2021}
-	}
-```
-
-## Acknowledgement
-
-This work has been funded by Michelin and the Industrial Data Analytics and Machine Learning chair from ENS Paris-Saclay, Borelli center.
-
-[<img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/michelin.png" width=200px alt="Michelin">](https://www.michelin.com/) [<img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/idaml.jpg" width=200px alt="IDAML">](https://centreborelli.ens-paris-saclay.fr/fr/chaire-idaml) [<img src="https://github.com/adapt-python/adapt/raw/41c13055facc0733faf49c4e3979709e82be10e5/docs/_static/images/borelli.jpg" alt="Centre Borelli" width=150px>](https://centreborelli.ens-paris-saclay.fr/fr)
-
-
```

#### html2text {}

```diff
@@ -1,15 +1,14 @@
-Metadata-Version: 2.1 Name: adapt Version: 0.4.2 Summary: Awesome Domain
+Metadata-Version: 2.1 Name: adapt Version: 0.4.3 Summary: Awesome Domain
 Adaptation Python Toolbox for Tensorflow and Scikit-learn Home-page: https://
 github.com/adapt-python/adapt.git Author: Antoine de Mathelin Author-email:
-antoine.demat@gmail.com License: BSD-2 Platform: UNKNOWN Description-Content-
-Type: text/markdown License-File: LICENSE.txt # ADAPT [![PyPI version](https://
-badge.fury.io/py/adapt.svg)](https://pypi.org/project/adapt) [![Build Status]
-(https://github.com/adapt-python/adapt/workflows/build/badge.svg)](https://
-github.com/adapt-python/adapt/actions) [![Python Version](https://
+antoine.demat@gmail.com License: BSD-2 Description: # ADAPT [![PyPI version]
+(https://badge.fury.io/py/adapt.svg)](https://pypi.org/project/adapt) [![Build
+Status](https://github.com/adapt-python/adapt/workflows/build/badge.svg)]
+(https://github.com/adapt-python/adapt/actions) [![Python Version](https://
 img.shields.io/badge/python-3.6%20|%203.7%20|%203.8|%203.9-blue)](https://
 img.shields.io/badge/python-3.6%20|%203.7%20|%203.8|%203.9-blue) [![Codecov
 Status](https://codecov.io/gh/adapt-python/adapt/branch/master/graph/
 badge.svg?token=IWQXMYGY2Q)](https://codecov.io/gh/adapt-python/adapt)
 **A**wesome **D**omain **A**daptation **P**ython **T**oolbox --- ADAPT is an
 open source library providing numerous tools to perform Transfer Learning and
 Domain Adaptation. The purpose of the ADAPT library is to facilitate the access
@@ -39,17 +38,17 @@
 ## Installation and Usage This package is available on [Pypi](https://pypi.org/
 project/adapt) and can be installed with the following command line: ``` pip
 install adapt ``` The following dependencies are required and will be installed
 with the library: - `numpy` - `scipy` - `tensorflow` (>= 2.0) - `scikit-learn`
 - `cvxopt` If for some reason, these packages failed to install, you can do it
 manually with: ``` pip install numpy scipy tensorflow scikit-learn cvxopt ```
 Finally import the module in your python scripts with: ```python import adapt
-``` A simple example of usage is given in the [Qick-Start](#Quick-Start) below.
-## ADAPT Guideline The transfer learning methods implemented in ADAPT can be
-seen as scikit-learn "Meta-estimators" or tensorflow "Custom Model":
+``` A simple example of usage is given in the [Quick-Start](#Quick-Start)
+below. ## ADAPT Guideline The transfer learning methods implemented in ADAPT
+can be seen as scikit-learn "Meta-estimators" or tensorflow "Custom Model":
 
 Adapt Estimator            Deep Adapt Estimator       Scikit-learn Meta-
                                                       Estimator
 ```python AdaptEstimator   ```python
 ( estimator = """A scikit- DeepAdaptEstimator         ```python
 learn estimator (like      ( encoder = "A Tensorflow  SklearnMetaEstimator
 Ridge(alpha=1.) for        Model (if required)", task ( base_estimator = """A
@@ -71,15 +70,15 @@
 is applied on data distributed according to the training distribution. This is
 why, in this setting, one performs cross-validation and splits uniformly the
 training set to evaluate a model. In the transfer learning framework, however,
 one assumes that the target data (on which the model will be used at the end)
 are not distributed like the source training data. Moreover, one assumes that
 the target distribution can be estimated and compared to the training
 distribution. Either because a small sample of labeled target data `Xt, yt` is
-avalaible or because a large sample of unlabeled target data `Xt` is at one's
+available or because a large sample of unlabeled target data `Xt` is at one's
 disposal. Thus, the transfer learning models from the ADAPT library can be seen
 as machine learning models that are fitted with a specific target in mind. This
 target is different but somewhat related to the training data. This is
 generally achieved by a transformation of the input features (see [feature-
 based transfer](https://adapt-python.github.io/adapt/contents.html#adapt-
 feature-based-feature-based-methods)) or by importance weighting (see
 [instance-based transfer](https://adapt-python.github.io/adapt/
@@ -90,21 +89,21 @@
 library proposes numerous transfer algorithms and it can be hard to know which
 algorithm is best suited for a particular problem. If you do not know which
 algorithm to choose, this [flowchart](https://adapt-python.github.io/adapt/
 map.html) may help you: [[https://github.com/adapt-python/adapt/raw/master/
 src_docs/_static/images/thumbnai_flowchart.PNG]](https://adapt-
 python.github.io/adapt/map.html) ## Quick Start Here is a simple usage example
 of the ADAPT library. This is a simulation of a 1D sample bias problem with
-binary classfication task. The source input data are distributed according to a
-Gaussian distribution centered in -1 with standard deviation of 2. The target
+binary classification task. The source input data are distributed according to
+a Gaussian distribution centered in -1 with standard deviation of 2. The target
 data are drawn from Gaussian distribution centered in 1 with standard deviation
 of 2. The output labels are equal to 1 in the interval [-1, 1] and 0 elsewhere.
 We apply the transfer method [KMM](https://adapt-python.github.io/adapt/
 generated/adapt.instance_based.KMM.html) which is an unsupervised instance-
-based algortihm. ```python # Import standard librairies import numpy as np from
+based algorithm. ```python # Import standard libraries import numpy as np from
 sklearn.linear_model import LogisticRegression # Import KMM method form
 adapt.instance_based module from adapt.instance_based import KMM np.random.seed
 (0) # Create source dataset (Xs ~ N(-1, 2)) # ys = 1 for ys in [-1, 1] else, ys
 = 0 Xs = np.random.randn(1000, 1)*2-1 ys = (Xs[:, 0] > -1.) & (Xs[:, 0] < 1.) #
 Create target dataset (Xt ~ N(1, 2)), yt ~ ys Xt = np.random.randn(1000, 1)*2+1
 yt = (Xt[:, 0] > -1.) & (Xt[:, 0] < 1.) # Instantiate and fit a source only
 model for comparison src_only = LogisticRegression(penalty="none") src_only.fit
@@ -125,15 +124,15 @@
 methods: ### Feature-based methods [https://raw.githubusercontent.com/adapt-
 python/adapt/a490a5c4cefb80d6222bc831a8cc25b2f65221ce/docs/_static/images/
 feature_based.png] - [FA](https://adapt-python.github.io/adapt/generated/
 adapt.feature_based.FA.html) (*Frustratingly Easy Domain Adaptation*) [[paper]]
 (https://arxiv.org/pdf/0907.1815.pdf) - [SA](https://adapt-python.github.io/
 adapt/generated/adapt.feature_based.SA.html) (*Subspace Alignment*) [[paper]]
 (https://arxiv.org/abs/1409.5241) - [fMMD](https://adapt-python.github.io/
-adapt/generated/adapt.feature_based.SA.html) (*feature Selection with MMD*) [
+adapt/generated/adapt.feature_based.fMMD.html) (*feature Selection with MMD*) [
 [paper]](https://www.cs.cmu.edu/afs/cs/Web/People/jgc/publication/
 Feature%20Selection%20for%20Transfer%20Learning.pdf) - [DANN](https://adapt-
 python.github.io/adapt/generated/adapt.feature_based.DANN.html)
 (*Discriminative Adversarial Neural Network*) [[paper]](https://jmlr.org/
 papers/volume17/15-239/15-239.pdf) - [ADDA](https://adapt-python.github.io/
 adapt/generated/adapt.feature_based.ADDA.html) (*Adversarial Discriminative
 Domain Adaptation*) [[paper]](https://arxiv.org/pdf/1702.05464.pdf) - [CORAL]
@@ -206,8 +205,9 @@
 Awesome Domain Adaptation Python Toolbox}, author={de Mathelin, Antoine and
 Deheeger, Fran{\c{c}}ois and Richard, Guillaume and Mougeot, Mathilde and
 Vayatis, Nicolas}, journal={arXiv preprint arXiv:2107.03049}, year={2021} } ```
 ## Acknowledgement This work has been funded by Michelin and the Industrial
 Data Analytics and Machine Learning chair from ENS Paris-Saclay, Borelli
 center. [[Michelin]](https://www.michelin.com/) [[IDAML]](https://
 centreborelli.ens-paris-saclay.fr/fr/chaire-idaml) [[Centre Borelli]](https://
-centreborelli.ens-paris-saclay.fr/fr)
+centreborelli.ens-paris-saclay.fr/fr) Platform: UNKNOWN Description-Content-
+Type: text/markdown
```

### Comparing `adapt-0.4.2/adapt.egg-info/SOURCES.txt` & `adapt-0.4.3/adapt.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE.txt
 README.md
 setup.cfg
 setup.py
 adapt/__init__.py
 adapt/_tree_utils.py
 adapt/base.py
 adapt/metrics.py
@@ -40,8 +39,21 @@
 adapt/instance_based/_tradaboost.py
 adapt/instance_based/_ulsif.py
 adapt/instance_based/_wann.py
 adapt/parameter_based/__init__.py
 adapt/parameter_based/_finetuning.py
 adapt/parameter_based/_linint.py
 adapt/parameter_based/_regular.py
-adapt/parameter_based/_transfer_tree.py
+adapt/parameter_based/_transfer_tree.py
+tests/__init__.py
+tests/test_adda.py
+tests/test_cdan.py
+tests/test_coral.py
+tests/test_dann.py
+tests/test_kliep.py
+tests/test_kmm.py
+tests/test_mcd.py
+tests/test_mdd.py
+tests/test_regular.py
+tests/test_tradaboost.py
+tests/test_utils.py
+tests/test_wdgrl.py
```

### Comparing `adapt-0.4.2/setup.py` & `adapt-0.4.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='adapt',
-    version='0.4.2',
+    version='0.4.3',
     description='Awesome Domain Adaptation Python Toolbox for Tensorflow and Scikit-learn',
     url='https://github.com/adapt-python/adapt.git',
     author='Antoine de Mathelin',
     author_email='antoine.demat@gmail.com',
     license='BSD-2',
     packages=find_packages(exclude=["tests"]),
-    install_requires=["numpy>=1.16", "scipy>=1.0", "tensorflow>=2.0", "scikit-learn>=0.2", "cvxopt>=1.2"],
+    install_requires=["numpy>=1.16", "scipy>=1.0", "tensorflow<2.12", "scikit-learn>=0.2", "cvxopt<=1.3.0"],
     zip_safe=False,
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

