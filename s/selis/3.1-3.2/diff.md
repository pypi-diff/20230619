# Comparing `tmp/selis-3.1.tar.gz` & `tmp/selis-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selis-3.1.tar", last modified: Mon Jun 19 05:02:48 2023, max compression
+gzip compressed data, was "selis-3.2.tar", last modified: Mon Jun 19 05:05:17 2023, max compression
```

## Comparing `selis-3.1.tar` & `selis-3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-19 05:02:48.448172 selis-3.1/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-19 05:02:48.448063 selis-3.1/PKG-INFO
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-19 05:02:48.447039 selis-3.1/selis/
--rw-r--r--   0 client     (501) staff       (20)        0 2023-06-17 14:59:11.000000 selis-3.1/selis/__init__.py
--rw-r--r--   0 client     (501) staff       (20)     3878 2023-06-19 05:01:10.000000 selis-3.1/selis/client.py
--rw-r--r--   0 client     (501) staff       (20)      786 2023-06-19 05:01:18.000000 selis-3.1/selis/computerinfo.py
--rw-r--r--   0 client     (501) staff       (20)     1148 2023-06-19 05:02:28.000000 selis-3.1/selis/selis.py
--rw-r--r--   0 client     (501) staff       (20)      289 2023-06-19 05:01:26.000000 selis-3.1/selis/utils.py
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-19 05:02:48.447906 selis-3.1/selis.egg-info/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-19 05:02:48.000000 selis-3.1/selis.egg-info/PKG-INFO
--rw-r--r--   0 client     (501) staff       (20)      270 2023-06-19 05:02:48.000000 selis-3.1/selis.egg-info/SOURCES.txt
--rw-r--r--   0 client     (501) staff       (20)        1 2023-06-19 05:02:48.000000 selis-3.1/selis.egg-info/dependency_links.txt
--rw-r--r--   0 client     (501) staff       (20)       44 2023-06-19 05:02:48.000000 selis-3.1/selis.egg-info/entry_points.txt
--rw-r--r--   0 client     (501) staff       (20)       24 2023-06-19 05:02:48.000000 selis-3.1/selis.egg-info/requires.txt
--rw-r--r--   0 client     (501) staff       (20)        6 2023-06-19 05:02:48.000000 selis-3.1/selis.egg-info/top_level.txt
--rw-r--r--   0 client     (501) staff       (20)       38 2023-06-19 05:02:48.448217 selis-3.1/setup.cfg
--rw-r--r--   0 client     (501) staff       (20)      279 2023-06-19 05:02:38.000000 selis-3.1/setup.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-19 05:05:17.479410 selis-3.2/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-19 05:05:17.479294 selis-3.2/PKG-INFO
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-19 05:05:17.478181 selis-3.2/selis/
+-rw-r--r--   0 client     (501) staff       (20)        0 2023-06-17 14:59:11.000000 selis-3.2/selis/__init__.py
+-rw-r--r--   0 client     (501) staff       (20)     3878 2023-06-19 05:01:10.000000 selis-3.2/selis/client.py
+-rw-r--r--   0 client     (501) staff       (20)      786 2023-06-19 05:01:18.000000 selis-3.2/selis/computerinfo.py
+-rw-r--r--   0 client     (501) staff       (20)     1149 2023-06-19 05:05:04.000000 selis-3.2/selis/selis.py
+-rw-r--r--   0 client     (501) staff       (20)      289 2023-06-19 05:01:26.000000 selis-3.2/selis/utils.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-19 05:05:17.479097 selis-3.2/selis.egg-info/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-19 05:05:17.000000 selis-3.2/selis.egg-info/PKG-INFO
+-rw-r--r--   0 client     (501) staff       (20)      270 2023-06-19 05:05:17.000000 selis-3.2/selis.egg-info/SOURCES.txt
+-rw-r--r--   0 client     (501) staff       (20)        1 2023-06-19 05:05:17.000000 selis-3.2/selis.egg-info/dependency_links.txt
+-rw-r--r--   0 client     (501) staff       (20)       44 2023-06-19 05:05:17.000000 selis-3.2/selis.egg-info/entry_points.txt
+-rw-r--r--   0 client     (501) staff       (20)       24 2023-06-19 05:05:17.000000 selis-3.2/selis.egg-info/requires.txt
+-rw-r--r--   0 client     (501) staff       (20)        6 2023-06-19 05:05:17.000000 selis-3.2/selis.egg-info/top_level.txt
+-rw-r--r--   0 client     (501) staff       (20)       38 2023-06-19 05:05:17.479455 selis-3.2/setup.cfg
+-rw-r--r--   0 client     (501) staff       (20)      279 2023-06-19 05:05:16.000000 selis-3.2/setup.py
```

### Comparing `selis-3.1/selis/client.py` & `selis-3.2/selis/client.py`

 * *Files identical despite different names*

### Comparing `selis-3.1/selis/computerinfo.py` & `selis-3.2/selis/computerinfo.py`

 * *Files identical despite different names*

### Comparing `selis-3.1/selis/selis.py` & `selis-3.2/selis/selis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 
 from optparse import OptionParser
-from selis.selis import ChatClient
+from selis.client import ChatClient
 
 
 def return_arguments():
     parser = OptionParser()
     parser.add_option("-v", "--version", dest="version", action="store_true", help="Show version then exit")
     parser.add_option("-p", "--port", dest="port", help="Connect to sever through this port")
     parser.add_option("-n", "--nickname", dest="nickname", help="Choose your name or a nickname")
```

