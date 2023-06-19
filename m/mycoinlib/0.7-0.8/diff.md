# Comparing `tmp/mycoinlib-0.7.tar.gz` & `tmp/mycoinlib-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mycoinlib-0.7.tar", last modified: Mon Jun 19 20:03:16 2023, max compression
+gzip compressed data, was "mycoinlib-0.8.tar", last modified: Mon Jun 19 20:09:42 2023, max compression
```

## Comparing `mycoinlib-0.7.tar` & `mycoinlib-0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 20:03:16.797041 mycoinlib-0.7/
--rw-rw-rw-   0        0        0       54 2023-06-19 20:03:16.785120 mycoinlib-0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-19 20:03:16.540202 mycoinlib-0.7/mycoinlib/
--rw-rw-rw-   0        0        0       38 2023-06-19 19:46:26.000000 mycoinlib-0.7/mycoinlib/__init__.py
--rw-rw-rw-   0        0        0     5791 2023-06-19 19:50:11.000000 mycoinlib-0.7/mycoinlib/mycoinlib.py
-drwxrwxrwx   0        0        0        0 2023-06-19 20:03:16.780635 mycoinlib-0.7/mycoinlib.egg-info/
--rw-rw-rw-   0        0        0       54 2023-06-19 20:03:14.000000 mycoinlib-0.7/mycoinlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-06-19 20:03:14.000000 mycoinlib-0.7/mycoinlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 20:03:14.000000 mycoinlib-0.7/mycoinlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-19 20:03:14.000000 mycoinlib-0.7/mycoinlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-19 20:03:14.000000 mycoinlib-0.7/mycoinlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 20:03:16.799025 mycoinlib-0.7/setup.cfg
--rw-rw-rw-   0        0        0      257 2023-06-19 20:03:09.000000 mycoinlib-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:09:42.003070 mycoinlib-0.8/
+-rw-rw-rw-   0        0        0       54 2023-06-19 20:09:41.998102 mycoinlib-0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 20:09:41.908170 mycoinlib-0.8/mycoinlib/
+-rw-rw-rw-   0        0        0       26 2023-06-19 20:09:20.000000 mycoinlib-0.8/mycoinlib/__init__.py
+-rw-rw-rw-   0        0        0     5791 2023-06-19 19:50:11.000000 mycoinlib-0.8/mycoinlib/mycoinlib.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:09:41.991150 mycoinlib-0.8/mycoinlib.egg-info/
+-rw-rw-rw-   0        0        0       54 2023-06-19 20:09:41.000000 mycoinlib-0.8/mycoinlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-06-19 20:09:41.000000 mycoinlib-0.8/mycoinlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 20:09:41.000000 mycoinlib-0.8/mycoinlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-19 20:09:41.000000 mycoinlib-0.8/mycoinlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-19 20:09:41.000000 mycoinlib-0.8/mycoinlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 20:09:42.004063 mycoinlib-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      257 2023-06-19 20:09:34.000000 mycoinlib-0.8/setup.py
```

### Comparing `mycoinlib-0.7/mycoinlib/mycoinlib.py` & `mycoinlib-0.8/mycoinlib/mycoinlib.py`

 * *Files identical despite different names*

