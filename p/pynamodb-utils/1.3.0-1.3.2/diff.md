# Comparing `tmp/pynamodb_utils-1.3.0.tar.gz` & `tmp/pynamodb_utils-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamodb_utils-1.3.0.tar", last modified: Fri Jun 16 19:02:07 2023, max compression
+gzip compressed data, was "pynamodb_utils-1.3.2.tar", last modified: Mon Jun 19 12:21:54 2023, max compression
```

## Comparing `pynamodb_utils-1.3.0.tar` & `pynamodb_utils-1.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:02:07.288944 pynamodb_utils-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-16 19:02:07.288944 pynamodb_utils-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-16 19:02:07.288944 pynamodb_utils-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:02:07.284944 pynamodb_utils-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:02:07.288944 pynamodb_utils-1.3.0/src/pynamodb_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/src/pynamodb_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/src/pynamodb_utils/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/src/pynamodb_utils/conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/src/pynamodb_utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/src/pynamodb_utils/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/src/pynamodb_utils/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/src/pynamodb_utils/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/src/pynamodb_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:02:07.288944 pynamodb_utils-1.3.0/src/pynamodb_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-16 19:02:07.000000 pynamodb_utils-1.3.0/src/pynamodb_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-16 19:02:07.000000 pynamodb_utils-1.3.0/src/pynamodb_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 19:02:07.000000 pynamodb_utils-1.3.0/src/pynamodb_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 19:02:07.000000 pynamodb_utils-1.3.0/src/pynamodb_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-16 19:02:07.000000 pynamodb_utils-1.3.0/src/pynamodb_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:21:54.878835 pynamodb_utils-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-19 12:21:47.000000 pynamodb_utils-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-19 12:21:54.878835 pynamodb_utils-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-19 12:21:47.000000 pynamodb_utils-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-19 12:21:54.878835 pynamodb_utils-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-19 12:21:47.000000 pynamodb_utils-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:21:54.878835 pynamodb_utils-1.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:21:54.878835 pynamodb_utils-1.3.2/src/pynamodb_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-19 12:21:47.000000 pynamodb_utils-1.3.2/src/pynamodb_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-19 12:21:47.000000 pynamodb_utils-1.3.2/src/pynamodb_utils/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-19 12:21:47.000000 pynamodb_utils-1.3.2/src/pynamodb_utils/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-19 12:21:47.000000 pynamodb_utils-1.3.2/src/pynamodb_utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-19 12:21:47.000000 pynamodb_utils-1.3.2/src/pynamodb_utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-06-19 12:21:47.000000 pynamodb_utils-1.3.2/src/pynamodb_utils/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-19 12:21:47.000000 pynamodb_utils-1.3.2/src/pynamodb_utils/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-19 12:21:47.000000 pynamodb_utils-1.3.2/src/pynamodb_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:21:54.878835 pynamodb_utils-1.3.2/src/pynamodb_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-19 12:21:54.000000 pynamodb_utils-1.3.2/src/pynamodb_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-19 12:21:54.000000 pynamodb_utils-1.3.2/src/pynamodb_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 12:21:54.000000 pynamodb_utils-1.3.2/src/pynamodb_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-19 12:21:54.000000 pynamodb_utils-1.3.2/src/pynamodb_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-19 12:21:54.000000 pynamodb_utils-1.3.2/src/pynamodb_utils.egg-info/top_level.txt
```

### Comparing `pynamodb_utils-1.3.0/LICENSE` & `pynamodb_utils-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamodb_utils-1.3.0/PKG-INFO` & `pynamodb_utils-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamodb_utils
-Version: 1.3.0
+Version: 1.3.2
 Summary: Utilities package for pynamodb.
 Home-page: https://github.com/micmurawski/pynamodb-utils/
 Author: Michal Murawski
 Author-email: mmurawski777@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pynamodb_utils-1.3.0/README.md` & `pynamodb_utils-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pynamodb_utils-1.3.0/setup.py` & `pynamodb_utils-1.3.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def read(*parts):
     return codecs.open(os.path.join(HERE, *parts), "r").read()
 
 
 setup(
     name="pynamodb_utils",
-    version="1.3.0",
+    version="1.3.2",
     author="Michal Murawski",
     author_email="mmurawski777@gmail.com",
     description="Utilities package for pynamodb.",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/micmurawski/pynamodb-utils/",
     package_dir={"": "src"},
```

### Comparing `pynamodb_utils-1.3.0/src/pynamodb_utils/attributes.py` & `pynamodb_utils-1.3.2/src/pynamodb_utils/attributes.py`

 * *Files identical despite different names*

### Comparing `pynamodb_utils-1.3.0/src/pynamodb_utils/conditions.py` & `pynamodb_utils-1.3.2/src/pynamodb_utils/conditions.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,20 +39,28 @@
 
     key: str
     value: Any
     for key, value in args.items():
         array: List[str] = key.rsplit('__', 1)
         field_path: str = array[0]
         operator_name: str = array[1] if len(array) > 1 and array[1] != 'not' else ''
+
+        if "." in field_path:
+            _field_path = field_path.split(".", 1)[0] + ".*"
+            is_available = _field_path in available_attributes
+        else:
+
+            is_available = field_path in available_attributes
+
         if operator_name.replace('not_', '') not in OPERATORS_MAPPING:
             raise FilterError(
                 message={key: [f'Operator {operator_name} does not exist.'
                                f' Choose some of available: {", ".join(OPERATORS_MAPPING.keys())}']}
             )
-        if field_path not in available_attributes and raise_exception:
+        if not is_available and raise_exception:
             raise FilterError(
                 message={
                     field_path: [
                         f"Parameter {field_path} does not exist."
                         f' Choose some of available: {", ".join(available_attributes)}'
                     ]
                 }
```

### Comparing `pynamodb_utils-1.3.0/src/pynamodb_utils/models.py` & `pynamodb_utils-1.3.2/src/pynamodb_utils/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,40 +10,41 @@
 
 
 class JSONQueryModel(Model):
     class Meta:
         abstract = True
 
     @classmethod
-    def get_conditions_from_json(cls, query: dict) -> Condition:
+    def get_conditions_from_json(cls, query: dict, raise_exception: bool = True) -> Condition:
         """
             Class method parses query dictionary and returns computed pynamodb condition.
 
             Parameters:
                     query (dict): A decimal integer
 
             Returns:
                     condtion (Condition): computed pynamodb condition
         """
         query_unavailable_attributes: List[str] = getattr(cls.Meta, "query_unavailable_attributes", [])
-        return ConditionsSerializer(cls, query_unavailable_attributes).load(data=query)
+        return ConditionsSerializer(cls, query_unavailable_attributes).load(data=query, raise_exception=raise_exception)
 
     @classmethod
-    def make_index_query(cls, query: dict, **kwargs) -> ResultIterator[Model]:
+    def make_index_query(cls, query: dict, raise_exception: bool = True, **kwargs) -> ResultIterator[Model]:
         """
             Class method parses query dictionary and executes query on index most suitable index
 
             Parameters:
                     query (dict): A decimal integer
 
             Returns:
                     result_iterator (result_iterator): result iterator for optimized query
         """
         query_unavailable_attributes: List[str] = getattr(cls.Meta, "query_unavailable_attributes", [])
-        idx, query = QuerySerializer(cls, query_unavailable_attributes).load(data=query)
+        idx, query = QuerySerializer(cls, query_unavailable_attributes).load(
+            data=query, raise_exception=raise_exception)
         return idx.query(**query, **kwargs)
 
 
 class AsDictModel(Model):
     class Meta:
         abstract = True
```

### Comparing `pynamodb_utils-1.3.0/src/pynamodb_utils/parsers.py` & `pynamodb_utils-1.3.2/src/pynamodb_utils/parsers.py`

 * *Files identical despite different names*

### Comparing `pynamodb_utils-1.3.0/src/pynamodb_utils/serializers.py` & `pynamodb_utils-1.3.2/src/pynamodb_utils/serializers.py`

 * *Files identical despite different names*

### Comparing `pynamodb_utils-1.3.0/src/pynamodb_utils/utils.py` & `pynamodb_utils-1.3.2/src/pynamodb_utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,21 +75,23 @@
 
 def get_attributes_list(model: Model, depth: int = 0) -> List[str]:
     attrs = []
     for attr_str in model.get_attributes().keys():
         attr = getattr(model, attr_str)
         if isinstance(attr, MapAttribute):
             attrs += [f"{attr_str}.{a}" for a in get_attributes_list(attr, depth=depth+1)]
+        if isinstance(attr, DynamicMapAttribute):
+            attrs.append(f"{attr_str}.*")
         attrs.append(attr_str)
     return attrs
 
 
 def get_available_attributes_list(model: Model, unavaiable_attrs: List[str] = []) -> Set[str]:
-    atts: set = set(get_attributes_list(model))
-    return atts.difference(unavaiable_attrs)
+    attrs: List[str] = get_attributes_list(model)
+    return [attr for attr in attrs if attr not in unavaiable_attrs]
 
 
 def get_attribute(model: Model, attr_string: str) -> Attribute:
     """
     Function gets nested attribute based on path (attr_string)
     """
     attrs = attr_string.split(".")
```

### Comparing `pynamodb_utils-1.3.0/src/pynamodb_utils.egg-info/PKG-INFO` & `pynamodb_utils-1.3.2/src/pynamodb_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamodb-utils
-Version: 1.3.0
+Version: 1.3.2
 Summary: Utilities package for pynamodb.
 Home-page: https://github.com/micmurawski/pynamodb-utils/
 Author: Michal Murawski
 Author-email: mmurawski777@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

