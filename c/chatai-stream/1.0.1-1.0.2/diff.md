# Comparing `tmp/chatai-stream-1.0.1.tar.gz` & `tmp/chatai-stream-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatai-stream-1.0.1.tar", last modified: Wed Jun 14 21:10:06 2023, max compression
+gzip compressed data, was "chatai-stream-1.0.2.tar", last modified: Mon Jun 19 14:08:06 2023, max compression
```

## Comparing `chatai-stream-1.0.1.tar` & `chatai-stream-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-14 21:10:06.084445 chatai-stream-1.0.1/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 11:25:30.000000 chatai-stream-1.0.1/LICENSE
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      594 2023-06-14 21:10:06.084445 chatai-stream-1.0.1/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     8218 2023-06-14 20:31:00.000000 chatai-stream-1.0.1/README.md
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-14 21:10:06.084445 chatai-stream-1.0.1/setup.cfg
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1162 2023-06-14 20:29:35.000000 chatai-stream-1.0.1/setup.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-14 21:10:06.084445 chatai-stream-1.0.1/src/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1695 2023-06-12 17:34:29.000000 chatai-stream-1.0.1/src/ChatAIStream.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       51 2023-06-14 20:29:47.000000 chatai-stream-1.0.1/src/__init__.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-14 21:10:06.084445 chatai-stream-1.0.1/src/chatai_stream.egg-info/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      594 2023-06-14 21:10:06.000000 chatai-stream-1.0.1/src/chatai_stream.egg-info/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      306 2023-06-14 21:10:06.000000 chatai-stream-1.0.1/src/chatai_stream.egg-info/SOURCES.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-14 21:10:06.000000 chatai-stream-1.0.1/src/chatai_stream.egg-info/dependency_links.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        2 2023-06-14 19:57:58.000000 chatai-stream-1.0.1/src/chatai_stream.egg-info/not-zip-safe
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       44 2023-06-14 21:10:06.000000 chatai-stream-1.0.1/src/chatai_stream.egg-info/requires.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       22 2023-06-14 21:10:06.000000 chatai-stream-1.0.1/src/chatai_stream.egg-info/top_level.txt
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-19 14:08:06.134224 chatai-stream-1.0.2/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 11:25:30.000000 chatai-stream-1.0.2/LICENSE
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      594 2023-06-19 14:08:06.134224 chatai-stream-1.0.2/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     8218 2023-06-14 20:31:00.000000 chatai-stream-1.0.2/README.md
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-19 14:08:06.134224 chatai-stream-1.0.2/setup.cfg
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1162 2023-06-19 13:59:59.000000 chatai-stream-1.0.2/setup.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-19 14:08:06.134224 chatai-stream-1.0.2/src/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1695 2023-06-12 17:34:29.000000 chatai-stream-1.0.2/src/ChatAIStream.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       51 2023-06-19 14:00:09.000000 chatai-stream-1.0.2/src/__init__.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-19 14:08:06.134224 chatai-stream-1.0.2/src/chatai_stream.egg-info/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      594 2023-06-19 14:08:06.000000 chatai-stream-1.0.2/src/chatai_stream.egg-info/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      306 2023-06-19 14:08:06.000000 chatai-stream-1.0.2/src/chatai_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-19 14:08:06.000000 chatai-stream-1.0.2/src/chatai_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        2 2023-06-14 19:57:58.000000 chatai-stream-1.0.2/src/chatai_stream.egg-info/not-zip-safe
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       44 2023-06-19 14:08:06.000000 chatai-stream-1.0.2/src/chatai_stream.egg-info/requires.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       22 2023-06-19 14:08:06.000000 chatai-stream-1.0.2/src/chatai_stream.egg-info/top_level.txt
```

### Comparing `chatai-stream-1.0.1/LICENSE` & `chatai-stream-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatai-stream-1.0.1/PKG-INFO` & `chatai-stream-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-stream
-Version: 1.0.1
+Version: 1.0.2
 Summary: ChatGPT reacts YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStream
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chatai-stream-1.0.1/README.md` & `chatai-stream-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `chatai-stream-1.0.1/setup.py` & `chatai-stream-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(
     name="chatai-stream",
-    version="1.0.1",
+    version="1.0.2",
     license="MIT",
     description="ChatGPT reacts YouTube chat messages.",
     author="General Yadoc",
     author_email="133023047+GeneralYadoc@users.noreply.github.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
```

### Comparing `chatai-stream-1.0.1/src/ChatAIStream.py` & `chatai-stream-1.0.2/src/ChatAIStream.py`

 * *Files identical despite different names*

### Comparing `chatai-stream-1.0.1/src/chatai_stream.egg-info/PKG-INFO` & `chatai-stream-1.0.2/src/chatai_stream.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-stream
-Version: 1.0.1
+Version: 1.0.2
 Summary: ChatGPT reacts YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStream
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

