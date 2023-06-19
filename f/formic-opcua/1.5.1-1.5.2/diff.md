# Comparing `tmp/formic_opcua-1.5.1.tar.gz` & `tmp/formic_opcua-1.5.2.tar.gz`

## Comparing `formic_opcua-1.5.1.tar` & `formic_opcua-1.5.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/README.md
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/examples/opcua_client.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/examples/example_configs/opcua_config.yaml
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/examples/example_configs/opcua_config_1.yaml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/examples/example_configs/opcua_config_2.yaml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/examples/example_configs/opcua_config_3.yaml
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/examples/example_configs/opcua_config_4.yaml
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/examples/example_configs/opcua_config_5.yaml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/formic_opcua/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/formic_opcua/client/__init__.py
--rw-r--r--   0        0        0    12239 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/formic_opcua/client/async_opcua_client.py
--rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/formic_opcua/client/opcua_client.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/formic_opcua/core/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/formic_opcua/core/exceptions.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/formic_opcua/core/parse.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/formic_opcua/core/type_conversions.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/formic_opcua/scripts/__init__.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/formic_opcua/scripts/formic_opcua_client.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/formic_opcua/scripts/formic_opcua_server.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/formic_opcua/server/__init__.py
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/formic_opcua/server/opcua_server.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/hooks/add_issue_prefix.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/tests/__init__.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/tests/test_server_config.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/pyproject.toml
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 formic_opcua-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/README.md
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/examples/opcua_client.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/examples/example_configs/opcua_config.yaml
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/examples/example_configs/opcua_config_1.yaml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/examples/example_configs/opcua_config_2.yaml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/examples/example_configs/opcua_config_3.yaml
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/examples/example_configs/opcua_config_4.yaml
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/examples/example_configs/opcua_config_5.yaml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/client/__init__.py
+-rw-r--r--   0        0        0    12239 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/client/async_opcua_client.py
+-rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/client/opcua_client.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/core/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/core/exceptions.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/core/parse.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/core/type_conversions.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/scripts/__init__.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/scripts/formic_opcua_client.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/scripts/formic_opcua_server.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/server/__init__.py
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/server/opcua_server.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/hooks/add_issue_prefix.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/tests/__init__.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/tests/test_server_config.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/PKG-INFO
```

### Comparing `formic_opcua-1.5.1/.pre-commit-config.yaml` & `formic_opcua-1.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.1/examples/opcua_client.py` & `formic_opcua-1.5.2/examples/opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.1/examples/example_configs/opcua_config.yaml` & `formic_opcua-1.5.2/examples/example_configs/opcua_config.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.1/examples/example_configs/opcua_config_1.yaml` & `formic_opcua-1.5.2/examples/example_configs/opcua_config_1.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.1/examples/example_configs/opcua_config_2.yaml` & `formic_opcua-1.5.2/examples/example_configs/opcua_config_2.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.1/formic_opcua/client/async_opcua_client.py` & `formic_opcua-1.5.2/formic_opcua/client/async_opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.1/formic_opcua/client/opcua_client.py` & `formic_opcua-1.5.2/formic_opcua/client/opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.1/formic_opcua/core/parse.py` & `formic_opcua-1.5.2/formic_opcua/core/parse.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.1/formic_opcua/core/type_conversions.py` & `formic_opcua-1.5.2/formic_opcua/core/type_conversions.py`

 * *Files 18% similar despite different names*

```diff
@@ -39,11 +39,15 @@
     VariantType.String: str,
     VariantType.DateTime: datetime,
     VariantType.Guid: uuid.UUID,
 }
 
 
 def convert_type(value, var_type):
-    if (type_map[var_type] == int or type_map[var_type] == float) and isinstance(value, str):
-        value = positive_sha256_hash(value)
+    if isinstance(value, list):
+        mapped_value = [type_map[var_type](element) for element in value]
+    elif (type_map[var_type] == int or type_map[var_type] == float) and isinstance(value, str):
+        mapped_value = type_map[var_type](positive_sha256_hash(value))
+    else:
+        mapped_value = type_map[var_type](value)
 
-    return type_map[var_type](value)
+    return mapped_value
```

### Comparing `formic_opcua-1.5.1/formic_opcua/scripts/formic_opcua_client.py` & `formic_opcua-1.5.2/formic_opcua/scripts/formic_opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.1/formic_opcua/scripts/formic_opcua_server.py` & `formic_opcua-1.5.2/formic_opcua/scripts/formic_opcua_server.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.1/formic_opcua/server/opcua_server.py` & `formic_opcua-1.5.2/formic_opcua/server/opcua_server.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.1/hooks/add_issue_prefix.py` & `formic_opcua-1.5.2/hooks/add_issue_prefix.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.1/tests/test_server_config.py` & `formic_opcua-1.5.2/tests/test_server_config.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.1/.gitignore` & `formic_opcua-1.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.1/pyproject.toml` & `formic_opcua-1.5.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ['hatchling']
 build-backend = 'hatchling.build'
 
 [project]
 name = 'formic_opcua'
 requires-python = ">=3.8"
-version = "1.5.1"
+version = "1.5.2"
 authors = [
     {name = "Spencer White", email = "swhite@formic.co"},
     {name = "Damian Stempel"},
     {name = "Viachaslau Zakharchuk"}
 
 ]
 dependencies = [
```

