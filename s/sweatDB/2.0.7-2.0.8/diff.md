# Comparing `tmp/sweatDB-2.0.7.tar.gz` & `tmp/sweatDB-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweatDB-2.0.7.tar", last modified: Sun Jun 18 12:12:43 2023, max compression
+gzip compressed data, was "sweatDB-2.0.8.tar", last modified: Mon Jun 19 15:20:58 2023, max compression
```

## Comparing `sweatDB-2.0.7.tar` & `sweatDB-2.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-18 12:12:43.217628 sweatDB-2.0.7/
--rw-r--r--   0 sweat     (1000) sweat     (1000)      286 2023-06-18 12:12:43.217628 sweatDB-2.0.7/PKG-INFO
--rw-r--r--   0 sweat     (1000) sweat     (1000)       81 2023-06-17 12:33:57.000000 sweatDB-2.0.7/pyproject.toml
--rw-r--r--   0 sweat     (1000) sweat     (1000)       38 2023-06-18 12:12:43.217628 sweatDB-2.0.7/setup.cfg
--rw-r--r--   0 sweat     (1000) sweat     (1000)      535 2023-06-18 12:12:22.000000 sweatDB-2.0.7/setup.py
-drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-18 12:12:43.213628 sweatDB-2.0.7/sweatDB/
--rw-r--r--   0 sweat     (1000) sweat     (1000)     3891 2023-06-18 11:50:17.000000 sweatDB-2.0.7/sweatDB/__init__.py
--rw-r--r--   0 sweat     (1000) sweat     (1000)     2249 2023-06-17 12:39:49.000000 sweatDB-2.0.7/sweatDB/sweatDB.py
-drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-18 12:12:43.217628 sweatDB-2.0.7/sweatDB.egg-info/
--rw-r--r--   0 sweat     (1000) sweat     (1000)      286 2023-06-18 12:12:43.000000 sweatDB-2.0.7/sweatDB.egg-info/PKG-INFO
--rw-r--r--   0 sweat     (1000) sweat     (1000)      186 2023-06-18 12:12:43.000000 sweatDB-2.0.7/sweatDB.egg-info/SOURCES.txt
--rw-r--r--   0 sweat     (1000) sweat     (1000)        1 2023-06-18 12:12:43.000000 sweatDB-2.0.7/sweatDB.egg-info/dependency_links.txt
--rw-r--r--   0 sweat     (1000) sweat     (1000)        8 2023-06-18 12:12:43.000000 sweatDB-2.0.7/sweatDB.egg-info/top_level.txt
+drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-19 15:20:58.729199 sweatDB-2.0.8/
+-rw-r--r--   0 sweat     (1000) sweat     (1000)      286 2023-06-19 15:20:58.729199 sweatDB-2.0.8/PKG-INFO
+-rw-r--r--   0 sweat     (1000) sweat     (1000)       81 2023-06-17 12:33:57.000000 sweatDB-2.0.8/pyproject.toml
+-rw-r--r--   0 sweat     (1000) sweat     (1000)       38 2023-06-19 15:20:58.729199 sweatDB-2.0.8/setup.cfg
+-rw-r--r--   0 sweat     (1000) sweat     (1000)      535 2023-06-19 15:17:24.000000 sweatDB-2.0.8/setup.py
+drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-19 15:20:58.729199 sweatDB-2.0.8/sweatDB/
+-rw-r--r--   0 sweat     (1000) sweat     (1000)     3914 2023-06-19 15:17:02.000000 sweatDB-2.0.8/sweatDB/__init__.py
+-rw-r--r--   0 sweat     (1000) sweat     (1000)     2249 2023-06-17 12:39:49.000000 sweatDB-2.0.8/sweatDB/sweatDB.py
+drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-19 15:20:58.729199 sweatDB-2.0.8/sweatDB.egg-info/
+-rw-r--r--   0 sweat     (1000) sweat     (1000)      286 2023-06-19 15:20:58.000000 sweatDB-2.0.8/sweatDB.egg-info/PKG-INFO
+-rw-r--r--   0 sweat     (1000) sweat     (1000)      186 2023-06-19 15:20:58.000000 sweatDB-2.0.8/sweatDB.egg-info/SOURCES.txt
+-rw-r--r--   0 sweat     (1000) sweat     (1000)        1 2023-06-19 15:20:58.000000 sweatDB-2.0.8/sweatDB.egg-info/dependency_links.txt
+-rw-r--r--   0 sweat     (1000) sweat     (1000)        8 2023-06-19 15:20:58.000000 sweatDB-2.0.8/sweatDB.egg-info/top_level.txt
```

### Comparing `sweatDB-2.0.7/setup.py` & `sweatDB-2.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 setup(
     name="sweatDB",
-    version='2.0.7',
+    version='2.0.8',
     author="0xsweat",
     author_email="<0x.sweat@tutanota.com>",
     description='A python3 DBMS',
     long_description_content_type="text/markdown",
     long_description='A database management system with an easier syntax than SQL',
     packages=find_packages(),
     install_requires=[],
```

### Comparing `sweatDB-2.0.7/sweatDB/__init__.py` & `sweatDB-2.0.8/sweatDB/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import datetime
 import os
 import lzma
 version = "v2.0"
 e = os.path.isfile
-c = lzma.LZMACompressor()
 lf = lzma.LZMAFile
 class actions :
     
     # Create a database.
     
     def create(db):
         if e(db):
@@ -60,15 +59,15 @@
                 f.close()
             output = ''
             for i in b:
                 if i.startswith(f'{item}'):
                     output += ''.join([f'{x} ' for x in i.split(" ")[1:]])[:-1] + "\n"
             return output
         elif option == "items":
-            if start > end and start == 1:
+            if start > end or start == 1 or type(start) != type(1) or type(end) != type(1):
                 return(''.join([f'{x.split(" ")[0]}\n' for x in str(lf(db, 'rb').read(),'utf-8').split('\n')[1:]])[:-1])
             else:
                 return(''.join([f'{x.split(" ")[0]}\n' for x in str(lf(db, 'rb').read(),'utf-8').split('\n')[start + 1:end + 2]])[:-1])
         elif option == "info":
             return(str(lf(db, 'rb').read(),'utf-8').split("\n")[0])
         elif option == "count":
             return(str(lf(db, 'rb').read(),'utf-8').count("\n") - 1)
```

### Comparing `sweatDB-2.0.7/sweatDB/sweatDB.py` & `sweatDB-2.0.8/sweatDB/sweatDB.py`

 * *Files identical despite different names*

