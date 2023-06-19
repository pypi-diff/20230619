# Comparing `tmp/nonebot_plugin_follow_withdraw-0.1.0.tar.gz` & `tmp/nonebot_plugin_follow_withdraw-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_follow_withdraw-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_follow_withdraw-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_follow_withdraw-0.1.0.tar` & `nonebot_plugin_follow_withdraw-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1062 2023-06-19 06:45:23.652090 nonebot_plugin_follow_withdraw-0.1.0/LICENSE
--rw-r--r--   0        0        0     2958 2023-06-19 06:45:23.652090 nonebot_plugin_follow_withdraw-0.1.0/README.md
--rw-r--r--   0        0        0     2144 2023-06-19 06:45:23.652090 nonebot_plugin_follow_withdraw-0.1.0/nonebot_plugin_follow_withdraw/__init__.py
--rw-r--r--   0        0        0     2880 2023-06-19 06:45:23.652090 nonebot_plugin_follow_withdraw-0.1.0/nonebot_plugin_follow_withdraw/adapter.py
--rw-r--r--   0        0        0      287 2023-06-19 06:45:23.652090 nonebot_plugin_follow_withdraw-0.1.0/nonebot_plugin_follow_withdraw/adapters/__init__.py
--rw-r--r--   0        0        0     1929 2023-06-19 06:45:23.652090 nonebot_plugin_follow_withdraw-0.1.0/nonebot_plugin_follow_withdraw/adapters/discord.py
--rw-r--r--   0        0        0     1680 2023-06-19 06:45:23.652090 nonebot_plugin_follow_withdraw-0.1.0/nonebot_plugin_follow_withdraw/adapters/kaiheila.py
--rw-r--r--   0        0        0     3654 2023-06-19 06:45:23.652090 nonebot_plugin_follow_withdraw-0.1.0/nonebot_plugin_follow_withdraw/adapters/onebot.py
--rw-r--r--   0        0        0     2110 2023-06-19 06:45:23.652090 nonebot_plugin_follow_withdraw-0.1.0/nonebot_plugin_follow_withdraw/adapters/qqguild.py
--rw-r--r--   0        0        0      586 2023-06-19 06:45:23.652090 nonebot_plugin_follow_withdraw-0.1.0/nonebot_plugin_follow_withdraw/config.py
--rw-r--r--   0        0        0     1515 2023-06-19 06:45:23.652090 nonebot_plugin_follow_withdraw-0.1.0/nonebot_plugin_follow_withdraw/migrations/258421aeb463_.py
--rw-r--r--   0        0        0     3166 2023-06-19 06:45:23.652090 nonebot_plugin_follow_withdraw-0.1.0/nonebot_plugin_follow_withdraw/model.py
--rw-r--r--   0        0        0      856 2023-06-19 06:45:23.652090 nonebot_plugin_follow_withdraw-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3646 1970-01-01 00:00:00.000000 nonebot_plugin_follow_withdraw-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2958 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/README.md
+-rw-r--r--   0        0        0     2146 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/__init__.py
+-rw-r--r--   0        0        0     2880 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapter.py
+-rw-r--r--   0        0        0      287 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapters/__init__.py
+-rw-r--r--   0        0        0     1929 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapters/discord.py
+-rw-r--r--   0        0        0     1680 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapters/kaiheila.py
+-rw-r--r--   0        0        0     3654 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapters/onebot.py
+-rw-r--r--   0        0        0     2110 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapters/qqguild.py
+-rw-r--r--   0        0        0      586 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/config.py
+-rw-r--r--   0        0        0     1515 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/migrations/258421aeb463_.py
+-rw-r--r--   0        0        0     3166 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/model.py
+-rw-r--r--   0        0        0      856 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3646 1970-01-01 00:00:00.000000 nonebot_plugin_follow_withdraw-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_follow_withdraw-0.1.0/LICENSE` & `nonebot_plugin_follow_withdraw-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_follow_withdraw-0.1.0/README.md` & `nonebot_plugin_follow_withdraw-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_follow_withdraw-0.1.0/nonebot_plugin_follow_withdraw/__init__.py` & `nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     type="application",
     homepage="https://github.com/CMHopeSunshine/nonebot-plugin-follow-withdraw",
     config=Config,
     supported_adapters={
         "~onebot.v11",
         "~onebot.v12",
         "~qqguild",
-        "~discord",
+        # "~discord",
         "~kaiheila",
     },
 )
 
 
 withdraw_notice = on_notice(rule=check_event)
```

### Comparing `nonebot_plugin_follow_withdraw-0.1.0/nonebot_plugin_follow_withdraw/adapter.py` & `nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_follow_withdraw-0.1.0/nonebot_plugin_follow_withdraw/adapters/discord.py` & `nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapters/discord.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_follow_withdraw-0.1.0/nonebot_plugin_follow_withdraw/adapters/kaiheila.py` & `nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapters/kaiheila.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_follow_withdraw-0.1.0/nonebot_plugin_follow_withdraw/adapters/onebot.py` & `nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapters/onebot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_follow_withdraw-0.1.0/nonebot_plugin_follow_withdraw/adapters/qqguild.py` & `nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapters/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_follow_withdraw-0.1.0/nonebot_plugin_follow_withdraw/config.py` & `nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_follow_withdraw-0.1.0/nonebot_plugin_follow_withdraw/migrations/258421aeb463_.py` & `nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/migrations/258421aeb463_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_follow_withdraw-0.1.0/nonebot_plugin_follow_withdraw/model.py` & `nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_follow_withdraw-0.1.0/pyproject.toml` & `nonebot_plugin_follow_withdraw-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-follow-withdraw"
-version = "0.1.0"
+version = "0.1.1"
 description = "A plugin for nonebot2 that follows the user's withdraw of a command."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_follow_withdraw"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_follow_withdraw-0.1.0/PKG-INFO` & `nonebot_plugin_follow_withdraw-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-follow-withdraw
-Version: 0.1.0
+Version: 0.1.1
 Summary: A plugin for nonebot2 that follows the user's withdraw of a command.
 License: MIT
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-follow-withdraw Version: 0.1.0
+Metadata-Version: 2.1 Name: nonebot-plugin-follow-withdraw Version: 0.1.1
 Summary: A plugin for nonebot2 that follows the user's withdraw of a command.
 License: MIT Author: CMHopeSunshine Author-email: 277073121@qq.com Requires-
 Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: nonebot-plugin-datastore
```

