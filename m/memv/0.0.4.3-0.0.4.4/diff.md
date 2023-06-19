# Comparing `tmp/memv-0.0.4.3.tar.gz` & `tmp/memv-0.0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memv-0.0.4.3.tar", last modified: Mon Jun 19 03:02:25 2023, max compression
+gzip compressed data, was "memv-0.0.4.4.tar", last modified: Mon Jun 19 03:45:31 2023, max compression
```

## Comparing `memv-0.0.4.3.tar` & `memv-0.0.4.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 03:02:25.597250 memv-0.0.4.3/
--rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.4.3/LICENSE
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 03:02:25.596983 memv-0.0.4.3/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      268 2023-06-19 02:00:06.000000 memv-0.0.4.3/README.md
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 03:02:25.593334 memv-0.0.4.3/memv/
--rw-r--r--   0 nhunh      (501) staff       (20)       22 2023-06-16 09:34:09.000000 memv-0.0.4.3/memv/__init__.py
--rw-r--r--   0 nhunh      (501) staff       (20)     4319 2023-06-19 03:02:08.000000 memv-0.0.4.3/memv/memv.py
--rw-r--r--   0 nhunh      (501) staff       (20)      975 2023-06-16 10:09:56.000000 memv-0.0.4.3/memv/utils.py
-drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 03:02:25.595389 memv-0.0.4.3/memv.egg-info/
--rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 03:02:25.000000 memv-0.0.4.3/memv.egg-info/PKG-INFO
--rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-19 03:02:25.000000 memv-0.0.4.3/memv.egg-info/SOURCES.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-19 03:02:25.000000 memv-0.0.4.3/memv.egg-info/dependency_links.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-19 03:02:25.000000 memv-0.0.4.3/memv.egg-info/entry_points.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       35 2023-06-19 03:02:25.000000 memv-0.0.4.3/memv.egg-info/requires.txt
--rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-19 03:02:25.000000 memv-0.0.4.3/memv.egg-info/top_level.txt
--rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-19 03:02:25.597303 memv-0.0.4.3/setup.cfg
--rw-r--r--   0 nhunh      (501) staff       (20)      412 2023-06-19 03:02:22.000000 memv-0.0.4.3/setup.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 03:45:31.594890 memv-0.0.4.4/
+-rw-r--r--   0 nhunh      (501) staff       (20)     1073 2023-06-16 07:55:34.000000 memv-0.0.4.4/LICENSE
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 03:45:31.594577 memv-0.0.4.4/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      268 2023-06-19 02:00:06.000000 memv-0.0.4.4/README.md
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 03:45:31.582800 memv-0.0.4.4/memv/
+-rw-r--r--   0 nhunh      (501) staff       (20)       35 2023-06-19 03:43:13.000000 memv-0.0.4.4/memv/__init__.py
+-rw-r--r--   0 nhunh      (501) staff       (20)     5219 2023-06-19 03:42:00.000000 memv-0.0.4.4/memv/memv.py
+-rw-r--r--   0 nhunh      (501) staff       (20)      975 2023-06-16 10:09:56.000000 memv-0.0.4.4/memv/utils.py
+drwxr-xr-x   0 nhunh      (501) staff       (20)        0 2023-06-19 03:45:31.594205 memv-0.0.4.4/memv.egg-info/
+-rw-r--r--   0 nhunh      (501) staff       (20)      134 2023-06-19 03:45:31.000000 memv-0.0.4.4/memv.egg-info/PKG-INFO
+-rw-r--r--   0 nhunh      (501) staff       (20)      240 2023-06-19 03:45:31.000000 memv-0.0.4.4/memv.egg-info/SOURCES.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        1 2023-06-19 03:45:31.000000 memv-0.0.4.4/memv.egg-info/dependency_links.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       40 2023-06-19 03:45:31.000000 memv-0.0.4.4/memv.egg-info/entry_points.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       35 2023-06-19 03:45:31.000000 memv-0.0.4.4/memv.egg-info/requires.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)        5 2023-06-19 03:45:31.000000 memv-0.0.4.4/memv.egg-info/top_level.txt
+-rw-r--r--   0 nhunh      (501) staff       (20)       38 2023-06-19 03:45:31.594948 memv-0.0.4.4/setup.cfg
+-rw-r--r--   0 nhunh      (501) staff       (20)      412 2023-06-19 03:45:29.000000 memv-0.0.4.4/setup.py
```

### Comparing `memv-0.0.4.3/LICENSE` & `memv-0.0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `memv-0.0.4.3/memv/utils.py` & `memv-0.0.4.4/memv/utils.py`

 * *Files identical despite different names*

