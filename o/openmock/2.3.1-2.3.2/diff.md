# Comparing `tmp/openmock-2.3.1.tar.gz` & `tmp/openmock-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmock-2.3.1.tar", max compression
+gzip compressed data, was "openmock-2.3.2.tar", max compression
```

## Comparing `openmock-2.3.1.tar` & `openmock-2.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1081 2023-06-05 22:38:14.210611 openmock-2.3.1/LICENSE
--rw-r--r--   0        0        0     4946 2023-06-05 22:38:14.210611 openmock-2.3.1/README.md
--rw-r--r--   0        0        0      830 2023-06-05 22:38:14.210611 openmock-2.3.1/openmock/__init__.py
--rw-r--r--   0        0        0      121 2023-06-05 22:38:14.210611 openmock-2.3.1/openmock/behaviour/__init__.py
--rw-r--r--   0        0        0      475 2023-06-05 22:38:14.210611 openmock-2.3.1/openmock/behaviour/server_failure.py
--rw-r--r--   0        0        0     1100 2023-06-05 22:38:14.210611 openmock-2.3.1/openmock/fake_cluster.py
--rw-r--r--   0        0        0     1179 2023-06-05 22:38:14.210611 openmock-2.3.1/openmock/fake_indices.py
--rw-r--r--   0        0        0    39924 2023-06-05 22:38:14.214606 openmock-2.3.1/openmock/fake_opensearch.py
--rw-r--r--   0        0        0     2154 2023-06-05 22:38:14.214606 openmock-2.3.1/openmock/normalize_hosts.py
--rw-r--r--   0        0        0      732 2023-06-05 22:38:14.214606 openmock-2.3.1/openmock/utilities/__init__.py
--rw-r--r--   0        0        0      451 2023-06-05 22:38:14.214606 openmock-2.3.1/openmock/utilities/decorator.py
--rw-r--r--   0        0        0     2302 2023-06-05 22:38:14.214606 openmock-2.3.1/pyproject.toml
--rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 openmock-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-19 17:10:42.530135 openmock-2.3.2/LICENSE
+-rw-r--r--   0        0        0     4946 2023-06-19 17:10:42.530135 openmock-2.3.2/README.md
+-rw-r--r--   0        0        0      830 2023-06-19 17:10:42.530135 openmock-2.3.2/openmock/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-19 17:10:42.530135 openmock-2.3.2/openmock/behaviour/__init__.py
+-rw-r--r--   0        0        0      475 2023-06-19 17:10:42.530135 openmock-2.3.2/openmock/behaviour/server_failure.py
+-rw-r--r--   0        0        0     1100 2023-06-19 17:10:42.530135 openmock-2.3.2/openmock/fake_cluster.py
+-rw-r--r--   0        0        0     1179 2023-06-19 17:10:42.530135 openmock-2.3.2/openmock/fake_indices.py
+-rw-r--r--   0        0        0    40327 2023-06-19 17:10:42.530135 openmock-2.3.2/openmock/fake_opensearch.py
+-rw-r--r--   0        0        0     2154 2023-06-19 17:10:42.530135 openmock-2.3.2/openmock/normalize_hosts.py
+-rw-r--r--   0        0        0      732 2023-06-19 17:10:42.530135 openmock-2.3.2/openmock/utilities/__init__.py
+-rw-r--r--   0        0        0      451 2023-06-19 17:10:42.530135 openmock-2.3.2/openmock/utilities/decorator.py
+-rw-r--r--   0        0        0     2302 2023-06-19 17:10:42.530135 openmock-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 openmock-2.3.2/PKG-INFO
```

### Comparing `openmock-2.3.1/LICENSE` & `openmock-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openmock-2.3.1/README.md` & `openmock-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `openmock-2.3.1/openmock/__init__.py` & `openmock-2.3.2/openmock/__init__.py`

 * *Files identical despite different names*

### Comparing `openmock-2.3.1/openmock/fake_cluster.py` & `openmock-2.3.2/openmock/fake_cluster.py`

 * *Files identical despite different names*

### Comparing `openmock-2.3.1/openmock/fake_indices.py` & `openmock-2.3.2/openmock/fake_indices.py`

 * *Files identical despite different names*

### Comparing `openmock-2.3.1/openmock/fake_opensearch.py` & `openmock-2.3.2/openmock/fake_opensearch.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     TERMS = "TERMS"
     MUST = "MUST"
     RANGE = "RANGE"
     SHOULD = "SHOULD"
     MINIMUM_SHOULD_MATCH = "MINIMUM_SHOULD_MATCH"
     MULTI_MATCH = "MULTI_MATCH"
     MUST_NOT = "MUST_NOT"
+    EXISTS = "EXISTS"
 
     @staticmethod
     def get_query_type(type_str):
         if type_str == "bool":
             return QueryType.BOOL
         if type_str == "filter":
             return QueryType.FILTER
@@ -118,14 +119,16 @@
             return QueryType.SHOULD
         if type_str == "minimum_should_match":
             return QueryType.MINIMUM_SHOULD_MATCH
         if type_str == "multi_match":
             return QueryType.MULTI_MATCH
         if type_str == "must_not":
             return QueryType.MUST_NOT
+        if type_str == "exists":
+            return QueryType.EXISTS
 
         raise NotImplementedError(f"type {type_str} is not implemented for QueryType")
 
 
 class MetricType:
     CARDINALITY = "CARDINALITY"
 
@@ -167,14 +170,16 @@
             return self._evaluate_for_compound_query_type(document)
         if self.type == QueryType.SHOULD:
             return self._evaluate_for_should_query_type(document)
         if self.type == QueryType.MULTI_MATCH:
             return self._evaluate_for_multi_match_query_type(document)
         if self.type == QueryType.MUST_NOT:
             return self._evaluate_for_must_not_query_type(document)
+        if self.type == QueryType.EXISTS:
+            return self._evaluate_for_exists_query_type(document)
         raise NotImplementedError(
             f"Fake query evaluation not implemented for query type: {self.type}"
         )
 
     def _evaluate_for_match_query_type(self, document):
         return self._evaluate_for_field(document, True)
 
@@ -299,29 +304,33 @@
                 if return_val:
                     return True
         return return_val
 
     def _evaluate_for_multi_match_query_type(self, document):
         return self._evaluate_for_fields(document)
 
+    def _evaluate_for_exists_query_type(self, document):
+        doc_source = document["_source"]
+        field = self.condition.get("field")
+        return not self._compare_value_for_field(doc_source, field, None, False)
+
     def _compare_value_for_field(self, doc_source, field, value, ignore_case):
         if ignore_case and isinstance(value, str):
             value = value.lower()
 
         doc_val = doc_source
         # Remove boosting
         field, *_ = field.split("*")
         for k in field.split("."):
             if hasattr(doc_val, k):
                 doc_val = getattr(doc_val, k)
-                break
-            if k in doc_val:
+            elif k in doc_val:
                 doc_val = doc_val[k]
-                break
-            return False
+            else:
+                return False
 
         if not isinstance(doc_val, list):
             doc_val = [doc_val]
 
         for val in doc_val:
             if not isinstance(val, (int, float, complex)) or val is None:
                 val = str(val)
```

### Comparing `openmock-2.3.1/openmock/normalize_hosts.py` & `openmock-2.3.2/openmock/normalize_hosts.py`

 * *Files identical despite different names*

### Comparing `openmock-2.3.1/openmock/utilities/__init__.py` & `openmock-2.3.2/openmock/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `openmock-2.3.1/pyproject.toml` & `openmock-2.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openmock"
-version = "2.3.1"
+version = "2.3.2"
 description = "Python OpenSearch Mock for test purposes"
 authors = ["Marcos Cardoso",
     "Mathew Martin <matthewdeanmartin@gmail.com>"]
 keywords = ["opensearch", "mocking", "testing"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/matthewdeanmartin/openmock"
```

### Comparing `openmock-2.3.1/PKG-INFO` & `openmock-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmock
-Version: 2.3.1
+Version: 2.3.2
 Summary: Python OpenSearch Mock for test purposes
 Home-page: https://github.com/matthewdeanmartin/openmock
 License: MIT
 Keywords: opensearch,mocking,testing
 Author: Marcos Cardoso
 Requires-Python: >=3.9
 Classifier: Environment :: Web Environment
```

