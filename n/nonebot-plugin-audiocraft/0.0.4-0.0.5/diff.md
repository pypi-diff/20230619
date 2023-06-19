# Comparing `tmp/nonebot_plugin_audiocraft-0.0.4.tar.gz` & `tmp/nonebot_plugin_audiocraft-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_audiocraft-0.0.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_audiocraft-0.0.5.tar", max compression
```

## Comparing `nonebot_plugin_audiocraft-0.0.4.tar` & `nonebot_plugin_audiocraft-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1752 2023-06-11 04:58:20.222484 nonebot_plugin_audiocraft-0.0.4/README.md
--rw-r--r--   0        0        0     6148 2023-06-10 13:04:05.827943 nonebot_plugin_audiocraft-0.0.4/nonebot_plugin_audiocraft/.DS_Store
--rw-r--r--   0        0        0     2579 2023-06-11 04:58:30.170828 nonebot_plugin_audiocraft-0.0.4/nonebot_plugin_audiocraft/__init__.py
--rw-r--r--   0        0        0      545 2023-06-11 04:58:44.244079 nonebot_plugin_audiocraft-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2534 1970-01-01 00:00:00.000000 nonebot_plugin_audiocraft-0.0.4/setup.py
--rw-r--r--   0        0        0     2450 1970-01-01 00:00:00.000000 nonebot_plugin_audiocraft-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1751 2023-06-19 10:48:22.257138 nonebot_plugin_audiocraft-0.0.5/README.md
+-rw-r--r--   0        0        0     2838 2023-06-19 10:55:07.686259 nonebot_plugin_audiocraft-0.0.5/nonebot_plugin_audiocraft/__init__.py
+-rw-r--r--   0        0        0      564 2023-06-19 10:55:59.363807 nonebot_plugin_audiocraft-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2559 1970-01-01 00:00:00.000000 nonebot_plugin_audiocraft-0.0.5/setup.py
+-rw-r--r--   0        0        0     2489 1970-01-01 00:00:00.000000 nonebot_plugin_audiocraft-0.0.5/PKG-INFO
```

### Comparing `nonebot_plugin_audiocraft-0.0.4/README.md` & `nonebot_plugin_audiocraft-0.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   plugin_dirs = ["xxxxxx","xxxxxx",......,"下载完成的插件路径/nonebot-plugin-audiocraft"]
   ```
 * 使用 pip
   ```
   pip install nonebot-plugin-audiocraft
   ```
 # 后端服务器部署
-参考[官方仓库](https://github.com/facebookresearch/audiocraft#usage)部署好gradio后端，获得后端网址。（coblab上部署的可以开启gradio的外链分享）
+参考[官方仓库](https://github.com/facebookresearch/audiocraft#usage)部署好gradio后端，获得后端网址。（colab上部署的可以开启gradio的外链分享）
 
 
 # 使用方法
 
 - 由于最近tx风控严重，go-cqhttp面临重启后可能掉账号的风险，所以插件使用给机器人发送消息配置后端服务器配置的方法。
 - 每次重启机器人后，使用 %%后端服务器地址 绑定audiocraft后端服务器。
 - 绑定后端服务器后，使用 AI作曲+乐曲的英文描述 即可触发AI作曲。
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 æå¨å®è£ ``` git clone https://github.com/Alpaca4610/
 nonebot_plugin_audiocraft.git ```
 ä¸è½½å®æåå¨boté¡¹ç®çpyproject.tomlæä»¶æå¨æ·»å æä»¶ï¼ ```
 plugin_dirs = ["xxxxxx","xxxxxx",......,"ä¸è½½å®æçæä»¶è·¯å¾/nonebot-
 plugin-audiocraft"] ``` * ä½¿ç¨ pip ``` pip install nonebot-plugin-audiocraft
 ``` # åç«¯æå¡å¨é¨ç½² åè[å®æ¹ä»åº](https://github.com/
 facebookresearch/
-audiocraft#usage)é¨ç½²å¥½gradioåç«¯ï¼è·å¾åç«¯ç½åãï¼coblabä¸é¨ç½²çå¯ä»¥å¼å¯gradioçå¤é¾åäº«ï¼
+audiocraft#usage)é¨ç½²å¥½gradioåç«¯ï¼è·å¾åç«¯ç½åãï¼colabä¸é¨ç½²çå¯ä»¥å¼å¯gradioçå¤é¾åäº«ï¼
 # ä½¿ç¨æ¹æ³ - ç±äºæè¿txé£æ§ä¸¥éï¼go-
 cqhttpé¢ä¸´éå¯åå¯è½æè´¦å·çé£é©ï¼æä»¥æä»¶ä½¿ç¨ç»æºå¨äººåéæ¶æ¯éç½®åç«¯æå¡å¨éç½®çæ¹æ³ã
 - æ¯æ¬¡éå¯æºå¨äººåï¼ä½¿ç¨ %%åç«¯æå¡å¨å°å
 ç»å®audiocraftåç«¯æå¡å¨ã - ç»å®åç«¯æå¡å¨åï¼ä½¿ç¨
 AIä½æ²+ä¹æ²çè±ææè¿° å³å¯è§¦åAIä½æ²ã -
 AIä½æ²çåæ°ï¼å¦æ¨¡åãæ¶é¿ï¼ç­éè¿ä»£ç è¿è¡ä¿®æ¹ï¼ä»£ç ä¸­ææ³¨éè¯´æã
 # ææ ![Alt](demo1.png) ![Alt](demo2.png)
```

### Comparing `nonebot_plugin_audiocraft-0.0.4/nonebot_plugin_audiocraft/__init__.py` & `nonebot_plugin_audiocraft-0.0.5/nonebot_plugin_audiocraft/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import io
 from gradio_client import Client
 import nonebot
+import asyncio
 
 from nonebot.plugin import PluginMetadata
 from nonebot import on_command
 from nonebot.params import CommandArg
 from nonebot.adapters.onebot.v11 import Message, MessageSegment
 
 
@@ -33,40 +34,50 @@
     if content == "" or content is None:
         await direct.finish(MessageSegment.text("内容不能为空！"))
     if url == "" or url is None:
         await direct.finish(MessageSegment.text("未设置服务器！"))
 
     await direct.send(MessageSegment.text("audiocraft正在努力作曲中......"))
 
+    try:
+        loop = asyncio.get_event_loop()
+        result = await loop.run_in_executor(None, getMusic, content)
+
+    except Exception as error:
+        await direct.finish(str(error))
+
+    with open(result, "rb") as file:
+        file_content = file.read()
+        audio = io.BytesIO(file_content) 
+        await direct.finish(MessageSegment.record(file=audio))
+
+def getMusic(content):
     client = Client(url)
     result = client.predict(
                     "small",	# str  in 'Model' Radio component
                     content,	# str  in 'Input Text' Textbox component
                     "",	# str (filepath or URL to file) in 'Melody Condition (optional)' Audio component
                     6,	# int | float (numeric value between 1 and 30) in 'Duration' Slider component
                     250,	# int | float  in 'Top-k' Number component
                     0,	# int | float  in 'Top-p' Number component
                     1,	# int | float  in 'Temperature' Number component
                     3,	# int | float  in 'Classifier Free Guidance' Number component
                     fn_index=0
     )
     print(result)
-
-
-    with open(result, "rb") as file:
-        file_content = file.read()
-        audio = io.BytesIO(file_content) 
-        await direct.finish(MessageSegment.record(file=audio))
+    return result
 
 
 config_url = on_command("%%", block=False, priority=1)
 
 
 @config_url.handle()
 async def _(msg: Message = CommandArg()):
     global url
     url_ = msg.extract_plain_text()
     if url_ == "" or url_ is None:
         await config_url.finish(MessageSegment.text("内容不能为空！"))
     url = url_
     await config_url.finish(MessageSegment.text(f"成功设置地址为{url_}"))
 
+
+
```

### Comparing `nonebot_plugin_audiocraft-0.0.4/pyproject.toml` & `nonebot_plugin_audiocraft-0.0.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "nonebot-plugin-audiocraft"
-version = "0.0.4"
+version = "0.0.5"
 description = "A nonebot plugin for facebook's audiocraft"
 authors = ["Alpaca <alpaca@bupt.edu.cn>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = "^2.0.0rc3"
 nonebot-adapter-onebot = "^2.2.1"
 gradio-client = "^0.2.5"
+asyncio = "^3.4.3"
 
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple/"
 default = true
```

### Comparing `nonebot_plugin_audiocraft-0.0.4/setup.py` & `nonebot_plugin_audiocraft-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 packages = \
 ['nonebot_plugin_audiocraft']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['gradio-client>=0.2.5,<0.3.0',
+['asyncio>=3.4.3,<4.0.0',
+ 'gradio-client>=0.2.5,<0.3.0',
  'nonebot-adapter-onebot>=2.2.1,<3.0.0',
  'nonebot2>=2.0.0rc3,<3.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-audiocraft',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': "A nonebot plugin for facebook's audiocraft",
-    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-audiocraft\n</div>\n\n# 介绍\n- 本插件适配[Facebook开源的AI作曲模型](https://github.com/facebookresearch/audiocraft/)，在nonebot框架下调用已经部署好的模型后端服务器API进行AI作曲\n- 本插件需要配合部署好的audiocraft进行使用\n\n# 安装\n\n* 手动安装\n  ```\n  git clone https://github.com/Alpaca4610/nonebot_plugin_audiocraft.git\n  ```\n\n  下载完成后在bot项目的pyproject.toml文件手动添加插件：\n\n  ```\n  plugin_dirs = ["xxxxxx","xxxxxx",......,"下载完成的插件路径/nonebot-plugin-audiocraft"]\n  ```\n* 使用 pip\n  ```\n  pip install nonebot-plugin-audiocraft\n  ```\n# 后端服务器部署\n参考[官方仓库](https://github.com/facebookresearch/audiocraft#usage)部署好gradio后端，获得后端网址。（coblab上部署的可以开启gradio的外链分享）\n\n\n# 使用方法\n\n- 由于最近tx风控严重，go-cqhttp面临重启后可能掉账号的风险，所以插件使用给机器人发送消息配置后端服务器配置的方法。\n- 每次重启机器人后，使用 %%后端服务器地址 绑定audiocraft后端服务器。\n- 绑定后端服务器后，使用 AI作曲+乐曲的英文描述 即可触发AI作曲。\n- AI作曲的参数（如模型、时长）等通过代码进行修改，代码中有注释说明。\n\n# 效果\n\n![Alt](demo1.png)\n![Alt](demo2.png)\n',
+    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-audiocraft\n</div>\n\n# 介绍\n- 本插件适配[Facebook开源的AI作曲模型](https://github.com/facebookresearch/audiocraft/)，在nonebot框架下调用已经部署好的模型后端服务器API进行AI作曲\n- 本插件需要配合部署好的audiocraft进行使用\n\n# 安装\n\n* 手动安装\n  ```\n  git clone https://github.com/Alpaca4610/nonebot_plugin_audiocraft.git\n  ```\n\n  下载完成后在bot项目的pyproject.toml文件手动添加插件：\n\n  ```\n  plugin_dirs = ["xxxxxx","xxxxxx",......,"下载完成的插件路径/nonebot-plugin-audiocraft"]\n  ```\n* 使用 pip\n  ```\n  pip install nonebot-plugin-audiocraft\n  ```\n# 后端服务器部署\n参考[官方仓库](https://github.com/facebookresearch/audiocraft#usage)部署好gradio后端，获得后端网址。（colab上部署的可以开启gradio的外链分享）\n\n\n# 使用方法\n\n- 由于最近tx风控严重，go-cqhttp面临重启后可能掉账号的风险，所以插件使用给机器人发送消息配置后端服务器配置的方法。\n- 每次重启机器人后，使用 %%后端服务器地址 绑定audiocraft后端服务器。\n- 绑定后端服务器后，使用 AI作曲+乐曲的英文描述 即可触发AI作曲。\n- AI作曲的参数（如模型、时长）等通过代码进行修改，代码中有注释说明。\n\n# 效果\n\n![Alt](demo1.png)\n![Alt](demo2.png)\n',
     'author': 'Alpaca',
     'author_email': 'alpaca@bupt.edu.cn',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_audiocraft'] package_data = \ {'': ['*']} install_requires = \
-['gradio-client>=0.2.5,<0.3.0', 'nonebot-adapter-onebot>=2.2.1,<3.0.0',
-'nonebot2>=2.0.0rc3,<3.0.0'] setup_kwargs = { 'name': 'nonebot-plugin-
-audiocraft', 'version': '0.0.4', 'description': "A nonebot plugin for
-facebook's audiocraft", 'long_description': '
+['asyncio>=3.4.3,<4.0.0', 'gradio-client>=0.2.5,<0.3.0', 'nonebot-adapter-
+onebot>=2.2.1,<3.0.0', 'nonebot2>=2.0.0rc3,<3.0.0'] setup_kwargs = { 'name':
+'nonebot-plugin-audiocraft', 'version': '0.0.5', 'description': "A nonebot
+plugin for facebook's audiocraft", 'long_description': '
                            \n [NoneBotPluginLogo]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n
                        \n\n# nonebot-plugin-audiocraft\n
 \n\n# ä»ç»\n- æ¬æä»¶éé[Facebookå¼æºçAIä½æ²æ¨¡å](https://
@@ -17,15 +17,15 @@
 æå¨å®è£\n ```\n git clone https://github.com/Alpaca4610/
 nonebot_plugin_audiocraft.git\n ```\n\n
 ä¸è½½å®æåå¨boté¡¹ç®çpyproject.tomlæä»¶æå¨æ·»å æä»¶ï¼\n\n
 ```\n plugin_dirs = ["xxxxxx","xxxxxx",......,"ä¸è½½å®æçæä»¶è·¯å¾/
 nonebot-plugin-audiocraft"]\n ```\n* ä½¿ç¨ pip\n ```\n pip install nonebot-
 plugin-audiocraft\n ```\n# åç«¯æå¡å¨é¨ç½²\nåè[å®æ¹ä»åº](https://
 github.com/facebookresearch/
-audiocraft#usage)é¨ç½²å¥½gradioåç«¯ï¼è·å¾åç«¯ç½åãï¼coblabä¸é¨ç½²çå¯ä»¥å¼å¯gradioçå¤é¾åäº«ï¼\n\n\n#
+audiocraft#usage)é¨ç½²å¥½gradioåç«¯ï¼è·å¾åç«¯ç½åãï¼colabä¸é¨ç½²çå¯ä»¥å¼å¯gradioçå¤é¾åäº«ï¼\n\n\n#
 ä½¿ç¨æ¹æ³\n\n- ç±äºæè¿txé£æ§ä¸¥éï¼go-
 cqhttpé¢ä¸´éå¯åå¯è½æè´¦å·çé£é©ï¼æä»¥æä»¶ä½¿ç¨ç»æºå¨äººåéæ¶æ¯éç½®åç«¯æå¡å¨éç½®çæ¹æ³ã\n-
 æ¯æ¬¡éå¯æºå¨äººåï¼ä½¿ç¨ %%åç«¯æå¡å¨å°å
 ç»å®audiocraftåç«¯æå¡å¨ã\n- ç»å®åç«¯æå¡å¨åï¼ä½¿ç¨
 AIä½æ²+ä¹æ²çè±ææè¿° å³å¯è§¦åAIä½æ²ã\n-
 AIä½æ²çåæ°ï¼å¦æ¨¡åãæ¶é¿ï¼ç­éè¿ä»£ç è¿è¡ä¿®æ¹ï¼ä»£ç ä¸­ææ³¨éè¯´æã\n\n#
 ææ\n\n![Alt](demo1.png)\n![Alt](demo2.png)\n', 'author': 'Alpaca',
```

### Comparing `nonebot_plugin_audiocraft-0.0.4/PKG-INFO` & `nonebot_plugin_audiocraft-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-audiocraft
-Version: 0.0.4
+Version: 0.0.5
 Summary: A nonebot plugin for facebook's audiocraft
 License: MIT
 Author: Alpaca
 Author-email: alpaca@bupt.edu.cn
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: gradio-client (>=0.2.5,<0.3.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0)
 Requires-Dist: nonebot2 (>=2.0.0rc3,<3.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
@@ -45,15 +46,15 @@
   plugin_dirs = ["xxxxxx","xxxxxx",......,"下载完成的插件路径/nonebot-plugin-audiocraft"]
   ```
 * 使用 pip
   ```
   pip install nonebot-plugin-audiocraft
   ```
 # 后端服务器部署
-参考[官方仓库](https://github.com/facebookresearch/audiocraft#usage)部署好gradio后端，获得后端网址。（coblab上部署的可以开启gradio的外链分享）
+参考[官方仓库](https://github.com/facebookresearch/audiocraft#usage)部署好gradio后端，获得后端网址。（colab上部署的可以开启gradio的外链分享）
 
 
 # 使用方法
 
 - 由于最近tx风控严重，go-cqhttp面临重启后可能掉账号的风险，所以插件使用给机器人发送消息配置后端服务器配置的方法。
 - 每次重启机器人后，使用 %%后端服务器地址 绑定audiocraft后端服务器。
 - 绑定后端服务器后，使用 AI作曲+乐曲的英文描述 即可触发AI作曲。
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-audiocraft Version: 0.0.4 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-audiocraft Version: 0.0.5 Summary: A
 nonebot plugin for facebook's audiocraft License: MIT Author: Alpaca Author-
 email: alpaca@bupt.edu.cn Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: gradio-client
-(>=0.2.5,<0.3.0) Requires-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0)
-Requires-Dist: nonebot2 (>=2.0.0rc3,<3.0.0) Description-Content-Type: text/
-markdown
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: asyncio
+(>=3.4.3,<4.0.0) Requires-Dist: gradio-client (>=0.2.5,<0.3.0) Requires-Dist:
+nonebot-adapter-onebot (>=2.2.1,<3.0.0) Requires-Dist: nonebot2
+(>=2.0.0rc3,<3.0.0) Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                           # nonebot-plugin-audiocraft
 # ä»ç» - æ¬æä»¶éé[Facebookå¼æºçAIä½æ²æ¨¡å](https://github.com/
 facebookresearch/audiocraft/
 )ï¼å¨nonebotæ¡æ¶ä¸è°ç¨å·²ç»é¨ç½²å¥½çæ¨¡ååç«¯æå¡å¨APIè¿è¡AIä½æ²
 - æ¬æä»¶éè¦éåé¨ç½²å¥½çaudiocraftè¿è¡ä½¿ç¨ # å®è£ *
 æå¨å®è£ ``` git clone https://github.com/Alpaca4610/
 nonebot_plugin_audiocraft.git ```
 ä¸è½½å®æåå¨boté¡¹ç®çpyproject.tomlæä»¶æå¨æ·»å æä»¶ï¼ ```
 plugin_dirs = ["xxxxxx","xxxxxx",......,"ä¸è½½å®æçæä»¶è·¯å¾/nonebot-
 plugin-audiocraft"] ``` * ä½¿ç¨ pip ``` pip install nonebot-plugin-audiocraft
 ``` # åç«¯æå¡å¨é¨ç½² åè[å®æ¹ä»åº](https://github.com/
 facebookresearch/
-audiocraft#usage)é¨ç½²å¥½gradioåç«¯ï¼è·å¾åç«¯ç½åãï¼coblabä¸é¨ç½²çå¯ä»¥å¼å¯gradioçå¤é¾åäº«ï¼
+audiocraft#usage)é¨ç½²å¥½gradioåç«¯ï¼è·å¾åç«¯ç½åãï¼colabä¸é¨ç½²çå¯ä»¥å¼å¯gradioçå¤é¾åäº«ï¼
 # ä½¿ç¨æ¹æ³ - ç±äºæè¿txé£æ§ä¸¥éï¼go-
 cqhttpé¢ä¸´éå¯åå¯è½æè´¦å·çé£é©ï¼æä»¥æä»¶ä½¿ç¨ç»æºå¨äººåéæ¶æ¯éç½®åç«¯æå¡å¨éç½®çæ¹æ³ã
 - æ¯æ¬¡éå¯æºå¨äººåï¼ä½¿ç¨ %%åç«¯æå¡å¨å°å
 ç»å®audiocraftåç«¯æå¡å¨ã - ç»å®åç«¯æå¡å¨åï¼ä½¿ç¨
 AIä½æ²+ä¹æ²çè±ææè¿° å³å¯è§¦åAIä½æ²ã -
 AIä½æ²çåæ°ï¼å¦æ¨¡åãæ¶é¿ï¼ç­éè¿ä»£ç è¿è¡ä¿®æ¹ï¼ä»£ç ä¸­ææ³¨éè¯´æã
 # ææ ![Alt](demo1.png) ![Alt](demo2.png)
```

