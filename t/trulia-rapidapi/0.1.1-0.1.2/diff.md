# Comparing `tmp/trulia_rapidapi-0.1.1.tar.gz` & `tmp/trulia_rapidapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trulia_rapidapi-0.1.1.tar", last modified: Sat Jun 17 09:38:53 2023, max compression
+gzip compressed data, was "trulia_rapidapi-0.1.2.tar", last modified: Mon Jun 19 20:01:09 2023, max compression
```

## Comparing `trulia_rapidapi-0.1.1.tar` & `trulia_rapidapi-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 09:38:53.923941 trulia_rapidapi-0.1.1/
--rw-rw-rw-   0        0        0     1848 2023-06-17 09:38:53.923941 trulia_rapidapi-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1232 2023-06-14 20:14:23.000000 trulia_rapidapi-0.1.1/README.md
--rw-rw-rw-   0        0        0      399 2023-06-17 09:38:53.925942 trulia_rapidapi-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      625 2023-06-17 09:36:05.000000 trulia_rapidapi-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 09:38:53.902941 trulia_rapidapi-0.1.1/trulia_rapidapi/
-drwxrwxrwx   0        0        0        0 2023-06-17 09:38:53.918940 trulia_rapidapi-0.1.1/trulia_rapidapi/src/
--rw-rw-rw-   0        0        0     6458 2023-06-17 08:53:53.000000 trulia_rapidapi-0.1.1/trulia_rapidapi/src/trulia_api.py
-drwxrwxrwx   0        0        0        0 2023-06-17 09:38:53.922941 trulia_rapidapi-0.1.1/trulia_rapidapi/src/trulia_models/
--rw-rw-rw-   0        0        0      110 2023-05-24 11:23:07.000000 trulia_rapidapi-0.1.1/trulia_rapidapi/src/trulia_models/base.py
--rw-rw-rw-   0        0        0     3175 2023-06-14 19:13:10.000000 trulia_rapidapi-0.1.1/trulia_rapidapi/src/trulia_models/enums.py
--rw-rw-rw-   0        0        0     1497 2023-06-14 18:52:49.000000 trulia_rapidapi-0.1.1/trulia_rapidapi/src/trulia_models/listing_model.py
--rw-rw-rw-   0        0        0      539 2023-06-14 19:49:05.000000 trulia_rapidapi-0.1.1/trulia_rapidapi/src/trulia_models/search_token_model.py
-drwxrwxrwx   0        0        0        0 2023-06-17 09:38:53.917944 trulia_rapidapi-0.1.1/trulia_rapidapi.egg-info/
--rw-rw-rw-   0        0        0     1848 2023-06-17 09:38:53.000000 trulia_rapidapi-0.1.1/trulia_rapidapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-06-17 09:38:53.000000 trulia_rapidapi-0.1.1/trulia_rapidapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 09:38:53.000000 trulia_rapidapi-0.1.1/trulia_rapidapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-14 20:08:36.000000 trulia_rapidapi-0.1.1/trulia_rapidapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-06-17 09:38:53.000000 trulia_rapidapi-0.1.1/trulia_rapidapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 20:01:09.254065 trulia_rapidapi-0.1.2/
+-rw-rw-rw-   0        0        0     1848 2023-06-19 20:01:09.254065 trulia_rapidapi-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1232 2023-06-14 20:14:23.000000 trulia_rapidapi-0.1.2/README.md
+-rw-rw-rw-   0        0        0      399 2023-06-19 20:01:09.257067 trulia_rapidapi-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      625 2023-06-19 20:00:46.000000 trulia_rapidapi-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:01:09.211466 trulia_rapidapi-0.1.2/trulia_rapidapi/
+drwxrwxrwx   0        0        0        0 2023-06-19 20:01:09.243458 trulia_rapidapi-0.1.2/trulia_rapidapi/src/
+-rw-rw-rw-   0        0        0     6879 2023-06-19 19:59:49.000000 trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_api.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:01:09.253071 trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_models/
+-rw-rw-rw-   0        0        0      110 2023-05-24 11:23:07.000000 trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_models/base.py
+-rw-rw-rw-   0        0        0     3207 2023-06-19 19:54:24.000000 trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_models/details_model.py
+-rw-rw-rw-   0        0        0     3175 2023-06-14 19:13:10.000000 trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_models/enums.py
+-rw-rw-rw-   0        0        0     1497 2023-06-14 18:52:49.000000 trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_models/listing_model.py
+-rw-rw-rw-   0        0        0      539 2023-06-14 19:49:05.000000 trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_models/search_token_model.py
+-rw-rw-rw-   0        0        0     2113 2023-06-19 19:58:43.000000 trulia_rapidapi-0.1.2/trulia_rapidapi/tests.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:01:09.241459 trulia_rapidapi-0.1.2/trulia_rapidapi.egg-info/
+-rw-rw-rw-   0        0        0     1848 2023-06-19 20:01:09.000000 trulia_rapidapi-0.1.2/trulia_rapidapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      524 2023-06-19 20:01:09.000000 trulia_rapidapi-0.1.2/trulia_rapidapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 20:01:09.000000 trulia_rapidapi-0.1.2/trulia_rapidapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-14 20:08:36.000000 trulia_rapidapi-0.1.2/trulia_rapidapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2023-06-19 20:01:09.000000 trulia_rapidapi-0.1.2/trulia_rapidapi.egg-info/top_level.txt
```

### Comparing `trulia_rapidapi-0.1.1/PKG-INFO` & `trulia_rapidapi-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trulia_rapidapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Trulia Real Estate API on RapidAPI
 Home-page: https://letsscrape.com/scrapers/trulia-real-estate-api/
 Author: LetsScrape
 Author-email: hello@letsscrape.com
 Project-URL: Documentation, https://rapidapi.com/letsscrape/api/trulia-real-estate-scraper/
 Project-URL: Bug Reports, https://github.com/letsscrape/python_trulia_rapidapi/issues
 Project-URL: Source Code, https://github.com/letsscrape/python_trulia_rapidapi
```

### Comparing `trulia_rapidapi-0.1.1/README.md` & `trulia_rapidapi-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `trulia_rapidapi-0.1.1/setup.py` & `trulia_rapidapi-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='trulia_rapidapi',
-    version='0.1.1',
+    version='0.1.2',
     description='Trulia Real Estate API on RapidAPI',
     packages=['trulia_rapidapi', 'trulia_rapidapi.src', 'trulia_rapidapi.src.trulia_models'],
     author_email='hello@letsscrape.com',
     zip_safe=False,
     author='LetsScrape',
     keywords=['trulia', 'real estate api', 'trulia real estate', 'trulia api', 'parsing', 'scraper'],
     classifiers=[],
```

### Comparing `trulia_rapidapi-0.1.1/trulia_rapidapi/src/trulia_api.py` & `trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from urllib.parse import urlencode
 from purl import URL
 import aiohttp
 
 from src.trulia_models.enums import *
 from src.trulia_models.listing_model import ListingModel
 from src.trulia_models.search_token_model import SearchTokenModel
+from src.trulia_models.details_model import DetailsModel
 
 
 
 class TruliaAPI(object):
     def __init__(self, rapid_api_key: AnyStr):
         """
         To obtain your rapid_api key, you first need to sign up on RapidAPI. You can do so by visiting this link: https://rapidapi.com/auth/sign-up.
@@ -51,26 +52,26 @@
         is_ok = False
 
         while True:
             async with aiohttp.ClientSession(headers=self.headers, timeout=session_timeout) as session:
                 async with session.get(url=url) as response:
                     try:
                         json_response = await response.json()  
-                        if response.status == 200:  
+                        print(response)
+                        if response.status == 200 or response.status == 400:  
                             is_ok = True
                     except aiohttp.client.ContentTypeError:
                         continue
                     if is_ok:
                         break
             await asyncio.sleep(0.3)
 
         return json_response
     
-    async def __wait(self):
-        await asyncio.sleep(1)
+
 
     async def get_search_token(self, search_type: TruliaSearchType, place: str) -> SearchTokenModel:
         """
         This function generates a token (or tokens in some cases) based on the variable {place}.
         For example, if we pass a part of {place} instead of 'Scottsdale', say 'Scot', we'll receive 
         several tokens along with the matched {places}, from which we can select the token to use
         in the search_by_token function.
@@ -126,8 +127,17 @@
         Parameters:
         page (int): The page number you want to work with. If you want the first page, pass in 1.
         """
         path = f"/search/{search_type}?search_token={token}&page={page}&sort={sort}&beds={beds}&min_price={min_price}&max_price={max_price}&house_type={house_type}&for_sale_by_agent={for_sale_by_agent}&for_sale_by_owner={for_sale_by_owner}&new_construction={new_construction}"
         path = path.replace('=None', '=')
         response_data = await self.__get_request(path=path)
         response = ListingModel.parse_obj(response_data)
+        return response
+    
+    async def details_by_url(self, url:str) -> DetailsModel:
+        """
+        Returns home details by url from https://www.trulia.com/
+        """
+        path = f"/homes/details_by_url?url={url}"
+        response_data = await self.__get_request(path=path)
+        response = DetailsModel.parse_obj(response_data)
         return response
```

### Comparing `trulia_rapidapi-0.1.1/trulia_rapidapi/src/trulia_models/enums.py` & `trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_models/enums.py`

 * *Files identical despite different names*

### Comparing `trulia_rapidapi-0.1.1/trulia_rapidapi/src/trulia_models/listing_model.py` & `trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_models/listing_model.py`

 * *Files identical despite different names*

### Comparing `trulia_rapidapi-0.1.1/trulia_rapidapi/src/trulia_models/search_token_model.py` & `trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_models/search_token_model.py`

 * *Files identical despite different names*

### Comparing `trulia_rapidapi-0.1.1/trulia_rapidapi.egg-info/PKG-INFO` & `trulia_rapidapi-0.1.2/trulia_rapidapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trulia-rapidapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Trulia Real Estate API on RapidAPI
 Home-page: https://letsscrape.com/scrapers/trulia-real-estate-api/
 Author: LetsScrape
 Author-email: hello@letsscrape.com
 Project-URL: Documentation, https://rapidapi.com/letsscrape/api/trulia-real-estate-scraper/
 Project-URL: Bug Reports, https://github.com/letsscrape/python_trulia_rapidapi/issues
 Project-URL: Source Code, https://github.com/letsscrape/python_trulia_rapidapi
```

