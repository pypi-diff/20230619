# Comparing `tmp/sixth-python-0.0.6.tar.gz` & `tmp/sixth-python-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sixth-python-0.0.6.tar", last modified: Mon Jun 19 18:10:59 2023, max compression
+gzip compressed data, was "dist/sixth-python-0.0.7.tar", last modified: Mon Jun 19 19:58:09 2023, max compression
```

## Comparing `sixth-python-0.0.6.tar` & `sixth-python-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-19 18:10:59.000000 sixth-python-0.0.6/
--rw-r--r--   0 mac        (501) staff       (20)     3114 2023-06-19 18:10:59.000000 sixth-python-0.0.6/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1909 2023-06-19 18:09:44.000000 sixth-python-0.0.6/README.md
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-19 18:10:59.000000 sixth-python-0.0.6/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     3773 2023-06-19 18:10:41.000000 sixth-python-0.0.6/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-19 18:10:59.000000 sixth-python-0.0.6/sixth/
--rw-r--r--   0 mac        (501) staff       (20)       32 2023-06-17 23:23:30.000000 sixth-python-0.0.6/sixth/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-19 18:10:59.000000 sixth-python-0.0.6/sixth/middlewares/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-python-0.0.6/sixth/middlewares/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3693 2023-06-19 15:43:56.000000 sixth-python-0.0.6/sixth/middlewares/encryption_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-python-0.0.6/sixth/middlewares/six_base_http_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     3919 2023-06-19 15:43:56.000000 sixth-python-0.0.6/sixth/middlewares/six_independent_rate_limiter.py
--rw-r--r--   0 mac        (501) staff       (20)     4387 2023-06-19 16:09:16.000000 sixth-python-0.0.6/sixth/middlewares/six_rate_limiter_middleware.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-19 18:10:59.000000 sixth-python-0.0.6/sixth/pen_test/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-12 15:04:45.000000 sixth-python-0.0.6/sixth/pen_test/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      165 2023-06-14 20:44:10.000000 sixth-python-0.0.6/sixth/pen_test/auto_pen_test.py
--rw-r--r--   0 mac        (501) staff       (20)      850 2023-06-19 15:54:59.000000 sixth-python-0.0.6/sixth/schemas.py
--rw-r--r--   0 mac        (501) staff       (20)     4155 2023-06-19 15:43:56.000000 sixth-python-0.0.6/sixth/sdk.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-19 18:10:59.000000 sixth-python-0.0.6/sixth/utils/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-python-0.0.6/sixth/utils/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-python-0.0.6/sixth/utils/encryption_utils.py
--rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-python-0.0.6/sixth/utils/time_utils.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-19 18:10:59.000000 sixth-python-0.0.6/sixth_python.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     3114 2023-06-19 18:10:59.000000 sixth-python-0.0.6/sixth_python.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      604 2023-06-19 18:10:59.000000 sixth-python-0.0.6/sixth_python.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-19 18:10:59.000000 sixth-python-0.0.6/sixth_python.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      610 2023-06-19 18:10:59.000000 sixth-python-0.0.6/sixth_python.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        6 2023-06-19 18:10:59.000000 sixth-python-0.0.6/sixth_python.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-19 19:58:09.000000 sixth-python-0.0.7/
+-rw-r--r--   0 mac        (501) staff       (20)     3117 2023-06-19 19:58:09.000000 sixth-python-0.0.7/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1909 2023-06-19 18:09:44.000000 sixth-python-0.0.7/README.md
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-19 19:58:09.000000 sixth-python-0.0.7/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     3776 2023-06-19 19:57:52.000000 sixth-python-0.0.7/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-19 19:58:09.000000 sixth-python-0.0.7/sixth/
+-rw-r--r--   0 mac        (501) staff       (20)       32 2023-06-17 23:23:30.000000 sixth-python-0.0.7/sixth/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-19 19:58:09.000000 sixth-python-0.0.7/sixth/middlewares/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-python-0.0.7/sixth/middlewares/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3703 2023-06-19 19:50:08.000000 sixth-python-0.0.7/sixth/middlewares/encryption_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-python-0.0.7/sixth/middlewares/six_base_http_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     3924 2023-06-19 19:50:08.000000 sixth-python-0.0.7/sixth/middlewares/six_independent_rate_limiter.py
+-rw-r--r--   0 mac        (501) staff       (20)     4392 2023-06-19 19:50:08.000000 sixth-python-0.0.7/sixth/middlewares/six_rate_limiter_middleware.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-19 19:58:09.000000 sixth-python-0.0.7/sixth/pen_test/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-12 15:04:45.000000 sixth-python-0.0.7/sixth/pen_test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      165 2023-06-14 20:44:10.000000 sixth-python-0.0.7/sixth/pen_test/auto_pen_test.py
+-rw-r--r--   0 mac        (501) staff       (20)      850 2023-06-19 15:54:59.000000 sixth-python-0.0.7/sixth/schemas.py
+-rw-r--r--   0 mac        (501) staff       (20)     4165 2023-06-19 19:50:08.000000 sixth-python-0.0.7/sixth/sdk.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-19 19:58:09.000000 sixth-python-0.0.7/sixth/utils/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-python-0.0.7/sixth/utils/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-python-0.0.7/sixth/utils/encryption_utils.py
+-rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-python-0.0.7/sixth/utils/time_utils.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-19 19:58:09.000000 sixth-python-0.0.7/sixth_python.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     3117 2023-06-19 19:58:09.000000 sixth-python-0.0.7/sixth_python.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      604 2023-06-19 19:58:09.000000 sixth-python-0.0.7/sixth_python.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-19 19:58:09.000000 sixth-python-0.0.7/sixth_python.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      610 2023-06-19 19:58:09.000000 sixth-python-0.0.7/sixth_python.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        6 2023-06-19 19:58:09.000000 sixth-python-0.0.7/sixth_python.egg-info/top_level.txt
```

### Comparing `sixth-python-0.0.6/PKG-INFO` & `sixth-python-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: sixth-python
-Version: 0.0.6
-Summary: Six offical python ackage
+Version: 0.0.7
+Summary: Six offical python package
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: 
         # **Sixth**
         
         
         [![N|Solid](https://firebasestorage.googleapis.com/v0/b/test-103bf.appspot.com/o/waves.png?alt=media&token=0fa4c489-d9c9-4a3b-9178-593b2b018613)](https://nodesource.com/products/nsolid)
         
-        Six helps you proactively identify security vulnerabilities and prevent cyberattacks on your system that could cost you millions of dollars.
+        Sixth helps you proactively identify security vulnerabilities and prevent cyberattacks on your system that could cost you millions of dollars.
         
         
         
         ## Features
         
         - Automated Penetration Testing
         - End to End encryption of data
```

### Comparing `sixth-python-0.0.6/README.md` & `sixth-python-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.6/setup.py` & `sixth-python-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 from pip._internal.req import parse_requirements
 
 
 
 
-VERSION = '0.0.6'
-DESCRIPTION = 'Six offical python ackage'
+VERSION = '0.0.7'
+DESCRIPTION = 'Six offical python package'
 LONG_DESCRIPTION = '''
 # **Sixth**
 
 
 [![N|Solid](https://firebasestorage.googleapis.com/v0/b/test-103bf.appspot.com/o/waves.png?alt=media&token=0fa4c489-d9c9-4a3b-9178-593b2b018613)](https://nodesource.com/products/nsolid)
 
-Six helps you proactively identify security vulnerabilities and prevent cyberattacks on your system that could cost you millions of dollars.
+Sixth helps you proactively identify security vulnerabilities and prevent cyberattacks on your system that could cost you millions of dollars.
 
 
 
 ## Features
 
 - Automated Penetration Testing
 - End to End encryption of data
```

### Comparing `sixth-python-0.0.6/sixth/middlewares/encryption_middleware.py` & `sixth-python-0.0.7/sixth/middlewares/encryption_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     
 
     async def dispatch(self,request: Request,call_next) -> None:
 
         req_body = await request.body()
         await self.set_body(request, req_body)
         req_body =await self._parse_bools(req_body)
-        private_key_request = requests.post("http://127.0.0.1:8000/encryption-service/get-user-private_key", data=json.dumps({
+        private_key_request = requests.post("https://backend.withsix.co/encryption-service/get-user-private_key", data=json.dumps({
             "apiKey": self._apikey
         }))
         if private_key_request.status_code == 200:
             private_key_url = private_key_request.json()["data"]["private_key"]
             private_key_txt = requests.get(private_key_url)
             data = private_key_txt.text
             if type(req_body) == str:
@@ -60,15 +60,15 @@
             except Exception as e:
                 raise HTTPException(401, {"Unauthorized":e})
             
 
         response = await call_next(200, output, headers)
         resp_body = response.body
         resp_body = await self._parse_bools(resp_body)
-        public_key_request = requests.post("http://127.0.0.1:8000/encryption-service/get-user-public-key", data=json.dumps({
+        public_key_request = requests.post("https://backend.withsix.co/encryption-service/get-user-public-key", data=json.dumps({
             "apiKey": self._apikey
         }))
         if public_key_request.status_code == 200:
             public_key_url = public_key_request.json()["data"]["public_key"]
             public_key_txt = requests.get(public_key_url)
             data = public_key_txt.text
             if type(resp_body) == str:
```

### Comparing `sixth-python-0.0.6/sixth/middlewares/six_base_http_middleware.py` & `sixth-python-0.0.7/sixth/middlewares/six_base_http_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.6/sixth/middlewares/six_independent_rate_limiter.py` & `sixth-python-0.0.7/sixth/middlewares/six_independent_rate_limiter.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         return out
         
     async def dispatch(self,request: Request,call_next) -> None:
         
         host = request.client.host
         route = request.scope["path"]
         route = re.sub(r'\W+', '~', route)
-        rate_limit_resp = requests.get("http://127.0.0.1:8000/project-config/config/get-route-rate-limit/"+self._apikey+"/"+route)
+        rate_limit_resp = requests.get("https://backend.withsix.co/project-config/config/get-route-rate-limit/"+self._apikey+"/"+route)
         body = await request.body()
         await self.set_body(request, body)
         body = await self._parse_bools(body)
         
 
         if rate_limit_resp.status_code == 200:
             rate_limit = schemas.RateLimiter.parse_obj(rate_limit_resp.json())
```

### Comparing `sixth-python-0.0.6/sixth/middlewares/six_rate_limiter_middleware.py` & `sixth-python-0.0.7/sixth/middlewares/six_rate_limiter_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         out=ast.literal_eval(string)
         return out
         
     async def dispatch(self,request: Request,call_next) -> None:
         host = request.client.host
         route = request.scope["path"]
         route = re.sub(r'\W+', '~', route)
-        rate_limit_resp = requests.get("http://127.0.0.1:8000/project-config/config/get-route-rate-limit/"+self._apikey+"/"+route)
+        rate_limit_resp = requests.get("https://backend.withsix.co/project-config/config/get-route-rate-limit/"+self._apikey+"/"+route)
         if rate_limit_resp.status_code == 200:
             rate_limit = schemas.RateLimiter.parse_obj(rate_limit_resp.json())
             self._config.rate_limiter[route] = rate_limit
             preferred_id = host if self._config.rate_limiter[route].unique_id == "" or self._config.rate_limiter[route].unique_id == "host" else self._config.rate_limiter[route].unique_id
             _response = await call_next(request)
             if self._is_rate_limit_reached(preferred_id, route): 
                 return _response
```

### Comparing `sixth-python-0.0.6/sixth/schemas.py` & `sixth-python-0.0.7/sixth/schemas.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.6/sixth/sdk.py` & `sixth-python-0.0.7/sixth/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 class SixthSense():
     def __init__(self, apikey: str, app: FastAPI):
         self._apikey = apikey
         self._app = app 
 
     def init(self):
-        _base_url = "http://127.0.0.1:8000"
+        _base_url = "https://backend.withsix.co"
         _project_config_resp = requests.get(_base_url+"/project-config/config/"+self._apikey)
         # get the user's project config
         try:
             if _project_config_resp.status_code == 200:
                 _config: schemas.ProjectConfig = schemas.ProjectConfig.parse_obj(dict(_project_config_resp.json()))
                 self._sync_project_route(_config)
             else:
@@ -70,15 +70,15 @@
             encryption = schemas.Encryption(public_key="dummy",private_key="dummy", use_count=0, last_updated=0,created_at=0), 
             base_url = "op",
             last_updated=get_time_now(), 
             created_at=get_time_now(), 
             encryption_enabled=config.encryption_enabled if config != None else False, 
             rate_limiter_enabled=config.rate_limiter_enabled if config != None else True
         )
-        _base_url = "http://127.0.0.1:8000"
+        _base_url = "https://backend.withsix.co"
         _project_config_resp = requests.post(_base_url+"/project-config/config/sync-user-config", json=_config.dict())
         if _project_config_resp.status_code == status.HTTP_200_OK:
             return _config
         else: 
             return _config
```

### Comparing `sixth-python-0.0.6/sixth/utils/encryption_utils.py` & `sixth-python-0.0.7/sixth/utils/encryption_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.6/sixth/utils/time_utils.py` & `sixth-python-0.0.7/sixth/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.6/sixth_python.egg-info/PKG-INFO` & `sixth-python-0.0.7/sixth_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: sixth-python
-Version: 0.0.6
-Summary: Six offical python ackage
+Version: 0.0.7
+Summary: Six offical python package
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: 
         # **Sixth**
         
         
         [![N|Solid](https://firebasestorage.googleapis.com/v0/b/test-103bf.appspot.com/o/waves.png?alt=media&token=0fa4c489-d9c9-4a3b-9178-593b2b018613)](https://nodesource.com/products/nsolid)
         
-        Six helps you proactively identify security vulnerabilities and prevent cyberattacks on your system that could cost you millions of dollars.
+        Sixth helps you proactively identify security vulnerabilities and prevent cyberattacks on your system that could cost you millions of dollars.
         
         
         
         ## Features
         
         - Automated Penetration Testing
         - End to End encryption of data
```

### Comparing `sixth-python-0.0.6/sixth_python.egg-info/SOURCES.txt` & `sixth-python-0.0.7/sixth_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.6/sixth_python.egg-info/requires.txt` & `sixth-python-0.0.7/sixth_python.egg-info/requires.txt`

 * *Files identical despite different names*

