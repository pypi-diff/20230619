# Comparing `tmp/sqlalchemy_mock-1.0.4.tar.gz` & `tmp/sqlalchemy_mock-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_mock-1.0.4.tar", max compression
+gzip compressed data, was "sqlalchemy_mock-1.0.5.tar", max compression
```

## Comparing `sqlalchemy_mock-1.0.4.tar` & `sqlalchemy_mock-1.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1647 2023-05-13 14:38:38.650122 sqlalchemy_mock-1.0.4/README.md
--rw-r--r--   0        0        0      448 2023-06-15 17:25:10.662370 sqlalchemy_mock-1.0.4/pyproject.toml
--rw-r--r--   0        0        0       98 2023-06-13 08:13:20.212930 sqlalchemy_mock-1.0.4/sqlalchemy_mock/__init__.py
--rw-r--r--   0        0        0      183 2023-06-13 08:13:20.213067 sqlalchemy_mock-1.0.4/sqlalchemy_mock/async_session.py
--rw-r--r--   0        0        0     4341 2023-06-13 08:13:20.213214 sqlalchemy_mock-1.0.4/sqlalchemy_mock/execute.py
--rw-r--r--   0        0        0     1427 2023-06-13 08:13:20.213390 sqlalchemy_mock-1.0.4/sqlalchemy_mock/query.py
--rw-r--r--   0        0        0     3258 2023-06-13 08:13:20.213584 sqlalchemy_mock-1.0.4/sqlalchemy_mock/session.py
--rw-r--r--   0        0        0     4575 2023-06-15 17:23:23.760224 sqlalchemy_mock-1.0.4/sqlalchemy_mock/utils.py
--rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 sqlalchemy_mock-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1647 2023-05-13 14:38:38.650122 sqlalchemy_mock-1.0.5/README.md
+-rw-r--r--   0        0        0      448 2023-06-19 08:56:10.306028 sqlalchemy_mock-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-06-13 08:13:20.212930 sqlalchemy_mock-1.0.5/sqlalchemy_mock/__init__.py
+-rw-r--r--   0        0        0      183 2023-06-13 08:13:20.213067 sqlalchemy_mock-1.0.5/sqlalchemy_mock/async_session.py
+-rw-r--r--   0        0        0     6433 2023-06-19 08:55:36.792688 sqlalchemy_mock-1.0.5/sqlalchemy_mock/execute.py
+-rw-r--r--   0        0        0     1427 2023-06-13 08:13:20.213390 sqlalchemy_mock-1.0.5/sqlalchemy_mock/query.py
+-rw-r--r--   0        0        0     3369 2023-06-19 08:55:36.792865 sqlalchemy_mock-1.0.5/sqlalchemy_mock/session.py
+-rw-r--r--   0        0        0     4575 2023-06-15 17:23:23.760224 sqlalchemy_mock-1.0.5/sqlalchemy_mock/utils.py
+-rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 sqlalchemy_mock-1.0.5/PKG-INFO
```

### Comparing `sqlalchemy_mock-1.0.4/README.md` & `sqlalchemy_mock-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.4/sqlalchemy_mock/query.py` & `sqlalchemy_mock-1.0.5/sqlalchemy_mock/query.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.4/sqlalchemy_mock/session.py` & `sqlalchemy_mock-1.0.5/sqlalchemy_mock/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,17 @@
         label_columns = self.get_label_columns(record.__class__)
         record = self.process_sql_columns(record, label_columns)
         return record
 
     def mock_session(self):
         return mock_sessions_methods(self)
 
+    def get_records_by_instance(self, instance: object):
+        return self.__storage.get(str(instance), [])
+
     def execute(self, expresion: object, *args, **kwargs):
         if not getattr(expresion, "element", None) is None:
             expresion = expresion.element
 
         expresion_selected_columns = getattr(expresion, "selected_columns", [])
         instance = expresion._propagate_attrs["plugin_subject"].class_
         selected_columns = [column.name for column in expresion_selected_columns]
```

### Comparing `sqlalchemy_mock-1.0.4/sqlalchemy_mock/utils.py` & `sqlalchemy_mock-1.0.5/sqlalchemy_mock/utils.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.4/PKG-INFO` & `sqlalchemy_mock-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-mock
-Version: 1.0.4
+Version: 1.0.5
 Summary: The package for working with SQLAlchemy in unit tests
 Author: ivanostapiuk
 Author-email: ost.ivan13@gmail.com
 Requires-Python: >=3.0,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

