# Comparing `tmp/pytmlib-1.1.0.dev2.tar.gz` & `tmp/pytmlib-1.1.0.dev3.tar.gz`

## Comparing `pytmlib-1.1.0.dev2.tar` & `pytmlib-1.1.0.dev3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/__init__.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/abstract_exercise.py
--rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/api.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/archiver.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/context.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/create_app.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/exceptions.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/handle_error.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/latex.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/serializer.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/output/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/output/abstract.py
--rw-r--r--   0        0        0     8898 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/output/builder.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/output/button.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/output/field.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/output/field_attribute.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/output/field_type_enum.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/output/figure.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/output/image.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/output/option.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/output/option_group.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/output/paragraph.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/output/table.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pytmlib/output/table_cell.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/LICENSE
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/README.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/pyproject.toml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/__init__.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/abstract_exercise.py
+-rw-r--r--   0        0        0     6046 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/api.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/archiver.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/context.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/create_app.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/exceptions.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/handle_error.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/latex.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/serializer.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/abstract.py
+-rw-r--r--   0        0        0     8898 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/builder.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/button.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/field.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/field_attribute.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/field_type_enum.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/figure.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/image.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/option.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/option_group.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/paragraph.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/table.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pytmlib/output/table_cell.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/LICENSE
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/README.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev3/PKG-INFO
```

### Comparing `pytmlib-1.1.0.dev2/pytmlib/abstract_exercise.py` & `pytmlib-1.1.0.dev3/pytmlib/abstract_exercise.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev2/pytmlib/api.py` & `pytmlib-1.1.0.dev3/pytmlib/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     def _create_blueprint(self) -> Blueprint:
         api: Blueprint = Blueprint('api', __name__)
 
         CORS(api)
 
         api.add_url_rule('/entrypoints', 'entrypoints', self.handle_entrypoints, methods=['GET'])
         api.add_url_rule('/start', 'start', self.handle_start, methods=['GET'])
-        api.add_url_rule('/entry/<entrypoint>', self.handle_entrypoint, methods=['GET'])
+        api.add_url_rule('/entry/<entrypoint>', 'entry', self.handle_entrypoint, methods=['GET'])
         api.add_url_rule('/call/<action>', 'call', self.handle_action, methods=['POST'])
         api.add_url_rule('/upload', 'upload', self.handle_upload, methods=['GET'])
 
         return api
 
     def _wrap_with_envelop(self, payload: Union[list, dict, str, int, float]) -> dict:
         return {
```

### Comparing `pytmlib-1.1.0.dev2/pytmlib/archiver.py` & `pytmlib-1.1.0.dev3/pytmlib/archiver.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev2/pytmlib/context.py` & `pytmlib-1.1.0.dev3/pytmlib/context.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev2/pytmlib/create_app.py` & `pytmlib-1.1.0.dev3/pytmlib/create_app.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev2/pytmlib/handle_error.py` & `pytmlib-1.1.0.dev3/pytmlib/handle_error.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev2/pytmlib/serializer.py` & `pytmlib-1.1.0.dev3/pytmlib/serializer.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev2/pytmlib/output/abstract.py` & `pytmlib-1.1.0.dev3/pytmlib/output/abstract.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev2/pytmlib/output/builder.py` & `pytmlib-1.1.0.dev3/pytmlib/output/builder.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev2/pytmlib/output/button.py` & `pytmlib-1.1.0.dev3/pytmlib/output/button.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev2/pytmlib/output/field.py` & `pytmlib-1.1.0.dev3/pytmlib/output/field.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev2/pytmlib/output/figure.py` & `pytmlib-1.1.0.dev3/pytmlib/output/figure.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev2/pytmlib/output/image.py` & `pytmlib-1.1.0.dev3/pytmlib/output/image.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev2/pytmlib/output/option.py` & `pytmlib-1.1.0.dev3/pytmlib/output/option.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev2/pytmlib/output/option_group.py` & `pytmlib-1.1.0.dev3/pytmlib/output/option_group.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev2/pytmlib/output/paragraph.py` & `pytmlib-1.1.0.dev3/pytmlib/output/paragraph.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev2/pytmlib/output/table.py` & `pytmlib-1.1.0.dev3/pytmlib/output/table.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev2/pytmlib/output/table_cell.py` & `pytmlib-1.1.0.dev3/pytmlib/output/table_cell.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev2/LICENSE` & `pytmlib-1.1.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytmlib-1.1.0.dev2/pyproject.toml` & `pytmlib-1.1.0.dev3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytmlib"
-version = "1.1.0.dev2"
+version = "1.1.0.dev3"
 authors = [
     { name = "Oliver Fabel", email = "oliver.fabel@fhnw.ch" },
 ]
 description = "This is the base library for the Python Tool Manager."
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
```

### Comparing `pytmlib-1.1.0.dev2/PKG-INFO` & `pytmlib-1.1.0.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmlib
-Version: 1.1.0.dev2
+Version: 1.1.0.dev3
 Summary: This is the base library for the Python Tool Manager.
 Project-URL: Homepage, https://github.com/ofabel/pytm-bootstrap
 Project-URL: Bug Tracker, https://github.com/ofabel/pytm-bootstrap/issues
 Project-URL: Changelog, https://github.com/ofabel/pytm-bootstrap/blob/main/CHANGELOG.md
 Author-email: Oliver Fabel <oliver.fabel@fhnw.ch>
 License-Expression: MIT
 License-File: LICENSE
```

