# Comparing `tmp/pymexc-1.0.5.tar.gz` & `tmp/pymexc-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pymexc-1.0.5.tar", last modified: Mon Jun 19 15:10:52 2023, max compression
+gzip compressed data, was "dist\pymexc-1.0.6.tar", last modified: Mon Jun 19 15:37:07 2023, max compression
```

## Comparing `pymexc-1.0.5.tar` & `pymexc-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 15:10:52.318189 pymexc-1.0.5/
--rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 pymexc-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     3321 2023-06-19 15:10:52.318189 pymexc-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2221 2023-05-30 13:04:58.000000 pymexc-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 15:10:52.293078 pymexc-1.0.5/pymexc/
--rw-rw-rw-   0        0        0     1431 2023-05-30 13:22:30.000000 pymexc-1.0.5/pymexc/__init__.py
--rw-rw-rw-   0        0        0     5892 2023-06-19 15:05:51.000000 pymexc-1.0.5/pymexc/base.py
--rw-rw-rw-   0        0        0    18102 2023-06-02 19:53:45.000000 pymexc-1.0.5/pymexc/base_websocket.py
--rw-rw-rw-   0        0        0    67666 2023-06-02 19:56:06.000000 pymexc-1.0.5/pymexc/futures.py
--rw-rw-rw-   0        0        0    68220 2023-06-02 19:56:58.000000 pymexc-1.0.5/pymexc/spot.py
-drwxrwxrwx   0        0        0        0 2023-06-19 15:10:52.317190 pymexc-1.0.5/pymexc.egg-info/
--rw-rw-rw-   0        0        0     3321 2023-06-19 15:10:52.000000 pymexc-1.0.5/pymexc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-06-19 15:10:52.000000 pymexc-1.0.5/pymexc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 15:10:52.000000 pymexc-1.0.5/pymexc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-19 15:10:52.000000 pymexc-1.0.5/pymexc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2023-06-19 15:10:52.000000 pymexc-1.0.5/pymexc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-19 15:10:52.000000 pymexc-1.0.5/pymexc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 15:10:52.319190 pymexc-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1697 2023-06-19 15:10:02.000000 pymexc-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:37:07.081679 pymexc-1.0.6/
+-rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 pymexc-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3321 2023-06-19 15:37:07.082679 pymexc-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2221 2023-05-30 13:04:58.000000 pymexc-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 15:37:07.066676 pymexc-1.0.6/pymexc/
+-rw-rw-rw-   0        0        0     1431 2023-05-30 13:22:30.000000 pymexc-1.0.6/pymexc/__init__.py
+-rw-rw-rw-   0        0        0     6057 2023-06-19 15:35:35.000000 pymexc-1.0.6/pymexc/base.py
+-rw-rw-rw-   0        0        0    18102 2023-06-02 19:53:45.000000 pymexc-1.0.6/pymexc/base_websocket.py
+-rw-rw-rw-   0        0        0    67666 2023-06-02 19:56:06.000000 pymexc-1.0.6/pymexc/futures.py
+-rw-rw-rw-   0        0        0    68220 2023-06-02 19:56:58.000000 pymexc-1.0.6/pymexc/spot.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:37:07.080679 pymexc-1.0.6/pymexc.egg-info/
+-rw-rw-rw-   0        0        0     3321 2023-06-19 15:37:06.000000 pymexc-1.0.6/pymexc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-06-19 15:37:06.000000 pymexc-1.0.6/pymexc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 15:37:06.000000 pymexc-1.0.6/pymexc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-19 15:37:06.000000 pymexc-1.0.6/pymexc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2023-06-19 15:37:06.000000 pymexc-1.0.6/pymexc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-19 15:37:06.000000 pymexc-1.0.6/pymexc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 15:37:07.086680 pymexc-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1697 2023-06-19 15:36:04.000000 pymexc-1.0.6/setup.py
```

### Comparing `pymexc-1.0.5/LICENSE` & `pymexc-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.5/PKG-INFO` & `pymexc-1.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pymexc
-Version: 1.0.5
+Version: 1.0.6
 Summary: Unofficial python library for interacting with the MEXC crypto exchange
 Home-page: https://github.com/makarworld/pymexc.git
-Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.5.zip
+Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.6.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymexc-1.0.5/README.md` & `pymexc-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.5/pymexc/__init__.py` & `pymexc-1.0.6/pymexc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.5/pymexc/base.py` & `pymexc-1.0.6/pymexc/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import hmac, hashlib
 import requests
 import logging
 import time
 
 logger = logging.getLogger(__name__)
 
+class MexcAPIError(Exception): pass
+
 class MexcSDK(ABC):
     """
     Initializes a new instance of the class with the given `api_key` and `api_secret` parameters.
 
     :param api_key: A string representing the API key.
     :param api_secret: A string representing the API secret.
     :param base_url: A string representing the base URL of the API.
@@ -80,14 +82,17 @@
             timestamp = str(int(time.time() * 1000))
         kwargs['params']['recvWindow'] = self.recvWindow
         kwargs['params']['timestamp']  = timestamp
         kwargs['params']['signature']  = self.sign(**kwargs['params'])
 
         response = self.session.request(method, f"{self.base_url}{router}", *args, **kwargs)
 
+        if not response.ok:
+            raise MexcAPIError(f'(code={response.json()["code"]}): {response.json()["msg"]}')
+
         return response.json()
     
 class _FuturesHTTP(MexcSDK):
     def __init__(self, api_key: str = None, api_secret: str = None, proxies: dict = None):
         super().__init__(api_key, api_secret, "https://contract.mexc.com", proxies = proxies)
 
         self.session.headers.update({
```

### Comparing `pymexc-1.0.5/pymexc/base_websocket.py` & `pymexc-1.0.6/pymexc/base_websocket.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.5/pymexc/futures.py` & `pymexc-1.0.6/pymexc/futures.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.5/pymexc/spot.py` & `pymexc-1.0.6/pymexc/spot.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.5/pymexc.egg-info/PKG-INFO` & `pymexc-1.0.6/pymexc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pymexc
-Version: 1.0.5
+Version: 1.0.6
 Summary: Unofficial python library for interacting with the MEXC crypto exchange
 Home-page: https://github.com/makarworld/pymexc.git
-Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.5.zip
+Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.6.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymexc-1.0.5/setup.py` & `pymexc-1.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 :author: abuztrade
 :license: MIT License, see LICENSE file.
 :copyright: (c) 2022 by abuztrade.
 """
 
 
-version = '1.0.5'
+version = '1.0.6'
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pymexc",
     version=version,
```

