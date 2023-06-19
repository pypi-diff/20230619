# Comparing `tmp/pymino-1.2.1.1.tar.gz` & `tmp/pymino-1.2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\seb\pymino\dist\.tmp-9f8s1jm8\pymino-1.2.1.1.tar", last modified: Sun Jun 18 20:07:20 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\seb\pymino\dist\.tmp-tu_mvue0\pymino-1.2.1.2.tar", last modified: Mon Jun 19 00:58:20 2023, max compression
```

## Comparing `pymino-1.2.1.1.tar` & `pymino-1.2.1.2.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 20:07:20.560312 pymino-1.2.1.1/
--rw-rw-rw-   0        0        0     1085 2023-06-18 20:03:12.000000 pymino-1.2.1.1/LICENSE
--rw-rw-rw-   0        0        0     7426 2023-06-18 20:07:20.560312 pymino-1.2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     6708 2023-06-18 20:03:12.000000 pymino-1.2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 20:07:20.492857 pymino-1.2.1.1/pymino/
--rw-rw-rw-   0        0        0      721 2023-06-18 20:05:18.000000 pymino-1.2.1.1/pymino/__init__.py
--rw-rw-rw-   0        0        0     7986 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/async_bot.py
--rw-rw-rw-   0        0        0    30208 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/bot.py
--rw-rw-rw-   0        0        0    65900 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-06-18 20:07:20.526088 pymino-1.2.1.1/pymino/ext/
--rw-rw-rw-   0        0        0      498 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0      192 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/_global.py
--rw-rw-rw-   0        0        0    13871 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/account.py
--rw-rw-rw-   0        0        0   328859 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    18079 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    24095 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0     7238 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   327444 2023-06-18 20:06:03.000000 pymino-1.2.1.1/pymino/ext/community.py
--rw-rw-rw-   0        0        0     3040 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/console.py
--rw-rw-rw-   0        0        0    42101 2023-06-18 20:06:09.000000 pymino-1.2.1.1/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1758 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-18 20:07:20.546920 pymino-1.2.1.1/pymino/ext/entities/
--rw-rw-rw-   0        0        0      355 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     8044 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/acm.py
--rw-rw-rw-   0        0        0     1670 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    20322 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    15638 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43596 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4802 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0     3831 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/member.py
--rw-rw-rw-   0        0        0    42520 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1847 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0     6185 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    31609 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0      543 2023-06-18 20:06:18.000000 pymino-1.2.1.1/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6729 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-06-18 20:07:20.558825 pymino-1.2.1.1/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11320 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0    11309 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6396 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     2078 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1110 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2911 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     2106 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10274 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-18 20:07:20.507765 pymino-1.2.1.1/pymino.egg-info/
--rw-rw-rw-   0        0        0     7426 2023-06-18 20:07:20.000000 pymino-1.2.1.1/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1433 2023-06-18 20:07:20.000000 pymino-1.2.1.1/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 20:07:20.000000 pymino-1.2.1.1/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-06-18 20:07:20.000000 pymino-1.2.1.1/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-18 20:07:20.000000 pymino-1.2.1.1/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-06-18 20:07:20.562296 pymino-1.2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-06-18 20:03:12.000000 pymino-1.2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 00:58:20.176039 pymino-1.2.1.2/
+-rw-rw-rw-   0        0        0     1085 2023-06-18 20:03:12.000000 pymino-1.2.1.2/LICENSE
+-rw-rw-rw-   0        0        0     7426 2023-06-19 00:58:20.176535 pymino-1.2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6708 2023-06-18 20:03:12.000000 pymino-1.2.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 00:58:20.090231 pymino-1.2.1.2/pymino/
+-rw-rw-rw-   0        0        0      721 2023-06-19 00:57:26.000000 pymino-1.2.1.2/pymino/__init__.py
+-rw-rw-rw-   0        0        0     7986 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    30208 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/bot.py
+-rw-rw-rw-   0        0        0    65900 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-06-19 00:58:20.131895 pymino-1.2.1.2/pymino/ext/
+-rw-rw-rw-   0        0        0      498 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0      192 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/_global.py
+-rw-rw-rw-   0        0        0    13871 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   328859 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    18079 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    24095 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0     7238 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   327444 2023-06-18 20:06:03.000000 pymino-1.2.1.2/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     3040 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    42101 2023-06-18 20:06:09.000000 pymino-1.2.1.2/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1758 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-19 00:58:20.159671 pymino-1.2.1.2/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      402 2023-06-19 00:16:35.000000 pymino-1.2.1.2/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     8044 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/acm.py
+-rw-rw-rw-   0        0        0     1670 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    17769 2023-06-19 00:57:52.000000 pymino-1.2.1.2/pymino/ext/entities/bubble.py
+-rw-rw-rw-   0        0        0    20322 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    15638 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43596 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4802 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0     3831 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/member.py
+-rw-rw-rw-   0        0        0    42520 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1847 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31711 2023-06-19 00:56:50.000000 pymino-1.2.1.2/pymino/ext/entities/sticker.py
+-rw-rw-rw-   0        0        0     6185 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    31609 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0      543 2023-06-18 20:06:18.000000 pymino-1.2.1.2/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6729 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-06-19 00:58:20.175047 pymino-1.2.1.2/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11320 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0    11309 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6396 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     2078 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1110 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2911 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2106 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10274 2023-06-18 20:03:12.000000 pymino-1.2.1.2/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-19 00:58:20.109575 pymino-1.2.1.2/pymino.egg-info/
+-rw-rw-rw-   0        0        0     7426 2023-06-19 00:58:20.000000 pymino-1.2.1.2/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1494 2023-06-19 00:58:20.000000 pymino-1.2.1.2/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 00:58:20.000000 pymino-1.2.1.2/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-06-19 00:58:20.000000 pymino-1.2.1.2/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-19 00:58:20.000000 pymino-1.2.1.2/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-06-19 00:58:20.182983 pymino-1.2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-06-18 20:03:12.000000 pymino-1.2.1.2/setup.py
```

### Comparing `pymino-1.2.1.1/LICENSE` & `pymino-1.2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/PKG-INFO` & `pymino-1.2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.1.1
+Version: 1.2.1.2
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.1.1 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.1.2 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.2.1.1/README.md` & `pymino-1.2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/__init__.py` & `pymino-1.2.1.2/pymino/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.2.1.1'
+__version__ = '1.2.1.2'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .async_bot import AsyncBot as AsyncBot
 from .client import Client as Client
 
 from requests import get
```

### Comparing `pymino-1.2.1.1/pymino/async_bot.py` & `pymino-1.2.1.2/pymino/async_bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/bot.py` & `pymino-1.2.1.2/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/client.py` & `pymino-1.2.1.2/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/account.py` & `pymino-1.2.1.2/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/async_community.py` & `pymino-1.2.1.2/pymino/ext/async_community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/async_context.py` & `pymino-1.2.1.2/pymino/ext/async_context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/async_event_handler.py` & `pymino-1.2.1.2/pymino/ext/async_event_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/async_socket.py` & `pymino-1.2.1.2/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/community.py` & `pymino-1.2.1.2/pymino/ext/community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/console.py` & `pymino-1.2.1.2/pymino/ext/console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/context.py` & `pymino-1.2.1.2/pymino/ext/context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/dispatcher.py` & `pymino-1.2.1.2/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/entities/acm.py` & `pymino-1.2.1.2/pymino/ext/entities/acm.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/entities/api_response.py` & `pymino-1.2.1.2/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/entities/chat_threads.py` & `pymino-1.2.1.2/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/entities/comments.py` & `pymino-1.2.1.2/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/entities/enums.py` & `pymino-1.2.1.2/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/entities/exceptions.py` & `pymino-1.2.1.2/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/entities/general.py` & `pymino-1.2.1.2/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/entities/handlers.py` & `pymino-1.2.1.2/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/entities/link_info.py` & `pymino-1.2.1.2/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/entities/member.py` & `pymino-1.2.1.2/pymino/ext/entities/member.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/entities/messages.py` & `pymino-1.2.1.2/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/entities/notification.py` & `pymino-1.2.1.2/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/entities/threads.py` & `pymino-1.2.1.2/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/entities/userprofile.py` & `pymino-1.2.1.2/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/entities/wsevents.py` & `pymino-1.2.1.2/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/handle_queue.py` & `pymino-1.2.1.2/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/socket.py` & `pymino-1.2.1.2/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/utilities/async_request_handler.py` & `pymino-1.2.1.2/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/utilities/chat_console.py` & `pymino-1.2.1.2/pymino/ext/utilities/chat_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/utilities/commands.py` & `pymino-1.2.1.2/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/utilities/community_console.py` & `pymino-1.2.1.2/pymino/ext/utilities/community_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/utilities/generate.py` & `pymino-1.2.1.2/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/utilities/menu.py` & `pymino-1.2.1.2/pymino/ext/utilities/menu.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/utilities/profile_console.py` & `pymino-1.2.1.2/pymino/ext/utilities/profile_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino/ext/utilities/request_handler.py` & `pymino-1.2.1.2/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.1/pymino.egg-info/PKG-INFO` & `pymino-1.2.1.2/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.1.1
+Version: 1.2.1.2
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.1.1 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.1.2 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.2.1.1/pymino.egg-info/SOURCES.txt` & `pymino-1.2.1.2/pymino.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,24 +23,26 @@
 pymino/ext/context.py
 pymino/ext/dispatcher.py
 pymino/ext/handle_queue.py
 pymino/ext/socket.py
 pymino/ext/entities/__init__.py
 pymino/ext/entities/acm.py
 pymino/ext/entities/api_response.py
+pymino/ext/entities/bubble.py
 pymino/ext/entities/chat_threads.py
 pymino/ext/entities/comments.py
 pymino/ext/entities/enums.py
 pymino/ext/entities/exceptions.py
 pymino/ext/entities/general.py
 pymino/ext/entities/handlers.py
 pymino/ext/entities/link_info.py
 pymino/ext/entities/member.py
 pymino/ext/entities/messages.py
 pymino/ext/entities/notification.py
+pymino/ext/entities/sticker.py
 pymino/ext/entities/threads.py
 pymino/ext/entities/userprofile.py
 pymino/ext/entities/wsevents.py
 pymino/ext/utilities/__init__.py
 pymino/ext/utilities/async_request_handler.py
 pymino/ext/utilities/chat_console.py
 pymino/ext/utilities/commands.py
```

### Comparing `pymino-1.2.1.1/setup.cfg` & `pymino-1.2.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e32 2e31 2e31 0d0a 6175  on = 1.2.1.1..au
+00000020: 6f6e 203d 2031 2e32 2e31 2e32 0d0a 6175  on = 1.2.1.2..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.2.1.1/setup.py` & `pymino-1.2.1.2/setup.py`

 * *Files identical despite different names*

