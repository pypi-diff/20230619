# Comparing `tmp/yplib-1.6.2.tar.gz` & `tmp/yplib-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.6.2.tar", last modified: Mon Jun 19 01:01:38 2023, max compression
+gzip compressed data, was "dist\yplib-1.6.3.tar", last modified: Mon Jun 19 01:13:57 2023, max compression
```

## Comparing `yplib-1.6.2.tar` & `yplib-1.6.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 01:01:38.430665 yplib-1.6.2/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.6.2/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-19 01:01:38.430665 yplib-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.6.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 01:01:38.431489 yplib-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-19 01:01:14.000000 yplib-1.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:01:38.427732 yplib-1.6.2/yplib/
--rw-rw-rw-   0        0        0      350 2023-06-19 01:01:06.000000 yplib-1.6.2/yplib/__init__.py
--rw-rw-rw-   0        0        0    11378 2023-06-16 08:54:15.000000 yplib-1.6.2/yplib/chart.py
--rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.6.2/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.6.2/yplib/file.py
--rw-rw-rw-   0        0        0      859 2023-06-19 00:59:15.000000 yplib-1.6.2/yplib/http.py
--rw-rw-rw-   0        0        0    24344 2023-06-19 00:55:36.000000 yplib-1.6.2/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:01:38.429932 yplib-1.6.2/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-19 01:01:38.000000 yplib-1.6.2/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-06-19 01:01:38.000000 yplib-1.6.2/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 01:01:38.000000 yplib-1.6.2/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 01:01:38.000000 yplib-1.6.2/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 01:13:57.147895 yplib-1.6.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.6.3/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-19 01:13:57.147395 yplib-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.6.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 01:13:57.148394 yplib-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-19 01:13:54.000000 yplib-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:13:57.144175 yplib-1.6.3/yplib/
+-rw-rw-rw-   0        0        0      350 2023-06-19 01:01:06.000000 yplib-1.6.3/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11378 2023-06-16 08:54:15.000000 yplib-1.6.3/yplib/chart.py
+-rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.6.3/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.6.3/yplib/file.py
+-rw-rw-rw-   0        0        0     1577 2023-06-19 01:13:34.000000 yplib-1.6.3/yplib/http_util.py
+-rw-rw-rw-   0        0        0    24344 2023-06-19 00:55:36.000000 yplib-1.6.3/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:13:57.146546 yplib-1.6.3/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-19 01:13:57.000000 yplib-1.6.3/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-19 01:13:57.000000 yplib-1.6.3/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 01:13:57.000000 yplib-1.6.3/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 01:13:57.000000 yplib-1.6.3/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.6.2/LICENSE` & `yplib-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.6.2/setup.py` & `yplib-1.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.6.2",
+  version="1.6.3",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.6.2/yplib/chart.py` & `yplib-1.6.3/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.2/yplib/chart_html.py` & `yplib-1.6.3/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.2/yplib/file.py` & `yplib-1.6.3/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.2/yplib/index.py` & `yplib-1.6.3/yplib/index.py`

 * *Files identical despite different names*

