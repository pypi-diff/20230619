# Comparing `tmp/alivebot-0.1.8.tar.gz` & `tmp/alivebot-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alivebot-0.1.8.tar", last modified: Sat Jul  2 16:45:18 2022, max compression
+gzip compressed data, was "alivebot-0.1.9.tar", last modified: Sat Jul  2 17:17:13 2022, max compression
```

## Comparing `alivebot-0.1.8.tar` & `alivebot-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwx---   0 root         (0)     9997        0 2022-07-02 16:45:17.975932 alivebot-0.1.8/
--rw-rw----   0 root         (0)     9997     1085 2021-11-06 12:36:38.000000 alivebot-0.1.8/LICENSE
--rw-rw----   0 root         (0)     9997      183 2021-11-07 20:31:33.000000 alivebot-0.1.8/MANIFEST.in
--rw-rw----   0 root         (0)     9997     2277 2022-07-02 16:45:17.975932 alivebot-0.1.8/PKG-INFO
--rw-rw----   0 root         (0)     9997     1738 2021-11-17 13:05:34.000000 alivebot-0.1.8/README.md
--rw-rw----   0 root         (0)     9997      211 2021-11-06 12:53:42.000000 alivebot-0.1.8/pyproject.toml
--rw-rw----   0 root         (0)     9997      709 2022-07-02 16:45:17.985932 alivebot-0.1.8/setup.cfg
--rw-rw----   0 root         (0)     9997      889 2022-07-02 16:44:02.000000 alivebot-0.1.8/setup.py
-drwxrwx---   0 root         (0)     9997        0 2022-07-02 16:45:17.715932 alivebot-0.1.8/src/
-drwxrwx---   0 root         (0)     9997        0 2022-07-02 16:45:17.895932 alivebot-0.1.8/src/alivebot/
--rw-rw----   0 root         (0)     9997        0 2021-11-06 12:41:10.000000 alivebot-0.1.8/src/alivebot/__init__.py
--rw-rw----   0 root         (0)     9997    12563 2022-07-02 16:41:33.000000 alivebot-0.1.8/src/alivebot/alivebot.py
-drwxrwx---   0 root         (0)     9997        0 2022-07-02 16:45:17.975932 alivebot-0.1.8/src/alivebot.egg-info/
--rw-rw----   0 root         (0)     9997     2277 2022-07-02 16:45:15.000000 alivebot-0.1.8/src/alivebot.egg-info/PKG-INFO
--rw-rw----   0 root         (0)     9997      292 2022-07-02 16:45:17.000000 alivebot-0.1.8/src/alivebot.egg-info/SOURCES.txt
--rw-rw----   0 root         (0)     9997        1 2022-07-02 16:45:15.000000 alivebot-0.1.8/src/alivebot.egg-info/dependency_links.txt
--rw-rw----   0 root         (0)     9997        1 2021-11-17 10:32:02.000000 alivebot-0.1.8/src/alivebot.egg-info/not-zip-safe
--rw-rw----   0 root         (0)     9997        9 2022-07-02 16:45:17.000000 alivebot-0.1.8/src/alivebot.egg-info/top_level.txt
+drwxrwx---   0 root         (0)     9997        0 2022-07-02 17:17:13.895931 alivebot-0.1.9/
+-rw-rw----   0 root         (0)     9997     1085 2021-11-06 12:36:38.000000 alivebot-0.1.9/LICENSE
+-rw-rw----   0 root         (0)     9997      183 2021-11-07 20:31:33.000000 alivebot-0.1.9/MANIFEST.in
+-rw-rw----   0 root         (0)     9997     2277 2022-07-02 17:17:13.895931 alivebot-0.1.9/PKG-INFO
+-rw-rw----   0 root         (0)     9997     1738 2021-11-17 13:05:34.000000 alivebot-0.1.9/README.md
+-rw-rw----   0 root         (0)     9997      211 2021-11-06 12:53:42.000000 alivebot-0.1.9/pyproject.toml
+-rw-rw----   0 root         (0)     9997      709 2022-07-02 17:17:13.895931 alivebot-0.1.9/setup.cfg
+-rw-rw----   0 root         (0)     9997      889 2022-07-02 17:15:32.000000 alivebot-0.1.9/setup.py
+drwxrwx---   0 root         (0)     9997        0 2022-07-02 17:17:13.425931 alivebot-0.1.9/src/
+drwxrwx---   0 root         (0)     9997        0 2022-07-02 17:17:13.775931 alivebot-0.1.9/src/alivebot/
+-rw-rw----   0 root         (0)     9997        0 2021-11-06 12:41:10.000000 alivebot-0.1.9/src/alivebot/__init__.py
+-rw-rw----   0 root         (0)     9997    12535 2022-07-02 17:15:04.000000 alivebot-0.1.9/src/alivebot/alivebot.py
+drwxrwx---   0 root         (0)     9997        0 2022-07-02 17:17:13.885931 alivebot-0.1.9/src/alivebot.egg-info/
+-rw-rw----   0 root         (0)     9997     2277 2022-07-02 17:17:11.000000 alivebot-0.1.9/src/alivebot.egg-info/PKG-INFO
+-rw-rw----   0 root         (0)     9997      292 2022-07-02 17:17:13.000000 alivebot-0.1.9/src/alivebot.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0)     9997        1 2022-07-02 17:17:11.000000 alivebot-0.1.9/src/alivebot.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0)     9997        1 2021-11-17 10:32:02.000000 alivebot-0.1.9/src/alivebot.egg-info/not-zip-safe
+-rw-rw----   0 root         (0)     9997        9 2022-07-02 17:17:12.000000 alivebot-0.1.9/src/alivebot.egg-info/top_level.txt
```

### Comparing `alivebot-0.1.8/LICENSE` & `alivebot-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alivebot-0.1.8/PKG-INFO` & `alivebot-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alivebot
-Version: 0.1.8
+Version: 0.1.9
 Summary: A script to find and react to ALIVE commands in comments
 Home-page: https://github.com/flaxz/alivebot
 Author: Erik Gustafsson and Hive Pizza Team
 Author-email: erikegse@gmail.com
 Project-URL: Bug Tracker, https://github.com/flaxz/alivebot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alivebot-0.1.8/README.md` & `alivebot-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `alivebot-0.1.8/setup.cfg` & `alivebot-0.1.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = alivebot
-version = 0.1.8
+version = 0.1.9
 author = Erik Gustafsson and Hive Pizza Team
 author_email = erikegse@gmail.com
 description = A script to find and react to ALIVE commands in comments
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/flaxz/alivebot
 project_urls =
```

### Comparing `alivebot-0.1.8/setup.py` & `alivebot-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="alivebot",
-    version="0.1.8",
+    version="0.1.9",
     author="Erik Gustafsson and Hive Pizza Team",
     author_email="erikegse@gmail.com",
     description="A script to find and react to ALIVE commands in comments",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/flaxz/alivebot",
     project_urls={
```

### Comparing `alivebot-0.1.8/src/alivebot/alivebot.py` & `alivebot-0.1.9/src/alivebot/alivebot.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 ACCOUNT_NAME = config['Global']['ACCOUNT_NAME']
 ACCOUNT_POSTING_KEY = config['Global']['ACCOUNT_POSTING_KEY']
 HIVE_API_NODE = config['Global']['HIVE_API_NODE']
 HIVE = Hive(node=[HIVE_API_NODE], keys=[config['Global']['ACCOUNT_ACTIVE_KEY']])
 HIVE.chain_params['chain_id'] = 'beeab0de00000000000000000000000000000000000000000000000000000000'
 beem.instance.set_shared_blockchain_instance(HIVE)
 
-api = Api(url = "https://engine.rishipanthee.com", rpcurl = "https://engine.rishipanthee.com")
+apiUrl = "https://engine.rishipanthee.com"
+api = Api(url = apiUrl)
 
 ACCOUNT = Account(ACCOUNT_NAME)
 TOKEN_NAME = config['HiveEngine']['TOKEN_NAME']
 
 BOT_COMMAND_STR = config['Global']['BOT_COMMAND_STR']
 
 SQLITE_DATABASE_FILE = 'alivebot.db'
```

### Comparing `alivebot-0.1.8/src/alivebot.egg-info/PKG-INFO` & `alivebot-0.1.9/src/alivebot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alivebot
-Version: 0.1.8
+Version: 0.1.9
 Summary: A script to find and react to ALIVE commands in comments
 Home-page: https://github.com/flaxz/alivebot
 Author: Erik Gustafsson and Hive Pizza Team
 Author-email: erikegse@gmail.com
 Project-URL: Bug Tracker, https://github.com/flaxz/alivebot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

