# Comparing `tmp/nonebot-plugin-grouplock-0.0.1.tar.gz` & `tmp/nonebot-plugin-grouplock-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-grouplock-0.0.1.tar", max compression
+gzip compressed data, was "nonebot-plugin-grouplock-0.0.2.tar", max compression
```

## Comparing `nonebot-plugin-grouplock-0.0.1.tar` & `nonebot-plugin-grouplock-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1084 2023-05-06 16:23:42.716890 nonebot-plugin-grouplock-0.0.1/LICENSE
--rw-r--r--   0        0        0      603 2023-05-06 16:30:05.256954 nonebot-plugin-grouplock-0.0.1/nonebot_plugin_grouplock/__init__.py
--rw-r--r--   0        0        0       19 2023-05-06 16:30:38.958298 nonebot-plugin-grouplock-0.0.1/nonebot_plugin_grouplock/models/__init__.py
--rw-r--r--   0        0        0     2610 2023-05-06 14:52:08.371042 nonebot-plugin-grouplock-0.0.1/nonebot_plugin_grouplock/models/group.py
--rw-r--r--   0        0        0       27 2023-05-06 13:44:53.528737 nonebot-plugin-grouplock-0.0.1/nonebot_plugin_grouplock/utils/__init__.py
--rw-r--r--   0        0        0     9463 2023-05-06 16:09:09.732331 nonebot-plugin-grouplock-0.0.1/nonebot_plugin_grouplock/utils/handel.py
--rw-r--r--   0        0        0     2107 2023-05-06 13:39:34.393433 nonebot-plugin-grouplock-0.0.1/nonebot_plugin_grouplock/utils/path.py
--rw-r--r--   0        0        0      538 2023-05-06 16:44:35.627296 nonebot-plugin-grouplock-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      466 2023-05-06 16:42:38.346133 nonebot-plugin-grouplock-0.0.1/README.md
--rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 nonebot-plugin-grouplock-0.0.1/setup.py
--rw-r--r--   0        0        0     1176 1970-01-01 00:00:00.000000 nonebot-plugin-grouplock-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-16 08:03:49.256339 nonebot-plugin-grouplock-0.0.2/LICENSE
+-rw-r--r--   0        0        0      737 2023-06-16 08:05:08.875963 nonebot-plugin-grouplock-0.0.2/nonebot_plugin_grouplock/__init__.py
+-rw-r--r--   0        0        0       19 2023-06-16 08:03:49.257344 nonebot-plugin-grouplock-0.0.2/nonebot_plugin_grouplock/models/__init__.py
+-rw-r--r--   0        0        0     2610 2023-06-16 08:03:49.257344 nonebot-plugin-grouplock-0.0.2/nonebot_plugin_grouplock/models/group.py
+-rw-r--r--   0        0        0       27 2023-06-16 08:03:49.258359 nonebot-plugin-grouplock-0.0.2/nonebot_plugin_grouplock/utils/__init__.py
+-rw-r--r--   0        0        0     9463 2023-06-16 08:03:49.258359 nonebot-plugin-grouplock-0.0.2/nonebot_plugin_grouplock/utils/handel.py
+-rw-r--r--   0        0        0     2107 2023-06-16 08:03:49.258359 nonebot-plugin-grouplock-0.0.2/nonebot_plugin_grouplock/utils/path.py
+-rw-r--r--   0        0        0      597 2023-06-19 06:38:09.797907 nonebot-plugin-grouplock-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      466 2023-06-16 08:03:49.256339 nonebot-plugin-grouplock-0.0.2/README.md
+-rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 nonebot-plugin-grouplock-0.0.2/setup.py
+-rw-r--r--   0        0        0     1173 1970-01-01 00:00:00.000000 nonebot-plugin-grouplock-0.0.2/PKG-INFO
```

### Comparing `nonebot-plugin-grouplock-0.0.1/LICENSE` & `nonebot-plugin-grouplock-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-grouplock-0.0.1/nonebot_plugin_grouplock/__init__.py` & `nonebot-plugin-grouplock-0.0.2/nonebot_plugin_grouplock/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 
 from . import utils,models
 
 __plugin_meta__ = PluginMetadata(
     name='nonebot-plugin-grouplock',
     description='一个可以锁定群聊人数的插件',
     usage='...',
+    homepage="https://github.com/ZM25XC/nonebot-plugin-grouplock",
+    type="application",
+    supported_adapters={"~onebot.v11"},
     extra={
         'author': 'ZM25XC',
         'version': '0.0.1',
         'priority': 50,
     }
 )
 DRIVER = get_driver()
```

### Comparing `nonebot-plugin-grouplock-0.0.1/nonebot_plugin_grouplock/models/group.py` & `nonebot-plugin-grouplock-0.0.2/nonebot_plugin_grouplock/models/group.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-grouplock-0.0.1/nonebot_plugin_grouplock/utils/handel.py` & `nonebot-plugin-grouplock-0.0.2/nonebot_plugin_grouplock/utils/handel.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-grouplock-0.0.1/nonebot_plugin_grouplock/utils/path.py` & `nonebot-plugin-grouplock-0.0.2/nonebot_plugin_grouplock/utils/path.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-grouplock-0.0.1/pyproject.toml` & `nonebot-plugin-grouplock-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 [tool.poetry]
 name = "nonebot-plugin-grouplock"
-version = "0.0.1"
+version = "0.0.2"
 description = "一个基于nonebot2和go-cqhttp的群聊人数锁定插件"
 authors = ["ZM25XC <xingling25@qq.com>"]
 license="MIT"
 readme="README.md"
 homepage="https://github.com/ZM25XC/nonebot-plugin-grouplock"
+packages = [
+  { include = "nonebot_plugin_grouplock" },
+]
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot-adapter-onebot="^2.2.1"
-nonebot2="^2.0.0rc3"
+nonebot-adapter-onebot="^2.2.3"
+nonebot2="^2.0.0"
 tortoise-orm="^0.19.3"
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot-plugin-grouplock-0.0.1/setup.py` & `nonebot-plugin-grouplock-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,21 +6,21 @@
  'nonebot_plugin_grouplock.models',
  'nonebot_plugin_grouplock.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['nonebot-adapter-onebot>=2.2.1,<3.0.0',
- 'nonebot2>=2.0.0rc3,<3.0.0',
+['nonebot-adapter-onebot>=2.2.3,<3.0.0',
+ 'nonebot2>=2.0.0,<3.0.0',
  'tortoise-orm>=0.19.3,<0.20.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-grouplock',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': '一个基于nonebot2和go-cqhttp的群聊人数锁定插件',
     'long_description': '<p align="center">\n  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>\n</p>\n\n<div align="center">\n\n#  nonebot-plugin-grouplock\n一个基于nonebot2和go-cqhttp的群聊人数锁定插件\n\n## 指令\n\n\n| 命令 | 示例 |\n|:--------:|:-------------:|\n| 锁定人数  |  锁定人数开 锁定人数500 锁定人数关 |\n|检查人数|   检查人数开 检查人数关 检查人数|',
     'author': 'ZM25XC',
     'author_email': 'xingling25@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ZM25XC/nonebot-plugin-grouplock',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_grouplock', 'nonebot_plugin_grouplock.models',
 'nonebot_plugin_grouplock.utils'] package_data = \ {'': ['*']} install_requires
-= \ ['nonebot-adapter-onebot>=2.2.1,<3.0.0', 'nonebot2>=2.0.0rc3,<3.0.0',
+= \ ['nonebot-adapter-onebot>=2.2.3,<3.0.0', 'nonebot2>=2.0.0,<3.0.0',
 'tortoise-orm>=0.19.3,<0.20.0'] setup_kwargs = { 'name': 'nonebot-plugin-
-grouplock', 'version': '0.0.1', 'description': 'ä¸ä¸ªåºäºnonebot2ågo-
+grouplock', 'version': '0.0.2', 'description': 'ä¸ä¸ªåºäºnonebot2ågo-
 cqhttpçç¾¤èäººæ°éå®æä»¶', 'long_description': '
                                 \n [nonebot]\n
 \n\n
           \n\n# nonebot-plugin-grouplock\nä¸ä¸ªåºäºnonebot2ågo-
 cqhttpçç¾¤èäººæ°éå®æä»¶\n\n## æä»¤\n\n\n| å½ä»¤ | ç¤ºä¾ |\n|:----
    ----:|:-------------:|\n| éå®äººæ° | éå®äººæ°å¼ éå®äººæ°500
        éå®äººæ°å³ |\n|æ£æ¥äººæ°| æ£æ¥äººæ°å¼ æ£æ¥äººæ°å³
```

### Comparing `nonebot-plugin-grouplock-0.0.1/PKG-INFO` & `nonebot-plugin-grouplock-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-grouplock
-Version: 0.0.1
+Version: 0.0.2
 Summary: 一个基于nonebot2和go-cqhttp的群聊人数锁定插件
 Home-page: https://github.com/ZM25XC/nonebot-plugin-grouplock
 License: MIT
 Author: ZM25XC
 Author-email: xingling25@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0)
-Requires-Dist: nonebot2 (>=2.0.0rc3,<3.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: tortoise-orm (>=0.19.3,<0.20.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-grouplock Version: 0.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-grouplock Version: 0.0.2 Summary:
 ä¸ä¸ªåºäºnonebot2ågo-cqhttpçç¾¤èäººæ°éå®æä»¶ Home-page: https://
 github.com/ZM25XC/nonebot-plugin-grouplock License: MIT Author: ZM25XC Author-
 email: xingling25@qq.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0) Requires-Dist: nonebot2
-(>=2.0.0rc3,<3.0.0) Requires-Dist: tortoise-orm (>=0.19.3,<0.20.0) Description-
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0) Requires-Dist: nonebot2
+(>=2.0.0,<3.0.0) Requires-Dist: tortoise-orm (>=0.19.3,<0.20.0) Description-
 Content-Type: text/markdown
                                    [nonebot]
              # nonebot-plugin-grouplock ä¸ä¸ªåºäºnonebot2ågo-
 cqhttpçç¾¤èäººæ°éå®æä»¶ ## æä»¤ | å½ä»¤ | ç¤ºä¾ | |:--------:|:--
 -----------:| | éå®äººæ° | éå®äººæ°å¼ éå®äººæ°500 éå®äººæ°å³
         | |æ£æ¥äººæ°| æ£æ¥äººæ°å¼ æ£æ¥äººæ°å³ æ£æ¥äººæ°|
```

