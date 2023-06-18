# Comparing `tmp/adaptivecard-0.0.6.tar.gz` & `tmp/adaptivecard-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptivecard-0.0.6.tar", last modified: Fri Sep 23 08:07:46 2022, max compression
+gzip compressed data, was "adaptivecard-0.0.7.tar", last modified: Sun Jun 18 22:03:20 2023, max compression
```

## Comparing `adaptivecard-0.0.6.tar` & `adaptivecard-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 cabutchei  (1000) cabutchei  (1000)        0 2022-09-23 08:07:46.139469 adaptivecard-0.0.6/
--rw-rw-r--   0 cabutchei  (1000) cabutchei  (1000)      607 2022-09-23 08:07:46.139469 adaptivecard-0.0.6/PKG-INFO
--rwxrwxrwx   0 cabutchei  (1000) cabutchei  (1000)       87 2022-05-26 18:45:12.000000 adaptivecard-0.0.6/README.md
-drwxrwxr-x   0 cabutchei  (1000) cabutchei  (1000)        0 2022-09-23 08:07:46.139469 adaptivecard-0.0.6/adaptivecard/
--rw-rw-r--   0 cabutchei  (1000) cabutchei  (1000)        0 2022-09-23 06:21:59.000000 adaptivecard-0.0.6/adaptivecard/__init__.py
--rwxrwxrwx   0 cabutchei  (1000) cabutchei  (1000)     6577 2022-09-23 08:06:55.000000 adaptivecard-0.0.6/adaptivecard/classes.py
--rwxrwxrwx   0 cabutchei  (1000) cabutchei  (1000)       46 2022-09-23 06:10:21.000000 adaptivecard-0.0.6/adaptivecard/exceptions.py
--rw-rw-r--   0 cabutchei  (1000) cabutchei  (1000)     3758 2022-09-23 07:13:25.000000 adaptivecard-0.0.6/adaptivecard/mixin.py
-drwxrwxr-x   0 cabutchei  (1000) cabutchei  (1000)        0 2022-09-23 08:07:46.139469 adaptivecard-0.0.6/adaptivecard.egg-info/
--rw-rw-r--   0 cabutchei  (1000) cabutchei  (1000)      607 2022-09-23 08:07:45.000000 adaptivecard-0.0.6/adaptivecard.egg-info/PKG-INFO
--rw-rw-r--   0 cabutchei  (1000) cabutchei  (1000)      260 2022-09-23 08:07:46.000000 adaptivecard-0.0.6/adaptivecard.egg-info/SOURCES.txt
--rw-rw-r--   0 cabutchei  (1000) cabutchei  (1000)        1 2022-09-23 08:07:45.000000 adaptivecard-0.0.6/adaptivecard.egg-info/dependency_links.txt
--rw-rw-r--   0 cabutchei  (1000) cabutchei  (1000)       13 2022-09-23 08:07:46.000000 adaptivecard-0.0.6/adaptivecard.egg-info/top_level.txt
--rw-rw-r--   0 cabutchei  (1000) cabutchei  (1000)       38 2022-09-23 08:07:46.139469 adaptivecard-0.0.6/setup.cfg
--rw-rw-r--   0 cabutchei  (1000) cabutchei  (1000)      857 2022-09-23 08:07:08.000000 adaptivecard-0.0.6/setup.py
+drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-06-18 22:03:20.233253 adaptivecard-0.0.7/
+-rw-r--r--   0 cabutchei   (501) staff       (20)      600 2023-06-18 22:03:20.233014 adaptivecard-0.0.7/PKG-INFO
+-rwxr-xr-x   0 cabutchei   (501) staff       (20)       87 2023-04-12 20:17:53.000000 adaptivecard-0.0.7/README.md
+drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-06-18 22:03:20.231832 adaptivecard-0.0.7/adaptivecard/
+-rw-r--r--   0 cabutchei   (501) staff       (20)        0 2023-06-18 19:00:27.000000 adaptivecard-0.0.7/adaptivecard/__init__.py
+-rwxr-xr-x   0 cabutchei   (501) staff       (20)    15621 2023-06-18 21:56:27.000000 adaptivecard-0.0.7/adaptivecard/classes.py
+-rwxr-xr-x   0 cabutchei   (501) staff       (20)       46 2023-04-12 20:17:53.000000 adaptivecard-0.0.7/adaptivecard/exceptions.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)     1610 2023-06-18 21:56:27.000000 adaptivecard-0.0.7/adaptivecard/mixin.py
+drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-06-18 22:03:20.232748 adaptivecard-0.0.7/adaptivecard.egg-info/
+-rw-r--r--   0 cabutchei   (501) staff       (20)      600 2023-06-18 22:03:20.000000 adaptivecard-0.0.7/adaptivecard.egg-info/PKG-INFO
+-rw-r--r--   0 cabutchei   (501) staff       (20)      260 2023-06-18 22:03:20.000000 adaptivecard-0.0.7/adaptivecard.egg-info/SOURCES.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)        1 2023-06-18 22:03:20.000000 adaptivecard-0.0.7/adaptivecard.egg-info/dependency_links.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)       13 2023-06-18 22:03:20.000000 adaptivecard-0.0.7/adaptivecard.egg-info/top_level.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)       38 2023-06-18 22:03:20.233318 adaptivecard-0.0.7/setup.cfg
+-rw-r--r--   0 cabutchei   (501) staff       (20)      886 2023-06-18 21:58:28.000000 adaptivecard-0.0.7/setup.py
```

### Comparing `adaptivecard-0.0.6/setup.py` & `adaptivecard-0.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from re import L
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Microsoft Adaptive Cards'
-LONG_DESCRIPTION = 'A package that helps you create adaptive cards.'
+LONG_DESCRIPTION = 'A package that helps you design adaptive cards in an object-oriented manner.'
 
 setup(
     name="adaptivecard",
     version=VERSION,
     author="cabutchei (Luan Paz)",
     author_email="<luropa_paz@hotmail.com>",
     description=DESCRIPTION,
```

