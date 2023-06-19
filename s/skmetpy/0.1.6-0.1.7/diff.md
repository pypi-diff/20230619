# Comparing `tmp/skmetpy-0.1.6.tar.gz` & `tmp/skmetpy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skmetpy-0.1.6.tar", last modified: Mon Jun 19 13:35:33 2023, max compression
+gzip compressed data, was "skmetpy-0.1.7.tar", last modified: Mon Jun 19 13:43:23 2023, max compression
```

## Comparing `skmetpy-0.1.6.tar` & `skmetpy-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 13:35:33.899213 skmetpy-0.1.6/
--rw-rw-rw-   0        0        0      259 2023-06-19 13:35:33.898211 skmetpy-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-19 13:35:33.893208 skmetpy-0.1.6/nunpy/
--rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.1.6/nunpy/__init__.py
--rw-rw-rw-   0        0        0    24712 2023-06-19 13:34:56.000000 skmetpy-0.1.6/nunpy/rechape.py
--rw-rw-rw-   0        0        0       42 2023-06-19 13:35:33.899213 skmetpy-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      324 2023-06-19 13:35:31.000000 skmetpy-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:35:33.897212 skmetpy-0.1.6/skmetpy.egg-info/
--rw-rw-rw-   0        0        0      259 2023-06-19 13:35:33.000000 skmetpy-0.1.6/skmetpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-06-19 13:35:33.000000 skmetpy-0.1.6/skmetpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 13:35:33.000000 skmetpy-0.1.6/skmetpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 13:35:33.000000 skmetpy-0.1.6/skmetpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 13:43:23.725192 skmetpy-0.1.7/
+-rw-rw-rw-   0        0        0      259 2023-06-19 13:43:23.724190 skmetpy-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 13:43:23.718113 skmetpy-0.1.7/nunpy/
+-rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.1.7/nunpy/__init__.py
+-rw-rw-rw-   0        0        0    24712 2023-06-19 13:34:56.000000 skmetpy-0.1.7/nunpy/rechape.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 13:43:23.725192 skmetpy-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      324 2023-06-19 13:43:21.000000 skmetpy-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:43:23.723188 skmetpy-0.1.7/skmetpy.egg-info/
+-rw-rw-rw-   0        0        0      259 2023-06-19 13:43:23.000000 skmetpy-0.1.7/skmetpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-06-19 13:43:23.000000 skmetpy-0.1.7/skmetpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 13:43:23.000000 skmetpy-0.1.7/skmetpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 13:43:23.000000 skmetpy-0.1.7/skmetpy.egg-info/top_level.txt
```

### Comparing `skmetpy-0.1.6/nunpy/rechape.py` & `skmetpy-0.1.7/nunpy/rechape.py`

 * *Files identical despite different names*

