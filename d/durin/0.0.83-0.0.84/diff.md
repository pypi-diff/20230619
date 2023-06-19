# Comparing `tmp/durin-0.0.83.tar.gz` & `tmp/durin-0.0.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "durin-0.0.83.tar", last modified: Fri Jun 16 14:08:22 2023, max compression
+gzip compressed data, was "durin-0.0.84.tar", last modified: Mon Jun 19 16:50:14 2023, max compression
```

## Comparing `durin-0.0.83.tar` & `durin-0.0.84.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:08:22.716153 durin-0.0.83/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-16 14:08:12.000000 durin-0.0.83/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-16 14:08:22.716153 durin-0.0.83/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2683 2023-06-16 14:08:12.000000 durin-0.0.83/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:08:22.708152 durin-0.0.83/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-06-16 14:08:12.000000 durin-0.0.83/bin/durin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:08:22.712152 durin-0.0.83/durin/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-16 14:08:12.000000 durin-0.0.83/durin/Profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-16 14:08:12.000000 durin-0.0.83/durin/Read_profilers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-06-16 14:08:12.000000 durin-0.0.83/durin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-06-16 14:08:12.000000 durin-0.0.83/durin/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-06-16 14:08:12.000000 durin-0.0.83/durin/actuator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4148 2023-06-16 14:08:12.000000 durin-0.0.83/durin/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:08:22.712152 durin-0.0.83/durin/controller/
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-06-16 14:08:12.000000 durin-0.0.83/durin/controller/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-06-16 14:08:12.000000 durin-0.0.83/durin/controller/dvs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4307 2023-06-16 14:08:12.000000 durin-0.0.83/durin/controller/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:08:22.712152 durin-0.0.83/durin/controller/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:08:12.000000 durin-0.0.83/durin/controller/test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      947 2023-06-16 14:08:12.000000 durin-0.0.83/durin/controller/test/test_stream.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4694 2023-06-16 14:08:12.000000 durin-0.0.83/durin/durin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   181742 2023-06-16 14:08:12.000000 durin-0.0.83/durin/durin_birdseye.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)      504 2023-06-16 14:08:12.000000 durin-0.0.83/durin/dvs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:08:22.712152 durin-0.0.83/durin/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-16 14:08:12.000000 durin-0.0.83/durin/examples/CPU_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:08:12.000000 durin-0.0.83/durin/examples/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2023-06-16 14:08:12.000000 durin-0.0.83/durin/examples/braitenberg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2631 2023-06-16 14:08:12.000000 durin-0.0.83/durin/examples/commands.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1448 2023-06-16 14:08:12.000000 durin-0.0.83/durin/examples/dashboard.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      923 2023-06-16 14:08:12.000000 durin-0.0.83/durin/examples/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-16 14:08:12.000000 durin-0.0.83/durin/examples/plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      589 2023-06-16 14:08:12.000000 durin-0.0.83/durin/examples/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-16 14:08:12.000000 durin-0.0.83/durin/examples/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:08:22.716153 durin-0.0.83/durin/io/
--rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-06-16 14:08:12.000000 durin-0.0.83/durin/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-16 14:08:12.000000 durin-0.0.83/durin/io/command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1418 2023-06-16 14:08:12.000000 durin-0.0.83/durin/io/gamepad.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6181 2023-06-16 14:08:12.000000 durin-0.0.83/durin/io/network.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-06-16 14:08:12.000000 durin-0.0.83/durin/io/ringbuffer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-06-16 14:08:12.000000 durin-0.0.83/durin/io/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-06-16 14:08:12.000000 durin-0.0.83/durin/io/schema.capnp
--rwxr-xr-x   0 runner    (1001) docker     (123)     7102 2023-06-16 14:08:12.000000 durin-0.0.83/durin/sensor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16014 2023-06-16 14:08:12.000000 durin-0.0.83/durin/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:08:22.712152 durin-0.0.83/durin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-16 14:08:22.000000 durin-0.0.83/durin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-16 14:08:22.000000 durin-0.0.83/durin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:08:22.000000 durin-0.0.83/durin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-16 14:08:22.000000 durin-0.0.83/durin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 14:08:22.000000 durin-0.0.83/durin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 14:08:22.716153 durin-0.0.83/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-06-16 14:08:12.000000 durin-0.0.83/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:50:14.134131 durin-0.0.84/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-19 16:50:03.000000 durin-0.0.84/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-19 16:50:14.134131 durin-0.0.84/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2683 2023-06-19 16:50:03.000000 durin-0.0.84/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:50:14.122131 durin-0.0.84/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-06-19 16:50:03.000000 durin-0.0.84/bin/durin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:50:14.126131 durin-0.0.84/durin/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-19 16:50:03.000000 durin-0.0.84/durin/Profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-19 16:50:03.000000 durin-0.0.84/durin/Read_profilers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-06-19 16:50:03.000000 durin-0.0.84/durin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-06-19 16:50:03.000000 durin-0.0.84/durin/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-06-19 16:50:03.000000 durin-0.0.84/durin/actuator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4148 2023-06-19 16:50:03.000000 durin-0.0.84/durin/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:50:14.130131 durin-0.0.84/durin/controller/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-06-19 16:50:03.000000 durin-0.0.84/durin/controller/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-06-19 16:50:03.000000 durin-0.0.84/durin/controller/dvs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4307 2023-06-19 16:50:03.000000 durin-0.0.84/durin/controller/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:50:14.130131 durin-0.0.84/durin/controller/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:50:03.000000 durin-0.0.84/durin/controller/test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      947 2023-06-19 16:50:03.000000 durin-0.0.84/durin/controller/test/test_stream.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4694 2023-06-19 16:50:03.000000 durin-0.0.84/durin/durin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   181742 2023-06-19 16:50:03.000000 durin-0.0.84/durin/durin_birdseye.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      504 2023-06-19 16:50:03.000000 durin-0.0.84/durin/dvs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:50:14.130131 durin-0.0.84/durin/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-19 16:50:03.000000 durin-0.0.84/durin/examples/CPU_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:50:03.000000 durin-0.0.84/durin/examples/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2023-06-19 16:50:03.000000 durin-0.0.84/durin/examples/braitenberg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2631 2023-06-19 16:50:03.000000 durin-0.0.84/durin/examples/commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1448 2023-06-19 16:50:03.000000 durin-0.0.84/durin/examples/dashboard.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      923 2023-06-19 16:50:03.000000 durin-0.0.84/durin/examples/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-19 16:50:03.000000 durin-0.0.84/durin/examples/plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      589 2023-06-19 16:50:03.000000 durin-0.0.84/durin/examples/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-19 16:50:03.000000 durin-0.0.84/durin/examples/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:50:14.130131 durin-0.0.84/durin/io/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-06-19 16:50:03.000000 durin-0.0.84/durin/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-19 16:50:03.000000 durin-0.0.84/durin/io/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1418 2023-06-19 16:50:03.000000 durin-0.0.84/durin/io/gamepad.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6181 2023-06-19 16:50:03.000000 durin-0.0.84/durin/io/network.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-06-19 16:50:03.000000 durin-0.0.84/durin/io/ringbuffer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-06-19 16:50:03.000000 durin-0.0.84/durin/io/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-06-19 16:50:03.000000 durin-0.0.84/durin/io/schema.capnp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7102 2023-06-19 16:50:03.000000 durin-0.0.84/durin/sensor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15427 2023-06-19 16:50:03.000000 durin-0.0.84/durin/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:50:14.126131 durin-0.0.84/durin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-19 16:50:14.000000 durin-0.0.84/durin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-19 16:50:14.000000 durin-0.0.84/durin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:50:14.000000 durin-0.0.84/durin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-19 16:50:14.000000 durin-0.0.84/durin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 16:50:14.000000 durin-0.0.84/durin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 16:50:14.134131 durin-0.0.84/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-06-19 16:50:03.000000 durin-0.0.84/setup.py
```

### Comparing `durin-0.0.83/PKG-INFO` & `durin-0.0.84/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durin
-Version: 0.0.83
+Version: 0.0.84
 Summary: Python control interface for the Durin robot
 Maintainer: Jens E. Pedersen
 Maintainer-email: jeped@kth.se
 License: LGPLv3
 Description-Content-Type: text/markdown
 Provides-Extra: aestream
```

### Comparing `durin-0.0.83/README.md` & `durin-0.0.84/README.md`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/actuator.py` & `durin-0.0.84/durin/actuator.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/cli.py` & `durin-0.0.84/durin/cli.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/controller/server.py` & `durin-0.0.84/durin/controller/server.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/controller/test/test_stream.py` & `durin-0.0.84/durin/controller/test/test_stream.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/durin.py` & `durin-0.0.84/durin/durin.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/durin_birdseye.jpg` & `durin-0.0.84/durin/durin_birdseye.jpg`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/examples/braitenberg.py` & `durin-0.0.84/durin/examples/braitenberg.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/examples/commands.py` & `durin-0.0.84/durin/examples/commands.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/examples/dashboard.py` & `durin-0.0.84/durin/examples/dashboard.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/examples/main.py` & `durin-0.0.84/durin/examples/main.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/examples/plot.py` & `durin-0.0.84/durin/examples/plot.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/examples/record.py` & `durin-0.0.84/durin/examples/record.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/examples/stats.py` & `durin-0.0.84/durin/examples/stats.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/io/__init__.py` & `durin-0.0.84/durin/io/__init__.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/io/command.py` & `durin-0.0.84/durin/io/command.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/io/gamepad.py` & `durin-0.0.84/durin/io/gamepad.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/io/network.py` & `durin-0.0.84/durin/io/network.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/io/ringbuffer.py` & `durin-0.0.84/durin/io/ringbuffer.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/io/runnable.py` & `durin-0.0.84/durin/io/runnable.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/io/schema.capnp` & `durin-0.0.84/durin/io/schema.capnp`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/sensor.py` & `durin-0.0.84/durin/sensor.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/durin/ui.py` & `durin-0.0.84/durin/ui.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import pygame
 import math
 import os
-import random
 import sys
 import ctypes
-import time
 
 import numpy as np
 from durin.actuator import Move
 
 from durin.durin import Durin
 from durin.io.gamepad import Gamepad
 from durin import SetSensorPeriod, GetSystemInfo, EnableTofStatus
@@ -57,28 +55,26 @@
 
 TOF_STATUS_PLACEMENT = (x, 0.1+25*d)
 
 
 class DurinUI(Durin):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        # self.gamepad = Gamepad()
 
         self.ip = None
         self.mac = None
         self.id = None
         self.debug = False
 
         self.vertical = 0
         self.horizontal = 0
         self.tau = 0.9999
         self.rot = 0
 
     def __enter__(self):
-        self.a = 0 # Just for debugging. Delete soon!
 
         self.set_frequency()
         self(EnableTofStatus(True))
 
         pygame.init()
         self.clock = pygame.time.Clock()
 
@@ -126,37 +122,24 @@
         # Create surfaces for ToF data.
         self.surfaces = []
         for o in range(8):
             surface = pygame.Surface((surface_width, surface_height), pygame.SRCALPHA)
             self.surfaces.append(surface)
 
         pygame.display.update()
-        # self.gamepad.start()
 
         return super().__enter__()
 
     def __exit__(self, e, b, t):
         pygame.quit()
-        # self.gamepad.stop()
         return super().__exit__(e, b, t)
 
     def read_user_input(self, allow_movement: bool = True, sleep_interval: float=0.02):
         keys = pygame.key.get_pressed()
 
-        # # Gamepad
-        # if not self.gamepad.queue.empty():
-        #     x, y, r = self.gamepad.queue.get()
-        #     self.horizontal = x
-        #     self.vertical = y
-        #     self.rot = -r
-        # else:
-        #     self.horizontal = self.horizontal - 0.1 * self.horizontal
-        #     self.vertical = self.vertical - 0.1 * self.vertical
-        #     self.rot = self.rot - 0.1 * self.rot
-
         for event in pygame.event.get():
             if event.type == pygame.QUIT or (event.type == pygame.KEYDOWN and event.key == pygame.K_ESCAPE):
                 return False
 
             # Keyboard
             elif event.type == pygame.KEYDOWN:
                 # Key pressed
@@ -203,21 +186,34 @@
             self(Move(self.horizontal, self.vertical, self.rot))
 
         # time.sleep(sleep_interval) # Sleep to avoid sending too many commands
 
         return True
 
 
-    def render_sensors(self, obs, size: int = 180):
+    def render_sensors(self, obs):
 
         self.screen.fill((0,0,0))   # Fill screen with black
         self.screen.blit(self.image_surface, (0,0))
 
+        self.update_tof(obs)
+        self.update_tof_status(obs)
+        self.update_uwb(obs)
+        self.update_battery(obs)
+        self.update_imu(obs)
+        self.update_position(obs)
+        self.update_movement_commands()
+
+        self.render_static_texts()
+
+        # Update screen
+        pygame.display.update()
 
-        # Update ToF-sensors ######################
+    def update_tof(self, obs):
+        """ Update ToF-sensors """
         tofs = (np.tanh((obs.tof / 1000)) * 255).astype(np.int32)
 
         # Rotated surfaces
         rotated_surfaces = []
 
         for o in range(len(self.surfaces)):
             surface = self.surfaces[o]
@@ -251,37 +247,34 @@
             rotation_angle = SENSOR_ROTATIONS[o]
             rotated_surface = pygame.transform.rotate(surface, rotation_angle)
             rotated_surfaces.append(rotated_surface)
 
         for i in range(8):
             self.screen.blit(rotated_surfaces[i], (SENSOR_PLACEMENTS[i][0]*self.screen_width,SENSOR_PLACEMENTS[i][1]*self.screen_height))
 
-        # Update UWB ######################
-
+    def update_uwb(self, obs):
         uwb = obs.uwb
-        #self.render_text("Becon ID\t\t\tDistance (mm)", UWB_PLACEMENT[0])
-
 
         for i in range(10):
             if uwb[i][0] != 0:
                 self.render_text(str(uwb[i][0]), (UWB_PLACEMENT[0], UWB_PLACEMENT[1] + (i+1)*d))
                 self.render_text(str(uwb[i][1]), (UWB_PLACEMENT[0]+ 7*d, UWB_PLACEMENT[1]+(i+1)*d))
             else:
                 break
 
-
-
-        # Update IMU ######################
+    def update_imu (self, obs):
         imu = obs.imu
-        #type = ["Acce", "Gyro", "Magn."]
+        # type = ["Acce", "Gyro", "Magn."]
         for type in range(3):
             for xyz in range(3):
                 self.render_text(str(imu[type][xyz]), (IMU_PLACEMENT[0]+(xyz+1)*3*d, IMU_PLACEMENT[1]+(type+1)*d))
 
-        # Update ToF status ###################
+    def update_tof_status(self, obs):
+        """ Updates the status (debugging data) of the tof-sensors """
+        
         summed_status = [0] * 8
         for i in range(8):
             tot = 0
             for v in obs.tof_status[i].flat:
                 if v != 0:
                     tot += 1
             summed_status[i] = tot
@@ -292,42 +285,31 @@
         self.render_text(f"2: {summed_status[2]}", (TOF_STATUS_PLACEMENT[0] + 2 * d * 2, TOF_STATUS_PLACEMENT[1] + d))
         self.render_text(f"3: {summed_status[3]}", (TOF_STATUS_PLACEMENT[0] + 3 * d * 2, TOF_STATUS_PLACEMENT[1] + d))
         self.render_text(f"4: {summed_status[4]}", (TOF_STATUS_PLACEMENT[0] + 0 * d * 2, TOF_STATUS_PLACEMENT[1] + d + d))
         self.render_text(f"5: {summed_status[5]}", (TOF_STATUS_PLACEMENT[0] + 1 * d * 2, TOF_STATUS_PLACEMENT[1] + d + d))
         self.render_text(f"6: {summed_status[6]}", (TOF_STATUS_PLACEMENT[0] + 2 * d * 2, TOF_STATUS_PLACEMENT[1] + d + d))
         self.render_text(f"7: {summed_status[7]}", (TOF_STATUS_PLACEMENT[0] + 3 * d * 2, TOF_STATUS_PLACEMENT[1] + d + d))
 
-        # Update battery level and voltage ######################
+    def update_battery(self, obs):
         voltage = obs.voltage
         charge = obs.charge
         self.render_text(str(charge) + " %", BATTERY_PLACEMENT)
         self.render_text(str(voltage) + " mV", (BATTERY_PLACEMENT[0]+5*d,BATTERY_PLACEMENT[1]))
 
-
-        # Update Durin position ######################
+    def update_position(self, obs):
+        # Update Durin position
         for m in range(3):
             self.render_text(str(obs.position[m]), (POSITION_PLACEMENT[0]+2*m*d, POSITION_PLACEMENT[1]+2*d))
 
-        # Update movement commands ################
+    def update_movement_commands(self):
+        # Update movement commands
         self.render_text(f"{self.horizontal:.0f}",(MV_CMD_PLACEMENT[0],MV_CMD_PLACEMENT[1]+2*d))
         self.render_text(f"{self.vertical:.0f}",(MV_CMD_PLACEMENT[0]+2*d,MV_CMD_PLACEMENT[1]+2*d))
         self.render_text(f"{self.rot:.0f}",(MV_CMD_PLACEMENT[0]+4*d,MV_CMD_PLACEMENT[1]+2*d))
 
-        self.render_static_texts()
-
-        # Just for debugging.
-        self.a += 1
-        #self.render_text("Time step (for debugging): " + str(self.a),(UWB_PLACEMENT[0],UWB_PLACEMENT[1]+10*d))
-
-        # Update screen
-        pygame.display.update()
-
-        # self.clock.tick(25)
-
-
     def render_text(self, input_text, position, color="w", size = "small"):
         if color == "w":
             c = (255,255,255)
         elif color == "o":
             c = (255,183,91)
         elif color == "b":
             c = (100,100,255)
```

### Comparing `durin-0.0.83/durin.egg-info/PKG-INFO` & `durin-0.0.84/durin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durin
-Version: 0.0.83
+Version: 0.0.84
 Summary: Python control interface for the Durin robot
 Maintainer: Jens E. Pedersen
 Maintainer-email: jeped@kth.se
 License: LGPLv3
 Description-Content-Type: text/markdown
 Provides-Extra: aestream
```

### Comparing `durin-0.0.83/durin.egg-info/SOURCES.txt` & `durin-0.0.84/durin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `durin-0.0.83/setup.py` & `durin-0.0.84/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = fp.read().split("\n")
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 setup(
     name="durin",
-    version="0.0.83",
+    version="0.0.84",
     install_requires=requirements,
     packages=find_packages(),
     license="LGPLv3",
     maintainer="Jens E. Pedersen",
     maintainer_email="jeped@kth.se",
     extras_require={"aestream": ["aestream"]},
     scripts=["bin/durin"],
```

