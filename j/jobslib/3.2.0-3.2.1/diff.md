# Comparing `tmp/jobslib-3.2.0.tar.gz` & `tmp/jobslib-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobslib-3.2.0.tar", last modified: Tue Oct  4 12:31:02 2022, max compression
+gzip compressed data, was "jobslib-3.2.1.tar", last modified: Mon Jun 19 13:26:25 2023, max compression
```

## Comparing `jobslib-3.2.0.tar` & `jobslib-3.2.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 seifert   (1000) seifert   (1000)        0 2022-10-04 12:31:02.743712 jobslib-3.2.0/
--rw-r--r--   0 seifert   (1000) seifert   (1000)     4203 2022-10-04 12:01:30.000000 jobslib-3.2.0/CHANGELOG.md
--rw-r--r--   0 seifert   (1000) seifert   (1000)     1508 2022-10-04 12:01:30.000000 jobslib-3.2.0/LICENSE
--rw-r--r--   0 seifert   (1000) seifert   (1000)       37 2022-10-04 12:01:30.000000 jobslib-3.2.0/MANIFEST.in
--rw-r--r--   0 seifert   (1000) seifert   (1000)     3355 2022-10-04 12:31:02.743712 jobslib-3.2.0/PKG-INFO
--rw-r--r--   0 seifert   (1000) seifert   (1000)     2557 2022-10-04 12:01:30.000000 jobslib-3.2.0/README.rst
-drwxr-xr-x   0 seifert   (1000) seifert   (1000)        0 2022-10-04 12:31:02.740379 jobslib-3.2.0/example/
--rw-r--r--   0 seifert   (1000) seifert   (1000)        0 2022-10-04 12:01:30.000000 jobslib-3.2.0/example/__init__.py
--rw-r--r--   0 seifert   (1000) seifert   (1000)      943 2022-10-04 12:01:30.000000 jobslib-3.2.0/example/helloworld.py
--rw-r--r--   0 seifert   (1000) seifert   (1000)     1202 2022-10-04 12:01:30.000000 jobslib-3.2.0/example/oneinstance.py
-drwxr-xr-x   0 seifert   (1000) seifert   (1000)        0 2022-10-04 12:31:02.740379 jobslib-3.2.0/jobslib/
--rw-r--r--   0 seifert   (1000) seifert   (1000)      462 2022-10-04 12:01:30.000000 jobslib-3.2.0/jobslib/__init__.py
--rw-r--r--   0 seifert   (1000) seifert   (1000)      871 2022-10-04 12:01:30.000000 jobslib-3.2.0/jobslib/cmdlineparser.py
--rw-r--r--   0 seifert   (1000) seifert   (1000)    12343 2022-10-04 12:01:30.000000 jobslib-3.2.0/jobslib/config.py
--rw-r--r--   0 seifert   (1000) seifert   (1000)     2750 2022-10-04 12:01:30.000000 jobslib-3.2.0/jobslib/context.py
--rw-r--r--   0 seifert   (1000) seifert   (1000)      385 2022-10-04 12:01:30.000000 jobslib-3.2.0/jobslib/exceptions.py
--rw-r--r--   0 seifert   (1000) seifert   (1000)      608 2022-10-04 12:01:30.000000 jobslib-3.2.0/jobslib/imports.py
-drwxr-xr-x   0 seifert   (1000) seifert   (1000)        0 2022-10-04 12:31:02.743712 jobslib-3.2.0/jobslib/liveness/
--rw-r--r--   0 seifert   (1000) seifert   (1000)     3071 2022-10-04 12:01:30.000000 jobslib-3.2.0/jobslib/liveness/__init__.py
--rw-r--r--   0 seifert   (1000) seifert   (1000)     4531 2022-10-04 12:01:30.000000 jobslib-3.2.0/jobslib/liveness/consul.py
--rw-r--r--   0 seifert   (1000) seifert   (1000)      612 2022-10-04 12:01:30.000000 jobslib-3.2.0/jobslib/liveness/dummy.py
--rw-r--r--   0 seifert   (1000) seifert   (1000)      680 2022-10-04 12:01:30.000000 jobslib-3.2.0/jobslib/logging.py
--rw-r--r--   0 seifert   (1000) seifert   (1000)     5085 2022-10-04 12:01:30.000000 jobslib-3.2.0/jobslib/main.py
-drwxr-xr-x   0 seifert   (1000) seifert   (1000)        0 2022-10-04 12:31:02.743712 jobslib-3.2.0/jobslib/metrics/
--rw-r--r--   0 seifert   (1000) seifert   (1000)     1396 2022-10-04 12:01:30.000000 jobslib-3.2.0/jobslib/metrics/__init__.py
--rw-r--r--   0 seifert   (1000) seifert   (1000)      555 2022-10-04 12:01:30.000000 jobslib-3.2.0/jobslib/metrics/dummy.py
--rw-r--r--   0 seifert   (1000) seifert   (1000)     4724 2022-10-04 12:01:30.000000 jobslib-3.2.0/jobslib/metrics/influxdb.py
-drwxr-xr-x   0 seifert   (1000) seifert   (1000)        0 2022-10-04 12:31:02.743712 jobslib-3.2.0/jobslib/oneinstance/
--rw-r--r--   0 seifert   (1000) seifert   (1000)     2446 2022-10-04 12:01:30.000000 jobslib-3.2.0/jobslib/oneinstance/__init__.py
--rw-r--r--   0 seifert   (1000) seifert   (1000)    11057 2022-10-04 12:01:30.000000 jobslib-3.2.0/jobslib/oneinstance/consul.py
--rw-r--r--   0 seifert   (1000) seifert   (1000)      714 2022-10-04 12:01:30.000000 jobslib-3.2.0/jobslib/oneinstance/dummy.py
--rw-r--r--   0 seifert   (1000) seifert   (1000)     8649 2022-10-04 12:01:30.000000 jobslib-3.2.0/jobslib/tasks.py
--rw-r--r--   0 seifert   (1000) seifert   (1000)      709 2022-10-04 12:01:30.000000 jobslib-3.2.0/jobslib/time.py
--rw-r--r--   0 seifert   (1000) seifert   (1000)       19 2022-10-04 12:01:30.000000 jobslib-3.2.0/jobslib/version.py
-drwxr-xr-x   0 seifert   (1000) seifert   (1000)        0 2022-10-04 12:31:02.743712 jobslib-3.2.0/jobslib.egg-info/
--rw-r--r--   0 seifert   (1000) seifert   (1000)     3355 2022-10-04 12:31:02.000000 jobslib-3.2.0/jobslib.egg-info/PKG-INFO
--rw-r--r--   0 seifert   (1000) seifert   (1000)      872 2022-10-04 12:31:02.000000 jobslib-3.2.0/jobslib.egg-info/SOURCES.txt
--rw-r--r--   0 seifert   (1000) seifert   (1000)        1 2022-10-04 12:31:02.000000 jobslib-3.2.0/jobslib.egg-info/dependency_links.txt
--rw-r--r--   0 seifert   (1000) seifert   (1000)       45 2022-10-04 12:31:02.000000 jobslib-3.2.0/jobslib.egg-info/entry_points.txt
--rw-r--r--   0 seifert   (1000) seifert   (1000)       73 2022-10-04 12:31:02.000000 jobslib-3.2.0/jobslib.egg-info/requires.txt
--rw-r--r--   0 seifert   (1000) seifert   (1000)       22 2022-10-04 12:31:02.000000 jobslib-3.2.0/jobslib.egg-info/top_level.txt
--rw-r--r--   0 seifert   (1000) seifert   (1000)        1 2022-10-04 12:02:11.000000 jobslib-3.2.0/jobslib.egg-info/zip-safe
--rw-r--r--   0 seifert   (1000) seifert   (1000)      385 2022-10-04 12:31:02.743712 jobslib-3.2.0/setup.cfg
--rw-r--r--   0 seifert   (1000) seifert   (1000)     1678 2022-10-04 12:12:08.000000 jobslib-3.2.0/setup.py
-drwxr-xr-x   0 seifert   (1000) seifert   (1000)        0 2022-10-04 12:31:02.743712 jobslib-3.2.0/tests/
--rw-r--r--   0 seifert   (1000) seifert   (1000)        0 2022-10-04 12:01:30.000000 jobslib-3.2.0/tests/__init__.py
--rw-r--r--   0 seifert   (1000) seifert   (1000)      990 2022-10-04 12:01:30.000000 jobslib-3.2.0/tests/test_cmdlineparser.py
--rw-r--r--   0 seifert   (1000) seifert   (1000)     4237 2022-10-04 12:01:30.000000 jobslib-3.2.0/tests/test_config.py
+drwxr-xr-x   0 seifert   (1000) seifert   (1000)        0 2023-06-19 13:26:25.355636 jobslib-3.2.1/
+-rw-r--r--   0 seifert   (1000) seifert   (1000)     4320 2023-06-19 13:19:23.000000 jobslib-3.2.1/CHANGELOG.md
+-rw-r--r--   0 seifert   (1000) seifert   (1000)     1508 2023-06-19 12:56:56.000000 jobslib-3.2.1/LICENSE
+-rw-r--r--   0 seifert   (1000) seifert   (1000)       37 2023-06-19 12:56:56.000000 jobslib-3.2.1/MANIFEST.in
+-rw-r--r--   0 seifert   (1000) seifert   (1000)     3355 2023-06-19 13:26:25.355636 jobslib-3.2.1/PKG-INFO
+-rw-r--r--   0 seifert   (1000) seifert   (1000)     2557 2023-06-19 12:56:56.000000 jobslib-3.2.1/README.rst
+drwxr-xr-x   0 seifert   (1000) seifert   (1000)        0 2023-06-19 13:26:25.352302 jobslib-3.2.1/example/
+-rw-r--r--   0 seifert   (1000) seifert   (1000)        0 2023-06-19 12:56:56.000000 jobslib-3.2.1/example/__init__.py
+-rw-r--r--   0 seifert   (1000) seifert   (1000)      943 2023-06-19 12:56:56.000000 jobslib-3.2.1/example/helloworld.py
+-rw-r--r--   0 seifert   (1000) seifert   (1000)     1202 2023-06-19 12:56:56.000000 jobslib-3.2.1/example/oneinstance.py
+drwxr-xr-x   0 seifert   (1000) seifert   (1000)        0 2023-06-19 13:26:25.355636 jobslib-3.2.1/jobslib/
+-rw-r--r--   0 seifert   (1000) seifert   (1000)      462 2023-06-19 12:56:56.000000 jobslib-3.2.1/jobslib/__init__.py
+-rw-r--r--   0 seifert   (1000) seifert   (1000)      956 2023-06-19 13:15:42.000000 jobslib-3.2.1/jobslib/cmdlineparser.py
+-rw-r--r--   0 seifert   (1000) seifert   (1000)    12343 2023-06-19 12:56:56.000000 jobslib-3.2.1/jobslib/config.py
+-rw-r--r--   0 seifert   (1000) seifert   (1000)     2750 2023-06-19 12:56:56.000000 jobslib-3.2.1/jobslib/context.py
+-rw-r--r--   0 seifert   (1000) seifert   (1000)      385 2023-06-19 12:56:56.000000 jobslib-3.2.1/jobslib/exceptions.py
+-rw-r--r--   0 seifert   (1000) seifert   (1000)      608 2023-06-19 12:56:56.000000 jobslib-3.2.1/jobslib/imports.py
+drwxr-xr-x   0 seifert   (1000) seifert   (1000)        0 2023-06-19 13:26:25.355636 jobslib-3.2.1/jobslib/liveness/
+-rw-r--r--   0 seifert   (1000) seifert   (1000)     3071 2023-06-19 12:56:56.000000 jobslib-3.2.1/jobslib/liveness/__init__.py
+-rw-r--r--   0 seifert   (1000) seifert   (1000)     4531 2023-06-19 12:56:56.000000 jobslib-3.2.1/jobslib/liveness/consul.py
+-rw-r--r--   0 seifert   (1000) seifert   (1000)      612 2023-06-19 12:56:56.000000 jobslib-3.2.1/jobslib/liveness/dummy.py
+-rw-r--r--   0 seifert   (1000) seifert   (1000)      680 2023-06-19 12:56:56.000000 jobslib-3.2.1/jobslib/logging.py
+-rw-r--r--   0 seifert   (1000) seifert   (1000)     5085 2023-06-19 12:56:56.000000 jobslib-3.2.1/jobslib/main.py
+drwxr-xr-x   0 seifert   (1000) seifert   (1000)        0 2023-06-19 13:26:25.355636 jobslib-3.2.1/jobslib/metrics/
+-rw-r--r--   0 seifert   (1000) seifert   (1000)     1396 2023-06-19 12:56:56.000000 jobslib-3.2.1/jobslib/metrics/__init__.py
+-rw-r--r--   0 seifert   (1000) seifert   (1000)      555 2023-06-19 12:56:56.000000 jobslib-3.2.1/jobslib/metrics/dummy.py
+-rw-r--r--   0 seifert   (1000) seifert   (1000)     4724 2023-06-19 12:56:56.000000 jobslib-3.2.1/jobslib/metrics/influxdb.py
+drwxr-xr-x   0 seifert   (1000) seifert   (1000)        0 2023-06-19 13:26:25.355636 jobslib-3.2.1/jobslib/oneinstance/
+-rw-r--r--   0 seifert   (1000) seifert   (1000)     2446 2023-06-19 12:56:56.000000 jobslib-3.2.1/jobslib/oneinstance/__init__.py
+-rw-r--r--   0 seifert   (1000) seifert   (1000)    11057 2023-06-19 12:56:56.000000 jobslib-3.2.1/jobslib/oneinstance/consul.py
+-rw-r--r--   0 seifert   (1000) seifert   (1000)      714 2023-06-19 12:56:56.000000 jobslib-3.2.1/jobslib/oneinstance/dummy.py
+-rw-r--r--   0 seifert   (1000) seifert   (1000)     8649 2023-06-19 12:56:56.000000 jobslib-3.2.1/jobslib/tasks.py
+-rw-r--r--   0 seifert   (1000) seifert   (1000)      709 2023-06-19 12:56:56.000000 jobslib-3.2.1/jobslib/time.py
+-rw-r--r--   0 seifert   (1000) seifert   (1000)       19 2023-06-19 13:19:36.000000 jobslib-3.2.1/jobslib/version.py
+drwxr-xr-x   0 seifert   (1000) seifert   (1000)        0 2023-06-19 13:26:25.355636 jobslib-3.2.1/jobslib.egg-info/
+-rw-r--r--   0 seifert   (1000) seifert   (1000)     3355 2023-06-19 13:26:25.000000 jobslib-3.2.1/jobslib.egg-info/PKG-INFO
+-rw-r--r--   0 seifert   (1000) seifert   (1000)      872 2023-06-19 13:26:25.000000 jobslib-3.2.1/jobslib.egg-info/SOURCES.txt
+-rw-r--r--   0 seifert   (1000) seifert   (1000)        1 2023-06-19 13:26:25.000000 jobslib-3.2.1/jobslib.egg-info/dependency_links.txt
+-rw-r--r--   0 seifert   (1000) seifert   (1000)       45 2023-06-19 13:26:25.000000 jobslib-3.2.1/jobslib.egg-info/entry_points.txt
+-rw-r--r--   0 seifert   (1000) seifert   (1000)       73 2023-06-19 13:26:25.000000 jobslib-3.2.1/jobslib.egg-info/requires.txt
+-rw-r--r--   0 seifert   (1000) seifert   (1000)       22 2023-06-19 13:26:25.000000 jobslib-3.2.1/jobslib.egg-info/top_level.txt
+-rw-r--r--   0 seifert   (1000) seifert   (1000)        1 2023-06-19 12:57:06.000000 jobslib-3.2.1/jobslib.egg-info/zip-safe
+-rw-r--r--   0 seifert   (1000) seifert   (1000)      385 2023-06-19 13:26:25.358969 jobslib-3.2.1/setup.cfg
+-rw-r--r--   0 seifert   (1000) seifert   (1000)     1678 2023-06-19 12:56:56.000000 jobslib-3.2.1/setup.py
+drwxr-xr-x   0 seifert   (1000) seifert   (1000)        0 2023-06-19 13:26:25.355636 jobslib-3.2.1/tests/
+-rw-r--r--   0 seifert   (1000) seifert   (1000)        0 2023-06-19 12:56:56.000000 jobslib-3.2.1/tests/__init__.py
+-rw-r--r--   0 seifert   (1000) seifert   (1000)     1073 2023-06-19 13:17:15.000000 jobslib-3.2.1/tests/test_cmdlineparser.py
+-rw-r--r--   0 seifert   (1000) seifert   (1000)     4237 2023-06-19 12:56:56.000000 jobslib-3.2.1/tests/test_config.py
```

### Comparing `jobslib-3.2.0/CHANGELOG.md` & `jobslib-3.2.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Jobslib
 
+## [3.2.1] - 2023-06-19 15:18 - Jan Seifert <jan.seifert@firma.seznam.cz>
+### Added
+- fix colored 1.5 compatibility
+
 ## [3.2.0] - 2022-09-05 09:33 - Ondrej Voves <ondrej.voves@firma.seznam.cz>
 ### Added
 - Option to release lock on error (DOP-7864)
 
 ## [3.1.0] - 2020-08-26 09:33 - Jan Seifert <jan.seifert@firma.seznam.cz>
 ### Added
 - retry when liveness/metrics/oneinstance failed
```

### Comparing `jobslib-3.2.0/LICENSE` & `jobslib-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/PKG-INFO` & `jobslib-3.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobslib
-Version: 3.2.0
+Version: 3.2.1
 Summary: Library for launching tasks in parallel environment
 Home-page: https://github.com/seznam/jobslib.git
 Author: Seznam.cz a.s.
 Author-email: doporucovani-vyvoj@firma.seznam.cz
 License: BSD
 Project-URL: Documentation, https://seznam.github.io/jobslib/
 Platform: any
```

### Comparing `jobslib-3.2.0/README.rst` & `jobslib-3.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/example/helloworld.py` & `jobslib-3.2.1/example/helloworld.py`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/example/oneinstance.py` & `jobslib-3.2.1/example/oneinstance.py`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/jobslib/cmdlineparser.py` & `jobslib-3.2.1/jobslib/cmdlineparser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 Command line parser helpers.
 """
 
 import argparse
 import sys
 
-from colored import fg, attr
+try:
+    from colored import fg as fore, attr as style
+except ImportError:
+    from colored import fore, style
 
 __all__ = ['argument']
 
 
 def argument(*args, **kwargs):
     """
     Define how a single command-line argument should be parsed.
@@ -29,8 +32,8 @@
         """
         Print on **stderr** error message from command line parser and
         exit process.
         """
         self.print_help(sys.stderr)
         self.exit(
             2, '\n{:s}{:s}: error: {}{:s}\n'.format(
-                fg('red'), self.prog, message, attr('reset')))
+                fore('red'), self.prog, message, style('reset')))
```

### Comparing `jobslib-3.2.0/jobslib/config.py` & `jobslib-3.2.1/jobslib/config.py`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/jobslib/context.py` & `jobslib-3.2.1/jobslib/context.py`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/jobslib/imports.py` & `jobslib-3.2.1/jobslib/imports.py`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/jobslib/liveness/__init__.py` & `jobslib-3.2.1/jobslib/liveness/__init__.py`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/jobslib/liveness/consul.py` & `jobslib-3.2.1/jobslib/liveness/consul.py`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/jobslib/liveness/dummy.py` & `jobslib-3.2.1/jobslib/liveness/dummy.py`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/jobslib/logging.py` & `jobslib-3.2.1/jobslib/logging.py`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/jobslib/main.py` & `jobslib-3.2.1/jobslib/main.py`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/jobslib/metrics/__init__.py` & `jobslib-3.2.1/jobslib/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/jobslib/metrics/dummy.py` & `jobslib-3.2.1/jobslib/metrics/dummy.py`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/jobslib/metrics/influxdb.py` & `jobslib-3.2.1/jobslib/metrics/influxdb.py`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/jobslib/oneinstance/__init__.py` & `jobslib-3.2.1/jobslib/oneinstance/__init__.py`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/jobslib/oneinstance/consul.py` & `jobslib-3.2.1/jobslib/oneinstance/consul.py`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/jobslib/oneinstance/dummy.py` & `jobslib-3.2.1/jobslib/oneinstance/dummy.py`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/jobslib/tasks.py` & `jobslib-3.2.1/jobslib/tasks.py`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/jobslib/time.py` & `jobslib-3.2.1/jobslib/time.py`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/jobslib.egg-info/PKG-INFO` & `jobslib-3.2.1/jobslib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobslib
-Version: 3.2.0
+Version: 3.2.1
 Summary: Library for launching tasks in parallel environment
 Home-page: https://github.com/seznam/jobslib.git
 Author: Seznam.cz a.s.
 Author-email: doporucovani-vyvoj@firma.seznam.cz
 License: BSD
 Project-URL: Documentation, https://seznam.github.io/jobslib/
 Platform: any
```

### Comparing `jobslib-3.2.0/jobslib.egg-info/SOURCES.txt` & `jobslib-3.2.1/jobslib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/setup.py` & `jobslib-3.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `jobslib-3.2.0/tests/test_cmdlineparser.py` & `jobslib-3.2.1/tests/test_cmdlineparser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 
 import sys
 
 from unittest import mock
 
-import colored
 import pytest
+try:
+    from colored import fg as fore, attr as style
+except ImportError:
+    from colored import fore, style
 
 from jobslib.cmdlineparser import argument, ArgumentParser
 
 
 @pytest.mark.parametrize(
     'args, kwargs, expected',
     [
@@ -25,11 +28,11 @@
 def test_argument_parser():
     parser = ArgumentParser()
     parser.prog = 'foo'
     with mock.patch.object(parser, 'print_help') as m_print_help:
         with mock.patch.object(parser, 'exit') as m_exit:
             parser.error('something is wrong')
     expected_message = (
-        '\n' + colored.fg('red') + 'foo: error: something is wrong' +
-        colored.attr('reset') + '\n')
+        '\n' + fore('red') + 'foo: error: something is wrong' +
+        style('reset') + '\n')
     m_print_help.assert_called_once_with(sys.stderr)
     m_exit.assert_called_once_with(2, expected_message)
```

### Comparing `jobslib-3.2.0/tests/test_config.py` & `jobslib-3.2.1/tests/test_config.py`

 * *Files identical despite different names*

