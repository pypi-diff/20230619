# Comparing `tmp/airstack-0.0.2.tar.gz` & `tmp/airstack-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airstack-0.0.2.tar", last modified: Fri Jun 16 18:08:22 2023, max compression
+gzip compressed data, was "airstack-0.0.3.tar", last modified: Mon Jun 19 07:46:44 2023, max compression
```

## Comparing `airstack-0.0.2.tar` & `airstack-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 deepeshkn   (501) staff       (20)        0 2023-06-16 18:08:22.440439 airstack-0.0.2/
--rw-r--r--   0 deepeshkn   (501) staff       (20)     3285 2023-06-16 18:08:22.440496 airstack-0.0.2/PKG-INFO
--rw-r--r--   0 deepeshkn   (501) staff       (20)     2785 2023-06-16 18:08:08.000000 airstack-0.0.2/README.md
--rw-r--r--   0 deepeshkn   (501) staff       (20)       85 2023-06-16 17:55:25.000000 airstack-0.0.2/pyproject.toml
--rw-r--r--   0 deepeshkn   (501) staff       (20)      704 2023-06-16 18:08:22.440764 airstack-0.0.2/setup.cfg
-drwxr-xr-x   0 deepeshkn   (501) staff       (20)        0 2023-06-16 18:08:22.438765 airstack-0.0.2/src/
-drwxr-xr-x   0 deepeshkn   (501) staff       (20)        0 2023-06-16 18:08:22.439787 airstack-0.0.2/src/airstack/
--rw-r--r--   0 deepeshkn   (501) staff       (20)        0 2023-06-16 17:55:25.000000 airstack-0.0.2/src/airstack/__init__.py
--rw-r--r--   0 deepeshkn   (501) staff       (20)      308 2023-06-16 17:55:25.000000 airstack-0.0.2/src/airstack/constant.py
--rw-r--r--   0 deepeshkn   (501) staff       (20)     8276 2023-06-16 17:57:10.000000 airstack-0.0.2/src/airstack/execute_query.py
--rw-r--r--   0 deepeshkn   (501) staff       (20)     8894 2023-06-16 17:57:10.000000 airstack-0.0.2/src/airstack/generic.py
--rw-r--r--   0 deepeshkn   (501) staff       (20)     1811 2023-06-16 17:55:25.000000 airstack-0.0.2/src/airstack/send_request.py
-drwxr-xr-x   0 deepeshkn   (501) staff       (20)        0 2023-06-16 18:08:22.440337 airstack-0.0.2/src/airstack.egg-info/
--rw-r--r--   0 deepeshkn   (501) staff       (20)     3285 2023-06-16 18:08:22.000000 airstack-0.0.2/src/airstack.egg-info/PKG-INFO
--rw-r--r--   0 deepeshkn   (501) staff       (20)      346 2023-06-16 18:08:22.000000 airstack-0.0.2/src/airstack.egg-info/SOURCES.txt
--rw-r--r--   0 deepeshkn   (501) staff       (20)        1 2023-06-16 18:08:22.000000 airstack-0.0.2/src/airstack.egg-info/dependency_links.txt
--rw-r--r--   0 deepeshkn   (501) staff       (20)       35 2023-06-16 18:08:22.000000 airstack-0.0.2/src/airstack.egg-info/requires.txt
--rw-r--r--   0 deepeshkn   (501) staff       (20)        9 2023-06-16 18:08:22.000000 airstack-0.0.2/src/airstack.egg-info/top_level.txt
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-19 07:46:44.267694 airstack-0.0.3/
+-rw-r--r--   0 sarvesh    (501) staff       (20)     3285 2023-06-19 07:46:44.267760 airstack-0.0.3/PKG-INFO
+-rw-r--r--   0 sarvesh    (501) staff       (20)     2785 2023-06-19 07:46:20.000000 airstack-0.0.3/README.md
+-rw-r--r--   0 sarvesh    (501) staff       (20)       85 2023-06-09 12:45:46.000000 airstack-0.0.3/pyproject.toml
+-rw-r--r--   0 sarvesh    (501) staff       (20)      704 2023-06-19 07:46:44.268016 airstack-0.0.3/setup.cfg
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-19 07:46:44.265411 airstack-0.0.3/src/
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-19 07:46:44.266708 airstack-0.0.3/src/airstack/
+-rw-r--r--   0 sarvesh    (501) staff       (20)        0 2023-06-09 12:45:46.000000 airstack-0.0.3/src/airstack/__init__.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)      308 2023-06-09 12:45:46.000000 airstack-0.0.3/src/airstack/constant.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     8401 2023-06-19 07:46:20.000000 airstack-0.0.3/src/airstack/execute_query.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     8894 2023-06-19 07:46:20.000000 airstack-0.0.3/src/airstack/generic.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     1811 2023-06-09 12:45:46.000000 airstack-0.0.3/src/airstack/send_request.py
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-19 07:46:44.267540 airstack-0.0.3/src/airstack.egg-info/
+-rw-r--r--   0 sarvesh    (501) staff       (20)     3285 2023-06-19 07:46:44.000000 airstack-0.0.3/src/airstack.egg-info/PKG-INFO
+-rw-r--r--   0 sarvesh    (501) staff       (20)      346 2023-06-19 07:46:44.000000 airstack-0.0.3/src/airstack.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)        1 2023-06-19 07:46:44.000000 airstack-0.0.3/src/airstack.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)       35 2023-06-19 07:46:44.000000 airstack-0.0.3/src/airstack.egg-info/requires.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)        9 2023-06-19 07:46:44.000000 airstack-0.0.3/src/airstack.egg-info/top_level.txt
```

### Comparing `airstack-0.0.2/PKG-INFO` & `airstack-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airstack
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python sdk for airstack apis
 Home-page: https://github.com/Airstack-xyz/airstack-python-sdk
 Author: Airstack
 Author-email: support@airstack.xyz
 Project-URL: Bug Tracker, https://github.com/Airstack-xyz/airstack-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `airstack-0.0.2/README.md` & `airstack-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `airstack-0.0.2/setup.cfg` & `airstack-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = airstack
-version = 0.0.2
+version = 0.0.3
 author = Airstack
 author_email = support@airstack.xyz
 description = Python sdk for airstack apis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Airstack-xyz/airstack-python-sdk
 project_urls =
```

### Comparing `airstack-0.0.2/src/airstack/execute_query.py` & `airstack-0.0.3/src/airstack/execute_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Module: execute_query.py
 Description: This module contains the methods to execute the query.
 """
 
 import json
+import warnings
 import re
 from graphql import parse, print_ast, visit
 from airstack.send_request import SendRequest
 from graphql.language.ast import OperationDefinition
 from airstack.generic import (
     find_page_info,
     add_cursor_to_input_field,
@@ -15,14 +16,15 @@
     has_cursor,
     RemoveQueryByStartingName,
     add_page_info_to_queries,
     remove_unused_variables
 )
 from airstack.constant import AirstackConstants
 
+warnings.filterwarnings("ignore", message="coroutine .* was never awaited")
 
 class QueryResponse:
     """Class for generate the query response
     """
     def __init__(self, response, status_code, error, has_next_page=None, has_prev_page=None,
     get_next_page=None, get_prev_page=None):
         """Init function
@@ -67,18 +69,18 @@
     
     def create_execute_query_object(self, query=None, variables=None):
         # Create a new object using the caller's `self` variables
         execute_query = ExecuteQuery(query=query, variables=variables, url=self.url, api_key=self.api_key, timeout=self.timeout)
         return execute_query
 
 class ExecuteQuery:
-    """_summary_
+    """Class to execute query functions
 
     Returns:
-        _type_: _description_
+        object: object of execute query
     """
     def __init__(self, query=None, variables=None, url=None, api_key=None, timeout=None):
         self.deleted_queries = []
         self.query = query
         self.variables = variables
         self.url = url
         self.api_key = api_key
```

### Comparing `airstack-0.0.2/src/airstack/generic.py` & `airstack-0.0.3/src/airstack/generic.py`

 * *Files identical despite different names*

### Comparing `airstack-0.0.2/src/airstack/send_request.py` & `airstack-0.0.3/src/airstack/send_request.py`

 * *Files identical despite different names*

### Comparing `airstack-0.0.2/src/airstack.egg-info/PKG-INFO` & `airstack-0.0.3/src/airstack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airstack
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python sdk for airstack apis
 Home-page: https://github.com/Airstack-xyz/airstack-python-sdk
 Author: Airstack
 Author-email: support@airstack.xyz
 Project-URL: Bug Tracker, https://github.com/Airstack-xyz/airstack-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

