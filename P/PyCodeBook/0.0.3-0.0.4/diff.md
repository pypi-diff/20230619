# Comparing `tmp/PyCodeBook-0.0.3.tar.gz` & `tmp/PyCodeBook-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCodeBook-0.0.3.tar", last modified: Sun Jun 18 04:00:17 2023, max compression
+gzip compressed data, was "PyCodeBook-0.0.4.tar", last modified: Mon Jun 19 00:38:43 2023, max compression
```

## Comparing `PyCodeBook-0.0.3.tar` & `PyCodeBook-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-18 04:00:17.498589 PyCodeBook-0.0.3/
-drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-18 04:00:17.497302 PyCodeBook-0.0.3/CodeBook/
--rw-r--r--   0 huangjiabao   (501) staff       (20)      243 2023-06-17 18:32:13.000000 PyCodeBook-0.0.3/CodeBook/__init__.py
--rw-r--r--   0 huangjiabao   (501) staff       (20)      516 2023-06-17 18:16:29.000000 PyCodeBook-0.0.3/CodeBook/__version__.py
--rw-r--r--   0 huangjiabao   (501) staff       (20)      305 2023-06-18 02:50:23.000000 PyCodeBook-0.0.3/CodeBook/engine.py
-drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-18 04:00:17.497698 PyCodeBook-0.0.3/CodeBook/variable/
--rw-r--r--   0 huangjiabao   (501) staff       (20)      162 2023-06-17 17:54:20.000000 PyCodeBook-0.0.3/CodeBook/variable/__init__.py
--rw-r--r--   0 huangjiabao   (501) staff       (20)      352 2023-06-18 02:51:23.000000 PyCodeBook-0.0.3/CodeBook/variable/__version__.py
--rw-r--r--   0 huangjiabao   (501) staff       (20)      316 2023-06-17 18:13:53.000000 PyCodeBook-0.0.3/CodeBook/variable/variable.py
--rw-r--r--   0 huangjiabao   (501) staff       (20)     1067 2023-06-17 17:44:13.000000 PyCodeBook-0.0.3/LICENSE
--rw-r--r--   0 huangjiabao   (501) staff       (20)       25 2023-06-17 17:43:01.000000 PyCodeBook-0.0.3/MANIFEST.in
--rw-r--r--   0 huangjiabao   (501) staff       (20)      732 2023-06-18 04:00:17.498449 PyCodeBook-0.0.3/PKG-INFO
-drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-18 04:00:17.498254 PyCodeBook-0.0.3/PyCodeBook.egg-info/
--rw-r--r--   0 huangjiabao   (501) staff       (20)      732 2023-06-18 04:00:17.000000 PyCodeBook-0.0.3/PyCodeBook.egg-info/PKG-INFO
--rw-r--r--   0 huangjiabao   (501) staff       (20)      331 2023-06-18 04:00:17.000000 PyCodeBook-0.0.3/PyCodeBook.egg-info/SOURCES.txt
--rw-r--r--   0 huangjiabao   (501) staff       (20)        1 2023-06-18 04:00:17.000000 PyCodeBook-0.0.3/PyCodeBook.egg-info/dependency_links.txt
--rw-r--r--   0 huangjiabao   (501) staff       (20)        9 2023-06-18 04:00:17.000000 PyCodeBook-0.0.3/PyCodeBook.egg-info/top_level.txt
--rw-r--r--   0 huangjiabao   (501) staff       (20)       60 2023-06-17 18:30:39.000000 PyCodeBook-0.0.3/README.md
--rw-r--r--   0 huangjiabao   (501) staff       (20)       38 2023-06-18 04:00:17.498637 PyCodeBook-0.0.3/setup.cfg
--rw-r--r--   0 huangjiabao   (501) staff       (20)     3894 2023-06-18 04:00:01.000000 PyCodeBook-0.0.3/setup.py
+drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-19 00:38:43.869682 PyCodeBook-0.0.4/
+drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-19 00:38:43.867505 PyCodeBook-0.0.4/CodeBook/
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      243 2023-06-17 18:32:13.000000 PyCodeBook-0.0.4/CodeBook/__init__.py
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      516 2023-06-17 18:16:29.000000 PyCodeBook-0.0.4/CodeBook/__version__.py
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      305 2023-06-18 02:50:23.000000 PyCodeBook-0.0.4/CodeBook/engine.py
+drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-19 00:38:43.868431 PyCodeBook-0.0.4/CodeBook/variable/
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      162 2023-06-17 17:54:20.000000 PyCodeBook-0.0.4/CodeBook/variable/__init__.py
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      352 2023-06-18 02:51:23.000000 PyCodeBook-0.0.4/CodeBook/variable/__version__.py
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      397 2023-06-19 00:38:22.000000 PyCodeBook-0.0.4/CodeBook/variable/variable.py
+-rw-r--r--   0 huangjiabao   (501) staff       (20)     1067 2023-06-17 17:44:13.000000 PyCodeBook-0.0.4/LICENSE
+-rw-r--r--   0 huangjiabao   (501) staff       (20)       25 2023-06-17 17:43:01.000000 PyCodeBook-0.0.4/MANIFEST.in
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      732 2023-06-19 00:38:43.869512 PyCodeBook-0.0.4/PKG-INFO
+drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-19 00:38:43.869231 PyCodeBook-0.0.4/PyCodeBook.egg-info/
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      732 2023-06-19 00:38:43.000000 PyCodeBook-0.0.4/PyCodeBook.egg-info/PKG-INFO
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      331 2023-06-19 00:38:43.000000 PyCodeBook-0.0.4/PyCodeBook.egg-info/SOURCES.txt
+-rw-r--r--   0 huangjiabao   (501) staff       (20)        1 2023-06-19 00:38:43.000000 PyCodeBook-0.0.4/PyCodeBook.egg-info/dependency_links.txt
+-rw-r--r--   0 huangjiabao   (501) staff       (20)        9 2023-06-19 00:38:43.000000 PyCodeBook-0.0.4/PyCodeBook.egg-info/top_level.txt
+-rw-r--r--   0 huangjiabao   (501) staff       (20)       60 2023-06-17 18:30:39.000000 PyCodeBook-0.0.4/README.md
+-rw-r--r--   0 huangjiabao   (501) staff       (20)       38 2023-06-19 00:38:43.869735 PyCodeBook-0.0.4/setup.cfg
+-rw-r--r--   0 huangjiabao   (501) staff       (20)     3894 2023-06-19 00:38:26.000000 PyCodeBook-0.0.4/setup.py
```

### Comparing `PyCodeBook-0.0.3/CodeBook/__version__.py` & `PyCodeBook-0.0.4/CodeBook/__version__.py`

 * *Files identical despite different names*

### Comparing `PyCodeBook-0.0.3/LICENSE` & `PyCodeBook-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCodeBook-0.0.3/PKG-INFO` & `PyCodeBook-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCodeBook
-Version: 0.0.3
+Version: 0.0.4
 Summary: 方便学员查询 Python 相关知识点,辅助考试。
 Home-page: https://github.com/AndersonHJB/PyNoteBook
 Author: Bornforthis
 Author-email: bornforthis@bornforthis.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `PyCodeBook-0.0.3/PyCodeBook.egg-info/PKG-INFO` & `PyCodeBook-0.0.4/PyCodeBook.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCodeBook
-Version: 0.0.3
+Version: 0.0.4
 Summary: 方便学员查询 Python 相关知识点,辅助考试。
 Home-page: https://github.com/AndersonHJB/PyNoteBook
 Author: Bornforthis
 Author-email: bornforthis@bornforthis.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `PyCodeBook-0.0.3/setup.py` & `PyCodeBook-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'PyCodeBook'
 DESCRIPTION = '方便学员查询 Python 相关知识点,辅助考试。'
 URL = 'https://github.com/AndersonHJB/PyNoteBook'
 EMAIL = 'bornforthis@bornforthis.com'
 AUTHOR = 'Bornforthis'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

