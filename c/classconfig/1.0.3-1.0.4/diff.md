# Comparing `tmp/classconfig-1.0.3.tar.gz` & `tmp/classconfig-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classconfig-1.0.3.tar", last modified: Thu May 11 12:40:41 2023, max compression
+gzip compressed data, was "classconfig-1.0.4.tar", last modified: Mon Jun 19 14:23:47 2023, max compression
```

## Comparing `classconfig-1.0.3.tar` & `classconfig-1.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-05-11 12:40:41.205677 classconfig-1.0.3/
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1211 2022-05-31 11:17:31.000000 classconfig-1.0.3/LICENSE
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       24 2023-04-27 11:55:37.000000 classconfig-1.0.3/MANIFEST.in
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3771 2023-05-11 12:40:41.205677 classconfig-1.0.3/PKG-INFO
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3321 2023-05-04 05:03:52.000000 classconfig-1.0.3/README.md
-drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-05-11 12:40:41.201677 classconfig-1.0.3/classconfig/
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      111 2023-04-26 13:54:46.000000 classconfig-1.0.3/classconfig/__init__.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2845 2023-04-26 14:19:24.000000 classconfig-1.0.3/classconfig/base.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2527 2023-05-11 12:12:31.000000 classconfig-1.0.3/classconfig/classes.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)    40390 2023-05-11 12:36:30.000000 classconfig-1.0.3/classconfig/configurable.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     7128 2023-04-27 11:23:40.000000 classconfig-1.0.3/classconfig/transforms.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     9236 2023-04-27 10:56:32.000000 classconfig-1.0.3/classconfig/validators.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      382 2023-04-26 15:16:39.000000 classconfig-1.0.3/classconfig/yaml.py
-drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-05-11 12:40:41.201677 classconfig-1.0.3/classconfig.egg-info/
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3771 2023-05-11 12:40:41.000000 classconfig-1.0.3/classconfig.egg-info/PKG-INFO
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      516 2023-05-11 12:40:41.000000 classconfig-1.0.3/classconfig.egg-info/SOURCES.txt
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)        1 2023-05-11 12:40:41.000000 classconfig-1.0.3/classconfig.egg-info/dependency_links.txt
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       21 2023-05-11 12:40:41.000000 classconfig-1.0.3/classconfig.egg-info/requires.txt
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       12 2023-05-11 12:40:41.000000 classconfig-1.0.3/classconfig.egg-info/top_level.txt
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       20 2023-04-26 13:45:04.000000 classconfig-1.0.3/requirements.txt
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       38 2023-05-11 12:40:41.205677 classconfig-1.0.3/setup.cfg
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1115 2023-05-11 12:39:58.000000 classconfig-1.0.3/setup.py
-drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-05-11 12:40:41.205677 classconfig-1.0.3/tests/
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2626 2023-04-27 11:14:46.000000 classconfig-1.0.3/tests/test_classes.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)    25594 2023-05-11 12:36:30.000000 classconfig-1.0.3/tests/test_configurable.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1948 2023-04-27 10:43:21.000000 classconfig-1.0.3/tests/test_readme.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2521 2023-04-27 11:32:32.000000 classconfig-1.0.3/tests/test_transforms.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     5872 2023-04-27 11:12:58.000000 classconfig-1.0.3/tests/test_validators.py
+drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-06-19 14:23:47.355648 classconfig-1.0.4/
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1211 2022-05-31 11:17:31.000000 classconfig-1.0.4/LICENSE
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       24 2023-04-27 11:55:37.000000 classconfig-1.0.4/MANIFEST.in
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3771 2023-06-19 14:23:47.355648 classconfig-1.0.4/PKG-INFO
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3321 2023-05-04 05:03:52.000000 classconfig-1.0.4/README.md
+drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-06-19 14:23:47.351648 classconfig-1.0.4/classconfig/
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      111 2023-04-26 13:54:46.000000 classconfig-1.0.4/classconfig/__init__.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2845 2023-04-26 14:19:24.000000 classconfig-1.0.4/classconfig/base.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2527 2023-05-11 12:12:31.000000 classconfig-1.0.4/classconfig/classes.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)    40433 2023-06-19 14:22:56.000000 classconfig-1.0.4/classconfig/configurable.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     7128 2023-04-27 11:23:40.000000 classconfig-1.0.4/classconfig/transforms.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     9236 2023-04-27 10:56:32.000000 classconfig-1.0.4/classconfig/validators.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      382 2023-04-26 15:16:39.000000 classconfig-1.0.4/classconfig/yaml.py
+drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-06-19 14:23:47.351648 classconfig-1.0.4/classconfig.egg-info/
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3771 2023-06-19 14:23:47.000000 classconfig-1.0.4/classconfig.egg-info/PKG-INFO
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      516 2023-06-19 14:23:47.000000 classconfig-1.0.4/classconfig.egg-info/SOURCES.txt
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)        1 2023-06-19 14:23:47.000000 classconfig-1.0.4/classconfig.egg-info/dependency_links.txt
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       21 2023-06-19 14:23:47.000000 classconfig-1.0.4/classconfig.egg-info/requires.txt
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       12 2023-06-19 14:23:47.000000 classconfig-1.0.4/classconfig.egg-info/top_level.txt
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       20 2023-04-26 13:45:04.000000 classconfig-1.0.4/requirements.txt
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       38 2023-06-19 14:23:47.355648 classconfig-1.0.4/setup.cfg
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1115 2023-06-19 14:23:02.000000 classconfig-1.0.4/setup.py
+drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-06-19 14:23:47.355648 classconfig-1.0.4/tests/
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2626 2023-04-27 11:14:46.000000 classconfig-1.0.4/tests/test_classes.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)    25594 2023-05-11 12:36:30.000000 classconfig-1.0.4/tests/test_configurable.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1948 2023-04-27 10:43:21.000000 classconfig-1.0.4/tests/test_readme.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2521 2023-04-27 11:32:32.000000 classconfig-1.0.4/tests/test_transforms.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     5872 2023-04-27 11:12:58.000000 classconfig-1.0.4/tests/test_validators.py
```

### Comparing `classconfig-1.0.3/LICENSE` & `classconfig-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.3/PKG-INFO` & `classconfig-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classconfig
-Version: 1.0.3
+Version: 1.0.4
 Summary: Package for creating configuration files automatically and loading objects from those configuration files.
 Home-page: https://github.com/mdocekal/classconfig
 Author: Martin Dočekal
 Keywords: configuration,auto config,config,configurable,configurable class,configurable object,configurable attribute
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `classconfig-1.0.3/README.md` & `classconfig-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.3/classconfig/base.py` & `classconfig-1.0.4/classconfig/base.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.3/classconfig/classes.py` & `classconfig-1.0.4/classconfig/classes.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.3/classconfig/configurable.py` & `classconfig-1.0.4/classconfig/configurable.py`

 * *Files 0% similar despite different names*

```diff
@@ -704,16 +704,16 @@
                     if hasattr(var.type, "__args__") and len(var.type.__args__) == 1:
                         call_with["type"] = var.type.__args__[0]
 
                     call_with["nargs"] = "+"
                 elif var.type in [str, int, float, bool]:
                     call_with["type"] = var.type
                 else:
-                    # unsupported type
-                    continue
+                    # it is expected that type will be transformed
+                    call_with["type"] = str
 
                 parser.add_argument("--" + var_name, **call_with)
 
         return parser
 
     def get_values_from_arguments(self) -> Dict[str, str]:
         """
```

### Comparing `classconfig-1.0.3/classconfig/transforms.py` & `classconfig-1.0.4/classconfig/transforms.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.3/classconfig/validators.py` & `classconfig-1.0.4/classconfig/validators.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.3/classconfig.egg-info/PKG-INFO` & `classconfig-1.0.4/classconfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classconfig
-Version: 1.0.3
+Version: 1.0.4
 Summary: Package for creating configuration files automatically and loading objects from those configuration files.
 Home-page: https://github.com/mdocekal/classconfig
 Author: Martin Dočekal
 Keywords: configuration,auto config,config,configurable,configurable class,configurable object,configurable attribute
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `classconfig-1.0.3/classconfig.egg-info/SOURCES.txt` & `classconfig-1.0.4/classconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.3/setup.py` & `classconfig-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 with open("requirements.txt") as f:
     REQUIREMENTS = [line.strip() for line in f if is_requirement(line)]
 
 
 setup_args = dict(
     name='classconfig',
-    version='1.0.3',
+    version='1.0.4',
     description='Package for creating configuration files automatically and loading objects from those configuration files.',
     long_description_content_type="text/markdown",
     long_description=README,
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     author='Martin Dočekal',
     keywords=['configuration', 'auto config', 'config', 'configurable', 'configurable class', 'configurable object',
               'configurable attribute'],
```

### Comparing `classconfig-1.0.3/tests/test_classes.py` & `classconfig-1.0.4/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.3/tests/test_configurable.py` & `classconfig-1.0.4/tests/test_configurable.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.3/tests/test_readme.py` & `classconfig-1.0.4/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.3/tests/test_transforms.py` & `classconfig-1.0.4/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.3/tests/test_validators.py` & `classconfig-1.0.4/tests/test_validators.py`

 * *Files identical despite different names*

