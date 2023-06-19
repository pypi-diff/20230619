# Comparing `tmp/probatus-2.0.0.tar.gz` & `tmp/probatus-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "probatus-2.0.0.tar", last modified: Thu Jun  8 12:53:18 2023, max compression
+gzip compressed data, was "probatus-2.0.1.tar", last modified: Mon Jun 19 07:44:05 2023, max compression
```

## Comparing `probatus-2.0.0.tar` & `probatus-2.0.1.tar`

### file list

```diff
@@ -1,84 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.690420 probatus-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-08 12:49:29.000000 probatus-2.0.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-08 12:53:18.690420 probatus-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-08 12:49:29.000000 probatus-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.682420 probatus-2.0.0/probatus/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.682420 probatus-2.0.0/probatus/binning/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/binning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16871 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/binning/binning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.682420 probatus-2.0.0/probatus/feature_elimination/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/feature_elimination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57143 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/feature_elimination/feature_elimination.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.682420 probatus-2.0.0/probatus/interpret/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/interpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20548 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/interpret/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/interpret/model_interpret.py
--rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/interpret/shap_dependence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.682420 probatus-2.0.0/probatus/metric_volatility/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/metric_volatility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/metric_volatility/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/metric_volatility/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29943 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/metric_volatility/volatility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.682420 probatus-2.0.0/probatus/missing_values/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/missing_values/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/missing_values/imputation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.686421 probatus-2.0.0/probatus/sample_similarity/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/sample_similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/sample_similarity/resemblance_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.686421 probatus-2.0.0/probatus/stat_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/stat_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/stat_tests/ad.py
--rw-r--r--   0 runner    (1001) docker     (123)    16996 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/stat_tests/distribution_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/stat_tests/es.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/stat_tests/ks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/stat_tests/psi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/stat_tests/sw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/stat_tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.686421 probatus-2.0.0/probatus/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/utils/arrayfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/utils/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/utils/missing_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/utils/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/utils/scoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/utils/shap_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.682420 probatus-2.0.0/probatus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-08 12:53:18.000000 probatus-2.0.0/probatus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-08 12:53:18.000000 probatus-2.0.0/probatus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:53:18.000000 probatus-2.0.0/probatus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:49:50.000000 probatus-2.0.0/probatus.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-08 12:53:18.000000 probatus-2.0.0/probatus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 12:53:18.000000 probatus-2.0.0/probatus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 12:53:18.690420 probatus-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-08 12:49:29.000000 probatus-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.678420 probatus-2.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.686421 probatus-2.0.0/tests/binning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/binning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/binning/test_binning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.686421 probatus-2.0.0/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/docs/test_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/docs/test_notebooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.690420 probatus-2.0.0/tests/interpret/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/interpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34609 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/interpret/test_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/interpret/test_model_interpret.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/interpret/test_shap_dependence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.690420 probatus-2.0.0/tests/metric_volatility/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/metric_volatility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/metric_volatility/test_metric_volatility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.690420 probatus-2.0.0/tests/sample_similarity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/sample_similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/sample_similarity/test_resemblance_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.690420 probatus-2.0.0/tests/stat_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/stat_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/stat_tests/test_distribution_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/stat_tests/test_stat_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/stat_tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.690420 probatus-2.0.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/utils/test_utils_array_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.726374 probatus-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-19 07:41:11.000000 probatus-2.0.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-06-19 07:44:05.726374 probatus-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-19 07:41:11.000000 probatus-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.718374 probatus-2.0.1/probatus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.718374 probatus-2.0.1/probatus/binning/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/binning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16871 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/binning/binning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.718374 probatus-2.0.1/probatus/feature_elimination/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/feature_elimination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57143 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/feature_elimination/feature_elimination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.722374 probatus-2.0.1/probatus/interpret/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/interpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20548 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/interpret/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/interpret/model_interpret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/interpret/shap_dependence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.722374 probatus-2.0.1/probatus/metric_volatility/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/metric_volatility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/metric_volatility/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/metric_volatility/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29943 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/metric_volatility/volatility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.722374 probatus-2.0.1/probatus/missing_values/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/missing_values/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/missing_values/imputation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.722374 probatus-2.0.1/probatus/sample_similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/sample_similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/sample_similarity/resemblance_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.722374 probatus-2.0.1/probatus/stat_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/stat_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/stat_tests/ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16996 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/stat_tests/distribution_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/stat_tests/es.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/stat_tests/ks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/stat_tests/psi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/stat_tests/sw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/stat_tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.722374 probatus-2.0.1/probatus/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/utils/arrayfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/utils/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/utils/missing_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/utils/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/utils/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/utils/shap_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/utils/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.718374 probatus-2.0.1/probatus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-06-19 07:44:05.000000 probatus-2.0.1/probatus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-19 07:44:05.000000 probatus-2.0.1/probatus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 07:44:05.000000 probatus-2.0.1/probatus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-19 07:44:05.000000 probatus-2.0.1/probatus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 07:44:05.000000 probatus-2.0.1/probatus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-19 07:41:11.000000 probatus-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 07:44:05.726374 probatus-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.718374 probatus-2.0.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.722374 probatus-2.0.1/tests/binning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/binning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/binning/test_binning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.726374 probatus-2.0.1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/docs/test_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/docs/test_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.726374 probatus-2.0.1/tests/feature_elimination/
+-rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/feature_elimination/test_feature_elimination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.726374 probatus-2.0.1/tests/interpret/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/interpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34609 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/interpret/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/interpret/test_model_interpret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/interpret/test_shap_dependence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.726374 probatus-2.0.1/tests/metric_volatility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/metric_volatility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/metric_volatility/test_metric_volatility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.726374 probatus-2.0.1/tests/missing_values/
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/missing_values/test_imputation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.726374 probatus-2.0.1/tests/sample_similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/sample_similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/sample_similarity/test_resemblance_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.726374 probatus-2.0.1/tests/stat_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/stat_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/stat_tests/test_distribution_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/stat_tests/test_stat_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/stat_tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.726374 probatus-2.0.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/utils/test_utils_array_funcs.py
```

### Comparing `probatus-2.0.0/LICENCE` & `probatus-2.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/README.md` & `probatus-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/__init__.py` & `probatus-2.0.1/probatus/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/binning/__init__.py` & `probatus-2.0.1/probatus/binning/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/binning/binning.py` & `probatus-2.0.1/probatus/binning/binning.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/feature_elimination/__init__.py` & `probatus-2.0.1/probatus/feature_elimination/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/feature_elimination/feature_elimination.py` & `probatus-2.0.1/probatus/feature_elimination/feature_elimination.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/interpret/__init__.py` & `probatus-2.0.1/probatus/interpret/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/interpret/inspector.py` & `probatus-2.0.1/probatus/interpret/inspector.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/interpret/model_interpret.py` & `probatus-2.0.1/probatus/interpret/model_interpret.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/interpret/shap_dependence.py` & `probatus-2.0.1/probatus/interpret/shap_dependence.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/metric_volatility/__init__.py` & `probatus-2.0.1/probatus/metric_volatility/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/metric_volatility/metric.py` & `probatus-2.0.1/probatus/metric_volatility/metric.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/metric_volatility/utils.py` & `probatus-2.0.1/probatus/metric_volatility/utils.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/metric_volatility/volatility.py` & `probatus-2.0.1/probatus/metric_volatility/volatility.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/missing_values/__init__.py` & `probatus-2.0.1/probatus/missing_values/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/missing_values/imputation.py` & `probatus-2.0.1/probatus/missing_values/imputation.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/sample_similarity/__init__.py` & `probatus-2.0.1/probatus/sample_similarity/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/sample_similarity/resemblance_model.py` & `probatus-2.0.1/probatus/sample_similarity/resemblance_model.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/stat_tests/__init__.py` & `probatus-2.0.1/probatus/stat_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/stat_tests/ad.py` & `probatus-2.0.1/probatus/stat_tests/ad.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/stat_tests/distribution_statistics.py` & `probatus-2.0.1/probatus/stat_tests/distribution_statistics.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/stat_tests/es.py` & `probatus-2.0.1/probatus/stat_tests/es.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/stat_tests/ks.py` & `probatus-2.0.1/probatus/stat_tests/ks.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/stat_tests/psi.py` & `probatus-2.0.1/probatus/stat_tests/psi.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/stat_tests/sw.py` & `probatus-2.0.1/probatus/stat_tests/sw.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/stat_tests/utils.py` & `probatus-2.0.1/probatus/stat_tests/utils.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/utils/__init__.py` & `probatus-2.0.1/probatus/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/utils/_utils.py` & `probatus-2.0.1/probatus/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/utils/arrayfuncs.py` & `probatus-2.0.1/probatus/utils/arrayfuncs.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/utils/exceptions.py` & `probatus-2.0.1/probatus/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/utils/interface.py` & `probatus-2.0.1/probatus/utils/interface.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/utils/missing_helpers.py` & `probatus-2.0.1/probatus/utils/missing_helpers.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/utils/plots.py` & `probatus-2.0.1/probatus/utils/plots.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/utils/scoring.py` & `probatus-2.0.1/probatus/utils/scoring.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/utils/shap_helpers.py` & `probatus-2.0.1/probatus/utils/shap_helpers.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus/utils/warnings.py` & `probatus-2.0.1/probatus/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/probatus.egg-info/SOURCES.txt` & `probatus-2.0.1/probatus.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENCE
 README.md
-setup.py
+pyproject.toml
 probatus/__init__.py
 probatus.egg-info/PKG-INFO
 probatus.egg-info/SOURCES.txt
 probatus.egg-info/dependency_links.txt
-probatus.egg-info/not-zip-safe
 probatus.egg-info/requires.txt
 probatus.egg-info/top_level.txt
 probatus/binning/__init__.py
 probatus/binning/binning.py
 probatus/feature_elimination/__init__.py
 probatus/feature_elimination/feature_elimination.py
 probatus/interpret/__init__.py
@@ -43,20 +42,22 @@
 probatus/utils/shap_helpers.py
 probatus/utils/warnings.py
 tests/binning/__init__.py
 tests/binning/test_binning.py
 tests/docs/__init__.py
 tests/docs/test_docstring.py
 tests/docs/test_notebooks.py
+tests/feature_elimination/test_feature_elimination.py
 tests/interpret/__init__.py
 tests/interpret/test_inspector.py
 tests/interpret/test_model_interpret.py
 tests/interpret/test_shap_dependence.py
 tests/metric_volatility/__init__.py
 tests/metric_volatility/test_metric_volatility.py
+tests/missing_values/test_imputation.py
 tests/sample_similarity/__init__.py
 tests/sample_similarity/test_resemblance_model.py
 tests/stat_tests/__init__.py
 tests/stat_tests/test_distribution_statistics.py
 tests/stat_tests/test_stat_tests.py
 tests/stat_tests/test_utils.py
 tests/utils/__init__.py
```

### Comparing `probatus-2.0.0/probatus.egg-info/requires.txt` & `probatus-2.0.1/probatus.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,53 @@
 scikit-learn>=0.22.2
 pandas>=1.0.0
 matplotlib>=3.1.1
 scipy>=1.4.0
 joblib>=0.13.2
 tqdm>=4.41.0
 shap==0.41.0
+
+[:python_version < "3.11"]
 numpy==1.23.0
 numba>=0.56.4
 
+[:python_version == "3.11"]
+numpy==1.23.2
+numba==0.57.0
+
 [all]
-scikit-learn>=0.22.2
-pandas>=1.0.0
-matplotlib>=3.1.1
-scipy>=1.4.0
-joblib>=0.13.2
-tqdm>=4.41.0
-shap==0.41.0
-numpy==1.23.0
-numba>=0.56.4
 lightgbm>=3.3.0
-catboost>=1.1
 xgboost>=1.5.0
-flake8>=3.8.3
+scipy>=1.4.0
 black>=19.10b0
 pre-commit>=2.5.0
 mypy>=0.770
-flake8-docstrings>=1.4.0
 pytest>=6.0.0
 pytest-cov>=2.10.0
 pyflakes
 seaborn>=0.9.0
+joblib>=0.13.2
 jupyter>=1.0.0
 tabulate>=0.8.7
 nbconvert>=6.0.7
 pre-commit>=2.7.1
 isort>=5.12.0
 codespell>=2.2.4
+ruff>=0.0.272
 mkdocs-material>=6.1.0
 mkdocs-git-revision-date-localized-plugin>=0.7.2
 mkdocs-git-authors-plugin>=0.3.2
 mkdocs-table-reader-plugin>=0.4.1
 mkdocs-enumerate-headings-plugin>=0.4.3
 mkdocs-awesome-pages-plugin>=2.4.0
 mkdocs-minify-plugin>=0.3.0
 mknotebooks>=0.6.2
 mkdocstrings>=0.13.6
 mkdocs-print-site-plugin>=0.8.2
 mkdocs-markdownextradata-plugin>=0.1.9
+mkdocstrings-python>=1.1.2
 
-[extras]
-scikit-learn>=0.22.2
-pandas>=1.0.0
-matplotlib>=3.1.1
-scipy>=1.4.0
-joblib>=0.13.2
-tqdm>=4.41.0
-shap==0.41.0
-numpy==1.23.0
-numba>=0.56.4
-lightgbm>=3.3.0
+[all:python_version != "3.8"]
 catboost>=1.1
-xgboost>=1.5.0
+
+[all:python_version == "3.8"]
+catboost<1.2
```

### Comparing `probatus-2.0.0/tests/binning/test_binning.py` & `probatus-2.0.1/tests/binning/test_binning.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/tests/docs/test_docstring.py` & `probatus-2.0.1/tests/docs/test_docstring.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/tests/docs/test_notebooks.py` & `probatus-2.0.1/tests/docs/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/tests/interpret/test_inspector.py` & `probatus-2.0.1/tests/interpret/test_inspector.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/tests/interpret/test_model_interpret.py` & `probatus-2.0.1/tests/interpret/test_model_interpret.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/tests/interpret/test_shap_dependence.py` & `probatus-2.0.1/tests/interpret/test_shap_dependence.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/tests/metric_volatility/test_metric_volatility.py` & `probatus-2.0.1/tests/metric_volatility/test_metric_volatility.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/tests/sample_similarity/test_resemblance_model.py` & `probatus-2.0.1/tests/sample_similarity/test_resemblance_model.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/tests/stat_tests/test_distribution_statistics.py` & `probatus-2.0.1/tests/stat_tests/test_distribution_statistics.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/tests/stat_tests/test_stat_tests.py` & `probatus-2.0.1/tests/stat_tests/test_stat_tests.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/tests/stat_tests/test_utils.py` & `probatus-2.0.1/tests/stat_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.0/tests/utils/test_utils_array_funcs.py` & `probatus-2.0.1/tests/utils/test_utils_array_funcs.py`

 * *Files identical despite different names*

