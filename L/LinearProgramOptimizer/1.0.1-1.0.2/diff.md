# Comparing `tmp/LinearProgramOptimizer-1.0.1.tar.gz` & `tmp/LinearProgramOptimizer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LinearProgramOptimizer-1.0.1.tar", last modified: Mon Jun 19 05:42:52 2023, max compression
+gzip compressed data, was "LinearProgramOptimizer-1.0.2.tar", last modified: Mon Jun 19 07:16:01 2023, max compression
```

## Comparing `LinearProgramOptimizer-1.0.1.tar` & `LinearProgramOptimizer-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 05:42:52.009671 LinearProgramOptimizer-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-19 05:42:51.998701 LinearProgramOptimizer-1.0.1/LinearProgramOptimizer/
--rw-rw-rw-   0        0        0       73 2023-06-18 21:40:22.000000 LinearProgramOptimizer-1.0.1/LinearProgramOptimizer/__init__.py
--rw-rw-rw-   0        0        0     3765 2023-06-18 21:40:22.000000 LinearProgramOptimizer-1.0.1/LinearProgramOptimizer/revisedSimplex.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:42:52.007677 LinearProgramOptimizer-1.0.1/LinearProgramOptimizer.egg-info/
--rw-rw-rw-   0        0        0      956 2023-06-19 05:42:51.000000 LinearProgramOptimizer-1.0.1/LinearProgramOptimizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-06-19 05:42:51.000000 LinearProgramOptimizer-1.0.1/LinearProgramOptimizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 05:42:51.000000 LinearProgramOptimizer-1.0.1/LinearProgramOptimizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 05:42:51.000000 LinearProgramOptimizer-1.0.1/LinearProgramOptimizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-19 05:42:51.000000 LinearProgramOptimizer-1.0.1/LinearProgramOptimizer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      956 2023-06-19 05:42:52.008674 LinearProgramOptimizer-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-06-18 21:40:22.000000 LinearProgramOptimizer-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 05:42:52.010669 LinearProgramOptimizer-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1144 2023-06-18 21:40:22.000000 LinearProgramOptimizer-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:16:01.993433 LinearProgramOptimizer-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-19 07:16:01.981979 LinearProgramOptimizer-1.0.2/LinearProgramOptimizer/
+-rw-rw-rw-   0        0        0       73 2023-06-18 23:11:30.000000 LinearProgramOptimizer-1.0.2/LinearProgramOptimizer/__init__.py
+-rw-rw-rw-   0        0        0     3567 2023-06-18 23:11:30.000000 LinearProgramOptimizer-1.0.2/LinearProgramOptimizer/revisedSimplex.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:16:01.990437 LinearProgramOptimizer-1.0.2/LinearProgramOptimizer.egg-info/
+-rw-rw-rw-   0        0        0      956 2023-06-19 07:16:01.000000 LinearProgramOptimizer-1.0.2/LinearProgramOptimizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-06-19 07:16:01.000000 LinearProgramOptimizer-1.0.2/LinearProgramOptimizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 07:16:01.000000 LinearProgramOptimizer-1.0.2/LinearProgramOptimizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 07:16:01.000000 LinearProgramOptimizer-1.0.2/LinearProgramOptimizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-19 07:16:01.000000 LinearProgramOptimizer-1.0.2/LinearProgramOptimizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      956 2023-06-19 07:16:01.992465 LinearProgramOptimizer-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-06-18 23:11:30.000000 LinearProgramOptimizer-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 07:16:01.993433 LinearProgramOptimizer-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1144 2023-06-19 07:15:34.000000 LinearProgramOptimizer-1.0.2/setup.py
```

### Comparing `LinearProgramOptimizer-1.0.1/LinearProgramOptimizer/revisedSimplex.py` & `LinearProgramOptimizer-1.0.2/LinearProgramOptimizer/revisedSimplex.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import pandas as pd
 import numpy as np
 
 
-def revised_simplex(c, A, b, n=None, verbose=False):
+def optimize(c, A, b, n=None, verbose=False):
     """
 
     :param c: An array of the coefficents of the objective function
     :param A: A square array of the coefficents of the LHS of the constraints 'must be <='
     :param b: An array of the coefficients of the RHS of the constraints 'must be <= '
     :param n: number of variables
     :return:
@@ -81,19 +80,15 @@
 
                 # Update the entering and leaving variables in the matrix B and N
                 a = np.copy(B[:, leaving_B:leaving_B + 1])
                 v = np.copy(N[:, entering_N:entering_N + 1])
                 B[:, leaving_B:leaving_B + 1], N[:, entering_N:entering_N + 1] = v, a
 
     optimal = {}
-    print(xb)
-    print(xb_prime)
-    print(cb.T[0])
-    #     for variable,value in zip(xb[cb.T[0]>0],xb_prime[cb.T[0]>0]):
-    #         optimal[f'X{variable}']=value
+  
     xb = list(xb)
     for variable in xb:
         if variable <= n:
             optimal[f'X{variable}'] = xb_prime[xb.index(variable)]
 
     optimal['obj function'] = z_prime
```

### Comparing `LinearProgramOptimizer-1.0.1/LinearProgramOptimizer.egg-info/PKG-INFO` & `LinearProgramOptimizer-1.0.2/LinearProgramOptimizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LinearProgramOptimizer
-Version: 1.0.1
+Version: 1.0.2
 Summary: Optimization models for solving Linear Programming Problems
 Author: OguntolaIbrahim
 Author-email: <oibrahimopeyemi@yahoo.com>
 Keywords: python,linear programming,operation research,optimization,simplex
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Other Audience
 Classifier: Programming Language :: Python :: 3
```

### Comparing `LinearProgramOptimizer-1.0.1/PKG-INFO` & `LinearProgramOptimizer-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LinearProgramOptimizer
-Version: 1.0.1
+Version: 1.0.2
 Summary: Optimization models for solving Linear Programming Problems
 Author: OguntolaIbrahim
 Author-email: <oibrahimopeyemi@yahoo.com>
 Keywords: python,linear programming,operation research,optimization,simplex
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Other Audience
 Classifier: Programming Language :: Python :: 3
```

### Comparing `LinearProgramOptimizer-1.0.1/setup.py` & `LinearProgramOptimizer-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = 'Optimization models for solving Linear Programming Problems'
 LONG_DESCRIPTION = 'Optimization models for solving Linear Programming Problems'
 
 # Setting up
 setup(
     name="LinearProgramOptimizer",
     version=VERSION,
```

