# Comparing `tmp/nonebot-plugin-msgbuf-0.3.1.tar.gz` & `tmp/nonebot-plugin-msgbuf-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-msgbuf-0.3.1.tar", last modified: Mon Jun 19 05:37:31 2023, max compression
+gzip compressed data, was "nonebot-plugin-msgbuf-0.3.2.tar", last modified: Mon Jun 19 08:03:36 2023, max compression
```

## Comparing `nonebot-plugin-msgbuf-0.3.1.tar` & `nonebot-plugin-msgbuf-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:37:31.355826 nonebot-plugin-msgbuf-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-19 05:37:16.000000 nonebot-plugin-msgbuf-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-19 05:37:31.355826 nonebot-plugin-msgbuf-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-19 05:37:16.000000 nonebot-plugin-msgbuf-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:37:31.351826 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-19 05:37:16.000000 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-19 05:37:16.000000 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-06-19 05:37:16.000000 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-06-19 05:37:16.000000 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/platforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-19 05:37:16.000000 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:37:31.355826 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-19 05:37:31.000000 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-19 05:37:31.000000 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 05:37:31.000000 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 05:37:31.000000 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 05:37:31.000000 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-19 05:37:16.000000 nonebot-plugin-msgbuf-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 05:37:31.355826 nonebot-plugin-msgbuf-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:03:36.260136 nonebot-plugin-msgbuf-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-19 08:03:25.000000 nonebot-plugin-msgbuf-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-19 08:03:36.260136 nonebot-plugin-msgbuf-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-19 08:03:25.000000 nonebot-plugin-msgbuf-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:03:36.260136 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-06-19 08:03:25.000000 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-19 08:03:25.000000 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-06-19 08:03:25.000000 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-06-19 08:03:25.000000 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-19 08:03:25.000000 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:03:36.260136 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-19 08:03:36.000000 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-19 08:03:36.000000 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:03:36.000000 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 08:03:36.000000 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 08:03:36.000000 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-19 08:03:25.000000 nonebot-plugin-msgbuf-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 08:03:36.260136 nonebot-plugin-msgbuf-0.3.2/setup.cfg
```

### Comparing `nonebot-plugin-msgbuf-0.3.1/LICENSE` & `nonebot-plugin-msgbuf-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.3.1/PKG-INFO` & `nonebot-plugin-msgbuf-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-msgbuf
-Version: 0.3.1
+Version: 0.3.2
 Summary: 适用于 NoneBot2 插件的被动消息构造集成
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-msgbuf
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-msgbuf
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `nonebot-plugin-msgbuf-0.3.1/README.md` & `nonebot-plugin-msgbuf-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/__init__.py` & `nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 from collections import deque
+from contextlib import suppress
 from types import TracebackType
 from typing import (
     Any,        Deque,      Generic,    List,       Optional,   Type,
     Union,      cast
 )
 from nonebot import logger, __version__ as nbver
 from nonebot.adapters import MessageSegment
```

### Comparing `nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/base.py` & `nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/base.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/models.py` & `nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/models.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/platforms.py` & `nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/platforms.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/utils.py` & `nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf.egg-info/PKG-INFO` & `nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-msgbuf
-Version: 0.3.1
+Version: 0.3.2
 Summary: 适用于 NoneBot2 插件的被动消息构造集成
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-msgbuf
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-msgbuf
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

