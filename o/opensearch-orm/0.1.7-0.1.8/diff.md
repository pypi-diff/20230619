# Comparing `tmp/opensearch_orm-0.1.7.tar.gz` & `tmp/opensearch_orm-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensearch_orm-0.1.7.tar", max compression
+gzip compressed data, was "opensearch_orm-0.1.8.tar", max compression
```

## Comparing `opensearch_orm-0.1.7.tar` & `opensearch_orm-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-04-16 08:43:48.684499 opensearch_orm-0.1.7/LICENSE
--rw-r--r--   0        0        0     3199 2023-06-17 07:12:43.411841 opensearch_orm-0.1.7/README.md
--rw-r--r--   0        0        0      120 2023-04-16 08:43:48.684682 opensearch_orm-0.1.7/opensearchorm/__init__.py
--rw-r--r--   0        0        0     1456 2023-04-16 08:43:48.684860 opensearch_orm-0.1.7/opensearchorm/aggs.py
--rw-r--r--   0        0        0      254 2023-04-16 08:43:48.684942 opensearch_orm-0.1.7/opensearchorm/model.py
--rw-r--r--   0        0        0     5570 2023-06-17 04:45:40.491762 opensearch_orm-0.1.7/opensearchorm/query.py
--rw-r--r--   0        0        0     6281 2023-04-16 09:17:40.380146 opensearch_orm-0.1.7/opensearchorm/session.py
--rw-r--r--   0        0        0      497 2023-04-16 08:43:48.685191 opensearch_orm-0.1.7/opensearchorm/utils.py
--rw-r--r--   0        0        0      444 2023-06-17 07:09:39.781719 opensearch_orm-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3814 1970-01-01 00:00:00.000000 opensearch_orm-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-16 08:43:48.684499 opensearch_orm-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3199 2023-06-17 07:12:43.411841 opensearch_orm-0.1.8/README.md
+-rw-r--r--   0        0        0      120 2023-04-16 08:43:48.684682 opensearch_orm-0.1.8/opensearchorm/__init__.py
+-rw-r--r--   0        0        0     1456 2023-04-16 08:43:48.684860 opensearch_orm-0.1.8/opensearchorm/aggs.py
+-rw-r--r--   0        0        0      254 2023-04-16 08:43:48.684942 opensearch_orm-0.1.8/opensearchorm/model.py
+-rw-r--r--   0        0        0     5570 2023-06-17 04:45:40.491762 opensearch_orm-0.1.8/opensearchorm/query.py
+-rw-r--r--   0        0        0     6598 2023-06-19 09:46:32.475159 opensearch_orm-0.1.8/opensearchorm/session.py
+-rw-r--r--   0        0        0      497 2023-04-16 08:43:48.685191 opensearch_orm-0.1.8/opensearchorm/utils.py
+-rw-r--r--   0        0        0      444 2023-06-19 14:39:11.001306 opensearch_orm-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3814 1970-01-01 00:00:00.000000 opensearch_orm-0.1.8/PKG-INFO
```

### Comparing `opensearch_orm-0.1.7/LICENSE` & `opensearch_orm-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `opensearch_orm-0.1.7/README.md` & `opensearch_orm-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `opensearch_orm-0.1.7/opensearchorm/aggs.py` & `opensearch_orm-0.1.8/opensearchorm/aggs.py`

 * *Files identical despite different names*

### Comparing `opensearch_orm-0.1.7/opensearchorm/query.py` & `opensearch_orm-0.1.8/opensearchorm/query.py`

 * *Files identical despite different names*

### Comparing `opensearch_orm-0.1.7/opensearchorm/session.py` & `opensearch_orm-0.1.8/opensearchorm/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 
 class QueryExecutor(Generic[Model]):
     def __init__(self, model_cls: Type[Model], session: SearchSession):
         self.__query = ModelQuery(model_cls)
         self.__model_cls = model_cls
         self.__limit: Optional[int] = None
         self.__offset: Optional[int] = None
+        self.__sort: list = []
         self.__session = session
 
     def filter(self, *args: Expr, **kwargs):
         self.__query.filter(*args, **kwargs)
         return self
 
     def union(self, *args: Expr, **kwargs):
@@ -82,23 +83,32 @@
         self.__limit = limit
         return self
 
     def offset(self, offset: int):
         self.__offset = offset
         return self
 
+    def sort_by(self, *fields: str):
+        sort = []
+        for field in fields:
+            order = 'desc' if field.startswith('-') else 'asc'
+            field = field.strip('+-')
+            sort.append({field: order})
+        self.__sort = sort
+
     def _search(self, fields: List[str], **kwargs):
         """
         :arg fields: include source fields
 
         :arg kwargs: any additional arguments will be passed on to the opensearch-py call
         """
 
         body = {
             'query': self.__query.compile(),
+            'sort': self.__sort,
         }
         logging.debug('query:\n%s', json.dumps(body))
 
         model = self.__model_cls
         assert model and model.__index__, 'model has no index'
 
         resp = self.__session.search(
```

### Comparing `opensearch_orm-0.1.7/PKG-INFO` & `opensearch_orm-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: opensearch-orm
-Version: 0.1.7
+Version: 0.1.8
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
 Requires-Dist: opensearch-py (>=2.0.0,<3.0.0)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: pydantic (>=1.10.0,<2.0.0)
 Requires-Dist: pytz (>=2022.2.1,<2023.0.0)
 Description-Content-Type: text/markdown
 
 # OpenSearch ORM
 `opensearch-orm` is a high-level OpenSearch ORM for Python. The query syntax is similar to django-orm.
 
 May be compatible with Elasticsearch, depending on opensearch-py.
```

