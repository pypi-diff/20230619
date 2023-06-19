# Comparing `tmp/memv-0.0.3.7.tar.gz` & `tmp/memv-0.0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memv-0.0.3.7.tar", last modified: Fri Jun 16 10:22:13 2023, max compression
+gzip compressed data, was "memv-0.0.3.8.tar", last modified: Mon Jun 19 01:56:41 2023, max compression
```

## Comparing `memv-0.0.3.7.tar` & `memv-0.0.3.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:22:13.696215 memv-0.0.3.7/
--rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.3.7/LICENSE
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 10:22:13.695971 memv-0.0.3.7/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      244 2023-06-16 10:14:03.000000 memv-0.0.3.7/README.md
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:22:13.693534 memv-0.0.3.7/memv/
--rw-r--r--   0 nhunh      (501) staff       (20)       22 2023-06-16 09:34:09.000000 memv-0.0.3.7/memv/__init__.py
--rw-r--r--   0 nhunh      (501) staff       (20)     3745 2023-06-16 10:13:24.000000 memv-0.0.3.7/memv/memv.py
--rw-r--r--   0 nhunh      (501) staff       (20)      975 2023-06-16 10:09:56.000000 memv-0.0.3.7/memv/utils.py
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-16 10:22:13.695731 memv-0.0.3.7/memv.egg-info/
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-16 10:22:13.000000 memv-0.0.3.7/memv.egg-info/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-16 10:22:13.000000 memv-0.0.3.7/memv.egg-info/SOURCES.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-16 10:22:13.000000 memv-0.0.3.7/memv.egg-info/dependency_links.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-16 10:22:13.000000 memv-0.0.3.7/memv.egg-info/entry_points.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       65 2023-06-16 10:22:13.000000 memv-0.0.3.7/memv.egg-info/requires.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-16 10:22:13.000000 memv-0.0.3.7/memv.egg-info/top_level.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-16 10:22:13.696298 memv-0.0.3.7/setup.cfg
--rw-r--r--   0 nhunh      (501) staff       (20)      442 2023-06-16 10:22:10.000000 memv-0.0.3.7/setup.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 01:56:41.299230 memv-0.0.3.8/
+-rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.3.8/LICENSE
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 01:56:41.298933 memv-0.0.3.8/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      244 2023-06-16 10:14:03.000000 memv-0.0.3.8/README.md
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 01:56:41.296347 memv-0.0.3.8/memv/
+-rw-r--r--   0 nhunh      (501) staff       (20)       22 2023-06-16 09:34:09.000000 memv-0.0.3.8/memv/__init__.py
+-rw-r--r--   0 nhunh      (501) staff       (20)     4434 2023-06-19 01:55:36.000000 memv-0.0.3.8/memv/memv.py
+-rw-r--r--   0 nhunh      (501) staff       (20)      975 2023-06-16 10:09:56.000000 memv-0.0.3.8/memv/utils.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 01:56:41.298661 memv-0.0.3.8/memv.egg-info/
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 01:56:41.000000 memv-0.0.3.8/memv.egg-info/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-19 01:56:41.000000 memv-0.0.3.8/memv.egg-info/SOURCES.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-19 01:56:41.000000 memv-0.0.3.8/memv.egg-info/dependency_links.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-19 01:56:41.000000 memv-0.0.3.8/memv.egg-info/entry_points.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       65 2023-06-19 01:56:41.000000 memv-0.0.3.8/memv.egg-info/requires.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-19 01:56:41.000000 memv-0.0.3.8/memv.egg-info/top_level.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-19 01:56:41.299278 memv-0.0.3.8/setup.cfg
+-rw-r--r--   0 nhunh      (501) staff       (20)      442 2023-06-19 01:55:45.000000 memv-0.0.3.8/setup.py
```

### Comparing `memv-0.0.3.7/LICENSE` & `memv-0.0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `memv-0.0.3.7/memv/memv.py` & `memv-0.0.3.8/memv/memv.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,24 +4,45 @@
 import datetime
 import matplotlib.pyplot as plt
 import tempfile
 import os
 import argparse
 import numpy as np
 import psutil
-from .utils import parseDurationToSecond
+import math
 
 parser = argparse.ArgumentParser()
 parser.add_argument('--duration', default='', help='Duration to export the memory usage. Accept format: 30s | 10m | 8h | 1d')
 
 temDir = tempfile.gettempdir()
 memDataFileName = 'mem_visualize_' + str(round(time.time())) + '.txt'
 memDataFilePath = os.path.join(temDir, memDataFileName)
 startTime = time.time()
 
+def parseDurationToSecond(duration_str):
+    duration_unit = duration_str[-1]
+    duration_value_str = duration_str[:-1]
+    try:
+        duration_value = int(duration_value_str)
+    except ValueError:
+        print('Invalid duration format: ' + duration_str + '. Supported 30s | 30m | 8h | 3d')
+        return None
+    
+    if duration_unit == 's':
+        return duration_value
+    elif duration_unit == 'm':
+        return duration_value * 60
+    elif duration_unit == 'h':
+        return duration_value * 60 * 60
+    elif duration_unit == 'd':
+        return duration_value * 60 * 60 * 24
+    else:
+        print('Invalid duration format: ' + duration_str + '. Supported 30s | 30m | 8h | 3d')
+        return None
+
 def visualizeMemoryData():
     endTime = time.time()
     timestamps = []
     used = []
     free = []
 
     with open(memDataFilePath,'r') as memDataFile:
```

### Comparing `memv-0.0.3.7/memv/utils.py` & `memv-0.0.3.8/memv/utils.py`

 * *Files identical despite different names*

