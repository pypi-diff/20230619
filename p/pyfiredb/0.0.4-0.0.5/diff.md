# Comparing `tmp/pyfiredb-0.0.4.tar.gz` & `tmp/pyfiredb-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfiredb-0.0.4.tar", last modified: Sun Jun 18 04:15:20 2023, max compression
+gzip compressed data, was "pyfiredb-0.0.5.tar", last modified: Mon Jun 19 03:14:55 2023, max compression
```

## Comparing `pyfiredb-0.0.4.tar` & `pyfiredb-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-18 04:15:20.143664 pyfiredb-0.0.4/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1084 2023-03-09 17:21:54.000000 pyfiredb-0.0.4/LICENSE.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)     1970 2023-06-18 04:15:20.139664 pyfiredb-0.0.4/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)     1295 2023-06-09 02:20:03.000000 pyfiredb-0.0.4/README.md
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-18 04:15:20.139664 pyfiredb-0.0.4/pyfiredb/
--rw-rw-r--   0 andres    (1000) andres    (1000)      128 2023-06-09 02:15:32.000000 pyfiredb-0.0.4/pyfiredb/__init__.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1776 2023-06-18 03:57:48.000000 pyfiredb-0.0.4/pyfiredb/database.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      666 2023-06-09 00:39:10.000000 pyfiredb-0.0.4/pyfiredb/session.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      299 2023-06-09 21:36:30.000000 pyfiredb-0.0.4/pyfiredb/settings.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-18 04:15:20.139664 pyfiredb-0.0.4/pyfiredb.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1970 2023-06-18 04:15:20.000000 pyfiredb-0.0.4/pyfiredb.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      272 2023-06-18 04:15:20.000000 pyfiredb-0.0.4/pyfiredb.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-06-18 04:15:20.000000 pyfiredb-0.0.4/pyfiredb.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        9 2023-06-18 04:15:20.000000 pyfiredb-0.0.4/pyfiredb.egg-info/requires.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        9 2023-06-18 04:15:20.000000 pyfiredb-0.0.4/pyfiredb.egg-info/top_level.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-06-18 04:15:20.143664 pyfiredb-0.0.4/setup.cfg
--rw-rw-r--   0 andres    (1000) andres    (1000)     1089 2023-06-18 04:15:08.000000 pyfiredb-0.0.4/setup.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-19 03:14:55.773995 pyfiredb-0.0.5/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1084 2023-03-09 17:21:54.000000 pyfiredb-0.0.5/LICENSE.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1970 2023-06-19 03:14:55.773995 pyfiredb-0.0.5/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1295 2023-06-09 02:20:03.000000 pyfiredb-0.0.5/README.md
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-19 03:14:55.769996 pyfiredb-0.0.5/pyfiredb/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      128 2023-06-09 02:15:32.000000 pyfiredb-0.0.5/pyfiredb/__init__.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1776 2023-06-18 03:57:48.000000 pyfiredb-0.0.5/pyfiredb/database.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      666 2023-06-09 00:39:10.000000 pyfiredb-0.0.5/pyfiredb/session.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      890 2023-06-19 03:10:46.000000 pyfiredb-0.0.5/pyfiredb/settings.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-19 03:14:55.773995 pyfiredb-0.0.5/pyfiredb.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1970 2023-06-19 03:14:55.000000 pyfiredb-0.0.5/pyfiredb.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      272 2023-06-19 03:14:55.000000 pyfiredb-0.0.5/pyfiredb.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-06-19 03:14:55.000000 pyfiredb-0.0.5/pyfiredb.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        9 2023-06-19 03:14:55.000000 pyfiredb-0.0.5/pyfiredb.egg-info/requires.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        9 2023-06-19 03:14:55.000000 pyfiredb-0.0.5/pyfiredb.egg-info/top_level.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-06-19 03:14:55.773995 pyfiredb-0.0.5/setup.cfg
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1089 2023-06-19 02:58:41.000000 pyfiredb-0.0.5/setup.py
```

### Comparing `pyfiredb-0.0.4/LICENSE.txt` & `pyfiredb-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfiredb-0.0.4/PKG-INFO` & `pyfiredb-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfiredb
-Version: 0.0.4
+Version: 0.0.5
 Summary: pyfire is a package that simplifies querying with Pyrebase,    making interactions with Firebase databases effortless.
 Home-page: https://github.com/andresroh/pyfire
 Author: Camilo Andrés Rodríguez
 Author-email: andres.roh@gmail.com
 License: MIT
 Keywords: python,alegra,alegra.com
 Platform: UNKNOWN
```

### Comparing `pyfiredb-0.0.4/README.md` & `pyfiredb-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyfiredb-0.0.4/pyfiredb/database.py` & `pyfiredb-0.0.5/pyfiredb/database.py`

 * *Files identical despite different names*

### Comparing `pyfiredb-0.0.4/pyfiredb/session.py` & `pyfiredb-0.0.5/pyfiredb/session.py`

 * *Files identical despite different names*

### Comparing `pyfiredb-0.0.4/pyfiredb.egg-info/PKG-INFO` & `pyfiredb-0.0.5/pyfiredb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfiredb
-Version: 0.0.4
+Version: 0.0.5
 Summary: pyfire is a package that simplifies querying with Pyrebase,    making interactions with Firebase databases effortless.
 Home-page: https://github.com/andresroh/pyfire
 Author: Camilo Andrés Rodríguez
 Author-email: andres.roh@gmail.com
 License: MIT
 Keywords: python,alegra,alegra.com
 Platform: UNKNOWN
```

