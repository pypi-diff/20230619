# Comparing `tmp/EntityNormalizer-0.1.0.post1.tar.gz` & `tmp/EntityNormalizer-0.1.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EntityNormalizer-0.1.0.post1.tar", last modified: Mon Jun 19 04:45:29 2023, max compression
+gzip compressed data, was "EntityNormalizer-0.1.0.post2.tar", last modified: Mon Jun 19 04:52:07 2023, max compression
```

## Comparing `EntityNormalizer-0.1.0.post1.tar` & `EntityNormalizer-0.1.0.post2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 gabriel-he   (501) staff       (20)        0 2023-06-19 04:45:29.334122 EntityNormalizer-0.1.0.post1/
-drwxr-xr-x   0 gabriel-he   (501) staff       (20)        0 2023-06-19 04:45:29.333425 EntityNormalizer-0.1.0.post1/EntityNormalizer/
--rw-r--r--   0 gabriel-he   (501) staff       (20)     2388 2023-06-14 01:47:35.000000 EntityNormalizer-0.1.0.post1/EntityNormalizer/__init__.py
-drwxr-xr-x   0 gabriel-he   (501) staff       (20)        0 2023-06-19 04:45:29.334004 EntityNormalizer-0.1.0.post1/EntityNormalizer.egg-info/
--rw-r--r--   0 gabriel-he   (501) staff       (20)      356 2023-06-19 04:45:29.000000 EntityNormalizer-0.1.0.post1/EntityNormalizer.egg-info/PKG-INFO
--rw-r--r--   0 gabriel-he   (501) staff       (20)      268 2023-06-19 04:45:29.000000 EntityNormalizer-0.1.0.post1/EntityNormalizer.egg-info/SOURCES.txt
--rw-r--r--   0 gabriel-he   (501) staff       (20)        1 2023-06-19 04:45:29.000000 EntityNormalizer-0.1.0.post1/EntityNormalizer.egg-info/dependency_links.txt
--rw-r--r--   0 gabriel-he   (501) staff       (20)       26 2023-06-19 04:45:29.000000 EntityNormalizer-0.1.0.post1/EntityNormalizer.egg-info/requires.txt
--rw-r--r--   0 gabriel-he   (501) staff       (20)       17 2023-06-19 04:45:29.000000 EntityNormalizer-0.1.0.post1/EntityNormalizer.egg-info/top_level.txt
--rw-r--r--   0 gabriel-he   (501) staff       (20)     1061 2023-06-19 04:28:05.000000 EntityNormalizer-0.1.0.post1/LICENSE.txt
--rw-r--r--   0 gabriel-he   (501) staff       (20)      356 2023-06-19 04:45:29.334186 EntityNormalizer-0.1.0.post1/PKG-INFO
--rw-r--r--   0 gabriel-he   (501) staff       (20)     2285 2023-06-19 04:40:59.000000 EntityNormalizer-0.1.0.post1/README.md
--rw-r--r--   0 gabriel-he   (501) staff       (20)       79 2023-06-19 04:45:29.334387 EntityNormalizer-0.1.0.post1/setup.cfg
--rw-r--r--   0 gabriel-he   (501) staff       (20)      545 2023-06-19 04:45:23.000000 EntityNormalizer-0.1.0.post1/setup.py
+drwxr-xr-x   0 gabriel-he   (501) staff       (20)        0 2023-06-19 04:52:07.237644 EntityNormalizer-0.1.0.post2/
+drwxr-xr-x   0 gabriel-he   (501) staff       (20)        0 2023-06-19 04:52:07.237017 EntityNormalizer-0.1.0.post2/EntityNormalizer/
+-rw-r--r--   0 gabriel-he   (501) staff       (20)     2388 2023-06-14 01:47:35.000000 EntityNormalizer-0.1.0.post2/EntityNormalizer/__init__.py
+drwxr-xr-x   0 gabriel-he   (501) staff       (20)        0 2023-06-19 04:52:07.237541 EntityNormalizer-0.1.0.post2/EntityNormalizer.egg-info/
+-rw-r--r--   0 gabriel-he   (501) staff       (20)     2682 2023-06-19 04:52:07.000000 EntityNormalizer-0.1.0.post2/EntityNormalizer.egg-info/PKG-INFO
+-rw-r--r--   0 gabriel-he   (501) staff       (20)      268 2023-06-19 04:52:07.000000 EntityNormalizer-0.1.0.post2/EntityNormalizer.egg-info/SOURCES.txt
+-rw-r--r--   0 gabriel-he   (501) staff       (20)        1 2023-06-19 04:52:07.000000 EntityNormalizer-0.1.0.post2/EntityNormalizer.egg-info/dependency_links.txt
+-rw-r--r--   0 gabriel-he   (501) staff       (20)       26 2023-06-19 04:52:07.000000 EntityNormalizer-0.1.0.post2/EntityNormalizer.egg-info/requires.txt
+-rw-r--r--   0 gabriel-he   (501) staff       (20)       17 2023-06-19 04:52:07.000000 EntityNormalizer-0.1.0.post2/EntityNormalizer.egg-info/top_level.txt
+-rw-r--r--   0 gabriel-he   (501) staff       (20)     1061 2023-06-19 04:28:05.000000 EntityNormalizer-0.1.0.post2/LICENSE.txt
+-rw-r--r--   0 gabriel-he   (501) staff       (20)     2682 2023-06-19 04:52:07.237712 EntityNormalizer-0.1.0.post2/PKG-INFO
+-rw-r--r--   0 gabriel-he   (501) staff       (20)     2285 2023-06-19 04:40:59.000000 EntityNormalizer-0.1.0.post2/README.md
+-rw-r--r--   0 gabriel-he   (501) staff       (20)      160 2023-06-19 04:52:07.237890 EntityNormalizer-0.1.0.post2/setup.cfg
+-rw-r--r--   0 gabriel-he   (501) staff       (20)      545 2023-06-19 04:52:02.000000 EntityNormalizer-0.1.0.post2/setup.py
```

### Comparing `EntityNormalizer-0.1.0.post1/EntityNormalizer/__init__.py` & `EntityNormalizer-0.1.0.post2/EntityNormalizer/__init__.py`

 * *Files identical despite different names*

### Comparing `EntityNormalizer-0.1.0.post1/LICENSE.txt` & `EntityNormalizer-0.1.0.post2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EntityNormalizer-0.1.0.post1/README.md` & `EntityNormalizer-0.1.0.post2/README.md`

 * *Files identical despite different names*

### Comparing `EntityNormalizer-0.1.0.post1/setup.py` & `EntityNormalizer-0.1.0.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 setup(
     name='EntityNormalizer',
     packages=find_packages(),
-    version='0.1.0-1',
+    version='0.1.0-2',
     description='Library for normalizing entities based on a dictionary',
     author='Gabriel Herman Bernardim Andrade',
     license='MIT',
     readme='README.md',
     url='https://github.com/sociocom/EntityNormalizer',
     download_url='https://github.com/sociocom/EntityNormalizer/archive/refs/tags/0.1.0.tar.gz',
     py_modules=['EntityNormalizer'],
```

