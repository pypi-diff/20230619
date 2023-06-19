# Comparing `tmp/loggerflow-0.0.1.tar.gz` & `tmp/loggerflow-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggerflow-0.0.1.tar", last modified: Sun Jun 11 11:47:24 2023, max compression
+gzip compressed data, was "loggerflow-0.0.2.tar", last modified: Mon Jun 19 13:15:42 2023, max compression
```

## Comparing `loggerflow-0.0.1.tar` & `loggerflow-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 11:47:24.217833 loggerflow-0.0.1/
--rw-rw-rw-   0        0        0     1114 2023-06-10 20:34:53.000000 loggerflow-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2360 2023-06-11 11:47:24.217833 loggerflow-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1543 2023-06-11 11:45:15.000000 loggerflow-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 11:47:24.198265 loggerflow-0.0.1/loggerflow/
--rw-rw-rw-   0        0        0      242 2023-06-10 20:56:46.000000 loggerflow-0.0.1/loggerflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 11:47:24.210757 loggerflow-0.0.1/loggerflow/backends/
--rw-rw-rw-   0        0        0        0 2023-06-10 20:36:08.000000 loggerflow-0.0.1/loggerflow/backends/__init__.py
--rw-rw-rw-   0        0        0      164 2023-06-11 09:55:09.000000 loggerflow-0.0.1/loggerflow/backends/abstract_backend.py
--rw-rw-rw-   0        0        0      893 2023-06-11 09:55:09.000000 loggerflow-0.0.1/loggerflow/backends/discord.py
--rw-rw-rw-   0        0        0      156 2023-06-11 08:26:33.000000 loggerflow-0.0.1/loggerflow/backends/filters.py
--rw-rw-rw-   0        0        0     1093 2023-06-11 10:22:36.000000 loggerflow-0.0.1/loggerflow/backends/telegram.py
--rw-rw-rw-   0        0        0     2161 2023-06-11 11:16:23.000000 loggerflow-0.0.1/loggerflow/loggerflow.py
-drwxrwxrwx   0        0        0        0 2023-06-11 11:47:24.214825 loggerflow-0.0.1/loggerflow/utils/
--rw-rw-rw-   0        0        0        0 2023-06-10 20:35:33.000000 loggerflow-0.0.1/loggerflow/utils/__init__.py
--rw-rw-rw-   0        0        0      285 2023-06-11 09:31:45.000000 loggerflow-0.0.1/loggerflow/utils/handler.py
-drwxrwxrwx   0        0        0        0 2023-06-11 11:47:24.206087 loggerflow-0.0.1/loggerflow.egg-info/
--rw-rw-rw-   0        0        0     2360 2023-06-11 11:47:24.000000 loggerflow-0.0.1/loggerflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      466 2023-06-11 11:47:24.000000 loggerflow-0.0.1/loggerflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 11:47:24.000000 loggerflow-0.0.1/loggerflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-11 11:47:24.000000 loggerflow-0.0.1/loggerflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-11 11:47:24.000000 loggerflow-0.0.1/loggerflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 11:47:24.218835 loggerflow-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1159 2023-06-11 11:47:00.000000 loggerflow-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:15:42.958906 loggerflow-0.0.2/
+-rw-rw-rw-   0        0        0     1114 2023-06-10 20:34:53.000000 loggerflow-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2575 2023-06-19 13:15:42.957901 loggerflow-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1830 2023-06-19 12:51:14.000000 loggerflow-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 13:15:42.940364 loggerflow-0.0.2/loggerflow/
+-rw-rw-rw-   0        0        0      242 2023-06-10 20:56:46.000000 loggerflow-0.0.2/loggerflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:15:42.954897 loggerflow-0.0.2/loggerflow/backends/
+-rw-rw-rw-   0        0        0        0 2023-06-10 20:36:08.000000 loggerflow-0.0.2/loggerflow/backends/__init__.py
+-rw-rw-rw-   0        0        0      164 2023-06-11 09:55:09.000000 loggerflow-0.0.2/loggerflow/backends/abstract_backend.py
+-rw-rw-rw-   0        0        0      893 2023-06-11 09:55:09.000000 loggerflow-0.0.2/loggerflow/backends/discord.py
+-rw-rw-rw-   0        0        0      156 2023-06-11 08:26:33.000000 loggerflow-0.0.2/loggerflow/backends/filters.py
+-rw-rw-rw-   0        0        0     1093 2023-06-19 09:45:46.000000 loggerflow-0.0.2/loggerflow/backends/telegram.py
+-rw-rw-rw-   0        0        0     2712 2023-06-19 12:21:45.000000 loggerflow-0.0.2/loggerflow/loggerflow.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:15:42.956900 loggerflow-0.0.2/loggerflow/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-10 20:35:33.000000 loggerflow-0.0.2/loggerflow/utils/__init__.py
+-rw-rw-rw-   0        0        0      241 2023-06-19 12:19:59.000000 loggerflow-0.0.2/loggerflow/utils/handler.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:15:42.948374 loggerflow-0.0.2/loggerflow.egg-info/
+-rw-rw-rw-   0        0        0     2575 2023-06-19 13:15:42.000000 loggerflow-0.0.2/loggerflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2023-06-19 13:15:42.000000 loggerflow-0.0.2/loggerflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 13:15:42.000000 loggerflow-0.0.2/loggerflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-19 13:15:42.000000 loggerflow-0.0.2/loggerflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 13:15:42.000000 loggerflow-0.0.2/loggerflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 13:15:42.958906 loggerflow-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1076 2023-06-19 13:11:18.000000 loggerflow-0.0.2/setup.py
```

### Comparing `loggerflow-0.0.1/LICENSE` & `loggerflow-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `loggerflow-0.0.1/PKG-INFO` & `loggerflow-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: loggerflow
-Version: 0.0.1
+Version: 0.0.2
 Summary: A new level of bug tracking for your Python projects
 Home-page: https://github.com/DeNRuDi/loggerflow
-Download-URL: https://github.com/DeNRuDi/loggerflow/archive/v0.0.1.zip
 Author: DeNRuDi, kad1m
 Author-email: denisrudnitskiy0@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -28,14 +27,23 @@
  |_|_____/
 ```
 
 A new level of bug tracking for your Python projects.
 
 
 <h5> Simple start (with Telegram backend): </h5>
+<details>
+  <summary>Changes (0.0.2 - actual)</summary>
+
+  - v.0.0.2
+    - add logging in threads (to disable logging in threads - pass the parameter thread_logging=False to the LoggerFlow constructor);
+    - minor fixes;
+  - v0.0.1 
+    - create project LoggerFlow;
+</details>
 
 ```
 from loggerflow.backends.telegram import TelegramBackend
 from loggerflow import LoggerFlow
 
 
 backend = TelegramBackend(
```

### Comparing `loggerflow-0.0.1/loggerflow/backends/discord.py` & `loggerflow-0.0.2/loggerflow/backends/discord.py`

 * *Files identical despite different names*

### Comparing `loggerflow-0.0.1/loggerflow/backends/telegram.py` & `loggerflow-0.0.2/loggerflow/backends/telegram.py`

 * *Files identical despite different names*

### Comparing `loggerflow-0.0.1/loggerflow/loggerflow.py` & `loggerflow-0.0.2/loggerflow/loggerflow.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 # | |   __  \___       /     __     __    __   ___   ___   ----         __
 # | |  |__/     |     /    /   /  / __  / __  /__   /  /  /___  /     /   /   /  /  /
 # | |      ____/     /___ /___/  /___/ /___/ /___  /     /     /___  /___/   /__/__/
 # |_|_____/
 
 from loggerflow.utils.handler import LoggingHandler
 from loggerflow.backends.filters import Filter
+from typing import Union
 
+import threading
 import traceback
 import logging
 import sys
 
 
 class LoggerFlow(Filter):
-    """
-    TODO write docstring
-    """
-    def __init__(self, project_name: str, backend, disable: bool = False):
+    def __init__(self, project_name: str, backend, disable: bool = False, thread_logging: bool = True):
         self.project_name = project_name
         self.original_stdout = sys.stdout
+        self.thread_logging = thread_logging
         self.backends = backend
         self.disable = disable
 
     def write(self, text):
         if not any(note in text for note in self.traceback_filters):
             self.original_stdout.write(text)
 
@@ -33,36 +33,45 @@
                     backend.write_flow(text, self.project_name)
             else:
                 self.backends.write_flow(text, self.project_name)
 
     def flush(self):
         self.original_stdout.flush()
 
-    def exclude_output_tb_filter(self, filter_: str):
+    def exclude_output_tb_filter(self, filter_: Union[str, list]):
         """
         Exclude a filter if you need to avoid double stacktrace output (for example, if used non-standard logging)
         """
         if isinstance(filter_, str):
             self.traceback_filters.append(filter_)
+        elif isinstance(filter_, list):
+            self.traceback_filters.extend(filter_)
 
-    def exclude_sending_filter(self, filter_):
+    def exclude_sending_filter(self, filter_: Union[str, list]):
         """
         Exclude filter from sending to telegram
         """
         if isinstance(filter_, str):
             self.filters.append(filter_)
-
+        elif isinstance(filter_, list):
+            self.filters.extend(filter_)
 
     @staticmethod
     def _except_hook(exctype, value, tb):
         print("".join(traceback.format_exception(exctype, value, tb)))
 
+    def _thread_excepthook(self, args):
+        exctype, value, tb = args.exc_type, args.exc_value, args.exc_traceback
+        self._except_hook(exctype, value, tb)
+
     def run(self):
         if not self.disable:
             logging_handler = LoggingHandler(self)
             sys.excepthook = self._except_hook
+            if self.thread_logging:
+                threading.excepthook = self._thread_excepthook
             sys.stdout = self
             logging_handler.setLevel(logging.ERROR)
             logging.getLogger().addHandler(logging_handler)
```

### Comparing `loggerflow-0.0.1/loggerflow.egg-info/PKG-INFO` & `loggerflow-0.0.2/loggerflow.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: loggerflow
-Version: 0.0.1
+Version: 0.0.2
 Summary: A new level of bug tracking for your Python projects
 Home-page: https://github.com/DeNRuDi/loggerflow
-Download-URL: https://github.com/DeNRuDi/loggerflow/archive/v0.0.1.zip
 Author: DeNRuDi, kad1m
 Author-email: denisrudnitskiy0@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -28,14 +27,23 @@
  |_|_____/
 ```
 
 A new level of bug tracking for your Python projects.
 
 
 <h5> Simple start (with Telegram backend): </h5>
+<details>
+  <summary>Changes (0.0.2 - actual)</summary>
+
+  - v.0.0.2
+    - add logging in threads (to disable logging in threads - pass the parameter thread_logging=False to the LoggerFlow constructor);
+    - minor fixes;
+  - v0.0.1 
+    - create project LoggerFlow;
+</details>
 
 ```
 from loggerflow.backends.telegram import TelegramBackend
 from loggerflow import LoggerFlow
 
 
 backend = TelegramBackend(
```

### Comparing `loggerflow-0.0.1/setup.py` & `loggerflow-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from setuptools import setup, find_packages
 
 
-version = '0.0.1'
+version = '0.0.2'
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='loggerflow',
     version=version,
     packages=find_packages(),
     url='https://github.com/DeNRuDi/loggerflow',
-    download_url=f'https://github.com/DeNRuDi/loggerflow/archive/v{version}.zip',
     author='DeNRuDi, kad1m',
     author_email='denisrudnitskiy0@gmail.com',
     description='A new level of bug tracking for your Python projects',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'requests',
```

