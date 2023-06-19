# Comparing `tmp/pytmlib-1.0.0rc5.tar.gz` & `tmp/pytmlib-1.1.0.dev0.tar.gz`

## Comparing `pytmlib-1.0.0rc5.tar` & `pytmlib-1.1.0.dev0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/__init__.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/abstract_exercise.py
--rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/api.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/archiver.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/context.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/create_app.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/handle_error.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/latex.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/method_call_exception.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/serializer.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/output/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/output/abstract.py
--rw-r--r--   0        0        0     8898 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/output/builder.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/output/button.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/output/field.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/output/field_attribute.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/output/field_type_enum.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/output/figure.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/output/image.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/output/option.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/output/option_group.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/output/paragraph.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/output/table.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pytmlib/output/table_cell.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/LICENSE
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/README.md
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/pyproject.toml
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc5/PKG-INFO
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/abstract_exercise.py
+-rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/api.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/archiver.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/context.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/create_app.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/handle_error.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/latex.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/method_call_exception.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/serializer.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/output/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/output/abstract.py
+-rw-r--r--   0        0        0     8898 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/output/builder.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/output/button.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/output/field.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/output/field_attribute.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/output/field_type_enum.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/output/figure.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/output/image.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/output/option.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/output/option_group.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/output/paragraph.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/output/table.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pytmlib/output/table_cell.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/LICENSE
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/README.md
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 pytmlib-1.1.0.dev0/PKG-INFO
```

### Comparing `pytmlib-1.0.0rc5/pytmlib/api.py` & `pytmlib-1.1.0.dev0/pytmlib/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,22 +34,36 @@
     def blueprint(self) -> Blueprint:
         return self._blueprint
 
     def handle_start(self) -> Response:
         result: 'OutputBuilder' = self._call_method(self.context.exercise.start)
         json: dict = result.to_json()
         envelop = self._wrap_with_envelop(json)
+
+        return jsonify(envelop)
+
+    def handle_entrypoints(self) -> Response:
+        try:
+            entrypoints = self.context.exercise.entrypoints()
+        except BaseException as reason:
+            raise MethodCallException() from reason
+
+        json: list = [entrypoint.__name__ for entrypoint in entrypoints]
+
+        envelop = self._wrap_with_envelop(json)
+
         return jsonify(envelop)
 
     def handle_action(self, action: str) -> Response:
         method: Callable[..., 'OutputBuilder'] = getattr(self.context.exercise, action, None)
         envelop_in: dict = request.json
         result: 'OutputBuilder' = self._call_action(method, envelop_in)
         json: dict = result.to_json()
         envelop_out: dict = self._wrap_with_envelop(json)
+
         return jsonify(envelop_out)
 
     def handle_upload(self) -> Response:
         data: bytes = Archiver('.').create_tar()
         mimetype: str = 'application/tar+gzip'
         b64_encoded_data: str = b64encode(data).decode('utf-8')
         data_uri: str = 'data:%s;base64,%s' % (mimetype, b64_encoded_data)
@@ -59,14 +73,15 @@
         return jsonify(json_data)
 
     def _create_blueprint(self) -> Blueprint:
         api: Blueprint = Blueprint('api', __name__)
 
         CORS(api)
 
+        api.add_url_rule('/entrypoints', 'entrypoints', self.handle_entrypoints, methods=['GET'])
         api.add_url_rule('/start', 'start', self.handle_start, methods=['GET'])
         api.add_url_rule('/call/<action>', 'call', self.handle_action, methods=['POST'])
         api.add_url_rule('/upload', 'upload', self.handle_upload, methods=['GET'])
 
         return api
 
     def _wrap_with_envelop(self, payload: Union[list, dict, str, int, float]) -> dict:
@@ -117,9 +132,9 @@
         elif parameter.kind == Parameter.VAR_KEYWORD:
             arguments.update(**applicable_arguments)
 
     @staticmethod
     def _call_method(method: Callable[..., 'OutputBuilder'], **kwargs) -> 'OutputBuilder':
         try:
             return method(**kwargs)
-        except BaseException as e:
-            raise MethodCallException() from e
+        except BaseException as reason:
+            raise MethodCallException() from reason
```

### Comparing `pytmlib-1.0.0rc5/pytmlib/archiver.py` & `pytmlib-1.1.0.dev0/pytmlib/archiver.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc5/pytmlib/context.py` & `pytmlib-1.1.0.dev0/pytmlib/context.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc5/pytmlib/create_app.py` & `pytmlib-1.1.0.dev0/pytmlib/create_app.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc5/pytmlib/handle_error.py` & `pytmlib-1.1.0.dev0/pytmlib/handle_error.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc5/pytmlib/serializer.py` & `pytmlib-1.1.0.dev0/pytmlib/serializer.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc5/pytmlib/output/abstract.py` & `pytmlib-1.1.0.dev0/pytmlib/output/abstract.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc5/pytmlib/output/builder.py` & `pytmlib-1.1.0.dev0/pytmlib/output/builder.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc5/pytmlib/output/button.py` & `pytmlib-1.1.0.dev0/pytmlib/output/button.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc5/pytmlib/output/field.py` & `pytmlib-1.1.0.dev0/pytmlib/output/field.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc5/pytmlib/output/figure.py` & `pytmlib-1.1.0.dev0/pytmlib/output/figure.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc5/pytmlib/output/image.py` & `pytmlib-1.1.0.dev0/pytmlib/output/image.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc5/pytmlib/output/option.py` & `pytmlib-1.1.0.dev0/pytmlib/output/option.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc5/pytmlib/output/option_group.py` & `pytmlib-1.1.0.dev0/pytmlib/output/option_group.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc5/pytmlib/output/paragraph.py` & `pytmlib-1.1.0.dev0/pytmlib/output/paragraph.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc5/pytmlib/output/table.py` & `pytmlib-1.1.0.dev0/pytmlib/output/table.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc5/pytmlib/output/table_cell.py` & `pytmlib-1.1.0.dev0/pytmlib/output/table_cell.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc5/LICENSE` & `pytmlib-1.1.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc5/pyproject.toml` & `pytmlib-1.1.0.dev0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytmlib"
-version = "1.0.0rc5"
+version = "1.1.0dev0"
 authors = [
     { name = "Oliver Fabel", email = "oliver.fabel@fhnw.ch" },
 ]
 description = "This is the base library for the Python Tool Manager."
 readme = "README.md"
-license = { file = "LICENSE" }
+license = "MIT"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

