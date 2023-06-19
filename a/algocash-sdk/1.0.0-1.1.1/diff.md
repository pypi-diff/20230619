# Comparing `tmp/algocash-sdk-1.0.0.tar.gz` & `tmp/algocash-sdk-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algocash-sdk-1.0.0.tar", last modified: Fri May 19 01:47:04 2023, max compression
+gzip compressed data, was "algocash-sdk-1.1.1.tar", last modified: Mon Jun 19 19:04:21 2023, max compression
```

## Comparing `algocash-sdk-1.0.0.tar` & `algocash-sdk-1.1.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:47:04.692953 algocash-sdk-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-19 01:47:04.692953 algocash-sdk-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:47:04.688953 algocash-sdk-1.0.0/algocash_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/algocash_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:47:04.692953 algocash-sdk-1.0.0/algocash_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/algocash_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/algocash_sdk/api/deposit_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/algocash_sdk/api/payout_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27919 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/algocash_sdk/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/algocash_sdk/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:47:04.692953 algocash-sdk-1.0.0/algocash_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/algocash_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/algocash_sdk/models/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/algocash_sdk/models/bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/algocash_sdk/models/callback_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/algocash_sdk/models/deposit_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/algocash_sdk/models/deposit_success.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/algocash_sdk/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/algocash_sdk/models/payer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/algocash_sdk/models/payout_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/algocash_sdk/models/payout_success.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/algocash_sdk/models/url.py
--rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/algocash_sdk/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:47:04.688953 algocash-sdk-1.0.0/algocash_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-19 01:47:04.000000 algocash-sdk-1.0.0/algocash_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-19 01:47:04.000000 algocash-sdk-1.0.0/algocash_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 01:47:04.000000 algocash-sdk-1.0.0/algocash_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-19 01:47:04.000000 algocash-sdk-1.0.0/algocash_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-19 01:47:04.000000 algocash-sdk-1.0.0/algocash_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 01:47:04.692953 algocash-sdk-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:47:04.692953 algocash-sdk-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/test/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/test/test_address.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/test/test_bank.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/test/test_callback_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/test/test_deposit_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/test/test_deposit_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/test/test_deposit_success.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/test/test_payer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/test/test_payout_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/test/test_payout_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/test/test_payout_success.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-19 01:46:53.000000 algocash-sdk-1.0.0/test/test_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:04:21.324744 algocash-sdk-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-19 19:04:21.324744 algocash-sdk-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:04:21.316744 algocash-sdk-1.1.1/algocash_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:04:21.320744 algocash-sdk-1.1.1/algocash_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/api/deposit_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/api/payout_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27984 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:04:21.320744 algocash-sdk-1.1.1/algocash_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/callback_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/deposit_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/deposit_success.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/payer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/payout_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/payout_success.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:04:21.320744 algocash-sdk-1.1.1/algocash_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-19 19:04:21.000000 algocash-sdk-1.1.1/algocash_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-19 19:04:21.000000 algocash-sdk-1.1.1/algocash_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:04:21.000000 algocash-sdk-1.1.1/algocash_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-19 19:04:21.000000 algocash-sdk-1.1.1/algocash_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 19:04:21.000000 algocash-sdk-1.1.1/algocash_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 19:04:21.324744 algocash-sdk-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:04:21.320744 algocash-sdk-1.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_callback_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_deposit_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_deposit_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_deposit_success.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_payer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_payout_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_payout_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_payout_success.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_url.py
```

### Comparing `algocash-sdk-1.0.0/README.md` & `algocash-sdk-1.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 payment_method = 'UPI' # str | 
 url = algocash_sdk.Url('callback_url', 'pending_url', 'success_url', 'error_url') # Url | 
 
 try:
     # create a deposit
     api_response = api_instance.create_deposit(invoice_id, amount, payer, payment_method, url)
     pprint(api_response)
+except ValueError as e:
+            print("ValueError Exception when calling DepositApi->create_deposit: %s\n" % e)
 except ApiException as e:
     print("Exception when calling DepositApi->create_deposit: %s\n" % e)
     pprint(json.loads(e.body))
 ```
 
 ## Documentation for API Endpoints
 
@@ -68,8 +70,8 @@
  - [Error](docs/Error.md)
  - [Payer](docs/Payer.md)
  - [PayoutRequest](docs/PayoutRequest.md)
  - [PayoutSuccess](docs/PayoutSuccess.md)
  - [Url](docs/Url.md)
 
  ### Author
-https://github.com/gitdevstar
+https://github.com/gitdevstar
```

### Comparing `algocash-sdk-1.0.0/algocash_sdk/__init__.py` & `algocash-sdk-1.1.1/algocash_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/algocash_sdk/api/deposit_api.py` & `algocash-sdk-1.1.1/algocash_sdk/api/deposit_api.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/algocash_sdk/api/payout_api.py` & `algocash-sdk-1.1.1/algocash_sdk/api/payout_api.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/algocash_sdk/api_client.py` & `algocash-sdk-1.1.1/algocash_sdk/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/1.0.0/python'
+        self.user_agent = 'Alogacash-sdk'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
@@ -135,15 +135,15 @@
         # body
         if body:
             body = self.sanitize_for_serialization(body)
             body = self.parameters_to_dicts(body)
 
         # auth setting
         self.update_params_for_auth(header_params, body, query_params, auth_settings)
-
+        
         # request url
         url = self.configuration.host + resource_path
 
         # perform request and return response
         response_data = self.request(
             method, url, query_params=query_params, headers=header_params,
             post_params=post_params, body=body,
@@ -222,15 +222,18 @@
         if response_type == "file":
             return self.__deserialize_file(response)
 
         # fetch data from response object
         try:
             data = json.loads(response.data)
         except ValueError:
-            return response.data
+            # return response.data
+            raise ValueError(
+                response.data
+            )
 
         return self.__deserialize(data, response_type)
 
     def __deserialize(self, data, klass):
         """Deserializes dict, list, str into an object.
 
         :param data: dict, list or str.
@@ -551,15 +554,15 @@
         :param querys: Query parameters tuple list to be updated.
         :param auth_settings: Authentication setting identifiers list.
         """
         if not auth_settings:
             return
 
         for auth in auth_settings:
-            auth_setting = self.configuration.auth_settings(post_params).get(auth)
+            auth_setting = self.configuration.auth_settings(auth, post_params)
             if auth_setting:
                 if not auth_setting['value']:
                     continue
                 elif auth_setting['in'] == 'header':
                     headers[auth_setting['key']] = auth_setting['value']
                 elif auth_setting['in'] == 'query':
                     querys.append((auth_setting['key'], auth_setting['value']))
```

### Comparing `algocash-sdk-1.0.0/algocash_sdk/configuration.py` & `algocash-sdk-1.1.1/algocash_sdk/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 import hashlib
 import json
+import hmac
 
 import six
 from six.moves import http_client as httplib
 
 
 class TypeWithDefault(type):
     def __init__(cls, name, bases, dct):
@@ -43,15 +44,15 @@
 
     Ref: https://github.com/swagger-api/swagger-codegen
     Do not edit the class manually.
     """
 
     def __init__(self):
         """Constructor"""
-        self.devmode = True
+        self.devmode = False
         # Default Base url
         self.host = "https://testapi2.algorithmic.cash" if self.devmode else "https://apiv2.algorithmic.cash"
         # Temp file folder for downloading files
         self.temp_folder_path = None
 
         # Authentication Settings
         # generate signature
@@ -202,37 +203,36 @@
         :return: The token for basic HTTP authentication.
         """
         return urllib3.util.make_headers(
             basic_auth=self.merchant_key + ':' + self.merchant_secret
         ).get('authorization')
     
     def generateSignature(self, post_params):
-        return  hashlib.sha256((json.dumps(post_params) + self.api_access_token).encode('utf-8')).hexdigest()
+        
+        signature = hmac.new(self.api_access_token.encode('utf-8'), json.dumps(post_params, separators=(',', ':')).encode('utf-8'), hashlib.sha256).hexdigest()
+        return signature
 
-    def auth_settings(self, post_params):
+    def auth_settings(self, auth, post_params):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
+        
         return {
-            'basicAuth':
-                {
                     'type': 'basic',
                     'in': 'header',
                     'key': 'Authorization',
                     'value': self.get_basic_auth_token()
-                },
-            'signatureAuth':
-                {
-                    'type': 'api_key',
-                    'in': 'header',
-                    'key': 'Signature',
-                    'value': self.generateSignature(post_params)
-                },
-        }
+                } if auth == 'basicAuth' else {
+                        'type': 'api_key',
+                        'in': 'header',
+                        'key': 'Signature',
+                        'value': self.generateSignature(post_params)
+                    }
+                
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
```

### Comparing `algocash-sdk-1.0.0/algocash_sdk/models/__init__.py` & `algocash-sdk-1.1.1/algocash_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/algocash_sdk/models/address.py` & `algocash-sdk-1.1.1/algocash_sdk/models/address.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/algocash_sdk/models/bank.py` & `algocash-sdk-1.1.1/algocash_sdk/models/bank.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/algocash_sdk/models/callback_payload.py` & `algocash-sdk-1.1.1/algocash_sdk/models/callback_payload.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/algocash_sdk/models/deposit_request.py` & `algocash-sdk-1.1.1/algocash_sdk/models/deposit_request.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/algocash_sdk/models/deposit_success.py` & `algocash-sdk-1.1.1/algocash_sdk/models/deposit_success.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/algocash_sdk/models/error.py` & `algocash-sdk-1.1.1/algocash_sdk/models/error.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/algocash_sdk/models/payer.py` & `algocash-sdk-1.1.1/algocash_sdk/models/payer.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/algocash_sdk/models/payout_request.py` & `algocash-sdk-1.1.1/algocash_sdk/models/payout_request.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/algocash_sdk/models/payout_success.py` & `algocash-sdk-1.1.1/algocash_sdk/models/payout_success.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/algocash_sdk/models/url.py` & `algocash-sdk-1.1.1/algocash_sdk/models/url.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/algocash_sdk/rest.py` & `algocash-sdk-1.1.1/algocash_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/algocash_sdk.egg-info/SOURCES.txt` & `algocash-sdk-1.1.1/algocash_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/setup.py` & `algocash-sdk-1.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "algocash-sdk"
-VERSION = "1.0.0"
+VERSION = "1.1.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -25,15 +24,15 @@
 
 setup(
     name=NAME,
     version=VERSION,
     description="Algocash API",
     author_email="loganph.work@gmail.com",
     url="",
-    keywords=["Swagger", "Algocash API"],
+    keywords=["Python", "Algocash API"],
     install_requires=REQUIRES,
     packages=find_packages(),
     include_package_data=True,
     long_description="""\
     This is a Algocash API  # noqa: E501
     """
 )
```

### Comparing `algocash-sdk-1.0.0/test/server.py` & `algocash-sdk-1.1.1/test/server.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/test/test_address.py` & `algocash-sdk-1.1.1/test/test_address.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/test/test_bank.py` & `algocash-sdk-1.1.1/test/test_bank.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/test/test_callback_payload.py` & `algocash-sdk-1.1.1/test/test_callback_payload.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/test/test_deposit_api.py` & `algocash-sdk-1.1.1/test/test_deposit_api.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/test/test_deposit_request.py` & `algocash-sdk-1.1.1/test/test_deposit_request.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/test/test_deposit_success.py` & `algocash-sdk-1.1.1/test/test_deposit_success.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/test/test_error.py` & `algocash-sdk-1.1.1/test/test_error.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/test/test_payer.py` & `algocash-sdk-1.1.1/test/test_payer.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/test/test_payout_api.py` & `algocash-sdk-1.1.1/test/test_payout_api.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/test/test_payout_request.py` & `algocash-sdk-1.1.1/test/test_payout_request.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/test/test_payout_success.py` & `algocash-sdk-1.1.1/test/test_payout_success.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.0.0/test/test_url.py` & `algocash-sdk-1.1.1/test/test_url.py`

 * *Files identical despite different names*

