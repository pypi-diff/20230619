# Comparing `tmp/pythorhead-0.1.1.tar.gz` & `tmp/pythorhead-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythorhead-0.1.1.tar", last modified: Sun Jun 18 22:07:17 2023, max compression
+gzip compressed data, was "pythorhead-0.2.0.tar", last modified: Mon Jun 19 15:36:06 2023, max compression
```

## Comparing `pythorhead-0.1.1.tar` & `pythorhead-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:07:17.074297 pythorhead-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:07:17.070297 pythorhead-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:07:17.074297 pythorhead-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-18 22:06:55.000000 pythorhead-0.1.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-18 22:06:55.000000 pythorhead-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-18 22:07:00.000000 pythorhead-0.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-18 22:06:55.000000 pythorhead-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40749 2023-06-18 22:07:17.074297 pythorhead-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-18 22:06:55.000000 pythorhead-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-18 22:06:55.000000 pythorhead-0.1.1/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-18 22:07:01.000000 pythorhead-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:07:17.074297 pythorhead-0.1.1/pythorhead/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-18 22:06:55.000000 pythorhead-0.1.1/pythorhead/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-18 22:06:55.000000 pythorhead-0.1.1/pythorhead/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-18 22:06:55.000000 pythorhead-0.1.1/pythorhead/lemmy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-06-18 22:06:55.000000 pythorhead-0.1.1/pythorhead/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:07:17.074297 pythorhead-0.1.1/pythorhead/types/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-18 22:06:55.000000 pythorhead-0.1.1/pythorhead/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-18 22:06:55.000000 pythorhead-0.1.1/pythorhead/types/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-18 22:06:55.000000 pythorhead-0.1.1/pythorhead/types/listing.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-18 22:06:55.000000 pythorhead-0.1.1/pythorhead/types/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:07:17.074297 pythorhead-0.1.1/pythorhead.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40749 2023-06-18 22:07:17.000000 pythorhead-0.1.1/pythorhead.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-18 22:07:17.000000 pythorhead-0.1.1/pythorhead.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 22:07:17.000000 pythorhead-0.1.1/pythorhead.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 22:07:17.000000 pythorhead-0.1.1/pythorhead.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-18 22:06:55.000000 pythorhead-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 22:07:17.074297 pythorhead-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:36:06.477785 pythorhead-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:36:06.473785 pythorhead-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:36:06.473785 pythorhead-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-19 15:35:47.000000 pythorhead-0.2.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-19 15:35:47.000000 pythorhead-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-19 15:35:53.000000 pythorhead-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-19 15:35:47.000000 pythorhead-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40749 2023-06-19 15:36:06.477785 pythorhead-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-19 15:35:47.000000 pythorhead-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-19 15:35:47.000000 pythorhead-0.2.0/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-19 15:35:53.000000 pythorhead-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:36:06.473785 pythorhead-0.2.0/pythorhead/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-19 15:35:47.000000 pythorhead-0.2.0/pythorhead/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-19 15:35:47.000000 pythorhead-0.2.0/pythorhead/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-19 15:35:47.000000 pythorhead-0.2.0/pythorhead/lemmy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-06-19 15:35:47.000000 pythorhead-0.2.0/pythorhead/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-19 15:35:47.000000 pythorhead-0.2.0/pythorhead/requestor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:36:06.477785 pythorhead-0.2.0/pythorhead/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-19 15:35:47.000000 pythorhead-0.2.0/pythorhead/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-19 15:35:47.000000 pythorhead-0.2.0/pythorhead/types/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-19 15:35:47.000000 pythorhead-0.2.0/pythorhead/types/listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-19 15:35:47.000000 pythorhead-0.2.0/pythorhead/types/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:36:06.473785 pythorhead-0.2.0/pythorhead.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40749 2023-06-19 15:36:06.000000 pythorhead-0.2.0/pythorhead.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-19 15:36:06.000000 pythorhead-0.2.0/pythorhead.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:36:06.000000 pythorhead-0.2.0/pythorhead.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-19 15:36:06.000000 pythorhead-0.2.0/pythorhead.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 15:35:47.000000 pythorhead-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 15:36:06.477785 pythorhead-0.2.0/setup.cfg
```

### Comparing `pythorhead-0.1.1/.github/workflows/pypi.yml` & `pythorhead-0.2.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pythorhead-0.1.1/.gitignore` & `pythorhead-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pythorhead-0.1.1/CHANGELOG.md` & `pythorhead-0.2.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # Changelog
 
+## [v0.2.0](https://github.com/db0/pythorhead/tree/v0.2.0) (2023-06-19)
+
+[Full Changelog](https://github.com/db0/pythorhead/compare/v0.1.1...v0.2.0)
+
+**Closed issues:**
+
+- TypeError: unsupported operand type\(s\) for |: 'type' and 'NoneType' [\#5](https://github.com/db0/pythorhead/issues/5)
+
+**Merged pull requests:**
+
+- Requestor class and standard logging [\#10](https://github.com/db0/pythorhead/pull/10) ([NicKoehler](https://github.com/NicKoehler))
+
 ## [v0.1.1](https://github.com/db0/pythorhead/tree/v0.1.1) (2023-06-18)
 
 [Full Changelog](https://github.com/db0/pythorhead/compare/v0.1.0...v0.1.1)
 
 **Merged pull requests:**
 
 - python 3.8 compatible static typing [\#8](https://github.com/db0/pythorhead/pull/8) ([NicKoehler](https://github.com/NicKoehler))
```

### Comparing `pythorhead-0.1.1/LICENSE` & `pythorhead-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pythorhead-0.1.1/PKG-INFO` & `pythorhead-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.1.1
+Version: 0.2.0
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pythorhead-0.1.1/logo.png` & `pythorhead-0.2.0/logo.png`

 * *Files identical despite different names*

### Comparing `pythorhead-0.1.1/pyproject.toml` & `pythorhead-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "pythorhead"
 description = "A python library for interacting with Lemmy API"
 authors = [
     {name = "db0", email = "mail@dbzer0.com"},
 ]
-version = "v0.1.1"
+version = "v0.2.0"
 readme = "README.md"
 requires-python = ">=3.8,<3.11"
 license = { file="LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
```

### Comparing `pythorhead-0.1.1/pythorhead/lemmy.py` & `pythorhead-0.2.0/pythorhead/lemmy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from typing import Optional
+import logging
 
-import requests
-from loguru import logger
+from typing import Optional
 
-from pythorhead.auth import Authentication
 from pythorhead.post import Post
+from pythorhead.requestor import Requestor, Request
+
+logging.basicConfig(format="%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 
 
 class Lemmy:
     post: Post
-    _auth: Authentication
     _known_communities = {}
+    _requestor: Requestor
 
     def __init__(self, api_base_url: str) -> None:
-        self._auth = Authentication()
-        self._auth.api_base_url = f"{api_base_url}/api/v3"
+        self._requestor = Requestor()
+        self._requestor.set_api_base_url(f"{api_base_url}/api/v3")
         self.post = Post()
 
     def log_in(self, username_or_email: str, password: str) -> bool:
-        return Authentication().log_in(username_or_email, password)
+        return self._requestor.log_in(username_or_email, password)
 
     def discover_community(self, community_name: str) -> Optional[int]:
         if community_name in self._known_communities:
             return self._known_communities[community_name]
-        try:
-            req = requests.get(f"{self._auth.api_base_url}/community?name={community_name}")
-            community_id = req.json()["community_view"]["community"]["id"]
+
+        request = self._requestor.request(Request.GET, "/community", params={"name": community_name})
+
+        if request is not None:
+            community_id = request["community_view"]["community"]["id"]
             self._known_communities[community_name] = community_id
-        except Exception as err:
-            logger.error(f"Error when looking up community '{community_name}': {err}")
-            return
-        return community_id
+            return community_id
```

### Comparing `pythorhead-0.1.1/pythorhead.egg-info/PKG-INFO` & `pythorhead-0.2.0/pythorhead.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.1.1
+Version: 0.2.0
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

