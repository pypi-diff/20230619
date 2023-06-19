# Comparing `tmp/LibKaleidoscope-1.3.1-3830370.tar.gz` & `tmp/LibKaleidoscope-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LibKaleidoscope-1.3.1.tar", last modified: Mon Jun 19 17:28:29 2023, max compression
+gzip compressed data, was "LibKaleidoscope-1.4.0.tar", last modified: Mon Jun 19 17:46:46 2023, max compression
```

## Comparing `LibKaleidoscope-1.3.1-3830370.tar` & `LibKaleidoscope-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)        0 2023-06-19 17:28:29.974163 LibKaleidoscope-1.3.1/
-drwxr-xr-x   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)        0 2023-06-19 17:28:29.974163 LibKaleidoscope-1.3.1/LibKaleidoscope.egg-info/
--rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)     6559 2023-06-19 17:28:29.000000 LibKaleidoscope-1.3.1/LibKaleidoscope.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)      321 2023-06-19 17:28:29.000000 LibKaleidoscope-1.3.1/LibKaleidoscope.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)        1 2023-06-19 17:28:29.000000 LibKaleidoscope-1.3.1/LibKaleidoscope.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)       13 2023-06-19 17:28:29.000000 LibKaleidoscope-1.3.1/LibKaleidoscope.egg-info/top_level.txt
--rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)      151 2023-06-19 17:28:21.000000 LibKaleidoscope-1.3.1/MANIFEST.in
--rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)     6559 2023-06-19 17:28:29.974163 LibKaleidoscope-1.3.1/PKG-INFO
--rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)     5669 2023-06-19 17:28:21.000000 LibKaleidoscope-1.3.1/README.md
--rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)      384 2023-06-19 17:28:21.000000 LibKaleidoscope-1.3.1/kaleidoscope-config.h
--rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)     9812 2023-06-19 17:28:21.000000 LibKaleidoscope-1.3.1/kaleidoscope.c
--rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)   169987 2023-06-19 17:28:29.000000 LibKaleidoscope-1.3.1/kaleidoscope.cpp
--rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)     3777 2023-06-19 17:28:21.000000 LibKaleidoscope-1.3.1/kaleidoscope.h
--rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)     1773 2023-06-19 17:28:21.000000 LibKaleidoscope-1.3.1/kaleidoscope.hpp
--rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)      299 2023-06-19 17:28:21.000000 LibKaleidoscope-1.3.1/kaleidoscope.pxd
--rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)      624 2023-06-19 17:28:21.000000 LibKaleidoscope-1.3.1/kaleidoscope.pyx
--rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)      100 2023-06-19 17:28:21.000000 LibKaleidoscope-1.3.1/pyproject.toml
--rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)       38 2023-06-19 17:28:29.974163 LibKaleidoscope-1.3.1/setup.cfg
--rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)     1248 2023-06-19 17:28:21.000000 LibKaleidoscope-1.3.1/setup.py
+drwxr-xr-x   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)        0 2023-06-19 17:46:46.813812 LibKaleidoscope-1.4.0/
+drwxr-xr-x   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)        0 2023-06-19 17:46:46.813812 LibKaleidoscope-1.4.0/LibKaleidoscope.egg-info/
+-rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)     6559 2023-06-19 17:46:46.000000 LibKaleidoscope-1.4.0/LibKaleidoscope.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)      321 2023-06-19 17:46:46.000000 LibKaleidoscope-1.4.0/LibKaleidoscope.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)        1 2023-06-19 17:46:46.000000 LibKaleidoscope-1.4.0/LibKaleidoscope.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)       13 2023-06-19 17:46:46.000000 LibKaleidoscope-1.4.0/LibKaleidoscope.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)      151 2023-06-19 17:46:24.000000 LibKaleidoscope-1.4.0/MANIFEST.in
+-rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)     6559 2023-06-19 17:46:46.813812 LibKaleidoscope-1.4.0/PKG-INFO
+-rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)     5669 2023-06-19 17:46:24.000000 LibKaleidoscope-1.4.0/README.md
+-rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)      384 2023-06-19 17:46:43.000000 LibKaleidoscope-1.4.0/kaleidoscope-config.h
+-rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)     9812 2023-06-19 17:46:24.000000 LibKaleidoscope-1.4.0/kaleidoscope.c
+-rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)   169987 2023-06-19 17:46:46.000000 LibKaleidoscope-1.4.0/kaleidoscope.cpp
+-rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)     3777 2023-06-19 17:46:24.000000 LibKaleidoscope-1.4.0/kaleidoscope.h
+-rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)     1773 2023-06-19 17:46:24.000000 LibKaleidoscope-1.4.0/kaleidoscope.hpp
+-rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)      299 2023-06-19 17:46:24.000000 LibKaleidoscope-1.4.0/kaleidoscope.pxd
+-rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)      624 2023-06-19 17:46:24.000000 LibKaleidoscope-1.4.0/kaleidoscope.pyx
+-rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)      100 2023-06-19 17:46:24.000000 LibKaleidoscope-1.4.0/pyproject.toml
+-rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)       38 2023-06-19 17:46:46.813812 LibKaleidoscope-1.4.0/setup.cfg
+-rw-r--r--   0 ubuntu-wsl  (1000) ubuntu-wsl  (1000)     1248 2023-06-19 17:46:43.000000 LibKaleidoscope-1.4.0/setup.py
```

### Comparing `LibKaleidoscope-1.3.1/LibKaleidoscope.egg-info/PKG-INFO` & `LibKaleidoscope-1.4.0/LibKaleidoscope.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LibKaleidoscope
-Version: 1.3.1
+Version: 1.4.0
 Summary: A library to create kaleidoscope effect on images.
 Home-page: https://egecetin.github.io/libKaleidoscope/
 Download-URL: https://github.com/egecetin/libKaleidoscope/releases
 Author: egecetin
 Author-email: egecetin@hotmail.com.tr
 Maintainer: egecetin
 Maintainer-email: egecetin@hotmail.com.tr
```

### Comparing `LibKaleidoscope-1.3.1/PKG-INFO` & `LibKaleidoscope-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LibKaleidoscope
-Version: 1.3.1
+Version: 1.4.0
 Summary: A library to create kaleidoscope effect on images.
 Home-page: https://egecetin.github.io/libKaleidoscope/
 Download-URL: https://github.com/egecetin/libKaleidoscope/releases
 Author: egecetin
 Author-email: egecetin@hotmail.com.tr
 Maintainer: egecetin
 Maintainer-email: egecetin@hotmail.com.tr
```

### Comparing `LibKaleidoscope-1.3.1/README.md` & `LibKaleidoscope-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `LibKaleidoscope-1.3.1/kaleidoscope.c` & `LibKaleidoscope-1.4.0/kaleidoscope.c`

 * *Files identical despite different names*

### Comparing `LibKaleidoscope-1.3.1/kaleidoscope.cpp` & `LibKaleidoscope-1.4.0/kaleidoscope.cpp`

 * *Files identical despite different names*

### Comparing `LibKaleidoscope-1.3.1/kaleidoscope.h` & `LibKaleidoscope-1.4.0/kaleidoscope.h`

 * *Files identical despite different names*

### Comparing `LibKaleidoscope-1.3.1/kaleidoscope.hpp` & `LibKaleidoscope-1.4.0/kaleidoscope.hpp`

 * *Files identical despite different names*

### Comparing `LibKaleidoscope-1.3.1/kaleidoscope.pyx` & `LibKaleidoscope-1.4.0/kaleidoscope.pyx`

 * *Files identical despite different names*

### Comparing `LibKaleidoscope-1.3.1/setup.py` & `LibKaleidoscope-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from Cython.Build import cythonize
 
 long_description = open("README.md").read()
 
 setup(
     name= "LibKaleidoscope",
-    version= "1.3.1",
+    version= "1.4.0",
     description= "A library to create kaleidoscope effect on images.",
     long_description= long_description,
     long_description_content_type= "text/markdown",
     author= "egecetin",
     author_email = "egecetin@hotmail.com.tr",
     maintainer= "egecetin",
     maintainer_email= "egecetin@hotmail.com.tr",
```

