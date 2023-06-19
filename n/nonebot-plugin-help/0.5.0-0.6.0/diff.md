# Comparing `tmp/nonebot_plugin_help-0.5.0.tar.gz` & `tmp/nonebot_plugin_help-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_help-0.5.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_help-0.6.0.tar", max compression
```

## Comparing `nonebot_plugin_help-0.5.0.tar` & `nonebot_plugin_help-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35184 2022-06-21 14:58:39.859249 nonebot_plugin_help-0.5.0/LICENSE
--rw-r--r--   0        0        0     1314 2023-06-06 14:57:51.950180 nonebot_plugin_help-0.5.0/nonebot_plugin_help/__init__.py
--rw-r--r--   0        0        0      220 2023-04-21 15:54:22.509482 nonebot_plugin_help-0.5.0/nonebot_plugin_help/config.py
--rw-r--r--   0        0        0     5147 2023-04-21 16:17:29.869180 nonebot_plugin_help-0.5.0/nonebot_plugin_help/handler.py
--rw-r--r--   0        0        0      570 2023-06-06 14:48:35.601209 nonebot_plugin_help-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     6433 2023-04-21 16:16:07.364334 nonebot_plugin_help-0.5.0/README.md
--rw-r--r--   0        0        0     7013 1970-01-01 00:00:00.000000 nonebot_plugin_help-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-06-21 14:58:39.859249 nonebot_plugin_help-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1454 2023-06-19 16:13:33.311125 nonebot_plugin_help-0.6.0/nonebot_plugin_help/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-19 16:10:37.194826 nonebot_plugin_help-0.6.0/nonebot_plugin_help/config.py
+-rw-r--r--   0        0        0     5344 2023-06-19 16:24:25.065109 nonebot_plugin_help-0.6.0/nonebot_plugin_help/handler.py
+-rw-r--r--   0        0        0      570 2023-06-19 16:34:11.421392 nonebot_plugin_help-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7877 2023-06-19 16:25:13.788420 nonebot_plugin_help-0.6.0/README.md
+-rw-r--r--   0        0        0     8414 1970-01-01 00:00:00.000000 nonebot_plugin_help-0.6.0/PKG-INFO
```

### Comparing `nonebot_plugin_help-0.5.0/LICENSE` & `nonebot_plugin_help-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_help-0.5.0/nonebot_plugin_help/__init__.py` & `nonebot_plugin_help-0.6.0/nonebot_plugin_help/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 Nonebot 2 Help Plugin
 Author: XZhouQD
 Since: 16 May 2021
 """
 import nonebot
+
+from .config import Config
 from .handler import helper
 
 
 default_start = list(nonebot.get_driver().config.command_start)[0]
 
 # Legacy way of self registering (use custom attributes)
 # Deprecated for nonebot-plugin-help 0.3.1+, prefer PluginMetadata.extra['version']
-__help_version__ = '0.5.0'
+__help_version__ = '0.6.0'
 # Deprecated for nonebot-plugin-help 0.3.0+, prefer PluginMetadata.name
 __help_plugin_name__ = "Nonebot2 Help Menu"
 # Deprecated for nonebot-plugin-help 0.3.0+, prefer PluginMetadata.usage
 __usage__ = f'''欢迎使用Nonebot2 Help Menu
 本插件提供公共帮助菜单能力
 此Bot配置的命令前缀：{" ".join(list(nonebot.get_driver().config.command_start))}
 '''
@@ -28,9 +30,12 @@
 本插件提供公共帮助菜单能力
 此Bot配置的命令前缀：{" ".join(list(nonebot.get_driver().config.command_start))}
 
 {default_start}help  # 获取本插件帮助
 {default_start}help list  # 展示已加载插件列表
 {default_start}help <插件名>  # 调取目标插件帮助信息
 ''',
-    extra={'version': '0.5.0'}
+    type='application',
+    homepage='https://github.com/xzhouqd/nonebot-plugin-help',
+    extra={'version': '0.6.0'},
+    config=Config,
 )
```

### Comparing `nonebot_plugin_help-0.5.0/nonebot_plugin_help/handler.py` & `nonebot_plugin_help-0.6.0/nonebot_plugin_help/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import nonebot.plugin
 from nonebot import on_command
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg, Arg
 from nonebot.adapters import Event
 from nonebot.adapters import Message
+from nonebot.rule import to_me
 
 from .config import Config
 
 command_starts = list(nonebot.get_driver().config.command_start)
 default_start = command_starts[0]
 plugin_config = Config.parse_obj(nonebot.get_driver().config)
 
-helper = on_command("help", priority=plugin_config.help_priority, aliases={"帮助"}, block=plugin_config.help_block)
+helper = on_command("help", priority=plugin_config.help_priority, aliases={"帮助"}, block=plugin_config.help_block,
+                    rule=to_me() if plugin_config.help_to_me else None)
 # Matcher level info registering, still active in-use
 helper.__help_name__ = 'help'
 helper.__help_info__ = f'''{default_start}help  # 获取本插件帮助
 {default_start}help list  # 展示已加载插件列表
 {default_start}help <plugin_name>  # 调取目标插件帮助信息'''
 
 
@@ -35,14 +37,16 @@
 @helper.got("content")
 async def get_result(event: Event, content: Message = Arg()):
     arg = content.extract_plain_text().strip()
     if arg.lower() == "list":
         plugin_set = nonebot.plugin.get_loaded_plugins()
         plugin_names = []
         for plugin in plugin_set:
+            if plugin.name in plugin_config.help_ignore_plugins:
+                continue
             # plugin.name, then metadata name or legacy help name
             name = f'{plugin.name} | '
             try:
                 name += plugin.metadata.name if plugin.metadata and plugin.metadata.name \
                     else plugin.module.__getattribute__("__help_plugin_name__")
             except:
                 name = plugin.name
```

### Comparing `nonebot_plugin_help-0.5.0/pyproject.toml` & `nonebot_plugin_help-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-help"
-version = "0.5.0"
+version = "0.6.0"
 description = "A general help lister for nonebot2 plugins"
 authors = ["XZhouQD <X.Zhou.QD@hotmail.com>"]
 license = "AGPL v3"
 readme = "README.md"
 homepage = "https://github.com/XZhouQD/nonebot-plugin-help"
 repository = "https://github.com/XZhouQD/nonebot-plugin-help"
 include = [
```

### Comparing `nonebot_plugin_help-0.5.0/README.md` & `nonebot_plugin_help-0.6.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 <div align="center">
 
 # nonebot-plugin-help
+
 ### Nonebot2 轻量级帮助插件
 
 <a href="https://raw.githubusercontent.com/xzhouqd/nonebot-plugin-help/main/LICENSE">
     <img src="https://img.shields.io/github/license/xzhouqd/nonebot-plugin-help?style=for-the-badge" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-help">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-help?color=green&style=for-the-badge" alt="pypi">
@@ -15,88 +16,127 @@
 <img src="https://img.shields.io/badge/require_python-3.8+-blue?style=for-the-badge" alt="python">
 <br />
 <img src="https://img.shields.io/badge/tested_python-3.10.6-blue?style=for-the-badge" alt="python">
 <img src="https://img.shields.io/badge/tested_env-go_cqhttp_1.0.0-blue?style=for-the-badge" alt="python">
 <img src="https://img.shields.io/badge/tested_Nonebot-2.0.0_rc4-red?style=for-the-badge" alt="nonebot">
 </div>
 
-## 配置help插件优先级与阻塞（可选） ![nonebot-plugin-help](https://img.shields.io/static/v1?label=nonebot-plugin-help&message=0.4.0&color=red)
-0.4.0版本起，新增插件优先级与阻塞设置（可选），默认为`priority=1, block=False`
+## Bot可对本插件进行的配置
+
+### 配置 help 插件优先级与阻塞（可选） ![nonebot-plugin-help](https://img.shields.io/static/v1?label=nonebot-plugin-help&message=0.4.0&color=red)
+
+0.4.0 版本起，新增插件优先级与阻塞设置（可选），默认为`priority=1, block=False`
+
+用户可在.env 配置文件内通过配置项`help_block`与`help_priority`进行配置，例如，以下配置可将 help 命令配置为`priority=100, block=True`
 
-用户可在.env配置文件内通过配置项`help_block`与`help_priority`进行配置，例如，以下配置可将help命令配置为`priority=100, block=True`
 ```
 help_block = true
 help_priority = 100
 ```
 
+### 配置 help 插件忽略列表与`to_me`规则（可选） ![nonebot-plugin-help](https://img.shields.io/static/v1?label=nonebot-plugin-help&message=0.6.0&color=red)
+
+0.6.0 版本起，新增忽略插件与`to_me`规则（可选），`help_ignore_plugins`默认不忽略任何插件，`to_me`默认值为`False`。  
+
+`help_ignore_plugins`：可配置不希望 help 插件列出的插件包名列表，例如，以下配置可忽略`nonebot_plugin_localstore`与`nonebot_plugin_apscheduler`插件。  
+`help_to_me`：可配置是否只有私聊或提及Bot时才响应 help 命令。
+
+```
+help_ignore_plugins=["nonebot_plugin_localstore", "nonebot_plugin_apscheduler"]
+help_to_me=true
+```
+
 ## 开发者接入此插件列表方法
+
 您可以直接参考本插件的接入方式，阅读源代码即可！
-### 插件级别元数据接入 ![nonebot2](https://img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.4&color=red)
-使用自 **Nonebot 2.0.0-beta.4** 版本起新增的插件元数据进行插件级统一接入（不包含Matcher级别接入）
+
+### 插件级别元数据接入 ![nonebot2](https://img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.4&color=red) ![In Use](https://img.shields.io/static/v1?label=Status&message=In%2DUse%26Preferred&color=green)
+
+使用自 **Nonebot 2.0.0-beta.4** 版本起新增的插件元数据进行插件级统一接入（不包含 Matcher 级别接入）
+
 ```python
 # New way of self registering (use PluginMetadata)
 __plugin_meta__ = nonebot.plugin.PluginMetadata(
     name='您的插件名称（有别于nonebot-plugin-xxx的包名）',
     description='您的简单插件描述',
     usage='''您想在使用命令/help <your plugin package name>时提供的帮助文本''',
-    extra={'version': '0.3.1'}
+    type='{插件分类}', # From 2.0.0 Stable Version, 发布必填，当前有效类型有：`library`（为其他插件编写提供功能），`application`（向机器人用户提供功能）。
+    homepage='{项目主页}', # From 2.0.0 Stable Version
+    config=Config, # From 2.0.0 Stable Version, 插件配置项类，如无需配置可不填写。
+    extra={'version': '0.6.0'}
 )
 ```
-### 插件级别传统接入 ![nonebot2](https://img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red)
-使用python包形态的插件（已发布/自行开发皆可），并在插件包的__init__.py文件内增加如下代码：
+
+### 插件级别传统接入 ![nonebot2](https://img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red) ![Deprecated](https://img.shields.io/static/v1?label=Status&message=deprecated)
+
+使用 python 包形态的插件（已发布/自行开发皆可），并在插件包的**init**.py 文件内增加如下代码：
+
 ```python
 # 您的插件版本号，将在/help list中显示
 # Deprecated for nonebot-plugin-help 0.3.1+, prefer PluginMetadata.extra['version']
-__help_version__ = '0.4.1'
+__help_version__ = '0.6.0'
 # 此名称有助于美化您的插件在/help list中的显示
 # 但使用/help xxx查询插件用途时仍必须使用包名
 # Deprecated for nonebot-plugin-help 0.3.0+, prefer PluginMetadata.name
 __help_plugin_name__ = "您的插件名称（有别于nonebot-plugin-xxx的包名）"
 # Deprecated for nonebot-plugin-help 0.3.0+, prefer PluginMetadata.usage
 # 若此文本不存在，将显示包的__doc__
 __usage__ = '您想在使用命令/help <your plugin package name>时提供的帮助文本'
 ```
-### Matcher级别接入 ![nonebot2](https://img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red)
-Matcher级别帮助请为Matcher添加如下代码：
+
+### Matcher 级别接入 ![nonebot2](https://img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red) ![In Use](https://img.shields.io/static/v1?label=Status&message=In%2DUse&color=green)
+
+Matcher 级别帮助请为 Matcher 添加如下代码：
+
 ```python
 default_start = list(nonebot.get_driver().config.command_start)[0]
 helper = on_command("help", priority=1, aliases={"帮助"})
 helper.__help_name__ = '您的命令触发指令名'
 helper.__help_info__ = '您为此命令提供的帮助文本'
 helper.__doc__ = '您为此命令提供的帮助文本, 当您不希望使用__help_info__提供时，可以使用__doc__提供'
 ```
-请注意：当您未提供`__help_name__`或`__help_info__`与`__doc__`中的一个时，此Matcher不会列入Matcher级别帮助！
+
+请注意：当您未提供`__help_name__`或`__help_info__`与`__doc__`中的一个时，此 Matcher 不会列入 Matcher 级别帮助！
 
 ## 实际使用
-此部分介绍以使用'/'作为command_start为例。
+
+此部分介绍以使用'/'作为 command_start 为例。
+
 ### 获取本插件帮助
+
 指令： /help
 
 返回示例：
+
 ```
 @<user_who_send_command> 欢迎使用Nonebot2 Help Menu
 支持使用的前缀：/
 /help  # 获取本插件帮助
 /help list  # 展示已加载插件列表
 /help <plugin_name>  # 调取目标插件帮助信息
 ```
+
 ### 查看已加载插件列表
+
 指令：/help list
 
 返回示例：
+
 ```
 @<user_who_send_command> 已加载插件：
 nonebot_plugin_cloverdata | 四叶草魔物娘属性计算插件 | 0.1.0
-nonebot_plugin_guild_patch 
+nonebot_plugin_guild_patch
 nonebot_plugin_help | Nonebot2 Help Menu | 0.4.1
 ```
 
 ### 查看已加载某一插件用途
+
 指令：/help <plugin_package_name | plugin_help_name>
 示例：
+
 ```
 /help nonebot_plugin_help
 
 @<user_who_send_command> Nonebot2 Help Menu: Nonebot2轻量级帮助插件
 欢迎使用Nonebot2 Help Menu                       // 这里是插件元数据提供的帮助
 本插件提供公共帮助菜单能力
 此Bot配置的命令前缀：/
@@ -107,15 +147,17 @@
 
 
 序号. 命令名: 命令用途                             // 这里是Matcher级别接入提供的帮助
 1. help: /help  # 获取本插件帮助
 /help list  # 展示已加载插件列表
 /help <plugin_name>  # 调取目标插件帮助信息
 ```
+
 或使用提供的插件美化名示例：
+
 ```
 /help Nonebot2 Help Menu
 
 @<user_who_send_command> Nonebot2 Help Menu: Nonebot2轻量级帮助插件
 欢迎使用Nonebot2 Help Menu                       // 这里是插件元数据提供的帮助
 本插件提供公共帮助菜单能力
 此Bot配置的命令前缀：/
@@ -127,15 +169,16 @@
 
 序号. 命令名: 命令用途                             // 这里是Matcher级别接入提供的帮助
 1. help: /help  # 获取本插件帮助
 /help list  # 展示已加载插件列表
 /help <plugin_name>  # 调取目标插件帮助信息
 ```
 
-若插件未提供__usage__，则会显示__doc__，示例：
+若插件未提供**usage**，则会显示**doc**，示例：
+
 ```
 /help nonebot_plugin_help
 
 @<user_who_send_command>
 Nonebot 2 Help Menu
 Author: XZhouQD
 Since: 16 May 2021
```

#### html2text {}

```diff
@@ -1,50 +1,73 @@
 # nonebot-plugin-help ### Nonebot2 è½»éçº§å¸®å©æä»¶ [license] [pypi] [pypi
                               download] [python]
                           [python] [python] [nonebot]
-## éç½®helpæä»¶ä¼åçº§ä¸é»å¡ï¼å¯éï¼ ![nonebot-plugin-help](https:
-//img.shields.io/static/v1?label=nonebot-plugin-help&message=0.4.0&color=red)
-0.4.0çæ¬èµ·ï¼æ°å¢æä»¶ä¼åçº§ä¸é»å¡è®¾ç½®ï¼å¯éï¼ï¼é»è®¤ä¸º`priority=1,
-block=False`
-ç¨æ·å¯å¨.envéç½®æä»¶åéè¿éç½®é¡¹`help_block`ä¸`help_priority`è¿è¡éç½®ï¼ä¾å¦ï¼ä»¥ä¸éç½®å¯å°helpå½ä»¤éç½®ä¸º`priority=100,
-block=True` ``` help_block = true help_priority = 100 ``` ##
+## Botå¯å¯¹æ¬æä»¶è¿è¡çéç½® ### éç½® help
+æä»¶ä¼åçº§ä¸é»å¡ï¼å¯éï¼ ![nonebot-plugin-help](https://
+img.shields.io/static/v1?label=nonebot-plugin-help&message=0.4.0&color=red)
+0.4.0
+çæ¬èµ·ï¼æ°å¢æä»¶ä¼åçº§ä¸é»å¡è®¾ç½®ï¼å¯éï¼ï¼é»è®¤ä¸º`priority=1,
+block=False` ç¨æ·å¯å¨.env
+éç½®æä»¶åéè¿éç½®é¡¹`help_block`ä¸`help_priority`è¿è¡éç½®ï¼ä¾å¦ï¼ä»¥ä¸éç½®å¯å°
+help å½ä»¤éç½®ä¸º`priority=100, block=True` ``` help_block = true
+help_priority = 100 ``` ### éç½® help
+æä»¶å¿½ç¥åè¡¨ä¸`to_me`è§åï¼å¯éï¼ ![nonebot-plugin-help](https://
+img.shields.io/static/v1?label=nonebot-plugin-help&message=0.6.0&color=red)
+0.6.0
+çæ¬èµ·ï¼æ°å¢å¿½ç¥æä»¶ä¸`to_me`è§åï¼å¯éï¼ï¼`help_ignore_plugins`é»è®¤ä¸å¿½ç¥ä»»ä½æä»¶ï¼`to_me`é»è®¤å¼ä¸º`False`ã
+`help_ignore_plugins`ï¼å¯éç½®ä¸å¸æ help
+æä»¶ååºçæä»¶åååè¡¨ï¼ä¾å¦ï¼ä»¥ä¸éç½®å¯å¿½ç¥`nonebot_plugin_localstore`ä¸`nonebot_plugin_apscheduler`æä»¶ã
+`help_to_me`ï¼å¯éç½®æ¯å¦åªæç§èææåBotæ¶æååº help
+å½ä»¤ã ``` help_ignore_plugins=["nonebot_plugin_localstore",
+"nonebot_plugin_apscheduler"] help_to_me=true ``` ##
 å¼åèæ¥å¥æ­¤æä»¶åè¡¨æ¹æ³
 æ¨å¯ä»¥ç´æ¥åèæ¬æä»¶çæ¥å¥æ¹å¼ï¼éè¯»æºä»£ç å³å¯ï¼ ###
 æä»¶çº§å«åæ°æ®æ¥å¥ ![nonebot2](https://img.shields.io/static/
-v1?label=Nonebot&message=2.0.0%2Dbeta.4&color=red) ä½¿ç¨èª **Nonebot 2.0.0-
-beta.4**
-çæ¬èµ·æ°å¢çæä»¶åæ°æ®è¿è¡æä»¶çº§ç»ä¸æ¥å¥ï¼ä¸åå«Matcherçº§å«æ¥å¥ï¼
-```python # New way of self registering (use PluginMetadata) __plugin_meta__ =
-nonebot.plugin.PluginMetadata( name='æ¨çæä»¶åç§°ï¼æå«äºnonebot-
-plugin-xxxçååï¼', description='æ¨çç®åæä»¶æè¿°',
-usage='''æ¨æ³å¨ä½¿ç¨å½ä»¤/help æ¶æä¾çå¸®å©ææ¬''', extra=
-{'version': '0.3.1'} ) ``` ### æä»¶çº§å«ä¼ ç»æ¥å¥ ![nonebot2](https://
-img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red)
-ä½¿ç¨pythonåå½¢æçæä»¶ï¼å·²åå¸/
-èªè¡å¼åçå¯ï¼ï¼å¹¶å¨æä»¶åç__init__.pyæä»¶åå¢å å¦ä¸ä»£ç ï¼
-```python # æ¨çæä»¶çæ¬å·ï¼å°å¨/help listä¸­æ¾ç¤º # Deprecated for
-nonebot-plugin-help 0.3.1+, prefer PluginMetadata.extra['version']
-__help_version__ = '0.4.1' # æ­¤åç§°æå©äºç¾åæ¨çæä»¶å¨/help
-listä¸­çæ¾ç¤º # ä½ä½¿ç¨/help xxxæ¥è¯¢æä»¶ç¨éæ¶ä»å¿é¡»ä½¿ç¨åå
-# Deprecated for nonebot-plugin-help 0.3.0+, prefer PluginMetadata.name
-__help_plugin_name__ = "æ¨çæä»¶åç§°ï¼æå«äºnonebot-plugin-
-xxxçååï¼" # Deprecated for nonebot-plugin-help 0.3.0+, prefer
-PluginMetadata.usage # è¥æ­¤ææ¬ä¸å­å¨ï¼å°æ¾ç¤ºåç__doc__ __usage__
-= 'æ¨æ³å¨ä½¿ç¨å½ä»¤/help æ¶æä¾çå¸®å©ææ¬' ``` ###
-Matcherçº§å«æ¥å¥ ![nonebot2](https://img.shields.io/static/
-v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red)
-Matcherçº§å«å¸®å©è¯·ä¸ºMatcheræ·»å å¦ä¸ä»£ç ï¼ ```python default_start =
-list(nonebot.get_driver().config.command_start)[0] helper = on_command("help",
+v1?label=Nonebot&message=2.0.0%2Dbeta.4&color=red) ![In Use](https://
+img.shields.io/static/v1?label=Status&message=In%2DUse%26Preferred&color=green)
+ä½¿ç¨èª **Nonebot 2.0.0-beta.4**
+çæ¬èµ·æ°å¢çæä»¶åæ°æ®è¿è¡æä»¶çº§ç»ä¸æ¥å¥ï¼ä¸åå«
+Matcher çº§å«æ¥å¥ï¼ ```python # New way of self registering (use
+PluginMetadata) __plugin_meta__ = nonebot.plugin.PluginMetadata
+( name='æ¨çæä»¶åç§°ï¼æå«äºnonebot-plugin-xxxçååï¼',
+description='æ¨çç®åæä»¶æè¿°', usage='''æ¨æ³å¨ä½¿ç¨å½ä»¤/help
+æ¶æä¾çå¸®å©ææ¬''', type='{æä»¶åç±»}', # From 2.0.0 Stable
+Version,
+åå¸å¿å¡«ï¼å½åææç±»åæï¼`library`ï¼ä¸ºå¶ä»æä»¶ç¼åæä¾åè½ï¼ï¼`application`ï¼åæºå¨äººç¨æ·æä¾åè½ï¼ã
+homepage='{é¡¹ç®ä¸»é¡µ}', # From 2.0.0 Stable Version config=Config, # From
+2.0.0 Stable Version, æä»¶éç½®é¡¹ç±»ï¼å¦æ ééç½®å¯ä¸å¡«åã
+extra={'version': '0.6.0'} ) ``` ### æä»¶çº§å«ä¼ ç»æ¥å¥ ![nonebot2]
+(https://img.shields.io/static/
+v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red) ![Deprecated](https://
+img.shields.io/static/v1?label=Status&message=deprecated) ä½¿ç¨ python
+åå½¢æçæä»¶ï¼å·²åå¸/
+èªè¡å¼åçå¯ï¼ï¼å¹¶å¨æä»¶åç**init**.py
+æä»¶åå¢å å¦ä¸ä»£ç ï¼ ```python # æ¨çæä»¶çæ¬å·ï¼å°å¨/help
+listä¸­æ¾ç¤º # Deprecated for nonebot-plugin-help 0.3.1+, prefer
+PluginMetadata.extra['version'] __help_version__ = '0.6.0' #
+æ­¤åç§°æå©äºç¾åæ¨çæä»¶å¨/help listä¸­çæ¾ç¤º # ä½ä½¿ç¨/help
+xxxæ¥è¯¢æä»¶ç¨éæ¶ä»å¿é¡»ä½¿ç¨åå # Deprecated for nonebot-plugin-
+help 0.3.0+, prefer PluginMetadata.name __help_plugin_name__ =
+"æ¨çæä»¶åç§°ï¼æå«äºnonebot-plugin-xxxçååï¼" # Deprecated for
+nonebot-plugin-help 0.3.0+, prefer PluginMetadata.usage #
+è¥æ­¤ææ¬ä¸å­å¨ï¼å°æ¾ç¤ºåç__doc__ __usage__ =
+'æ¨æ³å¨ä½¿ç¨å½ä»¤/help æ¶æä¾çå¸®å©ææ¬' ``` ### Matcher
+çº§å«æ¥å¥ ![nonebot2](https://img.shields.io/static/
+v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red) ![In Use](https://
+img.shields.io/static/v1?label=Status&message=In%2DUse&color=green) Matcher
+çº§å«å¸®å©è¯·ä¸º Matcher æ·»å å¦ä¸ä»£ç ï¼ ```python default_start = list
+(nonebot.get_driver().config.command_start)[0] helper = on_command("help",
 priority=1, aliases={"å¸®å©"}) helper.__help_name__ =
 'æ¨çå½ä»¤è§¦åæä»¤å' helper.__help_info__ =
 'æ¨ä¸ºæ­¤å½ä»¤æä¾çå¸®å©ææ¬' helper.__doc__ =
 'æ¨ä¸ºæ­¤å½ä»¤æä¾çå¸®å©ææ¬,
 å½æ¨ä¸å¸æä½¿ç¨__help_info__æä¾æ¶ï¼å¯ä»¥ä½¿ç¨__doc__æä¾' ```
-è¯·æ³¨æï¼å½æ¨æªæä¾`__help_name__`æ`__help_info__`ä¸`__doc__`ä¸­çä¸ä¸ªæ¶ï¼æ­¤Matcherä¸ä¼åå¥Matcherçº§å«å¸®å©ï¼
-## å®éä½¿ç¨ æ­¤é¨åä»ç»ä»¥ä½¿ç¨'/'ä½ä¸ºcommand_startä¸ºä¾ã ###
+è¯·æ³¨æï¼å½æ¨æªæä¾`__help_name__`æ`__help_info__`ä¸`__doc__`ä¸­çä¸ä¸ªæ¶ï¼æ­¤
+Matcher ä¸ä¼åå¥ Matcher çº§å«å¸®å©ï¼ ## å®éä½¿ç¨
+æ­¤é¨åä»ç»ä»¥ä½¿ç¨'/'ä½ä¸º command_start ä¸ºä¾ã ###
 è·åæ¬æä»¶å¸®å© æä»¤ï¼ /help è¿åç¤ºä¾ï¼ ``` @
 æ¬¢è¿ä½¿ç¨Nonebot2 Help Menu æ¯æä½¿ç¨çåç¼ï¼/ /help #
 è·åæ¬æä»¶å¸®å© /help list # å±ç¤ºå·²å è½½æä»¶åè¡¨ /help  #
 è°åç®æ æä»¶å¸®å©ä¿¡æ¯ ``` ### æ¥çå·²å è½½æä»¶åè¡¨ æä»¤ï¼/
 help list è¿åç¤ºä¾ï¼ ``` @ å·²å è½½æä»¶ï¼ nonebot_plugin_cloverdata |
 åå¶èé­ç©å¨å±æ§è®¡ç®æä»¶ | 0.1.0 nonebot_plugin_guild_patch
 nonebot_plugin_help | Nonebot2 Help Menu | 0.4.1 ``` ###
@@ -63,11 +86,11 @@
 / è¿éæ¯æä»¶åæ°æ®æä¾çå¸®å©
 æ¬æä»¶æä¾å¬å±å¸®å©èåè½å æ­¤Botéç½®çå½ä»¤åç¼ï¼/ /help #
 è·åæ¬æä»¶å¸®å© /help list # å±ç¤ºå·²å è½½æä»¶åè¡¨ /help
 <æä»¶å> # è°åç®æ æä»¶å¸®å©ä¿¡æ¯ åºå·. å½ä»¤å: å½ä»¤ç¨é /
 / è¿éæ¯Matcherçº§å«æ¥å¥æä¾çå¸®å© 1. help: /help #
 è·åæ¬æä»¶å¸®å© /help list # å±ç¤ºå·²å è½½æä»¶åè¡¨ /help  #
 è°åç®æ æä»¶å¸®å©ä¿¡æ¯ ```
-è¥æä»¶æªæä¾__usage__ï¼åä¼æ¾ç¤º__doc__ï¼ç¤ºä¾ï¼ ``` /help
+è¥æä»¶æªæä¾**usage**ï¼åä¼æ¾ç¤º**doc**ï¼ç¤ºä¾ï¼ ``` /help
 nonebot_plugin_help @ Nonebot 2 Help Menu Author: XZhouQD Since: 16 May 2021
 åºå·. å½ä»¤å: å½ä»¤ç¨é 1. help: /help # è·åæ¬æä»¶å¸®å© /help
 list # å±ç¤ºå·²å è½½æä»¶åè¡¨ /help  # è°åç®æ æä»¶å¸®å©ä¿¡æ¯ ```
```

### Comparing `nonebot_plugin_help-0.5.0/PKG-INFO` & `nonebot_plugin_help-0.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-help
-Version: 0.5.0
+Version: 0.6.0
 Summary: A general help lister for nonebot2 plugins
 Home-page: https://github.com/XZhouQD/nonebot-plugin-help
 License: AGPL v3
 Author: XZhouQD
 Author-email: X.Zhou.QD@hotmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: Other/Proprietary License
@@ -16,14 +16,15 @@
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/XZhouQD/nonebot-plugin-help
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # nonebot-plugin-help
+
 ### Nonebot2 轻量级帮助插件
 
 <a href="https://raw.githubusercontent.com/xzhouqd/nonebot-plugin-help/main/LICENSE">
     <img src="https://img.shields.io/github/license/xzhouqd/nonebot-plugin-help?style=for-the-badge" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-help">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-help?color=green&style=for-the-badge" alt="pypi">
@@ -34,88 +35,127 @@
 <img src="https://img.shields.io/badge/require_python-3.8+-blue?style=for-the-badge" alt="python">
 <br />
 <img src="https://img.shields.io/badge/tested_python-3.10.6-blue?style=for-the-badge" alt="python">
 <img src="https://img.shields.io/badge/tested_env-go_cqhttp_1.0.0-blue?style=for-the-badge" alt="python">
 <img src="https://img.shields.io/badge/tested_Nonebot-2.0.0_rc4-red?style=for-the-badge" alt="nonebot">
 </div>
 
-## 配置help插件优先级与阻塞（可选） ![nonebot-plugin-help](https://img.shields.io/static/v1?label=nonebot-plugin-help&message=0.4.0&color=red)
-0.4.0版本起，新增插件优先级与阻塞设置（可选），默认为`priority=1, block=False`
+## Bot可对本插件进行的配置
+
+### 配置 help 插件优先级与阻塞（可选） ![nonebot-plugin-help](https://img.shields.io/static/v1?label=nonebot-plugin-help&message=0.4.0&color=red)
+
+0.4.0 版本起，新增插件优先级与阻塞设置（可选），默认为`priority=1, block=False`
+
+用户可在.env 配置文件内通过配置项`help_block`与`help_priority`进行配置，例如，以下配置可将 help 命令配置为`priority=100, block=True`
 
-用户可在.env配置文件内通过配置项`help_block`与`help_priority`进行配置，例如，以下配置可将help命令配置为`priority=100, block=True`
 ```
 help_block = true
 help_priority = 100
 ```
 
+### 配置 help 插件忽略列表与`to_me`规则（可选） ![nonebot-plugin-help](https://img.shields.io/static/v1?label=nonebot-plugin-help&message=0.6.0&color=red)
+
+0.6.0 版本起，新增忽略插件与`to_me`规则（可选），`help_ignore_plugins`默认不忽略任何插件，`to_me`默认值为`False`。  
+
+`help_ignore_plugins`：可配置不希望 help 插件列出的插件包名列表，例如，以下配置可忽略`nonebot_plugin_localstore`与`nonebot_plugin_apscheduler`插件。  
+`help_to_me`：可配置是否只有私聊或提及Bot时才响应 help 命令。
+
+```
+help_ignore_plugins=["nonebot_plugin_localstore", "nonebot_plugin_apscheduler"]
+help_to_me=true
+```
+
 ## 开发者接入此插件列表方法
+
 您可以直接参考本插件的接入方式，阅读源代码即可！
-### 插件级别元数据接入 ![nonebot2](https://img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.4&color=red)
-使用自 **Nonebot 2.0.0-beta.4** 版本起新增的插件元数据进行插件级统一接入（不包含Matcher级别接入）
+
+### 插件级别元数据接入 ![nonebot2](https://img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.4&color=red) ![In Use](https://img.shields.io/static/v1?label=Status&message=In%2DUse%26Preferred&color=green)
+
+使用自 **Nonebot 2.0.0-beta.4** 版本起新增的插件元数据进行插件级统一接入（不包含 Matcher 级别接入）
+
 ```python
 # New way of self registering (use PluginMetadata)
 __plugin_meta__ = nonebot.plugin.PluginMetadata(
     name='您的插件名称（有别于nonebot-plugin-xxx的包名）',
     description='您的简单插件描述',
     usage='''您想在使用命令/help <your plugin package name>时提供的帮助文本''',
-    extra={'version': '0.3.1'}
+    type='{插件分类}', # From 2.0.0 Stable Version, 发布必填，当前有效类型有：`library`（为其他插件编写提供功能），`application`（向机器人用户提供功能）。
+    homepage='{项目主页}', # From 2.0.0 Stable Version
+    config=Config, # From 2.0.0 Stable Version, 插件配置项类，如无需配置可不填写。
+    extra={'version': '0.6.0'}
 )
 ```
-### 插件级别传统接入 ![nonebot2](https://img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red)
-使用python包形态的插件（已发布/自行开发皆可），并在插件包的__init__.py文件内增加如下代码：
+
+### 插件级别传统接入 ![nonebot2](https://img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red) ![Deprecated](https://img.shields.io/static/v1?label=Status&message=deprecated)
+
+使用 python 包形态的插件（已发布/自行开发皆可），并在插件包的**init**.py 文件内增加如下代码：
+
 ```python
 # 您的插件版本号，将在/help list中显示
 # Deprecated for nonebot-plugin-help 0.3.1+, prefer PluginMetadata.extra['version']
-__help_version__ = '0.4.1'
+__help_version__ = '0.6.0'
 # 此名称有助于美化您的插件在/help list中的显示
 # 但使用/help xxx查询插件用途时仍必须使用包名
 # Deprecated for nonebot-plugin-help 0.3.0+, prefer PluginMetadata.name
 __help_plugin_name__ = "您的插件名称（有别于nonebot-plugin-xxx的包名）"
 # Deprecated for nonebot-plugin-help 0.3.0+, prefer PluginMetadata.usage
 # 若此文本不存在，将显示包的__doc__
 __usage__ = '您想在使用命令/help <your plugin package name>时提供的帮助文本'
 ```
-### Matcher级别接入 ![nonebot2](https://img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red)
-Matcher级别帮助请为Matcher添加如下代码：
+
+### Matcher 级别接入 ![nonebot2](https://img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red) ![In Use](https://img.shields.io/static/v1?label=Status&message=In%2DUse&color=green)
+
+Matcher 级别帮助请为 Matcher 添加如下代码：
+
 ```python
 default_start = list(nonebot.get_driver().config.command_start)[0]
 helper = on_command("help", priority=1, aliases={"帮助"})
 helper.__help_name__ = '您的命令触发指令名'
 helper.__help_info__ = '您为此命令提供的帮助文本'
 helper.__doc__ = '您为此命令提供的帮助文本, 当您不希望使用__help_info__提供时，可以使用__doc__提供'
 ```
-请注意：当您未提供`__help_name__`或`__help_info__`与`__doc__`中的一个时，此Matcher不会列入Matcher级别帮助！
+
+请注意：当您未提供`__help_name__`或`__help_info__`与`__doc__`中的一个时，此 Matcher 不会列入 Matcher 级别帮助！
 
 ## 实际使用
-此部分介绍以使用'/'作为command_start为例。
+
+此部分介绍以使用'/'作为 command_start 为例。
+
 ### 获取本插件帮助
+
 指令： /help
 
 返回示例：
+
 ```
 @<user_who_send_command> 欢迎使用Nonebot2 Help Menu
 支持使用的前缀：/
 /help  # 获取本插件帮助
 /help list  # 展示已加载插件列表
 /help <plugin_name>  # 调取目标插件帮助信息
 ```
+
 ### 查看已加载插件列表
+
 指令：/help list
 
 返回示例：
+
 ```
 @<user_who_send_command> 已加载插件：
 nonebot_plugin_cloverdata | 四叶草魔物娘属性计算插件 | 0.1.0
-nonebot_plugin_guild_patch 
+nonebot_plugin_guild_patch
 nonebot_plugin_help | Nonebot2 Help Menu | 0.4.1
 ```
 
 ### 查看已加载某一插件用途
+
 指令：/help <plugin_package_name | plugin_help_name>
 示例：
+
 ```
 /help nonebot_plugin_help
 
 @<user_who_send_command> Nonebot2 Help Menu: Nonebot2轻量级帮助插件
 欢迎使用Nonebot2 Help Menu                       // 这里是插件元数据提供的帮助
 本插件提供公共帮助菜单能力
 此Bot配置的命令前缀：/
@@ -126,15 +166,17 @@
 
 
 序号. 命令名: 命令用途                             // 这里是Matcher级别接入提供的帮助
 1. help: /help  # 获取本插件帮助
 /help list  # 展示已加载插件列表
 /help <plugin_name>  # 调取目标插件帮助信息
 ```
+
 或使用提供的插件美化名示例：
+
 ```
 /help Nonebot2 Help Menu
 
 @<user_who_send_command> Nonebot2 Help Menu: Nonebot2轻量级帮助插件
 欢迎使用Nonebot2 Help Menu                       // 这里是插件元数据提供的帮助
 本插件提供公共帮助菜单能力
 此Bot配置的命令前缀：/
@@ -146,15 +188,16 @@
 
 序号. 命令名: 命令用途                             // 这里是Matcher级别接入提供的帮助
 1. help: /help  # 获取本插件帮助
 /help list  # 展示已加载插件列表
 /help <plugin_name>  # 调取目标插件帮助信息
 ```
 
-若插件未提供__usage__，则会显示__doc__，示例：
+若插件未提供**usage**，则会显示**doc**，示例：
+
 ```
 /help nonebot_plugin_help
 
 @<user_who_send_command>
 Nonebot 2 Help Menu
 Author: XZhouQD
 Since: 16 May 2021
```

#### html2text {}

```diff
@@ -1,60 +1,83 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-help Version: 0.5.0 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-help Version: 0.6.0 Summary: A
 general help lister for nonebot2 plugins Home-page: https://github.com/XZhouQD/
 nonebot-plugin-help License: AGPL v3 Author: XZhouQD Author-email:
 X.Zhou.QD@hotmail.com Requires-Python: >=3.8.0,<4.0.0 Classifier: License ::
 Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: nonebot2
 (>=2.0.0,<3.0.0) Project-URL: Repository, https://github.com/XZhouQD/nonebot-
 plugin-help Description-Content-Type: text/markdown
 # nonebot-plugin-help ### Nonebot2 è½»éçº§å¸®å©æä»¶ [license] [pypi] [pypi
                               download] [python]
                           [python] [python] [nonebot]
-## éç½®helpæä»¶ä¼åçº§ä¸é»å¡ï¼å¯éï¼ ![nonebot-plugin-help](https:
-//img.shields.io/static/v1?label=nonebot-plugin-help&message=0.4.0&color=red)
-0.4.0çæ¬èµ·ï¼æ°å¢æä»¶ä¼åçº§ä¸é»å¡è®¾ç½®ï¼å¯éï¼ï¼é»è®¤ä¸º`priority=1,
-block=False`
-ç¨æ·å¯å¨.envéç½®æä»¶åéè¿éç½®é¡¹`help_block`ä¸`help_priority`è¿è¡éç½®ï¼ä¾å¦ï¼ä»¥ä¸éç½®å¯å°helpå½ä»¤éç½®ä¸º`priority=100,
-block=True` ``` help_block = true help_priority = 100 ``` ##
+## Botå¯å¯¹æ¬æä»¶è¿è¡çéç½® ### éç½® help
+æä»¶ä¼åçº§ä¸é»å¡ï¼å¯éï¼ ![nonebot-plugin-help](https://
+img.shields.io/static/v1?label=nonebot-plugin-help&message=0.4.0&color=red)
+0.4.0
+çæ¬èµ·ï¼æ°å¢æä»¶ä¼åçº§ä¸é»å¡è®¾ç½®ï¼å¯éï¼ï¼é»è®¤ä¸º`priority=1,
+block=False` ç¨æ·å¯å¨.env
+éç½®æä»¶åéè¿éç½®é¡¹`help_block`ä¸`help_priority`è¿è¡éç½®ï¼ä¾å¦ï¼ä»¥ä¸éç½®å¯å°
+help å½ä»¤éç½®ä¸º`priority=100, block=True` ``` help_block = true
+help_priority = 100 ``` ### éç½® help
+æä»¶å¿½ç¥åè¡¨ä¸`to_me`è§åï¼å¯éï¼ ![nonebot-plugin-help](https://
+img.shields.io/static/v1?label=nonebot-plugin-help&message=0.6.0&color=red)
+0.6.0
+çæ¬èµ·ï¼æ°å¢å¿½ç¥æä»¶ä¸`to_me`è§åï¼å¯éï¼ï¼`help_ignore_plugins`é»è®¤ä¸å¿½ç¥ä»»ä½æä»¶ï¼`to_me`é»è®¤å¼ä¸º`False`ã
+`help_ignore_plugins`ï¼å¯éç½®ä¸å¸æ help
+æä»¶ååºçæä»¶åååè¡¨ï¼ä¾å¦ï¼ä»¥ä¸éç½®å¯å¿½ç¥`nonebot_plugin_localstore`ä¸`nonebot_plugin_apscheduler`æä»¶ã
+`help_to_me`ï¼å¯éç½®æ¯å¦åªæç§èææåBotæ¶æååº help
+å½ä»¤ã ``` help_ignore_plugins=["nonebot_plugin_localstore",
+"nonebot_plugin_apscheduler"] help_to_me=true ``` ##
 å¼åèæ¥å¥æ­¤æä»¶åè¡¨æ¹æ³
 æ¨å¯ä»¥ç´æ¥åèæ¬æä»¶çæ¥å¥æ¹å¼ï¼éè¯»æºä»£ç å³å¯ï¼ ###
 æä»¶çº§å«åæ°æ®æ¥å¥ ![nonebot2](https://img.shields.io/static/
-v1?label=Nonebot&message=2.0.0%2Dbeta.4&color=red) ä½¿ç¨èª **Nonebot 2.0.0-
-beta.4**
-çæ¬èµ·æ°å¢çæä»¶åæ°æ®è¿è¡æä»¶çº§ç»ä¸æ¥å¥ï¼ä¸åå«Matcherçº§å«æ¥å¥ï¼
-```python # New way of self registering (use PluginMetadata) __plugin_meta__ =
-nonebot.plugin.PluginMetadata( name='æ¨çæä»¶åç§°ï¼æå«äºnonebot-
-plugin-xxxçååï¼', description='æ¨çç®åæä»¶æè¿°',
-usage='''æ¨æ³å¨ä½¿ç¨å½ä»¤/help æ¶æä¾çå¸®å©ææ¬''', extra=
-{'version': '0.3.1'} ) ``` ### æä»¶çº§å«ä¼ ç»æ¥å¥ ![nonebot2](https://
-img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red)
-ä½¿ç¨pythonåå½¢æçæä»¶ï¼å·²åå¸/
-èªè¡å¼åçå¯ï¼ï¼å¹¶å¨æä»¶åç__init__.pyæä»¶åå¢å å¦ä¸ä»£ç ï¼
-```python # æ¨çæä»¶çæ¬å·ï¼å°å¨/help listä¸­æ¾ç¤º # Deprecated for
-nonebot-plugin-help 0.3.1+, prefer PluginMetadata.extra['version']
-__help_version__ = '0.4.1' # æ­¤åç§°æå©äºç¾åæ¨çæä»¶å¨/help
-listä¸­çæ¾ç¤º # ä½ä½¿ç¨/help xxxæ¥è¯¢æä»¶ç¨éæ¶ä»å¿é¡»ä½¿ç¨åå
-# Deprecated for nonebot-plugin-help 0.3.0+, prefer PluginMetadata.name
-__help_plugin_name__ = "æ¨çæä»¶åç§°ï¼æå«äºnonebot-plugin-
-xxxçååï¼" # Deprecated for nonebot-plugin-help 0.3.0+, prefer
-PluginMetadata.usage # è¥æ­¤ææ¬ä¸å­å¨ï¼å°æ¾ç¤ºåç__doc__ __usage__
-= 'æ¨æ³å¨ä½¿ç¨å½ä»¤/help æ¶æä¾çå¸®å©ææ¬' ``` ###
-Matcherçº§å«æ¥å¥ ![nonebot2](https://img.shields.io/static/
-v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red)
-Matcherçº§å«å¸®å©è¯·ä¸ºMatcheræ·»å å¦ä¸ä»£ç ï¼ ```python default_start =
-list(nonebot.get_driver().config.command_start)[0] helper = on_command("help",
+v1?label=Nonebot&message=2.0.0%2Dbeta.4&color=red) ![In Use](https://
+img.shields.io/static/v1?label=Status&message=In%2DUse%26Preferred&color=green)
+ä½¿ç¨èª **Nonebot 2.0.0-beta.4**
+çæ¬èµ·æ°å¢çæä»¶åæ°æ®è¿è¡æä»¶çº§ç»ä¸æ¥å¥ï¼ä¸åå«
+Matcher çº§å«æ¥å¥ï¼ ```python # New way of self registering (use
+PluginMetadata) __plugin_meta__ = nonebot.plugin.PluginMetadata
+( name='æ¨çæä»¶åç§°ï¼æå«äºnonebot-plugin-xxxçååï¼',
+description='æ¨çç®åæä»¶æè¿°', usage='''æ¨æ³å¨ä½¿ç¨å½ä»¤/help
+æ¶æä¾çå¸®å©ææ¬''', type='{æä»¶åç±»}', # From 2.0.0 Stable
+Version,
+åå¸å¿å¡«ï¼å½åææç±»åæï¼`library`ï¼ä¸ºå¶ä»æä»¶ç¼åæä¾åè½ï¼ï¼`application`ï¼åæºå¨äººç¨æ·æä¾åè½ï¼ã
+homepage='{é¡¹ç®ä¸»é¡µ}', # From 2.0.0 Stable Version config=Config, # From
+2.0.0 Stable Version, æä»¶éç½®é¡¹ç±»ï¼å¦æ ééç½®å¯ä¸å¡«åã
+extra={'version': '0.6.0'} ) ``` ### æä»¶çº§å«ä¼ ç»æ¥å¥ ![nonebot2]
+(https://img.shields.io/static/
+v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red) ![Deprecated](https://
+img.shields.io/static/v1?label=Status&message=deprecated) ä½¿ç¨ python
+åå½¢æçæä»¶ï¼å·²åå¸/
+èªè¡å¼åçå¯ï¼ï¼å¹¶å¨æä»¶åç**init**.py
+æä»¶åå¢å å¦ä¸ä»£ç ï¼ ```python # æ¨çæä»¶çæ¬å·ï¼å°å¨/help
+listä¸­æ¾ç¤º # Deprecated for nonebot-plugin-help 0.3.1+, prefer
+PluginMetadata.extra['version'] __help_version__ = '0.6.0' #
+æ­¤åç§°æå©äºç¾åæ¨çæä»¶å¨/help listä¸­çæ¾ç¤º # ä½ä½¿ç¨/help
+xxxæ¥è¯¢æä»¶ç¨éæ¶ä»å¿é¡»ä½¿ç¨åå # Deprecated for nonebot-plugin-
+help 0.3.0+, prefer PluginMetadata.name __help_plugin_name__ =
+"æ¨çæä»¶åç§°ï¼æå«äºnonebot-plugin-xxxçååï¼" # Deprecated for
+nonebot-plugin-help 0.3.0+, prefer PluginMetadata.usage #
+è¥æ­¤ææ¬ä¸å­å¨ï¼å°æ¾ç¤ºåç__doc__ __usage__ =
+'æ¨æ³å¨ä½¿ç¨å½ä»¤/help æ¶æä¾çå¸®å©ææ¬' ``` ### Matcher
+çº§å«æ¥å¥ ![nonebot2](https://img.shields.io/static/
+v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red) ![In Use](https://
+img.shields.io/static/v1?label=Status&message=In%2DUse&color=green) Matcher
+çº§å«å¸®å©è¯·ä¸º Matcher æ·»å å¦ä¸ä»£ç ï¼ ```python default_start = list
+(nonebot.get_driver().config.command_start)[0] helper = on_command("help",
 priority=1, aliases={"å¸®å©"}) helper.__help_name__ =
 'æ¨çå½ä»¤è§¦åæä»¤å' helper.__help_info__ =
 'æ¨ä¸ºæ­¤å½ä»¤æä¾çå¸®å©ææ¬' helper.__doc__ =
 'æ¨ä¸ºæ­¤å½ä»¤æä¾çå¸®å©ææ¬,
 å½æ¨ä¸å¸æä½¿ç¨__help_info__æä¾æ¶ï¼å¯ä»¥ä½¿ç¨__doc__æä¾' ```
-è¯·æ³¨æï¼å½æ¨æªæä¾`__help_name__`æ`__help_info__`ä¸`__doc__`ä¸­çä¸ä¸ªæ¶ï¼æ­¤Matcherä¸ä¼åå¥Matcherçº§å«å¸®å©ï¼
-## å®éä½¿ç¨ æ­¤é¨åä»ç»ä»¥ä½¿ç¨'/'ä½ä¸ºcommand_startä¸ºä¾ã ###
+è¯·æ³¨æï¼å½æ¨æªæä¾`__help_name__`æ`__help_info__`ä¸`__doc__`ä¸­çä¸ä¸ªæ¶ï¼æ­¤
+Matcher ä¸ä¼åå¥ Matcher çº§å«å¸®å©ï¼ ## å®éä½¿ç¨
+æ­¤é¨åä»ç»ä»¥ä½¿ç¨'/'ä½ä¸º command_start ä¸ºä¾ã ###
 è·åæ¬æä»¶å¸®å© æä»¤ï¼ /help è¿åç¤ºä¾ï¼ ``` @
 æ¬¢è¿ä½¿ç¨Nonebot2 Help Menu æ¯æä½¿ç¨çåç¼ï¼/ /help #
 è·åæ¬æä»¶å¸®å© /help list # å±ç¤ºå·²å è½½æä»¶åè¡¨ /help  #
 è°åç®æ æä»¶å¸®å©ä¿¡æ¯ ``` ### æ¥çå·²å è½½æä»¶åè¡¨ æä»¤ï¼/
 help list è¿åç¤ºä¾ï¼ ``` @ å·²å è½½æä»¶ï¼ nonebot_plugin_cloverdata |
 åå¶èé­ç©å¨å±æ§è®¡ç®æä»¶ | 0.1.0 nonebot_plugin_guild_patch
 nonebot_plugin_help | Nonebot2 Help Menu | 0.4.1 ``` ###
@@ -73,11 +96,11 @@
 / è¿éæ¯æä»¶åæ°æ®æä¾çå¸®å©
 æ¬æä»¶æä¾å¬å±å¸®å©èåè½å æ­¤Botéç½®çå½ä»¤åç¼ï¼/ /help #
 è·åæ¬æä»¶å¸®å© /help list # å±ç¤ºå·²å è½½æä»¶åè¡¨ /help
 <æä»¶å> # è°åç®æ æä»¶å¸®å©ä¿¡æ¯ åºå·. å½ä»¤å: å½ä»¤ç¨é /
 / è¿éæ¯Matcherçº§å«æ¥å¥æä¾çå¸®å© 1. help: /help #
 è·åæ¬æä»¶å¸®å© /help list # å±ç¤ºå·²å è½½æä»¶åè¡¨ /help  #
 è°åç®æ æä»¶å¸®å©ä¿¡æ¯ ```
-è¥æä»¶æªæä¾__usage__ï¼åä¼æ¾ç¤º__doc__ï¼ç¤ºä¾ï¼ ``` /help
+è¥æä»¶æªæä¾**usage**ï¼åä¼æ¾ç¤º**doc**ï¼ç¤ºä¾ï¼ ``` /help
 nonebot_plugin_help @ Nonebot 2 Help Menu Author: XZhouQD Since: 16 May 2021
 åºå·. å½ä»¤å: å½ä»¤ç¨é 1. help: /help # è·åæ¬æä»¶å¸®å© /help
 list # å±ç¤ºå·²å è½½æä»¶åè¡¨ /help  # è°åç®æ æä»¶å¸®å©ä¿¡æ¯ ```
```

