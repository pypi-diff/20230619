# Comparing `tmp/mod.io-0.4.3b2.tar.gz` & `tmp/mod.io-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mod.io-0.4.3b2.tar", last modified: Mon Nov 28 17:36:32 2022, max compression
+gzip compressed data, was "mod.io-0.5.0.tar", last modified: Mon Jun 19 14:34:13 2023, max compression
```

## Comparing `mod.io-0.4.3b2.tar` & `mod.io-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxrwxrwx   0        0        0        0 2022-11-28 17:36:32.957639 mod.io-0.4.3b2/
--rw-rw-rw-   0        0        0     1091 2022-11-26 17:04:58.000000 mod.io-0.4.3b2/LICENSE
--rw-rw-rw-   0        0        0     2440 2022-11-28 17:36:32.956639 mod.io-0.4.3b2/PKG-INFO
--rw-rw-rw-   0        0        0     2174 2022-11-26 17:04:58.000000 mod.io-0.4.3b2/README.md
-drwxrwxrwx   0        0        0        0 2022-11-28 17:36:32.933638 mod.io-0.4.3b2/mod.io.egg-info/
--rw-rw-rw-   0        0        0     2440 2022-11-28 17:36:32.000000 mod.io-0.4.3b2/mod.io.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2022-11-28 17:36:32.000000 mod.io-0.4.3b2/mod.io.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-28 17:36:32.000000 mod.io-0.4.3b2/mod.io.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2022-11-28 17:36:32.000000 mod.io-0.4.3b2/mod.io.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-11-28 17:36:32.000000 mod.io-0.4.3b2/mod.io.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-11-28 17:36:32.955639 mod.io-0.4.3b2/modio/
--rw-rw-rw-   0        0        0      229 2022-11-28 17:35:16.000000 mod.io-0.4.3b2/modio/__init__.py
--rw-rw-rw-   0        0        0    24859 2022-11-27 22:04:00.000000 mod.io-0.4.3b2/modio/client.py
--rw-rw-rw-   0        0        0    27854 2022-11-28 17:29:00.000000 mod.io-0.4.3b2/modio/entities.py
--rw-rw-rw-   0        0        0     5700 2022-11-28 17:35:24.000000 mod.io-0.4.3b2/modio/enums.py
--rw-rw-rw-   0        0        0      850 2022-11-26 17:04:58.000000 mod.io-0.4.3b2/modio/errors.py
--rw-rw-rw-   0        0        0    20223 2022-11-27 16:57:39.000000 mod.io-0.4.3b2/modio/game.py
--rw-rw-rw-   0        0        0     4927 2022-11-27 16:57:39.000000 mod.io-0.4.3b2/modio/mixins.py
--rw-rw-rw-   0        0        0    36367 2022-11-26 17:04:58.000000 mod.io-0.4.3b2/modio/mod.py
--rw-rw-rw-   0        0        0    16411 2022-11-26 17:04:58.000000 mod.io-0.4.3b2/modio/objects.py
--rw-rw-rw-   0        0        0     4519 2022-11-26 17:04:58.000000 mod.io-0.4.3b2/modio/utils.py
--rw-rw-rw-   0        0        0      356 2022-11-26 17:04:58.000000 mod.io-0.4.3b2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-11-28 17:36:32.957639 mod.io-0.4.3b2/setup.cfg
--rw-rw-rw-   0        0        0      797 2022-11-26 17:04:58.000000 mod.io-0.4.3b2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 14:34:13.107907 mod.io-0.5.0/
+-rw-rw-rw-   0        0        0     1091 2022-11-26 17:04:58.000000 mod.io-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     2333 2023-06-19 14:34:13.105906 mod.io-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2069 2023-06-18 20:41:40.000000 mod.io-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 14:34:13.064912 mod.io-0.5.0/mod.io.egg-info/
+-rw-rw-rw-   0        0        0     2333 2023-06-19 14:34:12.000000 mod.io-0.5.0/mod.io.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-06-19 14:34:13.000000 mod.io-0.5.0/mod.io.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 14:34:12.000000 mod.io-0.5.0/mod.io.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-19 14:34:12.000000 mod.io-0.5.0/mod.io.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 14:34:12.000000 mod.io-0.5.0/mod.io.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 14:34:13.093906 mod.io-0.5.0/modio/
+-rw-rw-rw-   0        0        0      227 2023-06-18 20:41:40.000000 mod.io-0.5.0/modio/__init__.py
+-rw-rw-rw-   0        0        0    26381 2023-06-18 21:07:50.000000 mod.io-0.5.0/modio/client.py
+-rw-rw-rw-   0        0        0    27854 2023-06-18 20:41:40.000000 mod.io-0.5.0/modio/entities.py
+-rw-rw-rw-   0        0        0     6023 2023-06-18 20:41:40.000000 mod.io-0.5.0/modio/enums.py
+-rw-rw-rw-   0        0        0      850 2022-11-26 17:04:58.000000 mod.io-0.5.0/modio/errors.py
+-rw-rw-rw-   0        0        0    20223 2022-11-27 16:57:39.000000 mod.io-0.5.0/modio/game.py
+-rw-rw-rw-   0        0        0     4927 2022-11-27 16:57:39.000000 mod.io-0.5.0/modio/mixins.py
+-rw-rw-rw-   0        0        0    36367 2022-11-26 17:04:58.000000 mod.io-0.5.0/modio/mod.py
+-rw-rw-rw-   0        0        0    16411 2022-11-26 17:04:58.000000 mod.io-0.5.0/modio/objects.py
+-rw-rw-rw-   0        0        0     5585 2023-06-18 21:07:50.000000 mod.io-0.5.0/modio/utils.py
+-rw-rw-rw-   0        0        0      356 2022-11-26 17:04:58.000000 mod.io-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 14:34:13.107907 mod.io-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      797 2023-06-18 21:07:50.000000 mod.io-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 14:34:13.103908 mod.io-0.5.0/tests/
+-rw-rw-rw-   0        0        0     3163 2023-06-18 21:07:50.000000 mod.io-0.5.0/tests/test_client.py
+-rw-rw-rw-   0        0        0     4453 2023-06-18 20:41:40.000000 mod.io-0.5.0/tests/test_game.py
+-rw-rw-rw-   0        0        0     9762 2023-06-18 21:07:50.000000 mod.io-0.5.0/tests/test_mod.py
+-rw-rw-rw-   0        0        0     8241 2023-06-18 21:07:50.000000 mod.io-0.5.0/tests/test_objects.py
```

### Comparing `mod.io-0.4.3b2/LICENSE` & `mod.io-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mod.io-0.4.3b2/PKG-INFO` & `mod.io-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: mod.io
-Version: 0.4.3b2
+Version: 0.5.0
 Summary: mod.io python wrapper
 Home-page: https://github.com/ClementJ18/mod.io
 Author: Clement Julia
 Author-email: clement.julia13@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mod.io
 
 ![mod.io Logo](https://static.mod.io/v1/images/branding/modio-color-dark.png "https://mod.io")
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 
 A wrapper for the mod.io API in Python. 
-* [Docs](https://modio.readthedocs.io/en/latest/) 
+* [Docs](https://modio.readthedocs.io) 
 * [Support](https://discord.gg/Hkq7X7n)
 
-Looking for the async wrapper? [Click here](https://github.com/ClementJ18/mod.io/tree/async)
 
 ## Basic Examples
 ```py
 import modio
 
 client = modio.Client(api_key="your api key here", access_token="your o auth 2 token here")
```

### Comparing `mod.io-0.4.3b2/README.md` & `mod.io-0.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # mod.io
 
 ![mod.io Logo](https://static.mod.io/v1/images/branding/modio-color-dark.png "https://mod.io")
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 
 A wrapper for the mod.io API in Python. 
-* [Docs](https://modio.readthedocs.io/en/latest/) 
+* [Docs](https://modio.readthedocs.io) 
 * [Support](https://discord.gg/Hkq7X7n)
 
-Looking for the async wrapper? [Click here](https://github.com/ClementJ18/mod.io/tree/async)
 
 ## Basic Examples
 ```py
 import modio
 
 client = modio.Client(api_key="your api key here", access_token="your o auth 2 token here")
```

### Comparing `mod.io-0.4.3b2/mod.io.egg-info/PKG-INFO` & `mod.io-0.5.0/mod.io.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: mod.io
-Version: 0.4.3b2
+Version: 0.5.0
 Summary: mod.io python wrapper
 Home-page: https://github.com/ClementJ18/mod.io
 Author: Clement Julia
 Author-email: clement.julia13@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mod.io
 
 ![mod.io Logo](https://static.mod.io/v1/images/branding/modio-color-dark.png "https://mod.io")
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 
 A wrapper for the mod.io API in Python. 
-* [Docs](https://modio.readthedocs.io/en/latest/) 
+* [Docs](https://modio.readthedocs.io) 
 * [Support](https://discord.gg/Hkq7X7n)
 
-Looking for the async wrapper? [Click here](https://github.com/ClementJ18/mod.io/tree/async)
 
 ## Basic Examples
 ```py
 import modio
 
 client = modio.Client(api_key="your api key here", access_token="your o auth 2 token here")
```

### Comparing `mod.io-0.4.3b2/modio/client.py` & `mod.io-0.5.0/modio/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,33 +2,39 @@
 this is where you can get your  games, authentify and get the models for
 your authenticated user.
 """
 import asyncio
 import datetime
 import logging
 import time
+from typing import Optional
 import aiohttp
 import requests
 
+from modio.utils import async_ratelimit_retry, ratelimit_retry
+
 from .errors import modioException
 from .entities import Event, Message, ModFile, Rating, User
+from .enums import TargetPlatform, TargetPortal
 from .objects import Pagination, Returned, Filter
 from .game import Game
 from .mod import Mod
 
 
 class Connection:
     """Class handling under the hood requests and ratelimits."""
 
-    def __init__(self, api_key, access_token, lang, version, test):
+    def __init__(self, api_key, access_token, lang, version, test, platform, portal):
         self.test = test
         self.version = version
         self.access_token = access_token
         self.api_key = api_key
         self.lang = lang
+        self.platform = platform
+        self.portal = portal
 
         self.rate_limit = None
         self.rate_remain = None
         self.retry_after = 0
 
         self.session = requests.Session()
         self._async_session = None
@@ -112,17 +118,23 @@
             # the parameters in the methods below
             headers = {
                 "Accept": "application/json",
                 "Accept-Language": self.lang,
                 "Content-Type": "application/x-www-form-urlencoded",
             }
 
+        if self.platform is not None:
+            headers["X-Modio-Platform"] = self.platform.value
+
+        if self.portal is not None:
+            headers["X-Modio-Portal"] = self.portal.value
+
         return headers
 
-    def _post(self, resp):
+    def _post_process(self, resp):
         try:
             resp_json = resp.json()
         except requests.JSONDecodeError:
             resp_json = {}
 
         try:
             data = self._error_check(resp, resp_json)
@@ -130,40 +142,44 @@
             if e.code == 429:
                 self.enforce_ratelimit()
 
             raise e
 
         return data
 
+    @ratelimit_retry(2)
     def get_request(self, url, *, h_type=0, **fields):
         filters = fields.pop("filters", None)
         filters = (filters or Filter()).get_dict()
 
         extra = {**fields, **filters}
 
         if not self.access_token:
             extra["api_key"] = self.api_key
             h_type = 2
 
         resp = self.session.get(self._base_path + url, headers=self._define_headers(h_type), params=extra)
-        return self._post(resp)
+        return self._post_process(resp)
 
+    @ratelimit_retry(2)
     def post_request(self, url, *, h_type=0, **fields):
         resp = self.session.post(self._base_path + url, headers=self._define_headers(h_type), **fields)
-        return self._post(resp)
+        return self._post_process(resp)
 
+    @ratelimit_retry(2)
     def put_request(self, url, *, h_type=0, **fields):
         resp = self.session.put(self._base_path + url, headers=self._define_headers(h_type), **fields)
-        return self._post(resp)
+        return self._post_process(resp)
 
+    @ratelimit_retry(2)
     def delete_request(self, url, *, h_type=0, **fields):
         resp = self.session.delete(self._base_path + url, headers=self._define_headers(h_type), **fields)
-        return self._post(resp)
+        return self._post_process(resp)
 
-    async def _async_post(self, resp):
+    async def _async_post_process(self, resp):
         try:
             resp_json = await resp.json()
         except aiohttp.ContentTypeError:
             resp_json = {}
 
         try:
             data = self._error_check(resp, resp_json)
@@ -171,29 +187,31 @@
             if e.code == 429:
                 await self.async_enforce_ratelimit()
 
             raise e
 
         return data
 
+    @async_ratelimit_retry(2)
     async def async_get_request(self, url, *, h_type=0, **fields):
         filters = fields.pop("filters", None)
         filters = (filters or Filter()).get_dict()
 
         extra = {**fields, **filters}
 
         if not self.access_token:
             extra["api_key"] = self.api_key
             h_type = 2
 
         async with self.async_session.get(
             self._base_path + url, headers=self._define_headers(h_type), params=extra
         ) as resp:
-            return await self._async_post(resp)
+            return await self._async_post_process(resp)
 
+    @async_ratelimit_retry(2)
     async def async_post_request(self, url, *, h_type=0, **fields):
         files = fields.pop("files", {})
         data = fields.pop("data", {})
 
         form = aiohttp.FormData()
         for key, value in data.items():
             if value is None:
@@ -209,27 +227,29 @@
                 form.add_field(key, value[1], filename=value[0], content_type="multipart/form-data")
             else:
                 form.add_field(key, value, content_type="multipart/form-data")
 
         async with self.async_session.post(
             self._base_path + url, headers=self._define_headers(h_type), data=form
         ) as resp:
-            return await self._async_post(resp)
+            return await self._async_post_process(resp)
 
+    @async_ratelimit_retry(2)
     async def async_put_request(self, url, *, h_type=0, **fields):
         async with self.async_session.put(
             self._base_path + url, headers=self._define_headers(h_type), **fields
         ) as resp:
-            return await self._async_post(resp)
+            return await self._async_post_process(resp)
 
+    @async_ratelimit_retry(2)
     async def async_delete_request(self, url, *, h_type=0, **fields):
         async with self.async_session.delete(
             self._base_path + url, headers=self._define_headers(h_type), **fields
         ) as resp:
-            return await self._async_post(resp)
+            return await self._async_post_process(resp)
 
 
 class Client:
     """Represents an authenticated client to make requests to the mod.io API with. If you desire
     to make aysnc requests you must call :ref:`Client.start` before making any async request.
 
     Parameters
@@ -248,33 +268,48 @@
         responses from the API to be in a particular language, simply provide the lang
         parameter with an ISO 639 compliant language code. Default is US English.
     test : Optional[bool]
         Whether or not to use the mod.io test environment. If not included will default to False.
     version : Optional[str]
         An optional keyword argument to allow you to pick a specific version of the API to query,
         usually you shouldn't need to change this. Default is the latest supported version.
+    platform : Optiona[TargetPlatform]
+        The platform to target with requests.
+    portal : Optional[TargetPortal]
+        The portal to target with requests.
 
     Attributes
     -----------
-    rate_limit : int
-        Number of requests that can be made using the supplied API Key/access token.
-    rate_remain : int
-        Number of requests remaining. Once this number hits 0 the requests will become
-        rejected and the library will sleep until the limit resets then raise 429 TooManyRequests.
     retry_after : int
         Number of seconds until the rate limits are reset for this API Key/access token.
-        Is 0 until the rate_remain is 0 and becomes 0 again once the rate limit is reset.
+        Is 0 until the API returns a 429.
     """
 
-    def __init__(self, *, api_key=None, access_token=None, lang="en", version="v1", test=False):
+    def __init__(
+        self,
+        *,
+        api_key=None,
+        access_token=None,
+        lang="en",
+        version="v1",
+        test=False,
+        platform=None,
+        portal=None,
+    ):
         self.lang = lang
         self.version = version
         self.test = test
         self.connection = Connection(
-            test=test, api_key=api_key, access_token=access_token, version=version, lang=lang
+            test=test,
+            api_key=api_key,
+            access_token=access_token,
+            version=version,
+            lang=lang,
+            platform=platform,
+            portal=portal,
         )
 
     def __repr__(self):
         return f"< Client version={self.version} test={self.test} >"
 
     @property
     def rate_limit(self):
@@ -284,14 +319,36 @@
     def rate_remain(self):
         return self.connection.rate_remain
 
     @property
     def retry_after(self):
         return self.connection.retry_after
 
+    def set_platform(self, platform: Optional[TargetPlatform] = None) -> None:
+        """Change the platform targetted by the client. Call without an argument to not target any specific
+        paltform.
+
+        Parameters
+        -----------
+        platform : Optional[TargetPlatform]
+            The platform to set
+        """
+        self.connection.platform = platform
+
+    def set_portal(self, portal: Optional[TargetPortal] = None) -> None:
+        """Change the portal targetted by the client. Call without an argument to not target any specific
+        portal.
+
+        Parameters
+        -----------
+        portal : Optional[TargetPortal]
+            The portal to set
+        """
+        self.connection.portal = portal
+
     async def close(self):
         """|async| This function is used to clean up the client in order to close the application that it uses gracefully.
         At the moment it is only used to close the client's Session.
 
         |coro|
         """
         await self.connection.close()
```

### Comparing `mod.io-0.4.3b2/modio/entities.py` & `mod.io-0.5.0/modio/entities.py`

 * *Files identical despite different names*

### Comparing `mod.io-0.4.3b2/modio/enums.py` & `mod.io-0.5.0/modio/enums.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,25 +14,42 @@
 
     __str__ = __repr__
 
 
 class TargetPlatform(enum.Enum):
     """Enums for different type of target platforms"""
 
-    windows = enum.auto()
-    mac = enum.auto()
-    linux = enum.auto()
-    android = enum.auto()
-    ios = enum.auto()
-    xboxone = enum.auto()
-    xboxseriesx = enum.auto()
-    ps4 = enum.auto()
-    ps5 = enum.auto()
-    switch = enum.auto()
-    oculus = enum.auto()
+    windows = "Windows"
+    mac = "Mac"
+    linux = "Linux"
+    android = "Android"
+    ios = "iOS"
+    xboxone = "XboxOne"
+    xboxseriesx = "XboxSeriesX"
+    ps4 = "PS4"
+    ps5 = "PS5"
+    switch = "Switch"
+    oculus = "Oculus"
+
+
+class TargetPortal(enum.Enum):
+    """Enums for different type of target portals"""
+
+    apple = "Apply"
+    discord = "Discord"
+    epic = "EGS"
+    facebook = "Facebook"
+    gog = "GOG"
+    google = "Google"
+    itchio = "Itchio"
+    nintendo = "Nintendo"
+    openid = "OpenID"
+    psn = "PSN"
+    steam = "Steam"
+    xboxlive = "XBoxLive"
 
 
 class Status(enum.Enum):
     """Status of the game.
     0 : Not accepted
     1 : Accepted (default)
     2 : Archived (default)
```

### Comparing `mod.io-0.4.3b2/modio/errors.py` & `mod.io-0.5.0/modio/errors.py`

 * *Files identical despite different names*

### Comparing `mod.io-0.4.3b2/modio/game.py` & `mod.io-0.5.0/modio/game.py`

 * *Files identical despite different names*

### Comparing `mod.io-0.4.3b2/modio/mixins.py` & `mod.io-0.5.0/modio/mixins.py`

 * *Files identical despite different names*

### Comparing `mod.io-0.4.3b2/modio/mod.py` & `mod.io-0.5.0/modio/mod.py`

 * *Files identical despite different names*

### Comparing `mod.io-0.4.3b2/modio/objects.py` & `mod.io-0.5.0/modio/objects.py`

 * *Files identical despite different names*

### Comparing `mod.io-0.4.3b2/modio/utils.py` & `mod.io-0.5.0/modio/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """Utility functions for the library"""
+from functools import wraps
 import inspect
 import enum
 import datetime
 
+from modio.errors import modioException
+
 
 def concat_docs(cls):
     """Does it look like I'm enjoying this?"""
     attributes = []
 
     def get_docs(parent):
         nonlocal attributes
@@ -150,7 +153,44 @@
         new_fields[key] = value
 
     return new_fields
 
 
 def _convert_date(time):
     return datetime.datetime.utcfromtimestamp(time)
+
+
+def ratelimit_retry(max_retries):
+    def wrapper(func):
+        @wraps(func)
+        def retry_logic(*args, **kwargs):
+            for _ in range(max_retries):
+                try:
+                    return func(*args, **kwargs)
+                except modioException as e:
+                    if e.code != 429:
+                        raise e
+                    
+                    error = e
+
+            raise error
+
+        return retry_logic
+    return wrapper
+
+def async_ratelimit_retry(max_retries):
+    def wrapper(func):
+        @wraps(func)
+        async def retry_logic(*args, **kwargs):
+            for _ in range(max_retries):
+                try:
+                    return await func(*args, **kwargs)
+                except modioException as e:
+                    if e.code != 429:
+                        raise e
+                    
+                    error = e
+
+            raise error
+
+        return retry_logic
+    return wrapper
```

### Comparing `mod.io-0.4.3b2/setup.py` & `mod.io-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,9 +18,9 @@
     description="mod.io python wrapper",
     author="Clement Julia",
     author_email="clement.julia13@gmail.com",
     url="https://github.com/ClementJ18/mod.io",
     long_description_content_type="text/markdown",
     long_description=readme,
     packages=find_packages(include=["modio", "modio.*"]),
-    install_requires=["aiohttp==3.8.1", "requests==2.28.1", "typing-extensions==4.3.0"],
+    install_requires=["aiohttp==3.8.1", "requests==2.31.0", "typing-extensions==4.3.0"],
 )
```

