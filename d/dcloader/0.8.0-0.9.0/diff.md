# Comparing `tmp/dcloader-0.8.0.tar.gz` & `tmp/dcloader-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcloader-0.8.0.tar", last modified: Fri Dec 16 11:57:42 2022, max compression
+gzip compressed data, was "dcloader-0.9.0.tar", last modified: Sun Dec 18 12:04:17 2022, max compression
```

## Comparing `dcloader-0.8.0.tar` & `dcloader-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2022-12-16 11:57:42.781320 dcloader-0.8.0/
--rw-rw-r--   0 ali       (1000) ali       (1000)      164 2022-12-16 11:57:42.781320 dcloader-0.8.0/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)      521 2022-11-08 15:23:28.000000 dcloader-0.8.0/README.md
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2022-12-16 11:57:42.777320 dcloader-0.8.0/dcloader/
--rw-rw-r--   0 ali       (1000) ali       (1000)       67 2022-12-16 10:48:28.000000 dcloader-0.8.0/dcloader/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     2102 2022-12-16 11:40:48.000000 dcloader-0.8.0/dcloader/loader.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2022-12-16 11:57:42.781320 dcloader-0.8.0/dcloader/source/
--rw-rw-r--   0 ali       (1000) ali       (1000)      138 2022-12-16 08:28:41.000000 dcloader-0.8.0/dcloader/source/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      425 2022-12-16 10:49:30.000000 dcloader-0.8.0/dcloader/source/dict.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      597 2022-12-16 10:49:14.000000 dcloader-0.8.0/dcloader/source/env.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      928 2022-12-16 11:38:59.000000 dcloader-0.8.0/dcloader/source/utils.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      588 2022-12-16 10:50:10.000000 dcloader-0.8.0/dcloader/source/yaml.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2022-12-16 11:57:42.781320 dcloader-0.8.0/dcloader.egg-info/
--rw-rw-r--   0 ali       (1000) ali       (1000)      164 2022-12-16 11:57:42.000000 dcloader-0.8.0/dcloader.egg-info/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)      371 2022-12-16 11:57:42.000000 dcloader-0.8.0/dcloader.egg-info/SOURCES.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        1 2022-12-16 11:57:42.000000 dcloader-0.8.0/dcloader.egg-info/dependency_links.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       14 2022-12-16 11:57:42.000000 dcloader-0.8.0/dcloader.egg-info/requires.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        9 2022-12-16 11:57:42.000000 dcloader-0.8.0/dcloader.egg-info/top_level.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       79 2022-12-16 11:57:42.781320 dcloader-0.8.0/setup.cfg
--rw-rw-r--   0 ali       (1000) ali       (1000)      360 2022-12-16 11:57:01.000000 dcloader-0.8.0/setup.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2022-12-16 11:57:42.781320 dcloader-0.8.0/test/
--rw-rw-r--   0 ali       (1000) ali       (1000)     2219 2022-12-16 11:35:46.000000 dcloader-0.8.0/test/test_loader.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2022-12-18 12:04:17.160123 dcloader-0.9.0/
+-rw-rw-r--   0 ali       (1000) ali       (1000)      164 2022-12-18 12:04:17.160123 dcloader-0.9.0/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)      521 2022-11-08 15:23:28.000000 dcloader-0.9.0/README.md
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2022-12-18 12:04:17.160123 dcloader-0.9.0/dcloader/
+-rw-rw-r--   0 ali       (1000) ali       (1000)       67 2022-12-16 10:48:28.000000 dcloader-0.9.0/dcloader/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     2102 2022-12-16 11:40:48.000000 dcloader-0.9.0/dcloader/loader.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2022-12-18 12:04:17.160123 dcloader-0.9.0/dcloader/source/
+-rw-rw-r--   0 ali       (1000) ali       (1000)      138 2022-12-16 08:28:41.000000 dcloader-0.9.0/dcloader/source/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      425 2022-12-16 10:49:30.000000 dcloader-0.9.0/dcloader/source/dict.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      597 2022-12-16 10:49:14.000000 dcloader-0.9.0/dcloader/source/env.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      934 2022-12-18 12:02:47.000000 dcloader-0.9.0/dcloader/source/utils.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      588 2022-12-16 10:50:10.000000 dcloader-0.9.0/dcloader/source/yaml.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2022-12-18 12:04:17.160123 dcloader-0.9.0/dcloader.egg-info/
+-rw-rw-r--   0 ali       (1000) ali       (1000)      164 2022-12-18 12:04:17.000000 dcloader-0.9.0/dcloader.egg-info/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)      371 2022-12-18 12:04:17.000000 dcloader-0.9.0/dcloader.egg-info/SOURCES.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        1 2022-12-18 12:04:17.000000 dcloader-0.9.0/dcloader.egg-info/dependency_links.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       14 2022-12-18 12:04:17.000000 dcloader-0.9.0/dcloader.egg-info/requires.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        9 2022-12-18 12:04:17.000000 dcloader-0.9.0/dcloader.egg-info/top_level.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       79 2022-12-18 12:04:17.160123 dcloader-0.9.0/setup.cfg
+-rw-rw-r--   0 ali       (1000) ali       (1000)      360 2022-12-18 12:03:04.000000 dcloader-0.9.0/setup.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2022-12-18 12:04:17.160123 dcloader-0.9.0/test/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     2219 2022-12-16 11:35:46.000000 dcloader-0.9.0/test/test_loader.py
```

### Comparing `dcloader-0.8.0/README.md` & `dcloader-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `dcloader-0.8.0/dcloader/loader.py` & `dcloader-0.9.0/dcloader/loader.py`

 * *Files identical despite different names*

### Comparing `dcloader-0.8.0/dcloader/source/env.py` & `dcloader-0.9.0/dcloader/source/env.py`

 * *Files identical despite different names*

### Comparing `dcloader-0.8.0/dcloader/source/utils.py` & `dcloader-0.9.0/dcloader/source/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     if duration.endswith("d"):
         return timedelta(days=int(duration[:-1]))
 
     raise ValueError("not supported")
 
 
 def from_str(value: str, t) -> Any:
-    if t in (str, int, float):
+    if t in (str, int, float, bool):
         return t(value)
 
     if t is timedelta:
         return timedelta_from_str(value)
 
     if get_origin(t) is builtins.list:
         item_type = next(iter(get_args(t)), str)
```

### Comparing `dcloader-0.8.0/dcloader/source/yaml.py` & `dcloader-0.9.0/dcloader/source/yaml.py`

 * *Files identical despite different names*

### Comparing `dcloader-0.8.0/test/test_loader.py` & `dcloader-0.9.0/test/test_loader.py`

 * *Files identical despite different names*

