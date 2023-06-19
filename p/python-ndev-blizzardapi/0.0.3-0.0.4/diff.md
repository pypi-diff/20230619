# Comparing `tmp/python-ndev-blizzardapi-0.0.3.tar.gz` & `tmp/python-ndev-blizzardapi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-ndev-blizzardapi-0.0.3.tar", last modified: Fri Mar 10 20:04:52 2023, max compression
+gzip compressed data, was "python-ndev-blizzardapi-0.0.4.tar", last modified: Mon Jun 19 21:29:18 2023, max compression
```

## Comparing `python-ndev-blizzardapi-0.0.3.tar` & `python-ndev-blizzardapi-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-10 20:04:52.410054 python-ndev-blizzardapi-0.0.3/
--rw-rw-rw-   0        0        0      134 2023-03-10 17:55:01.000000 python-ndev-blizzardapi-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2202 2023-03-10 20:04:52.410054 python-ndev-blizzardapi-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1475 2023-03-10 20:02:35.000000 python-ndev-blizzardapi-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-10 20:04:52.391960 python-ndev-blizzardapi-0.0.3/blizzardAPI/
--rw-rw-rw-   0        0        0      126 2023-03-10 03:27:21.000000 python-ndev-blizzardapi-0.0.3/blizzardAPI/__init__.py
--rw-rw-rw-   0        0        0     4121 2023-03-10 03:23:52.000000 python-ndev-blizzardapi-0.0.3/blizzardAPI/api.py
-drwxrwxrwx   0        0        0        0 2023-03-10 20:04:52.395265 python-ndev-blizzardapi-0.0.3/blizzardAPI/battlenet/
--rw-rw-rw-   0        0        0       25 2023-03-10 03:36:02.000000 python-ndev-blizzardapi-0.0.3/blizzardAPI/battlenet/__init__.py
--rw-rw-rw-   0        0        0      458 2023-03-10 03:44:26.000000 python-ndev-blizzardapi-0.0.3/blizzardAPI/battlenet/battlenet_api.py
--rw-rw-rw-   0        0        0     1539 2023-03-10 03:47:42.000000 python-ndev-blizzardapi-0.0.3/blizzardAPI/battlenet/battlenet_oauth.py
--rw-rw-rw-   0        0        0      646 2023-03-10 16:43:27.000000 python-ndev-blizzardapi-0.0.3/blizzardAPI/blizzard_api.py
-drwxrwxrwx   0        0        0        0 2023-03-10 20:04:52.409057 python-ndev-blizzardapi-0.0.3/python_ndev_blizzardapi.egg-info/
--rw-rw-rw-   0        0        0     2202 2023-03-10 20:04:52.000000 python-ndev-blizzardapi-0.0.3/python_ndev_blizzardapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-03-10 20:04:52.000000 python-ndev-blizzardapi-0.0.3/python_ndev_blizzardapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-10 20:04:52.000000 python-ndev-blizzardapi-0.0.3/python_ndev_blizzardapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-03-10 20:04:52.000000 python-ndev-blizzardapi-0.0.3/python_ndev_blizzardapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-10 20:04:52.000000 python-ndev-blizzardapi-0.0.3/python_ndev_blizzardapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-10 20:04:52.410054 python-ndev-blizzardapi-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1004 2023-03-10 20:02:23.000000 python-ndev-blizzardapi-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 21:29:18.952839 python-ndev-blizzardapi-0.0.4/
+-rw-rw-rw-   0        0        0      134 2023-03-10 17:55:01.000000 python-ndev-blizzardapi-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2202 2023-06-19 21:29:18.952339 python-ndev-blizzardapi-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1475 2023-03-10 20:02:35.000000 python-ndev-blizzardapi-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 21:29:18.916499 python-ndev-blizzardapi-0.0.4/blizzardAPI/
+-rw-rw-rw-   0        0        0      161 2023-03-11 02:36:09.000000 python-ndev-blizzardapi-0.0.4/blizzardAPI/__init__.py
+-rw-rw-rw-   0        0        0     4446 2023-06-19 02:12:09.000000 python-ndev-blizzardapi-0.0.4/blizzardAPI/api.py
+drwxrwxrwx   0        0        0        0 2023-06-19 21:29:18.933737 python-ndev-blizzardapi-0.0.4/blizzardAPI/battlenet/
+-rw-rw-rw-   0        0        0       25 2023-03-10 03:36:02.000000 python-ndev-blizzardapi-0.0.4/blizzardAPI/battlenet/__init__.py
+-rw-rw-rw-   0        0        0      458 2023-03-10 03:44:26.000000 python-ndev-blizzardapi-0.0.4/blizzardAPI/battlenet/battlenet_api.py
+-rw-rw-rw-   0        0        0     1539 2023-03-10 03:47:42.000000 python-ndev-blizzardapi-0.0.4/blizzardAPI/battlenet/battlenet_oauth.py
+-rw-rw-rw-   0        0        0      539 2023-06-19 02:10:51.000000 python-ndev-blizzardapi-0.0.4/blizzardAPI/blizzard_api.py
+drwxrwxrwx   0        0        0        0 2023-06-19 21:29:18.951366 python-ndev-blizzardapi-0.0.4/python_ndev_blizzardapi.egg-info/
+-rw-rw-rw-   0        0        0     2202 2023-06-19 21:29:18.000000 python-ndev-blizzardapi-0.0.4/python_ndev_blizzardapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2023-06-19 21:29:18.000000 python-ndev-blizzardapi-0.0.4/python_ndev_blizzardapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 21:29:18.000000 python-ndev-blizzardapi-0.0.4/python_ndev_blizzardapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-19 21:29:18.000000 python-ndev-blizzardapi-0.0.4/python_ndev_blizzardapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-19 21:29:18.000000 python-ndev-blizzardapi-0.0.4/python_ndev_blizzardapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 21:29:18.952839 python-ndev-blizzardapi-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1004 2023-06-19 21:28:52.000000 python-ndev-blizzardapi-0.0.4/setup.py
```

### Comparing `python-ndev-blizzardapi-0.0.3/PKG-INFO` & `python-ndev-blizzardapi-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ndev-blizzardapi
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python module created to integrate your Python project with the Blizzard API
 Home-page: https://github.com/natanrmaia/python-ndev-blizzardapi
 Author: natanrmaia
 Author-email: contato@natanael.dev.br
 Project-URL: Documentation, https://python-ndev-blizzardapi.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/natanrmaia/python-ndev-blizzardapi
 Project-URL: Bug Reports, https://github.com/natanrmaia/python-ndev-blizzardapi/issues
```

### Comparing `python-ndev-blizzardapi-0.0.3/README.md` & `python-ndev-blizzardapi-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `python-ndev-blizzardapi-0.0.3/blizzardAPI/api.py` & `python-ndev-blizzardapi-0.0.4/blizzardAPI/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import requests
+import requests, os, importlib, inspect
 
 class API:
 
     def __init__(self, client_id, client_secret):
 
         """ API Keys """
         self.client_id      = client_id         # <--- self.client_id
@@ -51,23 +51,25 @@
         :return: The access token is being returned.
         """
         url = self.format_url(region, '/oauth/token', 'oauth')
         data = {
             'grant_type': 'client_credentials',
         }
         response = self.session.post(url, data=data, auth=(self.client_id, self.client_secret))
+
         return self.response_handler(response)
 
     def response_handler(self, response):
         """
         It takes a response object, and returns the response object's json() method
 
         :param response: The response object returned by the request
         :return: The response.json() method will convert the JSON string into a Python dictionary.
         """
+
         return response.json()
 
     def request_handler(self, url, region, query_params):
 
         if self.access_token is None:
             client_token = self.get_client_token(region)
             self.access_token = client_token['access_token']
@@ -87,15 +89,26 @@
         :param api: The API you want to call
         :param query_params: The query parameters you want to pass to the API (optional)
         :return: The response is being returned.
         """
         if query_params is None:
             query_params = {}
 
+        query_params['access_token'] = self.access_token
+
+        if query_params['locale'] is None:
+            query_params['locale'] = ''
+
+        if region is None:
+            region = 'us'
+
+        query_params['namespace'] = '{}-{}'.format(query_params['namespace'], region)
+
         url = self.format_url(region, api)
+
         return self.request_handler(url, region, query_params)
 
     def get_oauth(self, region, api, query_params=None):
         """
         It takes a region, an api, and query_params, and returns the response
 
         :param region: The region of the server you want to connect to
@@ -103,8 +116,9 @@
         :param query_params: The query parameters you want to pass to the API (optional)
         :return: The response is being returned.
         """
         if query_params is None:
             query_params = {}
 
         url = self.format_url(region, api, 'oauth')
+
         return self.request_handler(url, region, query_params)
```

### Comparing `python-ndev-blizzardapi-0.0.3/blizzardAPI/battlenet/battlenet_oauth.py` & `python-ndev-blizzardapi-0.0.4/blizzardAPI/battlenet/battlenet_oauth.py`

 * *Files identical despite different names*

### Comparing `python-ndev-blizzardapi-0.0.3/blizzardAPI/blizzard_api.py` & `python-ndev-blizzardapi-0.0.4/blizzardAPI/blizzard_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from .battlenet.battlenet_api   import BattleNetAPI
-from .diablo3                   import D3API
-from .diablo4                   import D4API
-from .hearthstone               import HSAPI
-from .overwatch_league          import OWLAPI
-from .starcraft2                import SC2API
-from .world_of_warcraft         import WoWAPI
+from .world_of_warcraft.wow_api import WoWAPI
+# from .diablo3                   import D3API
+# from .diablo4                   import D4API
+# from .hearthstone               import HSAPI
+# from .overwatch_league          import OWLAPI
+# from .starcraft2                import SC2API
 
 class BlizzardAPI:
     
     def __init__(self, client_id, client_secret):
 
         self.bnet   = BattleNetAPI(client_id, client_secret)
-        # self.wow    = WoWAPI(client_id, client_secret)
-        # self.sc2    = SC2API(client_id, client_secret)
-        # self.d3     = D3API(client_id, client_secret)
+        self.wow    = WoWAPI(client_id, client_secret)
```

### Comparing `python-ndev-blizzardapi-0.0.3/python_ndev_blizzardapi.egg-info/PKG-INFO` & `python-ndev-blizzardapi-0.0.4/python_ndev_blizzardapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ndev-blizzardapi
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python module created to integrate your Python project with the Blizzard API
 Home-page: https://github.com/natanrmaia/python-ndev-blizzardapi
 Author: natanrmaia
 Author-email: contato@natanael.dev.br
 Project-URL: Documentation, https://python-ndev-blizzardapi.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/natanrmaia/python-ndev-blizzardapi
 Project-URL: Bug Reports, https://github.com/natanrmaia/python-ndev-blizzardapi/issues
```

### Comparing `python-ndev-blizzardapi-0.0.3/setup.py` & `python-ndev-blizzardapi-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="python-ndev-blizzardapi",
-    version="0.0.3",
+    version="0.0.4",
     packages=find_packages(),
     install_requires=[
         "requests>=2.28.2",
     ],
     author="natanrmaia",
     author_email="contato@natanael.dev.br",
     description="Python module created to integrate your Python project with the Blizzard API",
```

