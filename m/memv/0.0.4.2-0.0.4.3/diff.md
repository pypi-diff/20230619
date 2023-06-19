# Comparing `tmp/memv-0.0.4.2.tar.gz` & `tmp/memv-0.0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memv-0.0.4.2.tar", last modified: Mon Jun 19 02:10:46 2023, max compression
+gzip compressed data, was "memv-0.0.4.3.tar", last modified: Mon Jun 19 03:02:25 2023, max compression
```

## Comparing `memv-0.0.4.2.tar` & `memv-0.0.4.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 02:10:46.224279 memv-0.0.4.2/
--rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.4.2/LICENSE
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 02:10:46.224083 memv-0.0.4.2/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      268 2023-06-19 02:00:06.000000 memv-0.0.4.2/README.md
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 02:10:46.222231 memv-0.0.4.2/memv/
--rw-r--r--   0 nhunh      (501) staff       (20)       22 2023-06-16 09:34:09.000000 memv-0.0.4.2/memv/__init__.py
--rw-r--r--   0 nhunh      (501) staff       (20)     4434 2023-06-19 01:55:36.000000 memv-0.0.4.2/memv/memv.py
--rw-r--r--   0 nhunh      (501) staff       (20)      975 2023-06-16 10:09:56.000000 memv-0.0.4.2/memv/utils.py
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 02:10:46.223847 memv-0.0.4.2/memv.egg-info/
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 02:10:46.000000 memv-0.0.4.2/memv.egg-info/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-19 02:10:46.000000 memv-0.0.4.2/memv.egg-info/SOURCES.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-19 02:10:46.000000 memv-0.0.4.2/memv.egg-info/dependency_links.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-19 02:10:46.000000 memv-0.0.4.2/memv.egg-info/entry_points.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       35 2023-06-19 02:10:46.000000 memv-0.0.4.2/memv.egg-info/requires.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-19 02:10:46.000000 memv-0.0.4.2/memv.egg-info/top_level.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-19 02:10:46.224318 memv-0.0.4.2/setup.cfg
--rw-r--r--   0 nhunh      (501) staff       (20)      412 2023-06-19 02:10:21.000000 memv-0.0.4.2/setup.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 03:02:25.597250 memv-0.0.4.3/
+-rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.4.3/LICENSE
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 03:02:25.596983 memv-0.0.4.3/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      268 2023-06-19 02:00:06.000000 memv-0.0.4.3/README.md
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 03:02:25.593334 memv-0.0.4.3/memv/
+-rw-r--r--   0 nhunh      (501) staff       (20)       22 2023-06-16 09:34:09.000000 memv-0.0.4.3/memv/__init__.py
+-rw-r--r--   0 nhunh      (501) staff       (20)     4319 2023-06-19 03:02:08.000000 memv-0.0.4.3/memv/memv.py
+-rw-r--r--   0 nhunh      (501) staff       (20)      975 2023-06-16 10:09:56.000000 memv-0.0.4.3/memv/utils.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 03:02:25.595389 memv-0.0.4.3/memv.egg-info/
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 03:02:25.000000 memv-0.0.4.3/memv.egg-info/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-19 03:02:25.000000 memv-0.0.4.3/memv.egg-info/SOURCES.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-19 03:02:25.000000 memv-0.0.4.3/memv.egg-info/dependency_links.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-19 03:02:25.000000 memv-0.0.4.3/memv.egg-info/entry_points.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       35 2023-06-19 03:02:25.000000 memv-0.0.4.3/memv.egg-info/requires.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-19 03:02:25.000000 memv-0.0.4.3/memv.egg-info/top_level.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-19 03:02:25.597303 memv-0.0.4.3/setup.cfg
+-rw-r--r--   0 nhunh      (501) staff       (20)      412 2023-06-19 03:02:22.000000 memv-0.0.4.3/setup.py
```

### Comparing `memv-0.0.4.2/LICENSE` & `memv-0.0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `memv-0.0.4.2/memv/memv.py` & `memv-0.0.4.3/memv/memv.py`

 * *Files 14% similar despite different names*

```diff
@@ -64,40 +64,37 @@
     ax.set_title('Memory usage')
     ax.set_xlabel('Time')
     ax.set_ylabel('MB')
     ax.xaxis.set_major_locator(MaxNLocator(nbins=10))
     ax.tick_params(axis='x', rotation=90)
 
     dt_object = datetime.datetime.fromtimestamp(startTime)
-    formatted_start_time = dt_object.strftime('%Y_%m_%d_%H:%M')
+    formatted_start_time = dt_object.strftime('%Y_%m_%d_%H_%M')
     dt_object = datetime.datetime.fromtimestamp(endTime)
-    formatted_end_time = dt_object.strftime('%Y_%m_%d_%H:%M')
+    formatted_end_time = dt_object.strftime('%Y_%m_%d_%H_%M')
 
-    imageFileName = formatted_start_time + '-' + formatted_end_time + '.png'
+    imageFileName = 'RAM_' + formatted_start_time + '-' + formatted_end_time + '.png'
     plt.savefig(imageFileName, bbox_inches="tight")
     print('Created graph file:', imageFileName)
     plt.show()
 
 def signal_handler(sig, frame):
     print('Process was killed')
     sys.exit(0)
 
 signal.signal(signal.SIGTERM, signal_handler)
 
-def writeMemUsageHistory(endTime):
-    # output: PhysMem: 7585M used (1338M wired), 86M unused.
-    command = "top -l 1 -s 0 | grep PhysMem"  # your shell command here
-    
+def writeHardwareUsageHistory(endTime):    
     print('Writing memory usage history to:', memDataFilePath)
     dataFile = open(memDataFilePath, "w")
     dataFile.write('TIMESTAMP USED AVAI\n')
 
     try:
         while True:
-            time.sleep(1)
+            time.sleep(4)
             # Stop if over the endtime
             if endTime > 0:
                 if time.time() > endTime:
                     dataFile.close()
                     visualizeMemoryData()
                     break
 
@@ -126,8 +123,8 @@
     if args.duration != '':
         duration = parseDurationToSecond(args.duration)
         endTime = startTime + duration
         dt_object = datetime.datetime.fromtimestamp(endTime)
         formatted_time = dt_object.strftime('%H:%M:%S')
         print('Endtime:', formatted_time)
     
-    writeMemUsageHistory(endTime)
+    writeHardwareUsageHistory(endTime)
```

### Comparing `memv-0.0.4.2/memv/utils.py` & `memv-0.0.4.3/memv/utils.py`

 * *Files identical despite different names*

