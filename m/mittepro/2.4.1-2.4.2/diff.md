# Comparing `tmp/mittepro-2.4.1.tar.gz` & `tmp/mittepro-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mittepro-2.4.1.tar", last modified: Thu Oct  8 19:19:51 2020, max compression
+gzip compressed data, was "dist/mittepro-2.4.2.tar", last modified: Fri Oct  9 13:07:33 2020, max compression
```

## Comparing `mittepro-2.4.1.tar` & `mittepro-2.4.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2020-10-08 19:19:51.000000 mittepro-2.4.1/
--rw-rw-r--   0 thiago    (1000) thiago    (1000)       46 2020-10-08 12:10:09.000000 mittepro-2.4.1/MANIFEST.in
--rw-rw-r--   0 thiago    (1000) thiago    (1000)     5996 2020-10-08 19:19:51.000000 mittepro-2.4.1/PKG-INFO
--rw-rw-r--   0 thiago    (1000) thiago    (1000)     4326 2020-10-08 12:10:09.000000 mittepro-2.4.1/README.rst
-drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2020-10-08 19:19:51.000000 mittepro-2.4.1/mittepro/
--rw-rw-r--   0 thiago    (1000) thiago    (1000)       92 2020-10-08 18:21:07.000000 mittepro-2.4.1/mittepro/__init__.py
--rw-rw-r--   0 thiago    (1000) thiago    (1000)     4849 2020-10-08 19:17:00.000000 mittepro-2.4.1/mittepro/api.py
-drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2020-10-08 19:19:51.000000 mittepro-2.4.1/mittepro/apysignature/
--rw-rw-r--   0 thiago    (1000) thiago    (1000)        0 2020-10-08 12:10:10.000000 mittepro-2.4.1/mittepro/apysignature/__init__.py
--rw-rw-r--   0 thiago    (1000) thiago    (1000)      798 2020-10-08 17:17:12.000000 mittepro-2.4.1/mittepro/apysignature/query_encoder.py
--rw-rw-r--   0 thiago    (1000) thiago    (1000)     2732 2020-10-08 17:17:11.000000 mittepro-2.4.1/mittepro/apysignature/signature.py
--rw-rw-r--   0 thiago    (1000) thiago    (1000)     1841 2020-10-08 19:17:28.000000 mittepro-2.4.1/mittepro/client.py
--rw-rw-r--   0 thiago    (1000) thiago    (1000)     1682 2020-10-08 13:14:31.000000 mittepro-2.4.1/mittepro/mitte_exceptions.py
--rw-rw-r--   0 thiago    (1000) thiago    (1000)     7103 2020-10-08 19:17:45.000000 mittepro-2.4.1/mittepro/models.py
--rw-rw-r--   0 thiago    (1000) thiago    (1000)      621 2020-10-08 16:25:54.000000 mittepro-2.4.1/mittepro/test_variables.py
--rw-rw-r--   0 thiago    (1000) thiago    (1000)     6181 2020-10-08 17:13:14.000000 mittepro-2.4.1/mittepro/tests.py
--rw-rw-r--   0 thiago    (1000) thiago    (1000)      629 2020-10-08 12:10:10.000000 mittepro-2.4.1/mittepro/utils.py
-drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2020-10-08 19:19:51.000000 mittepro-2.4.1/mittepro.egg-info/
--rw-rw-r--   0 thiago    (1000) thiago    (1000)     5996 2020-10-08 19:19:50.000000 mittepro-2.4.1/mittepro.egg-info/PKG-INFO
--rw-rw-r--   0 thiago    (1000) thiago    (1000)      475 2020-10-08 19:19:50.000000 mittepro-2.4.1/mittepro.egg-info/SOURCES.txt
--rw-rw-r--   0 thiago    (1000) thiago    (1000)        1 2020-10-08 19:19:50.000000 mittepro-2.4.1/mittepro.egg-info/dependency_links.txt
--rw-rw-r--   0 thiago    (1000) thiago    (1000)       31 2020-10-08 19:19:50.000000 mittepro-2.4.1/mittepro.egg-info/requires.txt
--rw-rw-r--   0 thiago    (1000) thiago    (1000)        9 2020-10-08 19:19:50.000000 mittepro-2.4.1/mittepro.egg-info/top_level.txt
--rw-rw-r--   0 thiago    (1000) thiago    (1000)       79 2020-10-08 19:19:51.000000 mittepro-2.4.1/setup.cfg
--rw-rw-r--   0 thiago    (1000) thiago    (1000)     1313 2020-10-08 18:20:51.000000 mittepro-2.4.1/setup.py
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2020-10-09 13:07:33.000000 mittepro-2.4.2/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)       46 2020-10-08 12:10:09.000000 mittepro-2.4.2/MANIFEST.in
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     5996 2020-10-09 13:07:33.000000 mittepro-2.4.2/PKG-INFO
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     4326 2020-10-08 12:10:09.000000 mittepro-2.4.2/README.rst
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2020-10-09 13:07:33.000000 mittepro-2.4.2/mittepro/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)       92 2020-10-09 13:06:55.000000 mittepro-2.4.2/mittepro/__init__.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     4849 2020-10-09 13:06:55.000000 mittepro-2.4.2/mittepro/api.py
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2020-10-09 13:07:33.000000 mittepro-2.4.2/mittepro/apysignature/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)        0 2020-10-08 12:10:10.000000 mittepro-2.4.2/mittepro/apysignature/__init__.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      798 2020-10-08 17:17:12.000000 mittepro-2.4.2/mittepro/apysignature/query_encoder.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     2732 2020-10-08 17:17:11.000000 mittepro-2.4.2/mittepro/apysignature/signature.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1841 2020-10-08 19:17:28.000000 mittepro-2.4.2/mittepro/client.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1682 2020-10-08 13:14:31.000000 mittepro-2.4.2/mittepro/mitte_exceptions.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     7103 2020-10-08 19:17:45.000000 mittepro-2.4.2/mittepro/models.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      621 2020-10-08 16:25:54.000000 mittepro-2.4.2/mittepro/test_variables.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     6181 2020-10-08 17:13:14.000000 mittepro-2.4.2/mittepro/tests.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      629 2020-10-08 12:10:10.000000 mittepro-2.4.2/mittepro/utils.py
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2020-10-09 13:07:33.000000 mittepro-2.4.2/mittepro.egg-info/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     5996 2020-10-09 13:07:33.000000 mittepro-2.4.2/mittepro.egg-info/PKG-INFO
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      475 2020-10-09 13:07:33.000000 mittepro-2.4.2/mittepro.egg-info/SOURCES.txt
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)        1 2020-10-09 13:07:33.000000 mittepro-2.4.2/mittepro.egg-info/dependency_links.txt
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)       31 2020-10-09 13:07:33.000000 mittepro-2.4.2/mittepro.egg-info/requires.txt
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)        9 2020-10-09 13:07:33.000000 mittepro-2.4.2/mittepro.egg-info/top_level.txt
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)       79 2020-10-09 13:07:33.000000 mittepro-2.4.2/setup.cfg
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1313 2020-10-09 13:06:55.000000 mittepro-2.4.2/setup.py
```

### Comparing `mittepro-2.4.1/PKG-INFO` & `mittepro-2.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mittepro
-Version: 2.4.1
+Version: 2.4.2
 Summary: MittePro is a powerful marketing tool with features to help companies with their marketing goals and deliver emails from their websites and apps.
 Home-page: https://github.com/ThCC/mittepro-py
 Author: Thiago Cardoso de Castro
 Author-email: thiago.decastro2@gmail.com
 License: Apache-2.0
 Description: Client service, to send simple text emails or, using a template created at MittePro, send more complex emails.
```

### Comparing `mittepro-2.4.1/README.rst` & `mittepro-2.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `mittepro-2.4.1/mittepro/api.py` & `mittepro-2.4.2/mittepro/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import requests
 from .utils import is_json
 from .mitte_exceptions import APIError, TimeoutError
 from .apysignature.query_encoder import QueryEncoder
 from .apysignature.signature import Request as Request_sig, Token
 from requests import Request, Session, ReadTimeout, ConnectTimeout, HTTPError
 
-__version__ = '2.4.1'
+__version__ = '2.4.2'
 logging.basicConfig(format='%(asctime)s %(message)s')
 
 
 def endpoint(method, endpoint):
     def decorator(func):
         def wrapped(self, *args, **kwargs):
             self.http_method = method
```

### Comparing `mittepro-2.4.1/mittepro/apysignature/query_encoder.py` & `mittepro-2.4.2/mittepro/apysignature/query_encoder.py`

 * *Files identical despite different names*

### Comparing `mittepro-2.4.1/mittepro/apysignature/signature.py` & `mittepro-2.4.2/mittepro/apysignature/signature.py`

 * *Files identical despite different names*

### Comparing `mittepro-2.4.1/mittepro/client.py` & `mittepro-2.4.2/mittepro/client.py`

 * *Files identical despite different names*

### Comparing `mittepro-2.4.1/mittepro/mitte_exceptions.py` & `mittepro-2.4.2/mittepro/mitte_exceptions.py`

 * *Files identical despite different names*

### Comparing `mittepro-2.4.1/mittepro/models.py` & `mittepro-2.4.2/mittepro/models.py`

 * *Files identical despite different names*

### Comparing `mittepro-2.4.1/mittepro/test_variables.py` & `mittepro-2.4.2/mittepro/test_variables.py`

 * *Files identical despite different names*

### Comparing `mittepro-2.4.1/mittepro/tests.py` & `mittepro-2.4.2/mittepro/tests.py`

 * *Files identical despite different names*

### Comparing `mittepro-2.4.1/mittepro/utils.py` & `mittepro-2.4.2/mittepro/utils.py`

 * *Files identical despite different names*

### Comparing `mittepro-2.4.1/mittepro.egg-info/PKG-INFO` & `mittepro-2.4.2/mittepro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mittepro
-Version: 2.4.1
+Version: 2.4.2
 Summary: MittePro is a powerful marketing tool with features to help companies with their marketing goals and deliver emails from their websites and apps.
 Home-page: https://github.com/ThCC/mittepro-py
 Author: Thiago Cardoso de Castro
 Author-email: thiago.decastro2@gmail.com
 License: Apache-2.0
 Description: Client service, to send simple text emails or, using a template created at MittePro, send more complex emails.
```

### Comparing `mittepro-2.4.1/setup.py` & `mittepro-2.4.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='mittepro',
-    version='2.4.1',
+    version='2.4.2',
     install_requires=[
         'arrow>=0.17.0',
         'requests==2.24.0',
     ],
     url='https://github.com/ThCC/mittepro-py',
     description='MittePro is a powerful marketing tool with features to help companies with their marketing goals and deliver emails from their websites and apps.',
     long_description=open("README.rst").read(),
```

