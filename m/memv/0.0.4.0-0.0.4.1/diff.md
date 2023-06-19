# Comparing `tmp/memv-0.0.4.0.tar.gz` & `tmp/memv-0.0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memv-0.0.4.0.tar", last modified: Mon Jun 19 02:00:42 2023, max compression
+gzip compressed data, was "memv-0.0.4.1.tar", last modified: Mon Jun 19 02:01:13 2023, max compression
```

## Comparing `memv-0.0.4.0.tar` & `memv-0.0.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 02:00:42.716791 memv-0.0.4.0/
--rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.4.0/LICENSE
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 02:00:42.716539 memv-0.0.4.0/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      268 2023-06-19 02:00:06.000000 memv-0.0.4.0/README.md
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 02:00:42.714647 memv-0.0.4.0/memv/
--rw-r--r--   0 nhunh      (501) staff       (20)       22 2023-06-16 09:34:09.000000 memv-0.0.4.0/memv/__init__.py
--rw-r--r--   0 nhunh      (501) staff       (20)     4434 2023-06-19 01:55:36.000000 memv-0.0.4.0/memv/memv.py
--rw-r--r--   0 nhunh      (501) staff       (20)      975 2023-06-16 10:09:56.000000 memv-0.0.4.0/memv/utils.py
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 02:00:42.716301 memv-0.0.4.0/memv.egg-info/
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 02:00:42.000000 memv-0.0.4.0/memv.egg-info/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-19 02:00:42.000000 memv-0.0.4.0/memv.egg-info/SOURCES.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-19 02:00:42.000000 memv-0.0.4.0/memv.egg-info/dependency_links.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-19 02:00:42.000000 memv-0.0.4.0/memv.egg-info/entry_points.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       65 2023-06-19 02:00:42.000000 memv-0.0.4.0/memv.egg-info/requires.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-19 02:00:42.000000 memv-0.0.4.0/memv.egg-info/top_level.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-19 02:00:42.716850 memv-0.0.4.0/setup.cfg
--rw-r--r--   0 nhunh      (501) staff       (20)      442 2023-06-19 02:00:39.000000 memv-0.0.4.0/setup.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 02:01:13.650611 memv-0.0.4.1/
+-rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.4.1/LICENSE
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 02:01:13.650339 memv-0.0.4.1/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      268 2023-06-19 02:00:06.000000 memv-0.0.4.1/README.md
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 02:01:13.647950 memv-0.0.4.1/memv/
+-rw-r--r--   0 nhunh      (501) staff       (20)       22 2023-06-16 09:34:09.000000 memv-0.0.4.1/memv/__init__.py
+-rw-r--r--   0 nhunh      (501) staff       (20)     4434 2023-06-19 01:55:36.000000 memv-0.0.4.1/memv/memv.py
+-rw-r--r--   0 nhunh      (501) staff       (20)      975 2023-06-16 10:09:56.000000 memv-0.0.4.1/memv/utils.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 02:01:13.650051 memv-0.0.4.1/memv.egg-info/
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 02:01:13.000000 memv-0.0.4.1/memv.egg-info/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-19 02:01:13.000000 memv-0.0.4.1/memv.egg-info/SOURCES.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-19 02:01:13.000000 memv-0.0.4.1/memv.egg-info/dependency_links.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-19 02:01:13.000000 memv-0.0.4.1/memv.egg-info/entry_points.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       65 2023-06-19 02:01:13.000000 memv-0.0.4.1/memv.egg-info/requires.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-19 02:01:13.000000 memv-0.0.4.1/memv.egg-info/top_level.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-19 02:01:13.650664 memv-0.0.4.1/setup.cfg
+-rw-r--r--   0 nhunh      (501) staff       (20)      442 2023-06-19 02:01:11.000000 memv-0.0.4.1/setup.py
```

### Comparing `memv-0.0.4.0/LICENSE` & `memv-0.0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `memv-0.0.4.0/memv/memv.py` & `memv-0.0.4.1/memv/memv.py`

 * *Files identical despite different names*

### Comparing `memv-0.0.4.0/memv/utils.py` & `memv-0.0.4.1/memv/utils.py`

 * *Files identical despite different names*

