# Comparing `tmp/glis-2.0.1.tar.gz` & `tmp/glis-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glis-2.0.1.tar", last modified: Wed Feb  1 13:51:49 2023, max compression
+gzip compressed data, was "glis-2.0.2.tar", last modified: Mon Jun 19 16:52:28 2023, max compression
```

## Comparing `glis-2.0.1.tar` & `glis-2.0.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-02-01 13:51:49.607396 glis-2.0.1/
--rw-r--r--   0 bemporad   (501) staff       (20)    11345 2023-01-10 10:53:45.000000 glis-2.0.1/LICENSE.txt
--rw-r--r--   0 bemporad   (501) staff       (20)    22036 2023-02-01 13:51:49.607265 glis-2.0.1/PKG-INFO
--rw-r--r--   0 bemporad   (501) staff       (20)    21382 2023-01-22 14:49:54.000000 glis-2.0.1/README.md
--rw-r--r--   0 bemporad   (501) staff       (20)      821 2023-02-01 13:51:41.000000 glis-2.0.1/pyproject.toml
--rw-r--r--   0 bemporad   (501) staff       (20)       38 2023-02-01 13:51:49.607431 glis-2.0.1/setup.cfg
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-02-01 13:51:49.605789 glis-2.0.1/src/
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-02-01 13:51:49.606483 glis-2.0.1/src/glis/
--rw-r--r--   0 bemporad   (501) staff       (20)        0 2023-01-10 11:29:35.000000 glis-2.0.1/src/glis/__init__.py
--rwxr-xr-x   0 bemporad   (501) staff       (20)      954 2023-01-21 16:33:49.000000 glis-2.0.1/src/glis/rbf.py
--rwxr-xr-x   0 bemporad   (501) staff       (20)    64160 2023-01-21 16:34:21.000000 glis-2.0.1/src/glis/solvers.py
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-02-01 13:51:49.607101 glis-2.0.1/src/glis.egg-info/
--rw-r--r--   0 bemporad   (501) staff       (20)    22036 2023-02-01 13:51:49.000000 glis-2.0.1/src/glis.egg-info/PKG-INFO
--rw-r--r--   0 bemporad   (501) staff       (20)      252 2023-02-01 13:51:49.000000 glis-2.0.1/src/glis.egg-info/SOURCES.txt
--rw-r--r--   0 bemporad   (501) staff       (20)        1 2023-02-01 13:51:49.000000 glis-2.0.1/src/glis.egg-info/dependency_links.txt
--rw-r--r--   0 bemporad   (501) staff       (20)       32 2023-02-01 13:51:49.000000 glis-2.0.1/src/glis.egg-info/requires.txt
--rw-r--r--   0 bemporad   (501) staff       (20)        5 2023-02-01 13:51:49.000000 glis-2.0.1/src/glis.egg-info/top_level.txt
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-06-19 16:52:28.453963 glis-2.0.2/
+-rw-r--r--   0 bemporad   (501) staff       (20)    11345 2023-01-10 10:53:45.000000 glis-2.0.2/LICENSE.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)    22036 2023-06-19 16:52:28.453841 glis-2.0.2/PKG-INFO
+-rw-r--r--   0 bemporad   (501) staff       (20)    21382 2023-01-22 14:49:54.000000 glis-2.0.2/README.md
+-rw-r--r--   0 bemporad   (501) staff       (20)      821 2023-06-19 16:51:07.000000 glis-2.0.2/pyproject.toml
+-rw-r--r--   0 bemporad   (501) staff       (20)       38 2023-06-19 16:52:28.453995 glis-2.0.2/setup.cfg
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-06-19 16:52:28.452204 glis-2.0.2/src/
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-06-19 16:52:28.452957 glis-2.0.2/src/glis/
+-rw-r--r--   0 bemporad   (501) staff       (20)        0 2023-01-10 11:29:35.000000 glis-2.0.2/src/glis/__init__.py
+-rwxr-xr-x   0 bemporad   (501) staff       (20)      954 2023-01-21 16:33:49.000000 glis-2.0.2/src/glis/rbf.py
+-rwxr-xr-x   0 bemporad   (501) staff       (20)    64189 2023-03-03 12:18:48.000000 glis-2.0.2/src/glis/solvers.py
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-06-19 16:52:28.453565 glis-2.0.2/src/glis.egg-info/
+-rw-r--r--   0 bemporad   (501) staff       (20)    22036 2023-06-19 16:52:28.000000 glis-2.0.2/src/glis.egg-info/PKG-INFO
+-rw-r--r--   0 bemporad   (501) staff       (20)      271 2023-06-19 16:52:28.000000 glis-2.0.2/src/glis.egg-info/SOURCES.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)        1 2023-06-19 16:52:28.000000 glis-2.0.2/src/glis.egg-info/dependency_links.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)       32 2023-06-19 16:52:28.000000 glis-2.0.2/src/glis.egg-info/requires.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)        5 2023-06-19 16:52:28.000000 glis-2.0.2/src/glis.egg-info/top_level.txt
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-06-19 16:52:28.453682 glis-2.0.2/tests/
+-rw-r--r--   0 bemporad   (501) staff       (20)     9847 2023-01-22 14:33:09.000000 glis-2.0.2/tests/test_glis.py
```

### Comparing `glis-2.0.1/LICENSE.txt` & `glis-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `glis-2.0.1/PKG-INFO` & `glis-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glis
-Version: 2.0.1
+Version: 2.0.2
 Summary: GLIS - (GL)obal optimization by (I)nverse distance weighting and (S)urrogate radial basis functions
 Author-email: Alberto Bemporad <alberto.bemporad@imtlucca.it>, Mengjia Zhu <mengjia.zhu@imtlucca.it>
 Project-URL: Homepage, http://cse.lab.imtlucca.it/~bemporad/glis
 Keywords: global optimization,preference-based optimization,black-box optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `glis-2.0.1/README.md` & `glis-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `glis-2.0.1/pyproject.toml` & `glis-2.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "glis"
-version = "2.0.1"
+version = "2.0.2"
 authors = [
   { name="Alberto Bemporad", email="alberto.bemporad@imtlucca.it" },
   { name="Mengjia Zhu", email="mengjia.zhu@imtlucca.it" },
 ]
 description = "GLIS - (GL)obal optimization by (I)nverse distance weighting and (S)urrogate radial basis functions"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `glis-2.0.1/src/glis/rbf.py` & `glis-2.0.2/src/glis/rbf.py`

 * *Files identical despite different names*

### Comparing `glis-2.0.1/src/glis/solvers.py` & `glis-2.0.2/src/glis/solvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 [3] M. Zhu, D. Piga, and A. Bemporad, “C-GLISp: Preference-based global optimization under
     unknown constraints with applications to controller calibration,” IEEE Trans. Contr.
     Systems Technology, vol. 30, no. 3, pp. 2176–2187, Sept. 2022.
 
 """
 
 import numpy as np
+import math as mt
 from pyswarm import pso  # the "pyswarms" package could be used here too
 import contextlib
 import io
 from scipy.optimize import linprog
 from pyDOE import lhs
 import time
 from numba import njit
@@ -240,16 +241,16 @@
 
     lm1 = max(PHI_W + sepvalue, 0.0)
     l0 = max(0, PHI_W - sepvalue, -PHI_W - sepvalue)
     l1 = max(sepvalue - PHI_W, 0.0)
     c0 = 1.0
     cm1 = 1.0
     c1 = 1.0
-    em1 = exp(-cm1 * lm1)
-    f = -em1 / (em1 + exp(-c0 * l0) + exp(-c1 * l1))
+    em1 = mt.exp(-cm1 * lm1)
+    f = -em1 / (em1 + mt.exp(-c0 * l0) + mt.exp(-c1 * l1))
 
     return f
 
 
 class GLIS_base(object):
     """
     Base class of GLIS to set up the problem and provide the default values to related parameters
@@ -1439,15 +1440,15 @@
                 delta_G = 0.
             if self.has_satisfaction_fun:
                 delta_S_default = self.delta / 2.
                 delta_S = self.get_delta_adpt(Xs, np.array(self.UnknownSatisfactory), delta_S_default)
             else:
                 delta_S = 0.
 
-            dF = self.Fmax - self.Fmin
+            # dF = self.Fmax - self.Fmin
 
             M = self.MM[self.itheta]  # current RBF matrix
 
             t0 = time.time()
             # update weights associated with RBF matrix M and current preference info
             W = self.get_rbf_weights(M, N + 1, np.array(self.I), np.array(self.Ieq), self.ibest)
```

### Comparing `glis-2.0.1/src/glis.egg-info/PKG-INFO` & `glis-2.0.2/src/glis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glis
-Version: 2.0.1
+Version: 2.0.2
 Summary: GLIS - (GL)obal optimization by (I)nverse distance weighting and (S)urrogate radial basis functions
 Author-email: Alberto Bemporad <alberto.bemporad@imtlucca.it>, Mengjia Zhu <mengjia.zhu@imtlucca.it>
 Project-URL: Homepage, http://cse.lab.imtlucca.it/~bemporad/glis
 Keywords: global optimization,preference-based optimization,black-box optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

