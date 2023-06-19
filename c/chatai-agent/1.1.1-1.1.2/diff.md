# Comparing `tmp/chatai-agent-1.1.1.tar.gz` & `tmp/chatai-agent-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatai-agent-1.1.1.tar", last modified: Wed Jun 14 20:19:22 2023, max compression
+gzip compressed data, was "chatai-agent-1.1.2.tar", last modified: Mon Jun 19 13:52:32 2023, max compression
```

## Comparing `chatai-agent-1.1.1.tar` & `chatai-agent-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-14 20:19:22.654445 chatai-agent-1.1.1/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 02:02:45.000000 chatai-agent-1.1.1/LICENSE
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      609 2023-06-14 20:19:22.654445 chatai-agent-1.1.1/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     6212 2023-06-12 17:17:48.000000 chatai-agent-1.1.1/README.md
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-14 20:19:22.654445 chatai-agent-1.1.1/setup.cfg
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1177 2023-06-14 20:01:44.000000 chatai-agent-1.1.1/setup.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-14 20:19:22.654445 chatai-agent-1.1.1/src/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     3298 2023-06-14 19:57:02.000000 chatai-agent-1.1.1/src/ChatAIAgent.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       50 2023-06-14 20:02:08.000000 chatai-agent-1.1.1/src/__init__.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-14 20:19:22.654445 chatai-agent-1.1.1/src/chatai_agent.egg-info/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      609 2023-06-14 20:19:22.000000 chatai-agent-1.1.1/src/chatai_agent.egg-info/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      299 2023-06-14 20:19:22.000000 chatai-agent-1.1.1/src/chatai_agent.egg-info/SOURCES.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-14 20:19:22.000000 chatai-agent-1.1.1/src/chatai_agent.egg-info/dependency_links.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-14 20:13:07.000000 chatai-agent-1.1.1/src/chatai_agent.egg-info/not-zip-safe
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       15 2023-06-14 20:19:22.000000 chatai-agent-1.1.1/src/chatai_agent.egg-info/requires.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       21 2023-06-14 20:19:22.000000 chatai-agent-1.1.1/src/chatai_agent.egg-info/top_level.txt
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-19 13:52:32.614221 chatai-agent-1.1.2/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 02:02:45.000000 chatai-agent-1.1.2/LICENSE
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      609 2023-06-19 13:52:32.614221 chatai-agent-1.1.2/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     6212 2023-06-12 17:17:48.000000 chatai-agent-1.1.2/README.md
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-19 13:52:32.614221 chatai-agent-1.1.2/setup.cfg
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1177 2023-06-19 13:28:29.000000 chatai-agent-1.1.2/setup.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-19 13:52:32.614221 chatai-agent-1.1.2/src/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     3369 2023-06-19 13:25:23.000000 chatai-agent-1.1.2/src/ChatAIAgent.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       50 2023-06-19 13:28:12.000000 chatai-agent-1.1.2/src/__init__.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-19 13:52:32.614221 chatai-agent-1.1.2/src/chatai_agent.egg-info/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      609 2023-06-19 13:52:32.000000 chatai-agent-1.1.2/src/chatai_agent.egg-info/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      299 2023-06-19 13:52:32.000000 chatai-agent-1.1.2/src/chatai_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-19 13:52:32.000000 chatai-agent-1.1.2/src/chatai_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-14 20:13:07.000000 chatai-agent-1.1.2/src/chatai_agent.egg-info/not-zip-safe
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       15 2023-06-19 13:52:32.000000 chatai-agent-1.1.2/src/chatai_agent.egg-info/requires.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       21 2023-06-19 13:52:32.000000 chatai-agent-1.1.2/src/chatai_agent.egg-info/top_level.txt
```

### Comparing `chatai-agent-1.1.1/LICENSE` & `chatai-agent-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatai-agent-1.1.1/PKG-INFO` & `chatai-agent-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-agent
-Version: 1.1.1
+Version: 1.1.2
 Summary: Send messages to ChatGPT and get answers conveniently.
 Home-page: https://github.com/GeneralYadoc/ChatAIAgent
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chatai-agent-1.1.1/README.md` & `chatai-agent-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `chatai-agent-1.1.1/setup.py` & `chatai-agent-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(
     name="chatai-agent",
-    version="1.1.1",
+    version="1.1.2",
     license="MIT",
     description="Send messages to ChatGPT and get answers conveniently.",
     author="General Yadoc",
     author_email="133023047+GeneralYadoc@users.noreply.github.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
```

### Comparing `chatai-agent-1.1.1/src/ChatAIAgent.py` & `chatai-agent-1.1.2/src/ChatAIAgent.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,16 @@
           time.sleep(0.1)
         if completion:
           if self.__answer_cb:
             self.__answer_cb(user_message=user_message, completion=completion)
           self.__current_context.append({"role": "assistant", "content": completion.choices[0]["message"]["content"]})
           if len(self.__current_context) >= self.__max_messages_in_context:
             self.__current_context.pop(1)
+        self.__sleep_from(start_time)
+        start_time = time.time()
       self.__sleep_from(start_time)
       start_time = time.time()
 
   def __sleep_from(self, start_time, interval_sec=None):
     if not interval_sec:
       interval_sec = self.__interval_sec
     cur_time = time.time()
```

### Comparing `chatai-agent-1.1.1/src/chatai_agent.egg-info/PKG-INFO` & `chatai-agent-1.1.2/src/chatai_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-agent
-Version: 1.1.1
+Version: 1.1.2
 Summary: Send messages to ChatGPT and get answers conveniently.
 Home-page: https://github.com/GeneralYadoc/ChatAIAgent
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

