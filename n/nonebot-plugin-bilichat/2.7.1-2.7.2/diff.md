# Comparing `tmp/nonebot_plugin_bilichat-2.7.1.tar.gz` & `tmp/nonebot_plugin_bilichat-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-2.7.1.tar", last modified: Sun Jun 18 17:45:08 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.7.2.tar", last modified: Mon Jun 19 03:28:03 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-2.7.1.tar` & `nonebot_plugin_bilichat-2.7.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    34523 2023-06-18 17:44:58.233824 nonebot_plugin_bilichat-2.7.1/LICENSE
--rw-r--r--   0        0        0    13119 2023-06-18 17:44:58.233824 nonebot_plugin_bilichat-2.7.1/README.md
--rw-r--r--   0        0        0     9452 2023-06-18 17:44:58.249824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     5512 2023-06-18 17:44:58.249824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-06-18 17:44:58.249824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-06-18 17:44:58.249824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-06-18 17:44:58.249824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      871 2023-06-18 17:44:58.249824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6502 2023-06-18 17:44:58.249824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0    15476 2023-06-18 17:44:58.249824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3812 2023-06-18 17:44:58.249824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      555 2023-06-18 17:44:58.249824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-06-18 17:44:58.249824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-06-18 17:44:58.249824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-06-18 17:44:58.249824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-06-18 17:44:58.249824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-06-18 17:44:58.249824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-06-18 17:44:58.249824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-06-18 17:44:58.249824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-06-18 17:44:58.249824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-06-18 17:44:58.249824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-06-18 17:44:58.249824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-06-18 17:44:58.253824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1187 2023-06-18 17:44:58.253824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/static/style_blue/assets/business.png
--rw-r--r--   0        0        0     1200 2023-06-18 17:44:58.253824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
--rw-r--r--   0        0        0    14952 2023-06-18 17:44:58.253824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf
--rw-r--r--   0        0        0    93905 2023-06-18 17:44:58.253824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
--rw-r--r--   0        0        0     7114 2023-06-18 17:44:58.253824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/static/style_blue/video-details.html
--rw-r--r--   0        0        0     1363 2023-06-18 17:44:58.253824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     6899 2023-06-18 17:44:58.253824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4916 2023-06-18 17:44:58.253824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2363 2023-06-18 17:44:58.253824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-06-18 17:44:58.253824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1780 2023-06-18 17:44:58.253824 nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1583 2023-06-18 17:45:08.833996 nonebot_plugin_bilichat-2.7.1/pyproject.toml
--rw-r--r--   0        0        0    14694 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.7.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-19 03:27:53.285987 nonebot_plugin_bilichat-2.7.2/LICENSE
+-rw-r--r--   0        0        0    13119 2023-06-19 03:27:53.285987 nonebot_plugin_bilichat-2.7.2/README.md
+-rw-r--r--   0        0        0     9598 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     5512 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      871 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6502 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0    15476 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3812 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      555 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1187 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    14952 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf
+-rw-r--r--   0        0        0    93905 2023-06-19 03:27:53.309988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7114 2023-06-19 03:27:53.309988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     1363 2023-06-19 03:27:53.309988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     6899 2023-06-19 03:27:53.309988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4916 2023-06-19 03:27:53.309988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2363 2023-06-19 03:27:53.309988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-06-19 03:27:53.309988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-06-19 03:27:53.309988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1583 2023-06-19 03:28:03.958270 nonebot_plugin_bilichat-2.7.2/pyproject.toml
+-rw-r--r--   0        0        0    14694 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.7.2/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-2.7.1/LICENSE` & `nonebot_plugin_bilichat-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/README.md` & `nonebot_plugin_bilichat-2.7.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -69,22 +69,31 @@
 )
 
 
 async def _bili_check(bot: BOT, event: MESSAGE_EVENT, state: T_State):
     # 检查并提取 raw_bililink
     if plugin_config.bilichat_only_self and isinstance(event, V11_ME) and event.reply:
         # 仅自身的情况下，检查是否是回复，是的话则取被回复的消息
-        msg = str(event.reply.message)
+        _msg = event.reply.message
     else:
         # 其余情况取该条消息
-        msg = str(event.get_message())
+        _msg = event.get_message()
 
-    for seg in ("av", "BV", "cv", "b23"):
-        if seg in msg:
-            state["_raw_bililink_"] = msg
+    # 如果是 B23 格式的链接，先转为正常的链接
+    _msg_str = str(_msg)
+    if "b23" in _msg_str:
+        if b23 := re.search(r"b23.(tv|wtf)[\\/]+(\w+)", _msg_str):  # type: ignore
+            state["_bililink_"] = await b23_extract(list(b23.groups()))
+            return True
+
+    # av bv cv 仅匹配纯文本部分，防止误触
+    _msg_str = _msg.extract_plain_text()
+    for seg in ("av", "AV", "bv", "BV", "cv", "CV"):
+        if seg in _msg_str:
+            state["_bililink_"] = _msg_str
             return True
     return False
 
 
 async def _permission_check(bot: BOT, event: MESSAGE_EVENT, state: T_State):
     # 检查权限
     # check if self msg
@@ -133,20 +142,15 @@
         ),  # type: ignore
         namespace=Options(),
     )[0]
 
 
 @bilichat.handle()
 async def get_bili_number(state: T_State):
-    raw_bililink = state["_raw_bililink_"]
-    # 如果是 B23 格式的链接，先转为正常的链接
-    if b23 := re.search(r"b23.(tv|wtf)[\\/]+(\w+)", raw_bililink):  # type: ignore
-        bililink = await b23_extract(list(b23.groups()))
-    else:
-        bililink = raw_bililink
+    bililink = state["_bililink_"]
     # 提取其 AV BV CV 号
     if matched := re.search(
         r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})|cv(\d{1,16})", bililink  # type: ignore
     ):
         state["bili_number"] = matched.group()
     else:
         logger.info(f"{bililink} is not video or column")
```

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/static/style_blue/assets/business.png` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/style_blue/assets/business.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/static/style_blue/assets/personal.png` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/style_blue/assets/personal.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/static/style_blue/video-details.html` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/style_blue/video-details.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.1/pyproject.toml` & `nonebot_plugin_bilichat-2.7.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "2.7.1"
+version = "2.7.2"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.4",
```

### Comparing `nonebot_plugin_bilichat-2.7.1/PKG-INFO` & `nonebot_plugin_bilichat-2.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 2.7.1
+Version: 2.7.2
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.7.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.7.2 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-Dist: nonebot-plugin-
 segbuilder>=0.2.0 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-
```

