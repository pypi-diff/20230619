# Comparing `tmp/e2enetworks-0.1.1.tar.gz` & `tmp/e2enetworks-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2enetworks-0.1.1.tar", last modified: Wed Jun 14 13:35:51 2023, max compression
+gzip compressed data, was "e2enetworks-0.1.2.tar", last modified: Mon Jun 19 08:50:01 2023, max compression
```

## Comparing `e2enetworks-0.1.1.tar` & `e2enetworks-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-14 13:35:51.837435 e2enetworks-0.1.1/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)    10786 2023-05-17 07:28:09.000000 e2enetworks-0.1.1/LICENSE.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1160 2023-06-14 13:35:51.837305 e2enetworks-0.1.1/PKG-INFO
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-06-14 10:02:45.000000 e2enetworks-0.1.1/README.rst
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-14 13:35:51.834582 e2enetworks-0.1.1/e2enetworks/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-17 07:28:09.000000 e2enetworks-0.1.1/e2enetworks/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-14 13:35:51.835556 e2enetworks-0.1.1/e2enetworks/cloud/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-17 07:28:09.000000 e2enetworks-0.1.1/e2enetworks/cloud/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-14 13:35:51.835948 e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-14 13:35:51.836081 e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/APIToken/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     3871 2023-06-14 11:34:48.000000 e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/APIToken/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-14 13:35:51.836213 e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/Dataset/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     2949 2023-06-14 11:43:02.000000 e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/Dataset/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-14 13:35:51.836343 e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/EndPoint/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5746 2023-06-14 11:43:02.000000 e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/EndPoint/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-14 13:35:51.836479 e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/Model/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     4955 2023-06-14 11:40:20.000000 e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/Model/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-14 13:35:51.836607 e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/Notebooks/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     7539 2023-06-14 13:33:00.000000 e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/Notebooks/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-14 13:35:51.836739 e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/Project/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     4281 2023-06-14 11:43:02.000000 e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/Project/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-14 13:35:51.836871 e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/Teams/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     3065 2023-06-14 11:55:25.000000 e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/Teams/__init__.py
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1396 2023-06-14 12:47:59.000000 e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/__init__.py
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)       32 2023-05-29 06:58:13.000000 e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/config.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-14 13:35:51.837120 e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/decorators/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-06-14 09:45:49.000000 e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/decorators/__init__.py
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      371 2023-06-14 10:41:32.000000 e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/decorators/validate_access_key_and_token.py
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1704 2023-06-14 11:44:21.000000 e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/init.py
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      147 2023-05-17 07:28:09.000000 e2enetworks-0.1.1/e2enetworks/cloud/test.py
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      216 2023-06-07 11:14:26.000000 e2enetworks-0.1.1/e2enetworks/constants.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-14 13:35:51.835307 e2enetworks-0.1.1/e2enetworks.egg-info/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1160 2023-06-14 13:35:51.000000 e2enetworks-0.1.1/e2enetworks.egg-info/PKG-INFO
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      895 2023-06-14 13:35:51.000000 e2enetworks-0.1.1/e2enetworks.egg-info/SOURCES.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        1 2023-06-14 13:35:51.000000 e2enetworks-0.1.1/e2enetworks.egg-info/dependency_links.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)       25 2023-06-14 13:35:51.000000 e2enetworks-0.1.1/e2enetworks.egg-info/requires.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)       12 2023-06-14 13:35:51.000000 e2enetworks-0.1.1/e2enetworks.egg-info/top_level.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)       38 2023-06-14 13:35:51.837482 e2enetworks-0.1.1/setup.cfg
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1675 2023-06-14 13:35:34.000000 e2enetworks-0.1.1/setup.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-19 08:50:01.192858 e2enetworks-0.1.2/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)    10786 2023-05-17 07:28:09.000000 e2enetworks-0.1.2/LICENSE.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1160 2023-06-19 08:50:01.192692 e2enetworks-0.1.2/PKG-INFO
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-06-14 10:02:45.000000 e2enetworks-0.1.2/README.rst
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-19 08:50:01.187207 e2enetworks-0.1.2/e2enetworks/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-17 07:28:09.000000 e2enetworks-0.1.2/e2enetworks/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-19 08:50:01.188254 e2enetworks-0.1.2/e2enetworks/cloud/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-17 07:28:09.000000 e2enetworks-0.1.2/e2enetworks/cloud/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-19 08:50:01.189782 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-19 08:50:01.190000 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/APIToken/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     3744 2023-06-15 06:17:52.000000 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/APIToken/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-19 08:50:01.190246 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/Dataset/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5014 2023-06-19 07:43:11.000000 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/Dataset/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-19 08:50:01.190540 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/EndPoint/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     4796 2023-06-15 06:18:39.000000 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/EndPoint/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-19 08:50:01.190803 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/Images/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1054 2023-06-19 07:11:21.000000 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/Images/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-19 08:50:01.190976 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/Model/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     4740 2023-06-15 06:17:36.000000 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/Model/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-19 08:50:01.191281 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/Notebooks/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     6642 2023-06-19 07:19:08.000000 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/Notebooks/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-19 08:50:01.191516 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/Project/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     4021 2023-06-19 07:16:26.000000 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/Project/__init__.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1459 2023-06-19 07:16:26.000000 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/Skus.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-19 08:50:01.191689 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/Teams/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     2796 2023-06-15 06:17:36.000000 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/Teams/__init__.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1848 2023-06-19 07:06:57.000000 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/__init__.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)       32 2023-05-29 06:58:13.000000 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/config.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      918 2023-06-19 07:46:43.000000 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/constants.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-19 08:50:01.192241 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/decorators/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-06-14 09:45:49.000000 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/decorators/__init__.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      371 2023-06-14 10:41:32.000000 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/decorators/validate_access_key_and_token.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1743 2023-06-19 07:46:43.000000 e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/init.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      147 2023-05-17 07:28:09.000000 e2enetworks-0.1.2/e2enetworks/cloud/test.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-19 08:50:01.187990 e2enetworks-0.1.2/e2enetworks.egg-info/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1160 2023-06-19 08:50:01.000000 e2enetworks-0.1.2/e2enetworks.egg-info/PKG-INFO
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      997 2023-06-19 08:50:01.000000 e2enetworks-0.1.2/e2enetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        1 2023-06-19 08:50:01.000000 e2enetworks-0.1.2/e2enetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)       25 2023-06-19 08:50:01.000000 e2enetworks-0.1.2/e2enetworks.egg-info/requires.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)       12 2023-06-19 08:50:01.000000 e2enetworks-0.1.2/e2enetworks.egg-info/top_level.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)       38 2023-06-19 08:50:01.192918 e2enetworks-0.1.2/setup.cfg
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1675 2023-06-19 08:49:33.000000 e2enetworks-0.1.2/setup.py
```

### Comparing `e2enetworks-0.1.1/LICENSE.txt` & `e2enetworks-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `e2enetworks-0.1.1/PKG-INFO` & `e2enetworks-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 0.1.1
+Version: 0.1.2
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
```

### Comparing `e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/APIToken/__init__.py` & `e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/APIToken/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 
 import requests
 
 from e2enetworks.cloud.aiplatform import config
-from e2enetworks.constants import BASE_GPU_URL, INDENTATION
+from e2enetworks.cloud.aiplatform.constants import BASE_GPU_URL, INDENTATION
 from e2enetworks.cloud.aiplatform.decorators.validate_access_key_and_token import validate_access_key_and_token
+from e2enetworks.cloud.aiplatform.constants import headers
 
 
 class APITokens:
     def __init__(self, team_id, project_id):
         self.team_id = team_id
         self.project_id = project_id
         self.validate()
@@ -33,39 +34,38 @@
 
         if not status:
             return response
 
         payload = json.dumps({
             "auth_token": auth_token,
         })
+
+        headers['Authorization'] = f'Bearer {config.auth_token}'
+
         url = f"{BASE_GPU_URL}teams/{self.team_id}/auth-token/?apikey={config.apikey}&project_id={self.project_id}"
 
-        headers = {
-            'Content-Type': 'application/json',
-            'Authorization': f'Bearer {config.auth_token}'
-        }
         response = requests.request("POST", url, headers=headers, data=payload)
 
-        print(json.dumps(response.json(), indent=INDENTATION))
+        
 
     @validate_access_key_and_token
     def list(self):
 
         status, response = self.validate()
 
         if not status:
             return response
 
         url = f"{BASE_GPU_URL}teams/{self.team_id}/auth-token/?apikey={config.apikey}&project_id={self.project_id}"
+
         payload = ""
-        headers = {
-            'Authorization': f'Bearer {config.auth_token}'
-        }
+        headers['Authorization'] = f'Bearer {config.auth_token}'
+
         response = requests.request("GET", url, headers=headers, data=payload)
-        print(json.dumps(response.json(), indent=INDENTATION))
+        
 
     @validate_access_key_and_token
     def delete(self, token_id):
 
         status, response = self.validate()
 
         if not status:
@@ -73,36 +73,36 @@
 
         if type(token_id) != int:
             print(f"Token ID - {token_id} Should be Integer")
             return
 
         url = f"{BASE_GPU_URL}teams/{self.team_id}/auth-token/{token_id}/?apikey={config.apikey}&project_id=" \
               f"{self.project_id}"
+
         payload = ""
-        headers = {
-            'Authorization': f'Bearer {config.auth_token}'
-        }
+        headers['Authorization'] = f'Bearer {config.auth_token}'
+
         response = requests.request("DELETE", url, headers=headers, data=payload)
-        print(json.dumps(response.json(), indent=INDENTATION))
+        return response
 
     @staticmethod
     def help():
         print("APITokens Class Help")
-        print("====================")
-        print("This class provides functionalities to manage API tokens.")
-        print("Available methods:")
+        print("\t\t====================")
+        print("\t\tThis class provides functionalities to manage API tokens.")
+        print("\t\tAvailable methods:")
         print(
-            "1. __init__(team_id, project_id): Initializes an APITokens instance with the specified team ID and "
+            "\t\t1. __init__(team_id, project_id): Initializes an APITokens instance with the specified team ID and "
             "project ID.")
-        print("2. create(auth_token): Creates a new API token with the provided authentication token.")
-        print("3. list(): Lists all API tokens associated with the team and project.")
-        print("4. delete(token_id): Deletes an API token with the given token ID.")
-        print("5. clear_values(): Resets the team ID and project ID to None.")
-        print("6. validate(): Checks if the team ID and project ID are of integer type.")
-        print("7. help(): Displays this help message.")
+        print("\t\t2. create(auth_token): Creates a new API token with the provided authentication token.")
+        print("\t\t3. list(): Lists all API tokens associated with the team and project.")
+        print("\t\t4. delete(token_id): Deletes an API token with the given token ID.")
+        print("\t\t5. clear_values(): Resets the team ID and project ID to None.")
+        print("\t\t6. validate(): Checks if the team ID and project ID are of integer type.")
+        print("\t\t7. help(): Displays this help message.")
 
         # Example usages
-        print("\nExample usages:")
-        print("api_tokens = APITokens(123, 456)")
-        print("api_tokens.create('auth_token')")
-        print("api_tokens.list()")
-        print("api_tokens.delete(789)")
+        print("\t\tExample usages:")
+        print("\t\tapi_tokens = APITokens(123, 456)")
+        print("\t\tapi_tokens.create('auth_token')")
+        print("\t\tapi_tokens.list()")
+        print("\t\tapi_tokens.delete(789)")
```

### Comparing `e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/EndPoint/__init__.py` & `e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/EndPoint/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 
 import requests
 
 from e2enetworks.cloud.aiplatform import config
-from e2enetworks.constants import BASE_GPU_URL, INDENTATION
+from e2enetworks.cloud.aiplatform.constants import BASE_GPU_URL, INDENTATION
 from e2enetworks.cloud.aiplatform.decorators.validate_access_key_and_token import validate_access_key_and_token
+from e2enetworks.cloud.aiplatform.constants import headers
 
 
 class EndPoints:
     def __init__(self, team_id, project_id):
         self.team_id = team_id
         self.project_id = project_id
         self.validate()
@@ -37,23 +38,22 @@
         payload = json.dumps({
             "name": name,
             "sku_id": sku_id,
             "prefix": prefix,
             "replica": replica,
             "model_id": model_id
         })
+
         url = f"{BASE_GPU_URL}teams/{self.team_id}/projects/{self.project_id}/serving/inference/" \
               f"?apikey={config.apikey}"
-        headers = {
-            'Content-Type': 'application/json',
-            'Authorization': f'Bearer {config.auth_token}'
-        }
+        headers['Authorization'] = f'Bearer {config.auth_token}'
+
         response = requests.request("POST", url, headers=headers, data=payload)
 
-        print(json.dumps(response.json(), indent=INDENTATION))
+        
 
     @validate_access_key_and_token
     def get(self, endpoint_id):
 
         status, response = self.validate()
 
         if not status:
@@ -61,39 +61,39 @@
 
         if type(endpoint_id) != int:
             print(f"EndPoint ID - {endpoint_id} Should be Integer")
             return
 
         url = f"{BASE_GPU_URL}teams/{self.team_id}/projects/{self.project_id}/serving/inference/{endpoint_id}/?" \
               f"apikey={config.apikey}"
+
         payload = ""
-        headers = {
-            'Authorization': f'Bearer {config.auth_token}'
-        }
+        headers['Authorization'] = f'Bearer {config.auth_token}'
+
         response = requests.request("GET", url, headers=headers, data=payload)
-        print(json.dumps(response.json(), indent=INDENTATION))
-        # return response.json()
+        
+        return response
 
     @validate_access_key_and_token
     def list(self):
 
         status, response = self.validate()
 
         if not status:
             return response
 
         url = f"{BASE_GPU_URL}teams/{self.team_id}/projects/{self.project_id}/serving/inference/" \
               f"?apikey={config.apikey}"
+
         payload = ""
-        headers = {
-            'Authorization': f'Bearer {config.auth_token}'
-        }
+        headers['Authorization'] = f'Bearer {config.auth_token}'
+
         response = requests.request("GET", url, headers=headers, data=payload)
-        print(json.dumps(response.json(), indent=INDENTATION))
-        # return response.json()
+        
+        return response
 
     @validate_access_key_and_token
     def delete(self, endpoint_id):
 
         status, response = self.validate()
 
         if not status:
@@ -101,60 +101,38 @@
 
         if type(endpoint_id) != int:
             print(f"EndPoint ID - {endpoint_id} Should be Integer")
             return
 
         url = f"{BASE_GPU_URL}teams/{self.team_id}/projects/{self.project_id}/serving/inference/{endpoint_id}/" \
               f"?apikey={config.apikey}"
-        payload = ""
-        headers = {
-            'Authorization': f'Bearer {config.auth_token}'
-        }
-        response = requests.request("DELETE", url, headers=headers, data=payload)
-        print(json.dumps(response.json(), indent=INDENTATION))
-        # return response.json()
-
-    @validate_access_key_and_token
-    def logs(self, endpoint_id):
-
-        status, response = self.validate()
 
-        if not status:
-            return response
-
-        if type(endpoint_id) != int:
-            print(f"EndPoint ID - {endpoint_id} Should be Integer")
-            return
-
-        url = f"{BASE_GPU_URL}teams/{self.team_id}/projects/{self.project_id}/serving/inference/{endpoint_id}/logs?" \
-              f"apikey={config.apikey}"
         payload = ""
-        headers = {
-            'Authorization': f'Bearer {config.auth_token}'
-        }
-        response = requests.request("GET", url, headers=headers, data=payload)
-        print(json.dumps(response.json(), indent=INDENTATION))
+        headers['Authorization'] = f'Bearer {config.auth_token}'
+
+        response = requests.request("DELETE", url, headers=headers, data=payload)
+        
+        return response
 
     @staticmethod
     def help():
         print("EndPoint Class Help")
-        print("=================")
-        print("This class provides functionalities to interact with EndPoint.")
-        print("Available methods:")
-        print(
-            "1. __init__(team_id, project_id): Initializes an EndPoints instance with the specified team and "
-            "project IDs.")
-        print("2. create(name, sku_id, prefix, replica, model_id): Creates an endpoint with the provided details.")
-        print("3. get(endpoint_id): Retrieves information about a specific endpoint using its ID.")
-        print("4. list(): Lists all endpoints associated with the team and project.")
-        print("5. delete(endpoint_id): Deletes an endpoint with the given ID.")
-        print("6. clear_values(): Resets the team and project IDs to None.")
-        print("7. validate(): Checks if the team and project IDs are of integer type.")
-        print("8. help(): Displays this help message.")
+        print("\t\t=================")
+        print("\t\tThis class provides functionalities to interact with EndPoint.")
+        print("\t\tAvailable methods:")
+        print("\t\t1. __init__(team_id, project_id): Initializes an EndPoints instance with the specified team and "
+              "project IDs.")
+        print("\t\t2. create(name, sku_id, prefix, replica, model_id): Creates an endpoint with the provided details.")
+        print("\t\t3. get(endpoint_id): Retrieves information about a specific endpoint using its ID.")
+        print("\t\t4. list(): Lists all endpoints associated with the team and project.")
+        print("\t\t5. delete(endpoint_id): Deletes an endpoint with the given ID.")
+        print("\t\t6. clear_values(): Resets the team and project IDs to None.")
+        print("\t\t7. validate(): Checks if the team and project IDs are of integer type.")
+        print("\t\t8. help(): Displays this help message.")
 
         # Example usages
-        print("\nExample usages:")
-        print("endpoints = EndPoints(123, 456)")
-        print("endpoints.create('Name', sku_id, 'Prefix', replica, model_id)")
-        print("endpoints.get(789)")
-        print("endpoints.list()")
-        print("endpoints.delete(789)")
+        print("\t\tExample usages:")
+        print("\t\tendpoints = EndPoints(123, 456)")
+        print("\t\tendpoints.create('Name', sku_id, 'Prefix', replica, model_id)")
+        print("\t\tendpoints.get(789)")
+        print("\t\tendpoints.list()")
+        print("\t\tendpoints.delete(789)")
```

### Comparing `e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/Model/__init__.py` & `e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/Model/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 
 import requests
 
 from e2enetworks.cloud.aiplatform import config
-from e2enetworks.constants import BASE_GPU_URL, INDENTATION
+from e2enetworks.cloud.aiplatform.constants import BASE_GPU_URL, INDENTATION
 from e2enetworks.cloud.aiplatform.decorators.validate_access_key_and_token import validate_access_key_and_token
+from e2enetworks.cloud.aiplatform.constants import headers
 
 
 class Models:
     def __init__(self, team_id, project_id):
         self.team_id = team_id
         self.project_id = project_id
         self.validate()
@@ -36,25 +37,23 @@
 
         payload = json.dumps({
             "name": name,
             "type": bucket_type,
             "bucket_name": bucket_name,
             "model_type": model_type
         })
+
         url = f"{BASE_GPU_URL}teams/{self.team_id}/projects/{self.project_id}/serving/model/" \
               f"?apikey={config.apikey}"
+        headers['Authorization'] = f'Bearer {config.auth_token}'
 
-        headers = {
-            'Content-Type': 'application/json',
-            'Authorization': f'Bearer {config.auth_token}'
-        }
         response = requests.request("POST", url, headers=headers, data=payload)
 
-        print(json.dumps(response.json(), indent=INDENTATION))
-        # return response.json()
+        
+        return response
 
     @validate_access_key_and_token
     def get(self, model_id):
 
         status, response = self.validate()
 
         if not status:
@@ -62,76 +61,78 @@
 
         if type(model_id) != int:
             print(f"Model ID - {model_id} Should be Integer")
             return
 
         url = f"{BASE_GPU_URL}teams/{self.team_id}/projects/{self.project_id}/serving/model/{model_id}" \
               f"?apikey={config.apikey}"
+
         payload = ""
-        headers = {
-            'Authorization': f'Bearer {config.auth_token}'
-        }
+        headers['Authorization'] = f'Bearer {config.auth_token}'
+
         response = requests.request("GET", url, headers=headers, data=payload)
-        print(json.dumps(response.json(), indent=INDENTATION))
-        # return response.json()
+        
+        return response
 
     @validate_access_key_and_token
     def list(self):
 
         status, response = self.validate()
 
         if not status:
             return response
 
         url = f"{BASE_GPU_URL}teams/{self.team_id}/projects/{self.project_id}/serving/model/" \
               f"?apikey={config.apikey}"
+
         payload = ""
-        headers = {
-            'Authorization': f'Bearer {config.auth_token}'
-        }
+        headers['Authorization'] = f'Bearer {config.auth_token}'
+
         response = requests.request("GET", url, headers=headers, data=payload)
-        print(json.dumps(response.json(), indent=INDENTATION))
-        # return response.json()
+        
+        return response
 
     @validate_access_key_and_token
     def delete(self, model_id):
         status, response = self.validate()
 
         if not status:
             return response
 
         if type(model_id) != int:
             return f"Model ID - {model_id} Should be Integer"
 
         url = f"{BASE_GPU_URL}teams/{self.team_id}/projects/{self.project_id}/serving/model/{model_id}/" \
               f"?apikey={config.apikey}"
+
         payload = ""
-        headers = {
-            'Authorization': f'Bearer {config.auth_token}'
-        }
+        headers['Authorization'] = f'Bearer {config.auth_token}'
+
         response = requests.request("DELETE", url, headers=headers, data=payload)
-        print(json.dumps(response.json(), indent=INDENTATION))
-        # return response.json()
+        
+        return response
 
     @staticmethod
     def help():
         print("Models Class Help")
-        print("=================")
-        print("This class provides functionalities to interact with models.")
-        print("Available methods:")
+        print("\t\t=================")
+        print("\t\tThis class provides functionalities to interact with models.")
+        print("\t\tAvailable methods:")
         print(
-            "1. __init__(team_id, project_id): Initializes a Models instance with the specified team and project IDs.")
-        print("2. create(name, bucket_type, bucket_name, model_type): Creates a new model with the provided details.")
-        print("3. get(model_id): Retrieves information about a specific model using its ID.")
-        print("4. list(): Lists all models associated with the team and project.")
-        print("5. delete(model_id): Deletes a model with the given ID.")
-        print("6. clear_values(): Resets the team and project IDs to None.")
-        print("7. validate(): Checks if the team and project IDs are of integer type.")
-        print("8. help(): Displays this help message.")
+            "\t\t1. __init__(team_id, project_id): Initializes a Models instance with the specified team and project "
+            "IDs.")
+        print("\t\t2. create(name, bucket_type, bucket_name, model_type): Creates a new model with the provided "
+              "details.")
+        print("\t\t3. get(model_id): Retrieves information about a specific model using its ID.")
+        print("\t\t4. list(): Lists all models associated with the team and project.")
+        print("\t\t5. delete(model_id): Deletes a model with the given ID.")
+        print("\t\t6. clear_values(): Resets the team and project IDs to None.")
+        print("\t\t7. validate(): Checks if the team and project IDs are of integer type.")
+        print("\t\t8. help(): Displays this help message.")
 
         # Example usages
-        print("\nExample usages:")
-        print("models = Models(123, 456)")
-        print("models.create('Model Name', 'Bucket Type', 'Bucket Name', 'Model Type')")
-        print("models.get(789)")
-        print("models.list()")
-        print("models.delete(789)")
+        print("\t\tExample usages:")
+        print("\t\tmodels = Models(123, 456)")
+        print("\t\tmodels.create('Model Name', 'Bucket Type', 'Bucket Name', 'Model Type')")
+        print("\t\tmodels.get(789)")
+        print("\t\tmodels.list()")
+        print("\t\tmodels.delete(789)")
```

### Comparing `e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/Notebooks/__init__.py` & `e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/Notebooks/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 
 import requests
 
 from e2enetworks.cloud.aiplatform import config
-from e2enetworks.constants import BASE_GPU_URL, INDENTATION
+from e2enetworks.cloud.aiplatform.constants import BASE_GPU_URL, INDENTATION
 from e2enetworks.cloud.aiplatform.decorators.validate_access_key_and_token import validate_access_key_and_token
+from e2enetworks.cloud.aiplatform.constants import headers
 
 
 class Notebooks:
     def __init__(self, team_id, project_id):
         self.team_id = team_id
         self.project_id = project_id
         self.validate()
@@ -35,23 +36,19 @@
 
         payload = json.dumps({
             "name": name,
             "image_id": image_id,
             "sku_id": sku_id,
             "instance_type": instance_type
         })
+        headers['Authorization'] = f'Bearer {config.auth_token}'
         url = f"{BASE_GPU_URL}teams/{self.team_id}/projects/{self.project_id}/notebooks/" \
               f"?apikey={config.apikey}"
-        headers = {
-            'Content-Type': 'application/json',
-            'Authorization': f'Bearer {config.auth_token}'
-        }
-        response = requests.request("POST", url, headers=headers, data=payload)
 
-        print(json.dumps(response.json(), indent=INDENTATION))
+        return requests.request("POST", url, headers=headers, data=payload)
 
     @validate_access_key_and_token
     def get(self, notebook_id):
 
         status, response = self.validate()
 
         if not status:
@@ -59,39 +56,36 @@
 
         if type(notebook_id) != int:
             print(f"Notebook ID - {notebook_id} Should be Integer")
             return
 
         url = f"{BASE_GPU_URL}teams/{self.team_id}/projects/{self.project_id}/notebooks/{notebook_id}/?" \
               f"apikey={config.apikey}"
+
         payload = ""
-        headers = {
-            'Authorization': f'Bearer {config.auth_token}'
-        }
+        headers['Authorization'] = f'Bearer {config.auth_token}'
+
         response = requests.request("GET", url, headers=headers, data=payload)
-        print(json.dumps(response.json(), indent=INDENTATION))
-        # return response.json()
+        
+        return response
 
     @validate_access_key_and_token
     def list(self):
 
         status, response = self.validate()
 
         if not status:
             return response
 
         url = f"{BASE_GPU_URL}teams/{self.team_id}/projects/{self.project_id}/notebooks/" \
               f"?apikey={config.apikey}"
         payload = ""
-        headers = {
-            'Authorization': f'Bearer {config.auth_token}'
-        }
         response = requests.request("GET", url, headers=headers, data=payload)
-        print(json.dumps(response.json(), indent=INDENTATION))
-        # return response.json()
+        
+        return response
 
     @validate_access_key_and_token
     def delete(self, notebook_id):
 
         status, response = self.validate()
 
         if not status:
@@ -99,21 +93,21 @@
 
         if type(notebook_id) != int:
             print(f"Notebook ID - {notebook_id} Should be Integer")
             return
 
         url = f"{BASE_GPU_URL}teams/{self.team_id}/projects/{self.project_id}/notebooks/{notebook_id}/?" \
               f"apikey={config.apikey}"
+
         payload = ""
-        headers = {
-            'Authorization': f'Bearer {config.auth_token}'
-        }
+        headers['Authorization'] = f'Bearer {config.auth_token}'
+
         response = requests.request("DELETE", url, headers=headers, data=payload)
-        print(json.dumps(response.json(), indent=INDENTATION))
-        # return response.json()
+        
+        return response
 
     @validate_access_key_and_token
     def stop(self, notebook_id):
 
         status, response = self.validate()
 
         if not status:
@@ -121,21 +115,21 @@
 
         if type(notebook_id) != int:
             print(f"Notebook ID - {notebook_id} Should be Integer")
             return
 
         url = f"{BASE_GPU_URL}teams/{self.team_id}/projects/{self.project_id}/notebooks/{notebook_id}/actions/" \
               f"?action=stop&apikey={config.apikey}"
+
         payload = ""
-        headers = {
-            'Authorization': f'Bearer {config.auth_token}'
-        }
+        headers['Authorization'] = f'Bearer {config.auth_token}'
+
         response = requests.request("PUT", url, headers=headers, data=payload)
-        print(json.dumps(response.json(), indent=INDENTATION))
-        # return response.json()
+        
+        return response
 
     @validate_access_key_and_token
     def start(self, notebook_id):
 
         status, response = self.validate()
 
         if not status:
@@ -143,21 +137,21 @@
 
         if type(notebook_id) != int:
             print(f"Notebook ID - {notebook_id} Should be Integer")
             return
 
         url = f"{BASE_GPU_URL}teams/{self.team_id}/projects/{self.project_id}/notebooks/{notebook_id}/actions/" \
               f"?action=start&apikey={config.apikey}"
+
         payload = ""
-        headers = {
-            'Authorization': f'Bearer {config.auth_token}'
-        }
+        headers['Authorization'] = f'Bearer {config.auth_token}'
+
         response = requests.request("PUT", url, headers=headers, data=payload)
-        print(json.dumps(response.json(), indent=INDENTATION))
-        # return response.json()
+        
+        return response
 
     def upgrade(self, notebook_id, size):
         status, response = self.validate()
 
         if not status:
             return response
 
@@ -167,33 +161,28 @@
 
         if type(size) != int:
             print(f"Size - {size} Should be Integer")
             return
 
         url = f"{BASE_GPU_URL}teams/{self.team_id}/projects/{self.project_id}/notebooks/{notebook_id}/pvc/" \
               f"upgrade/?apikey={config.apikey}"
+
         payload = json.dumps({
             "size": size
         })
-        headers = {
-            'Authorization': f'Bearer {config.auth_token}',
-            'Connection': 'keep-alive',
-            'Content-Type': 'application/json',
-            'Origin': 'https://gpu-notebooks.e2enetworks.com',
-            'Referer': 'https://gpu-notebooks.e2enetworks.com/',
-            'Sec-Fetch-Dest': 'empty',
-            'Sec-Fetch-Mode': 'cors',
-            'Sec-Fetch-Site': 'same-site',
-        }
+        headers['Authorization'] = f'Bearer {config.auth_token}'
+
         response = requests.request("PUT", url, headers=headers, data=payload)
-        print(json.dumps(response.json(), indent=INDENTATION))
-        # return response.json()
+        
+        return response
 
     @staticmethod
     def help():
+        print("\t\tNotebook Class Help")
+        print("\t\t=================")
         help_text = """
                 Notebooks class provides methods to interact with notebooks in a project.
 
                 Available methods:
                 1. create(name, sku_id, image_id, instance_type): Create a new notebook.
                 2. get(notebook_id): Get information about a notebook.
                 3. list(): List all notebooks in the project.
```

### Comparing `e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/Teams/__init__.py` & `e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/Teams/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,86 @@
 import json
 
 import requests
 
 from e2enetworks.cloud.aiplatform import config
-from e2enetworks.constants import BASE_GPU_URL, INDENTATION
+from e2enetworks.cloud.aiplatform.constants import BASE_GPU_URL, INDENTATION
 from e2enetworks.cloud.aiplatform.decorators.validate_access_key_and_token import validate_access_key_and_token
+from e2enetworks.cloud.aiplatform.constants import headers
 
 
 class Teams:
     @validate_access_key_and_token
     def create(self, team_name):
         payload = json.dumps({
             "team_name": team_name,
         })
         url = f"{BASE_GPU_URL}teams/?apikey={config.apikey}"
 
-        headers = {
-            'Content-Type': 'application/json',
-            'Authorization': f'Bearer {config.auth_token}'
-        }
+        headers['Authorization'] = f'Bearer {config.auth_token}'
+
         response = requests.request("POST", url, headers=headers, data=payload)
 
-        print(json.dumps(response.json(), indent=INDENTATION))
-        # return response.json()
+        
+        return response
 
     @validate_access_key_and_token
     def get(self, team_id):
 
         if type(team_id) != int:
             print(f"Team ID - {team_id} Should be Integer")
             return
 
         url = f"{BASE_GPU_URL}teams/{team_id}/?apikey={config.apikey}"
+
         payload = ""
-        headers = {
-            'Authorization': f'Bearer {config.auth_token}'
-        }
+
+        headers['Authorization'] = f'Bearer {config.auth_token}'
 
         response = requests.request("GET", url, headers=headers, data=payload)
-        print(json.dumps(response.json(), indent=INDENTATION))
-        # return response.json()
+        
+        return response
 
     @validate_access_key_and_token
     def list(self):
         url = f"{BASE_GPU_URL}teams/?apikey={config.apikey}"
         payload = ""
-        headers = {
-            'Authorization': f'Bearer {config.auth_token}'
-        }
+
+        headers['Authorization'] = f'Bearer {config.auth_token}'
+
         response = requests.request("GET", url, headers=headers, data=payload)
-        print(json.dumps(response.json(), indent=INDENTATION))
-        # return response.json()
+        return response
 
     @validate_access_key_and_token
     def delete(self, team_id):
 
         if type(team_id) != int:
             print(f"Team ID - {team_id} Should be Integer")
             return
 
         url = f"{BASE_GPU_URL}teams/{team_id}/?apikey={config.apikey}"
         payload = ""
-        headers = {
-            'Authorization': f'Bearer {config.auth_token}'
-        }
+
+        headers['Authorization'] = f'Bearer {config.auth_token}'
         response = requests.request("DELETE", url, headers=headers, data=payload)
-        print(json.dumps(response.json(), indent=INDENTATION))
-        # return response.json()
+        
+        return response
 
     @staticmethod
     def help():
         print("Teams Class Help")
-        print("================")
-        print("This class provides functionalities to interact with teams.")
-        print("Available methods:")
-        print("1. create(team_name): Creates a new team with the provided team name.")
-        print("2. get(team_id): Retrieves information about a specific team using its ID.")
-        print("3. list(): Lists all teams.")
-        print("4. delete(team_id): Deletes a team with the given ID.")
-        print("5. help(): Displays this help message.")
+        print("\t\t================")
+        print("\t\tThis class provides functionalities to interact with teams.")
+        print("\t\tAvailable methods:")
+        print("\t\t1. create(team_name): Creates a new team with the provided team name.")
+        print("\t\t2. get(team_id): Retrieves information about a specific team using its ID.")
+        print("\t\t3. list(): Lists all teams.")
+        print("\t\t4. delete(team_id): Deletes a team with the given ID.")
+        print("\t\t5. help(): Displays this help message.")
 
         # Example usages
-        print("\nExample usages:")
-        print("teams = Teams()")
-        print("teams.create('Team Name')")
-        print("teams.get(123)")
-        print("teams.list()")
-        print("teams.delete(123)")
+        print("\t\tExample usages:")
+        print("\t\tteams = Teams()")
+        print("\t\tteams.create('Team Name')")
+        print("\t\tteams.get(123)")
+        print("\t\tteams.list()")
+        print("\t\tteams.delete(123)")
```

### Comparing `e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/__init__.py` & `e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,44 @@
+import json
+from e2enetworks.cloud.aiplatform.init import init
+from e2enetworks.cloud.aiplatform.Images import Images
+from e2enetworks.cloud.aiplatform.Skus import Skus
 from e2enetworks.cloud.aiplatform.Notebooks import Notebooks
 from e2enetworks.cloud.aiplatform.Dataset import Datasets
 from e2enetworks.cloud.aiplatform.EndPoint import EndPoints
-from e2enetworks.cloud.aiplatform.init import init
 from e2enetworks.cloud.aiplatform.Model import Models
 from e2enetworks.cloud.aiplatform.Project import Projects
 from e2enetworks.cloud.aiplatform.Teams import Teams
 from e2enetworks.cloud.aiplatform.APIToken import APITokens
 
 
 def help():
-    print("AIPlatform Help")
-    print("=================")
-    print("Available classes:")
-    print("- Datasets: Provides functionalities to interact with datasets.")
-    print("- EndPoints: Provides functionalities to interact with endpoints.")
-    print("- Init: Provides functionalities for initialization.")
-    print("- Models: Provides functionalities to interact with models.")
-    print("- Projects: Provides functionalities to interact with projects.")
-    print("- Teams: Provides functionalities to interact with teams.")
-    print("- APITokens: Provides functionalities to interact with API tokens.")
+    print("\t\tAIPlatform Help")
+    print("\t\t=================")
+    print("\t\tAvailable classes:")
+    print("\t\t- init: Provides functionalities for initialization.")
+    print("\t\t- Images: Provides functionalities to interact with images.")
+    print("\t\t- Skus: Provides functionalities to interact with skus.")
+    print("\t\t- Notebooks: Provides functionalities to interact with notebooks.")
+    print("\t\t- Datasets: Provides functionalities to interact with datasets.")
+    print("\t\t- EndPoints: Provides functionalities to interact with endpoints.")
+    print("\t\t- Models: Provides functionalities to interact with models.")
+    print("\t\t- Projects: Provides functionalities to interact with projects.")
+    print("\t\t- Teams: Provides functionalities to interact with teams.")
+    print("\t\t- APITokens: Provides functionalities to interact with API tokens.")
+    print("\t\t- beautify: beautify and print the specific response")
 
     # Call help() method on each class
-    Datasets(team_id=1, project_id=2).help()
-    EndPoints(team_id=1, project_id=2).help()
-    init(auth_token="", apikey="").help()
-    Models(team_id=1, project_id=2).help()
-    Projects(team_id=1).help()
-    Teams().help()
-    APITokens(team_id=1, project_id=2).help()
+    init.help()
+    Images.help()
+    Skus.help()
+    Notebooks.help()
+    Datasets.help()
+    EndPoints.help()
+    Models.help()
+    Projects.help()
+    Teams.help()
+    APITokens.help()
+
+
+def beautify(response):
+    print(json.dumps(response.json(), indent=5))
```

### Comparing `e2enetworks-0.1.1/e2enetworks/cloud/aiplatform/init.py` & `e2enetworks-0.1.2/e2enetworks/cloud/aiplatform/init.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 
 import requests
 
 from e2enetworks.cloud.aiplatform import config
-from e2enetworks.constants import (BASE_GPU_URL, INDENTATION, STATUS_CODE,
-                                   VALIDATED_SUCCESSFULLY)
+from e2enetworks.cloud.aiplatform.constants import (BASE_GPU_URL, STATUS_CODE,
+                                                    VALIDATED_SUCCESSFULLY, INVALID_CREDENTIALS)
 
 
 class init:
     def __init__(self, auth_token, apikey):
         config.apikey = apikey
         config.auth_token = auth_token
         self.validate(auth_token, apikey)
@@ -19,30 +19,29 @@
         headers = {
             'Authorization': f'Bearer {auth_token}'
         }
         response = requests.request("GET", url, headers=headers, data=payload)
         if response.status_code == STATUS_CODE:
             print(VALIDATED_SUCCESSFULLY)
         else:
+            print(INVALID_CREDENTIALS)
             self.clear_values()
-            print(json.dumps(response.json(), indent=INDENTATION))
 
     def clear_values(self):
         config.apikey = None
         config.auth_token = None
 
     @staticmethod
     def help():
         print("Init Class Help")
-        print("=================")
-        print("This class provides functionalities for initialization.")
-        print("Available methods:")
-        print(
-            "1. __init__(auth_token, apikey): Initializes an Init instance with the provided authentication token and "
-            "API key.")
-        print("2. validate(auth_token, apikey): Validates the provided authentication token and API key.")
-        print("3. clear_values(): Resets the API key and authentication token to None.")
-        print("4. help(): Displays this help message.")
+        print("\t\t=================")
+        print("\t\tThis class provides functionalities for initialization.")
+        print("\t\tAvailable methods:")
+        print("\t\t1. __init__(auth_token, apikey): Initializes an Init instance with the provided authentication"
+              " token and API key.")
+        print("\t\t2. validate(auth_token, apikey): Validates the provided authentication token and API key.")
+        print("\t\t3. clear_values(): Resets the API key and authentication token to None.")
+        print("\t\t4. help(): Displays this help message.")
 
         # Example usage
-        print("\nExample usage:")
-        print("init = init('Auth Token', 'API Key')")
+        print("\t\t\nExample usage:")
+        print("\t\tinit = init('Auth Token', 'API Key')")
```

### Comparing `e2enetworks-0.1.1/e2enetworks.egg-info/PKG-INFO` & `e2enetworks-0.1.2/e2enetworks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 0.1.1
+Version: 0.1.2
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
```

### Comparing `e2enetworks-0.1.1/e2enetworks.egg-info/SOURCES.txt` & `e2enetworks-0.1.2/e2enetworks.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 LICENSE.txt
 README.rst
 setup.py
 e2enetworks/__init__.py
-e2enetworks/constants.py
 e2enetworks.egg-info/PKG-INFO
 e2enetworks.egg-info/SOURCES.txt
 e2enetworks.egg-info/dependency_links.txt
 e2enetworks.egg-info/requires.txt
 e2enetworks.egg-info/top_level.txt
 e2enetworks/cloud/__init__.py
 e2enetworks/cloud/test.py
+e2enetworks/cloud/aiplatform/Skus.py
 e2enetworks/cloud/aiplatform/__init__.py
 e2enetworks/cloud/aiplatform/config.py
+e2enetworks/cloud/aiplatform/constants.py
 e2enetworks/cloud/aiplatform/init.py
 e2enetworks/cloud/aiplatform/APIToken/__init__.py
 e2enetworks/cloud/aiplatform/Dataset/__init__.py
 e2enetworks/cloud/aiplatform/EndPoint/__init__.py
+e2enetworks/cloud/aiplatform/Images/__init__.py
 e2enetworks/cloud/aiplatform/Model/__init__.py
 e2enetworks/cloud/aiplatform/Notebooks/__init__.py
 e2enetworks/cloud/aiplatform/Project/__init__.py
 e2enetworks/cloud/aiplatform/Teams/__init__.py
 e2enetworks/cloud/aiplatform/decorators/__init__.py
 e2enetworks/cloud/aiplatform/decorators/validate_access_key_and_token.py
```

### Comparing `e2enetworks-0.1.1/setup.py` & `e2enetworks-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 from os import path
 
-version = "0.1.1"
+version = "0.1.2"
 install_requires = [
     "requests",
     "urllib3==1.26.6",
 ]
 # read the contents of your README file
 
 this_directory = path.abspath(path.dirname(__file__))
```

