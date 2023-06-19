# Comparing `tmp/pymodaq_plugins_hamamatsu-0.1.0.tar.gz` & `tmp/pymodaq_plugins_hamamatsu-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_hamamatsu-0.1.0.tar", last modified: Mon Oct 24 11:42:06 2022, max compression
+gzip compressed data, was "pymodaq_plugins_hamamatsu-0.2.0.tar", last modified: Mon Jun 19 10:22:42 2023, max compression
```

## Comparing `pymodaq_plugins_hamamatsu-0.1.0.tar` & `pymodaq_plugins_hamamatsu-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:42:06.298155 pymodaq_plugins_hamamatsu-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)    21395 2022-10-24 11:41:58.000000 pymodaq_plugins_hamamatsu-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-10-24 11:41:58.000000 pymodaq_plugins_hamamatsu-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1896 2022-10-24 11:42:06.298155 pymodaq_plugins_hamamatsu-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-10-24 11:41:58.000000 pymodaq_plugins_hamamatsu-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-24 11:42:06.298155 pymodaq_plugins_hamamatsu-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1819 2022-10-24 11:41:58.000000 pymodaq_plugins_hamamatsu-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:42:06.294155 pymodaq_plugins_hamamatsu-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:42:06.298155 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-24 11:41:58.000000 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-10-24 11:41:58.000000 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:42:06.298155 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu/daq_move_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-10-24 11:41:58.000000 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu/daq_move_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:42:06.298155 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-24 11:41:58.000000 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:42:06.298155 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/plugins_0D/
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-10-24 11:41:58.000000 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/plugins_0D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:42:06.298155 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/plugins_1D/
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-10-24 11:41:58.000000 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/plugins_1D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:42:06.298155 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/plugins_2D/
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-10-24 11:41:58.000000 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/plugins_2D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9099 2022-10-24 11:41:58.000000 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Hamamatsu.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:42:06.298155 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/plugins_ND/
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-10-24 11:41:58.000000 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/plugins_ND/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:42:06.298155 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu/hardware/
--rw-r--r--   0 runner    (1001) docker     (121)    24957 2022-10-24 11:41:58.000000 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu/hardware/Hamamatsu_camera_dom.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 11:41:58.000000 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu/hardware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:42:06.298155 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1896 2022-10-24 11:42:06.000000 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-10-24 11:42:06.000000 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 11:42:06.000000 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-10-24 11:42:06.000000 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-24 11:42:06.000000 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-10-24 11:42:06.000000 pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:42.097986 pymodaq_plugins_hamamatsu-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    21395 2023-06-19 10:22:32.000000 pymodaq_plugins_hamamatsu-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-19 10:22:32.000000 pymodaq_plugins_hamamatsu-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-19 10:22:42.097986 pymodaq_plugins_hamamatsu-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-19 10:22:32.000000 pymodaq_plugins_hamamatsu-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 10:22:42.097986 pymodaq_plugins_hamamatsu-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-19 10:22:32.000000 pymodaq_plugins_hamamatsu-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:42.093985 pymodaq_plugins_hamamatsu-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:42.097986 pymodaq_plugins_hamamatsu-0.2.0/src/pymodaq_plugins_hamamatsu/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 10:22:32.000000 pymodaq_plugins_hamamatsu-0.2.0/src/pymodaq_plugins_hamamatsu/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-19 10:22:32.000000 pymodaq_plugins_hamamatsu-0.2.0/src/pymodaq_plugins_hamamatsu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:42.097986 pymodaq_plugins_hamamatsu-0.2.0/src/pymodaq_plugins_hamamatsu/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-19 10:22:32.000000 pymodaq_plugins_hamamatsu-0.2.0/src/pymodaq_plugins_hamamatsu/daq_move_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:42.097986 pymodaq_plugins_hamamatsu-0.2.0/src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-19 10:22:32.000000 pymodaq_plugins_hamamatsu-0.2.0/src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:42.097986 pymodaq_plugins_hamamatsu-0.2.0/src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-19 10:22:32.000000 pymodaq_plugins_hamamatsu-0.2.0/src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/plugins_2D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-06-19 10:22:32.000000 pymodaq_plugins_hamamatsu-0.2.0/src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Hamamatsu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:42.097986 pymodaq_plugins_hamamatsu-0.2.0/src/pymodaq_plugins_hamamatsu/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:32.000000 pymodaq_plugins_hamamatsu-0.2.0/src/pymodaq_plugins_hamamatsu/hardware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:42.097986 pymodaq_plugins_hamamatsu-0.2.0/src/pymodaq_plugins_hamamatsu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-19 10:22:42.000000 pymodaq_plugins_hamamatsu-0.2.0/src/pymodaq_plugins_hamamatsu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-19 10:22:42.000000 pymodaq_plugins_hamamatsu-0.2.0/src/pymodaq_plugins_hamamatsu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 10:22:42.000000 pymodaq_plugins_hamamatsu-0.2.0/src/pymodaq_plugins_hamamatsu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-19 10:22:42.000000 pymodaq_plugins_hamamatsu-0.2.0/src/pymodaq_plugins_hamamatsu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-19 10:22:42.000000 pymodaq_plugins_hamamatsu-0.2.0/src/pymodaq_plugins_hamamatsu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-19 10:22:42.000000 pymodaq_plugins_hamamatsu-0.2.0/src/pymodaq_plugins_hamamatsu.egg-info/top_level.txt
```

### Comparing `pymodaq_plugins_hamamatsu-0.1.0/LICENSE` & `pymodaq_plugins_hamamatsu-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_hamamatsu-0.1.0/setup.py` & `pymodaq_plugins_hamamatsu-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_hamamatsu-0.1.0/src/pymodaq_plugins_hamamatsu.egg-info/SOURCES.txt` & `pymodaq_plugins_hamamatsu-0.2.0/src/pymodaq_plugins_hamamatsu.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,10 @@
 src/pymodaq_plugins_hamamatsu.egg-info/SOURCES.txt
 src/pymodaq_plugins_hamamatsu.egg-info/dependency_links.txt
 src/pymodaq_plugins_hamamatsu.egg-info/entry_points.txt
 src/pymodaq_plugins_hamamatsu.egg-info/requires.txt
 src/pymodaq_plugins_hamamatsu.egg-info/top_level.txt
 src/pymodaq_plugins_hamamatsu/daq_move_plugins/__init__.py
 src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/__init__.py
-src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/plugins_0D/__init__.py
-src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/plugins_1D/__init__.py
 src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/plugins_2D/__init__.py
 src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Hamamatsu.py
-src/pymodaq_plugins_hamamatsu/daq_viewer_plugins/plugins_ND/__init__.py
-src/pymodaq_plugins_hamamatsu/hardware/Hamamatsu_camera_dom.py
 src/pymodaq_plugins_hamamatsu/hardware/__init__.py
```

