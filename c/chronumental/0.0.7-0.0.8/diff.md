# Comparing `tmp/chronumental-0.0.7.tar.gz` & `tmp/chronumental-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chronumental-0.0.7.tar", last modified: Fri Oct  8 17:23:07 2021, max compression
+gzip compressed data, was "chronumental-0.0.8.tar", last modified: Fri Oct  8 17:35:09 2021, max compression
```

## Comparing `chronumental-0.0.7.tar` & `chronumental-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-10-08 17:23:07.699706 chronumental-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-10-08 17:23:07.695706 chronumental-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-10-08 17:23:07.699706 chronumental-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)      836 2021-10-08 17:22:56.000000 chronumental-0.0.7/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (116)      601 2021-10-08 17:23:07.699706 chronumental-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       87 2021-10-08 17:22:56.000000 chronumental-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      195 2021-10-08 17:22:56.000000 chronumental-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       85 2021-10-08 17:22:56.000000 chronumental-0.0.7/run.sh
--rw-r--r--   0 runner    (1001) docker     (116)      678 2021-10-08 17:23:07.703706 chronumental-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-10-08 17:23:07.695706 chronumental-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-10-08 17:23:07.699706 chronumental-0.0.7/src/chronumental/
--rw-r--r--   0 runner    (1001) docker     (116)       23 2021-10-08 17:22:56.000000 chronumental-0.0.7/src/chronumental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9007 2021-10-08 17:22:56.000000 chronumental-0.0.7/src/chronumental/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)      142 2021-10-08 17:23:07.000000 chronumental-0.0.7/src/chronumental/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)      620 2021-10-08 17:22:56.000000 chronumental-0.0.7/src/chronumental/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-10-08 17:23:07.699706 chronumental-0.0.7/src/chronumental.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      601 2021-10-08 17:23:07.000000 chronumental-0.0.7/src/chronumental.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      382 2021-10-08 17:23:07.000000 chronumental-0.0.7/src/chronumental.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-10-08 17:23:07.000000 chronumental-0.0.7/src/chronumental.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       30 2021-10-08 17:23:07.000000 chronumental-0.0.7/src/chronumental.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2021-10-08 17:23:07.000000 chronumental-0.0.7/src/chronumental.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-10-08 17:35:09.093340 chronumental-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-10-08 17:35:09.089340 chronumental-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-10-08 17:35:09.093340 chronumental-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)      836 2021-10-08 17:34:58.000000 chronumental-0.0.8/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      349 2021-10-08 17:34:58.000000 chronumental-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)      601 2021-10-08 17:35:09.093340 chronumental-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)       87 2021-10-08 17:34:58.000000 chronumental-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      195 2021-10-08 17:34:58.000000 chronumental-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)       85 2021-10-08 17:34:58.000000 chronumental-0.0.8/run.sh
+-rw-r--r--   0 runner    (1001) docker     (116)      764 2021-10-08 17:35:09.093340 chronumental-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-10-08 17:35:09.089340 chronumental-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-10-08 17:35:09.093340 chronumental-0.0.8/src/chronumental/
+-rw-r--r--   0 runner    (1001) docker     (116)       23 2021-10-08 17:34:58.000000 chronumental-0.0.8/src/chronumental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9007 2021-10-08 17:34:58.000000 chronumental-0.0.8/src/chronumental/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      142 2021-10-08 17:35:09.000000 chronumental-0.0.8/src/chronumental/_version.py
+-rw-r--r--   0 runner    (1001) docker     (116)      620 2021-10-08 17:34:58.000000 chronumental-0.0.8/src/chronumental/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-10-08 17:35:09.093340 chronumental-0.0.8/src/chronumental.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      601 2021-10-08 17:35:09.000000 chronumental-0.0.8/src/chronumental.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      436 2021-10-08 17:35:09.000000 chronumental-0.0.8/src/chronumental.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-10-08 17:35:09.000000 chronumental-0.0.8/src/chronumental.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       61 2021-10-08 17:35:09.000000 chronumental-0.0.8/src/chronumental.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       30 2021-10-08 17:35:09.000000 chronumental-0.0.8/src/chronumental.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       13 2021-10-08 17:35:09.000000 chronumental-0.0.8/src/chronumental.egg-info/top_level.txt
```

### Comparing `chronumental-0.0.7/.github/workflows/main.yml` & `chronumental-0.0.8/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `chronumental-0.0.7/PKG-INFO` & `chronumental-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chronumental
-Version: 0.0.7
+Version: 0.0.8
 Summary: Large timetrees
 Home-page: https://github.com/theosanderson/chronumental
 Author: Theo Sanderson
 Author-email: theo@theo.io
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/theosanderson/chronumental/issues
 Platform: UNKNOWN
```

### Comparing `chronumental-0.0.7/src/chronumental/__main__.py` & `chronumental-0.0.8/src/chronumental/__main__.py`

 * *Files identical despite different names*

### Comparing `chronumental-0.0.7/src/chronumental/helpers.py` & `chronumental-0.0.8/src/chronumental/helpers.py`

 * *Files identical despite different names*

### Comparing `chronumental-0.0.7/src/chronumental.egg-info/PKG-INFO` & `chronumental-0.0.8/src/chronumental.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chronumental
-Version: 0.0.7
+Version: 0.0.8
 Summary: Large timetrees
 Home-page: https://github.com/theosanderson/chronumental
 Author: Theo Sanderson
 Author-email: theo@theo.io
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/theosanderson/chronumental/issues
 Platform: UNKNOWN
```

