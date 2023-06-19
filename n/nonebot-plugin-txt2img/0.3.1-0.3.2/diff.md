# Comparing `tmp/nonebot_plugin_txt2img-0.3.1.tar.gz` & `tmp/nonebot_plugin_txt2img-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_txt2img-0.3.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_txt2img-0.3.2.tar", max compression
```

## Comparing `nonebot_plugin_txt2img-0.3.1.tar` & `nonebot_plugin_txt2img-0.3.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1083 2023-01-07 12:36:54.628923 nonebot_plugin_txt2img-0.3.1/LICENSE
--rw-r--r--   0        0        0     2349 2023-02-12 13:56:40.792138 nonebot_plugin_txt2img-0.3.1/nonebot_plugin_txt2img/__init__.py
--rw-r--r--   0        0        0     3259 2023-04-22 13:44:08.530095 nonebot_plugin_txt2img-0.3.1/nonebot_plugin_txt2img/config.py
--rw-r--r--   0        0        0     8208 2023-02-12 13:57:11.657372 nonebot_plugin_txt2img-0.3.1/nonebot_plugin_txt2img/txt2img.py
--rw-r--r--   0        0        0      815 2023-04-22 13:45:23.730914 nonebot_plugin_txt2img-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4700 2023-04-22 13:46:28.057055 nonebot_plugin_txt2img-0.3.1/README.md
--rw-r--r--   0        0        0     5628 1970-01-01 00:00:00.000000 nonebot_plugin_txt2img-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-01-07 12:36:54.628923 nonebot_plugin_txt2img-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2143 2023-06-19 09:17:42.597166 nonebot_plugin_txt2img-0.3.2/nonebot_plugin_txt2img/__init__.py
+-rw-r--r--   0        0        0     3254 2023-06-19 09:23:37.720827 nonebot_plugin_txt2img-0.3.2/nonebot_plugin_txt2img/config.py
+-rw-r--r--   0        0        0     8202 2023-06-19 09:11:28.260282 nonebot_plugin_txt2img-0.3.2/nonebot_plugin_txt2img/txt2img.py
+-rw-r--r--   0        0        0      827 2023-06-19 09:28:45.990949 nonebot_plugin_txt2img-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4700 2023-04-22 13:46:28.057055 nonebot_plugin_txt2img-0.3.2/README.md
+-rw-r--r--   0        0        0     5640 1970-01-01 00:00:00.000000 nonebot_plugin_txt2img-0.3.2/PKG-INFO
```

### Comparing `nonebot_plugin_txt2img-0.3.1/LICENSE` & `nonebot_plugin_txt2img-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_txt2img-0.3.1/nonebot_plugin_txt2img/__init__.py` & `nonebot_plugin_txt2img-0.3.2/nonebot_plugin_txt2img/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,48 @@
-from nonebot import get_driver, on_command, on_metaevent
-from nonebot.adapters.onebot.v11 import Bot, LifecycleMetaEvent, MessageSegment
+from nonebot import get_driver, on_command, require
 from nonebot.log import logger
 from nonebot.params import ArgPlainText
 from nonebot.plugin import PluginMetadata
 from nonebot.rule import to_me
 
 from .config import download_template
 from .txt2img import Txt2Img
 
+require("nonebot_plugin_saa")
+from nonebot_plugin_saa import Image
+
 __plugin_meta__ = PluginMetadata(
     name="文字转图片",
     description="使用 Pillow 进行文字转图片",
     usage="""发送 txt2img 命令即可交互进行文字转图片""",
-    extra={"version": "0.3.0"},
+    type="library",
+    homepage="https://github.com/mobyw/nonebot-plugin-txt2img",
+    supported_adapters={
+        "~onebot.v11",
+        "~onebot.v12",
+        "~kaiheila",
+        "~qqguild",
+        "~telegram",
+    },
 )
 
-
-def check_first_connect(_: LifecycleMetaEvent) -> bool:
-    return True
-
-
-start_metaevent = on_metaevent(rule=check_first_connect, temp=True)
+driver = get_driver()
 
 
-@start_metaevent.handle()
-async def start(bot: Bot) -> None:
+@driver.on_startup
+async def start() -> None:
     logger.info("开始检查资源文件")
     flag = await download_template()
     if flag == 2:
         logger.info("模板文件完好")
     elif flag == 1:
         logger.info("模板文件下载完成")
     else:
         message = "模板文件下载失败，请尝试手动下载并放置到工程目录下的 data/TXT2IMG 文件夹中"
-        logger.warning(message)
-        try:
-            await bot.send_private_msg(
-                user_id=int(list(get_driver().config.superusers)[0]), message=message
-            )
-        except Exception as e:
-            logger.warning(f"发送提示消息失败: {e}")
+        logger.error(message)
 
 
 txt2img = on_command("txt2img", rule=to_me())
 
 
 @txt2img.got("TITLE", prompt="请输入标题（空格表示留空）")
 @txt2img.got("TEXT", prompt="请输入内容")
@@ -55,12 +54,14 @@
 ):
     if size.isdigit():
         if 20 <= int(size) <= 120:
             font_size = int(size)
             img = Txt2Img()
             img.set_font_size(font_size)
             pic = img.draw(title, text)
-            await txt2img.finish(MessageSegment.image(pic))  # type: ignore
+            msg_builder = Image(pic)
+            await msg_builder.send()
+            await txt2img.finish()
         else:
-            await txt2img.reject("字体大小需要在20到120之间，请重新输入")  # type: ignore
+            await txt2img.reject("字体大小需要在20到120之间，请重新输入")
     else:
-        await txt2img.reject("字体大小格式有误，请输入20到120之间的数字")  # type: ignore
+        await txt2img.reject("字体大小格式有误，请输入20到120之间的数字")
```

### Comparing `nonebot_plugin_txt2img-0.3.1/nonebot_plugin_txt2img/config.py` & `nonebot_plugin_txt2img-0.3.2/nonebot_plugin_txt2img/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 DATA_PATH = DATA_ROOT / "TXT2IMG"
 FONT_PATH = DATA_PATH / "font"
 IMAGE_PATH = DATA_PATH / "image"
 FONT_FILE = FONT_PATH / "sarasa-mono-sc-regular.ttf"
 MI_BACKGROUND_FILE = IMAGE_PATH / "mi_background.png"
 
 
-github_proxy = "https://github.moeyy.xyz/"
+github_proxy = "https://ghproxy.net/"
 data_url = (
     github_proxy
     + "https://raw.githubusercontent.com/mobyw/nonebot-plugin-txt2img/main/data/TXT2IMG"
 )
 font_url = data_url + "/font/sarasa-mono-sc-regular.ttf"
 mi_background_url = data_url + "/image/mi_background.png"
```

### Comparing `nonebot_plugin_txt2img-0.3.1/nonebot_plugin_txt2img/txt2img.py` & `nonebot_plugin_txt2img-0.3.2/nonebot_plugin_txt2img/txt2img.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
                     result += "\n"
         result = result.rstrip()
         return result
 
     def draw_img(
         self, title: str, text: str, template: Union[str, dict] = "mi"
     ) -> Image.Image:
-        """绘制给定模板模板下的图片"""
+        """绘制给定模板下的图片"""
 
         if isinstance(template, str):
             try:
                 template = templates[template]  # type: ignore
             except KeyError:
                 template = templates["mi"]  # type: ignore
```

### Comparing `nonebot_plugin_txt2img-0.3.1/pyproject.toml` & `nonebot_plugin_txt2img-0.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "nonebot-plugin-txt2img"
-version = "0.3.1"
+version = "0.3.2"
 description = "轻量文字转图片插件"
 authors = ["mobyw <mobyw66@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/mobyw/nonebot-plugin-txt2img"
 repository = "https://github.com/mobyw/nonebot-plugin-txt2img"
 documentation = "https://github.com/mobyw/nonebot-plugin-txt2img/blob/main/README.md"
 keywords = ["nonebot2", "qq", "plugin"]
 packages = [
     { include = "nonebot_plugin_txt2img" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-nonebot2 = {version = "^2.0.0rc1", extras = ["fastapi"]}
-nonebot-adapter-onebot = "^2.1.3"
+nonebot2 = {version = "^2.0.0", extras = ["fastapi"]}
 pillow = "^9.0.0"
 httpx = "^0.22.0"
+nonebot-plugin-send-anything-anywhere = "^0.2.7"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_txt2img-0.3.1/README.md` & `nonebot_plugin_txt2img-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_txt2img-0.3.1/PKG-INFO` & `nonebot_plugin_txt2img-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-txt2img
-Version: 0.3.1
+Version: 0.3.2
 Summary: 轻量文字转图片插件
 Home-page: https://github.com/mobyw/nonebot-plugin-txt2img
 License: MIT
 Keywords: nonebot2,qq,plugin
 Author: mobyw
 Author-email: mobyw66@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.22.0,<0.23.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.1.3,<3.0.0)
-Requires-Dist: nonebot2[fastapi] (>=2.0.0rc1,<3.0.0)
+Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.7,<0.3.0)
+Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
 Requires-Dist: pillow (>=9.0.0,<10.0.0)
 Project-URL: Documentation, https://github.com/mobyw/nonebot-plugin-txt2img/blob/main/README.md
 Project-URL: Repository, https://github.com/mobyw/nonebot-plugin-txt2img
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD033 MD036 MD041-->
 <p align="center">
```

