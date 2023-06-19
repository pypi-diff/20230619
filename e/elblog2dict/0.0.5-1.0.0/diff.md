# Comparing `tmp/elblog2dict-0.0.5.tar.gz` & `tmp/elblog2dict-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elblog2dict-0.0.5.tar", last modified: Mon Jun 19 09:56:10 2023, max compression
+gzip compressed data, was "elblog2dict-1.0.0.tar", last modified: Mon Jun 19 10:16:36 2023, max compression
```

## Comparing `elblog2dict-0.0.5.tar` & `elblog2dict-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 09:56:10.818934 elblog2dict-0.0.5/
--rw-r--r--   0 jonghun    (501) staff       (20)     1036 2023-06-19 06:50:28.000000 elblog2dict-0.0.5/LICENSE
--rw-r--r--   0 jonghun    (501) staff       (20)      588 2023-06-19 09:56:10.818827 elblog2dict-0.0.5/PKG-INFO
--rw-r--r--   0 jonghun    (501) staff       (20)        6 2023-06-19 09:11:12.000000 elblog2dict-0.0.5/README.md
-drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 09:56:10.818021 elblog2dict-0.0.5/elblog2dict/
--rw-r--r--   0 jonghun    (501) staff       (20)       21 2023-06-19 09:56:08.000000 elblog2dict-0.0.5/elblog2dict/__init__.py
--rw-r--r--   0 jonghun    (501) staff       (20)     1490 2023-06-19 08:45:21.000000 elblog2dict-0.0.5/elblog2dict/parser.py
-drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 09:56:10.818675 elblog2dict-0.0.5/elblog2dict.egg-info/
--rw-r--r--   0 jonghun    (501) staff       (20)      588 2023-06-19 09:56:10.000000 elblog2dict-0.0.5/elblog2dict.egg-info/PKG-INFO
--rw-r--r--   0 jonghun    (501) staff       (20)      246 2023-06-19 09:56:10.000000 elblog2dict-0.0.5/elblog2dict.egg-info/SOURCES.txt
--rw-r--r--   0 jonghun    (501) staff       (20)        1 2023-06-19 09:56:10.000000 elblog2dict-0.0.5/elblog2dict.egg-info/dependency_links.txt
--rw-r--r--   0 jonghun    (501) staff       (20)        1 2023-06-19 09:56:10.000000 elblog2dict-0.0.5/elblog2dict.egg-info/not-zip-safe
--rw-r--r--   0 jonghun    (501) staff       (20)       12 2023-06-19 09:56:10.000000 elblog2dict-0.0.5/elblog2dict.egg-info/top_level.txt
--rw-r--r--   0 jonghun    (501) staff       (20)       38 2023-06-19 09:56:10.818968 elblog2dict-0.0.5/setup.cfg
--rw-r--r--   0 jonghun    (501) staff       (20)     1012 2023-06-19 09:56:04.000000 elblog2dict-0.0.5/setup.py
+drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 10:16:36.822314 elblog2dict-1.0.0/
+-rw-r--r--   0 jonghun    (501) staff       (20)     1036 2023-06-19 06:50:28.000000 elblog2dict-1.0.0/LICENSE
+-rw-r--r--   0 jonghun    (501) staff       (20)     3267 2023-06-19 10:16:36.822206 elblog2dict-1.0.0/PKG-INFO
+-rw-r--r--   0 jonghun    (501) staff       (20)     2686 2023-06-19 10:15:19.000000 elblog2dict-1.0.0/README.md
+drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 10:16:36.821308 elblog2dict-1.0.0/elblog2dict/
+-rw-r--r--   0 jonghun    (501) staff       (20)       21 2023-06-19 10:16:04.000000 elblog2dict-1.0.0/elblog2dict/__init__.py
+-rw-r--r--   0 jonghun    (501) staff       (20)     1490 2023-06-19 08:45:21.000000 elblog2dict-1.0.0/elblog2dict/parser.py
+drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 10:16:36.822052 elblog2dict-1.0.0/elblog2dict.egg-info/
+-rw-r--r--   0 jonghun    (501) staff       (20)     3267 2023-06-19 10:16:36.000000 elblog2dict-1.0.0/elblog2dict.egg-info/PKG-INFO
+-rw-r--r--   0 jonghun    (501) staff       (20)      246 2023-06-19 10:16:36.000000 elblog2dict-1.0.0/elblog2dict.egg-info/SOURCES.txt
+-rw-r--r--   0 jonghun    (501) staff       (20)        1 2023-06-19 10:16:36.000000 elblog2dict-1.0.0/elblog2dict.egg-info/dependency_links.txt
+-rw-r--r--   0 jonghun    (501) staff       (20)        1 2023-06-19 10:16:36.000000 elblog2dict-1.0.0/elblog2dict.egg-info/not-zip-safe
+-rw-r--r--   0 jonghun    (501) staff       (20)       12 2023-06-19 10:16:36.000000 elblog2dict-1.0.0/elblog2dict.egg-info/top_level.txt
+-rw-r--r--   0 jonghun    (501) staff       (20)       38 2023-06-19 10:16:36.822353 elblog2dict-1.0.0/setup.cfg
+-rw-r--r--   0 jonghun    (501) staff       (20)     1012 2023-06-19 10:15:59.000000 elblog2dict-1.0.0/setup.py
```

### Comparing `elblog2dict-0.0.5/LICENSE` & `elblog2dict-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elblog2dict-0.0.5/elblog2dict/parser.py` & `elblog2dict-1.0.0/elblog2dict/parser.py`

 * *Files identical despite different names*

### Comparing `elblog2dict-0.0.5/setup.py` & `elblog2dict-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='elblog2dict',
-    version='0.0.5',
+    version='1.0.0',
     description='Utility for parsing and extracting data from ELB logs',
     author='leemhoon00',
     author_email='leemhoon000@gmail.com',
     url='https://github.com/leemhoon00/elblog2dict',
     install_requires=[],
     packages=find_packages(exclude=['.git', '.gitignore', '*.gz', 'test.py']),
     keywords=['elb', 'log', 'parser', 'elblog2dict', 'regular expression'],
```

