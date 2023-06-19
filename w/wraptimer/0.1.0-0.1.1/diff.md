# Comparing `tmp/wraptimer-0.1.0.tar.gz` & `tmp/wraptimer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wraptimer-0.1.0.tar", max compression
+gzip compressed data, was "wraptimer-0.1.1.tar", max compression
```

## Comparing `wraptimer-0.1.0.tar` & `wraptimer-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1523 2023-06-19 11:44:46.642770 wraptimer-0.1.0/README.md
--rw-r--r--   0        0        0      968 2023-06-19 12:01:38.496958 wraptimer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      186 2023-06-19 10:53:18.100216 wraptimer-0.1.0/wraptimer/__init__.py
--rw-r--r--   0        0        0     4231 2023-06-19 10:53:19.444284 wraptimer-0.1.0/wraptimer/timeit.py
--rw-r--r--   0        0        0     4259 2023-06-19 10:53:19.396282 wraptimer-0.1.0/wraptimer/timer.py
--rw-r--r--   0        0        0     4871 2023-06-19 10:55:34.979160 wraptimer-0.1.0/wraptimer/utils.py
--rw-r--r--   0        0        0     1956 1970-01-01 00:00:00.000000 wraptimer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1523 2023-06-19 11:44:46.642770 wraptimer-0.1.1/README.md
+-rw-r--r--   0        0        0     2801 2023-06-19 12:24:44.884070 wraptimer-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      186 2023-06-19 10:53:18.100216 wraptimer-0.1.1/wraptimer/__init__.py
+-rw-r--r--   0        0        0     4231 2023-06-19 10:53:19.444284 wraptimer-0.1.1/wraptimer/timeit.py
+-rw-r--r--   0        0        0     4259 2023-06-19 10:53:19.396282 wraptimer-0.1.1/wraptimer/timer.py
+-rw-r--r--   0        0        0     4871 2023-06-19 10:55:34.979160 wraptimer-0.1.1/wraptimer/utils.py
+-rw-r--r--   0        0        0     2190 1970-01-01 00:00:00.000000 wraptimer-0.1.1/PKG-INFO
```

### Comparing `wraptimer-0.1.0/README.md` & `wraptimer-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `wraptimer-0.1.0/wraptimer/timeit.py` & `wraptimer-0.1.1/wraptimer/timeit.py`

 * *Files identical despite different names*

### Comparing `wraptimer-0.1.0/wraptimer/timer.py` & `wraptimer-0.1.1/wraptimer/timer.py`

 * *Files identical despite different names*

### Comparing `wraptimer-0.1.0/wraptimer/utils.py` & `wraptimer-0.1.1/wraptimer/utils.py`

 * *Files identical despite different names*

### Comparing `wraptimer-0.1.0/PKG-INFO` & `wraptimer-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: wraptimer
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: An amazing alternative to Python's builtin timeit module that allows for high resolution timing of functions as well as in-depth line-by-line timing. It also exposes convenient classes to measure execution time for any arbitrary code.
 Author: Anthony Mugendi
 Author-email: ngurumugz@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

