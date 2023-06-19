# Comparing `tmp/cullinan-0.51.tar.gz` & `tmp/cullinan-0.52a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cullinan-0.51.tar", last modified: Sun Apr 16 12:37:04 2023, max compression
+gzip compressed data, was "cullinan-0.52a3.tar", last modified: Mon Jun 19 18:46:59 2023, max compression
```

## Comparing `cullinan-0.51.tar` & `cullinan-0.52a3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 hansion    (501) staff       (20)        0 2023-04-16 12:37:04.928964 cullinan-0.51/
--rw-r--r--   0 hansion    (501) staff       (20)    11357 2023-04-11 05:12:10.000000 cullinan-0.51/LICENSE
--rw-r--r--   0 hansion    (501) staff       (20)     3244 2023-04-16 12:37:04.928517 cullinan-0.51/PKG-INFO
-drwxr-xr-x   0 hansion    (501) staff       (20)        0 2023-04-16 12:37:04.925787 cullinan-0.51/cullinan/
--rw-r--r--   0 hansion    (501) staff       (20)     5589 2023-04-11 05:12:10.000000 cullinan-0.51/cullinan/application.py
--rw-r--r--   0 hansion    (501) staff       (20)    23605 2023-04-11 05:12:10.000000 cullinan-0.51/cullinan/controller.py
--rw-r--r--   0 hansion    (501) staff       (20)      881 2023-04-11 05:12:10.000000 cullinan-0.51/cullinan/dao.py
--rw-r--r--   0 hansion    (501) staff       (20)     4564 2023-04-11 05:12:10.000000 cullinan-0.51/cullinan/request.py
--rw-r--r--   0 hansion    (501) staff       (20)     2111 2023-04-11 05:12:10.000000 cullinan-0.51/cullinan/service.py
-drwxr-xr-x   0 hansion    (501) staff       (20)        0 2023-04-16 12:37:04.927576 cullinan-0.51/cullinan.egg-info/
--rw-r--r--   0 hansion    (501) staff       (20)     3244 2023-04-16 12:37:04.000000 cullinan-0.51/cullinan.egg-info/PKG-INFO
--rw-r--r--   0 hansion    (501) staff       (20)      278 2023-04-16 12:37:04.000000 cullinan-0.51/cullinan.egg-info/SOURCES.txt
--rw-r--r--   0 hansion    (501) staff       (20)        1 2023-04-16 12:37:04.000000 cullinan-0.51/cullinan.egg-info/dependency_links.txt
--rw-r--r--   0 hansion    (501) staff       (20)       41 2023-04-16 12:37:04.000000 cullinan-0.51/cullinan.egg-info/requires.txt
--rw-r--r--   0 hansion    (501) staff       (20)        9 2023-04-16 12:37:04.000000 cullinan-0.51/cullinan.egg-info/top_level.txt
--rw-r--r--   0 hansion    (501) staff       (20)       38 2023-04-16 12:37:04.929187 cullinan-0.51/setup.cfg
--rw-r--r--   0 hansion    (501) staff       (20)     1282 2023-04-16 12:36:58.000000 cullinan-0.51/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:46:59.598644 cullinan-0.52a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-06-19 18:46:41.000000 cullinan-0.52a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-19 18:46:59.598644 cullinan-0.52a3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:46:59.598644 cullinan-0.52a3/cullinan/
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-06-19 18:46:41.000000 cullinan-0.52a3/cullinan/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25143 2023-06-19 18:46:41.000000 cullinan-0.52a3/cullinan/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-19 18:46:41.000000 cullinan-0.52a3/cullinan/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-19 18:46:41.000000 cullinan-0.52a3/cullinan/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-19 18:46:41.000000 cullinan-0.52a3/cullinan/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-19 18:46:41.000000 cullinan-0.52a3/cullinan/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:46:59.598644 cullinan-0.52a3/cullinan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-19 18:46:59.000000 cullinan-0.52a3/cullinan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-19 18:46:59.000000 cullinan-0.52a3/cullinan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 18:46:59.000000 cullinan-0.52a3/cullinan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-19 18:46:59.000000 cullinan-0.52a3/cullinan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 18:46:59.000000 cullinan-0.52a3/cullinan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 18:46:59.598644 cullinan-0.52a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-19 18:46:41.000000 cullinan-0.52a3/setup.py
```

### Comparing `cullinan-0.51/LICENSE` & `cullinan-0.52a3/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2023 plumeink
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cullinan-0.51/PKG-INFO` & `cullinan-0.52a3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cullinan
-Version: 0.51
+Version: 0.52a3
 Summary: Cullinan is written based on tornado and Sqlalchemy to help the project quickly build web application
 Home-page: https://github.com/plumeink/Cullinan
 Author: plumeink
-Author-email: python@plumeink.com
+Author-email: official@plumeink.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Source, https://github.com/plumeink/Cullinan
 Project-URL: Wiki, https://github.com/plumeink/Cullinan/wiki
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cullinan-0.51/cullinan/application.py` & `cullinan-0.52a3/cullinan/application.py`

 * *Files identical despite different names*

### Comparing `cullinan-0.51/cullinan/controller.py` & `cullinan-0.52a3/cullinan/controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 
 import json
 import tornado.web
+import tornado.websocket
 import types
 import functools
 from cullinan.service import service_list, response_build
 from typing import Callable
 
 handler_list = []
 header_list = []
@@ -51,14 +52,44 @@
                     return item[1]
             else:
                 servlet.set_instance_method(servlet, f)
                 servlet.f = types.MethodType(f, servlet)
                 handler_list.append((url, servlet))
                 return servlet
 
+    @staticmethod
+    def add_url_ws(url: str, cls: Callable) -> object:
+        servlet = type('Servlet' + url.replace('/', ''), (tornado.websocket.WebSocketHandler,),
+                       {"set_instance_method": EncapsulationHandler.set_fragment_method})
+        if handler_list.__len__() == 0:
+            for item in dir(cls):
+                if not item.startswith('__') and not item.endswith('__'):
+                    servlet.set_instance_method(servlet, cls.__dict__[item])
+                    servlet.f = types.MethodType(cls.__dict__[item], servlet)
+            handler_list.append((url, servlet))
+            print(servlet)
+            return servlet
+        else:
+            for item in handler_list:
+                if url == item[0]:
+                    for i in dir(cls):
+                        if not i.startswith('__') and not i.endswith('__'):
+                            item[1].set_instance_method(item[1], cls.__dict__[i])
+                            item[1].f = types.MethodType(cls.__dict__[i], item[1])
+                    print(servlet)
+                    return item[1]
+            else:
+                for item in dir(cls):
+                    if not item.startswith('__') and not item.endswith('__'):
+                        servlet.set_instance_method(servlet, cls.__dict__[item])
+                        servlet.f = types.MethodType(cls.__dict__[item], servlet)
+                handler_list.append((url, servlet))
+                print(servlet)
+                return servlet
+
 
 class Handler(tornado.web.RequestHandler):
 
     def data_received(self, chunk):
         pass
 
     def set_default_headers(self):
```

### Comparing `cullinan-0.51/cullinan/dao.py` & `cullinan-0.52a3/cullinan/dao.py`

 * *Files identical despite different names*

### Comparing `cullinan-0.51/cullinan/request.py` & `cullinan-0.52a3/cullinan/request.py`

 * *Files identical despite different names*

### Comparing `cullinan-0.51/cullinan/service.py` & `cullinan-0.52a3/cullinan/service.py`

 * *Files identical despite different names*

### Comparing `cullinan-0.51/cullinan.egg-info/PKG-INFO` & `cullinan-0.52a3/cullinan.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cullinan
-Version: 0.51
+Version: 0.52a3
 Summary: Cullinan is written based on tornado and Sqlalchemy to help the project quickly build web application
 Home-page: https://github.com/plumeink/Cullinan
 Author: plumeink
-Author-email: python@plumeink.com
+Author-email: official@plumeink.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Source, https://github.com/plumeink/Cullinan
 Project-URL: Wiki, https://github.com/plumeink/Cullinan/wiki
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cullinan-0.51/setup.py` & `cullinan-0.52a3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 
-with open("README.md", "r", encoding="UTF-8") as fh:
+with open("README.MD", "r", encoding="UTF-8") as fh:
     long_description = fh.read()
 
 setup(
     name='cullinan',
-    version='0.51',
+    version='0.52a3',
     packages=['cullinan'],
     description='Cullinan is written based on tornado and Sqlalchemy to help the project quickly build web application',
     author='plumeink',
     project_urls={
             'Source': 'https://github.com/plumeink/Cullinan',
             'Wiki': 'https://github.com/plumeink/Cullinan/wiki',
       },
     long_description=long_description,
     long_description_content_type="text/markdown",
-    author_email='python@plumeink.com',
+    author_email='official@plumeink.com',
     url='https://github.com/plumeink/Cullinan',
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

