# Comparing `tmp/markapp-0.2.1.tar.gz` & `tmp/markapp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markapp-0.2.1.tar", last modified: Tue Jun 13 12:47:03 2023, max compression
+gzip compressed data, was "markapp-0.3.0.tar", last modified: Mon Jun 19 15:16:35 2023, max compression
```

## Comparing `markapp-0.2.1.tar` & `markapp-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 spierce   (1000) spierce   (1000)        0 2023-06-13 12:47:03.230563 markapp-0.2.1/
--rw-r--r--   0 spierce   (1000) spierce   (1000)     1069 2023-06-13 02:41:46.000000 markapp-0.2.1/LICENSE
--rw-r--r--   0 spierce   (1000) spierce   (1000)     1763 2023-06-13 12:47:03.230563 markapp-0.2.1/PKG-INFO
--rw-r--r--   0 spierce   (1000) spierce   (1000)     1334 2023-06-13 12:35:04.000000 markapp-0.2.1/README.md
--rw-r--r--   0 spierce   (1000) spierce   (1000)      460 2023-06-13 12:43:32.000000 markapp-0.2.1/pyproject.toml
--rw-r--r--   0 spierce   (1000) spierce   (1000)       38 2023-06-13 12:47:03.230563 markapp-0.2.1/setup.cfg
--rw-r--r--   0 spierce   (1000) spierce   (1000)      769 2023-06-13 12:44:43.000000 markapp-0.2.1/setup.py
-drwxr-xr-x   0 spierce   (1000) spierce   (1000)        0 2023-06-13 12:47:03.226562 markapp-0.2.1/src/
-drwxr-xr-x   0 spierce   (1000) spierce   (1000)        0 2023-06-13 12:47:03.230563 markapp-0.2.1/src/markapp/
--rw-r--r--   0 spierce   (1000) spierce   (1000)        0 2023-06-13 02:41:46.000000 markapp-0.2.1/src/markapp/__init__.py
--rw-r--r--   0 spierce   (1000) spierce   (1000)     1904 2023-06-13 12:42:10.000000 markapp-0.2.1/src/markapp/cli.py
--rw-r--r--   0 spierce   (1000) spierce   (1000)     1903 2023-06-13 12:08:15.000000 markapp-0.2.1/src/markapp/markapp.py
--rw-r--r--   0 spierce   (1000) spierce   (1000)     1336 2023-06-13 11:47:29.000000 markapp-0.2.1/src/markapp/watcher.py
-drwxr-xr-x   0 spierce   (1000) spierce   (1000)        0 2023-06-13 12:47:03.230563 markapp-0.2.1/src/markapp.egg-info/
--rw-r--r--   0 spierce   (1000) spierce   (1000)     1763 2023-06-13 12:47:03.000000 markapp-0.2.1/src/markapp.egg-info/PKG-INFO
--rw-r--r--   0 spierce   (1000) spierce   (1000)      342 2023-06-13 12:47:03.000000 markapp-0.2.1/src/markapp.egg-info/SOURCES.txt
--rw-r--r--   0 spierce   (1000) spierce   (1000)        1 2023-06-13 12:47:03.000000 markapp-0.2.1/src/markapp.egg-info/dependency_links.txt
--rw-r--r--   0 spierce   (1000) spierce   (1000)       44 2023-06-13 12:47:03.000000 markapp-0.2.1/src/markapp.egg-info/entry_points.txt
--rw-r--r--   0 spierce   (1000) spierce   (1000)       15 2023-06-13 12:47:03.000000 markapp-0.2.1/src/markapp.egg-info/requires.txt
--rw-r--r--   0 spierce   (1000) spierce   (1000)        8 2023-06-13 12:47:03.000000 markapp-0.2.1/src/markapp.egg-info/top_level.txt
+drwxr-xr-x   0 spierce   (1000) spierce   (1000)        0 2023-06-19 15:16:35.726273 markapp-0.3.0/
+-rw-r--r--   0 spierce   (1000) spierce   (1000)     1069 2023-06-13 02:41:46.000000 markapp-0.3.0/LICENSE
+-rw-r--r--   0 spierce   (1000) spierce   (1000)     1763 2023-06-19 15:16:35.722272 markapp-0.3.0/PKG-INFO
+-rw-r--r--   0 spierce   (1000) spierce   (1000)     1334 2023-06-13 12:35:04.000000 markapp-0.3.0/README.md
+-rw-r--r--   0 spierce   (1000) spierce   (1000)      460 2023-06-19 15:01:38.000000 markapp-0.3.0/pyproject.toml
+-rw-r--r--   0 spierce   (1000) spierce   (1000)       38 2023-06-19 15:16:35.726273 markapp-0.3.0/setup.cfg
+-rw-r--r--   0 spierce   (1000) spierce   (1000)      769 2023-06-19 15:01:32.000000 markapp-0.3.0/setup.py
+drwxr-xr-x   0 spierce   (1000) spierce   (1000)        0 2023-06-19 15:16:35.718272 markapp-0.3.0/src/
+drwxr-xr-x   0 spierce   (1000) spierce   (1000)        0 2023-06-19 15:16:35.722272 markapp-0.3.0/src/markapp/
+-rw-r--r--   0 spierce   (1000) spierce   (1000)        0 2023-06-13 02:41:46.000000 markapp-0.3.0/src/markapp/__init__.py
+-rw-r--r--   0 spierce   (1000) spierce   (1000)     1904 2023-06-13 12:42:10.000000 markapp-0.3.0/src/markapp/cli.py
+-rw-r--r--   0 spierce   (1000) spierce   (1000)     3058 2023-06-19 14:58:57.000000 markapp-0.3.0/src/markapp/markapp.py
+-rw-r--r--   0 spierce   (1000) spierce   (1000)     1336 2023-06-13 11:47:29.000000 markapp-0.3.0/src/markapp/watcher.py
+drwxr-xr-x   0 spierce   (1000) spierce   (1000)        0 2023-06-19 15:16:35.722272 markapp-0.3.0/src/markapp.egg-info/
+-rw-r--r--   0 spierce   (1000) spierce   (1000)     1763 2023-06-19 15:16:35.000000 markapp-0.3.0/src/markapp.egg-info/PKG-INFO
+-rw-r--r--   0 spierce   (1000) spierce   (1000)      342 2023-06-19 15:16:35.000000 markapp-0.3.0/src/markapp.egg-info/SOURCES.txt
+-rw-r--r--   0 spierce   (1000) spierce   (1000)        1 2023-06-19 15:16:35.000000 markapp-0.3.0/src/markapp.egg-info/dependency_links.txt
+-rw-r--r--   0 spierce   (1000) spierce   (1000)       44 2023-06-19 15:16:35.000000 markapp-0.3.0/src/markapp.egg-info/entry_points.txt
+-rw-r--r--   0 spierce   (1000) spierce   (1000)       15 2023-06-19 15:16:35.000000 markapp-0.3.0/src/markapp.egg-info/requires.txt
+-rw-r--r--   0 spierce   (1000) spierce   (1000)        8 2023-06-19 15:16:35.000000 markapp-0.3.0/src/markapp.egg-info/top_level.txt
```

### Comparing `markapp-0.2.1/LICENSE` & `markapp-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `markapp-0.2.1/PKG-INFO` & `markapp-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markapp
-Version: 0.2.1
+Version: 0.3.0
 Summary: A simple markdown to HTML compiler
 Home-page: https://github.com/ddrscott/markapp
 Author: Scott Pierce
 Author-email: ddrscott@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `markapp-0.2.1/README.md` & `markapp-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `markapp-0.2.1/setup.py` & `markapp-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='markapp',
-    version='0.2.1',
+    version='0.3.0',
     author='Scott Pierce',
     author_email='ddrscott@gmail.com',
     description='A simple markdown to HTML compiler',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ddrscott/markapp',
     packages=['markapp'],
```

### Comparing `markapp-0.2.1/src/markapp/cli.py` & `markapp-0.3.0/src/markapp/cli.py`

 * *Files identical despite different names*

### Comparing `markapp-0.2.1/src/markapp/watcher.py` & `markapp-0.3.0/src/markapp/watcher.py`

 * *Files identical despite different names*

### Comparing `markapp-0.2.1/src/markapp.egg-info/PKG-INFO` & `markapp-0.3.0/src/markapp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markapp
-Version: 0.2.1
+Version: 0.3.0
 Summary: A simple markdown to HTML compiler
 Home-page: https://github.com/ddrscott/markapp
 Author: Scott Pierce
 Author-email: ddrscott@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

