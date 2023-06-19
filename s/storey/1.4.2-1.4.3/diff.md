# Comparing `tmp/storey-1.4.2.tar.gz` & `tmp/storey-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/storey/storey/dist/.tmp-qtid9xr6/storey-1.4.2.tar", last modified: Wed Jun 14 08:27:44 2023, max compression
+gzip compressed data, was "/home/runner/work/storey/storey/dist/.tmp-o0b9u66t/storey-1.4.3.tar", last modified: Mon Jun 19 05:31:15 2023, max compression
```

## Comparing `storey-1.4.2.tar` & `storey-1.4.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:27:44.000000 storey-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-14 08:24:33.000000 storey-1.4.2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 08:24:33.000000 storey-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-14 08:24:33.000000 storey-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-06-14 08:27:44.000000 storey-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-14 08:24:33.000000 storey-1.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-14 08:24:33.000000 storey-1.4.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:27:44.000000 storey-1.4.2/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-14 08:24:33.000000 storey-1.4.2/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-14 08:24:33.000000 storey-1.4.2/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-06-14 08:24:33.000000 storey-1.4.2/integration/integration_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   170272 2023-06-14 08:24:33.000000 storey-1.4.2/integration/test_aggregation_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-06-14 08:24:33.000000 storey-1.4.2/integration/test_azure_filesystem_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21737 2023-06-14 08:24:33.000000 storey-1.4.2/integration/test_filesystems_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    42755 2023-06-14 08:24:33.000000 storey-1.4.2/integration/test_flow_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-06-14 08:24:33.000000 storey-1.4.2/integration/test_kafka_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-14 08:24:33.000000 storey-1.4.2/integration/test_redis_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-06-14 08:24:33.000000 storey-1.4.2/integration/test_s3_filesystem_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-14 08:24:33.000000 storey-1.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-14 08:27:44.000000 storey-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-14 08:24:33.000000 storey-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:27:44.000000 storey-1.4.2/storey/
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-14 08:27:39.000000 storey-1.4.2/storey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-14 08:24:33.000000 storey-1.4.2/storey/aggregation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17699 2023-06-14 08:24:33.000000 storey-1.4.2/storey/aggregations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-06-14 08:24:33.000000 storey-1.4.2/storey/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    28065 2023-06-14 08:24:33.000000 storey-1.4.2/storey/drivers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15755 2023-06-14 08:24:33.000000 storey-1.4.2/storey/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    50623 2023-06-14 08:24:33.000000 storey-1.4.2/storey/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-14 08:24:33.000000 storey-1.4.2/storey/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    27610 2023-06-14 08:24:33.000000 storey-1.4.2/storey/redis_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    37793 2023-06-14 08:24:33.000000 storey-1.4.2/storey/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-14 08:24:33.000000 storey-1.4.2/storey/sql_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:27:44.000000 storey-1.4.2/storey/steps/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-14 08:24:33.000000 storey-1.4.2/storey/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-14 08:24:33.000000 storey-1.4.2/storey/steps/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-14 08:24:33.000000 storey-1.4.2/storey/steps/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-14 08:24:33.000000 storey-1.4.2/storey/steps/foreach.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-14 08:24:33.000000 storey-1.4.2/storey/steps/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-14 08:24:33.000000 storey-1.4.2/storey/steps/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    79910 2023-06-14 08:24:33.000000 storey-1.4.2/storey/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    50747 2023-06-14 08:24:33.000000 storey-1.4.2/storey/targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:27:44.000000 storey-1.4.2/storey/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-14 08:24:33.000000 storey-1.4.2/storey/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-06-14 08:24:33.000000 storey-1.4.2/storey/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-06-14 08:24:33.000000 storey-1.4.2/storey/windowed_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:27:44.000000 storey-1.4.2/storey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-06-14 08:27:44.000000 storey-1.4.2/storey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-14 08:27:44.000000 storey-1.4.2/storey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:27:44.000000 storey-1.4.2/storey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-14 08:27:44.000000 storey-1.4.2/storey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-14 08:27:44.000000 storey-1.4.2/storey.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:27:44.000000 storey-1.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-14 08:24:33.000000 storey-1.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144374 2023-06-14 08:24:33.000000 storey-1.4.2/tests/test_aggregate_by_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-14 08:24:33.000000 storey-1.4.2/tests/test_aggregate_store.py
--rw-r--r--   0 runner    (1001) docker     (123)   124403 2023-06-14 08:24:33.000000 storey-1.4.2/tests/test_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-06-14 08:24:33.000000 storey-1.4.2/tests/test_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-14 08:24:33.000000 storey-1.4.2/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-14 08:24:33.000000 storey-1.4.2/tests/test_v3io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-14 08:24:33.000000 storey-1.4.2/tests/test_windowed_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:31:15.000000 storey-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-19 05:26:44.000000 storey-1.4.3/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 05:26:44.000000 storey-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-19 05:26:44.000000 storey-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-06-19 05:31:15.000000 storey-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-19 05:26:44.000000 storey-1.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-19 05:26:44.000000 storey-1.4.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:31:15.000000 storey-1.4.3/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-19 05:26:44.000000 storey-1.4.3/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-19 05:26:44.000000 storey-1.4.3/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-06-19 05:26:44.000000 storey-1.4.3/integration/integration_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   170272 2023-06-19 05:26:44.000000 storey-1.4.3/integration/test_aggregation_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-06-19 05:26:44.000000 storey-1.4.3/integration/test_azure_filesystem_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21737 2023-06-19 05:26:44.000000 storey-1.4.3/integration/test_filesystems_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42755 2023-06-19 05:26:44.000000 storey-1.4.3/integration/test_flow_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-06-19 05:26:44.000000 storey-1.4.3/integration/test_kafka_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-19 05:26:44.000000 storey-1.4.3/integration/test_redis_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-06-19 05:26:44.000000 storey-1.4.3/integration/test_s3_filesystem_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-19 05:26:44.000000 storey-1.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-19 05:31:15.000000 storey-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-19 05:26:44.000000 storey-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:31:15.000000 storey-1.4.3/storey/
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-19 05:31:10.000000 storey-1.4.3/storey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-19 05:26:44.000000 storey-1.4.3/storey/aggregation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17699 2023-06-19 05:26:44.000000 storey-1.4.3/storey/aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-06-19 05:26:44.000000 storey-1.4.3/storey/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28065 2023-06-19 05:26:44.000000 storey-1.4.3/storey/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15755 2023-06-19 05:26:44.000000 storey-1.4.3/storey/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50622 2023-06-19 05:26:44.000000 storey-1.4.3/storey/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-19 05:26:44.000000 storey-1.4.3/storey/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27610 2023-06-19 05:26:44.000000 storey-1.4.3/storey/redis_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37793 2023-06-19 05:26:44.000000 storey-1.4.3/storey/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-19 05:26:44.000000 storey-1.4.3/storey/sql_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:31:15.000000 storey-1.4.3/storey/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-19 05:26:44.000000 storey-1.4.3/storey/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-19 05:26:44.000000 storey-1.4.3/storey/steps/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-19 05:26:44.000000 storey-1.4.3/storey/steps/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-19 05:26:44.000000 storey-1.4.3/storey/steps/foreach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-19 05:26:44.000000 storey-1.4.3/storey/steps/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-19 05:26:44.000000 storey-1.4.3/storey/steps/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79910 2023-06-19 05:26:44.000000 storey-1.4.3/storey/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50757 2023-06-19 05:26:44.000000 storey-1.4.3/storey/targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:31:15.000000 storey-1.4.3/storey/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-19 05:26:44.000000 storey-1.4.3/storey/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-06-19 05:26:44.000000 storey-1.4.3/storey/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-06-19 05:26:44.000000 storey-1.4.3/storey/windowed_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:31:15.000000 storey-1.4.3/storey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-06-19 05:31:15.000000 storey-1.4.3/storey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-19 05:31:15.000000 storey-1.4.3/storey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 05:31:15.000000 storey-1.4.3/storey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-19 05:31:15.000000 storey-1.4.3/storey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-19 05:31:15.000000 storey-1.4.3/storey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:31:15.000000 storey-1.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-19 05:26:44.000000 storey-1.4.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144374 2023-06-19 05:26:44.000000 storey-1.4.3/tests/test_aggregate_by_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-19 05:26:44.000000 storey-1.4.3/tests/test_aggregate_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125163 2023-06-19 05:26:44.000000 storey-1.4.3/tests/test_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-06-19 05:26:44.000000 storey-1.4.3/tests/test_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-19 05:26:44.000000 storey-1.4.3/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-19 05:26:44.000000 storey-1.4.3/tests/test_v3io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-19 05:26:44.000000 storey-1.4.3/tests/test_windowed_store.py
```

### Comparing `storey-1.4.2/LICENSE` & `storey-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/PKG-INFO` & `storey-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storey
-Version: 1.4.2
+Version: 1.4.3
 Summary: Async flows
 Home-page: https://github.com/mlrun/storey
 Author: Iguazio
 Author-email: yaronh@iguazio.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `storey-1.4.2/README.md` & `storey-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/integration/__init__.py` & `storey-1.4.3/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/integration/conftest.py` & `storey-1.4.3/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/integration/integration_test_utils.py` & `storey-1.4.3/integration/integration_test_utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/integration/test_aggregation_integration.py` & `storey-1.4.3/integration/test_aggregation_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/integration/test_azure_filesystem_integration.py` & `storey-1.4.3/integration/test_azure_filesystem_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/integration/test_filesystems_integration.py` & `storey-1.4.3/integration/test_filesystems_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/integration/test_flow_integration.py` & `storey-1.4.3/integration/test_flow_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/integration/test_kafka_integration.py` & `storey-1.4.3/integration/test_kafka_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/integration/test_redis_specific.py` & `storey-1.4.3/integration/test_redis_specific.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/integration/test_s3_filesystem_integration.py` & `storey-1.4.3/integration/test_s3_filesystem_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/setup.py` & `storey-1.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/storey/__init__.py` & `storey-1.4.3/storey/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.4.2"
+__version__ = "1.4.3"
 
 # Importing supported filesystems explicitly so that they will get registered as an fsspec filesystem
 import v3iofs  # noqa: F401
 
 from .aggregations import AggregateByKey, QueryByKey  # noqa: F401
 from .dataframe import ReduceToDataFrame, ToDataFrame  # noqa: F401
 from .drivers import Driver, NoopDriver, V3ioDriver  # noqa: F401
```

### Comparing `storey-1.4.2/storey/aggregation_utils.py` & `storey-1.4.3/storey/aggregation_utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/storey/aggregations.py` & `storey-1.4.3/storey/aggregations.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/storey/dataframe.py` & `storey-1.4.3/storey/dataframe.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/storey/drivers.py` & `storey-1.4.3/storey/drivers.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/storey/dtypes.py` & `storey-1.4.3/storey/dtypes.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/storey/flow.py` & `storey-1.4.3/storey/flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -949,15 +949,15 @@
 
 class _Batching(Flow):
     _do_downstream_per_event = True
 
     def __init__(
         self,
         max_events: Optional[int] = None,
-        flush_after_seconds: Optional[int] = None,
+        flush_after_seconds: Union[int, float, None] = None,
         key_field: Optional[Union[str, Callable[[Event], str]]] = None,
         **kwargs,
     ):
         if max_events:
             kwargs["max_events"] = max_events
         if flush_after_seconds is not None:
             kwargs["flush_after_seconds"] = flush_after_seconds
@@ -976,15 +976,14 @@
     def _init(self):
         super()._init()
         self._batch: Dict[Optional[str], List[Any]] = defaultdict(list)
         self._batch_first_event_time: Dict[Optional[str], datetime.datetime] = {}
         self._batch_last_event_time: Dict[Optional[str], datetime.datetime] = {}
         self._batch_start_time: Dict[Optional[str], float] = {}
         self._timeout_task: Optional[Task] = None
-        self._timeout_task_ex: Optional[Exception] = None
 
     @staticmethod
     def _create_key_extractor(key_field) -> Callable:
         if key_field is None:
             return lambda event: None
         elif callable(key_field):
             return key_field
@@ -1018,17 +1017,14 @@
         if len(self._batch[key]) == 0:
             self._batch_first_event_time[key] = event_time
             self._batch_start_time[key] = time.monotonic()
             self._batch_last_event_time[key] = event_time
         elif self._batch_last_event_time[key] < event_time:
             self._batch_last_event_time[key] = event_time
 
-        if self._timeout_task_ex:
-            raise self._timeout_task_ex
-
         if self._flush_after_seconds is not None and self._timeout_task is None:
             self._timeout_task = asyncio.get_running_loop().create_task(self._sleep_and_emit())
 
         self._batch[key].append(self._event_to_batch_entry(event))
 
         if len(self._batch[key]) == self._max_events:
             await self._emit_batch(key)
@@ -1040,16 +1036,18 @@
         try:
             while self._batch:
                 key = next(iter(self._batch.keys()))
                 delta_seconds = time.monotonic() - self._batch_start_time[key]
                 if delta_seconds < self._flush_after_seconds:
                     await asyncio.sleep(self._flush_after_seconds - delta_seconds)
                 await self._emit_batch(key)
-        except Exception as ex:
-            self._timeout_task_ex = ex
+        except Exception:
+            message = traceback.format_exc()
+            if self.logger:
+                self.logger.error(f"Failed to flush batch in step '{self.name}':\n{message}")
 
         self._timeout_task = None
 
     def _event_to_batch_entry(self, event):
         return self._get_event_or_body(event)
 
     async def _emit_batch(self, batch_key: Optional[str] = None):
```

### Comparing `storey-1.4.2/storey/queue.py` & `storey-1.4.3/storey/queue.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/storey/redis_driver.py` & `storey-1.4.3/storey/redis_driver.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/storey/sources.py` & `storey-1.4.3/storey/sources.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/storey/sql_driver.py` & `storey-1.4.3/storey/sql_driver.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/storey/steps/__init__.py` & `storey-1.4.3/storey/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/storey/steps/assertion.py` & `storey-1.4.3/storey/steps/assertion.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/storey/steps/flatten.py` & `storey-1.4.3/storey/steps/flatten.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/storey/steps/foreach.py` & `storey-1.4.3/storey/steps/foreach.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/storey/steps/partition.py` & `storey-1.4.3/storey/steps/partition.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/storey/steps/sample.py` & `storey-1.4.3/storey/steps/sample.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/storey/table.py` & `storey-1.4.3/storey/table.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/storey/targets.py` & `storey-1.4.3/storey/targets.py`

 * *Files 0% similar despite different names*

```diff
@@ -520,15 +520,15 @@
         index_cols: Union[str, Union[List[str], List[Tuple[str, str]]], None] = None,
         columns: Union[str, Union[List[str], List[Tuple[str, str]]], None] = None,
         partition_cols: Union[str, Union[List[str], List[Tuple[str, int]]], None] = None,
         time_field: Union[None, str, int] = None,
         time_format: Optional[str] = None,
         infer_columns_from_data: Optional[bool] = None,
         max_events: Optional[int] = None,
-        flush_after_seconds: Optional[int] = None,
+        flush_after_seconds: Union[int, float, None] = None,
         **kwargs,
     ):
         self._single_file_mode = False
         if isinstance(partition_cols, str):
             partition_cols = [partition_cols]
         if partition_cols is None:
             if path.endswith(".parquet") or path.endswith(".pq"):
```

### Comparing `storey-1.4.2/storey/transformations/__init__.py` & `storey-1.4.3/storey/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/storey/utils.py` & `storey-1.4.3/storey/utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/storey/windowed_store.py` & `storey-1.4.3/storey/windowed_store.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/storey.egg-info/PKG-INFO` & `storey-1.4.3/storey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storey
-Version: 1.4.2
+Version: 1.4.3
 Summary: Async flows
 Home-page: https://github.com/mlrun/storey
 Author: Iguazio
 Author-email: yaronh@iguazio.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `storey-1.4.2/storey.egg-info/SOURCES.txt` & `storey-1.4.3/storey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/tests/__init__.py` & `storey-1.4.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/tests/test_aggregate_by_key.py` & `storey-1.4.3/tests/test_aggregate_by_key.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/tests/test_aggregate_store.py` & `storey-1.4.3/tests/test_aggregate_store.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/tests/test_flow.py` & `storey-1.4.3/tests/test_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -779,14 +779,38 @@
         await controller.await_termination()
 
 
 def test_write_parquet_flush(tmpdir):
     asyncio.run(async_test_write_parquet_flush(tmpdir))
 
 
+def test_parquet_flush_with_inconsistent_schema_logs_error(tmpdir):
+    out_dir = f"{tmpdir}/test_parquet_flush_with_inconsistent_schema_logs_error/{uuid.uuid4().hex}/"
+
+    logger = MockLogger()
+    context = MockContext(logger, False)
+
+    columns = [("my_int_or_string", "int"), ("my_string", "str")]
+    target = ParquetTarget(
+        out_dir,
+        columns=columns,
+        partition_cols=[],
+        flush_after_seconds=0.5,
+        context=context,
+    )
+    controller = build_flow([SyncEmitSource(), target]).run()
+    controller.emit(["it is actually a string", "abc"])
+    time.sleep(1)
+
+    assert logger.logs[0][1][0].startswith("Failed to flush batch in step 'ParquetTarget':")
+
+    controller.terminate()
+    controller.await_termination()
+
+
 def test_error_flow():
     controller = build_flow(
         [
             SyncEmitSource(),
             Map(lambda x: x + 1),
             Map(RaiseEx(500).raise_ex),
             Reduce(0, lambda acc, x: acc + x),
```

### Comparing `storey-1.4.2/tests/test_steps.py` & `storey-1.4.3/tests/test_steps.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/tests/test_types.py` & `storey-1.4.3/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/tests/test_v3io.py` & `storey-1.4.3/tests/test_v3io.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.2/tests/test_windowed_store.py` & `storey-1.4.3/tests/test_windowed_store.py`

 * *Files identical despite different names*

