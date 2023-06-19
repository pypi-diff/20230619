# Comparing `tmp/bbhbot-0.0.6.tar.gz` & `tmp/bbhbot-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbhbot-0.0.6.tar", last modified: Sat Oct 15 13:50:21 2022, max compression
+gzip compressed data, was "bbhbot-0.0.7.tar", last modified: Mon Jun 19 16:04:28 2023, max compression
```

## Comparing `bbhbot-0.0.6.tar` & `bbhbot-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwx---   0 root         (0)     9997        0 2022-10-15 13:50:21.142161 bbhbot-0.0.6/
--rw-rw----   0 root         (0)     9997     1092 2022-08-20 16:47:14.000000 bbhbot-0.0.6/LICENSE
--rw-rw----   0 root         (0)     9997      181 2022-08-20 16:47:48.000000 bbhbot-0.0.6/MANIFEST.in
--rw-rw----   0 root         (0)     9997     2279 2022-10-15 13:50:21.142161 bbhbot-0.0.6/PKG-INFO
--rw-rw----   0 root         (0)     9997     1735 2022-10-12 14:07:44.000000 bbhbot-0.0.6/README.md
--rw-rw----   0 root         (0)     9997      211 2022-08-20 16:24:02.000000 bbhbot-0.0.6/pyproject.toml
--rw-rw----   0 root         (0)     9997      714 2022-10-15 13:50:21.152161 bbhbot-0.0.6/setup.cfg
--rw-rw----   0 root         (0)     9997      894 2022-10-15 13:40:05.000000 bbhbot-0.0.6/setup.py
-drwxrwx---   0 root         (0)     9997        0 2022-10-15 13:50:20.802161 bbhbot-0.0.6/src/
-drwxrwx---   0 root         (0)     9997        0 2022-10-15 13:50:21.052161 bbhbot-0.0.6/src/bbhbot/
--rw-rw----   0 root         (0)     9997        0 2022-08-20 16:24:01.000000 bbhbot-0.0.6/src/bbhbot/__init__.py
--rw-rw----   0 root         (0)     9997    12414 2022-10-15 13:39:29.000000 bbhbot-0.0.6/src/bbhbot/bbhbot.py
-drwxrwx---   0 root         (0)     9997        0 2022-10-15 13:50:21.132161 bbhbot-0.0.6/src/bbhbot.egg-info/
--rw-rw----   0 root         (0)     9997     2279 2022-10-15 13:50:20.000000 bbhbot-0.0.6/src/bbhbot.egg-info/PKG-INFO
--rw-rw----   0 root         (0)     9997      276 2022-10-15 13:50:20.000000 bbhbot-0.0.6/src/bbhbot.egg-info/SOURCES.txt
--rw-rw----   0 root         (0)     9997        1 2022-10-15 13:50:20.000000 bbhbot-0.0.6/src/bbhbot.egg-info/dependency_links.txt
--rw-rw----   0 root         (0)     9997        1 2022-08-21 13:37:28.000000 bbhbot-0.0.6/src/bbhbot.egg-info/not-zip-safe
--rw-rw----   0 root         (0)     9997        7 2022-10-15 13:50:20.000000 bbhbot-0.0.6/src/bbhbot.egg-info/top_level.txt
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-06-19 16:04:28.291768 bbhbot-0.0.7/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1092 2023-06-19 16:03:23.000000 bbhbot-0.0.7/LICENSE
+-rw-r--r--   0 debian    (1000) debian    (1000)      181 2023-06-19 16:03:23.000000 bbhbot-0.0.7/MANIFEST.in
+-rw-r--r--   0 debian    (1000) debian    (1000)     2279 2023-06-19 16:04:28.291768 bbhbot-0.0.7/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)     1735 2023-06-19 16:03:23.000000 bbhbot-0.0.7/README.md
+-rw-r--r--   0 debian    (1000) debian    (1000)      211 2023-06-19 16:03:23.000000 bbhbot-0.0.7/pyproject.toml
+-rw-r--r--   0 debian    (1000) debian    (1000)      714 2023-06-19 16:04:28.291768 bbhbot-0.0.7/setup.cfg
+-rw-r--r--   0 debian    (1000) debian    (1000)      894 2023-06-19 16:03:23.000000 bbhbot-0.0.7/setup.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-06-19 16:04:28.287768 bbhbot-0.0.7/src/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-06-19 16:04:28.291768 bbhbot-0.0.7/src/bbhbot/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-06-19 16:03:23.000000 bbhbot-0.0.7/src/bbhbot/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    12409 2023-06-19 16:03:23.000000 bbhbot-0.0.7/src/bbhbot/bbhbot.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-06-19 16:04:28.291768 bbhbot-0.0.7/src/bbhbot.egg-info/
+-rw-r--r--   0 debian    (1000) debian    (1000)     2279 2023-06-19 16:04:28.000000 bbhbot-0.0.7/src/bbhbot.egg-info/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)      276 2023-06-19 16:04:28.000000 bbhbot-0.0.7/src/bbhbot.egg-info/SOURCES.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        1 2023-06-19 16:04:28.000000 bbhbot-0.0.7/src/bbhbot.egg-info/dependency_links.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        1 2023-06-19 16:04:27.000000 bbhbot-0.0.7/src/bbhbot.egg-info/not-zip-safe
+-rw-r--r--   0 debian    (1000) debian    (1000)        7 2023-06-19 16:04:28.000000 bbhbot-0.0.7/src/bbhbot.egg-info/top_level.txt
```

### Comparing `bbhbot-0.0.6/LICENSE` & `bbhbot-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bbhbot-0.0.6/PKG-INFO` & `bbhbot-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbhbot
-Version: 0.0.6
+Version: 0.0.7
 Summary: A script to find and react to BBH commands in comments
 Home-page: https://github.com/flaxz/bbhbot
 Author: Erik Gustafsson (Team Alive) and Hive Pizza Team
 Author-email: erikegse@gmail.com
 Project-URL: Bug Tracker, https://github.com/flaxz/bbhbot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bbhbot-0.0.6/README.md` & `bbhbot-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `bbhbot-0.0.6/setup.cfg` & `bbhbot-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bbhbot
-version = 0.0.6
+version = 0.0.7
 author = Erik Gustafsson (Team Alive) and Hive Pizza Team
 author_email = erikegse@gmail.com
 description = A script to find and react to BBH commands in comments
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/flaxz/bbhbot
 project_urls =
```

### Comparing `bbhbot-0.0.6/setup.py` & `bbhbot-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="bbhbot",
-    version="0.0.6",
+    version="0.0.7",
     author="Erik Gustafsson (Team Alive) and Hive Pizza Team",
     author_email="erikegse@gmail.com",
     description="A script to find and react to BBH commands in comments",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/flaxz/bbhbot",
     project_urls={
```

### Comparing `bbhbot-0.0.6/src/bbhbot/bbhbot.py` & `bbhbot-0.0.7/src/bbhbot/bbhbot.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ACCOUNT_NAME = config['Global']['ACCOUNT_NAME']
 ACCOUNT_POSTING_KEY = config['Global']['ACCOUNT_POSTING_KEY']
 HIVE_API_NODE = config['Global']['HIVE_API_NODE']
 HIVE = Hive(node=[HIVE_API_NODE], keys=[config['Global']['ACCOUNT_ACTIVE_KEY']])
 HIVE.chain_params['chain_id'] = 'beeab0de00000000000000000000000000000000000000000000000000000000'
 beem.instance.set_shared_blockchain_instance(HIVE)
 
-setApi = Api(url = "https://engine.rishipanthee.com/")
+setApi = Api(url = "https://api.primersion.com/")
 
 ACCOUNT = Account(ACCOUNT_NAME)
 TOKEN_NAME = config['HiveEngine']['TOKEN_NAME']
 
 BOT_COMMAND_STR = config['Global']['BOT_COMMAND_STR']
 
 SQLITE_DATABASE_FILE = 'bbhbot.db'
```

### Comparing `bbhbot-0.0.6/src/bbhbot.egg-info/PKG-INFO` & `bbhbot-0.0.7/src/bbhbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbhbot
-Version: 0.0.6
+Version: 0.0.7
 Summary: A script to find and react to BBH commands in comments
 Home-page: https://github.com/flaxz/bbhbot
 Author: Erik Gustafsson (Team Alive) and Hive Pizza Team
 Author-email: erikegse@gmail.com
 Project-URL: Bug Tracker, https://github.com/flaxz/bbhbot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

