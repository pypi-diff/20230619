# Comparing `tmp/skorecard-1.6.6.tar.gz` & `tmp/skorecard-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skorecard-1.6.6.tar", last modified: Fri Jun 16 15:57:15 2023, max compression
+gzip compressed data, was "skorecard-1.6.7.tar", last modified: Mon Jun 19 07:44:08 2023, max compression
```

## Comparing `skorecard-1.6.6.tar` & `skorecard-1.6.7.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.828713 skorecard-1.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-16 15:53:32.000000 skorecard-1.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-16 15:53:32.000000 skorecard-1.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-16 15:57:15.828713 skorecard-1.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-16 15:53:32.000000 skorecard-1.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-16 15:53:32.000000 skorecard-1.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 15:57:15.828713 skorecard-1.6.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.820713 skorecard-1.6.6/skorecard/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.820713 skorecard-1.6.6/skorecard/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/apps/app_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    16357 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/apps/app_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/apps/app_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.820713 skorecard-1.6.6/skorecard/apps/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   181482 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/apps/assets/united-bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/bucket_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.820713 skorecard-1.6.6/skorecard/bucketers/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/bucketers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/bucketers/base_bucketer.py
--rw-r--r--   0 runner    (1001) docker     (123)    55337 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/bucketers/bucketers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.820713 skorecard-1.6.6/skorecard/data/
--rw-r--r--   0 runner    (1001) docker     (123)    31668 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/data/UCI_Credit_Card.zip
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/features_bucket_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.820713 skorecard-1.6.6/skorecard/linear_model/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/linear_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/linear_model/linear_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.820713 skorecard-1.6.6/skorecard/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.820713 skorecard-1.6.6/skorecard/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18468 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/pipeline/bucketing_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    16658 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/pipeline/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.824713 skorecard-1.6.6/skorecard/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/preprocessing/_WoEEncoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/preprocessing/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.824713 skorecard-1.6.6/skorecard/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/reporting/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/reporting/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.824713 skorecard-1.6.6/skorecard/rescale/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/rescale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/rescale/rescale.py
--rw-r--r--   0 runner    (1001) docker     (123)    15835 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/skorecard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.824713 skorecard-1.6.6/skorecard/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/utils/arrayfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-16 15:53:32.000000 skorecard-1.6.6/skorecard/utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.820713 skorecard-1.6.6/skorecard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-16 15:57:15.000000 skorecard-1.6.6/skorecard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-16 15:57:15.000000 skorecard-1.6.6/skorecard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:57:15.000000 skorecard-1.6.6/skorecard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-16 15:57:15.000000 skorecard-1.6.6/skorecard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-16 15:57:15.000000 skorecard-1.6.6/skorecard.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:15.828713 skorecard-1.6.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_Skorecard_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucket_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucket_table_woe_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucketer_AsIsCategoricalBucketer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucketer_AsIsNumericalBucketer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucketer_DecisionTreeBucketer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucketer_OptimalBucketer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucketer_OrdinalCategoricalBucketer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucketer_UserInputBucketer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucketer_WoEBucketer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucketers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14751 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_bucketing_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_column_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_linear_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_manual_bucketer_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_rescale.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_sklearn_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_specials_bucketers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_suppressor_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_usage_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-16 15:53:32.000000 skorecard-1.6.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.873167 skorecard-1.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-19 07:39:06.000000 skorecard-1.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-19 07:39:06.000000 skorecard-1.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-19 07:44:08.873167 skorecard-1.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-19 07:39:06.000000 skorecard-1.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-19 07:39:06.000000 skorecard-1.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 07:44:08.873167 skorecard-1.6.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.853166 skorecard-1.6.7/skorecard/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.857166 skorecard-1.6.7/skorecard/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/apps/app_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16449 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/apps/app_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/apps/app_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.857166 skorecard-1.6.7/skorecard/apps/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   181482 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/apps/assets/united-bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/bucket_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.861166 skorecard-1.6.7/skorecard/bucketers/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/bucketers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/bucketers/base_bucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55337 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/bucketers/bucketers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.861166 skorecard-1.6.7/skorecard/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    31668 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/data/UCI_Credit_Card.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/features_bucket_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.861166 skorecard-1.6.7/skorecard/linear_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/linear_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/linear_model/linear_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.861166 skorecard-1.6.7/skorecard/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.865167 skorecard-1.6.7/skorecard/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18468 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/pipeline/bucketing_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16658 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/pipeline/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.865167 skorecard-1.6.7/skorecard/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/preprocessing/_WoEEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/preprocessing/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.865167 skorecard-1.6.7/skorecard/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/reporting/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/reporting/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.865167 skorecard-1.6.7/skorecard/rescale/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/rescale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/rescale/rescale.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15835 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/skorecard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.865167 skorecard-1.6.7/skorecard/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/utils/arrayfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.857166 skorecard-1.6.7/skorecard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-19 07:44:08.000000 skorecard-1.6.7/skorecard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-19 07:44:08.000000 skorecard-1.6.7/skorecard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 07:44:08.000000 skorecard-1.6.7/skorecard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-19 07:44:08.000000 skorecard-1.6.7/skorecard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-19 07:44:08.000000 skorecard-1.6.7/skorecard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.873167 skorecard-1.6.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_Skorecard_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucket_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucket_table_woe_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucketer_AsIsCategoricalBucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucketer_AsIsNumericalBucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucketer_DecisionTreeBucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucketer_OptimalBucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucketer_OrdinalCategoricalBucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucketer_UserInputBucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucketer_WoEBucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucketers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14751 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucketing_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_column_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_linear_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_manual_bucketer_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_rescale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_sklearn_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_specials_bucketers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_suppressor_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_usage_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_utils.py
```

### Comparing `skorecard-1.6.6/LICENSE` & `skorecard-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/PKG-INFO` & `skorecard-1.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skorecard
-Version: 1.6.6
+Version: 1.6.7
 Summary: Tools for building scorecard models in python, with a sklearn-compatible API
 Author-email: "ING Bank N.V." <anilkumar.panda@ing.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 ING Bank NV
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `skorecard-1.6.6/README.md` & `skorecard-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/pyproject.toml` & `skorecard-1.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "skorecard"
-version = "1.6.6"
+version = "1.6.7"
 requires-python= ">=3.8"
 description = "Tools for building scorecard models in python, with a sklearn-compatible API"
 readme = { file = "README.md", content-type = "text/markdown" }
 authors = [
     { name = "ING Bank N.V.", email = "anilkumar.panda@ing.com" }
 ]
 license = { file = "LICENSE" }
@@ -22,15 +22,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
     "scipy>=1.5.2",
     "numpy>=1.19.5",
-    "pandas==1.5.3",
+    "pandas>=1.5.3",
     "scikit-learn>=0.23.2",
     "pyyaml",
     "category_encoders>=2.2.2",
     "optbinning>=0.8.0",
 ]
 
 [project.urls]
@@ -112,8 +112,8 @@
 filter_files = true
 extend_skip = ["__init__.py", "docs"]
 
 [tool.codespell]
 skip = "**.egg-info*"
 
 [tool.black]
-line-length = 120
+line-length = 120
```

### Comparing `skorecard-1.6.6/skorecard/apps/app_callbacks.py` & `skorecard-1.6.7/skorecard/apps/app_callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from skorecard.apps.app_utils import determine_boundaries, is_increasing, is_sequential
 from skorecard.reporting import build_bucket_table
 from skorecard.utils.exceptions import NotInstalledError
 
 # Dash + dependencies
 try:
-    import dash_table
     from dash import no_update
     from dash.dependencies import Input, Output, State
 except ModuleNotFoundError:
     Input = NotInstalledError("dash", "dashboard")
     Output = NotInstalledError("dash", "dashboard")
     State = NotInstalledError("dash", "dashboard")
     dash_table = NotInstalledError("dash_table", "dashboard")
```

### Comparing `skorecard-1.6.6/skorecard/apps/app_layout.py` & `skorecard-1.6.7/skorecard/apps/app_layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from skorecard.apps.app_utils import colorize_cell, perc_data_bars
 from skorecard.utils.exceptions import NotInstalledError
 
 # Dash + dependencies
 try:
-    import dash_core_components as dcc
-    import dash_html_components as html
-    import dash_table
+    try:
+        from dash import dash_table, dcc, html
+    except ImportError:
+        import dash_core_components as dcc
+        import dash_html_components as html
+        import dash_table
 except ModuleNotFoundError:
     dcc = NotInstalledError("dash_core_components", "dashboard")
     html = NotInstalledError("dash_html_components", "dashboard")
     Input = NotInstalledError("dash", "dashboard")
     Output = NotInstalledError("dash", "dashboard")
     State = NotInstalledError("dash", "dashboard")
     dash_table = NotInstalledError("dash_table", "dashboard")
```

### Comparing `skorecard-1.6.6/skorecard/apps/app_utils.py` & `skorecard-1.6.7/skorecard/apps/app_utils.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard/apps/assets/united-bootstrap.min.css` & `skorecard-1.6.7/skorecard/apps/assets/united-bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard/bucket_mapping.py` & `skorecard-1.6.7/skorecard/bucket_mapping.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard/bucketers/__init__.py` & `skorecard-1.6.7/skorecard/bucketers/__init__.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard/bucketers/base_bucketer.py` & `skorecard-1.6.7/skorecard/bucketers/base_bucketer.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard/bucketers/bucketers.py` & `skorecard-1.6.7/skorecard/bucketers/bucketers.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard/data/UCI_Credit_Card.zip` & `skorecard-1.6.7/skorecard/data/UCI_Credit_Card.zip`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard/datasets.py` & `skorecard-1.6.7/skorecard/datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,18 +57,20 @@
         - is both are false (default setting): returns a dictionary where the key `data` contains the features,
         and the key `target` is the target
 
     """
     try:
         data = fetch_openml(
             name="default-of-credit-card-clients",
+            version=1,
             data_home=None,
             cache=True,
             as_frame=as_frame,
             return_X_y=return_X_y,
+            parser="liac-arff",
         )
     except Exception as e:
         # update the error message with a more helpful message.
         error_msg = (
             "Cannot retrieve the dataset from repository. Make sure there is no firewall blocking "
             "the connection.\nAlternatively, download it manually from https://www.openml.org/d/42477"
         )
```

### Comparing `skorecard-1.6.6/skorecard/features_bucket_mapping.py` & `skorecard-1.6.7/skorecard/features_bucket_mapping.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard/linear_model/linear_model.py` & `skorecard-1.6.7/skorecard/linear_model/linear_model.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard/metrics/metrics.py` & `skorecard-1.6.7/skorecard/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard/pipeline/bucketing_process.py` & `skorecard-1.6.7/skorecard/pipeline/bucketing_process.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard/pipeline/pipeline.py` & `skorecard-1.6.7/skorecard/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard/preprocessing/_WoEEncoder.py` & `skorecard-1.6.7/skorecard/preprocessing/_WoEEncoder.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard/preprocessing/preprocessing.py` & `skorecard-1.6.7/skorecard/preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard/reporting/plotting.py` & `skorecard-1.6.7/skorecard/reporting/plotting.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import pandas as pd
 from sklearn.pipeline import Pipeline
 from sklearn.utils.validation import check_is_fitted
 
 from skorecard.utils.exceptions import NotInstalledError
 
 try:
-    import plotly.express as px
     import plotly.graph_objects as go
     from plotly.subplots import make_subplots
 except ModuleNotFoundError:
-    px = NotInstalledError("plotly", "reporting")
+    NotInstalledError("plotly", "reporting")
 
 try:
-    from IPython.display import Image
+    from IPython.core.display import Image
 except ModuleNotFoundError:
-    Image = NotInstalledError("psutil")  # type: ignore
+    NotInstalledError("psutil")
 
 
 def make_plot_figure(bucket_table: pd.DataFrame, line="event_rate"):
     """
     Make a plotly object out of a table. The line defines what is plotted on the y-axis.
     """
     # To support both pre-buckets and buckets
@@ -48,15 +47,20 @@
     # and thus we need to output a simpler plot
     if column_to_plot in bucket_table.columns:
         plotdf[column_to_plot] = [event for event in bucket_table[column_to_plot].values]
         fig = make_subplots(specs=[[{"secondary_y": True}]])
 
         # Add trace with event rate
         fig.add_trace(
-            go.Scatter(x=plotdf["label"], y=plotdf[column_to_plot], name=column_to_plot, line=dict(color="#454c57")),
+            go.Scatter(
+                x=plotdf["label"],
+                y=plotdf[column_to_plot],
+                name=column_to_plot,
+                line=dict(color="#454c57"),
+            ),
             secondary_y=True,
         )
         fig.update_yaxes(title_text=f"Bucket {column_to_plot}", secondary_y=True, tickformat=",.0%")
 
     else:
         fig = make_subplots(specs=[[{"secondary_y": False}]])
 
@@ -81,15 +85,23 @@
     fig.update_layout(
         margin=dict(l=20, r=20, t=40, b=20),
         height=350,
     )
     return fig
 
 
-def plot_prebucket_table(prebucket_table, column="", line="", format=None, scale=None, width=None, height=None):
+def plot_prebucket_table(
+    prebucket_table,
+    column="",
+    line="",
+    format=None,
+    scale=None,
+    width=None,
+    height=None,
+):
     """
     Given the prebucketed data, plot the pre-buckets.
 
     Args:
         prebucket_table (pd.DataFrame): the table of the prebucketed data
         column (str): The column to plot
         line (str): The line to plot on the secondary axis
@@ -182,15 +194,23 @@
 class PlotPreBucketMethod:
     """
     Add methods for plotting bucketing tables to another class.
 
     To be used with skorecard.pipeline.BucketingProcess and skorecard.bucketers.BaseBucketer
     """
 
-    def plot_prebucket(self, column, line="event_rate", format=None, scale=None, width=None, height=None):
+    def plot_prebucket(
+        self,
+        column,
+        line="event_rate",
+        format=None,
+        scale=None,
+        width=None,
+        height=None,
+    ):
         """
         Generates the prebucket table and produces a corresponding plotly plot.
 
         Args:
             column: The column we want to visualise
             line: The line to plot on the secondary axis. Default is Event Rate.
             format: The format of the image, such as 'png'. The default None returns a plotly image.
@@ -220,15 +240,23 @@
 class PlotBucketMethod:
     """
     Add methods for plotting bucketing tables to another class.
 
     To be used with skorecard.pipeline.BucketingProcess and skorecard.bucketers.BaseBucketer
     """
 
-    def plot_bucket(self, column, line="event_rate", format=None, scale=None, width=None, height=None):
+    def plot_bucket(
+        self,
+        column,
+        line="event_rate",
+        format=None,
+        scale=None,
+        width=None,
+        height=None,
+    ):
         """
         Plot the buckets.
 
         Args:
             column: The column we want to visualise
             line: The line to plot on the secondary axis. Default is Event Rate.
             format: The format of the image, such as 'png'. The default None returns a plotly image.
```

### Comparing `skorecard-1.6.6/skorecard/reporting/report.py` & `skorecard-1.6.7/skorecard/reporting/report.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard/rescale/rescale.py` & `skorecard-1.6.7/skorecard/rescale/rescale.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,16 @@
     scp = ScoreCardPoints(model)
     scp.transform(X)
     ```
 
     """
 
     def __init__(self, skorecard_model, *, pdo=20, ref_score=100, ref_odds=1):
-        """
+        """Initialize the transformer.
+
         Args:
             skorecard_model: the fitted Skorecard class
             pdo: number of points necessary to double the odds
             ref_score: reference score set for the reference odds
             ref_odds: odds that correspond to the ref_score
         """
         assert isinstance(skorecard_model, Skorecard), (
@@ -120,15 +121,15 @@
             self.features = fbm.columns
         woe_dict = woe_enc.mapping
 
         self.buckets = {k: fbm.get(k) for k in fbm.columns if k in self.features}
         self.woes = {k: woe_dict[k] for k in woe_dict.keys() if k in self.features}
 
     def _calculate_scorecard_points(self):
-        # Put together the features in a list of table, containing all the buckets.
+        # Put together the features in a list of tables, containing all the buckets.
         list_dfs = list()
         for ix, col in enumerate(self.features):
             df_ = (
                 pd.concat([pd.Series(self.buckets[col].labels), pd.Series(self.woes[col])], axis=1)
                 .reset_index()
                 .rename(columns={"index": "bin_index", 0: "map", 1: "woe"})
             )
@@ -136,16 +137,21 @@
 
             df_.loc[:, "coef"] = self.model.coef_[0][ix]
             #
             list_dfs.append(df_)
 
         # Reduce the list of tables, to build the final scorecard feature points
         scorecard = reduce(lambda x, y: pd.concat([x, y]), list_dfs)
-        scorecard = scorecard.append(
-            {"feature": "Intercept", "coef": self.model.intercept_[0], "bin_index": 0, "map": 0, "woe": 0},
+        scorecard = pd.concat(
+            [
+                scorecard,
+                pd.DataFrame(
+                    [{"feature": "Intercept", "coef": self.model.intercept_[0], "bin_index": 0, "map": 0, "woe": 0}]
+                ),
+            ],
             ignore_index=True,
         )
         #     return buckets, woes
         scorecard["contribution"] = scorecard["woe"] * scorecard["coef"]
 
         self.scorecard = _scale_scorecard(
             scorecard, pdo=self.pdo, ref_score=self.ref_score, ref_odds=self.ref_odds, features=self.features
@@ -177,14 +183,15 @@
         bin_points.index = X.index
 
         return bin_points
 
 
 def _scale_scorecard(df, *, pdo, ref_score, ref_odds, features):
     """Equations to scale the feature scorecards.
+
     Args:
         df: Pandas DataFrame
         pdo: number of points necessary to double the odds
         ref_score: reference score set for the reference odds
         ref_odds: odds that correspond to the ref_score
         features (list): The list of features
```

### Comparing `skorecard-1.6.6/skorecard/skorecard.py` & `skorecard-1.6.7/skorecard/skorecard.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard/utils/__init__.py` & `skorecard-1.6.7/skorecard/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard/utils/arrayfuncs.py` & `skorecard-1.6.7/skorecard/utils/arrayfuncs.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard/utils/dataframe.py` & `skorecard-1.6.7/skorecard/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard/utils/exceptions.py` & `skorecard-1.6.7/skorecard/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard/utils/validation.py` & `skorecard-1.6.7/skorecard/utils/validation.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard.egg-info/PKG-INFO` & `skorecard-1.6.7/skorecard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skorecard
-Version: 1.6.6
+Version: 1.6.7
 Summary: Tools for building scorecard models in python, with a sklearn-compatible API
 Author-email: "ING Bank N.V." <anilkumar.panda@ing.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 ING Bank NV
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `skorecard-1.6.6/skorecard.egg-info/SOURCES.txt` & `skorecard-1.6.7/skorecard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/skorecard.egg-info/requires.txt` & `skorecard-1.6.7/skorecard.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 scipy>=1.5.2
 numpy>=1.19.5
-pandas==1.5.3
+pandas>=1.5.3
 scikit-learn>=0.23.2
 pyyaml
 category_encoders>=2.2.2
 optbinning>=0.8.0
 
 [all]
 dash>=1.21.0
```

### Comparing `skorecard-1.6.6/tests/test_Skorecard_class.py` & `skorecard-1.6.7/tests/test_Skorecard_class.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_bucket_mapping.py` & `skorecard-1.6.7/tests/test_bucket_mapping.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_bucket_table_woe_values.py` & `skorecard-1.6.7/tests/test_bucket_table_woe_values.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_bucketer_AsIsCategoricalBucketer.py` & `skorecard-1.6.7/tests/test_bucketer_AsIsCategoricalBucketer.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_bucketer_AsIsNumericalBucketer.py` & `skorecard-1.6.7/tests/test_bucketer_AsIsNumericalBucketer.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_bucketer_DecisionTreeBucketer.py` & `skorecard-1.6.7/tests/test_bucketer_DecisionTreeBucketer.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_bucketer_OptimalBucketer.py` & `skorecard-1.6.7/tests/test_bucketer_OptimalBucketer.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_bucketer_OrdinalCategoricalBucketer.py` & `skorecard-1.6.7/tests/test_bucketer_OrdinalCategoricalBucketer.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_bucketer_UserInputBucketer.py` & `skorecard-1.6.7/tests/test_bucketer_UserInputBucketer.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_bucketer_WoEBucketer.py` & `skorecard-1.6.7/tests/test_bucketer_WoEBucketer.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_bucketers.py` & `skorecard-1.6.7/tests/test_bucketers.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_bucketing_process.py` & `skorecard-1.6.7/tests/test_bucketing_process.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_column_selector.py` & `skorecard-1.6.7/tests/test_column_selector.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_datasets.py` & `skorecard-1.6.7/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_docstring.py` & `skorecard-1.6.7/tests/test_docstring.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_io.py` & `skorecard-1.6.7/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_linear_model.py` & `skorecard-1.6.7/tests/test_linear_model.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_manual_bucketer_app.py` & `skorecard-1.6.7/tests/test_manual_bucketer_app.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_metrics.py` & `skorecard-1.6.7/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_pipelines.py` & `skorecard-1.6.7/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_reports.py` & `skorecard-1.6.7/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_rescale.py` & `skorecard-1.6.7/tests/test_rescale.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_sklearn_compat.py` & `skorecard-1.6.7/tests/test_sklearn_compat.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_specials_bucketers.py` & `skorecard-1.6.7/tests/test_specials_bucketers.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_suppressor_warning.py` & `skorecard-1.6.7/tests/test_suppressor_warning.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.6/tests/test_usage_flows.py` & `skorecard-1.6.7/tests/test_usage_flows.py`

 * *Files identical despite different names*

