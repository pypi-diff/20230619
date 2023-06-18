# Comparing `tmp/sysdm-0.8.65.tar.gz` & `tmp/sysdm-0.8.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysdm-0.8.65.tar", last modified: Sat Nov  5 00:14:14 2022, max compression
+gzip compressed data, was "sysdm-0.8.67.tar", last modified: Sun Jun 18 22:53:49 2023, max compression
```

## Comparing `sysdm-0.8.65.tar` & `sysdm-0.8.67.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2022-11-05 00:14:14.814686 sysdm-0.8.65/
--rw-r--r--   0 pascal    (1000) pascal    (1000)      182 2019-05-07 22:15:54.000000 sysdm-0.8.65/.gitignore
--rw-r--r--   0 pascal    (1000) pascal    (1000)     3466 2022-11-05 00:14:14.814686 sysdm-0.8.65/PKG-INFO
--rw-r--r--   0 pascal    (1000) pascal    (1000)     1764 2019-10-07 10:33:57.000000 sysdm-0.8.65/README.md
--rw-r--r--   0 pascal    (1000) pascal    (1000)  4237450 2020-01-09 22:43:45.000000 sysdm-0.8.65/demo.gif
--rw-r--r--   0 pascal    (1000) pascal    (1000)      912 2019-03-29 17:35:00.000000 sysdm-0.8.65/deploy.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)    23405 2019-10-07 10:35:38.000000 sysdm-0.8.65/logo.png
--rw-r--r--   0 pascal    (1000) pascal    (1000)      137 2022-11-05 00:14:14.814686 sysdm-0.8.65/setup.cfg
--rw-r--r--   0 pascal    (1000) pascal    (1000)     1863 2022-11-05 00:14:14.000000 sysdm-0.8.65/setup.py
-drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2022-11-05 00:14:14.814686 sysdm-0.8.65/sysdm/
--rw-r--r--   0 pascal    (1000) pascal    (1000)      700 2022-11-05 00:14:14.000000 sysdm-0.8.65/sysdm/__init__.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)    10410 2022-08-12 15:48:19.000000 sysdm-0.8.65/sysdm/__main__.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     1396 2021-10-28 17:37:02.000000 sysdm-0.8.65/sysdm/file_watcher.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     1162 2021-03-05 13:45:09.000000 sysdm-0.8.65/sysdm/notify.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     9690 2022-11-05 00:13:44.000000 sysdm-0.8.65/sysdm/runner.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)    11824 2022-08-12 15:47:36.000000 sysdm-0.8.65/sysdm/sysctl.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     2293 2021-12-01 22:15:04.000000 sysdm-0.8.65/sysdm/utils.py
-drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2022-11-05 00:14:14.814686 sysdm-0.8.65/sysdm.egg-info/
--rw-r--r--   0 pascal    (1000) pascal    (1000)     3466 2022-11-05 00:14:14.000000 sysdm-0.8.65/sysdm.egg-info/PKG-INFO
--rw-r--r--   0 pascal    (1000) pascal    (1000)      392 2022-11-05 00:14:14.000000 sysdm-0.8.65/sysdm.egg-info/SOURCES.txt
--rw-r--r--   0 pascal    (1000) pascal    (1000)        1 2022-11-05 00:14:14.000000 sysdm-0.8.65/sysdm.egg-info/dependency_links.txt
--rw-r--r--   0 pascal    (1000) pascal    (1000)       47 2022-11-05 00:14:14.000000 sysdm-0.8.65/sysdm.egg-info/entry_points.txt
--rw-r--r--   0 pascal    (1000) pascal    (1000)        1 2019-03-29 16:19:53.000000 sysdm-0.8.65/sysdm.egg-info/not-zip-safe
--rw-r--r--   0 pascal    (1000) pascal    (1000)       36 2022-11-05 00:14:14.000000 sysdm-0.8.65/sysdm.egg-info/requires.txt
--rw-r--r--   0 pascal    (1000) pascal    (1000)        6 2022-11-05 00:14:14.000000 sysdm-0.8.65/sysdm.egg-info/top_level.txt
+drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2023-06-18 22:53:49.554941 sysdm-0.8.67/
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      182 2019-05-07 22:15:54.000000 sysdm-0.8.67/.gitignore
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     3466 2023-06-18 22:53:49.554941 sysdm-0.8.67/PKG-INFO
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     1764 2019-10-07 10:33:57.000000 sysdm-0.8.67/README.md
+-rw-r--r--   0 pascal    (1000) pascal    (1000)  4237450 2020-01-09 22:43:45.000000 sysdm-0.8.67/demo.gif
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      912 2019-03-29 17:35:00.000000 sysdm-0.8.67/deploy.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)    23405 2019-10-07 10:35:38.000000 sysdm-0.8.67/logo.png
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      137 2023-06-18 22:53:49.554941 sysdm-0.8.67/setup.cfg
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     1863 2023-06-18 22:53:49.000000 sysdm-0.8.67/setup.py
+drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2023-06-18 22:53:49.554941 sysdm-0.8.67/sysdm/
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      700 2023-06-18 22:53:49.000000 sysdm-0.8.67/sysdm/__init__.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)    10704 2023-01-29 21:14:09.000000 sysdm-0.8.67/sysdm/__main__.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     1396 2021-10-28 17:37:02.000000 sysdm-0.8.67/sysdm/file_watcher.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     1162 2021-03-05 13:45:09.000000 sysdm-0.8.67/sysdm/notify.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     9690 2022-11-05 00:13:44.000000 sysdm-0.8.67/sysdm/runner.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)    11824 2022-12-08 10:39:54.000000 sysdm-0.8.67/sysdm/sysctl.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     2293 2021-12-01 22:15:04.000000 sysdm-0.8.67/sysdm/utils.py
+drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2023-06-18 22:53:49.554941 sysdm-0.8.67/sysdm.egg-info/
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     3466 2023-06-18 22:53:49.000000 sysdm-0.8.67/sysdm.egg-info/PKG-INFO
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      392 2023-06-18 22:53:49.000000 sysdm-0.8.67/sysdm.egg-info/SOURCES.txt
+-rw-r--r--   0 pascal    (1000) pascal    (1000)        1 2023-06-18 22:53:49.000000 sysdm-0.8.67/sysdm.egg-info/dependency_links.txt
+-rw-r--r--   0 pascal    (1000) pascal    (1000)       47 2023-06-18 22:53:49.000000 sysdm-0.8.67/sysdm.egg-info/entry_points.txt
+-rw-r--r--   0 pascal    (1000) pascal    (1000)        1 2019-03-29 16:19:53.000000 sysdm-0.8.67/sysdm.egg-info/not-zip-safe
+-rw-r--r--   0 pascal    (1000) pascal    (1000)       36 2023-06-18 22:53:49.000000 sysdm-0.8.67/sysdm.egg-info/requires.txt
+-rw-r--r--   0 pascal    (1000) pascal    (1000)        6 2023-06-18 22:53:49.000000 sysdm-0.8.67/sysdm.egg-info/top_level.txt
```

### Comparing `sysdm-0.8.65/PKG-INFO` & `sysdm-0.8.67/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysdm
-Version: 0.8.65
+Version: 0.8.67
 Summary: Scripts as a service. Builds on systemd.
 Home-page: https://github.com/kootenpv/sysdm
 Author: Pascal van Kooten
 Author-email: kootenpv@gmail.com
 License: MIT
 Description: <p align="center">
           <img src="logo.png" width="300px"/>
```

### Comparing `sysdm-0.8.65/README.md` & `sysdm-0.8.67/README.md`

 * *Files identical despite different names*

### Comparing `sysdm-0.8.65/demo.gif` & `sysdm-0.8.67/demo.gif`

 * *Files identical despite different names*

### Comparing `sysdm-0.8.65/deploy.py` & `sysdm-0.8.67/deploy.py`

 * *Files identical despite different names*

### Comparing `sysdm-0.8.65/logo.png` & `sysdm-0.8.67/logo.png`

 * *Files identical despite different names*

### Comparing `sysdm-0.8.65/setup.py` & `sysdm-0.8.67/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 MAJOR_VERSION = "0"
 MINOR_VERSION = "8"
-MICRO_VERSION = "65"
+MICRO_VERSION = "67"
 VERSION = "{}.{}.{}".format(MAJOR_VERSION, MINOR_VERSION, MICRO_VERSION)
 
 with open("README.md") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name='sysdm',
```

### Comparing `sysdm-0.8.65/sysdm/__init__.py` & `sysdm-0.8.67/sysdm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 
 __project__ = "sysdm"
-__version__ = "0.8.65"
+__version__ = "0.8.67"
 __repo__ = "https://github.com/kootenpv/sysdm"
 
 
 def version():
     """ Prints the current version of rebrand, and more """
     sv = sys.version_info
     py_version = "{}.{}.{}".format(sv.major, sv.minor, sv.micro)
```

### Comparing `sysdm-0.8.65/sysdm/__main__.py` & `sysdm-0.8.67/sysdm/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,23 @@
             units = ls(self.systempath)
             unit = choose_unit(self.systempath, units)
             if unit is None:
                 sys.exit()
         show(self.systempath, unit)
 
     @cli
+    def stop_all(self):
+        """Interactively show units and allow viewing them"""
+        units = ls(self.systempath)
+        for unit in units:
+            if is_unit_running(unit):
+                print("Stopping unit", unit)
+                systemctl("stop {}".format(unit))
+
+    @cli
     def ls(self):
         """Interactively show units and allow viewing them"""
         while True:
             units = ls(self.systempath)
             if units:
                 unit = choose_unit(self.systempath, units)
                 if unit is None:
@@ -263,15 +272,15 @@
     quit = "-- Quit --"
     formatted_options.append(" ")
     formatted_options.append(quit)
     title = "These are known units:\n\n{}| Active  | On boot |   Port".format(" " * (offset + 2))
     default_index = 0
     while True:
         p = Picker(formatted_options, title, default_index=default_index)
-        p.register_custom_handler(ord("q"), lambda _: sys.exit(0))
+        # p.register_custom_handler(ord("q"), lambda _: sys.exit(0))
         chosen, index = p.start()
         if chosen == quit:
             return None
         elif chosen == " ":
             default_index = index
             continue
         else:
```

### Comparing `sysdm-0.8.65/sysdm/file_watcher.py` & `sysdm-0.8.67/sysdm/file_watcher.py`

 * *Files identical despite different names*

### Comparing `sysdm-0.8.65/sysdm/notify.py` & `sysdm-0.8.67/sysdm/notify.py`

 * *Files identical despite different names*

### Comparing `sysdm-0.8.65/sysdm/runner.py` & `sysdm-0.8.67/sysdm/runner.py`

 * *Files identical despite different names*

### Comparing `sysdm-0.8.65/sysdm/sysctl.py` & `sysdm-0.8.67/sysdm/sysctl.py`

 * *Files identical despite different names*

### Comparing `sysdm-0.8.65/sysdm/utils.py` & `sysdm-0.8.67/sysdm/utils.py`

 * *Files identical despite different names*

### Comparing `sysdm-0.8.65/sysdm.egg-info/PKG-INFO` & `sysdm-0.8.67/sysdm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysdm
-Version: 0.8.65
+Version: 0.8.67
 Summary: Scripts as a service. Builds on systemd.
 Home-page: https://github.com/kootenpv/sysdm
 Author: Pascal van Kooten
 Author-email: kootenpv@gmail.com
 License: MIT
 Description: <p align="center">
           <img src="logo.png" width="300px"/>
```

