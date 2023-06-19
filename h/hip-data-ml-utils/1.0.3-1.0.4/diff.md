# Comparing `tmp/hip_data_ml_utils-1.0.3.tar.gz` & `tmp/hip_data_ml_utils-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hip_data_ml_utils-1.0.3.tar", max compression
+gzip compressed data, was "hip_data_ml_utils-1.0.4.tar", max compression
```

## Comparing `hip_data_ml_utils-1.0.3.tar` & `hip_data_ml_utils-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1085 2023-03-28 03:51:21.389634 hip_data_ml_utils-1.0.3/LICENSE.txt
--rwxr-xr-x   0        0        0     1580 2023-06-15 03:41:54.867127 hip_data_ml_utils-1.0.3/README.md
--rwxr-xr-x   0        0        0        0 2023-03-30 05:32:20.928557 hip_data_ml_utils-1.0.3/hip_data_ml_utils/core/__init__.py
--rwxr-xr-x   0        0        0      642 2023-05-11 01:34:24.776444 hip_data_ml_utils-1.0.3/hip_data_ml_utils/core/config.py
--rw-r--r--   0        0        0     2158 2023-04-04 23:47:04.268778 hip_data_ml_utils-1.0.3/hip_data_ml_utils/core/databricks_utils.py
--rw-r--r--   0        0        0     3119 2023-04-04 23:47:04.269549 hip_data_ml_utils-1.0.3/hip_data_ml_utils/core/pyathena_utils.py
--rwxr-xr-x   0        0        0        0 2023-03-30 05:32:20.930078 hip_data_ml_utils-1.0.3/hip_data_ml_utils/mlflow_databricks/__init__.py
--rw-r--r--   0        0        0     7529 2023-05-11 01:34:24.777536 hip_data_ml_utils-1.0.3/hip_data_ml_utils/mlflow_databricks/mlflow_model_utils.py
--rw-r--r--   0        0        0     2578 2023-05-11 01:34:24.778338 hip_data_ml_utils-1.0.3/hip_data_ml_utils/mlflow_databricks/mlflow_prediction_requests.py
--rw-r--r--   0        0        0     6370 2023-05-11 01:34:24.779153 hip_data_ml_utils-1.0.3/hip_data_ml_utils/mlflow_databricks/mlflow_serve.py
--rw-r--r--   0        0        0     4470 2023-03-30 05:32:20.932267 hip_data_ml_utils-1.0.3/hip_data_ml_utils/mlflow_databricks/mlflow_tracker.py
--rwxr-xr-x   0        0        0        0 2023-03-30 05:32:20.932369 hip_data_ml_utils-1.0.3/hip_data_ml_utils/pyathena_client/__init__.py
--rw-r--r--   0        0        0     4368 2023-03-30 05:32:20.932900 hip_data_ml_utils-1.0.3/hip_data_ml_utils/pyathena_client/client.py
--rw-r--r--   0        0        0     1267 2023-06-15 01:55:07.851264 hip_data_ml_utils-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3727 1970-01-01 00:00:00.000000 hip_data_ml_utils-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-03-28 03:51:21.389634 hip_data_ml_utils-1.0.4/LICENSE.txt
+-rwxr-xr-x   0        0        0     1581 2023-06-19 00:52:07.912570 hip_data_ml_utils-1.0.4/README.md
+-rwxr-xr-x   0        0        0        0 2023-03-30 05:32:20.928557 hip_data_ml_utils-1.0.4/hip_data_ml_utils/core/__init__.py
+-rwxr-xr-x   0        0        0      642 2023-05-11 01:34:24.776444 hip_data_ml_utils-1.0.4/hip_data_ml_utils/core/config.py
+-rw-r--r--   0        0        0     2158 2023-04-04 23:47:04.268778 hip_data_ml_utils-1.0.4/hip_data_ml_utils/core/databricks_utils.py
+-rw-r--r--   0        0        0     3119 2023-04-04 23:47:04.269549 hip_data_ml_utils-1.0.4/hip_data_ml_utils/core/pyathena_utils.py
+-rwxr-xr-x   0        0        0        0 2023-03-30 05:32:20.930078 hip_data_ml_utils-1.0.4/hip_data_ml_utils/mlflow_databricks/__init__.py
+-rw-r--r--   0        0        0     7529 2023-05-11 01:34:24.777536 hip_data_ml_utils-1.0.4/hip_data_ml_utils/mlflow_databricks/mlflow_model_utils.py
+-rw-r--r--   0        0        0     2578 2023-05-11 01:34:24.778338 hip_data_ml_utils-1.0.4/hip_data_ml_utils/mlflow_databricks/mlflow_prediction_requests.py
+-rw-r--r--   0        0        0     6370 2023-05-11 01:34:24.779153 hip_data_ml_utils-1.0.4/hip_data_ml_utils/mlflow_databricks/mlflow_serve.py
+-rw-r--r--   0        0        0     4515 2023-06-19 00:51:13.412725 hip_data_ml_utils-1.0.4/hip_data_ml_utils/mlflow_databricks/mlflow_tracker.py
+-rwxr-xr-x   0        0        0        0 2023-03-30 05:32:20.932369 hip_data_ml_utils-1.0.4/hip_data_ml_utils/pyathena_client/__init__.py
+-rw-r--r--   0        0        0     4368 2023-03-30 05:32:20.932900 hip_data_ml_utils-1.0.4/hip_data_ml_utils/pyathena_client/client.py
+-rw-r--r--   0        0        0     1267 2023-06-19 00:49:22.247878 hip_data_ml_utils-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3728 1970-01-01 00:00:00.000000 hip_data_ml_utils-1.0.4/PKG-INFO
```

### Comparing `hip_data_ml_utils-1.0.3/LICENSE.txt` & `hip_data_ml_utils-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.3/README.md` & `hip_data_ml_utils-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # data-ml-utils
 A utility python package that covers the common libraries we use.
 
 ## Installation
-This is an open source library hosted on pypi. Run the following command to install the library
+This is an open source library hosted on pypi. Run the following command to install the library.
 ```
 pip install hip-data-ml-utils --upgrade
 ```
 
 ## Documentation
 Head over to https://hip-data-ml-utils.readthedocs.io/en/latest/index.html# to read our library documentation
```

### Comparing `hip_data_ml_utils-1.0.3/hip_data_ml_utils/core/config.py` & `hip_data_ml_utils-1.0.4/hip_data_ml_utils/core/config.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.3/hip_data_ml_utils/core/databricks_utils.py` & `hip_data_ml_utils-1.0.4/hip_data_ml_utils/core/databricks_utils.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.3/hip_data_ml_utils/core/pyathena_utils.py` & `hip_data_ml_utils-1.0.4/hip_data_ml_utils/core/pyathena_utils.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.3/hip_data_ml_utils/mlflow_databricks/mlflow_model_utils.py` & `hip_data_ml_utils-1.0.4/hip_data_ml_utils/mlflow_databricks/mlflow_model_utils.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.3/hip_data_ml_utils/mlflow_databricks/mlflow_prediction_requests.py` & `hip_data_ml_utils-1.0.4/hip_data_ml_utils/mlflow_databricks/mlflow_prediction_requests.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.3/hip_data_ml_utils/mlflow_databricks/mlflow_serve.py` & `hip_data_ml_utils-1.0.4/hip_data_ml_utils/mlflow_databricks/mlflow_serve.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.3/hip_data_ml_utils/mlflow_databricks/mlflow_tracker.py` & `hip_data_ml_utils-1.0.4/hip_data_ml_utils/mlflow_databricks/mlflow_tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         if mlflow.active_run():
             model_func = getattr(mlflow, model_func_dict[type_of_model][0])
             model_func.log_model(
                 **{type_of_model: model, model_func_dict[type_of_model][1]: code_path},
                 registered_model_name=name_of_registered_model,
                 artifact_path=artifact_path,
                 extra_pip_requirements=extra_pip_requirements,
+                await_registration_for=1800,
             )
             return (
                 "model logged"
                 if name_of_registered_model is None
                 else f"model logged and registered as {name_of_registered_model}"
             )
```

### Comparing `hip_data_ml_utils-1.0.3/hip_data_ml_utils/pyathena_client/client.py` & `hip_data_ml_utils-1.0.4/hip_data_ml_utils/pyathena_client/client.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.3/pyproject.toml` & `hip_data_ml_utils-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hip_data_ml_utils"
-version = "1.0.3"
+version = "1.0.4"
 description = "Common Python tools and utilities for Hipages ML work"
 authors = ["Hipages Data Team <datascience@hipagesgroup.com.au>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
```

### Comparing `hip_data_ml_utils-1.0.3/PKG-INFO` & `hip_data_ml_utils-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hip-data-ml-utils
-Version: 1.0.3
+Version: 1.0.4
 Summary: Common Python tools and utilities for Hipages ML work
 License: MIT
 Author: Hipages Data Team
 Author-email: datascience@hipagesgroup.com.au
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -58,15 +58,15 @@
 Requires-Dist: typing-extensions (>=4.2.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # data-ml-utils
 A utility python package that covers the common libraries we use.
 
 ## Installation
-This is an open source library hosted on pypi. Run the following command to install the library
+This is an open source library hosted on pypi. Run the following command to install the library.
 ```
 pip install hip-data-ml-utils --upgrade
 ```
 
 ## Documentation
 Head over to https://hip-data-ml-utils.readthedocs.io/en/latest/index.html# to read our library documentation
```

