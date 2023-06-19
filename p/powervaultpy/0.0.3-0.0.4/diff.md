# Comparing `tmp/powervaultpy-0.0.3.tar.gz` & `tmp/powervaultpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powervaultpy-0.0.3.tar", last modified: Sat Jun 17 23:28:40 2023, max compression
+gzip compressed data, was "powervaultpy-0.0.4.tar", last modified: Mon Jun 19 00:14:18 2023, max compression
```

## Comparing `powervaultpy-0.0.3.tar` & `powervaultpy-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-17 23:28:40.969420 powervaultpy-0.0.3/
--rw-r--r--   0 adam       (501) staff       (20)      701 2023-06-17 23:28:40.968971 powervaultpy-0.0.3/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     1468 2023-06-17 23:28:21.000000 powervaultpy-0.0.3/pyproject.toml
--rw-r--r--   0 adam       (501) staff       (20)       38 2023-06-17 23:28:40.969562 powervaultpy-0.0.3/setup.cfg
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-17 23:28:40.963018 powervaultpy-0.0.3/src/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-17 23:28:40.965095 powervaultpy-0.0.3/src/powervaultpy/
--rw-r--r--   0 adam       (501) staff       (20)       47 2023-06-17 23:03:23.000000 powervaultpy-0.0.3/src/powervaultpy/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)     3222 2023-06-17 23:26:40.000000 powervaultpy-0.0.3/src/powervaultpy/powervault.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-17 23:28:40.968230 powervaultpy-0.0.3/src/powervaultpy.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)      701 2023-06-17 23:28:40.000000 powervaultpy-0.0.3/src/powervaultpy.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      273 2023-06-17 23:28:40.000000 powervaultpy-0.0.3/src/powervaultpy.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-06-17 23:28:40.000000 powervaultpy-0.0.3/src/powervaultpy.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)       94 2023-06-17 23:28:40.000000 powervaultpy-0.0.3/src/powervaultpy.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)       13 2023-06-17 23:28:40.000000 powervaultpy-0.0.3/src/powervaultpy.egg-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-19 00:14:18.740920 powervaultpy-0.0.4/
+-rw-r--r--   0 adam       (501) staff       (20)      701 2023-06-19 00:14:18.740512 powervaultpy-0.0.4/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     1478 2023-06-19 00:08:35.000000 powervaultpy-0.0.4/pyproject.toml
+-rw-r--r--   0 adam       (501) staff       (20)       38 2023-06-19 00:14:18.741030 powervaultpy-0.0.4/setup.cfg
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-19 00:14:18.726480 powervaultpy-0.0.4/src/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-19 00:14:18.729976 powervaultpy-0.0.4/src/powervaultpy/
+-rw-r--r--   0 adam       (501) staff       (20)       47 2023-06-17 23:03:23.000000 powervaultpy-0.0.4/src/powervaultpy/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)     7249 2023-06-19 00:06:05.000000 powervaultpy-0.0.4/src/powervaultpy/powervault.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-19 00:14:18.739508 powervaultpy-0.0.4/src/powervaultpy.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)      701 2023-06-19 00:14:18.000000 powervaultpy-0.0.4/src/powervaultpy.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      273 2023-06-19 00:14:18.000000 powervaultpy-0.0.4/src/powervaultpy.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-06-19 00:14:18.000000 powervaultpy-0.0.4/src/powervaultpy.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)       99 2023-06-19 00:14:18.000000 powervaultpy-0.0.4/src/powervaultpy.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)       13 2023-06-19 00:14:18.000000 powervaultpy-0.0.4/src/powervaultpy.egg-info/top_level.txt
```

### Comparing `powervaultpy-0.0.3/PKG-INFO` & `powervaultpy-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powervaultpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: An integration to control the Powervault battery
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/powervaultpy
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/powervaultpy/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/powervaultpy/blob/main/CHANGELOG.md
 Keywords: powervault,home,automation
```

### Comparing `powervaultpy-0.0.3/pyproject.toml` & `powervaultpy-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "powervaultpy"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Adam McDonagh", email="adam@elitemonkey.net" },
 ]
 license = { text = "GPLv3" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: POSIX",
 ]
 keywords = ["powervault", "home", "automation"]
 dependencies = [
-  "requests >= 2.28"
+  "requests >= 2.28",
+  "pytz"
 ]
 description = "An integration to control the Powervault battery"
 readme = "README.md"
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `powervaultpy-0.0.3/src/powervaultpy.egg-info/PKG-INFO` & `powervaultpy-0.0.4/src/powervaultpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powervaultpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: An integration to control the Powervault battery
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/powervaultpy
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/powervaultpy/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/powervaultpy/blob/main/CHANGELOG.md
 Keywords: powervault,home,automation
```

