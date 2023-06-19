# Comparing `tmp/nonebot-plugin-mixin-0.1.1.tar.gz` & `tmp/nonebot-plugin-mixin-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mixin-0.1.1.tar", last modified: Sun Apr 23 11:30:24 2023, max compression
+gzip compressed data, was "nonebot-plugin-mixin-0.1.2.tar", last modified: Mon Jun 19 08:05:10 2023, max compression
```

## Comparing `nonebot-plugin-mixin-0.1.1.tar` & `nonebot-plugin-mixin-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:30:24.405837 nonebot-plugin-mixin-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-23 11:30:13.000000 nonebot-plugin-mixin-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-23 11:30:24.405837 nonebot-plugin-mixin-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-23 11:30:13.000000 nonebot-plugin-mixin-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:30:24.405837 nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin/
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-23 11:30:13.000000 nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-23 11:30:13.000000 nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:30:24.405837 nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-23 11:30:24.000000 nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-23 11:30:24.000000 nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 11:30:24.000000 nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 11:30:24.000000 nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-23 11:30:24.000000 nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-23 11:30:13.000000 nonebot-plugin-mixin-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 11:30:24.405837 nonebot-plugin-mixin-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:05:10.393718 nonebot-plugin-mixin-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-19 08:04:53.000000 nonebot-plugin-mixin-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-06-19 08:05:10.393718 nonebot-plugin-mixin-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-19 08:04:53.000000 nonebot-plugin-mixin-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:05:10.389717 nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-06-19 08:04:53.000000 nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-19 08:04:53.000000 nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:05:10.389717 nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-06-19 08:05:10.000000 nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-19 08:05:10.000000 nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:05:10.000000 nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 08:05:10.000000 nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-19 08:05:10.000000 nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-19 08:04:53.000000 nonebot-plugin-mixin-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 08:05:10.393718 nonebot-plugin-mixin-0.1.2/setup.cfg
```

### Comparing `nonebot-plugin-mixin-0.1.1/LICENSE` & `nonebot-plugin-mixin-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mixin-0.1.1/PKG-INFO` & `nonebot-plugin-mixin-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mixin
-Version: 0.1.1
+Version: 0.1.2
 Summary: 通过代码或非代码方式外部介入 NoneBot2 插件行为
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-mixin
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-mixin
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-mixin Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-mixin Version: 0.1.2 Summary:
 éè¿ä»£ç æéä»£ç æ¹å¼å¤é¨ä»å¥ NoneBot2 æä»¶è¡ä¸º Author-email:
 HivertMoZara
 163.com> License: MIT Project-URL: Homepage, https://github.com/NCBM/nonebot-
 plugin-mixin Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-
 mixin Requires-Python: >=3.8 Description-Content-Type: text/markdown License-
 File: LICENSE
 # nonebot-plugin-mixin _â¨ éè¿ä»£ç æéä»£ç æ¹å¼å¤é¨ä»å¥ NoneBot2
```

### Comparing `nonebot-plugin-mixin-0.1.1/README.md` & `nonebot-plugin-mixin-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin/__init__.py` & `nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,30 +4,55 @@
 注意：本插件并不保证更改会被稳定应用，部分插件可能会在运行时修改自身部分行为。
 """
 
 from functools import partial, reduce
 import json
 from operator import and_
 from pathlib import Path
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Type, Union
-from nonebot import get_driver, logger
+from typing import Any, Iterable, List, Optional, Tuple, Type, Union
+from nonebot import get_driver, logger, __version__ as nbver
 from nonebot.internal.matcher import Matcher, matchers
 from nonebot.internal.rule import Rule
 from nonebot.rule import (
     StartswithRule, EndswithRule, FullmatchRule,
     KeywordsRule, CommandRule, RegexRule, ToMeRule,
     command
 )
+from nonebot.plugin import PluginMetadata
 from pydantic import BaseModel, Field
 
 from .config import Config
 
 global_config = get_driver().config
 config_ = Config.parse_obj(global_config)
 
+_extra_meta_source = {
+    "type": "library",
+    "homepage": "https://github.com/NCBM/nonebot-plugin-mixin"
+}
+
+if (
+    not nbver
+    or not nbver.startswith("2.0.0")
+    or not (_suf := nbver[5:])
+    or _suf[0] not in "abr"
+    or (_suf.startswith("rc") and int(_suf[2:]) > 4)
+):
+    _extra_meta = _extra_meta_source
+else:
+    _extra_meta = {"extra": _extra_meta_source}
+
+__plugin_meta__ = PluginMetadata(
+    name="Mixin",
+    description="通过代码或非代码方式外部介入 NoneBot2 插件行为",
+    usage="[请查阅插件介绍文档]",
+    config=Config,
+    **_extra_meta
+)
+
 driver = get_driver()
 
 
 class CaseMatch(BaseModel):
     msg: Tuple[str, ...]
     ignorecase: bool = False
```

### Comparing `nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin.egg-info/PKG-INFO` & `nonebot-plugin-mixin-0.1.2/nonebot_plugin_mixin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mixin
-Version: 0.1.1
+Version: 0.1.2
 Summary: 通过代码或非代码方式外部介入 NoneBot2 插件行为
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-mixin
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-mixin
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-mixin Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-mixin Version: 0.1.2 Summary:
 éè¿ä»£ç æéä»£ç æ¹å¼å¤é¨ä»å¥ NoneBot2 æä»¶è¡ä¸º Author-email:
 HivertMoZara
 163.com> License: MIT Project-URL: Homepage, https://github.com/NCBM/nonebot-
 plugin-mixin Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-
 mixin Requires-Python: >=3.8 Description-Content-Type: text/markdown License-
 File: LICENSE
 # nonebot-plugin-mixin _â¨ éè¿ä»£ç æéä»£ç æ¹å¼å¤é¨ä»å¥ NoneBot2
```

