# Comparing `tmp/opensearch_orm-0.1.8.tar.gz` & `tmp/opensearch_orm-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensearch_orm-0.1.8.tar", max compression
+gzip compressed data, was "opensearch_orm-0.1.9.tar", max compression
```

## Comparing `opensearch_orm-0.1.8.tar` & `opensearch_orm-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-04-16 08:43:48.684499 opensearch_orm-0.1.8/LICENSE
--rw-r--r--   0        0        0     3199 2023-06-17 07:12:43.411841 opensearch_orm-0.1.8/README.md
--rw-r--r--   0        0        0      120 2023-04-16 08:43:48.684682 opensearch_orm-0.1.8/opensearchorm/__init__.py
--rw-r--r--   0        0        0     1456 2023-04-16 08:43:48.684860 opensearch_orm-0.1.8/opensearchorm/aggs.py
--rw-r--r--   0        0        0      254 2023-04-16 08:43:48.684942 opensearch_orm-0.1.8/opensearchorm/model.py
--rw-r--r--   0        0        0     5570 2023-06-17 04:45:40.491762 opensearch_orm-0.1.8/opensearchorm/query.py
--rw-r--r--   0        0        0     6598 2023-06-19 09:46:32.475159 opensearch_orm-0.1.8/opensearchorm/session.py
--rw-r--r--   0        0        0      497 2023-04-16 08:43:48.685191 opensearch_orm-0.1.8/opensearchorm/utils.py
--rw-r--r--   0        0        0      444 2023-06-19 14:39:11.001306 opensearch_orm-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3814 1970-01-01 00:00:00.000000 opensearch_orm-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-16 08:43:48.684499 opensearch_orm-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3199 2023-06-17 07:12:43.411841 opensearch_orm-0.1.9/README.md
+-rw-r--r--   0        0        0      120 2023-04-16 08:43:48.684682 opensearch_orm-0.1.9/opensearchorm/__init__.py
+-rw-r--r--   0        0        0     1456 2023-04-16 08:43:48.684860 opensearch_orm-0.1.9/opensearchorm/aggs.py
+-rw-r--r--   0        0        0      254 2023-04-16 08:43:48.684942 opensearch_orm-0.1.9/opensearchorm/model.py
+-rw-r--r--   0        0        0     5570 2023-06-17 04:45:40.491762 opensearch_orm-0.1.9/opensearchorm/query.py
+-rw-r--r--   0        0        0     6598 2023-06-19 09:46:32.475159 opensearch_orm-0.1.9/opensearchorm/session.py
+-rw-r--r--   0        0        0      497 2023-04-16 08:43:48.685191 opensearch_orm-0.1.9/opensearchorm/utils.py
+-rw-r--r--   0        0        0      443 2023-06-19 14:51:43.058855 opensearch_orm-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3813 1970-01-01 00:00:00.000000 opensearch_orm-0.1.9/PKG-INFO
```

### Comparing `opensearch_orm-0.1.8/LICENSE` & `opensearch_orm-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `opensearch_orm-0.1.8/README.md` & `opensearch_orm-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `opensearch_orm-0.1.8/opensearchorm/aggs.py` & `opensearch_orm-0.1.9/opensearchorm/aggs.py`

 * *Files identical despite different names*

### Comparing `opensearch_orm-0.1.8/opensearchorm/query.py` & `opensearch_orm-0.1.9/opensearchorm/query.py`

 * *Files identical despite different names*

### Comparing `opensearch_orm-0.1.8/opensearchorm/session.py` & `opensearch_orm-0.1.9/opensearchorm/session.py`

 * *Files identical despite different names*

### Comparing `opensearch_orm-0.1.8/PKG-INFO` & `opensearch_orm-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: opensearch-orm
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: yim7
 Author-email: yimchiu7@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: opensearch-py (>=2.0.0,<3.0.0)
-Requires-Dist: pydantic (>=1.10.0,<2.0.0)
+Requires-Dist: opensearch-py (>=1.0.0,<2.0.0)
+Requires-Dist: pydantic (>=1.6.0,<2.0.0)
 Requires-Dist: pytz (>=2022.2.1,<2023.0.0)
 Description-Content-Type: text/markdown
 
 # OpenSearch ORM
 `opensearch-orm` is a high-level OpenSearch ORM for Python. The query syntax is similar to django-orm.
 
 May be compatible with Elasticsearch, depending on opensearch-py.
```

