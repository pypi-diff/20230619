# Comparing `tmp/pymexc-1.0.4.tar.gz` & `tmp/pymexc-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pymexc-1.0.4.tar", last modified: Fri Jun  2 20:27:56 2023, max compression
+gzip compressed data, was "dist\pymexc-1.0.5.tar", last modified: Mon Jun 19 15:10:52 2023, max compression
```

## Comparing `pymexc-1.0.4.tar` & `pymexc-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 20:27:56.528108 pymexc-1.0.4/
--rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 pymexc-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     3321 2023-06-02 20:27:56.528108 pymexc-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2221 2023-05-30 13:04:58.000000 pymexc-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 20:27:56.508103 pymexc-1.0.4/pymexc/
--rw-rw-rw-   0        0        0     1431 2023-05-30 13:22:30.000000 pymexc-1.0.4/pymexc/__init__.py
--rw-rw-rw-   0        0        0     5890 2023-06-02 20:17:49.000000 pymexc-1.0.4/pymexc/base.py
--rw-rw-rw-   0        0        0    18102 2023-06-02 19:53:45.000000 pymexc-1.0.4/pymexc/base_websocket.py
--rw-rw-rw-   0        0        0    67666 2023-06-02 19:56:06.000000 pymexc-1.0.4/pymexc/futures.py
--rw-rw-rw-   0        0        0    68220 2023-06-02 19:56:58.000000 pymexc-1.0.4/pymexc/spot.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:27:56.527108 pymexc-1.0.4/pymexc.egg-info/
--rw-rw-rw-   0        0        0     3321 2023-06-02 20:27:56.000000 pymexc-1.0.4/pymexc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-06-02 20:27:56.000000 pymexc-1.0.4/pymexc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 20:27:56.000000 pymexc-1.0.4/pymexc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-02 20:27:56.000000 pymexc-1.0.4/pymexc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2023-06-02 20:27:56.000000 pymexc-1.0.4/pymexc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-02 20:27:56.000000 pymexc-1.0.4/pymexc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 20:27:56.529108 pymexc-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1697 2023-06-02 19:59:59.000000 pymexc-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:10:52.318189 pymexc-1.0.5/
+-rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 pymexc-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3321 2023-06-19 15:10:52.318189 pymexc-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2221 2023-05-30 13:04:58.000000 pymexc-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 15:10:52.293078 pymexc-1.0.5/pymexc/
+-rw-rw-rw-   0        0        0     1431 2023-05-30 13:22:30.000000 pymexc-1.0.5/pymexc/__init__.py
+-rw-rw-rw-   0        0        0     5892 2023-06-19 15:05:51.000000 pymexc-1.0.5/pymexc/base.py
+-rw-rw-rw-   0        0        0    18102 2023-06-02 19:53:45.000000 pymexc-1.0.5/pymexc/base_websocket.py
+-rw-rw-rw-   0        0        0    67666 2023-06-02 19:56:06.000000 pymexc-1.0.5/pymexc/futures.py
+-rw-rw-rw-   0        0        0    68220 2023-06-02 19:56:58.000000 pymexc-1.0.5/pymexc/spot.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:10:52.317190 pymexc-1.0.5/pymexc.egg-info/
+-rw-rw-rw-   0        0        0     3321 2023-06-19 15:10:52.000000 pymexc-1.0.5/pymexc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-06-19 15:10:52.000000 pymexc-1.0.5/pymexc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 15:10:52.000000 pymexc-1.0.5/pymexc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-19 15:10:52.000000 pymexc-1.0.5/pymexc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2023-06-19 15:10:52.000000 pymexc-1.0.5/pymexc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-19 15:10:52.000000 pymexc-1.0.5/pymexc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 15:10:52.319190 pymexc-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1697 2023-06-19 15:10:02.000000 pymexc-1.0.5/setup.py
```

### Comparing `pymexc-1.0.4/LICENSE` & `pymexc-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.4/PKG-INFO` & `pymexc-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pymexc
-Version: 1.0.4
+Version: 1.0.5
 Summary: Unofficial python library for interacting with the MEXC crypto exchange
 Home-page: https://github.com/makarworld/pymexc.git
-Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.4.zip
+Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.5.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymexc-1.0.4/README.md` & `pymexc-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.4/pymexc/__init__.py` & `pymexc-1.0.5/pymexc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.4/pymexc/base.py` & `pymexc-1.0.5/pymexc/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,21 +68,23 @@
             router = f"/{router}"
 
         # clear None values
         kwargs = {k: v for k, v in kwargs.items() if v is not None}
 
         if kwargs.get('params'):
             kwargs['params'] = {k: v for k, v in kwargs['params'].items() if v is not None}
-            
-            if self.api_key and self.api_secret:
-                # add signature
-                timestamp = str(int(time.time() * 1000))
-                kwargs['params']['recvWindow'] = self.recvWindow
-                kwargs['params']['timestamp']  = timestamp
-                kwargs['params']['signature']  = self.sign(**kwargs['params'])
+        else:
+            kwargs['params'] = {}
+
+        if self.api_key and self.api_secret:
+            # add signature
+            timestamp = str(int(time.time() * 1000))
+        kwargs['params']['recvWindow'] = self.recvWindow
+        kwargs['params']['timestamp']  = timestamp
+        kwargs['params']['signature']  = self.sign(**kwargs['params'])
 
         response = self.session.request(method, f"{self.base_url}{router}", *args, **kwargs)
 
         return response.json()
     
 class _FuturesHTTP(MexcSDK):
     def __init__(self, api_key: str = None, api_secret: str = None, proxies: dict = None):
```

### Comparing `pymexc-1.0.4/pymexc/base_websocket.py` & `pymexc-1.0.5/pymexc/base_websocket.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.4/pymexc/futures.py` & `pymexc-1.0.5/pymexc/futures.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.4/pymexc/spot.py` & `pymexc-1.0.5/pymexc/spot.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.4/pymexc.egg-info/PKG-INFO` & `pymexc-1.0.5/pymexc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pymexc
-Version: 1.0.4
+Version: 1.0.5
 Summary: Unofficial python library for interacting with the MEXC crypto exchange
 Home-page: https://github.com/makarworld/pymexc.git
-Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.4.zip
+Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.5.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymexc-1.0.4/setup.py` & `pymexc-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 :author: abuztrade
 :license: MIT License, see LICENSE file.
 :copyright: (c) 2022 by abuztrade.
 """
 
 
-version = '1.0.4'
+version = '1.0.5'
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pymexc",
     version=version,
```

