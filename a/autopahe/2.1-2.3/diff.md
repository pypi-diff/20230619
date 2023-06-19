# Comparing `tmp/autopahe-2.1.tar.gz` & `tmp/autopahe-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopahe-2.1.tar", last modified: Mon Jun 19 20:30:56 2023, max compression
+gzip compressed data, was "autopahe-2.3.tar", last modified: Mon Jun 19 20:35:16 2023, max compression
```

## Comparing `autopahe-2.1.tar` & `autopahe-2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:30:56.031206 autopahe-2.1/
--rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       62 2023-06-16 06:52:54.000000 autopahe-2.1/MANIFEST.in
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6397 2023-06-19 20:30:56.027206 autopahe-2.1/PKG-INFO
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     5746 2023-06-19 20:04:44.000000 autopahe-2.1/README.md
-drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:30:56.027206 autopahe-2.1/autopahe/
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:29:36.000000 autopahe-2.1/autopahe/__init__.py
--rwxrwxr-x   0 haxsys    (1000) haxsys    (1000)    19650 2023-06-19 20:29:25.000000 autopahe-2.1/autopahe/auto_pahe.py
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     4392 2023-06-19 19:43:52.000000 autopahe-2.1/autopahe/kwikdown.py
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      248 2023-06-19 19:57:40.000000 autopahe-2.1/autopahe/test.py
-drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:30:56.027206 autopahe-2.1/autopahe.egg-info/
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6397 2023-06-19 20:30:55.000000 autopahe-2.1/autopahe.egg-info/PKG-INFO
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      337 2023-06-19 20:30:55.000000 autopahe-2.1/autopahe.egg-info/SOURCES.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        1 2023-06-19 20:30:55.000000 autopahe-2.1/autopahe.egg-info/dependency_links.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       56 2023-06-19 20:30:55.000000 autopahe-2.1/autopahe.egg-info/entry_points.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       95 2023-06-19 20:30:55.000000 autopahe-2.1/autopahe.egg-info/requires.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        9 2023-06-19 20:30:55.000000 autopahe-2.1/autopahe.egg-info/top_level.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       86 2023-06-16 07:47:47.000000 autopahe-2.1/pyproject.toml
--rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       98 2023-06-16 07:18:50.000000 autopahe-2.1/requirements.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       38 2023-06-19 20:30:56.031206 autopahe-2.1/setup.cfg
--rwxrwxr-x   0 haxsys    (1000) haxsys    (1000)     1374 2023-06-19 20:30:08.000000 autopahe-2.1/setup.py
+drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:35:16.434912 autopahe-2.3/
+-rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       62 2023-06-16 06:52:54.000000 autopahe-2.3/MANIFEST.in
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6397 2023-06-19 20:35:16.434912 autopahe-2.3/PKG-INFO
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     5746 2023-06-19 20:04:44.000000 autopahe-2.3/README.md
+drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:35:16.422911 autopahe-2.3/autopahe/
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:29:36.000000 autopahe-2.3/autopahe/__init__.py
+-rwxrwxr-x   0 haxsys    (1000) haxsys    (1000)    19650 2023-06-19 20:29:25.000000 autopahe-2.3/autopahe/auto_pahe.py
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     4392 2023-06-19 19:43:52.000000 autopahe-2.3/autopahe/kwikdown.py
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      248 2023-06-19 19:57:40.000000 autopahe-2.3/autopahe/test.py
+drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-19 20:35:16.434912 autopahe-2.3/autopahe.egg-info/
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     6397 2023-06-19 20:35:16.000000 autopahe-2.3/autopahe.egg-info/PKG-INFO
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      337 2023-06-19 20:35:16.000000 autopahe-2.3/autopahe.egg-info/SOURCES.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        1 2023-06-19 20:35:16.000000 autopahe-2.3/autopahe.egg-info/dependency_links.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       53 2023-06-19 20:35:16.000000 autopahe-2.3/autopahe.egg-info/entry_points.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       95 2023-06-19 20:35:16.000000 autopahe-2.3/autopahe.egg-info/requires.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        9 2023-06-19 20:35:16.000000 autopahe-2.3/autopahe.egg-info/top_level.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       86 2023-06-16 07:47:47.000000 autopahe-2.3/pyproject.toml
+-rwxrwxrwx   0 haxsys    (1000) haxsys    (1000)       98 2023-06-16 07:18:50.000000 autopahe-2.3/requirements.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       38 2023-06-19 20:35:16.434912 autopahe-2.3/setup.cfg
+-rwxrwxr-x   0 haxsys    (1000) haxsys    (1000)     1371 2023-06-19 20:34:31.000000 autopahe-2.3/setup.py
```

### Comparing `autopahe-2.1/PKG-INFO` & `autopahe-2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopahe
-Version: 2.1
+Version: 2.3
 Summary: A python script to automate downloads from animepahe
 Home-page: https://github.com/haxsysgit/autopahe
 Author: Elenasulu Arinze
 Author-email: pentacker@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `autopahe-2.1/README.md` & `autopahe-2.3/README.md`

 * *Files identical despite different names*

### Comparing `autopahe-2.1/autopahe/auto_pahe.py` & `autopahe-2.3/autopahe/auto_pahe.py`

 * *Files identical despite different names*

### Comparing `autopahe-2.1/autopahe/kwikdown.py` & `autopahe-2.3/autopahe/kwikdown.py`

 * *Files identical despite different names*

### Comparing `autopahe-2.1/autopahe.egg-info/PKG-INFO` & `autopahe-2.3/autopahe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopahe
-Version: 2.1
+Version: 2.3
 Summary: A python script to automate downloads from animepahe
 Home-page: https://github.com/haxsysgit/autopahe
 Author: Elenasulu Arinze
 Author-email: pentacker@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `autopahe-2.1/setup.py` & `autopahe-2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = 'autopahe',
-    version = '2.1',
+    version = '2.3',
     author_email="pentacker@gmail.com",
     description = "A python script to automate downloads from animepahe",
     url = "https://github.com/haxsysgit/autopahe",
     author = "Elenasulu Arinze",
     license = "MIT",
     py_modules = [
         'autopahe',
 
     ],
     package_dir = {'autopahe':'autopahe'},
     entry_points ={
-            'console_scripts': ['autopahe = autopahe.auto_pahe.py:main']
+            'console_scripts': ['autopahe = autopahe.auto_pahe:main']
     },
     include_package_data=True,
     packages = [
         "autopahe",
     ],
     python_requires = '>=3.7',
     install_requires = [
```

