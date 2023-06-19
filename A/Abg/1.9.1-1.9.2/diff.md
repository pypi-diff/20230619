# Comparing `tmp/Abg-1.9.1.tar.gz` & `tmp/Abg-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Abg-1.9.1.tar", last modified: Mon Jun 19 09:31:12 2023, max compression
+gzip compressed data, was "Abg-1.9.2.tar", last modified: Mon Jun 19 09:46:33 2023, max compression
```

## Comparing `Abg-1.9.1.tar` & `Abg-1.9.2.tar`

### file list

```diff
@@ -1,10 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:31:12.862737 Abg-1.9.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:31:12.862737 Abg-1.9.1/Abg.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4992 2023-06-19 09:31:12.000000 Abg-1.9.1/Abg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      126 2023-06-19 09:31:12.000000 Abg-1.9.1/Abg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 09:31:12.000000 Abg-1.9.1/Abg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 09:31:12.000000 Abg-1.9.1/Abg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     4992 2023-06-19 09:31:12.862737 Abg-1.9.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2479 2023-06-19 09:30:55.000000 Abg-1.9.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 09:31:12.862737 Abg-1.9.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2987 2023-06-19 09:30:55.000000 Abg-1.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.105302 Abg-1.9.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.101302 Abg-1.9.2/Abg/
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.101302 Abg-1.9.2/Abg/pyro/
+-rw-r--r--   0 root         (0) root         (0)      242 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.101302 Abg-1.9.2/Abg/pyro/chat_status/
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/chat_status/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5154 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/chat_status/chat_status.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/chat_status/custom_filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.101302 Abg-1.9.2/Abg/pyro/helpers/
+-rw-r--r--   0 root         (0) root         (0)      784 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3179 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/helpers/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/helpers/http_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2591 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/helpers/human_read.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/helpers/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/helpers/pyro_progress.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/helpers/ratelimit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.105302 Abg-1.9.2/Abg/pyro/inline/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/inline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6105 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/inline/inline_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     4267 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/inline/inline_pagination_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/inline/reply_keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.105302 Abg-1.9.2/Abg/pyro/patch/
+-rw-r--r--   0 root         (0) root         (0)       79 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/patch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.105302 Abg-1.9.2/Abg/pyro/patch/bound/
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/patch/bound/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11979 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/patch/bound/message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.105302 Abg-1.9.2/Abg/pyro/patch/listen/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/patch/listen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12016 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/patch/listen/listen.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/patch/listen/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.105302 Abg-1.9.2/Abg/pyro/patch/methods/
+-rw-r--r--   0 root         (0) root         (0)      127 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/patch/methods/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2172 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/patch/methods/edit_message_text.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/patch/methods/send_as_file.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/patch/methods/send_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.101302 Abg-1.9.2/Abg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4992 2023-06-19 09:46:33.000000 Abg-1.9.2/Abg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      971 2023-06-19 09:46:33.000000 Abg-1.9.2/Abg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 09:46:33.000000 Abg-1.9.2/Abg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-19 09:46:33.000000 Abg-1.9.2/Abg.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     4992 2023-06-19 09:46:33.105302 Abg-1.9.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2479 2023-06-19 09:46:08.000000 Abg-1.9.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 09:46:33.105302 Abg-1.9.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2987 2023-06-19 09:46:08.000000 Abg-1.9.2/setup.py
```

### Comparing `Abg-1.9.1/Abg.egg-info/PKG-INFO` & `Abg-1.9.2/Abg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 1.9.1
+Version: 1.9.2
 Summary: Bot Helpers
 Home-page: https://github.com/Abishnoi69
 Author: Abishnoi1M
 Author-email: Abishnoi69@Abg.org
 License: MIT
 Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
```

### Comparing `Abg-1.9.1/PKG-INFO` & `Abg-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 1.9.1
+Version: 1.9.2
 Summary: Bot Helpers
 Home-page: https://github.com/Abishnoi69
 Author: Abishnoi1M
 Author-email: Abishnoi69@Abg.org
 License: MIT
 Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
```

### Comparing `Abg-1.9.1/README.md` & `Abg-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `Abg-1.9.1/setup.py` & `Abg-1.9.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     with open(file, encoding="utf-8") as r:
         return [i.strip() for i in r]
 """
 
 setuptools.setup(
     name="Abg",
     packages=setuptools.find_packages(),
-    version="1.9.1",
+    version="1.9.2",
     description="Bot Helpers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Abishnoi69",
     download_url="https://github.com/Abishnoi69/Abg/releases/latest",
     author="Abishnoi1M",
     author_email="Abishnoi69@Abg.org",
```

