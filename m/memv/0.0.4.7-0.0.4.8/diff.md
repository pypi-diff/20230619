# Comparing `tmp/memv-0.0.4.7.tar.gz` & `tmp/memv-0.0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memv-0.0.4.7.tar", last modified: Mon Jun 19 04:28:19 2023, max compression
+gzip compressed data, was "memv-0.0.4.8.tar", last modified: Mon Jun 19 08:01:45 2023, max compression
```

## Comparing `memv-0.0.4.7.tar` & `memv-0.0.4.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 04:28:19.374788 memv-0.0.4.7/
--rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.4.7/LICENSE
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 04:28:19.374550 memv-0.0.4.7/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      268 2023-06-19 02:00:06.000000 memv-0.0.4.7/README.md
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 04:28:19.372347 memv-0.0.4.7/memv/
--rw-r--r--   0 nhunh      (501) staff       (20)       63 2023-06-19 04:01:02.000000 memv-0.0.4.7/memv/__init__.py
--rw-r--r--   0 nhunh      (501) staff       (20)     5425 2023-06-19 04:27:25.000000 memv-0.0.4.7/memv/memv.py
--rw-r--r--   0 nhunh      (501) staff       (20)      975 2023-06-16 10:09:56.000000 memv-0.0.4.7/memv/utils.py
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 04:28:19.374166 memv-0.0.4.7/memv.egg-info/
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 04:28:19.000000 memv-0.0.4.7/memv.egg-info/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-19 04:28:19.000000 memv-0.0.4.7/memv.egg-info/SOURCES.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-19 04:28:19.000000 memv-0.0.4.7/memv.egg-info/dependency_links.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-19 04:28:19.000000 memv-0.0.4.7/memv.egg-info/entry_points.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       35 2023-06-19 04:28:19.000000 memv-0.0.4.7/memv.egg-info/requires.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-19 04:28:19.000000 memv-0.0.4.7/memv.egg-info/top_level.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-19 04:28:19.374851 memv-0.0.4.7/setup.cfg
--rw-r--r--   0 nhunh      (501) staff       (20)      412 2023-06-19 04:28:03.000000 memv-0.0.4.7/setup.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 08:01:45.634042 memv-0.0.4.8/
+-rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.4.8/LICENSE
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 08:01:45.633818 memv-0.0.4.8/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      268 2023-06-19 02:00:06.000000 memv-0.0.4.8/README.md
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 08:01:45.631807 memv-0.0.4.8/memv/
+-rw-r--r--   0 nhunh      (501) staff       (20)       63 2023-06-19 04:01:02.000000 memv-0.0.4.8/memv/__init__.py
+-rw-r--r--   0 nhunh      (501) staff       (20)     5426 2023-06-19 08:01:38.000000 memv-0.0.4.8/memv/memv.py
+-rw-r--r--   0 nhunh      (501) staff       (20)      975 2023-06-16 10:09:56.000000 memv-0.0.4.8/memv/utils.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 08:01:45.633576 memv-0.0.4.8/memv.egg-info/
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 08:01:45.000000 memv-0.0.4.8/memv.egg-info/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-19 08:01:45.000000 memv-0.0.4.8/memv.egg-info/SOURCES.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-19 08:01:45.000000 memv-0.0.4.8/memv.egg-info/dependency_links.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-19 08:01:45.000000 memv-0.0.4.8/memv.egg-info/entry_points.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       35 2023-06-19 08:01:45.000000 memv-0.0.4.8/memv.egg-info/requires.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-19 08:01:45.000000 memv-0.0.4.8/memv.egg-info/top_level.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-19 08:01:45.634108 memv-0.0.4.8/setup.cfg
+-rw-r--r--   0 nhunh      (501) staff       (20)      412 2023-06-19 08:01:42.000000 memv-0.0.4.8/setup.py
```

### Comparing `memv-0.0.4.7/LICENSE` & `memv-0.0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `memv-0.0.4.7/memv/memv.py` & `memv-0.0.4.8/memv/memv.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
     print('Writing CPU usage history to:', cpuDataFilePath)
     cpuDataFile = open(cpuDataFilePath, "w")
     cpuDataFile.write('TIMESTAMP USED AVAI\n')
 
     try:
         while True:
-            cpu_percent = psutil.cpu_percent(interval=4)
+            cpu_percent = psutil.cpu_percent(interval=30)
 
             # Stop if over the endtime
             if endTime > 0:
                 if time.time() > endTime:
                     memDataFile.close()
                     cpuDataFile.close()
                     visualizeMemoryData()
```

### Comparing `memv-0.0.4.7/memv/utils.py` & `memv-0.0.4.8/memv/utils.py`

 * *Files identical despite different names*

