# Comparing `tmp/nonebot-plugin-msgbuf-0.3.0.tar.gz` & `tmp/nonebot-plugin-msgbuf-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-msgbuf-0.3.0.tar", last modified: Sat May 27 13:22:37 2023, max compression
+gzip compressed data, was "nonebot-plugin-msgbuf-0.3.1.tar", last modified: Mon Jun 19 05:37:31 2023, max compression
```

## Comparing `nonebot-plugin-msgbuf-0.3.0.tar` & `nonebot-plugin-msgbuf-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 13:22:37.515633 nonebot-plugin-msgbuf-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-27 13:22:26.000000 nonebot-plugin-msgbuf-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-27 13:22:37.511633 nonebot-plugin-msgbuf-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-27 13:22:26.000000 nonebot-plugin-msgbuf-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 13:22:37.511633 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf/
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-05-27 13:22:26.000000 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-27 13:22:26.000000 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-05-27 13:22:26.000000 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-05-27 13:22:26.000000 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf/platforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-27 13:22:26.000000 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 13:22:37.511633 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-27 13:22:37.000000 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-27 13:22:37.000000 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 13:22:37.000000 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-27 13:22:37.000000 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 13:22:37.000000 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-27 13:22:26.000000 nonebot-plugin-msgbuf-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 13:22:37.515633 nonebot-plugin-msgbuf-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:37:31.355826 nonebot-plugin-msgbuf-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-19 05:37:16.000000 nonebot-plugin-msgbuf-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-19 05:37:31.355826 nonebot-plugin-msgbuf-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-19 05:37:16.000000 nonebot-plugin-msgbuf-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:37:31.351826 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-19 05:37:16.000000 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-19 05:37:16.000000 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-06-19 05:37:16.000000 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-06-19 05:37:16.000000 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-19 05:37:16.000000 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:37:31.355826 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-19 05:37:31.000000 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-19 05:37:31.000000 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 05:37:31.000000 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 05:37:31.000000 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 05:37:31.000000 nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-19 05:37:16.000000 nonebot-plugin-msgbuf-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 05:37:31.355826 nonebot-plugin-msgbuf-0.3.1/setup.cfg
```

### Comparing `nonebot-plugin-msgbuf-0.3.0/LICENSE` & `nonebot-plugin-msgbuf-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.3.0/PKG-INFO` & `nonebot-plugin-msgbuf-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-msgbuf
-Version: 0.3.0
+Version: 0.3.1
 Summary: 适用于 NoneBot2 插件的被动消息构造集成
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-msgbuf
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-msgbuf
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `nonebot-plugin-msgbuf-0.3.0/README.md` & `nonebot-plugin-msgbuf-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf/__init__.py` & `nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 from nonebot.plugin import PluginMetadata
 
 from .base import MsgBufManager
 from .models import (
     Face,       File,       Image,      Location,   Mention,    Model,
     Raw,        Reply,      Share,      Text,       Video,      Voice
 )
-from .platforms import _BotT, _EventT, ForwardBuffer, Specs, find_proxy
+from .platforms import _BotT, _EventT, Specs, find_proxy
 
 _extra_meta_source = {
     "type": "library",
-    "homepage": "https://github.com/NCBM/nonebot-plugin-msgbuf"
+    "homepage": "https://github.com/NCBM/nonebot-plugin-msgbuf",
+    "supported_adapters": {"~onebot.v11", "~onebot.v12", "~qqguild"}
 }
 
 if (
     not nbver
     or not nbver.startswith("2.0.0")
     or not (_suf := nbver[5:])
     or _suf[0] not in "abr"
@@ -135,15 +136,18 @@
         """发送当前缓冲的消息并清空缓冲区"""
         res = await self.send()
         self.msgbuf.clear()
         return res
 
 
 MsgBuf = MessageBuffer
-FwdBuf = ForwardBuffer
 
 __all__ = (
     "Face",     "File",     "Image",    "Location", "Mention",  "Raw",
     "Reply",    "Share",    "Text",     "Video",    "Voice",
     "MessageBuffer",        "MsgBuf",               "Specs",
-    "ForwardBuffer",        "FwdBuf"
-)
+)
+
+with suppress(ImportError):
+    from .platforms import ForwardBuffer
+    FwdBuf = ForwardBuffer
+    __all__ += ("ForwardBuffer", "FwdBuf")
```

### Comparing `nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf/base.py` & `nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/base.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf/models.py` & `nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/models.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf/platforms.py` & `nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/platforms.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf/utils.py` & `nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf.egg-info/PKG-INFO` & `nonebot-plugin-msgbuf-0.3.1/nonebot_plugin_msgbuf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-msgbuf
-Version: 0.3.0
+Version: 0.3.1
 Summary: 适用于 NoneBot2 插件的被动消息构造集成
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-msgbuf
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-msgbuf
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

