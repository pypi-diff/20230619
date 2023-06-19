# Comparing `tmp/nw_connections-1.2.3.tar.gz` & `tmp/nw_connections-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nw_connections-1.2.3.tar", last modified: Wed Dec  1 12:27:35 2021, max compression
+gzip compressed data, was "nw_connections-1.2.4.tar", last modified: Mon Jun 19 14:08:50 2023, max compression
```

## Comparing `nw_connections-1.2.3.tar` & `nw_connections-1.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jens      (1001) jens      (1001)        0 2021-12-01 12:27:35.814507 nw_connections-1.2.3/
--rw-rw-r--   0 jens      (1001) jens      (1001)        6 2021-12-01 12:27:17.000000 nw_connections-1.2.3/CURRENT_VERSION.txt
--rw-rw-r--   0 jens      (1001) jens      (1001)       28 2021-11-18 14:50:20.000000 nw_connections-1.2.3/MANIFEST.in
--rw-rw-r--   0 jens      (1001) jens      (1001)      294 2021-12-01 12:27:35.814507 nw_connections-1.2.3/PKG-INFO
--rw-rw-r--   0 jens      (1001) jens      (1001)      506 2021-11-18 14:50:20.000000 nw_connections-1.2.3/README.md
-drwxrwxr-x   0 jens      (1001) jens      (1001)        0 2021-12-01 12:27:35.810506 nw_connections-1.2.3/nw_connections/
--rw-rw-r--   0 jens      (1001) jens      (1001)      281 2021-11-18 14:50:20.000000 nw_connections-1.2.3/nw_connections/__init__.py
--rw-rw-r--   0 jens      (1001) jens      (1001)    20949 2021-12-01 12:25:57.000000 nw_connections-1.2.3/nw_connections/connection.py
--rw-rw-r--   0 jens      (1001) jens      (1001)    10895 2021-11-24 14:13:11.000000 nw_connections-1.2.3/nw_connections/postgrest.py
--rw-rw-r--   0 jens      (1001) jens      (1001)     2955 2021-11-18 14:50:20.000000 nw_connections-1.2.3/nw_connections/robotwriter.py
--rw-rw-r--   0 jens      (1001) jens      (1001)      251 2021-11-18 14:50:20.000000 nw_connections-1.2.3/nw_connections/utils.py
-drwxrwxr-x   0 jens      (1001) jens      (1001)        0 2021-12-01 12:27:35.814507 nw_connections-1.2.3/nw_connections.egg-info/
--rwxrwxrwx   0 jens      (1001) jens      (1001)      294 2021-12-01 12:27:35.000000 nw_connections-1.2.3/nw_connections.egg-info/PKG-INFO
--rwxrwxrwx   0 jens      (1001) jens      (1001)      424 2021-12-01 12:27:35.000000 nw_connections-1.2.3/nw_connections.egg-info/SOURCES.txt
--rwxrwxrwx   0 jens      (1001) jens      (1001)        1 2021-12-01 12:27:35.000000 nw_connections-1.2.3/nw_connections.egg-info/dependency_links.txt
--rwxrwxrwx   0 jens      (1001) jens      (1001)        1 2019-10-07 20:14:36.000000 nw_connections-1.2.3/nw_connections.egg-info/not-zip-safe
--rwxrwxrwx   0 jens      (1001) jens      (1001)      100 2021-12-01 12:27:35.000000 nw_connections-1.2.3/nw_connections.egg-info/requires.txt
--rwxrwxrwx   0 jens      (1001) jens      (1001)       15 2021-12-01 12:27:35.000000 nw_connections-1.2.3/nw_connections.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1001) jens      (1001)       91 2021-12-01 12:27:35.814507 nw_connections-1.2.3/setup.cfg
--rw-rw-r--   0 jens      (1001) jens      (1001)      707 2021-11-18 14:50:20.000000 nw_connections-1.2.3/setup.py
+drwxrwxr-x   0 jens      (1001) jens      (1001)        0 2023-06-19 14:08:50.911127 nw_connections-1.2.4/
+-rw-rw-r--   0 jens      (1001) jens      (1001)        6 2023-06-19 14:08:10.000000 nw_connections-1.2.4/CURRENT_VERSION.txt
+-rw-rw-r--   0 jens      (1001) jens      (1001)       28 2021-11-18 14:50:20.000000 nw_connections-1.2.4/MANIFEST.in
+-rw-rw-r--   0 jens      (1001) jens      (1001)      294 2023-06-19 14:08:50.911127 nw_connections-1.2.4/PKG-INFO
+-rw-rw-r--   0 jens      (1001) jens      (1001)      506 2021-11-18 14:50:20.000000 nw_connections-1.2.4/README.md
+drwxrwxr-x   0 jens      (1001) jens      (1001)        0 2023-06-19 14:08:50.911127 nw_connections-1.2.4/nw_connections/
+-rw-rw-r--   0 jens      (1001) jens      (1001)      281 2021-11-18 14:50:20.000000 nw_connections-1.2.4/nw_connections/__init__.py
+-rw-rw-r--   0 jens      (1001) jens      (1001)    20949 2023-06-19 14:02:58.000000 nw_connections-1.2.4/nw_connections/connection.py
+-rw-rw-r--   0 jens      (1001) jens      (1001)    10895 2023-06-19 13:36:33.000000 nw_connections-1.2.4/nw_connections/postgrest.py
+-rw-rw-r--   0 jens      (1001) jens      (1001)     2955 2021-11-18 14:50:20.000000 nw_connections-1.2.4/nw_connections/robotwriter.py
+-rw-rw-r--   0 jens      (1001) jens      (1001)      183 2023-06-19 13:35:56.000000 nw_connections-1.2.4/nw_connections/utils.py
+drwxrwxr-x   0 jens      (1001) jens      (1001)        0 2023-06-19 14:08:50.911127 nw_connections-1.2.4/nw_connections.egg-info/
+-rwxrwxrwx   0 jens      (1001) jens      (1001)      294 2023-06-19 14:08:50.000000 nw_connections-1.2.4/nw_connections.egg-info/PKG-INFO
+-rwxrwxrwx   0 jens      (1001) jens      (1001)      424 2023-06-19 14:08:50.000000 nw_connections-1.2.4/nw_connections.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jens      (1001) jens      (1001)        1 2023-06-19 14:08:50.000000 nw_connections-1.2.4/nw_connections.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jens      (1001) jens      (1001)        1 2019-10-07 20:14:36.000000 nw_connections-1.2.4/nw_connections.egg-info/not-zip-safe
+-rwxrwxrwx   0 jens      (1001) jens      (1001)       98 2023-06-19 14:08:50.000000 nw_connections-1.2.4/nw_connections.egg-info/requires.txt
+-rwxrwxrwx   0 jens      (1001) jens      (1001)       15 2023-06-19 14:08:50.000000 nw_connections-1.2.4/nw_connections.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1001) jens      (1001)       91 2023-06-19 14:08:50.915127 nw_connections-1.2.4/setup.cfg
+-rw-rw-r--   0 jens      (1001) jens      (1001)      705 2023-06-19 11:25:15.000000 nw_connections-1.2.4/setup.py
```

### Comparing `nw_connections-1.2.3/nw_connections/connection.py` & `nw_connections-1.2.4/nw_connections/connection.py`

 * *Files identical despite different names*

### Comparing `nw_connections-1.2.3/nw_connections/postgrest.py` & `nw_connections-1.2.4/nw_connections/postgrest.py`

 * *Files identical despite different names*

### Comparing `nw_connections-1.2.3/nw_connections/robotwriter.py` & `nw_connections-1.2.4/nw_connections/robotwriter.py`

 * *Files identical despite different names*

### Comparing `nw_connections-1.2.3/setup.py` & `nw_connections-1.2.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 required = [
     'boto3>=1.9',
     'requests>=2,<3',
-    'requests-cache>=0.4,<1',
+    'requests-cache>=1,<2',
     'PyJWT>=1.7.1,<2',
     'requests-jwt>=0.4,<1',
     'simplejson>=3',
 ]
 
 # Get current version
 with open("CURRENT_VERSION.txt") as f:
```

