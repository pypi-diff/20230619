# Comparing `tmp/vectordb-0.0.1.tar.gz` & `tmp/vectordb-0.0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vectordb-0.0.1.tar", last modified: Mon Jun 19 11:05:35 2023, max compression
+gzip compressed data, was "vectordb-0.0.1.dev1.tar", last modified: Mon Jun 19 11:05:02 2023, max compression
```

## Comparing `vectordb-0.0.1.tar` & `vectordb-0.0.1.dev1.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:35.000000 vectordb-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-19 11:05:35.000000 vectordb-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-06-19 11:05:21.000000 vectordb-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 11:05:35.000000 vectordb-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-19 11:05:21.000000 vectordb-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:35.000000 vectordb-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:21.000000 vectordb-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-19 11:05:21.000000 vectordb-0.0.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:35.000000 vectordb-0.0.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:21.000000 vectordb-0.0.1/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-06-19 11:05:21.000000 vectordb-0.0.1/tests/integration/test_hnswlib_vectordb_serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-06-19 11:05:21.000000 vectordb-0.0.1/tests/integration/test_inmemory_vectordb_serve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:35.000000 vectordb-0.0.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:21.000000 vectordb-0.0.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-06-19 11:05:21.000000 vectordb-0.0.1/tests/unit/test_hnswlib_vectordb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-06-19 11:05:21.000000 vectordb-0.0.1/tests/unit/test_inmemory_vectordb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:35.000000 vectordb-0.0.1/vectordb/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-19 11:05:21.000000 vectordb-0.0.1/vectordb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-19 11:05:21.000000 vectordb-0.0.1/vectordb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:35.000000 vectordb-0.0.1/vectordb/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:21.000000 vectordb-0.0.1/vectordb/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-19 11:05:21.000000 vectordb-0.0.1/vectordb/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:35.000000 vectordb-0.0.1/vectordb/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:21.000000 vectordb-0.0.1/vectordb/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-06-19 11:05:21.000000 vectordb-0.0.1/vectordb/db/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:35.000000 vectordb-0.0.1/vectordb/db/executors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:21.000000 vectordb-0.0.1/vectordb/db/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-19 11:05:21.000000 vectordb-0.0.1/vectordb/db/executors/hnsw_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-19 11:05:21.000000 vectordb-0.0.1/vectordb/db/executors/inmemory_exact_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-19 11:05:21.000000 vectordb-0.0.1/vectordb/db/executors/typed_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-19 11:05:21.000000 vectordb-0.0.1/vectordb/db/hnsw_vectordb.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-19 11:05:21.000000 vectordb-0.0.1/vectordb/db/inmemory_exact_vectordb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-19 11:05:21.000000 vectordb-0.0.1/vectordb/db/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:35.000000 vectordb-0.0.1/vectordb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:21.000000 vectordb-0.0.1/vectordb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-19 11:05:21.000000 vectordb-0.0.1/vectordb/utils/create_doc_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-19 11:05:21.000000 vectordb-0.0.1/vectordb/utils/pass_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-19 11:05:21.000000 vectordb-0.0.1/vectordb/utils/push_to_hubble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-19 11:05:21.000000 vectordb-0.0.1/vectordb/utils/sort_matches_by_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-19 11:05:21.000000 vectordb-0.0.1/vectordb/utils/unify_input_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:35.000000 vectordb-0.0.1/vectordb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-19 11:05:35.000000 vectordb-0.0.1/vectordb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-19 11:05:35.000000 vectordb-0.0.1/vectordb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 11:05:35.000000 vectordb-0.0.1/vectordb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-19 11:05:35.000000 vectordb-0.0.1/vectordb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-19 11:05:35.000000 vectordb-0.0.1/vectordb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-19 11:05:35.000000 vectordb-0.0.1/vectordb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:02.515303 vectordb-0.0.1.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-19 11:05:02.515303 vectordb-0.0.1.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 11:05:02.515303 vectordb-0.0.1.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:02.507303 vectordb-0.0.1.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:02.507303 vectordb-0.0.1.dev1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/tests/integration/test_hnswlib_vectordb_serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/tests/integration/test_inmemory_vectordb_serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:02.507303 vectordb-0.0.1.dev1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/tests/unit/test_hnswlib_vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/tests/unit/test_inmemory_vectordb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:02.507303 vectordb-0.0.1.dev1/vectordb/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-19 11:05:02.000000 vectordb-0.0.1.dev1/vectordb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/vectordb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:02.511303 vectordb-0.0.1.dev1/vectordb/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/vectordb/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/vectordb/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:02.511303 vectordb-0.0.1.dev1/vectordb/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/vectordb/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/vectordb/db/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:02.511303 vectordb-0.0.1.dev1/vectordb/db/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/vectordb/db/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/vectordb/db/executors/hnsw_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/vectordb/db/executors/inmemory_exact_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/vectordb/db/executors/typed_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/vectordb/db/hnsw_vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/vectordb/db/inmemory_exact_vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/vectordb/db/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:02.511303 vectordb-0.0.1.dev1/vectordb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/vectordb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/vectordb/utils/create_doc_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/vectordb/utils/pass_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/vectordb/utils/push_to_hubble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/vectordb/utils/sort_matches_by_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-19 11:04:55.000000 vectordb-0.0.1.dev1/vectordb/utils/unify_input_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:02.511303 vectordb-0.0.1.dev1/vectordb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-19 11:05:02.000000 vectordb-0.0.1.dev1/vectordb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-19 11:05:02.000000 vectordb-0.0.1.dev1/vectordb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 11:05:02.000000 vectordb-0.0.1.dev1/vectordb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-19 11:05:02.000000 vectordb-0.0.1.dev1/vectordb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-19 11:05:02.000000 vectordb-0.0.1.dev1/vectordb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-19 11:05:02.000000 vectordb-0.0.1.dev1/vectordb.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vectordb-0.0.1/PKG-INFO` & `vectordb-0.0.1.dev1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: vectordb
-Version: 0.0.1
+Version: 0.0.1.dev1
 Summary: The Python VectorDB. Build your vector database from working as a library to scaling as a database in the cloud
 Home-page: https://github.com/jina-ai/vectordb/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/vectordb/tags
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Provides-Extra: test
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `vectordb-0.0.1/README.md` & `vectordb-0.0.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.1/setup.py` & `vectordb-0.0.1.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.1/tests/integration/test_hnswlib_vectordb_serve.py` & `vectordb-0.0.1.dev1/tests/integration/test_hnswlib_vectordb_serve.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.1/tests/integration/test_inmemory_vectordb_serve.py` & `vectordb-0.0.1.dev1/tests/integration/test_inmemory_vectordb_serve.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.1/tests/unit/test_hnswlib_vectordb.py` & `vectordb-0.0.1.dev1/tests/unit/test_hnswlib_vectordb.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.1/tests/unit/test_inmemory_vectordb.py` & `vectordb-0.0.1.dev1/tests/unit/test_inmemory_vectordb.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.1/vectordb/__main__.py` & `vectordb-0.0.1.dev1/vectordb/__main__.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.1/vectordb/client/client.py` & `vectordb-0.0.1.dev1/vectordb/client/client.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.1/vectordb/db/base.py` & `vectordb-0.0.1.dev1/vectordb/db/base.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.1/vectordb/db/executors/hnsw_indexer.py` & `vectordb-0.0.1.dev1/vectordb/db/executors/hnsw_indexer.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.1/vectordb/db/executors/inmemory_exact_indexer.py` & `vectordb-0.0.1.dev1/vectordb/db/executors/inmemory_exact_indexer.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.1/vectordb/db/executors/typed_executor.py` & `vectordb-0.0.1.dev1/vectordb/db/executors/typed_executor.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.1/vectordb/db/service.py` & `vectordb-0.0.1.dev1/vectordb/db/service.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.1/vectordb/utils/create_doc_type.py` & `vectordb-0.0.1.dev1/vectordb/utils/create_doc_type.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.1/vectordb/utils/pass_parameters.py` & `vectordb-0.0.1.dev1/vectordb/utils/pass_parameters.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.1/vectordb/utils/push_to_hubble.py` & `vectordb-0.0.1.dev1/vectordb/utils/push_to_hubble.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.1/vectordb/utils/sort_matches_by_score.py` & `vectordb-0.0.1.dev1/vectordb/utils/sort_matches_by_score.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.1/vectordb/utils/unify_input_output.py` & `vectordb-0.0.1.dev1/vectordb/utils/unify_input_output.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.1/vectordb.egg-info/PKG-INFO` & `vectordb-0.0.1.dev1/vectordb.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: vectordb
-Version: 0.0.1
+Version: 0.0.1.dev1
 Summary: The Python VectorDB. Build your vector database from working as a library to scaling as a database in the cloud
 Home-page: https://github.com/jina-ai/vectordb/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/vectordb/tags
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Provides-Extra: test
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `vectordb-0.0.1/vectordb.egg-info/SOURCES.txt` & `vectordb-0.0.1.dev1/vectordb.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 tests/__init__.py
 tests/conftest.py
 tests/integration/__init__.py
 tests/integration/test_hnswlib_vectordb_serve.py
 tests/integration/test_inmemory_vectordb_serve.py
```

