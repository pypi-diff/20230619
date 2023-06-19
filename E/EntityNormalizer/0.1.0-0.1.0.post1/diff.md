# Comparing `tmp/EntityNormalizer-0.1.0.tar.gz` & `tmp/EntityNormalizer-0.1.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EntityNormalizer-0.1.0.tar", last modified: Mon Jun 19 04:33:51 2023, max compression
+gzip compressed data, was "EntityNormalizer-0.1.0.post1.tar", last modified: Mon Jun 19 04:45:29 2023, max compression
```

## Comparing `EntityNormalizer-0.1.0.tar` & `EntityNormalizer-0.1.0.post1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 gabriel-he   (501) staff       (20)        0 2023-06-19 04:33:51.643770 EntityNormalizer-0.1.0/
-drwxr-xr-x   0 gabriel-he   (501) staff       (20)        0 2023-06-19 04:33:51.642859 EntityNormalizer-0.1.0/EntityNormalizer/
--rw-r--r--   0 gabriel-he   (501) staff       (20)     2388 2023-06-14 01:47:35.000000 EntityNormalizer-0.1.0/EntityNormalizer/__init__.py
-drwxr-xr-x   0 gabriel-he   (501) staff       (20)        0 2023-06-19 04:33:51.643628 EntityNormalizer-0.1.0/EntityNormalizer.egg-info/
--rw-r--r--   0 gabriel-he   (501) staff       (20)      350 2023-06-19 04:33:51.000000 EntityNormalizer-0.1.0/EntityNormalizer.egg-info/PKG-INFO
--rw-r--r--   0 gabriel-he   (501) staff       (20)      268 2023-06-19 04:33:51.000000 EntityNormalizer-0.1.0/EntityNormalizer.egg-info/SOURCES.txt
--rw-r--r--   0 gabriel-he   (501) staff       (20)        1 2023-06-19 04:33:51.000000 EntityNormalizer-0.1.0/EntityNormalizer.egg-info/dependency_links.txt
--rw-r--r--   0 gabriel-he   (501) staff       (20)       26 2023-06-19 04:33:51.000000 EntityNormalizer-0.1.0/EntityNormalizer.egg-info/requires.txt
--rw-r--r--   0 gabriel-he   (501) staff       (20)       17 2023-06-19 04:33:51.000000 EntityNormalizer-0.1.0/EntityNormalizer.egg-info/top_level.txt
--rw-r--r--   0 gabriel-he   (501) staff       (20)     1061 2023-06-19 04:28:05.000000 EntityNormalizer-0.1.0/LICENSE.txt
--rw-r--r--   0 gabriel-he   (501) staff       (20)      350 2023-06-19 04:33:51.643832 EntityNormalizer-0.1.0/PKG-INFO
--rw-r--r--   0 gabriel-he   (501) staff       (20)     2328 2023-06-14 01:42:57.000000 EntityNormalizer-0.1.0/README.md
--rw-r--r--   0 gabriel-he   (501) staff       (20)       79 2023-06-19 04:33:51.644017 EntityNormalizer-0.1.0/setup.cfg
--rw-r--r--   0 gabriel-he   (501) staff       (20)      519 2023-06-19 04:26:49.000000 EntityNormalizer-0.1.0/setup.py
+drwxr-xr-x   0 gabriel-he   (501) staff       (20)        0 2023-06-19 04:45:29.334122 EntityNormalizer-0.1.0.post1/
+drwxr-xr-x   0 gabriel-he   (501) staff       (20)        0 2023-06-19 04:45:29.333425 EntityNormalizer-0.1.0.post1/EntityNormalizer/
+-rw-r--r--   0 gabriel-he   (501) staff       (20)     2388 2023-06-14 01:47:35.000000 EntityNormalizer-0.1.0.post1/EntityNormalizer/__init__.py
+drwxr-xr-x   0 gabriel-he   (501) staff       (20)        0 2023-06-19 04:45:29.334004 EntityNormalizer-0.1.0.post1/EntityNormalizer.egg-info/
+-rw-r--r--   0 gabriel-he   (501) staff       (20)      356 2023-06-19 04:45:29.000000 EntityNormalizer-0.1.0.post1/EntityNormalizer.egg-info/PKG-INFO
+-rw-r--r--   0 gabriel-he   (501) staff       (20)      268 2023-06-19 04:45:29.000000 EntityNormalizer-0.1.0.post1/EntityNormalizer.egg-info/SOURCES.txt
+-rw-r--r--   0 gabriel-he   (501) staff       (20)        1 2023-06-19 04:45:29.000000 EntityNormalizer-0.1.0.post1/EntityNormalizer.egg-info/dependency_links.txt
+-rw-r--r--   0 gabriel-he   (501) staff       (20)       26 2023-06-19 04:45:29.000000 EntityNormalizer-0.1.0.post1/EntityNormalizer.egg-info/requires.txt
+-rw-r--r--   0 gabriel-he   (501) staff       (20)       17 2023-06-19 04:45:29.000000 EntityNormalizer-0.1.0.post1/EntityNormalizer.egg-info/top_level.txt
+-rw-r--r--   0 gabriel-he   (501) staff       (20)     1061 2023-06-19 04:28:05.000000 EntityNormalizer-0.1.0.post1/LICENSE.txt
+-rw-r--r--   0 gabriel-he   (501) staff       (20)      356 2023-06-19 04:45:29.334186 EntityNormalizer-0.1.0.post1/PKG-INFO
+-rw-r--r--   0 gabriel-he   (501) staff       (20)     2285 2023-06-19 04:40:59.000000 EntityNormalizer-0.1.0.post1/README.md
+-rw-r--r--   0 gabriel-he   (501) staff       (20)       79 2023-06-19 04:45:29.334387 EntityNormalizer-0.1.0.post1/setup.cfg
+-rw-r--r--   0 gabriel-he   (501) staff       (20)      545 2023-06-19 04:45:23.000000 EntityNormalizer-0.1.0.post1/setup.py
```

### Comparing `EntityNormalizer-0.1.0/EntityNormalizer/__init__.py` & `EntityNormalizer-0.1.0.post1/EntityNormalizer/__init__.py`

 * *Files identical despite different names*

### Comparing `EntityNormalizer-0.1.0/LICENSE.txt` & `EntityNormalizer-0.1.0.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EntityNormalizer-0.1.0/README.md` & `EntityNormalizer-0.1.0.post1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Python tool for normalizing entities based on a dictionary.
 
 ## Usage
 
 This tool can be used as:
 - a *command line tool*, by cloning this repository and running `pip install .` under the root of this source; then you can run`main.py` with the required parameters to process your entity-listed file.
-- a *Python package* , by installing the package using `pip install git+https://github.com/gabrielandrade2/EntityNormalizer.git`
+- a *Python package* , by installing the package using `pip install EntityNormalizer`
 
 ### Input and output
   
 The input file must contain one entity per line. 
 The output file will contain the normalized entities, again, one per line.  
 The dicitory file must be a comma-separated table file, i.e., `csv`.
```

### Comparing `EntityNormalizer-0.1.0/setup.py` & `EntityNormalizer-0.1.0.post1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from setuptools import find_packages, setup
 setup(
     name='EntityNormalizer',
     packages=find_packages(),
-    version='0.1.0',
+    version='0.1.0-1',
     description='Library for normalizing entities based on a dictionary',
     author='Gabriel Herman Bernardim Andrade',
     license='MIT',
+    readme='README.md',
     url='https://github.com/sociocom/EntityNormalizer',
     download_url='https://github.com/sociocom/EntityNormalizer/archive/refs/tags/0.1.0.tar.gz',
     py_modules=['EntityNormalizer'],
     install_requires=['pandas', 'rapidfuzz', 'mojimoji'],
 )
```

