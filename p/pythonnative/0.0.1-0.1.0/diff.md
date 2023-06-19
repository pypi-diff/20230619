# Comparing `tmp/pythonnative-0.0.1.tar.gz` & `tmp/pythonnative-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonnative-0.0.1.tar", last modified: Wed Jun 14 19:55:15 2023, max compression
+gzip compressed data, was "pythonnative-0.1.0.tar", last modified: Mon Jun 19 01:44:37 2023, max compression
```

## Comparing `pythonnative-0.0.1.tar` & `pythonnative-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,26 @@
-drwxr-xr-x   0 owenthcarey   (501) staff       (20)        0 2023-06-14 19:55:15.509298 pythonnative-0.0.1/
--rw-r--r--   0 owenthcarey   (501) staff       (20)     1068 2023-06-14 18:55:42.000000 pythonnative-0.0.1/LICENSE
--rw-r--r--   0 owenthcarey   (501) staff       (20)     1242 2023-06-14 19:55:15.508495 pythonnative-0.0.1/PKG-INFO
--rw-r--r--   0 owenthcarey   (501) staff       (20)      800 2023-06-14 19:47:55.000000 pythonnative-0.0.1/README.md
-drwxr-xr-x   0 owenthcarey   (501) staff       (20)        0 2023-06-14 19:55:15.503115 pythonnative-0.0.1/pythonnative/
--rw-r--r--   0 owenthcarey   (501) staff       (20)        0 2023-06-14 16:22:09.000000 pythonnative-0.0.1/pythonnative/__init__.py
--rw-r--r--   0 owenthcarey   (501) staff       (20)     1996 2023-06-14 19:25:55.000000 pythonnative-0.0.1/pythonnative/pythonnative.py
-drwxr-xr-x   0 owenthcarey   (501) staff       (20)        0 2023-06-14 19:55:15.505920 pythonnative-0.0.1/pythonnative.egg-info/
--rw-r--r--   0 owenthcarey   (501) staff       (20)     1242 2023-06-14 19:55:15.000000 pythonnative-0.0.1/pythonnative.egg-info/PKG-INFO
--rw-r--r--   0 owenthcarey   (501) staff       (20)      304 2023-06-14 19:55:15.000000 pythonnative-0.0.1/pythonnative.egg-info/SOURCES.txt
--rw-r--r--   0 owenthcarey   (501) staff       (20)        1 2023-06-14 19:55:15.000000 pythonnative-0.0.1/pythonnative.egg-info/dependency_links.txt
--rw-r--r--   0 owenthcarey   (501) staff       (20)       27 2023-06-14 19:55:15.000000 pythonnative-0.0.1/pythonnative.egg-info/requires.txt
--rw-r--r--   0 owenthcarey   (501) staff       (20)       19 2023-06-14 19:55:15.000000 pythonnative-0.0.1/pythonnative.egg-info/top_level.txt
--rw-r--r--   0 owenthcarey   (501) staff       (20)       38 2023-06-14 19:55:15.509561 pythonnative-0.0.1/setup.cfg
--rw-r--r--   0 owenthcarey   (501) staff       (20)      719 2023-06-14 19:49:32.000000 pythonnative-0.0.1/setup.py
-drwxr-xr-x   0 owenthcarey   (501) staff       (20)        0 2023-06-14 19:55:15.507447 pythonnative-0.0.1/tests/
--rw-r--r--   0 owenthcarey   (501) staff       (20)        0 2023-06-14 16:22:18.000000 pythonnative-0.0.1/tests/__init__.py
--rw-r--r--   0 owenthcarey   (501) staff       (20)        0 2023-06-14 16:25:27.000000 pythonnative-0.0.1/tests/test_pythonnative.py
+drwxr-xr-x   0 owenthcarey   (501) staff       (20)        0 2023-06-19 01:44:37.914871 pythonnative-0.1.0/
+-rw-r--r--   0 owenthcarey   (501) staff       (20)     1068 2023-06-14 18:55:42.000000 pythonnative-0.1.0/LICENSE
+-rw-r--r--   0 owenthcarey   (501) staff       (20)     1242 2023-06-19 01:44:37.914128 pythonnative-0.1.0/PKG-INFO
+-rw-r--r--   0 owenthcarey   (501) staff       (20)      800 2023-06-14 19:47:55.000000 pythonnative-0.1.0/README.md
+drwxr-xr-x   0 owenthcarey   (501) staff       (20)        0 2023-06-19 01:44:37.901751 pythonnative-0.1.0/cli/
+-rw-r--r--   0 owenthcarey   (501) staff       (20)        0 2023-06-17 22:48:00.000000 pythonnative-0.1.0/cli/__init__.py
+-rw-r--r--   0 owenthcarey   (501) staff       (20)     3695 2023-06-18 20:32:40.000000 pythonnative-0.1.0/cli/pn.py
+drwxr-xr-x   0 owenthcarey   (501) staff       (20)        0 2023-06-19 01:44:37.907120 pythonnative-0.1.0/pythonnative/
+-rw-r--r--   0 owenthcarey   (501) staff       (20)      207 2023-06-18 21:47:47.000000 pythonnative-0.1.0/pythonnative/__init__.py
+-rw-r--r--   0 owenthcarey   (501) staff       (20)     1090 2023-06-18 21:42:02.000000 pythonnative-0.1.0/pythonnative/button.py
+-rw-r--r--   0 owenthcarey   (501) staff       (20)     1051 2023-06-18 21:42:20.000000 pythonnative-0.1.0/pythonnative/label.py
+-rw-r--r--   0 owenthcarey   (501) staff       (20)     1149 2023-06-18 21:45:51.000000 pythonnative-0.1.0/pythonnative/linear_layout.py
+-rw-r--r--   0 owenthcarey   (501) staff       (20)     1536 2023-06-18 21:44:29.000000 pythonnative-0.1.0/pythonnative/screen.py
+-rw-r--r--   0 owenthcarey   (501) staff       (20)      458 2023-06-18 22:03:41.000000 pythonnative-0.1.0/pythonnative/view.py
+drwxr-xr-x   0 owenthcarey   (501) staff       (20)        0 2023-06-19 01:44:37.911985 pythonnative-0.1.0/pythonnative.egg-info/
+-rw-r--r--   0 owenthcarey   (501) staff       (20)     1242 2023-06-19 01:44:37.000000 pythonnative-0.1.0/pythonnative.egg-info/PKG-INFO
+-rw-r--r--   0 owenthcarey   (501) staff       (20)      459 2023-06-19 01:44:37.000000 pythonnative-0.1.0/pythonnative.egg-info/SOURCES.txt
+-rw-r--r--   0 owenthcarey   (501) staff       (20)        1 2023-06-19 01:44:37.000000 pythonnative-0.1.0/pythonnative.egg-info/dependency_links.txt
+-rw-r--r--   0 owenthcarey   (501) staff       (20)       35 2023-06-19 01:44:37.000000 pythonnative-0.1.0/pythonnative.egg-info/entry_points.txt
+-rw-r--r--   0 owenthcarey   (501) staff       (20)       27 2023-06-19 01:44:37.000000 pythonnative-0.1.0/pythonnative.egg-info/requires.txt
+-rw-r--r--   0 owenthcarey   (501) staff       (20)       23 2023-06-19 01:44:37.000000 pythonnative-0.1.0/pythonnative.egg-info/top_level.txt
+-rw-r--r--   0 owenthcarey   (501) staff       (20)       38 2023-06-19 01:44:37.915132 pythonnative-0.1.0/setup.cfg
+-rw-r--r--   0 owenthcarey   (501) staff       (20)      815 2023-06-19 01:42:30.000000 pythonnative-0.1.0/setup.py
+drwxr-xr-x   0 owenthcarey   (501) staff       (20)        0 2023-06-19 01:44:37.913399 pythonnative-0.1.0/tests/
+-rw-r--r--   0 owenthcarey   (501) staff       (20)        0 2023-06-14 16:22:18.000000 pythonnative-0.1.0/tests/__init__.py
+-rw-r--r--   0 owenthcarey   (501) staff       (20)        0 2023-06-14 16:25:27.000000 pythonnative-0.1.0/tests/test_pythonnative.py
```

### Comparing `pythonnative-0.0.1/LICENSE` & `pythonnative-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pythonnative-0.0.1/PKG-INFO` & `pythonnative-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonnative
-Version: 0.0.1
+Version: 0.1.0
 Summary: A cross-platform Python tool kit for Android and iOS
 Home-page: https://pythonnative.com
 Author: Owen Carey
 Author-email: pythonnative@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pythonnative-0.0.1/README.md` & `pythonnative-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pythonnative-0.0.1/pythonnative.egg-info/PKG-INFO` & `pythonnative-0.1.0/pythonnative.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonnative
-Version: 0.0.1
+Version: 0.1.0
 Summary: A cross-platform Python tool kit for Android and iOS
 Home-page: https://pythonnative.com
 Author: Owen Carey
 Author-email: pythonnative@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pythonnative-0.0.1/setup.py` & `pythonnative-0.1.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pythonnative",
-    version="0.0.1",
+    version="0.1.0",
     author="Owen Carey",
     author_email="pythonnative@gmail.com",
     description="A cross-platform Python tool kit for Android and iOS",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://pythonnative.com",
     packages=find_packages(),
@@ -16,8 +16,13 @@
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
     install_requires=[
         "rubicon-objc>=0.4.6,<0.5.0",
         # Add more requirements here as necessary
     ],
+    entry_points={
+        "console_scripts": [
+            "pn=cli.pn:main",
+        ],
+    },
 )
```

