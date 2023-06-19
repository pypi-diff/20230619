# Comparing `tmp/elblog2dict-0.0.4.tar.gz` & `tmp/elblog2dict-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elblog2dict-0.0.4.tar", last modified: Mon Jun 19 09:11:41 2023, max compression
+gzip compressed data, was "elblog2dict-0.0.5.tar", last modified: Mon Jun 19 09:56:10 2023, max compression
```

## Comparing `elblog2dict-0.0.4.tar` & `elblog2dict-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 09:11:41.584382 elblog2dict-0.0.4/
--rw-r--r--   0 jonghun    (501) staff       (20)     1036 2023-06-19 06:50:28.000000 elblog2dict-0.0.4/LICENSE
--rw-r--r--   0 jonghun    (501) staff       (20)      540 2023-06-19 09:11:41.584280 elblog2dict-0.0.4/PKG-INFO
--rw-r--r--   0 jonghun    (501) staff       (20)        6 2023-06-19 09:11:12.000000 elblog2dict-0.0.4/README.md
-drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 09:11:41.583441 elblog2dict-0.0.4/elblog2dict/
--rw-r--r--   0 jonghun    (501) staff       (20)       21 2023-06-19 09:11:04.000000 elblog2dict-0.0.4/elblog2dict/__init__.py
--rw-r--r--   0 jonghun    (501) staff       (20)     1490 2023-06-19 08:45:21.000000 elblog2dict-0.0.4/elblog2dict/parser.py
-drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 09:11:41.584133 elblog2dict-0.0.4/elblog2dict.egg-info/
--rw-r--r--   0 jonghun    (501) staff       (20)      540 2023-06-19 09:11:41.000000 elblog2dict-0.0.4/elblog2dict.egg-info/PKG-INFO
--rw-r--r--   0 jonghun    (501) staff       (20)      246 2023-06-19 09:11:41.000000 elblog2dict-0.0.4/elblog2dict.egg-info/SOURCES.txt
--rw-r--r--   0 jonghun    (501) staff       (20)        1 2023-06-19 09:11:41.000000 elblog2dict-0.0.4/elblog2dict.egg-info/dependency_links.txt
--rw-r--r--   0 jonghun    (501) staff       (20)        1 2023-06-19 09:11:41.000000 elblog2dict-0.0.4/elblog2dict.egg-info/not-zip-safe
--rw-r--r--   0 jonghun    (501) staff       (20)       12 2023-06-19 09:11:41.000000 elblog2dict-0.0.4/elblog2dict.egg-info/top_level.txt
--rw-r--r--   0 jonghun    (501) staff       (20)       38 2023-06-19 09:11:41.584416 elblog2dict-0.0.4/setup.cfg
--rw-r--r--   0 jonghun    (501) staff       (20)      780 2023-06-19 09:11:01.000000 elblog2dict-0.0.4/setup.py
+drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 09:56:10.818934 elblog2dict-0.0.5/
+-rw-r--r--   0 jonghun    (501) staff       (20)     1036 2023-06-19 06:50:28.000000 elblog2dict-0.0.5/LICENSE
+-rw-r--r--   0 jonghun    (501) staff       (20)      588 2023-06-19 09:56:10.818827 elblog2dict-0.0.5/PKG-INFO
+-rw-r--r--   0 jonghun    (501) staff       (20)        6 2023-06-19 09:11:12.000000 elblog2dict-0.0.5/README.md
+drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 09:56:10.818021 elblog2dict-0.0.5/elblog2dict/
+-rw-r--r--   0 jonghun    (501) staff       (20)       21 2023-06-19 09:56:08.000000 elblog2dict-0.0.5/elblog2dict/__init__.py
+-rw-r--r--   0 jonghun    (501) staff       (20)     1490 2023-06-19 08:45:21.000000 elblog2dict-0.0.5/elblog2dict/parser.py
+drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 09:56:10.818675 elblog2dict-0.0.5/elblog2dict.egg-info/
+-rw-r--r--   0 jonghun    (501) staff       (20)      588 2023-06-19 09:56:10.000000 elblog2dict-0.0.5/elblog2dict.egg-info/PKG-INFO
+-rw-r--r--   0 jonghun    (501) staff       (20)      246 2023-06-19 09:56:10.000000 elblog2dict-0.0.5/elblog2dict.egg-info/SOURCES.txt
+-rw-r--r--   0 jonghun    (501) staff       (20)        1 2023-06-19 09:56:10.000000 elblog2dict-0.0.5/elblog2dict.egg-info/dependency_links.txt
+-rw-r--r--   0 jonghun    (501) staff       (20)        1 2023-06-19 09:56:10.000000 elblog2dict-0.0.5/elblog2dict.egg-info/not-zip-safe
+-rw-r--r--   0 jonghun    (501) staff       (20)       12 2023-06-19 09:56:10.000000 elblog2dict-0.0.5/elblog2dict.egg-info/top_level.txt
+-rw-r--r--   0 jonghun    (501) staff       (20)       38 2023-06-19 09:56:10.818968 elblog2dict-0.0.5/setup.cfg
+-rw-r--r--   0 jonghun    (501) staff       (20)     1012 2023-06-19 09:56:04.000000 elblog2dict-0.0.5/setup.py
```

### Comparing `elblog2dict-0.0.4/LICENSE` & `elblog2dict-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `elblog2dict-0.0.4/PKG-INFO` & `elblog2dict-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: elblog2dict
-Version: 0.0.4
+Version: 0.0.5
 Summary: Utility for parsing and extracting data from ELB logs
 Home-page: https://github.com/leemhoon00/elblog2dict
 Author: leemhoon00
 Author-email: leemhoon000@gmail.com
 License: MIT
 Keywords: elb,log,parser,elblog2dict,regular expression
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# test
```

### Comparing `elblog2dict-0.0.4/elblog2dict/parser.py` & `elblog2dict-0.0.5/elblog2dict/parser.py`

 * *Files identical despite different names*

### Comparing `elblog2dict-0.0.4/elblog2dict.egg-info/PKG-INFO` & `elblog2dict-0.0.5/elblog2dict.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: elblog2dict
-Version: 0.0.4
+Version: 0.0.5
 Summary: Utility for parsing and extracting data from ELB logs
 Home-page: https://github.com/leemhoon00/elblog2dict
 Author: leemhoon00
 Author-email: leemhoon000@gmail.com
 License: MIT
 Keywords: elb,log,parser,elblog2dict,regular expression
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# test
```

