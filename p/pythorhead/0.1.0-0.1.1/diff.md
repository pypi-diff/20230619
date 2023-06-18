# Comparing `tmp/pythorhead-0.1.0.tar.gz` & `tmp/pythorhead-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythorhead-0.1.0.tar", last modified: Fri Jun 16 13:14:09 2023, max compression
+gzip compressed data, was "pythorhead-0.1.1.tar", last modified: Sun Jun 18 22:07:17 2023, max compression
```

## Comparing `pythorhead-0.1.0.tar` & `pythorhead-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:14:09.796255 pythorhead-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:14:09.796255 pythorhead-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:14:09.796255 pythorhead-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-16 13:13:50.000000 pythorhead-0.1.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-16 13:13:50.000000 pythorhead-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-16 13:13:56.000000 pythorhead-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 13:13:50.000000 pythorhead-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40749 2023-06-16 13:14:09.796255 pythorhead-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-16 13:13:50.000000 pythorhead-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-16 13:13:50.000000 pythorhead-0.1.0/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-16 13:13:56.000000 pythorhead-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:14:09.796255 pythorhead-0.1.0/pythorhead/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 13:13:50.000000 pythorhead-0.1.0/pythorhead/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-16 13:13:50.000000 pythorhead-0.1.0/pythorhead/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-16 13:13:50.000000 pythorhead-0.1.0/pythorhead/lemmy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-06-16 13:13:50.000000 pythorhead-0.1.0/pythorhead/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:14:09.796255 pythorhead-0.1.0/pythorhead/types/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-16 13:13:50.000000 pythorhead-0.1.0/pythorhead/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-16 13:13:50.000000 pythorhead-0.1.0/pythorhead/types/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-16 13:13:50.000000 pythorhead-0.1.0/pythorhead/types/listing.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-16 13:13:50.000000 pythorhead-0.1.0/pythorhead/types/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:14:09.796255 pythorhead-0.1.0/pythorhead.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40749 2023-06-16 13:14:09.000000 pythorhead-0.1.0/pythorhead.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-16 13:14:09.000000 pythorhead-0.1.0/pythorhead.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:14:09.000000 pythorhead-0.1.0/pythorhead.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 13:14:09.000000 pythorhead-0.1.0/pythorhead.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 13:13:50.000000 pythorhead-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 13:14:09.796255 pythorhead-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:07:17.074297 pythorhead-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:07:17.070297 pythorhead-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:07:17.074297 pythorhead-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-18 22:06:55.000000 pythorhead-0.1.1/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-18 22:06:55.000000 pythorhead-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-18 22:07:00.000000 pythorhead-0.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-18 22:06:55.000000 pythorhead-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40749 2023-06-18 22:07:17.074297 pythorhead-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-18 22:06:55.000000 pythorhead-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-18 22:06:55.000000 pythorhead-0.1.1/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-18 22:07:01.000000 pythorhead-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:07:17.074297 pythorhead-0.1.1/pythorhead/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-18 22:06:55.000000 pythorhead-0.1.1/pythorhead/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-18 22:06:55.000000 pythorhead-0.1.1/pythorhead/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-18 22:06:55.000000 pythorhead-0.1.1/pythorhead/lemmy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-06-18 22:06:55.000000 pythorhead-0.1.1/pythorhead/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:07:17.074297 pythorhead-0.1.1/pythorhead/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-18 22:06:55.000000 pythorhead-0.1.1/pythorhead/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-18 22:06:55.000000 pythorhead-0.1.1/pythorhead/types/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-18 22:06:55.000000 pythorhead-0.1.1/pythorhead/types/listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-18 22:06:55.000000 pythorhead-0.1.1/pythorhead/types/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:07:17.074297 pythorhead-0.1.1/pythorhead.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40749 2023-06-18 22:07:17.000000 pythorhead-0.1.1/pythorhead.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-18 22:07:17.000000 pythorhead-0.1.1/pythorhead.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 22:07:17.000000 pythorhead-0.1.1/pythorhead.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 22:07:17.000000 pythorhead-0.1.1/pythorhead.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-18 22:06:55.000000 pythorhead-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 22:07:17.074297 pythorhead-0.1.1/setup.cfg
```

### Comparing `pythorhead-0.1.0/.github/workflows/pypi.yml` & `pythorhead-0.1.1/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pythorhead-0.1.0/.gitignore` & `pythorhead-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pythorhead-0.1.0/CHANGELOG.md` & `pythorhead-0.1.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## [v0.1.1](https://github.com/db0/pythorhead/tree/v0.1.1) (2023-06-18)
+
+[Full Changelog](https://github.com/db0/pythorhead/compare/v0.1.0...v0.1.1)
+
+**Merged pull requests:**
+
+- python 3.8 compatible static typing [\#8](https://github.com/db0/pythorhead/pull/8) ([NicKoehler](https://github.com/NicKoehler))
+- Update pyproject.toml to specify minimum python 3.10 [\#7](https://github.com/db0/pythorhead/pull/7) ([tanitna](https://github.com/tanitna))
+- Add SO attribution [\#4](https://github.com/db0/pythorhead/pull/4) ([JodanJodan](https://github.com/JodanJodan))
+
 ## [v0.1.0](https://github.com/db0/pythorhead/tree/v0.1.0) (2023-06-16)
 
 [Full Changelog](https://github.com/db0/pythorhead/compare/v0.0.5...v0.1.0)
 
 **Merged pull requests:**
 
 - Refactoring [\#3](https://github.com/db0/pythorhead/pull/3) ([NicKoehler](https://github.com/NicKoehler))
```

### Comparing `pythorhead-0.1.0/LICENSE` & `pythorhead-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pythorhead-0.1.0/PKG-INFO` & `pythorhead-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pythorhead-0.1.0/logo.png` & `pythorhead-0.1.1/logo.png`

 * *Files identical despite different names*

### Comparing `pythorhead-0.1.0/pyproject.toml` & `pythorhead-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "pythorhead"
 description = "A python library for interacting with Lemmy API"
 authors = [
     {name = "db0", email = "mail@dbzer0.com"},
 ]
-version = "v0.1.0"
+version = "v0.1.1"
 readme = "README.md"
 requires-python = ">=3.8,<3.11"
 license = { file="LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
```

### Comparing `pythorhead-0.1.0/pythorhead/auth.py` & `pythorhead-0.1.1/pythorhead/auth.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+from typing import Optional
+
 import requests
 from loguru import logger
 
 
+# Stack Overflow: Creating a singleton in Python
+# https://stackoverflow.com/q/6760685
+# CC BY-SA 3.0
 class Singleton(type):
     _instances = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
             cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
         return cls._instances[cls]
 
 
 class Authentication(metaclass=Singleton):
-    token: str | None = None
-    api_base_url: str | None = None
+    token: Optional[str] = None
+    api_base_url: Optional[str] = None
 
     def log_in(self, username_or_email: str, password: str) -> bool:
         payload = {
             "username_or_email": username_or_email,
             "password": password,
         }
         try:
```

### Comparing `pythorhead-0.1.0/pythorhead/lemmy.py` & `pythorhead-0.1.1/pythorhead/lemmy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 import requests
 from loguru import logger
 
 from pythorhead.auth import Authentication
 from pythorhead.post import Post
 
 
@@ -14,15 +16,15 @@
         self._auth = Authentication()
         self._auth.api_base_url = f"{api_base_url}/api/v3"
         self.post = Post()
 
     def log_in(self, username_or_email: str, password: str) -> bool:
         return Authentication().log_in(username_or_email, password)
 
-    def discover_community(self, community_name: str) -> int | None:
+    def discover_community(self, community_name: str) -> Optional[int]:
         if community_name in self._known_communities:
             return self._known_communities[community_name]
         try:
             req = requests.get(f"{self._auth.api_base_url}/community?name={community_name}")
             community_id = req.json()["community_view"]["community"]["id"]
             self._known_communities[community_name] = community_id
         except Exception as err:
```

### Comparing `pythorhead-0.1.0/pythorhead/post.py` & `pythorhead-0.1.1/pythorhead/post.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Literal
+from typing import Any, Literal, Optional, List
 
 import requests
 from loguru import logger
 
 from pythorhead.auth import Authentication
 from pythorhead.types import FeatureType, ListingType, SortType
 
@@ -10,15 +10,15 @@
 class Post:
     def __init__(self):
         self._auth = Authentication()
 
     def get(
         self,
         post_id: int,
-        comment_id: int | None = None,
+        comment_id: Optional[int] = None,
     ) -> dict:
         """
         Get a post.
 
         Args:
             post_id (int)
             comment_id (int, optional) Defaults to None.
@@ -38,22 +38,22 @@
         if not re.ok:
             logger.error(f"Error encountered while getting posts: {re.text}")
             return {}
         return re.json()
 
     def list(  # noqa: A003
         self,
-        community_id: int | None = None,
-        community_name: str | None = None,
-        limit: int | None = None,
-        page: int | None = None,
-        saved_only: bool | None = None,
-        sort: SortType | None = None,
-        type_: ListingType | None = None,
-    ) -> list[dict]:
+        community_id: Optional[int] = None,
+        community_name: Optional[str] = None,
+        limit: Optional[int] = None,
+        page: Optional[int] = None,
+        saved_only: Optional[bool] = None,
+        sort: Optional[SortType] = None,
+        type_: Optional[ListingType] = None,
+    ) -> List[dict]:
         """
 
         Get posts, with various filters.
 
         Args:
             community_id (int, optional): Defaults to None.
             community_name (str, optional): Defaults to None.
@@ -91,19 +91,19 @@
             return []
         return re.json()["posts"]
 
     def create(
         self,
         community_id: int,
         name: str,
-        url: str | None = None,
-        body: str | None = None,
-        nsfw: bool | None = None,
-        honeypot: str | None = None,
-        language_id: int | None = None,
+        url: Optional[str] = None,
+        body: Optional[str] = None,
+        nsfw: Optional[bool] = None,
+        honeypot: Optional[str] = None,
+        language_id: Optional[int] = None,
     ) -> bool:
         """
         Create a post
 
         Args:
             community_id (int)
             name (str)
@@ -157,15 +157,15 @@
             "deleted": deleted,
         }
         re = requests.post(f"{self._auth.api_base_url}/post/delete", json=delete_post)
         if not re.ok:
             logger.error(f"Error encountered while deleting post: {re.text}")
         return re.ok
 
-    def remove(self, post_id: int, removed: bool, reason: str | None = None) -> bool:
+    def remove(self, post_id: int, removed: bool, reason: Optional[str] = None) -> bool:
         """
 
         Moderator remove / restore a post.
 
         Args:
             post_id (int)
             removed (bool)
@@ -185,19 +185,19 @@
         if not re.ok:
             logger.error(f"Error encountered while removing post: {re.text}")
         return re.ok
 
     def edit(
         self,
         post_id: int,
-        name: str | None = None,
-        url: str | None = None,
-        body: str | None = None,
-        nsfw: bool | None = None,
-        language_id: int | None = None,
+        name: Optional[str] = None,
+        url: Optional[str] = None,
+        body: Optional[str] = None,
+        nsfw: Optional[bool] = None,
+        language_id: Optional[int] = None,
     ) -> bool:
         """
 
         Edit a post
 
         Args:
             post_id (int)
```

### Comparing `pythorhead-0.1.0/pythorhead.egg-info/PKG-INFO` & `pythorhead-0.1.1/pythorhead.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

