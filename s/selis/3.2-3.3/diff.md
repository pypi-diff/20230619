# Comparing `tmp/selis-3.2.tar.gz` & `tmp/selis-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selis-3.2.tar", last modified: Mon Jun 19 05:05:17 2023, max compression
+gzip compressed data, was "selis-3.3.tar", last modified: Mon Jun 19 05:08:36 2023, max compression
```

## Comparing `selis-3.2.tar` & `selis-3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-19 05:05:17.479410 selis-3.2/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-19 05:05:17.479294 selis-3.2/PKG-INFO
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-19 05:05:17.478181 selis-3.2/selis/
--rw-r--r--   0 client     (501) staff       (20)        0 2023-06-17 14:59:11.000000 selis-3.2/selis/__init__.py
--rw-r--r--   0 client     (501) staff       (20)     3878 2023-06-19 05:01:10.000000 selis-3.2/selis/client.py
--rw-r--r--   0 client     (501) staff       (20)      786 2023-06-19 05:01:18.000000 selis-3.2/selis/computerinfo.py
--rw-r--r--   0 client     (501) staff       (20)     1149 2023-06-19 05:05:04.000000 selis-3.2/selis/selis.py
--rw-r--r--   0 client     (501) staff       (20)      289 2023-06-19 05:01:26.000000 selis-3.2/selis/utils.py
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-19 05:05:17.479097 selis-3.2/selis.egg-info/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-19 05:05:17.000000 selis-3.2/selis.egg-info/PKG-INFO
--rw-r--r--   0 client     (501) staff       (20)      270 2023-06-19 05:05:17.000000 selis-3.2/selis.egg-info/SOURCES.txt
--rw-r--r--   0 client     (501) staff       (20)        1 2023-06-19 05:05:17.000000 selis-3.2/selis.egg-info/dependency_links.txt
--rw-r--r--   0 client     (501) staff       (20)       44 2023-06-19 05:05:17.000000 selis-3.2/selis.egg-info/entry_points.txt
--rw-r--r--   0 client     (501) staff       (20)       24 2023-06-19 05:05:17.000000 selis-3.2/selis.egg-info/requires.txt
--rw-r--r--   0 client     (501) staff       (20)        6 2023-06-19 05:05:17.000000 selis-3.2/selis.egg-info/top_level.txt
--rw-r--r--   0 client     (501) staff       (20)       38 2023-06-19 05:05:17.479455 selis-3.2/setup.cfg
--rw-r--r--   0 client     (501) staff       (20)      279 2023-06-19 05:05:16.000000 selis-3.2/setup.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-19 05:08:36.984958 selis-3.3/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-19 05:08:36.984845 selis-3.3/PKG-INFO
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-19 05:08:36.983659 selis-3.3/selis/
+-rw-r--r--   0 client     (501) staff       (20)        0 2023-06-17 14:59:11.000000 selis-3.3/selis/__init__.py
+-rw-r--r--   0 client     (501) staff       (20)     3862 2023-06-19 05:07:34.000000 selis-3.3/selis/client.py
+-rw-r--r--   0 client     (501) staff       (20)      786 2023-06-19 05:07:04.000000 selis-3.3/selis/computerinfo.py
+-rw-r--r--   0 client     (501) staff       (20)     1149 2023-06-19 05:07:57.000000 selis-3.3/selis/selis.py
+-rw-r--r--   0 client     (501) staff       (20)      289 2023-06-19 05:01:26.000000 selis-3.3/selis/utils.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-19 05:08:36.984633 selis-3.3/selis.egg-info/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-19 05:08:36.000000 selis-3.3/selis.egg-info/PKG-INFO
+-rw-r--r--   0 client     (501) staff       (20)      270 2023-06-19 05:08:36.000000 selis-3.3/selis.egg-info/SOURCES.txt
+-rw-r--r--   0 client     (501) staff       (20)        1 2023-06-19 05:08:36.000000 selis-3.3/selis.egg-info/dependency_links.txt
+-rw-r--r--   0 client     (501) staff       (20)       44 2023-06-19 05:08:36.000000 selis-3.3/selis.egg-info/entry_points.txt
+-rw-r--r--   0 client     (501) staff       (20)       24 2023-06-19 05:08:36.000000 selis-3.3/selis.egg-info/requires.txt
+-rw-r--r--   0 client     (501) staff       (20)        6 2023-06-19 05:08:36.000000 selis-3.3/selis.egg-info/top_level.txt
+-rw-r--r--   0 client     (501) staff       (20)       38 2023-06-19 05:08:36.985000 selis-3.3/setup.cfg
+-rw-r--r--   0 client     (501) staff       (20)      279 2023-06-19 05:08:14.000000 selis-3.3/setup.py
```

### Comparing `selis-3.2/selis/client.py` & `selis-3.3/selis/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import socket
 import threading
 import sys
 import webbrowser
 import getpass
 
-from module.client.computerinfo import ComputerInfo
-from module.client.utils import convert_color, guide_to_exit
+from selis.computerinfo import ComputerInfo
+from selis.utils import convert_color, guide_to_exit
 
 
 class ChatClient:
     def __init__(self, ip, port, nickname):
         self.connection = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         try:
             self.connection.connect((ip, port))
```

### Comparing `selis-3.2/selis/computerinfo.py` & `selis-3.3/selis/computerinfo.py`

 * *Files identical despite different names*

### Comparing `selis-3.2/selis/selis.py` & `selis-3.3/selis/selis.py`

 * *Files identical despite different names*

