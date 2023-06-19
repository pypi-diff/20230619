# Comparing `tmp/autopahe-2.0.tar.gz` & `tmp/autopahe-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopahe-2.0.tar", last modified: Mon Jun 19 20:10:06 2023, max compression
+gzip compressed data, was "autopahe-2.1.tar", last modified: Mon Jun 19 20:30:56 2023, max compression
```

## Comparing `autopahe-2.0.tar` & `autopahe-2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:10:06.483865 autopahe-2.0/
--rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       62 2023-06-16 06:52:54.000000 autopahe-2.0/MANIFEST.in
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6397 2023-06-19 20:10:06.483865 autopahe-2.0/PKG-INFO
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     5746 2023-06-19 20:04:44.000000 autopahe-2.0/README.md
-drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:10:06.475865 autopahe-2.0/autopahe/
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       24 2023-06-18 08:58:01.000000 autopahe-2.0/autopahe/__init__.py
--rwxrwxr-x   0 haxsys    (1000) haxsys    (1000)    19649 2023-06-19 20:02:01.000000 autopahe-2.0/autopahe/auto_pahe.py
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     4392 2023-06-19 19:43:52.000000 autopahe-2.0/autopahe/kwikdown.py
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      248 2023-06-19 19:57:40.000000 autopahe-2.0/autopahe/test.py
-drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:10:06.483865 autopahe-2.0/autopahe.egg-info/
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6397 2023-06-19 20:10:06.000000 autopahe-2.0/autopahe.egg-info/PKG-INFO
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      337 2023-06-19 20:10:06.000000 autopahe-2.0/autopahe.egg-info/SOURCES.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        1 2023-06-19 20:10:06.000000 autopahe-2.0/autopahe.egg-info/dependency_links.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       56 2023-06-19 20:10:06.000000 autopahe-2.0/autopahe.egg-info/entry_points.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       95 2023-06-19 20:10:06.000000 autopahe-2.0/autopahe.egg-info/requires.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        9 2023-06-19 20:10:06.000000 autopahe-2.0/autopahe.egg-info/top_level.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       86 2023-06-16 07:47:47.000000 autopahe-2.0/pyproject.toml
--rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       98 2023-06-16 07:18:50.000000 autopahe-2.0/requirements.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       38 2023-06-19 20:10:06.483865 autopahe-2.0/setup.cfg
--rwxrwxr-x   0 haxsys    (1000) haxsys    (1000)     1372 2023-06-19 19:27:13.000000 autopahe-2.0/setup.py
+drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:30:56.031206 autopahe-2.1/
+-rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       62 2023-06-16 06:52:54.000000 autopahe-2.1/MANIFEST.in
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6397 2023-06-19 20:30:56.027206 autopahe-2.1/PKG-INFO
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     5746 2023-06-19 20:04:44.000000 autopahe-2.1/README.md
+drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:30:56.027206 autopahe-2.1/autopahe/
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:29:36.000000 autopahe-2.1/autopahe/__init__.py
+-rwxrwxr-x   0 haxsys    (1000) haxsys    (1000)    19650 2023-06-19 20:29:25.000000 autopahe-2.1/autopahe/auto_pahe.py
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     4392 2023-06-19 19:43:52.000000 autopahe-2.1/autopahe/kwikdown.py
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      248 2023-06-19 19:57:40.000000 autopahe-2.1/autopahe/test.py
+drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:30:56.027206 autopahe-2.1/autopahe.egg-info/
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6397 2023-06-19 20:30:55.000000 autopahe-2.1/autopahe.egg-info/PKG-INFO
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      337 2023-06-19 20:30:55.000000 autopahe-2.1/autopahe.egg-info/SOURCES.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        1 2023-06-19 20:30:55.000000 autopahe-2.1/autopahe.egg-info/dependency_links.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       56 2023-06-19 20:30:55.000000 autopahe-2.1/autopahe.egg-info/entry_points.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       95 2023-06-19 20:30:55.000000 autopahe-2.1/autopahe.egg-info/requires.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        9 2023-06-19 20:30:55.000000 autopahe-2.1/autopahe.egg-info/top_level.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       86 2023-06-16 07:47:47.000000 autopahe-2.1/pyproject.toml
+-rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       98 2023-06-16 07:18:50.000000 autopahe-2.1/requirements.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       38 2023-06-19 20:30:56.031206 autopahe-2.1/setup.cfg
+-rwxrwxr-x   0 haxsys    (1000) haxsys    (1000)     1374 2023-06-19 20:30:08.000000 autopahe-2.1/setup.py
```

### Comparing `autopahe-2.0/PKG-INFO` & `autopahe-2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopahe
-Version: 2.0
+Version: 2.1
 Summary: A python script to automate downloads from animepahe
 Home-page: https://github.com/haxsysgit/autopahe
 Author: Elenasulu Arinze
 Author-email: pentacker@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `autopahe-2.0/README.md` & `autopahe-2.1/README.md`

 * *Files identical despite different names*

### Comparing `autopahe-2.0/autopahe/auto_pahe.py` & `autopahe-2.1/autopahe/auto_pahe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/python3
 import time,requests,argparse,os
 import sys
 from json import loads,load,dump
 from re import search
 from bs4 import BeautifulSoup
-from kwikdown import kwik_download
+from .kwikdown import kwik_download
 import concurrent.futures as concur
 
 
 
 start = time.perf_counter()
 
 def data_report(data:dict,filepath = "autopahe_data.json",):
```

### Comparing `autopahe-2.0/autopahe/kwikdown.py` & `autopahe-2.1/autopahe/kwikdown.py`

 * *Files identical despite different names*

### Comparing `autopahe-2.0/autopahe.egg-info/PKG-INFO` & `autopahe-2.1/autopahe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopahe
-Version: 2.0
+Version: 2.1
 Summary: A python script to automate downloads from animepahe
 Home-page: https://github.com/haxsysgit/autopahe
 Author: Elenasulu Arinze
 Author-email: pentacker@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `autopahe-2.0/setup.py` & `autopahe-2.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = 'autopahe',
-    version = '2.0',
+    version = '2.1',
     author_email="pentacker@gmail.com",
     description = "A python script to automate downloads from animepahe",
     url = "https://github.com/haxsysgit/autopahe",
     author = "Elenasulu Arinze",
     license = "MIT",
     py_modules = [
         'autopahe',
+
     ],
     package_dir = {'autopahe':'autopahe'},
     entry_points ={
             'console_scripts': ['autopahe = autopahe.auto_pahe.py:main']
     },
     include_package_data=True,
     packages = [
```

