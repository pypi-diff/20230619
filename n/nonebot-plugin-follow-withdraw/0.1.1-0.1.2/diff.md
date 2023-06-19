# Comparing `tmp/nonebot_plugin_follow_withdraw-0.1.1.tar.gz` & `tmp/nonebot_plugin_follow_withdraw-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_follow_withdraw-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_follow_withdraw-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_follow_withdraw-0.1.1.tar` & `nonebot_plugin_follow_withdraw-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1062 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/LICENSE
--rw-r--r--   0        0        0     2958 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/README.md
--rw-r--r--   0        0        0     2146 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/__init__.py
--rw-r--r--   0        0        0     2880 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapter.py
--rw-r--r--   0        0        0      287 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapters/__init__.py
--rw-r--r--   0        0        0     1929 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapters/discord.py
--rw-r--r--   0        0        0     1680 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapters/kaiheila.py
--rw-r--r--   0        0        0     3654 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapters/onebot.py
--rw-r--r--   0        0        0     2110 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapters/qqguild.py
--rw-r--r--   0        0        0      586 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/config.py
--rw-r--r--   0        0        0     1515 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/migrations/258421aeb463_.py
--rw-r--r--   0        0        0     3166 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/model.py
--rw-r--r--   0        0        0      856 2023-06-19 06:56:13.986397 nonebot_plugin_follow_withdraw-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3646 1970-01-01 00:00:00.000000 nonebot_plugin_follow_withdraw-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-19 07:56:03.790381 nonebot_plugin_follow_withdraw-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2958 2023-06-19 07:56:03.790381 nonebot_plugin_follow_withdraw-0.1.2/README.md
+-rw-r--r--   0        0        0     2114 2023-06-19 07:56:03.790381 nonebot_plugin_follow_withdraw-0.1.2/nonebot_plugin_follow_withdraw/__init__.py
+-rw-r--r--   0        0        0     2880 2023-06-19 07:56:03.790381 nonebot_plugin_follow_withdraw-0.1.2/nonebot_plugin_follow_withdraw/adapter.py
+-rw-r--r--   0        0        0      287 2023-06-19 07:56:03.790381 nonebot_plugin_follow_withdraw-0.1.2/nonebot_plugin_follow_withdraw/adapters/__init__.py
+-rw-r--r--   0        0        0     1929 2023-06-19 07:56:03.790381 nonebot_plugin_follow_withdraw-0.1.2/nonebot_plugin_follow_withdraw/adapters/discord.py
+-rw-r--r--   0        0        0     1680 2023-06-19 07:56:03.790381 nonebot_plugin_follow_withdraw-0.1.2/nonebot_plugin_follow_withdraw/adapters/kaiheila.py
+-rw-r--r--   0        0        0     3654 2023-06-19 07:56:03.790381 nonebot_plugin_follow_withdraw-0.1.2/nonebot_plugin_follow_withdraw/adapters/onebot.py
+-rw-r--r--   0        0        0     2110 2023-06-19 07:56:03.790381 nonebot_plugin_follow_withdraw-0.1.2/nonebot_plugin_follow_withdraw/adapters/qqguild.py
+-rw-r--r--   0        0        0      586 2023-06-19 07:56:03.790381 nonebot_plugin_follow_withdraw-0.1.2/nonebot_plugin_follow_withdraw/config.py
+-rw-r--r--   0        0        0     1515 2023-06-19 07:56:03.790381 nonebot_plugin_follow_withdraw-0.1.2/nonebot_plugin_follow_withdraw/migrations/258421aeb463_.py
+-rw-r--r--   0        0        0     3219 2023-06-19 07:56:03.790381 nonebot_plugin_follow_withdraw-0.1.2/nonebot_plugin_follow_withdraw/model.py
+-rw-r--r--   0        0        0      856 2023-06-19 07:56:03.790381 nonebot_plugin_follow_withdraw-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3646 1970-01-01 00:00:00.000000 nonebot_plugin_follow_withdraw-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_follow_withdraw-0.1.1/LICENSE` & `nonebot_plugin_follow_withdraw-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_follow_withdraw-0.1.1/README.md` & `nonebot_plugin_follow_withdraw-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/__init__.py` & `nonebot_plugin_follow_withdraw-0.1.2/nonebot_plugin_follow_withdraw/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
 withdraw_notice = on_notice(rule=check_event)
 
 
 @withdraw_notice.handle()
 async def handle_withdraw(bot: Bot, state: T_State):
     messages: Optional[List[FollowMessage]] = state.get("follow_messages")
-    print("messages", messages)
     if messages:
         for message in messages:
             await withdraw_message(bot.adapter.get_name(), bot, message)
             if not withdraw_config.folow_withdraw_all:
                 return
             await asyncio.sleep(withdraw_config.folow_withdraw_interval)
```

### Comparing `nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapter.py` & `nonebot_plugin_follow_withdraw-0.1.2/nonebot_plugin_follow_withdraw/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapters/discord.py` & `nonebot_plugin_follow_withdraw-0.1.2/nonebot_plugin_follow_withdraw/adapters/discord.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapters/kaiheila.py` & `nonebot_plugin_follow_withdraw-0.1.2/nonebot_plugin_follow_withdraw/adapters/kaiheila.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapters/onebot.py` & `nonebot_plugin_follow_withdraw-0.1.2/nonebot_plugin_follow_withdraw/adapters/onebot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/adapters/qqguild.py` & `nonebot_plugin_follow_withdraw-0.1.2/nonebot_plugin_follow_withdraw/adapters/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/config.py` & `nonebot_plugin_follow_withdraw-0.1.2/nonebot_plugin_follow_withdraw/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/migrations/258421aeb463_.py` & `nonebot_plugin_follow_withdraw-0.1.2/nonebot_plugin_follow_withdraw/migrations/258421aeb463_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_follow_withdraw-0.1.1/nonebot_plugin_follow_withdraw/model.py` & `nonebot_plugin_follow_withdraw-0.1.2/nonebot_plugin_follow_withdraw/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 ) -> None:
     async with create_session() as session:
         statement = (
             select(OriginMessage)
             .where(OriginMessage.adapter_name == adapter_name)
             .where(OriginMessage.message_id == origin_message_dict["message_id"])
             .where(OriginMessage.channel_id == origin_message_dict.get("channel_id"))
-        )
+        ).options(selectinload(OriginMessage.follow_messages))
         if result := await session.scalar(statement):
             follow_message = FollowMessage(
                 message_id=message_dict["message_id"],
                 channel_id=message_dict.get("channel_id"),
                 adapter_name=adapter_name,
                 origin_message_id=origin_message_dict["message_id"],
             )
```

### Comparing `nonebot_plugin_follow_withdraw-0.1.1/pyproject.toml` & `nonebot_plugin_follow_withdraw-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-follow-withdraw"
-version = "0.1.1"
+version = "0.1.2"
 description = "A plugin for nonebot2 that follows the user's withdraw of a command."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_follow_withdraw"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_follow_withdraw-0.1.1/PKG-INFO` & `nonebot_plugin_follow_withdraw-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-follow-withdraw
-Version: 0.1.1
+Version: 0.1.2
 Summary: A plugin for nonebot2 that follows the user's withdraw of a command.
 License: MIT
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-follow-withdraw Version: 0.1.1
+Metadata-Version: 2.1 Name: nonebot-plugin-follow-withdraw Version: 0.1.2
 Summary: A plugin for nonebot2 that follows the user's withdraw of a command.
 License: MIT Author: CMHopeSunshine Author-email: 277073121@qq.com Requires-
 Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: nonebot-plugin-datastore
```

