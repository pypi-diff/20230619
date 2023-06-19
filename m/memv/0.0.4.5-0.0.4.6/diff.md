# Comparing `tmp/memv-0.0.4.5.tar.gz` & `tmp/memv-0.0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memv-0.0.4.5.tar", last modified: Mon Jun 19 04:01:09 2023, max compression
+gzip compressed data, was "memv-0.0.4.6.tar", last modified: Mon Jun 19 04:19:01 2023, max compression
```

## Comparing `memv-0.0.4.5.tar` & `memv-0.0.4.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 04:01:09.686313 memv-0.0.4.5/
--rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.4.5/LICENSE
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 04:01:09.686087 memv-0.0.4.5/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      268 2023-06-19 02:00:06.000000 memv-0.0.4.5/README.md
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 04:01:09.683599 memv-0.0.4.5/memv/
--rw-r--r--   0 nhunh      (501) staff       (20)       63 2023-06-19 04:01:02.000000 memv-0.0.4.5/memv/__init__.py
--rw-r--r--   0 nhunh      (501) staff       (20)     5219 2023-06-19 03:42:00.000000 memv-0.0.4.5/memv/memv.py
--rw-r--r--   0 nhunh      (501) staff       (20)      975 2023-06-16 10:09:56.000000 memv-0.0.4.5/memv/utils.py
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 04:01:09.685751 memv-0.0.4.5/memv.egg-info/
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 04:01:09.000000 memv-0.0.4.5/memv.egg-info/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-19 04:01:09.000000 memv-0.0.4.5/memv.egg-info/SOURCES.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-19 04:01:09.000000 memv-0.0.4.5/memv.egg-info/dependency_links.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-19 04:01:09.000000 memv-0.0.4.5/memv.egg-info/entry_points.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       35 2023-06-19 04:01:09.000000 memv-0.0.4.5/memv.egg-info/requires.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-19 04:01:09.000000 memv-0.0.4.5/memv.egg-info/top_level.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-19 04:01:09.686358 memv-0.0.4.5/setup.cfg
--rw-r--r--   0 nhunh      (501) staff       (20)      412 2023-06-19 04:01:07.000000 memv-0.0.4.5/setup.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 04:19:01.767130 memv-0.0.4.6/
+-rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.4.6/LICENSE
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 04:19:01.766942 memv-0.0.4.6/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      268 2023-06-19 02:00:06.000000 memv-0.0.4.6/README.md
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 04:19:01.764972 memv-0.0.4.6/memv/
+-rw-r--r--   0 nhunh      (501) staff       (20)       63 2023-06-19 04:01:02.000000 memv-0.0.4.6/memv/__init__.py
+-rw-r--r--   0 nhunh      (501) staff       (20)     5399 2023-06-19 04:15:59.000000 memv-0.0.4.6/memv/memv.py
+-rw-r--r--   0 nhunh      (501) staff       (20)      975 2023-06-16 10:09:56.000000 memv-0.0.4.6/memv/utils.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 04:19:01.766710 memv-0.0.4.6/memv.egg-info/
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 04:19:01.000000 memv-0.0.4.6/memv.egg-info/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-19 04:19:01.000000 memv-0.0.4.6/memv.egg-info/SOURCES.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-19 04:19:01.000000 memv-0.0.4.6/memv.egg-info/dependency_links.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-19 04:19:01.000000 memv-0.0.4.6/memv.egg-info/entry_points.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       35 2023-06-19 04:19:01.000000 memv-0.0.4.6/memv.egg-info/requires.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-19 04:19:01.000000 memv-0.0.4.6/memv.egg-info/top_level.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-19 04:19:01.767183 memv-0.0.4.6/setup.cfg
+-rw-r--r--   0 nhunh      (501) staff       (20)      412 2023-06-19 04:17:10.000000 memv-0.0.4.6/setup.py
```

### Comparing `memv-0.0.4.5/LICENSE` & `memv-0.0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `memv-0.0.4.5/memv/memv.py` & `memv-0.0.4.6/memv/memv.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,22 +10,26 @@
 import psutil
 import math
 from matplotlib.ticker import MaxNLocator
 from .utils import parseDurationToSecond
 
 parser = argparse.ArgumentParser()
 parser.add_argument('--duration', default='', help='Duration to export the memory usage. Accept format: 30s | 10m | 8h | 1d')
+parser.add_argument('--location', default='', help='Location to save the usage log file')
+
+location = tempfile.gettempdir()
+if parser.parse_args().location != '':
+    location = parser.parse_args().location
 
-temDir = tempfile.gettempdir()
 currTime = time.time()
 memDataFileName = 'mem_visualize_' + str(round(currTime)) + '.txt'
-memDataFilePath = os.path.join(temDir, memDataFileName)
+memDataFilePath = os.path.join(location, memDataFileName)
 
 cpuDataFileName = 'cpu_visualize_' + str(round(currTime)) + '.txt'
-cpuDataFilePath = os.path.join(temDir, cpuDataFileName)
+cpuDataFilePath = os.path.join(location, cpuDataFileName)
 startTime = time.time()
 
 def visualizeMemoryData():
     endTime = time.time()
     mem_timestamps = []
     mem_used = []
     mem_free = []
```

### Comparing `memv-0.0.4.5/memv/utils.py` & `memv-0.0.4.6/memv/utils.py`

 * *Files identical despite different names*

