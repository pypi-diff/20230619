# Comparing `tmp/Abg-1.3.tar.gz` & `tmp/Abg-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Abg-1.3.tar", last modified: Sun Jun 11 04:04:46 2023, max compression
+gzip compressed data, was "Abg-1.9.tar", last modified: Mon Jun 19 06:12:48 2023, max compression
```

## Comparing `Abg-1.3.tar` & `Abg-1.9.tar`

### file list

```diff
@@ -1,48 +1,9 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.720066 Abg-1.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.716066 Abg-1.3/Abg/
--rw-r--r--   0 root         (0) root         (0)      210 2023-06-11 04:03:36.000000 Abg-1.3/Abg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.716066 Abg-1.3/Abg/chat_status/
--rw-r--r--   0 root         (0) root         (0)       72 2023-06-11 04:03:36.000000 Abg-1.3/Abg/chat_status/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5273 2023-06-11 04:03:36.000000 Abg-1.3/Abg/chat_status/chat_status.py
--rw-r--r--   0 root         (0) root         (0)     2344 2023-06-11 04:03:36.000000 Abg-1.3/Abg/chat_status/custom_filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.716066 Abg-1.3/Abg/conversation/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-11 04:03:36.000000 Abg-1.3/Abg/conversation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5532 2023-06-11 04:03:36.000000 Abg-1.3/Abg/conversation/conversation.py
--rw-r--r--   0 root         (0) root         (0)      824 2023-06-11 04:03:36.000000 Abg-1.3/Abg/conversation/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.716066 Abg-1.3/Abg/helpers/
--rw-r--r--   0 root         (0) root         (0)      844 2023-06-11 04:03:36.000000 Abg-1.3/Abg/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3181 2023-06-11 04:03:36.000000 Abg-1.3/Abg/helpers/helpers.py
--rw-r--r--   0 root         (0) root         (0)     1597 2023-06-11 04:03:36.000000 Abg-1.3/Abg/helpers/http_helper.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-06-11 04:03:36.000000 Abg-1.3/Abg/helpers/human_read.py
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-11 04:03:36.000000 Abg-1.3/Abg/helpers/lock.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-06-11 04:03:36.000000 Abg-1.3/Abg/helpers/parser.py
--rw-r--r--   0 root         (0) root         (0)     2471 2023-06-11 04:03:36.000000 Abg-1.3/Abg/helpers/pyro_progress.py
--rw-r--r--   0 root         (0) root         (0)     2835 2023-06-11 04:03:36.000000 Abg-1.3/Abg/helpers/ratelimit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.716066 Abg-1.3/Abg/inline/
--rw-r--r--   0 root         (0) root         (0)      280 2023-06-11 04:03:36.000000 Abg-1.3/Abg/inline/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6245 2023-06-11 04:03:36.000000 Abg-1.3/Abg/inline/inline_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     4268 2023-06-11 04:03:36.000000 Abg-1.3/Abg/inline/inline_pagination_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     1434 2023-06-11 04:03:36.000000 Abg-1.3/Abg/inline/reply_keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.716066 Abg-1.3/Abg/patch/
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-11 04:03:36.000000 Abg-1.3/Abg/patch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.716066 Abg-1.3/Abg/patch/bound/
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-11 04:03:36.000000 Abg-1.3/Abg/patch/bound/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11748 2023-06-11 04:03:36.000000 Abg-1.3/Abg/patch/bound/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.720066 Abg-1.3/Abg/patch/listen/
--rw-r--r--   0 root         (0) root         (0)       55 2023-06-11 04:03:36.000000 Abg-1.3/Abg/patch/listen/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11641 2023-06-11 04:03:36.000000 Abg-1.3/Abg/patch/listen/listen.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-06-11 04:03:36.000000 Abg-1.3/Abg/patch/listen/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.720066 Abg-1.3/Abg/patch/methods/
--rw-r--r--   0 root         (0) root         (0)      127 2023-06-11 04:03:36.000000 Abg-1.3/Abg/patch/methods/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2127 2023-06-11 04:03:36.000000 Abg-1.3/Abg/patch/methods/edit_message_text.py
--rw-r--r--   0 root         (0) root         (0)     1634 2023-06-11 04:03:36.000000 Abg-1.3/Abg/patch/methods/send_as_file.py
--rw-r--r--   0 root         (0) root         (0)     2926 2023-06-11 04:03:36.000000 Abg-1.3/Abg/patch/methods/send_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.716066 Abg-1.3/Abg.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6936 2023-06-11 04:04:46.000000 Abg-1.3/Abg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      939 2023-06-11 04:04:46.000000 Abg-1.3/Abg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-11 04:04:46.000000 Abg-1.3/Abg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-11 04:04:46.000000 Abg-1.3/Abg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     6936 2023-06-11 04:04:46.720066 Abg-1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4097 2023-06-11 04:03:36.000000 Abg-1.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-11 04:04:46.720066 Abg-1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3071 2023-06-11 04:03:36.000000 Abg-1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 06:12:48.940524 Abg-1.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 06:12:48.940524 Abg-1.9/Abg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4999 2023-06-19 06:12:48.000000 Abg-1.9/Abg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      116 2023-06-19 06:12:48.000000 Abg-1.9/Abg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 06:12:48.000000 Abg-1.9/Abg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 06:12:48.000000 Abg-1.9/Abg.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     4999 2023-06-19 06:12:48.940524 Abg-1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 06:12:48.940524 Abg-1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2993 2023-06-19 06:12:21.000000 Abg-1.9/setup.py
```

### Comparing `Abg-1.3/setup.py` & `Abg-1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Abg - Easy conversation handler for pyrogram 
+
 #  Copyright (C) 2023-present Abishnoi6 <https://github.com/Abishnoi69>
 #
 #  This file is part of Abg.
 #
 #  Abg is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
@@ -14,41 +14,36 @@
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Abg.  If not, see <http://www.gnu.org/licenses/>.
 
 # ===================================================================
 
-import re
-from sys import argv
 import setuptools
 
-
-
-with open("README.md", encoding="utf8") as readme:
+with open(".github/README.md", encoding="utf8") as readme:
     long_description = readme.read()
 
-    
 """    
 def read(file: str) -> list:
     with open(file, encoding="utf-8") as r:
         return [i.strip() for i in r]
 """
 
 setuptools.setup(
     name="Abg",
     packages=setuptools.find_packages(),
-    version="1.3",
-    description="pyrogram helpers / add-on for pyrogram",
+    version="1.9",
+    description="Bot Helpers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Abishnoi69",
     download_url="https://github.com/Abishnoi69/Abg/releases/latest",
     author="Abishnoi1M",
-    author_email="Abishnoi69@Abg.org", 
+    author_email="Abishnoi69@Abg.org",
     license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
@@ -62,19 +57,19 @@
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Internet",
         "Topic :: Communications",
         "Topic :: Communications :: Chat",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
-        "Topic :: Software Development :: Libraries :: Application Frameworks"
+        "Topic :: Software Development :: Libraries :: Application Frameworks",
     ],
-    keywords="telegram bot chat messenger mtproto api client library python conversation keyboard userbot patch",
+    keywords="telegram bot chat messenger mtproto api client library python conversation keyboard userbot patch botapi https",
     project_urls={
         "Tracker": "https://github.com/Abishnoi69/Abg/issues",
-        "Community": "https://t.me/Abg",
+        "Community": "https://t.me/Abgpy",
         "Source": "https://github.com/Abishnoi69/Abg",
-        "Documentation": "https://github.com/Abishnoi69/Abg/wiki",
+        "Documentation": "https://github.com/Abishnoi69/Abg/tree/master/doce",
     },
     python_requires="~=3.7",
     # install_requires=read("requirements.txt")
 )
```

