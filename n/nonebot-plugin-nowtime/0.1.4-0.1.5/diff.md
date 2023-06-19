# Comparing `tmp/nonebot_plugin_nowtime-0.1.4.tar.gz` & `tmp/nonebot_plugin_nowtime-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nowtime-0.1.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_nowtime-0.1.5.tar", max compression
```

## Comparing `nonebot_plugin_nowtime-0.1.4.tar` & `nonebot_plugin_nowtime-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1084 2023-01-08 02:12:09.783792 nonebot_plugin_nowtime-0.1.4/LICENSE
--rw-r--r--   0        0        0     5480 2023-01-09 01:53:27.293867 nonebot_plugin_nowtime-0.1.4/nonebot_plugin_nowtime/__init__.py
--rw-r--r--   0        0        0       29 2023-01-08 04:02:20.613764 nonebot_plugin_nowtime-0.1.4/nonebot_plugin_nowtime/config/nowtime.json
--rw-r--r--   0        0        0      185 2023-01-09 01:16:34.047613 nonebot_plugin_nowtime-0.1.4/nonebot_plugin_nowtime/config.py
--rw-r--r--   0        0        0     2640 2023-01-09 02:10:27.532201 nonebot_plugin_nowtime-0.1.4/nonebot_plugin_nowtime/resource/time_words.json
--rw-r--r--   0        0        0      734 2023-01-09 02:04:42.302545 nonebot_plugin_nowtime-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1629 2023-01-09 02:10:43.576438 nonebot_plugin_nowtime-0.1.4/README.md
--rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 nonebot_plugin_nowtime-0.1.4/setup.py
--rw-r--r--   0        0        0     2537 1970-01-01 00:00:00.000000 nonebot_plugin_nowtime-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-01-08 02:12:09.783792 nonebot_plugin_nowtime-0.1.5/LICENSE
+-rw-r--r--   0        0        0     6461 2023-06-19 08:50:48.175763 nonebot_plugin_nowtime-0.1.5/nonebot_plugin_nowtime/__init__.py
+-rw-r--r--   0        0        0       29 2023-01-08 04:02:20.613764 nonebot_plugin_nowtime-0.1.5/nonebot_plugin_nowtime/config/nowtime.json
+-rw-r--r--   0        0        0      185 2023-01-09 01:16:34.047613 nonebot_plugin_nowtime-0.1.5/nonebot_plugin_nowtime/config.py
+-rw-r--r--   0        0        0     2640 2023-01-09 02:10:27.532201 nonebot_plugin_nowtime-0.1.5/nonebot_plugin_nowtime/resource/time_words.json
+-rw-r--r--   0        0        0      733 2023-06-19 08:54:43.403356 nonebot_plugin_nowtime-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2102 2023-06-19 08:37:59.758354 nonebot_plugin_nowtime-0.1.5/README.md
+-rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 nonebot_plugin_nowtime-0.1.5/PKG-INFO
```

### Comparing `nonebot_plugin_nowtime-0.1.4/LICENSE` & `nonebot_plugin_nowtime-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nowtime-0.1.4/nonebot_plugin_nowtime/__init__.py` & `nonebot_plugin_nowtime-0.1.5/nonebot_plugin_nowtime/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,58 @@
-from nonebot.plugin import on_regex
+from nonebot.plugin import on_regex, PluginMetadata
 from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN, GROUP_OWNER
 from nonebot.permission import SUPERUSER
 from nonebot.params import Matcher, RegexGroup
-from nonebot import require,get_bot,get_driver
+from nonebot import require, get_bot, get_driver
 from nonebot.adapters.onebot.v11 import (
     Bot,
     MessageEvent,
     MessageSegment,
     GroupMessageEvent,
     ActionFailed,
 )
 from nonebot.log import logger
 from typing import Dict, List, Optional, Tuple
+from httpx import AsyncClient
 from pathlib import Path
 from datetime import datetime
 from .config import Config
 import asyncio
 import aiofiles
 import os
-import json
-import requests
-
+try:
+    import ujson as json
+except ModuleNotFoundError:
+    import json
+
+
+__plugin_meta__ = PluginMetadata(
+    name="整点报时",
+    description="每时每刻正点报时",
+    config=Config,
+    usage='''现在时间\n
+        查看整点报时列表\n
+        开启整点报时\n
+        关闭整点报时''',
+    type="application",
+    homepage="https://github.com/Cvandia/nonebot_plugin_nowtime",
+    supported_adapters={"~onebot.v11"},
+    extra={
+        "unique_name": "nonebot-plugin-nowtime",
+        "example":
+        """
+        现在时间\n
+        查看整点报时列表\n
+        开启整点报时\n
+        关闭整点报时
+        """,
+        "author": "divandia <106718176+Cvandia@users.noreply.github.com>",
+        "version": "0.1.5",
+    }
+)
 
 config_path = Path("config/nowtime.json")
 config_path.parent.mkdir(parents=True, exist_ok=True)
 if config_path.exists():
     with open(config_path, "r", encoding="utf8") as f:
         CONFIG: Dict[str, List] = json.load(f)
 else:
@@ -34,42 +62,46 @@
 
 try:
     scheduler = require("nonebot_plugin_apscheduler").scheduler
 except Exception:
     scheduler = None
 
 
-
-
 time_now = on_regex(r"(现在|当前|北京)时间", block=True, priority=5)
-trun_on_nowtime = on_regex(r"^(开启|关闭)整点报时([0-9]*)$", priority=99, block=True, permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER)
-list_matcher = on_regex(r"^查看整点报时列表$", priority=99, permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER)
+trun_on_nowtime = on_regex(r"^(开启|关闭)整点报时([0-9]*)$", priority=99,
+                           block=True, permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER)
+list_matcher = on_regex(r"^查看整点报时列表$", priority=99,
+                        permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER)
 
 
 @time_now.handle()
 async def _():
-    await time_now.send(message = "正在查看当前时间……")
-    get_json = requests.get(url='https://v.api.aa1.cn/api/time-tx/index.php',timeout=30)
+    await time_now.send(message="正在查看当前时间……")
+    async with AsyncClient() as client:
+        get_json = await client.get('https://v.api.aa1.cn/api/time-tx/index.php', timeout=30)
     get_msg = json.loads(get_json.text)
     msg = (f"⭐{get_msg['msg']}⭐\n"
-    +f"\n现在是北京时间:\n{get_msg['nowtime']}"
-    +f"送你一句：\n⭐{get_msg['nxyj']}⭐"
-    )
+           + f"\n现在是北京时间:\n{get_msg['nowtime']}"
+           + f"送你一句：\n⭐{get_msg['nxyj']}⭐"
+           )
     await time_now.send(message=(msg))
 
+
 @list_matcher.handle()
 async def _(bot: Bot, event: MessageEvent, matcher: Matcher):
     if not scheduler:
         await matcher.finish("未安装软依赖nonebot_plugin_apscheduler，不能使用定时发送功能")
     msg = "当前打开整点报时的群聊有：\n"
     for group_id in CONFIG["opened_groups"]:
         msg += f"{group_id}\n"
     await matcher.finish(msg.strip())
 
-#为群聊添加整点报时
+# 为群聊添加整点报时
+
+
 @trun_on_nowtime.handle()
 async def _(
     bot: Bot,
     event: MessageEvent,
     matcher: Matcher,
     args: Tuple[Optional[str], ...] = RegexGroup(),
 ):
@@ -94,58 +126,61 @@
         else:
             await matcher.finish("该群尚未开启，无需关闭")
     async with asyncio.Lock():
         async with aiofiles.open(config_path, "w", encoding="utf8") as f:
             await f.write(json.dumps(CONFIG, ensure_ascii=False, indent=4))
     await matcher.finish(f"已成功{mode}{group_id}的整点报时")
 
-#读取配置的开始和结束时间
+# 读取配置的开始和结束时间
 star_time = Config.parse_obj(get_driver().config.dict()).start_time
 end_time = Config.parse_obj(get_driver().config.dict()).end_time
 
-#发送报时
+# 发送报时
+
+
 async def post_scheduler():
     bot: Bot = get_bot()
     delay = 2 * 0.5
-    if datetime.now().hour in range(star_time,end_time):   
+    if datetime.now().hour in range(star_time, end_time):
         for group_id in CONFIG["opened_groups"]:
             try:
-            #整点语音
+                # 整点语音
                 url = 'https://v.api.aa1.cn/api/api-baoshi/data/baoshi/'
-                url = url +str(datetime.now().hour)+ '.mp3'
+                url = url + str(datetime.now().hour) + '.mp3'
                 record = MessageSegment.record(url)
                 await bot.send_group_msg(group_id=int(group_id), message=record)
             except ActionFailed as e:
                 logger.warning(f'{repr(e)}')
             await asyncio.sleep(delay)
             try:
                 msg = await get_word_result()
-                await bot.send_group_msg(group_id=int(group_id), message= msg) 
+                await bot.send_group_msg(group_id=int(group_id), message=msg)
             except ActionFailed as e:
-                logger.warning(f"定时发送整点报时到 {group_id} 失败，可能是风控或机器人不在该群聊 {repr(e)}")
+                logger.warning(
+                    f"定时发送整点报时到 {group_id} 失败，可能是风控或机器人不在该群聊 {repr(e)}")
             await asyncio.sleep(delay)
 
 
-
-#加载整点报时词库
+# 加载整点报时词库
 words_for_time = json.load(open(Path(os.path.join(os.path.dirname(
     __file__), "resource")) / "time_words.json", "r", encoding="utf8"))
 
-#匹配词库
+# 匹配词库
+
+
 async def get_word_result() -> str:
     keys = words_for_time.keys()
     for key in keys:
         try:
             if int(datetime.now().hour) == int(key):
                 return words_for_time[key]
-        except: 
+        except:
             return '整点报时出错了！'
 
 
-#添加定时任务
+# 添加定时任务
 try:
     scheduler.add_job(
         post_scheduler, "cron", hour='*', id="everyday_nowtime"
     )
 except ActionFailed as e:
-    logger.warning(f"定时任务添加失败，{repr(e)}")   
-
+    logger.warning(f"定时任务添加失败，{repr(e)}")
```

### Comparing `nonebot_plugin_nowtime-0.1.4/nonebot_plugin_nowtime/resource/time_words.json` & `nonebot_plugin_nowtime-0.1.5/nonebot_plugin_nowtime/resource/time_words.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nowtime-0.1.4/pyproject.toml` & `nonebot_plugin_nowtime-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "nonebot_plugin_nowtime"
-version = "0.1.4"
+version = "0.1.5"
 description = "Nonebot2 plugin for telling the time per hour"
-authors = ["Cvadia"]
+authors = ["Cvandia"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Cvandia/nonebot_plugin_nowtime"
 repository = "https://github.com/Cvandia/nonebot_plugin_nowtime"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 nonebot2 = ">=2.0.0-beta.1"
 nonebot-adapter-onebot = ">=2.0.0-beta.1"
 httpx = ">=0.19.0"
 aiofiles = ">=0.7.0"
 nonebot-plugin-apscheduler= ">=0.1.3"
-requests = ">=2.28.1"
 pydantic = ">=1.10.2"
+pathlib = ">=1.0.1"
 
 [tool.poetry.dev-dependencies]
 nb-cli = "^0.6.0"
 black = "^22.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `nonebot_plugin_nowtime-0.1.4/README.md` & `nonebot_plugin_nowtime-0.1.5/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 # nonebot-plugin-nowtime
 
 _⭐基于Nonebot2的一款整点报时的插件⭐_
 
 
 </div>
 
+<div align="center">
+<a href="https://www.python.org/downloads/release/python-390/"><img src="https://img.shields.io/badge/python-3.8+-blue"></a>  <a href=""><img src="https://img.shields.io/badge/QQ-1141538825-yellow"></a> <a href="https://github.com/Cvandia/nonebot_plugin_nowtime/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue"></a> <a href="https://v2.nonebot.dev/"><img src="https://img.shields.io/badge/Nonebot2-rc1+-red"></a>
+</div>
+
 
 ## ⭐ 介绍
 
 让机器人为你整点报时吧，
 由于本人第一次创建，有不足的地方还请指出
 
 ## 💿 安装
```

#### html2text {}

```diff
@@ -1,9 +1,12 @@
                               [NoneBotPluginLogo]
  # nonebot-plugin-nowtime _â­åºäºNonebot2çä¸æ¬¾æ´ç¹æ¥æ¶çæä»¶â­_
+[https://img.shields.io/badge/python-3.8+-blue] [https://img.shields.io/badge/
+QQ-1141538825-yellow] [https://img.shields.io/badge/license-MIT-blue] [https://
+                    img.shields.io/badge/Nonebot2-rc1+-red]
 ## â­ ä»ç» è®©æºå¨äººä¸ºä½ æ´ç¹æ¥æ¶å§ï¼
 ç±äºæ¬äººç¬¬ä¸æ¬¡åå»ºï¼æä¸è¶³çå°æ¹è¿è¯·æåº ## ð¿ å®è£
 nb-cliå®è£ å¨é¡¹ç®ç®å½æä»¶ä¸è¿è¡ ``` nb plugin install
 nonebot_plugin_nowtime ```   pipå®è£ ``` pip install nonebot-plugin-nowtime
 ```  ## âï¸ éç½® å¨å¨å±éç½®æä»¶`.env`ä¸­æ·»å å¦ä¸ ``` start_time
 = 8 end_time = 20 ```
 >é»è®¤ä¸éç½®ä¸º24å°æ¶å¨å¤©æ­æ¥ï¼æä»¥è§å¾å¾ç¦çè¯·èªè¡è®¾ç½®æ¶é´ï¼éç¨24å°æ¶å¶ï¼
```

### Comparing `nonebot_plugin_nowtime-0.1.4/PKG-INFO` & `nonebot_plugin_nowtime-0.1.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nowtime
-Version: 0.1.4
+Version: 0.1.5
 Summary: Nonebot2 plugin for telling the time per hour
 Home-page: https://github.com/Cvandia/nonebot_plugin_nowtime
 License: MIT
-Author: Cvadia
+Author: Cvandia
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=0.7.0)
 Requires-Dist: httpx (>=0.19.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.1.3)
 Requires-Dist: nonebot2 (>=2.0.0-beta.1)
+Requires-Dist: pathlib (>=1.0.1)
 Requires-Dist: pydantic (>=1.10.2)
-Requires-Dist: requests (>=2.28.1)
 Project-URL: Repository, https://github.com/Cvandia/nonebot_plugin_nowtime
 Description-Content-Type: text/markdown
 
 
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store"><img src="https://img.zcool.cn/community/014c9a55420cdc0000019ae952d851.jpg@1280w_1l_2o_100sh.jpg" width="180" height="180" alt="NoneBotPluginLogo"></a>
@@ -35,14 +35,18 @@
 # nonebot-plugin-nowtime
 
 _⭐基于Nonebot2的一款整点报时的插件⭐_
 
 
 </div>
 
+<div align="center">
+<a href="https://www.python.org/downloads/release/python-390/"><img src="https://img.shields.io/badge/python-3.8+-blue"></a>  <a href=""><img src="https://img.shields.io/badge/QQ-1141538825-yellow"></a> <a href="https://github.com/Cvandia/nonebot_plugin_nowtime/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue"></a> <a href="https://v2.nonebot.dev/"><img src="https://img.shields.io/badge/Nonebot2-rc1+-red"></a>
+</div>
+
 
 ## ⭐ 介绍
 
 让机器人为你整点报时吧，
 由于本人第一次创建，有不足的地方还请指出
 
 ## 💿 安装
```

#### html2text {}

```diff
@@ -1,23 +1,26 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nowtime Version: 0.1.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-nowtime Version: 0.1.5 Summary:
 Nonebot2 plugin for telling the time per hour Home-page: https://github.com/
-Cvandia/nonebot_plugin_nowtime License: MIT Author: Cvadia Requires-Python:
+Cvandia/nonebot_plugin_nowtime License: MIT Author: Cvandia Requires-Python:
 >=3.7 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: aiofiles (>=0.7.0) Requires-Dist: httpx (>=0.19.0) Requires-Dist:
 nonebot-adapter-onebot (>=2.0.0-beta.1) Requires-Dist: nonebot-plugin-
 apscheduler (>=0.1.3) Requires-Dist: nonebot2 (>=2.0.0-beta.1) Requires-Dist:
-pydantic (>=1.10.2) Requires-Dist: requests (>=2.28.1) Project-URL: Repository,
+pathlib (>=1.0.1) Requires-Dist: pydantic (>=1.10.2) Project-URL: Repository,
 https://github.com/Cvandia/nonebot_plugin_nowtime Description-Content-Type:
 text/markdown
                               [NoneBotPluginLogo]
  # nonebot-plugin-nowtime _â­åºäºNonebot2çä¸æ¬¾æ´ç¹æ¥æ¶çæä»¶â­_
+[https://img.shields.io/badge/python-3.8+-blue] [https://img.shields.io/badge/
+QQ-1141538825-yellow] [https://img.shields.io/badge/license-MIT-blue] [https://
+                    img.shields.io/badge/Nonebot2-rc1+-red]
 ## â­ ä»ç» è®©æºå¨äººä¸ºä½ æ´ç¹æ¥æ¶å§ï¼
 ç±äºæ¬äººç¬¬ä¸æ¬¡åå»ºï¼æä¸è¶³çå°æ¹è¿è¯·æåº ## ð¿ å®è£
 nb-cliå®è£ å¨é¡¹ç®ç®å½æä»¶ä¸è¿è¡ ``` nb plugin install
 nonebot_plugin_nowtime ```   pipå®è£ ``` pip install nonebot-plugin-nowtime
 ```  ## âï¸ éç½® å¨å¨å±éç½®æä»¶`.env`ä¸­æ·»å å¦ä¸ ``` start_time
 = 8 end_time = 20 ```
 >é»è®¤ä¸éç½®ä¸º24å°æ¶å¨å¤©æ­æ¥ï¼æä»¥è§å¾å¾ç¦çè¯·èªè¡è®¾ç½®æ¶é´ï¼éç¨24å°æ¶å¶ï¼
```

