# Comparing `tmp/yud102023-0.0.1.tar.gz` & `tmp/yud102023-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yud102023-0.0.1.tar", last modified: Sun Jun 18 23:57:36 2023, max compression
+gzip compressed data, was "yud102023-0.0.2.tar", last modified: Mon Jun 19 00:37:49 2023, max compression
```

## Comparing `yud102023-0.0.1.tar` & `yud102023-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-18 23:57:36.027119 yud102023-0.0.1/
--rw-r--r--   0 tomereliel   (501) staff       (20)     1054 2023-06-18 22:55:32.000000 yud102023-0.0.1/LICENSE
--rw-r--r--   0 tomereliel   (501) staff       (20)      573 2023-06-18 23:57:36.027215 yud102023-0.0.1/PKG-INFO
--rw-r--r--   0 tomereliel   (501) staff       (20)       49 2023-06-18 22:56:17.000000 yud102023-0.0.1/README.md
--rw-r--r--   0 tomereliel   (501) staff       (20)       86 2023-06-18 23:41:47.000000 yud102023-0.0.1/pyproject.toml
--rw-r--r--   0 tomereliel   (501) staff       (20)      648 2023-06-18 23:57:36.027520 yud102023-0.0.1/setup.cfg
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-18 23:57:36.025392 yud102023-0.0.1/src/
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-18 23:57:36.026983 yud102023-0.0.1/src/yud102023.egg-info/
--rw-r--r--   0 tomereliel   (501) staff       (20)      573 2023-06-18 23:57:36.000000 yud102023-0.0.1/src/yud102023.egg-info/PKG-INFO
--rw-r--r--   0 tomereliel   (501) staff       (20)      190 2023-06-18 23:57:36.000000 yud102023-0.0.1/src/yud102023.egg-info/SOURCES.txt
--rw-r--r--   0 tomereliel   (501) staff       (20)        1 2023-06-18 23:57:36.000000 yud102023-0.0.1/src/yud102023.egg-info/dependency_links.txt
--rw-r--r--   0 tomereliel   (501) staff       (20)        1 2023-06-18 23:57:36.000000 yud102023-0.0.1/src/yud102023.egg-info/top_level.txt
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 00:37:49.353753 yud102023-0.0.2/
+-rw-r--r--   0 tomereliel   (501) staff       (20)     1054 2023-06-18 22:55:32.000000 yud102023-0.0.2/LICENSE
+-rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-19 00:37:49.353612 yud102023-0.0.2/PKG-INFO
+-rw-r--r--   0 tomereliel   (501) staff       (20)       49 2023-06-18 22:56:17.000000 yud102023-0.0.2/README.md
+-rw-r--r--   0 tomereliel   (501) staff       (20)      600 2023-06-19 00:36:30.000000 yud102023-0.0.2/pyproject.toml
+-rw-r--r--   0 tomereliel   (501) staff       (20)       38 2023-06-19 00:37:49.353801 yud102023-0.0.2/setup.cfg
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 00:37:49.351364 yud102023-0.0.2/src/
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 00:37:49.352813 yud102023-0.0.2/src/yud102023/
+-rw-r--r--   0 tomereliel   (501) staff       (20)    29940 2023-06-18 23:00:03.000000 yud102023-0.0.2/src/yud102023/goodbye.py
+-rw-r--r--   0 tomereliel   (501) staff       (20)        0 2023-06-14 14:29:08.000000 yud102023-0.0.2/src/yud102023/init.py
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 00:37:49.353392 yud102023-0.0.2/src/yud102023.egg-info/
+-rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-19 00:37:49.000000 yud102023-0.0.2/src/yud102023.egg-info/PKG-INFO
+-rw-r--r--   0 tomereliel   (501) staff       (20)      227 2023-06-19 00:37:49.000000 yud102023-0.0.2/src/yud102023.egg-info/SOURCES.txt
+-rw-r--r--   0 tomereliel   (501) staff       (20)        1 2023-06-19 00:37:49.000000 yud102023-0.0.2/src/yud102023.egg-info/dependency_links.txt
+-rw-r--r--   0 tomereliel   (501) staff       (20)       10 2023-06-19 00:37:49.000000 yud102023-0.0.2/src/yud102023.egg-info/top_level.txt
```

### Comparing `yud102023-0.0.1/LICENSE` & `yud102023-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yud102023-0.0.1/PKG-INFO` & `yud102023-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: yud102023
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small creactive goodbye project for my students
-Home-page: https://github.com/pypa/sampleproject
-Author: Tomer Eliel
-Author-email: tomereliel.dev@gmail.com
+Author-email: Tomereliel <tomereliel.dev@gmail.com>
+Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 A small creactive goodbye project for my students
```

### Comparing `yud102023-0.0.1/src/yud102023.egg-info/PKG-INFO` & `yud102023-0.0.2/src/yud102023.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: yud102023
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small creactive goodbye project for my students
-Home-page: https://github.com/pypa/sampleproject
-Author: Tomer Eliel
-Author-email: tomereliel.dev@gmail.com
+Author-email: Tomereliel <tomereliel.dev@gmail.com>
+Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 A small creactive goodbye project for my students
```

