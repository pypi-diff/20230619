# Comparing `tmp/nonebot_plugin_al-0.2.1.tar.gz` & `tmp/nonebot_plugin_al-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_al-0.2.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_al-0.3.0.tar", max compression
```

## Comparing `nonebot_plugin_al-0.2.1.tar` & `nonebot_plugin_al-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-06-13 07:45:36.610418 nonebot_plugin_al-0.2.1/LICENSE
--rw-r--r--   0        0        0     1835 2023-06-13 07:45:36.610418 nonebot_plugin_al-0.2.1/README.md
--rw-r--r--   0        0        0     2631 2023-06-13 07:45:36.610418 nonebot_plugin_al-0.2.1/nonebot_plugin_al/__init__.py
--rw-r--r--   0        0        0      757 2023-06-13 07:45:36.610418 nonebot_plugin_al-0.2.1/nonebot_plugin_al/api.py
--rw-r--r--   0        0        0     3349 2023-06-13 07:45:36.610418 nonebot_plugin_al-0.2.1/nonebot_plugin_al/bili.py
--rw-r--r--   0        0        0    69109 2023-06-13 07:45:36.610418 nonebot_plugin_al-0.2.1/nonebot_plugin_al/data/eq.json
--rw-r--r--   0        0        0    41850 2023-06-13 07:45:36.610418 nonebot_plugin_al-0.2.1/nonebot_plugin_al/data/ship.json
--rw-r--r--   0        0        0      943 2023-06-13 07:45:36.610418 nonebot_plugin_al-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2798 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3645 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/README.md
+-rw-r--r--   0        0        0     6475 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/nonebot_plugin_al/__init__.py
+-rw-r--r--   0        0        0    69693 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/nonebot_plugin_al/api.py
+-rw-r--r--   0        0        0     3348 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/nonebot_plugin_al/bili.py
+-rw-r--r--   0        0        0    69109 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/nonebot_plugin_al/data/eq.json
+-rw-r--r--   0        0        0    41850 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/nonebot_plugin_al/data/ship.json
+-rw-r--r--   0        0        0    10152 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/nonebot_plugin_al/draw.py
+-rw-r--r--   0        0        0     7529 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/nonebot_plugin_al/name.py
+-rw-r--r--   0        0        0    13339 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/nonebot_plugin_al/send_message.py
+-rw-r--r--   0        0        0     5832 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/nonebot_plugin_al/utils.py
+-rw-r--r--   0        0        0     1003 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4733 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_al-0.2.1/LICENSE` & `nonebot_plugin_al-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.2.1/nonebot_plugin_al/bili.py` & `nonebot_plugin_al-0.3.0/nonebot_plugin_al/bili.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import asyncio
 from bs4 import BeautifulSoup
 from pathlib import Path
 import time
 
 from nonebot import require
 from nonebot.log import logger
-require("nonebot_plugin_htmlrender")
 from nonebot_plugin_htmlrender import (
     html_to_pic,
 )
-
-from .api import get_data
+require("nonebot_plugin_htmlrender")
 
 
+from .api import get_data
 
 async def jinghao(tag):
     data = await get_data('https://wiki.biligame.com/blhx/井号碧蓝榜合集')
     soup = BeautifulSoup(data, 'html.parser')
     if tag == '强度榜':
         img_tag = soup.find('img', alt="认知觉醒主线推荐榜.jpg")
     elif tag == '装备榜':
```

### Comparing `nonebot_plugin_al-0.2.1/nonebot_plugin_al/data/eq.json` & `nonebot_plugin_al-0.3.0/nonebot_plugin_al/data/eq.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.2.1/nonebot_plugin_al/data/ship.json` & `nonebot_plugin_al-0.3.0/nonebot_plugin_al/data/ship.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.2.1/pyproject.toml` & `nonebot_plugin_al-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_al"
-version = "0.2.1"
+version = "0.3.0"
 description = "Azuer L plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_AL"
 repository = "https://github.com/Agnes4m/nonebot_plugin_AL"
 keywords = ["game", "nonebot2", "plugin","bilibili"]
@@ -23,11 +23,14 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = "^2.0.0"
 nonebot-adapter-onebot = ">=2.2.1"
 nonebot_plugin_htmlrender = "^0.2.0.3"
 aiohttp = ">=3.8.3"
 bs4 = "^0.0.1"
+aiofiles = "^23.1.0"
+pypinyin = "^0.49.0"
+imgkit = "^1.2.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

