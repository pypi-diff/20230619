# Comparing `tmp/foxglove-web-0.0.8.tar.gz` & `tmp/foxglove-web-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/foxglove-web-0.0.8.tar", last modified: Thu Sep 17 11:59:54 2020, max compression
+gzip compressed data, was "dist/foxglove-web-0.0.9.tar", last modified: Tue Sep 29 16:45:37 2020, max compression
```

## Comparing `foxglove-web-0.0.8.tar` & `foxglove-web-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-17 11:59:54.878828 foxglove-web-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)      990 2020-09-17 11:59:54.878828 foxglove-web-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       27 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-17 11:59:54.874828 foxglove-web-0.0.8/foxglove/
--rw-r--r--   0 runner    (1001) docker     (116)      211 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/foxglove/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       59 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/foxglove/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)       59 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/foxglove/asgi.py
--rw-r--r--   0 runner    (1001) docker     (116)     7570 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/foxglove/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-17 11:59:54.874828 foxglove-web-0.0.8/foxglove/db/
--rw-r--r--   0 runner    (1001) docker     (116)       72 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/foxglove/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4852 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/foxglove/db/helpers.py
--rw-r--r--   0 runner    (1001) docker     (116)     4859 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/foxglove/db/main.py
--rw-r--r--   0 runner    (1001) docker     (116)      836 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/foxglove/db/middleware.py
--rw-r--r--   0 runner    (1001) docker     (116)     4080 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/foxglove/db/patches.py
--rw-r--r--   0 runner    (1001) docker     (116)     1828 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/foxglove/devtools.py
--rw-r--r--   0 runner    (1001) docker     (116)     2799 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/foxglove/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     4904 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/foxglove/logs.py
--rw-r--r--   0 runner    (1001) docker     (116)     2620 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/foxglove/main.py
--rw-r--r--   0 runner    (1001) docker     (116)     7347 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/foxglove/middleware.py
--rw-r--r--   0 runner    (1001) docker     (116)      655 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/foxglove/redis.py
--rw-r--r--   0 runner    (1001) docker     (116)     5003 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/foxglove/settings.py
--rw-r--r--   0 runner    (1001) docker     (116)     3890 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/foxglove/templates.py
--rw-r--r--   0 runner    (1001) docker     (116)     3812 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/foxglove/test_server.py
--rw-r--r--   0 runner    (1001) docker     (116)     1102 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/foxglove/testing.py
--rw-r--r--   0 runner    (1001) docker     (116)      321 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/foxglove/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)       41 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/foxglove/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-17 11:59:54.878828 foxglove-web-0.0.8/foxglove_web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      990 2020-09-17 11:59:54.000000 foxglove-web-0.0.8/foxglove_web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      712 2020-09-17 11:59:54.000000 foxglove-web-0.0.8/foxglove_web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-09-17 11:59:54.000000 foxglove-web-0.0.8/foxglove_web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       70 2020-09-17 11:59:54.000000 foxglove-web-0.0.8/foxglove_web.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      213 2020-09-17 11:59:54.000000 foxglove-web-0.0.8/foxglove_web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2020-09-17 11:59:54.000000 foxglove-web-0.0.8/foxglove_web.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-09-17 11:59:53.000000 foxglove-web-0.0.8/foxglove_web.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)     1055 2020-09-17 11:59:54.878828 foxglove-web-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1973 2020-09-17 11:59:26.000000 foxglove-web-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-29 16:45:37.745326 foxglove-web-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)      990 2020-09-29 16:45:37.745326 foxglove-web-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)       27 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-29 16:45:37.741325 foxglove-web-0.0.9/foxglove/
+-rw-r--r--   0 runner    (1001) docker     (116)      211 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       59 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       59 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7570 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-29 16:45:37.741325 foxglove-web-0.0.9/foxglove/db/
+-rw-r--r--   0 runner    (1001) docker     (116)       72 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4852 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/db/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4859 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/db/main.py
+-rw-r--r--   0 runner    (1001) docker     (116)      836 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/db/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4080 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/db/patches.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1828 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/devtools.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2799 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4904 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/logs.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2620 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/main.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11388 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (116)      655 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/redis.py
+-rw-r--r--   0 runner    (1001) docker     (116)      819 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/route_class.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5003 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/settings.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3890 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/templates.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3812 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1102 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/testing.py
+-rw-r--r--   0 runner    (1001) docker     (116)      321 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)       41 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/foxglove/version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-29 16:45:37.745326 foxglove-web-0.0.9/foxglove_web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      990 2020-09-29 16:45:37.000000 foxglove-web-0.0.9/foxglove_web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      736 2020-09-29 16:45:37.000000 foxglove-web-0.0.9/foxglove_web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-09-29 16:45:37.000000 foxglove-web-0.0.9/foxglove_web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       70 2020-09-29 16:45:37.000000 foxglove-web-0.0.9/foxglove_web.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      213 2020-09-29 16:45:37.000000 foxglove-web-0.0.9/foxglove_web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        9 2020-09-29 16:45:37.000000 foxglove-web-0.0.9/foxglove_web.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-09-29 16:45:35.000000 foxglove-web-0.0.9/foxglove_web.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)     1055 2020-09-29 16:45:37.745326 foxglove-web-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1973 2020-09-29 16:45:07.000000 foxglove-web-0.0.9/setup.py
```

### Comparing `foxglove-web-0.0.8/PKG-INFO` & `foxglove-web-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-web
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools for Starlette
 Home-page: https://github.com/samuelcolvin/foxglove
 Author: Samuel Colvin
 Author-email: s@muelcolvin.com
 License: MIT
 Description: # foxglove
```

### Comparing `foxglove-web-0.0.8/foxglove/cli.py` & `foxglove-web-0.0.9/foxglove/cli.py`

 * *Files identical despite different names*

### Comparing `foxglove-web-0.0.8/foxglove/db/helpers.py` & `foxglove-web-0.0.9/foxglove/db/helpers.py`

 * *Files identical despite different names*

### Comparing `foxglove-web-0.0.8/foxglove/db/main.py` & `foxglove-web-0.0.9/foxglove/db/main.py`

 * *Files identical despite different names*

### Comparing `foxglove-web-0.0.8/foxglove/db/middleware.py` & `foxglove-web-0.0.9/foxglove/db/middleware.py`

 * *Files identical despite different names*

### Comparing `foxglove-web-0.0.8/foxglove/db/patches.py` & `foxglove-web-0.0.9/foxglove/db/patches.py`

 * *Files identical despite different names*

### Comparing `foxglove-web-0.0.8/foxglove/devtools.py` & `foxglove-web-0.0.9/foxglove/devtools.py`

 * *Files identical despite different names*

### Comparing `foxglove-web-0.0.8/foxglove/exceptions.py` & `foxglove-web-0.0.9/foxglove/exceptions.py`

 * *Files identical despite different names*

### Comparing `foxglove-web-0.0.8/foxglove/logs.py` & `foxglove-web-0.0.9/foxglove/logs.py`

 * *Files identical despite different names*

### Comparing `foxglove-web-0.0.8/foxglove/main.py` & `foxglove-web-0.0.9/foxglove/main.py`

 * *Files identical despite different names*

### Comparing `foxglove-web-0.0.8/foxglove/redis.py` & `foxglove-web-0.0.9/foxglove/redis.py`

 * *Files identical despite different names*

### Comparing `foxglove-web-0.0.8/foxglove/settings.py` & `foxglove-web-0.0.9/foxglove/settings.py`

 * *Files identical despite different names*

### Comparing `foxglove-web-0.0.8/foxglove/templates.py` & `foxglove-web-0.0.9/foxglove/templates.py`

 * *Files identical despite different names*

### Comparing `foxglove-web-0.0.8/foxglove/test_server.py` & `foxglove-web-0.0.9/foxglove/test_server.py`

 * *Files identical despite different names*

### Comparing `foxglove-web-0.0.8/foxglove/testing.py` & `foxglove-web-0.0.9/foxglove/testing.py`

 * *Files identical despite different names*

### Comparing `foxglove-web-0.0.8/foxglove_web.egg-info/PKG-INFO` & `foxglove-web-0.0.9/foxglove_web.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-web
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools for Starlette
 Home-page: https://github.com/samuelcolvin/foxglove
 Author: Samuel Colvin
 Author-email: s@muelcolvin.com
 License: MIT
 Description: # foxglove
```

### Comparing `foxglove-web-0.0.8/foxglove_web.egg-info/SOURCES.txt` & `foxglove-web-0.0.9/foxglove_web.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 foxglove/cli.py
 foxglove/devtools.py
 foxglove/exceptions.py
 foxglove/logs.py
 foxglove/main.py
 foxglove/middleware.py
 foxglove/redis.py
+foxglove/route_class.py
 foxglove/settings.py
 foxglove/templates.py
 foxglove/test_server.py
 foxglove/testing.py
 foxglove/utils.py
 foxglove/version.py
 foxglove/db/__init__.py
```

### Comparing `foxglove-web-0.0.8/setup.cfg` & `foxglove-web-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `foxglove-web-0.0.8/setup.py` & `foxglove-web-0.0.9/setup.py`

 * *Files identical despite different names*

