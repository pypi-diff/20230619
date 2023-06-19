# Comparing `tmp/elblog2dict-0.0.3.tar.gz` & `tmp/elblog2dict-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elblog2dict-0.0.3.tar", last modified: Mon Jun 19 08:46:11 2023, max compression
+gzip compressed data, was "elblog2dict-0.0.4.tar", last modified: Mon Jun 19 09:11:41 2023, max compression
```

## Comparing `elblog2dict-0.0.3.tar` & `elblog2dict-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 08:46:11.798334 elblog2dict-0.0.3/
--rw-r--r--   0 jonghun    (501) staff       (20)     1036 2023-06-19 06:50:28.000000 elblog2dict-0.0.3/LICENSE
--rw-r--r--   0 jonghun    (501) staff       (20)      408 2023-06-19 08:46:11.798231 elblog2dict-0.0.3/PKG-INFO
--rw-r--r--   0 jonghun    (501) staff       (20)        0 2023-06-19 06:18:59.000000 elblog2dict-0.0.3/README.md
-drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 08:46:11.797572 elblog2dict-0.0.3/elblog2dict/
--rw-r--r--   0 jonghun    (501) staff       (20)       21 2023-06-19 08:45:58.000000 elblog2dict-0.0.3/elblog2dict/__init__.py
--rw-r--r--   0 jonghun    (501) staff       (20)     1490 2023-06-19 08:45:21.000000 elblog2dict-0.0.3/elblog2dict/parser.py
-drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 08:46:11.798080 elblog2dict-0.0.3/elblog2dict.egg-info/
--rw-r--r--   0 jonghun    (501) staff       (20)      408 2023-06-19 08:46:11.000000 elblog2dict-0.0.3/elblog2dict.egg-info/PKG-INFO
--rw-r--r--   0 jonghun    (501) staff       (20)      246 2023-06-19 08:46:11.000000 elblog2dict-0.0.3/elblog2dict.egg-info/SOURCES.txt
--rw-r--r--   0 jonghun    (501) staff       (20)        1 2023-06-19 08:46:11.000000 elblog2dict-0.0.3/elblog2dict.egg-info/dependency_links.txt
--rw-r--r--   0 jonghun    (501) staff       (20)        1 2023-06-19 08:46:11.000000 elblog2dict-0.0.3/elblog2dict.egg-info/not-zip-safe
--rw-r--r--   0 jonghun    (501) staff       (20)       12 2023-06-19 08:46:11.000000 elblog2dict-0.0.3/elblog2dict.egg-info/top_level.txt
--rw-r--r--   0 jonghun    (501) staff       (20)       38 2023-06-19 08:46:11.798367 elblog2dict-0.0.3/setup.cfg
--rw-r--r--   0 jonghun    (501) staff       (20)      636 2023-06-19 08:46:04.000000 elblog2dict-0.0.3/setup.py
+drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 09:11:41.584382 elblog2dict-0.0.4/
+-rw-r--r--   0 jonghun    (501) staff       (20)     1036 2023-06-19 06:50:28.000000 elblog2dict-0.0.4/LICENSE
+-rw-r--r--   0 jonghun    (501) staff       (20)      540 2023-06-19 09:11:41.584280 elblog2dict-0.0.4/PKG-INFO
+-rw-r--r--   0 jonghun    (501) staff       (20)        6 2023-06-19 09:11:12.000000 elblog2dict-0.0.4/README.md
+drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 09:11:41.583441 elblog2dict-0.0.4/elblog2dict/
+-rw-r--r--   0 jonghun    (501) staff       (20)       21 2023-06-19 09:11:04.000000 elblog2dict-0.0.4/elblog2dict/__init__.py
+-rw-r--r--   0 jonghun    (501) staff       (20)     1490 2023-06-19 08:45:21.000000 elblog2dict-0.0.4/elblog2dict/parser.py
+drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 09:11:41.584133 elblog2dict-0.0.4/elblog2dict.egg-info/
+-rw-r--r--   0 jonghun    (501) staff       (20)      540 2023-06-19 09:11:41.000000 elblog2dict-0.0.4/elblog2dict.egg-info/PKG-INFO
+-rw-r--r--   0 jonghun    (501) staff       (20)      246 2023-06-19 09:11:41.000000 elblog2dict-0.0.4/elblog2dict.egg-info/SOURCES.txt
+-rw-r--r--   0 jonghun    (501) staff       (20)        1 2023-06-19 09:11:41.000000 elblog2dict-0.0.4/elblog2dict.egg-info/dependency_links.txt
+-rw-r--r--   0 jonghun    (501) staff       (20)        1 2023-06-19 09:11:41.000000 elblog2dict-0.0.4/elblog2dict.egg-info/not-zip-safe
+-rw-r--r--   0 jonghun    (501) staff       (20)       12 2023-06-19 09:11:41.000000 elblog2dict-0.0.4/elblog2dict.egg-info/top_level.txt
+-rw-r--r--   0 jonghun    (501) staff       (20)       38 2023-06-19 09:11:41.584416 elblog2dict-0.0.4/setup.cfg
+-rw-r--r--   0 jonghun    (501) staff       (20)      780 2023-06-19 09:11:01.000000 elblog2dict-0.0.4/setup.py
```

### Comparing `elblog2dict-0.0.3/LICENSE` & `elblog2dict-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `elblog2dict-0.0.3/elblog2dict/parser.py` & `elblog2dict-0.0.4/elblog2dict/parser.py`

 * *Files identical despite different names*

### Comparing `elblog2dict-0.0.3/setup.py` & `elblog2dict-0.0.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='elblog2dict',
-    version='0.0.3',
-    description='temp',
+    version='0.0.4',
+    description='Utility for parsing and extracting data from ELB logs',
     author='leemhoon00',
     author_email='leemhoon000@gmail.com',
-    url='',
+    url='https://github.com/leemhoon00/elblog2dict',
     install_requires=[],
     packages=find_packages(exclude=['.git', '.gitignore', '*.gz', 'test.py']),
-    keywords=['elb'],
+    keywords=['elb', 'log', 'parser', 'elblog2dict', 'regular expression'],
     python_requires='>=3.6',
     package_data={},
     zip_safe=False,
     classifiers=[
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```

