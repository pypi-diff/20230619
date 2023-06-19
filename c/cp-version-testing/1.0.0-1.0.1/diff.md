# Comparing `tmp/cp_version_testing-1.0.0.tar.gz` & `tmp/cp_version_testing-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cp_version_testing-1.0.0.tar", last modified: Mon Jun 19 17:15:47 2023, max compression
+gzip compressed data, was "cp_version_testing-1.0.1.tar", last modified: Mon Jun 19 17:20:31 2023, max compression
```

## Comparing `cp_version_testing-1.0.0.tar` & `cp_version_testing-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:15:47.836774 cp_version_testing-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-19 17:15:47.836774 cp_version_testing-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 17:15:39.000000 cp_version_testing-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:15:47.836774 cp_version_testing-1.0.0/cp_version_testing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-19 17:15:47.000000 cp_version_testing-1.0.0/cp_version_testing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-19 17:15:47.000000 cp_version_testing-1.0.0/cp_version_testing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 17:15:47.000000 cp_version_testing-1.0.0/cp_version_testing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 17:15:47.000000 cp_version_testing-1.0.0/cp_version_testing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 17:15:47.836774 cp_version_testing-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-19 17:15:39.000000 cp_version_testing-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:20:31.344240 cp_version_testing-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-19 17:20:31.344240 cp_version_testing-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 17:20:21.000000 cp_version_testing-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:20:31.344240 cp_version_testing-1.0.1/cp_version_testing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-19 17:20:31.000000 cp_version_testing-1.0.1/cp_version_testing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-19 17:20:31.000000 cp_version_testing-1.0.1/cp_version_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 17:20:31.000000 cp_version_testing-1.0.1/cp_version_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 17:20:31.000000 cp_version_testing-1.0.1/cp_version_testing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 17:20:31.344240 cp_version_testing-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-19 17:20:21.000000 cp_version_testing-1.0.1/setup.py
```

### Comparing `cp_version_testing-1.0.0/setup.py` & `cp_version_testing-1.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from setuptools import setup
 
 setup(
     name="cp_version_testing",
-    version="1.0.0",
+    version="1.0.1",
     author_email="roniz@checkpoint.com",
     author="Check Point",
     license='Apache 2.0',
     description="Check Point",
     long_description="Check Point",
     long_description_content_type="text/plain",
     url="https://github.com/CheckPointSW/",
```

