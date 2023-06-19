# Comparing `tmp/linearProgramOptimizer-0.0.1.tar.gz` & `tmp/LinearProgramOptimizer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linearProgramOptimizer-0.0.1.tar", last modified: Mon Jun 19 05:23:07 2023, max compression
+gzip compressed data, was "LinearProgramOptimizer-1.0.1.tar", last modified: Mon Jun 19 05:42:52 2023, max compression
```

## Comparing `linearProgramOptimizer-0.0.1.tar` & `LinearProgramOptimizer-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 05:23:07.783286 linearProgramOptimizer-0.0.1/
--rw-rw-rw-   0        0        0      956 2023-06-19 05:23:07.781706 linearProgramOptimizer-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-06-18 20:08:00.000000 linearProgramOptimizer-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 05:23:07.779741 linearProgramOptimizer-0.0.1/linearProgramOptimizer.egg-info/
--rw-rw-rw-   0        0        0      956 2023-06-19 05:23:07.000000 linearProgramOptimizer-0.0.1/linearProgramOptimizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-06-19 05:23:07.000000 linearProgramOptimizer-0.0.1/linearProgramOptimizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 05:23:07.000000 linearProgramOptimizer-0.0.1/linearProgramOptimizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 05:23:07.000000 linearProgramOptimizer-0.0.1/linearProgramOptimizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 05:23:07.000000 linearProgramOptimizer-0.0.1/linearProgramOptimizer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 05:23:07.783286 linearProgramOptimizer-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1144 2023-06-19 05:22:36.000000 linearProgramOptimizer-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:42:52.009671 LinearProgramOptimizer-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-06-19 05:42:51.998701 LinearProgramOptimizer-1.0.1/LinearProgramOptimizer/
+-rw-rw-rw-   0        0        0       73 2023-06-18 21:40:22.000000 LinearProgramOptimizer-1.0.1/LinearProgramOptimizer/__init__.py
+-rw-rw-rw-   0        0        0     3765 2023-06-18 21:40:22.000000 LinearProgramOptimizer-1.0.1/LinearProgramOptimizer/revisedSimplex.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:42:52.007677 LinearProgramOptimizer-1.0.1/LinearProgramOptimizer.egg-info/
+-rw-rw-rw-   0        0        0      956 2023-06-19 05:42:51.000000 LinearProgramOptimizer-1.0.1/LinearProgramOptimizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-06-19 05:42:51.000000 LinearProgramOptimizer-1.0.1/LinearProgramOptimizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 05:42:51.000000 LinearProgramOptimizer-1.0.1/LinearProgramOptimizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 05:42:51.000000 LinearProgramOptimizer-1.0.1/LinearProgramOptimizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-19 05:42:51.000000 LinearProgramOptimizer-1.0.1/LinearProgramOptimizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      956 2023-06-19 05:42:52.008674 LinearProgramOptimizer-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-06-18 21:40:22.000000 LinearProgramOptimizer-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 05:42:52.010669 LinearProgramOptimizer-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1144 2023-06-18 21:40:22.000000 LinearProgramOptimizer-1.0.1/setup.py
```

### Comparing `linearProgramOptimizer-0.0.1/PKG-INFO` & `LinearProgramOptimizer-1.0.1/LinearProgramOptimizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: linearProgramOptimizer
-Version: 0.0.1
+Name: LinearProgramOptimizer
+Version: 1.0.1
 Summary: Optimization models for solving Linear Programming Problems
 Author: OguntolaIbrahim
 Author-email: <oibrahimopeyemi@yahoo.com>
 Keywords: python,linear programming,operation research,optimization,simplex
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Other Audience
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linearProgramOptimizer-0.0.1/linearProgramOptimizer.egg-info/PKG-INFO` & `LinearProgramOptimizer-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: linearProgramOptimizer
-Version: 0.0.1
+Name: LinearProgramOptimizer
+Version: 1.0.1
 Summary: Optimization models for solving Linear Programming Problems
 Author: OguntolaIbrahim
 Author-email: <oibrahimopeyemi@yahoo.com>
 Keywords: python,linear programming,operation research,optimization,simplex
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Other Audience
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linearProgramOptimizer-0.0.1/setup.py` & `LinearProgramOptimizer-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '1.0.1'
 DESCRIPTION = 'Optimization models for solving Linear Programming Problems'
 LONG_DESCRIPTION = 'Optimization models for solving Linear Programming Problems'
 
 # Setting up
 setup(
-    name="linearProgramOptimizer",
+    name="LinearProgramOptimizer",
     version=VERSION,
     author="OguntolaIbrahim",
     author_email="<oibrahimopeyemi@yahoo.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

