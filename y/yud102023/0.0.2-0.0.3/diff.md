# Comparing `tmp/yud102023-0.0.2.tar.gz` & `tmp/yud102023-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yud102023-0.0.2.tar", last modified: Mon Jun 19 00:37:49 2023, max compression
+gzip compressed data, was "yud102023-0.0.3.tar", last modified: Mon Jun 19 00:45:25 2023, max compression
```

## Comparing `yud102023-0.0.2.tar` & `yud102023-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 00:37:49.353753 yud102023-0.0.2/
--rw-r--r--   0 tomereliel   (501) staff       (20)     1054 2023-06-18 22:55:32.000000 yud102023-0.0.2/LICENSE
--rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-19 00:37:49.353612 yud102023-0.0.2/PKG-INFO
--rw-r--r--   0 tomereliel   (501) staff       (20)       49 2023-06-18 22:56:17.000000 yud102023-0.0.2/README.md
--rw-r--r--   0 tomereliel   (501) staff       (20)      600 2023-06-19 00:36:30.000000 yud102023-0.0.2/pyproject.toml
--rw-r--r--   0 tomereliel   (501) staff       (20)       38 2023-06-19 00:37:49.353801 yud102023-0.0.2/setup.cfg
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 00:37:49.351364 yud102023-0.0.2/src/
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 00:37:49.352813 yud102023-0.0.2/src/yud102023/
--rw-r--r--   0 tomereliel   (501) staff       (20)    29940 2023-06-18 23:00:03.000000 yud102023-0.0.2/src/yud102023/goodbye.py
--rw-r--r--   0 tomereliel   (501) staff       (20)        0 2023-06-14 14:29:08.000000 yud102023-0.0.2/src/yud102023/init.py
-drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 00:37:49.353392 yud102023-0.0.2/src/yud102023.egg-info/
--rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-19 00:37:49.000000 yud102023-0.0.2/src/yud102023.egg-info/PKG-INFO
--rw-r--r--   0 tomereliel   (501) staff       (20)      227 2023-06-19 00:37:49.000000 yud102023-0.0.2/src/yud102023.egg-info/SOURCES.txt
--rw-r--r--   0 tomereliel   (501) staff       (20)        1 2023-06-19 00:37:49.000000 yud102023-0.0.2/src/yud102023.egg-info/dependency_links.txt
--rw-r--r--   0 tomereliel   (501) staff       (20)       10 2023-06-19 00:37:49.000000 yud102023-0.0.2/src/yud102023.egg-info/top_level.txt
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 00:45:25.636767 yud102023-0.0.3/
+-rw-r--r--   0 tomereliel   (501) staff       (20)     1054 2023-06-18 22:55:32.000000 yud102023-0.0.3/LICENSE
+-rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-19 00:45:25.636611 yud102023-0.0.3/PKG-INFO
+-rw-r--r--   0 tomereliel   (501) staff       (20)       49 2023-06-18 22:56:17.000000 yud102023-0.0.3/README.md
+-rw-r--r--   0 tomereliel   (501) staff       (20)      633 2023-06-19 00:45:13.000000 yud102023-0.0.3/pyproject.toml
+-rw-r--r--   0 tomereliel   (501) staff       (20)       38 2023-06-19 00:45:25.636819 yud102023-0.0.3/setup.cfg
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 00:45:25.634178 yud102023-0.0.3/src/
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 00:45:25.635678 yud102023-0.0.3/src/yud102023/
+-rw-r--r--   0 tomereliel   (501) staff       (20)    29940 2023-06-18 23:00:03.000000 yud102023-0.0.3/src/yud102023/goodbye.py
+-rw-r--r--   0 tomereliel   (501) staff       (20)        0 2023-06-14 14:29:08.000000 yud102023-0.0.3/src/yud102023/init.py
+drwxr-xr-x   0 tomereliel   (501) staff       (20)        0 2023-06-19 00:45:25.636374 yud102023-0.0.3/src/yud102023.egg-info/
+-rw-r--r--   0 tomereliel   (501) staff       (20)      578 2023-06-19 00:45:25.000000 yud102023-0.0.3/src/yud102023.egg-info/PKG-INFO
+-rw-r--r--   0 tomereliel   (501) staff       (20)      263 2023-06-19 00:45:25.000000 yud102023-0.0.3/src/yud102023.egg-info/SOURCES.txt
+-rw-r--r--   0 tomereliel   (501) staff       (20)        1 2023-06-19 00:45:25.000000 yud102023-0.0.3/src/yud102023.egg-info/dependency_links.txt
+-rw-r--r--   0 tomereliel   (501) staff       (20)        9 2023-06-19 00:45:25.000000 yud102023-0.0.3/src/yud102023.egg-info/requires.txt
+-rw-r--r--   0 tomereliel   (501) staff       (20)       10 2023-06-19 00:45:25.000000 yud102023-0.0.3/src/yud102023.egg-info/top_level.txt
```

### Comparing `yud102023-0.0.2/LICENSE` & `yud102023-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yud102023-0.0.2/PKG-INFO` & `yud102023-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yud102023
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small creactive goodbye project for my students
 Author-email: Tomereliel <tomereliel.dev@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yud102023-0.0.2/src/yud102023/goodbye.py` & `yud102023-0.0.3/src/yud102023/goodbye.py`

 * *Files identical despite different names*

### Comparing `yud102023-0.0.2/src/yud102023.egg-info/PKG-INFO` & `yud102023-0.0.3/src/yud102023.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yud102023
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small creactive goodbye project for my students
 Author-email: Tomereliel <tomereliel.dev@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

