# Comparing `tmp/nonebot_plugin_setu_now-0.5.0a2.tar.gz` & `tmp/nonebot_plugin_setu_now-0.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_setu_now-0.5.0a2.tar", max compression
+gzip compressed data, was "nonebot_plugin_setu_now-0.6.0b1.tar", last modified: Mon Jun 19 12:45:51 2023, max compression
```

## Comparing `nonebot_plugin_setu_now-0.5.0a2.tar` & `nonebot_plugin_setu_now-0.6.0b1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1062 2023-04-03 03:09:57.810706 nonebot_plugin_setu_now-0.5.0a2/LICENSE
--rw-r--r--   0        0        0     3403 2023-04-03 03:09:57.810706 nonebot_plugin_setu_now-0.5.0a2/README.md
--rwxr-xr-x   0        0        0     7420 2023-04-03 03:09:57.810706 nonebot_plugin_setu_now-0.5.0a2/nonebot_plugin_setu_now/__init__.py
--rw-r--r--   0        0        0      305 2023-04-03 03:09:57.810706 nonebot_plugin_setu_now-0.5.0a2/nonebot_plugin_setu_now/aioutils/__init__.py
--rw-r--r--   0        0        0     3922 2023-04-03 03:09:57.810706 nonebot_plugin_setu_now-0.5.0a2/nonebot_plugin_setu_now/aioutils/_main.py
--rw-r--r--   0        0        0     1030 2023-04-03 03:09:57.810706 nonebot_plugin_setu_now-0.5.0a2/nonebot_plugin_setu_now/config.py
--rw-r--r--   0        0        0     2416 2023-04-03 03:09:57.810706 nonebot_plugin_setu_now-0.5.0a2/nonebot_plugin_setu_now/data_source.py
--rw-r--r--   0        0        0      906 2023-04-03 03:09:57.810706 nonebot_plugin_setu_now-0.5.0a2/nonebot_plugin_setu_now/database.py
--rw-r--r--   0        0        0     4260 2023-04-03 03:09:57.810706 nonebot_plugin_setu_now-0.5.0a2/nonebot_plugin_setu_now/img_utils.py
--rw-r--r--   0        0        0     1592 2023-04-03 03:09:57.810706 nonebot_plugin_setu_now-0.5.0a2/nonebot_plugin_setu_now/models.py
--rw-r--r--   0        0        0      613 2023-04-03 03:09:57.810706 nonebot_plugin_setu_now-0.5.0a2/nonebot_plugin_setu_now/perf_timer.py
--rw-r--r--   0        0        0     2032 2023-04-03 03:09:57.810706 nonebot_plugin_setu_now-0.5.0a2/nonebot_plugin_setu_now/r18_whitelist.py
--rw-r--r--   0        0        0     2895 2023-04-03 03:09:57.810706 nonebot_plugin_setu_now-0.5.0a2/nonebot_plugin_setu_now/utils.py
--rw-r--r--   0        0        0      667 2023-04-03 03:09:57.810706 nonebot_plugin_setu_now-0.5.0a2/pyproject.toml
--rw-r--r--   0        0        0     4296 1970-01-01 00:00:00.000000 nonebot_plugin_setu_now-0.5.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/LICENSE
+-rw-r--r--   0        0        0     3403 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/README.md
+-rwxr-xr-x   0        0        0     7447 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/__init__.py
+-rw-r--r--   0        0        0      305 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/aioutils/__init__.py
+-rw-r--r--   0        0        0     3922 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/aioutils/_main.py
+-rw-r--r--   0        0        0     1030 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/config.py
+-rw-r--r--   0        0        0     2410 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/data_source.py
+-rw-r--r--   0        0        0     1123 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/database.py
+-rw-r--r--   0        0        0     4274 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/img_utils.py
+-rw-r--r--   0        0        0      959 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/models.py
+-rw-r--r--   0        0        0      613 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/perf_timer.py
+-rw-r--r--   0        0        0     1711 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/r18_whitelist.py
+-rw-r--r--   0        0        0     3031 2023-06-19 12:45:37.659352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/utils.py
+-rw-r--r--   0        0        0      806 2023-06-19 12:45:51.367339 nonebot_plugin_setu_now-0.6.0b1/pyproject.toml
+-rw-r--r--   0        0        0     4035 1970-01-01 00:00:00.000000 nonebot_plugin_setu_now-0.6.0b1/PKG-INFO
```

### Comparing `nonebot_plugin_setu_now-0.5.0a2/LICENSE` & `nonebot_plugin_setu_now-0.6.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.5.0a2/README.md` & `nonebot_plugin_setu_now-0.6.0b1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.5.0a2/nonebot_plugin_setu_now/__init__.py` & `nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,59 @@
 import asyncio
 from re import I, sub
-from typing import Union
+from typing import Any, Union, Annotated
 from pathlib import Path
 
 from PIL import UnidentifiedImageError
 from nonebot import on_regex, on_command
-from sqlalchemy import select
 from nonebot.log import logger
-from nonebot.params import Depends
-from nonebot.plugin import require
-from nonebot.typing import T_State
+from nonebot.params import Depends, RegexGroup
+from nonebot.plugin import PluginMetadata, require
 from nonebot.exception import ActionFailed
-from nonebot.adapters.onebot.v11 import GROUP, PRIVATE_FRIEND, Bot, Message, MessageEvent, MessageSegment, GroupMessageEvent, PrivateMessageEvent
-from sqlalchemy.ext.asyncio.session import AsyncSession
-from nonebot.adapters.onebot.v11.helpers import Cooldown, CooldownIsolateLevel, autorevoke_send
+from nonebot.adapters.onebot.v11 import (
+    GROUP,
+    PRIVATE_FRIEND,
+    Bot,
+    Message,
+    MessageEvent,
+    MessageSegment,
+    GroupMessageEvent,
+    PrivateMessageEvent,
+)
+from nonebot.adapters.onebot.v11.helpers import (
+    Cooldown,
+    CooldownIsolateLevel,
+    autorevoke_send,
+)
 
 from .utils import SpeedLimiter
-from .config import MAX, CDTIME, EFFECT, SETU_PATH, WITHDRAW_TIME
-from .models import Setu, SetuInfo, MessageInfo, SetuNotFindError
-from .database import bind_message_data, auto_upgrade_setuinfo
+from .config import MAX, CDTIME, EFFECT, SETU_PATH, WITHDRAW_TIME, Config
+from .models import Setu, SetuNotFindError
+from .database import SetuInfo, MessageInfo, bind_message_data, auto_upgrade_setuinfo
 from .img_utils import EFFECT_FUNC_LIST, image_segment_convert
 from .perf_timer import PerfTimer
 from .data_source import SetuHandler
 from .r18_whitelist import get_group_white_list_record
 
-require("nonebot_plugin_datastore")
+usage_msg = """TL;DR: 色图 或 看文档"""
+
+__plugin_meta__ = PluginMetadata(
+    name="nonebot-plugin-setu-now",
+    description="另一个色图插件",
+    usage=usage_msg,
+    type="application",
+    config=Config,
+    extra={},
+)
+
 require("nonebot_plugin_localstore")
+require("nonebot_plugin_tortoise_orm")
+from nonebot_plugin_tortoise_orm import add_model
 
-from nonebot_plugin_datastore import get_session, create_session
+add_model("nonebot_plugin_setu_now.database")
 
 global_speedlimiter = SpeedLimiter()
 
 setu_matcher = on_regex(
     r"^(setu|色图|涩图|来点色色|色色|涩涩|来点色图)\s?([x|✖️|×|X|*]?\d+[张|个|份]?)?\s?(r18)?\s?\s?(tag)?\s?(.*)?",
     flags=I,
     permission=PRIVATE_FRIEND | GROUP,
@@ -46,20 +68,22 @@
             isolate_level=CooldownIsolateLevel.USER,
         )
     ]
 )
 async def _(
     bot: Bot,
     event: Union[PrivateMessageEvent, GroupMessageEvent],
-    state: T_State,
+    # state: T_State,
+    regex_group: Annotated[tuple[Any, ...], RegexGroup()],
     white_list_record=Depends(get_group_white_list_record),
 ):
     # await setu_matcher.finish("服务器维护喵，暂停服务抱歉喵")
     setu_total_timer = PerfTimer("Image request total")
-    args = list(state["_matched_groups"])
+    args = list(regex_group)
+    logger.debug(f"args={args}")
     num = args[1]
     r18 = args[2]
     tags = args[3]
     key = args[4]
 
     num = int(sub(r"[张|个|份|x|✖️|×|X|*]", "", num)) if num else 1
     num = min(num, MAX)
@@ -111,21 +135,23 @@
             try:
                 await global_speedlimiter.async_speedlimit()
                 send_timer = PerfTimer("Image send")
                 message_id = 0
                 if not WITHDRAW_TIME:
                     # 未设置撤回时间 正常发送
                     message_id: int = (await setu_matcher.send(msg))["message_id"]
-                    async with create_session() as temp_db_session:
-                        await auto_upgrade_setuinfo(temp_db_session, setu)
-                        await bind_message_data(temp_db_session, message_id, setu.pid)
+
+                    await auto_upgrade_setuinfo(setu)
+                    await bind_message_data(message_id, setu.pid)
                     logger.debug(f"Message ID: {message_id}")
                 else:
                     logger.debug(f"Using auto revoke API, interval: {WITHDRAW_TIME}")
-                    await autorevoke_send(bot=bot, event=event, message=msg, revoke_interval=WITHDRAW_TIME)
+                    await autorevoke_send(
+                        bot=bot, event=event, message=msg, revoke_interval=WITHDRAW_TIME
+                    )
                 """
                 发送成功
                 """
                 send_timer.stop()
                 global_speedlimiter.send_success()
                 if SETU_PATH is None:  # 未设置缓存路径，删除缓存
                     Path(setu.img).unlink()
@@ -155,31 +181,35 @@
 
 setuinfo_matcher = on_command("信息")
 
 
 @setuinfo_matcher.handle()
 async def _(
     event: MessageEvent,
-    db_session: AsyncSession = Depends(get_session),
 ):
     logger.debug("Running setu info handler")
     event_message = event.original_message
     reply_segment = event_message["reply"]
+
     if reply_segment == []:
         logger.debug("Command invalid: Not specified setu info to get!")
         await setuinfo_matcher.finish("请直接回复需要作品信息的插画")
+
     reply_segment = reply_segment[0]
     reply_message_id = reply_segment.data["id"]
+
     logger.debug(f"Get setu info for message id: {reply_message_id}")
-    statement = select(MessageInfo).where(MessageInfo.message_id == reply_message_id)
-    messageinfo_result: MessageInfo = (await db_session.scalars(statement)).first()  # type: ignore
-    if not messageinfo_result:
+
+    if message_info := await MessageInfo.get_or_none(message_id=reply_message_id):
+        message_pid = message_info.pid
+    else:
         await setuinfo_matcher.finish("未找到该插画相关信息")
-    message_pid = messageinfo_result.pid
-    statement = select(SetuInfo).where(SetuInfo.pid == message_pid)
-    setu_info = (await db_session.scalars(statement)).first()  # type: ignore
-    if not setu_info:
+
+    if setu_info := await SetuInfo.get_or_none(pid=message_pid):
+
+        info_message = MessageSegment.text(f"标题：{setu_info.title}\n")
+        info_message += MessageSegment.text(f"画师：{setu_info.author}\n")
+        info_message += MessageSegment.text(f"PID：{setu_info.pid}")
+
+        await setu_matcher.finish(MessageSegment.reply(reply_message_id) + info_message)
+    else:
         await setuinfo_matcher.finish("该插画相关信息已被移除")
-    info_message = MessageSegment.text(f"标题：{setu_info.title}\n")
-    info_message += MessageSegment.text(f"画师：{setu_info.author}\n")
-    info_message += MessageSegment.text(f"PID：{setu_info.pid}")
-    await setu_matcher.finish(MessageSegment.reply(reply_message_id) + info_message)
```

### Comparing `nonebot_plugin_setu_now-0.5.0a2/nonebot_plugin_setu_now/aioutils/_main.py` & `nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/aioutils/_main.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import sys
 import functools
+import sys
 from typing import (
     Any,
     Awaitable,
     Callable,
     Coroutine,
     Dict,
     Generic,
```

### Comparing `nonebot_plugin_setu_now-0.5.0a2/nonebot_plugin_setu_now/config.py` & `nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 
 from nonebot import get_driver
-from pydantic import Extra, BaseModel
+from pydantic import BaseModel, Extra
 
 
 class Config(BaseModel, extra=Extra.ignore):
     superusers: set
     debug: Optional[bool] = False
     setu_cd: int = 60
     setu_path: Optional[str] = None
```

### Comparing `nonebot_plugin_setu_now-0.5.0a2/nonebot_plugin_setu_now/data_source.py` & `nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/data_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import List, Callable
 from asyncio import gather
 from pathlib import Path
 
+import nonebot_plugin_localstore as store
 from httpx import AsyncClient
+
 from nonebot import require
 from nonebot.log import logger
 
 from .utils import download_pic
-from .config import API_URL, REVERSE_PROXY, PROXY, SETU_SIZE, EFFECT
+from .config import PROXY, API_URL, SETU_SIZE, REVERSE_PROXY
 from .models import Setu, SetuApiData, SetuNotFindError
 
 
-require("nonebot_plugin_localstore")
-
-import nonebot_plugin_localstore as store
+require("nonebot_plugin_tortoise_orm")
 
 CACHE_PATH = Path(store.get_cache_dir("nonebot_plugin_setu_now"))
 if not CACHE_PATH.exists():
     logger.info("Creating setu cache floder")
     CACHE_PATH.mkdir(parents=True, exist_ok=True)
```

### Comparing `nonebot_plugin_setu_now-0.5.0a2/nonebot_plugin_setu_now/img_utils.py` & `nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/img_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import time
 from io import BytesIO
+from pathlib import Path
 from random import choice, randint
 from typing import Union
-from pathlib import Path
 
-from PIL import Image, ImageFilter
-from nonebot.log import logger
 from nonebot.adapters.onebot.v11 import MessageSegment
+from nonebot.log import logger
+from PIL import Image, ImageFilter
 
 from .perf_timer import PerfTimer
 
 
 def image_param_converter(source: Union[Path, Image.Image, bytes]) -> Image.Image:
     FORCE_RESIZE = True
     IMAGE_RESIZE_RES = 1080  # 限制被处理图片最大为1080P
@@ -51,15 +51,17 @@
     resize_resoluation = (
         int(img.width * (BLUR_HEIGHT_QUALITY / img.height)),
         BLUR_HEIGHT_QUALITY,
     )
     background = img
     background = background.resize(resize_resoluation)
     background = background.filter(ImageFilter.GaussianBlur(6))
-    background = background.resize((int(img.width * FRAME_RATIO), int(img.height * FRAME_RATIO)))
+    background = background.resize(
+        (int(img.width * FRAME_RATIO), int(img.height * FRAME_RATIO))
+    )
     background.paste(
         img,
         (
             int((background.width - img.width) / 2),
             int((background.height - img.height) / 2),
         ),
     )
```

### Comparing `nonebot_plugin_setu_now-0.5.0a2/nonebot_plugin_setu_now/perf_timer.py` & `nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/perf_timer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.5.0a2/nonebot_plugin_setu_now/utils.py` & `nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,27 +12,38 @@
 from .perf_timer import PerfTimer
 
 require("nonebot_plugin_localstore")
 
 import nonebot_plugin_localstore as store
 
 
-async def download_pic(url: str, proxies: Optional[str] = None, file_mode=False, file_name="") -> Optional[Path]:
+async def download_pic(
+    url: str, proxies: Optional[str] = None, file_mode=False, file_name=""
+) -> Optional[Path]:
     headers = {
         "Referer": "https://accounts.pixiv.net/login?lang=zh&source=pc&view_type=page&ref=wwwtop_accounts_index",
-        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) " "AppleWebKit/537.36 (KHTML, like Gecko) Chrome/56.0.2924.87 Safari/537.36",
+        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) "
+        "AppleWebKit/537.36 (KHTML, like Gecko) Chrome/56.0.2924.87 Safari/537.36",
     }
     download_timer = PerfTimer.start("Image download")
-    image_path = store.get_cache_file("nonebot_plugin_setu_now", file_name) if SETU_PATH is None else Path(SETU_PATH, file_name)
+    image_path = (
+        store.get_cache_file("nonebot_plugin_setu_now", file_name)
+        if SETU_PATH is None
+        else Path(SETU_PATH, file_name)
+    )
     client = AsyncClient(proxies=proxies, timeout=5)
     try:
         async with client.stream(method="GET", url=url, headers=headers, timeout=15) as response:  # type: ignore # params={"proxies": [proxies]}
             if response.status_code != 200:
-                logger.warning(f"Image respond status code error: {response.status_code}")
-                raise ValueError(f"Image respond status code error: {response.status_code}")
+                logger.warning(
+                    f"Image respond status code error: {response.status_code}"
+                )
+                raise ValueError(
+                    f"Image respond status code error: {response.status_code}"
+                )
             with open(image_path, "wb") as f:
                 async for chunk in response.aiter_bytes():
                     f.write(chunk)
     except Exception:
         logger.warning(f"Image download failed: {url}")
         return None
     finally:
@@ -61,15 +72,17 @@
       * `msgs: List[Message]`: 消息列表
     """
 
     def to_json(msg: Message):
         return {"type": "node", "data": {"name": name, "uin": uin, "content": msg}}
 
     messages = [to_json(msg) for msg in msgs]
-    await bot.call_api("send_group_forward_msg", group_id=event.group_id, messages=messages)
+    await bot.call_api(
+        "send_group_forward_msg", group_id=event.group_id, messages=messages
+    )
 
 
 class SpeedLimiter:
     def __init__(self) -> None:
         self.send_success_time = 0
 
     def send_success(self) -> None:
```

### Comparing `nonebot_plugin_setu_now-0.5.0a2/PKG-INFO` & `nonebot_plugin_setu_now-0.6.0b1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-setu-now
-Version: 0.5.0a2
+Version: 0.6.0b1
 Summary: 另一个色图插件
 Home-page: https://github.com/kexue-z/nonebot-plugin-setu-now
+Author-Email: kexue <xana278@foxmail.com>
 License: MIT
-Author: kexue
-Author-email: x@kexue-cloud.cn
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: httpx (>=0.18.0,<1.0.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1)
-Requires-Dist: nonebot-plugin-datastore (>=0.6.0)
-Requires-Dist: nonebot-plugin-localstore (>=0.3.0)
-Requires-Dist: nonebot2 (>=2.0.0-beta.1)
-Requires-Dist: pillow (>=8.0.0)
-Requires-Dist: pydantic (>=1.5.0)
+Project-URL: Homepage, https://github.com/kexue-z/nonebot-plugin-setu-now
+Requires-Python: <4.0,>=3.8
+Requires-Dist: httpx<1.0.0,>=0.18.0
+Requires-Dist: nonebot2>=2.0.0
+Requires-Dist: nonebot-adapter-onebot>=2.0.0
+Requires-Dist: pydantic>=1.5.0
+Requires-Dist: pillow>=8.0.0
+Requires-Dist: nonebot-plugin-tortoise-orm>=0.0.1a3
+Requires-Dist: nonebot-plugin-localstore>=0.5.0
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://user-images.githubusercontent.com/44545625/209862575-acdc9feb-3c76-471d-ad89-cc78927e5875.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
 </p>
 
 <div align="center">
@@ -136,8 +130,7 @@
   - `涩涩10份魅魔`
 
 # 在吗？
 
 - 这个是 `on_regex` 而不是 `on_command`（不需要带命令前缀）
 - 本插件一般都经过测试后才发版，如果遇到了任何问题，请先自行解决
 - 任何`不正确使用插件`的 issue 将会直接关闭
-
```

#### html2text {}

```diff
@@ -1,19 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-setu-now Version: 0.5.0a2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-setu-now Version: 0.6.0b1 Summary:
 å¦ä¸ä¸ªè²å¾æä»¶ Home-page: https://github.com/kexue-z/nonebot-plugin-
-setu-now License: MIT Author: kexue Author-email: x@kexue-cloud.cn Requires-
-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: httpx (>=0.18.0,<1.0.0) Requires-
-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1) Requires-Dist: nonebot-plugin-
-datastore (>=0.6.0) Requires-Dist: nonebot-plugin-localstore (>=0.3.0)
-Requires-Dist: nonebot2 (>=2.0.0-beta.1) Requires-Dist: pillow (>=8.0.0)
-Requires-Dist: pydantic (>=1.5.0) Description-Content-Type: text/markdown
+setu-now Author-Email: kexue
+foxmail.com> License: MIT Project-URL: Homepage, https://github.com/kexue-z/
+nonebot-plugin-setu-now Requires-Python: <4.0,>=3.8 Requires-Dist:
+httpx<1.0.0,>=0.18.0 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-
+adapter-onebot>=2.0.0 Requires-Dist: pydantic>=1.5.0 Requires-Dist:
+pillow>=8.0.0 Requires-Dist: nonebot-plugin-tortoise-orm>=0.0.1a3 Requires-
+Dist: nonebot-plugin-localstore>=0.5.0 Description-Content-Type: text/markdown
                               [NoneBotPluginLogo]
            # nonebot-plugin-setu-now _â¨ NoneBot2 æ¶©å¾æä»¶ â¨_
                            [license] [pypi] [python]
 ## ç®ä» å¯éè¿ç¾¤èæç§èè·å Pixiv æ¶©å¾ç NoneBot2 æä»¶ ##
 ç¹è² - **æé«çæ¶©å¾åéæåçï¼ä»é0.5.0ä»¥ä¸æ°çæ¬ï¼** -
 éè¿åå¤è·åå¾çä¿¡æ¯ - èªå¨æ¤åæ¶©å¾ - R18ç½ååç¾¤ç» -
 èªå¨æ¤åæ¶©å¾ - ç¬ç«çä¸è½½åéä»»å¡ç»æï¼éåº¦æ´å¿« ## å®è£
```

