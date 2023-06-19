# Comparing `tmp/cryptography318-0.3.2.tar.gz` & `tmp/cryptography318-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptography318-0.3.2.tar", last modified: Mon May 23 19:21:29 2022, max compression
+gzip compressed data, was "cryptography318-0.4.0.tar", last modified: Mon Jun 19 21:14:12 2023, max compression
```

## Comparing `cryptography318-0.3.2.tar` & `cryptography318-0.4.0.tar`

### file list

```diff
@@ -1,35 +1,33 @@
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2022-05-23 19:21:29.228117 cryptography318-0.3.2/
--rw-r--r--   0 andrew     (501) staff       (20)     1704 2022-05-23 19:21:29.227155 cryptography318-0.3.2/PKG-INFO
--rw-r--r--   0 andrew     (501) staff       (20)     1079 2022-03-01 16:25:03.000000 cryptography318-0.3.2/README.md
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2022-05-23 19:21:29.197876 cryptography318-0.3.2/cryptography318/
--rw-r--r--   0 andrew     (501) staff       (20)     1049 2022-05-12 16:21:13.000000 cryptography318-0.3.2/cryptography318/__init__.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2022-05-23 19:21:29.202656 cryptography318-0.3.2/cryptography318/dlp/
--rw-r--r--   0 andrew     (501) staff       (20)      150 2022-03-18 04:48:41.000000 cryptography318-0.3.2/cryptography318/dlp/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     5400 2022-03-18 04:48:41.000000 cryptography318-0.3.2/cryptography318/dlp/dlp.py
--rw-r--r--   0 andrew     (501) staff       (20)     2918 2022-03-21 00:45:43.000000 cryptography318-0.3.2/cryptography318/dlp/icm.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2022-05-23 19:21:29.206911 cryptography318-0.3.2/cryptography318/factor/
--rw-r--r--   0 andrew     (501) staff       (20)      271 2022-03-18 04:48:41.000000 cryptography318-0.3.2/cryptography318/factor/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)    10582 2022-05-11 15:30:49.000000 cryptography318-0.3.2/cryptography318/factor/curve.py
--rw-r--r--   0 andrew     (501) staff       (20)     8825 2022-05-11 15:30:49.000000 cryptography318-0.3.2/cryptography318/factor/elliptic.py
--rw-r--r--   0 andrew     (501) staff       (20)     5530 2022-03-21 00:45:43.000000 cryptography318-0.3.2/cryptography318/factor/factor.py
--rw-r--r--   0 andrew     (501) staff       (20)    10508 2022-03-18 04:48:41.000000 cryptography318-0.3.2/cryptography318/factor/siqs.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2022-05-23 19:21:29.217767 cryptography318-0.3.2/cryptography318/linalg/
--rw-r--r--   0 andrew     (501) staff       (20)      309 2022-03-18 17:26:42.000000 cryptography318-0.3.2/cryptography318/linalg/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)    11176 2022-05-12 16:21:13.000000 cryptography318-0.3.2/cryptography318/linalg/linalg.py
--rw-r--r--   0 andrew     (501) staff       (20)    11875 2022-05-12 16:21:13.000000 cryptography318-0.3.2/cryptography318/linalg/matrix.py
--rw-r--r--   0 andrew     (501) staff       (20)     5119 2022-05-11 15:30:49.000000 cryptography318-0.3.2/cryptography318/linalg/vector.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2022-05-23 19:21:29.224445 cryptography318-0.3.2/cryptography318/prime/
--rw-r--r--   0 andrew     (501) staff       (20)      440 2022-05-13 13:15:10.000000 cryptography318-0.3.2/cryptography318/prime/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     3468 2022-03-18 04:48:41.000000 cryptography318-0.3.2/cryptography318/prime/bailliepsw_helper.py
--rw-r--r--   0 andrew     (501) staff       (20)    17463 2022-05-13 13:24:19.000000 cryptography318-0.3.2/cryptography318/prime/prime.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2022-05-23 19:21:29.226172 cryptography318-0.3.2/cryptography318/utils/
--rw-r--r--   0 andrew     (501) staff       (20)       66 2022-03-18 04:48:41.000000 cryptography318-0.3.2/cryptography318/utils/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     3026 2022-05-12 16:21:13.000000 cryptography318-0.3.2/cryptography318/utils/utils.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2022-05-23 19:21:29.200433 cryptography318-0.3.2/cryptography318.egg-info/
--rw-r--r--   0 andrew     (501) staff       (20)     1704 2022-05-23 19:21:29.000000 cryptography318-0.3.2/cryptography318.egg-info/PKG-INFO
--rw-r--r--   0 andrew     (501) staff       (20)      799 2022-05-23 19:21:29.000000 cryptography318-0.3.2/cryptography318.egg-info/SOURCES.txt
--rw-r--r--   0 andrew     (501) staff       (20)        1 2022-05-23 19:21:29.000000 cryptography318-0.3.2/cryptography318.egg-info/dependency_links.txt
--rw-r--r--   0 andrew     (501) staff       (20)       24 2022-05-23 19:21:29.000000 cryptography318-0.3.2/cryptography318.egg-info/requires.txt
--rw-r--r--   0 andrew     (501) staff       (20)       16 2022-05-23 19:21:29.000000 cryptography318-0.3.2/cryptography318.egg-info/top_level.txt
--rw-r--r--   0 andrew     (501) staff       (20)       38 2022-05-23 19:21:29.229579 cryptography318-0.3.2/setup.cfg
--rw-r--r--   0 andrew     (501) staff       (20)     1666 2022-05-23 19:20:34.000000 cryptography318-0.3.2/setup.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-19 21:14:12.624491 cryptography318-0.4.0/
+-rw-r--r--   0 andrew     (501) staff       (20)     1718 2023-06-19 21:14:12.624350 cryptography318-0.4.0/PKG-INFO
+-rw-r--r--   0 andrew     (501) staff       (20)     1128 2023-03-15 02:24:32.000000 cryptography318-0.4.0/README.md
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-19 21:14:12.621548 cryptography318-0.4.0/cryptography318/
+-rw-r--r--   0 andrew     (501) staff       (20)      987 2023-03-15 00:29:52.000000 cryptography318-0.4.0/cryptography318/__init__.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-19 21:14:12.622498 cryptography318-0.4.0/cryptography318/dlp/
+-rw-r--r--   0 andrew     (501) staff       (20)      150 2023-03-15 00:26:39.000000 cryptography318-0.4.0/cryptography318/dlp/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     5516 2023-03-15 01:53:10.000000 cryptography318-0.4.0/cryptography318/dlp/dlp.py
+-rw-r--r--   0 andrew     (501) staff       (20)     2901 2023-03-15 01:50:49.000000 cryptography318-0.4.0/cryptography318/dlp/icm.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-19 21:14:12.623079 cryptography318-0.4.0/cryptography318/factor/
+-rw-r--r--   0 andrew     (501) staff       (20)      370 2023-06-19 20:52:32.000000 cryptography318-0.4.0/cryptography318/factor/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)    10578 2023-03-15 00:26:39.000000 cryptography318-0.4.0/cryptography318/factor/curve.py
+-rw-r--r--   0 andrew     (501) staff       (20)     8832 2023-03-15 00:26:39.000000 cryptography318-0.4.0/cryptography318/factor/elliptic.py
+-rw-r--r--   0 andrew     (501) staff       (20)     7009 2023-06-19 20:52:32.000000 cryptography318-0.4.0/cryptography318/factor/factor.py
+-rw-r--r--   0 andrew     (501) staff       (20)    10914 2023-03-15 02:17:46.000000 cryptography318-0.4.0/cryptography318/factor/siqs.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-19 21:14:12.623324 cryptography318-0.4.0/cryptography318/linalg/
+-rw-r--r--   0 andrew     (501) staff       (20)      117 2023-03-15 00:26:39.000000 cryptography318-0.4.0/cryptography318/linalg/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     7370 2023-03-15 00:27:38.000000 cryptography318-0.4.0/cryptography318/linalg/linalg.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-19 21:14:12.623776 cryptography318-0.4.0/cryptography318/prime/
+-rw-r--r--   0 andrew     (501) staff       (20)      478 2023-06-19 20:52:32.000000 cryptography318-0.4.0/cryptography318/prime/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     3531 2023-03-15 01:46:28.000000 cryptography318-0.4.0/cryptography318/prime/bailliepsw_helper.py
+-rw-r--r--   0 andrew     (501) staff       (20)    24675 2023-06-19 20:52:32.000000 cryptography318-0.4.0/cryptography318/prime/prime.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-19 21:14:12.624166 cryptography318-0.4.0/cryptography318/utils/
+-rw-r--r--   0 andrew     (501) staff       (20)       66 2022-03-18 04:48:41.000000 cryptography318-0.4.0/cryptography318/utils/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     3640 2023-06-19 20:19:13.000000 cryptography318-0.4.0/cryptography318/utils/utils.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-19 21:14:12.622170 cryptography318-0.4.0/cryptography318.egg-info/
+-rw-r--r--   0 andrew     (501) staff       (20)     1718 2023-06-19 21:14:12.000000 cryptography318-0.4.0/cryptography318.egg-info/PKG-INFO
+-rw-r--r--   0 andrew     (501) staff       (20)      733 2023-06-19 21:14:12.000000 cryptography318-0.4.0/cryptography318.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew     (501) staff       (20)        1 2023-06-19 21:14:12.000000 cryptography318-0.4.0/cryptography318.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew     (501) staff       (20)       26 2023-06-19 21:14:12.000000 cryptography318-0.4.0/cryptography318.egg-info/requires.txt
+-rw-r--r--   0 andrew     (501) staff       (20)       16 2023-06-19 21:14:12.000000 cryptography318-0.4.0/cryptography318.egg-info/top_level.txt
+-rw-r--r--   0 andrew     (501) staff       (20)       38 2023-06-19 21:14:12.624534 cryptography318-0.4.0/setup.cfg
+-rw-r--r--   0 andrew     (501) staff       (20)     1668 2022-09-09 15:43:03.000000 cryptography318-0.4.0/setup.py
```

### Comparing `cryptography318-0.3.2/PKG-INFO` & `cryptography318-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: cryptography318
-Version: 0.3.2
+Version: 0.4.0
 Summary: A set of functions useful in cryptography and linear algebra
 Home-page: https://github.com/aarpyy/Cryptography
 Author: Andrew Carpenter
-Author-email: acarpent@oberlin.edu
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: andrewcarp00@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: License :: Public Domain
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
@@ -34,9 +32,8 @@
 
 ## Install
 ```angular2html
 $ pip install cryptography318
 ```
 
 ### License
-This package is unlicensed and not intended for public use.
-
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `cryptography318-0.3.2/README.md` & `cryptography318-0.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 
 ## Install
 ```angular2html
 $ pip install cryptography318
 ```
 
 ### License
-This package is unlicensed and not intended for public use.
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `cryptography318-0.3.2/cryptography318/__init__.py` & `cryptography318-0.4.0/cryptography318/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,40 @@
+import sys
+
 import setuptools.version
 
-from .factor import *
-from .prime import *
-from .utils import *
-from .linalg import *
-from .dlp import *
+from cryptography318.dlp import *
+from cryptography318.factor import *
+from cryptography318.linalg import *
+from cryptography318.prime import *
+from cryptography318.utils import *
 
-import sys
 if sys.version_info < (3, 10):
     raise ImportError("cryptography318 requires Python 3.10 or higher!")
 del sys
 
 try:
     import numpy
-    import sympy
 except ImportError:
-    raise ImportError("cryptography318 depends on both numpy and sympy!")
+    raise ImportError("cryptography318 depends on numpy!")
 else:
     del numpy
-    del sympy
-
 
 __all__ = [
     "factor", "pollard_rho_factor", "pollard_p1",
 
     "siqs",
 
     "randprime", "prime_range", "next_prime", "prev_prime", "isprime", "miller_rabin", "baillie_psw", "confirm_prime",
     "sqrt_mod", "quadratic_residue", "quadratic_non_residue", "chinese_remainder",
 
     "ecm_mont", "ecm_weierstrass", "lenstra_ecm",
 
     "extended_gcd",
 
-    "rref", "kernel", "binary_kernel", "minor", "det", "eigvals", "eigvec", "char_poly", "flatten",
-    "matmul", "transpose",
+    "rref", "kernel_gf2", "kernel",
 
     "baby_step_giant_step", "pollard_rho_dlp", "pohlig_hellman"
 ]
 
 __version__ = setuptools.version.__version__
 __author__ = 'Andrew Carpenter'
```

### Comparing `cryptography318-0.3.2/cryptography318/dlp/dlp.py` & `cryptography318-0.4.0/cryptography318/dlp/dlp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from math import isqrt, gcd, sqrt
 from functools import reduce
+from math import gcd, isqrt, sqrt
 
 from cryptography318.prime.prime import primesieve
-from cryptography318.utils.utils import smooth_factor, from_base
+from cryptography318.utils.utils import from_base, smooth_factor
 
 
 def baby_step_giant_step(g, h, p, order=None):
     """Function attempts to solve DLP using classic baby-step-giant-step algorithm."""
     if order is None:
         order = p - 1
 
@@ -33,15 +33,15 @@
 def pollard_rho_dlp(g, h, p, order=None):
     """Uses Pollard's Rho algorithm for logarithms to solve given discrete log problem. Function will run
     indefinitely until a solution is found.
 
     :param g: integer base
     :param h: integer solution to g^x for some x
     :param p: integer prime modulus
-    :param order: integer order of g (smallest integer s.t. pow(g, order, p) == 1
+    :param order: integer order of g (the smallest integer s.t. pow(g, order, p) == 1
     :return: solution to g^x = h for integer x"""
 
     xstate = (1, 0, 0)
     ystate = (1, 0, 0)
 
     if order is None:
         order = p - 1
@@ -147,27 +147,32 @@
 
 
 def pohlig_hellman(g, h, p, q, exp, prog=False):
     """Function attempts to solve DLP mod p where order of g, q, is some prime raised to a power."""
 
     X = []
     if prog:
-        print("Starting process for X0")
+        prog_print = print
+    else:
+        def prog_print(*args, **kwargs):
+            pass
+
+    prog_print("Starting process for X0")
 
     r = pow(g, pow(q, exp - 1), p)
     X0 = baby_step_giant_step(r, pow(h, pow(q, exp - 1), p), p, q)
     X.append(X0)
 
     if prog:
-        print(f"Found X0 = {X0}\n")
+        prog_print(f"Found X0 = {X0}\n")
 
     for i in range(1, exp):
         if prog:
-            print(f"Starting process for X{i}")
+            prog_print(f"Starting process for X{i}")
         exp_term = from_base(X[::-1], q)
         h_term = pow(h * pow(pow(g, exp_term, p), -1, p), pow(q, exp - i - 1), p)
         Xi = baby_step_giant_step(r, h_term, p, q)
         X.append(Xi)
         if prog:
-            print(f"Found X{i} = {Xi}\n")
+            prog_print(f"Found X{i} = {Xi}\n")
 
     return from_base(X[::-1], q)
```

### Comparing `cryptography318-0.3.2/cryptography318/dlp/icm.py` & `cryptography318-0.4.0/cryptography318/dlp/icm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from cryptography318.prime.prime import prime_range, isprime
-from cryptography318.utils.utils import smooth_factor
-from cryptography318.factor import factor
-from cryptography318.linalg.linalg import matrix_copy
-from .dlp import pollard_rho_dlp
-
-from math import sqrt, log, exp
+from copy import deepcopy
+from math import exp, log, sqrt
 from random import Random
 
+from cryptography318.factor import factor
+from cryptography318.prime.prime import isprime, prime_range
+from cryptography318.utils.utils import smooth_factor
+from cryptography318.dlp.dlp import pollard_rho_dlp
 
 required_relations_ratio = 2
 
 rand = Random()
 
 
 def row_reduce_mod(a, row, col, m):
@@ -31,15 +30,15 @@
     print(f"isprime {n}: {isprime(n)}")
 
     pivot_row = 0  # first pivot belongs in first row
 
     w = len(matrix[0]) - 1
     h = len(matrix)
 
-    array = matrix_copy(matrix)
+    array = deepcopy(matrix)
 
     for j in range(w):
 
         # start at looking for pivot after previous pivot row
         for i in range(pivot_row, h):
 
             # if non-zero element, this row can become pivot row
@@ -49,15 +48,15 @@
                     # Make j'th element the pivot, reducing rest of row as well
                     array[i] = make_pivot_mod(array[i], j, n)
                     assert array[i][j] == 1
 
                 if i > pivot_row:  # if pivot row not already in correct position, swap
                     array[i], array[pivot_row] = array[pivot_row][:], array[i][:]
 
-                row_reduce_mod(array, pivot_row, j, n)      # row reduce everything else
+                row_reduce_mod(array, pivot_row, j, n)  # row reduce everything else
                 pivot_row += 1
                 break
 
     print(f"Array: \n{array}")
 
     if any(array[0][j] for j in range(1, w)):
         print(f"System was not fully solved")
```

### Comparing `cryptography318-0.3.2/cryptography318/factor/curve.py` & `cryptography318-0.4.0/cryptography318/factor/curve.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from abc import ABCMeta, abstractmethod
 from random import Random
-from cryptography318.prime.prime import sqrt_mod
 
+from cryptography318.prime.prime import sqrt_mod
 
 rndm = Random()
 
 
 class Curve(metaclass=ABCMeta):
-
     # parameters of each curve are dependent on the form of each curve, but all operate over FF(m)
     __slots__ = 'modulus'
 
     # __new__ is required for all curves but is not an abstract method since each curve
     # relies on calling super().__new__ which should inherit __new__ from ABCMeta
     # each curve relying on __new__ instead of __init__ also indicates that all curves are immutables
 
@@ -24,15 +23,14 @@
 
     @abstractmethod
     def point(self, *args):
         raise NotImplementedError
 
 
 class Weierstrass(Curve):
-
     __slots__ = 'a', 'b',
 
     def __new__(cls, a, b, mod):
         self = super().__new__(cls)
         self.a, self.b, self.modulus = a, b, mod
         return self
 
@@ -79,15 +77,14 @@
         (a + 2) / 4, x, and z, thus this method will remain unimplemented as it is unimportant
         in its utility in Lenstra's ECM.
         """
         raise NotImplementedError
 
 
 class Point(metaclass=ABCMeta):
-
     __slots__ = 'x', 'curve', 'modulus'
 
     # __new__ is required for all points but is not an abstract method since each point
     # relies on calling super().__new__ which should inherit __new__ from ABCMeta
     # each point relying on __new__ instead of __init__ also indicates that all points are immutables
 
     @abstractmethod
@@ -134,15 +131,14 @@
 
     @property
     def points(self):
         return None, None
 
 
 class WeierstrassPoint(Point):
-
     __slots__ = 'y',
 
     def __new__(cls, x, y, curve):
         self = super().__new__(cls)
         self.x, self.y, self.curve = x % curve.modulus, y % curve.modulus, curve
         self.modulus = curve.modulus
         return self
```

### Comparing `cryptography318-0.3.2/cryptography318/factor/elliptic.py` & `cryptography318-0.4.0/cryptography318/factor/elliptic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from math import log, isqrt, floor, sqrt, gcd
+from math import floor, gcd, isqrt, log, sqrt
 from typing import Union
 
-from .curve import *
+from cryptography318.factor.curve import *
 from cryptography318.prime.prime import isprime, primesieve
 
 
 def safe_weierstrass(p):
     """
     Computes a non-singular Weierstrass elliptic curve safe for elliptic
     curve cryptography, and a point (x, y) that lies on the curve.
@@ -224,22 +224,22 @@
         S[0] = Q
         S[1] = Q.add(Q_2, Q_0)
         for i in range(2, D + 1):
             S[i] = S[i - 1].add(Q_2, S[i - 2])
 
         d = 1
 
-        R = Q_0.ladder(B1)          # B * Q
-        T = Q_0.ladder(B1 - D)      # (B - D) * Q
+        R = Q_0.ladder(B1)  # B * Q
+        T = Q_0.ladder(B1 - D)  # (B - D) * Q
         Q_D = S[D]
         for i in range(1, D + 1):
             d = (d * (R.x * S[i].z - R.z * S[i].x))
 
             # Swap T, R to keep track of difference between points for montgomery addition
-            T, R = R, R.add(Q_D, T)     # R = (B + kD)Q + DQ, T = (B + (k-1) * D)Q = diff
+            T, R = R, R.add(Q_D, T)  # R = (B + kD)Q + DQ, T = (B + (k-1) * D)Q = diff
 
         q = gcd(d, N)
         if 1 < q < N:
             return q
 
     return None
```

### Comparing `cryptography318-0.3.2/cryptography318/factor/factor.py` & `cryptography318-0.4.0/cryptography318/factor/factor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 import os
-
-from math import sqrt, log, gcd
+from math import gcd, log, sqrt
 from random import randrange
 
 from cryptography318.factor import lenstra_ecm
 from cryptography318.factor import siqs
-from cryptography318.prime.prime import isprime, primesieve, next_prime
+from cryptography318.prime.prime import isprime, next_prime, primesieve
+from cryptography318.utils.utils import Details
+
+factor_details = Details(**{
+    "Pollard's Rho": None,
+    "ECM": None,
+    "Pollard's P-1": None,
+    "Quadratic Sieve": None,
+    "Direct": None
+})
+
 
+def get_details():
+    global factor_details
+    return str(factor_details)
 
-def factor(n, rho=True, ecm=True, p1=True, qs=True, limit=None):
+
+def factor(n, rho=True, ecm=True, p1=True, qs=True, limit=None, *, details=False):
     """
     Attempts to factor given integer with four methods, returning None if un-factorable.
     Function first checks if number is prime then finds all small factors if any exist.
     Then (assuming no specific methods were set to False) Pollard's Rho, Lenstra's ECM,
     Pollard's P-1, and the Quadratic Sieve are used sequentially to find non-trivial factor
     of n. If any of these methods succeed, a recursive call of factor is used to factor
     the remaining n. All boolean values for use of methods are preserved in the
@@ -20,57 +33,88 @@
 
     :param n: int number to be factored
     :param rho: bool determining if Pollard's Rho algorithm should be used
     :param ecm: bool determining if Lenstra's ECM algorithm should be used
     :param p1: bool determining if Pollard's P-1 algorithm should be used
     :param qs: bool determining if Quadratic Sieve algorithm should be used
     :param limit: integer limit of factors to be found using small_factors()
+    :param details: bool determining if factor details should be updated
     :return: dictionary of all primes factors and their powers, or None if not factorable
     """
+    global factor_details
+    if details:
+        factor_details.clear_details()
 
     if n == 1:
+        if details:
+            factor_details.add_details("Direct", True)
         return {}
     elif isprime(n):
+        if details:
+            factor_details.add_details("Direct", True)
         return {n: 1}
 
     if limit is None:
         limit = 32768
 
     factors = {}
     k, p = factor_small(factors, n, limit)
+    # If we factored it completely with small factors, return factors
     if k == 1:
+        if details:
+            factor_details.add_details("Direct", True)
         return factors
+    # If we factored it partially with small factors, recursively factor the rest
     elif k != n:
+        # If remaining factor is prime, we are done factoring
         if isprime(k):
             factors[k] = factors.get(k, 0) + 1
+            if details:
+                factor_details.add_details("Direct", True)
             return factors
         n = k
 
     factor_kwargs = {"rho": rho, "ecm": ecm, "p1": p1, "qs": qs, "limit": limit}
 
     if rho:
-        if not _factor_further(n, pollard_rho_factor(n), factors, **factor_kwargs):
+        if details:
+            factor_details.add_details("Pollard's Rho", True)
+        n = _factor_further(n, pollard_rho_factor(n), factors, **factor_kwargs)
+        if n == 1:
             return factors
 
     if ecm:
-        if not _factor_further(n, lenstra_ecm(n), factors, **factor_kwargs):
+        if details:
+            factor_details.add_details("ECM", True)
+        n = _factor_further(n, lenstra_ecm(n), factors, **factor_kwargs)
+        if n == 1:
             return factors
 
     if p1:
-        if not _factor_further(n, pollard_p1(n), factors, **factor_kwargs):
+        if details:
+            factor_details.add_details("Pollard's P-1", True)
+        n = _factor_further(n, pollard_p1(n), factors, **factor_kwargs)
+        if n == 1:
             return factors
 
     if qs:
+        if details:
+            factor_details.add_details("Quadratic Sieve", True)
 
+        # Use local primes.txt if we can find it, otherwise don't use a file (slow)
         fp = "primes.txt" if os.path.exists("../prime/primes.txt") else None
 
         # Nothing left after quadratic sieve, so just return factors
-        _factor_further(n, siqs(n, fp=fp, loud=False), factors, **factor_kwargs)
+        n = _factor_further(n, siqs(n, fp=fp, loud=False), factors, **factor_kwargs)
+        if n != 1:
+            factors[n] = factors.get(n, 0) + 1
         return factors
 
+    return None
+
 
 def pollard_p1(n, B=None, _retry=5):
     """
     Pollard's p - 1 algorithm for factoring large composites.
     Returns one non-trivial factor if factor-able, False if otherwise.
 
     Pollard's p - 1 is best used to remove smaller factors from a larger composite.
@@ -103,15 +147,16 @@
     return None
 
 
 def pollard_rho_factor(n, mix=None, _retry=5):
     if n < 10:
         return factor_small({}, n, 10)
     elif not callable(mix):
-        def mix(e): return (pow(e, 2, n) + 1) % n
+        def mix(e):
+            return (pow(e, 2, n) + 1) % n
 
     y = 2
     for _ in range(_retry):
         x = y
         while True:
             x = mix(x)
             y = mix(mix(y))
@@ -122,15 +167,16 @@
             elif 1 < q:
                 return q
 
         # If didn't find any, try new mixing function and starting value
         y = randrange(0, n - 1)
         a = randrange(1, n - 3)
 
-        def mix(e): return (pow(e, 2, n) + a) % n
+        def mix(e):
+            return (pow(e, 2, n) + a) % n
 
     return None
 
 
 def factor_small(factors, n, limit):
     """
     Computes all prime factors, up to integer limit, of n when given n is small. Returns
@@ -176,25 +222,28 @@
 
 def _factor_further(n, f, factors, **kwargs):
     """
     Helper function for factor that tries to finish factoring n, having found one
     non-trivial factor f. Function also checks if f needs to be factored. Returns
     False if n has been completely factored, True otherwise.
     """
-    if f:
-        n //= f
-        if isprime(f):
-            factors[f] = factors.get(f, 0) + 1
-        else:
-            factors_f = factor(f, **kwargs)
-            for prime in factors_f:
-                factors[prime] = factors.get(prime, 0) + factors_f[prime]
+    if f <= 0:
+        return n
 
-        if n == 1:
-            return False
-        else:
-            more_facs = factor(n, **kwargs)
-            for prime in more_facs:
-                factors[prime] = factors.get(prime, 0) + more_facs[prime]
-            return False
+    n //= f
+    if isprime(f):
+        factors[f] = factors.get(f, 0) + 1
     else:
-        return True
+        factors_f = factor(f, **kwargs)
+        for prime in factors_f:
+            factors[prime] = factors.get(prime, 0) + factors_f[prime]
+
+    if n == 1:
+        return n
+
+    more_facs = factor(n, **kwargs)
+    if more_facs is None:
+        return n
+
+    for prime in more_facs:
+        factors[prime] = factors.get(prime, 0) + more_facs[prime]
+    return 1
```

### Comparing `cryptography318-0.3.2/cryptography318/factor/siqs.py` & `cryptography318-0.4.0/cryptography318/factor/siqs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-from random import Random
-from math import log2, sqrt, isqrt, gcd, ceil
-from functools import reduce
 from collections.abc import Callable
+from functools import reduce
+from math import ceil, gcd, isqrt, log2, prod, sqrt
+from random import Random
 
-from cryptography318.utils.utils import n_digits, smooth_factor, eval_power
-from cryptography318.linalg.linalg import binary_kernel, dot
-from cryptography318.prime.prime import primesieve, quadratic_residue, sqrt_mod
+import numpy as np
 
+from cryptography318.linalg import kernel_gf2
+from cryptography318.prime.prime import primesieve, quadratic_residue, sqrt_mod
+from cryptography318.utils.utils import n_digits, smooth_factor
 
-MIN_A_FACTOR = 2000
-MAX_A_FACTOR = 4000
+# Constants for SIQS algorithm
+MIN_A_FACTOR = 2000  # Smallest factor of a
+MAX_A_FACTOR = 4000  # Largest factor of a
 MIN_N_FACTORS = 20
 TRIALS_A = 30
 TRIAL_ERROR_MARGIN = 25
-REQUIRED_RELATIONS_RATIO = 1.05
-TRIALS_LINALG = 5
+REQUIRED_RELATIONS_RATIO = 1.05  # Required relations-found:factor-base-size ratio (how tall should matrix be)
+TRIALS_LINALG = 5  # Number of allowed attempts at solving linear system before giving up
 
 relations_found = 0
 min_sieve = 0
 loud_print = True
 
 a = b = 0
 B = []
@@ -34,34 +36,42 @@
 smooth_u = []
 smooth_t = []
 
 rand = Random()
 
 
 class QSPoly(Callable[[int], int]):
-
     __slots__ = "args",
 
     def __new__(cls, *args):
         self = super().__new__(cls)
         self.args = [*args]
         return self
 
-    def __call__(self, x: int) -> int:
+    def __call__(self, x):
         return reduce(lambda y, z: (y * x) + z, self.args, 0)
 
 
 def l_print(*args, **kwargs):
     global loud_print
 
     if loud_print:
         print(*args, **kwargs)
 
 
+l_print.__doc__ = print.__doc__
+
+
 def choose_f(digits):
+    """
+    Choose size of factor base. Hard coded values for sizes of n.
+
+    :param digits: Number of digits in n
+    :return: Size of factor base, f
+    """
     if digits < 38:
         return 4200
     elif digits < 40:
         return 5600
     elif digits < 42:
         return 7000
     elif digits < 44:
@@ -90,29 +100,25 @@
     elif digits < 88:
         return 196608
     else:
         return 589824
 
 
 def init_siqs(n, *, fp=None):
-
     global factor_base, t_sqrt, log_p, primes, soln1, soln2
 
     F = choose_f(n_digits(n))
 
     l_print(f"F: {F}")
 
-    p = 1
-    if fp is None:
-        primesieve.extend(F)
-        primes = primesieve[:F]
-    else:
-        with open(fp, "r") as prime_file:
-            while p < F:
-                primes.append(p := int(prime_file.readline()))
+    if fp is not None:
+        primesieve.load(fp)
+
+    primesieve.extend(F)
+    primes = [*primesieve.range(F)]
 
     l_print(f"primes < F: {len(primes)}")
 
     for prime in primes:
         if quadratic_residue(n, prime):
             factor_base.append(prime)
 
@@ -155,17 +161,17 @@
         raise ValueError("Not enough factors in factor base, try increasing F")
 
     target = isqrt(n + n) // m
     min_a = target / sqrt((factor_base[stop] + factor_base[start]) / 2)
     opt_ratio = 0.9
 
     a_factors = set()
-    best_ratio = None   # type: None | float
+    best_ratio = None  # type: None | float
 
-    # Try several different ones to find the a approximately closest to our target
+    # Try several ones to find the approximately closest to our target
     for _ in range(TRIALS_A):
 
         A = 1
         tmp_factors = set()
         while A < min_a:
             i = rand.randrange(start, stop)
             if i not in tmp_factors:
@@ -180,22 +186,21 @@
 
     set_fb = set(range(len(factor_base)))
     a_non_factors = set_fb - a_factors
 
 
 def first_poly(n, m):
     """
-    Given number to be factored and sieve range, compute a as the product of primes in the
-    factor base, and from that b such that a | b * b - n. Use this coefficients to
+    Given number to be factored and sieve range, compute `a` as the product of primes in the
+    factor base, and from that b such that a | b * b - n. Use these coefficients to
     create two polynomials, one used for finding smooth numbers and the other for finding
     the square root of the value square to find a smooth output.
-
-    :param n: number to be factored
+    :param n:number to be factored
     :param m: sieve range
-    :returns: two polynomials (ax + b)^2 - n and ax + b
+    :return: two polynomials (ax + b)^2 - n and ax + b
     """
 
     global a, b, B, factor_base, t_sqrt, B_ainv_2, a_factors, a_non_factors
 
     smooth_a(n, m)
 
     B = []
@@ -235,15 +240,14 @@
         soln1[p] = (a_inv * (t - b)) % prime
         soln2[p] = (a_inv * (-t - b)) % prime
 
     return QSPoly(a * a, 2 * a * _b, _b * _b - n), QSPoly(a, _b)
 
 
 def next_poly(i, n):
-
     global b, B, a_non_factors, soln1, soln2, B_ainv_2, factor_base
 
     v = 1
     j = i
     while not j & 1:
         j >>= 1
         v += 1
@@ -301,39 +305,31 @@
 
 def vec_matmul_T(vector, matrix):
     """
     Vector x matrix multiplication that takes in matrix
     already transposed, to save time when multiplying against the
     same matrix repeatedly.
     """
-    return [dot(vector, row) for row in matrix]
+
+    # Cast to Python int so that when we take power later it doesn't throw overflow error
+    return (int(vector @ row) // 2 for row in matrix)
 
 
 def solve_matrix(n):
     global smooth_t, smooth_u, primes
 
-    mod2 = []
-    T = []
-    for i in range(len(smooth_u[0])):
-        mod2.append([])
-        T.append([])
-        for j in range(len(smooth_u)):
-            mod2[i].append(smooth_u[j][i] % 2)
-            T[i].append(smooth_u[j][i])
-
-    kernel = binary_kernel(mod2)
-
-    for vector in kernel:  # iterate over basis of kernel
-        powers = map(lambda v: v // 2, vec_matmul_T(vector, T))
-        x = 1
-        for j, k in zip(vector, smooth_t):
-            if j:
-                x *= k
+    T = np.array(smooth_u, dtype=object).transpose()
+    kernel = kernel_gf2(T)
+
+    for vector in kernel:
+        powers = vec_matmul_T(vector, T)
 
-        y = eval_power(powers, primes)
+        # We need to do this instead of dot because dot will return the sum instead of product
+        x = prod(k for j, k in zip(vector, smooth_t) if j)
+        y = prod(pow(p, e) for p, e in zip(primes, powers))
         p, q = gcd(x + y, n), gcd(x - y, n)
 
         if 1 < p < n:
             return p
         if 1 < q < n:
             return q
 
@@ -350,20 +346,19 @@
     References
     ----------
     https://citeseerx.ist.psu.edu/viewdoc/download;jsessionid=53C827A542A8A950780D34E79261FF99?doi=10.1.1.26.6924&rep=rep1&type=pdf
     https://github.com/skollmann/PyFactorise/blob/master/factorise.py
     https://www.rieselprime.de/ziki/Self-initializing_quadratic_sieve
 
     :param n: number to be factored
-    :param fp: file containing list of primes with newline as the delimiter
-    :param loud: boolean determining if all information is printed or just factor
+    :param fp: file containing list of primes
+    :param loud: if information should be printed during execution
     :return: factor of n if one exists, otherwise None
-    :rtype: int | None
     """
-    global min_sieve, factor_base, relations_found, a_factors, loud_print
+    global min_sieve, factor_base, relations_found, a_factors, loud_print, smooth_u, smooth_t
 
     loud_print = loud
 
     # Initialize factor base, square root N mod p, and log p for all primes p
     # where N is a quadratic residue mod p
     init_siqs(n, fp=fp)
     required_relations = int(len(factor_base) * REQUIRED_RELATIONS_RATIO)
@@ -381,26 +376,33 @@
     g, h = first_poly(n, m)
     for _ in range(TRIALS_LINALG):
         l_print("Finding relations...")
         while relations_found < required_relations:
             sieve_array = sieve(m)
             trial_division(sieve_array, m, g, h)
 
+            # If we have found anymore relations, print
             if relations_found >= last_printed:
                 last_printed = relations_found
                 l_print(f"\r{relations_found}/{required_relations}", end="")
 
             if i >= n_poly:
                 g, h = first_poly(n, m)
                 n_poly = pow(2, len(a_factors) - 1) - 1
                 i = 0
             else:
                 g, h = next_poly(i, n)
 
             i += 1
 
-        if (factor := solve_matrix(n)) is not None:
+        l_print()
 
+        if (factor := solve_matrix(n)) is not None:
             l_print(f"Factor: {factor}")
             return factor
+        else:
+            # Reset relations found and smooth values found
+            last_printed = relations_found = 0
+            smooth_u = []
+            smooth_t = []
 
     return None
```

### Comparing `cryptography318-0.3.2/cryptography318/prime/bailliepsw_helper.py` & `cryptography318-0.4.0/cryptography318/prime/bailliepsw_helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This file is directly from https://github.com/smllmn/baillie-psw excluding jacobi. It is
 included in a project otherwise consisting of entirely original work because my focus
 was largely on factoring, but since the Miller-Rabin primality test is only deterministic
-up to 3317044064679887385961981 and I needed to confirm that integers larger than that limit
+up to 3317044064679887385961981, and I needed to confirm that integers larger than that limit
 were composite before factoring, I included this project as a further primality test.
 """
 
 
 def D_chooser(candidate):
     """Choose a D value suitable for the Baillie-PSW test - from internet"""
 
@@ -21,90 +21,90 @@
     """Helper function that returns suitable integer values
     for Lucas pseudoprime test - from internet"""
 
     k, n, U, V, P, Q, D = map(int, (k, n, U, V, P, Q, D))
     digits = list(map(int, str(bin(k))[2:]))
     subscript = 1
     for digit in digits[1:]:
-        U, V = U*V % n, (pow(V, 2, n) - 2*pow(Q, subscript, n)) % n
+        U, V = U * V % n, (pow(V, 2, n) - 2 * pow(Q, subscript, n)) % n
         subscript <<= 1
         if digit == 1:
-            if not (P*U + V) & 1:
-                if not (D*U + P*V) & 1:
-                    U, V = (P*U + V) >> 1, (D*U + P*V) >> 1
+            if not (P * U + V) & 1:
+                if not (D * U + P * V) & 1:
+                    U, V = (P * U + V) >> 1, (D * U + P * V) >> 1
                 else:
-                    U, V = (P*U + V) >> 1, (D*U + P*V + n) >> 1
-            elif not (D*U + P*V) & 1:
-                U, V = (P*U + V + n) >> 1, (D*U + P*V) >> 1
+                    U, V = (P * U + V) >> 1, (D * U + P * V + n) >> 1
+            elif not (D * U + P * V) & 1:
+                U, V = (P * U + V + n) >> 1, (D * U + P * V) >> 1
             else:
-                U, V = (P*U + V + n) >> 1, (D*U + P*V + n) >> 1
+                U, V = (P * U + V + n) >> 1, (D * U + P * V + n) >> 1
             subscript += 1
             U, V = U % n, V % n
     return U, V
 
 
 def LucasPseudoPrime(n, D, P, Q):
     """Perform the Lucas probable prime test - from internet
     Test performed with D, P, Q, s.t. P = 1,
     Q = (1 - D) / 4, and D is an integer that satisfies Jacobi(D / n) = -1"""
 
-    U, V = U_V_subscript(n+1, n, 1, P, P, Q, D)
+    U, V = U_V_subscript(n + 1, n, 1, P, P, Q, D)
 
     if U != 0:
         return False
 
     d = n + 1
     s = 0
     while not d & 1:
         d >>= 1
         s += 1
 
-    U, V = U_V_subscript(n+1, n, 1, P, P, Q, D)
+    U, V = U_V_subscript(n + 1, n, 1, P, P, Q, D)
 
     if not U:
         return True
 
     for r in range(s):
-        U, V = (U*V) % n, (pow(V, 2, n) - 2*pow(Q, d*(2**r), n)) % n
+        U, V = (U * V) % n, (pow(V, 2, n) - 2 * pow(Q, d * (2 ** r), n)) % n
         if not V:
             return True
 
     return False
 
 
 def jacobi(a, n):
     """
     Function that returns Jacobi symbol, assuming n is odd - original
     --
     If n is odd prime: the Jacobi symbol for (a / n) = 0 iff
-    a reduces to 0 mod n, = 1 iff a is a quadratic residue
+    a reduces to 0 mod n, = 1 iff `a` is a quadratic residue
     s.t. there exists some c where c^2 = a mod n,
     = -1 iff there does not exist some c where c^2 = a mod n
     """
 
     # checks to see if n is odd
     if not n & 1:
         raise ValueError(f"modulus 'n' must be odd")
 
-    # if a is 0 or 1, automatically return a
+    # if `a` is 0 or 1, automatically return `a`
     if a in (0, 1):
         return a
 
-    # if a is not already mod n, reduce it mod n
+    # if `a` is not already mod n, reduce it mod n
     elif a != a % n:
         return jacobi(a % n, n)
 
-    # if a is even, it can be reduced until it is odd, multiplying
+    # if `a` is even, it can be reduced until it is odd, multiplying
     # the Legendre symbol for (a / n) for each iteration of a being even
     elif not a & 1:
 
         # checks if n = +/- 1 mod 8, multiplying by the result
         # of the Legendre symbol (a / n) = 1
         # otherwise, multiply result by Legendre symbol (a / n) = -1
         return jacobi(a >> 1, n) if n % 8 in (1, 7) else -jacobi(a >> 1, n)
 
     else:
 
-        # if a is odd, return Jacobi of (n / a)
+        # if `a` is odd, return Jacobi of (n / a)
         # if a and n both reduce to 3 mod 4, return the negative
         # otherwise, return (n / a)
         return -jacobi(n % a, a) if a % 4 == 3 == n % 4 else jacobi(n % a, a)
```

### Comparing `cryptography318-0.3.2/cryptography318/prime/prime.py` & `cryptography318-0.4.0/cryptography318/prime/prime.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,188 +1,319 @@
-from math import prod
-from random import randrange, choice
-from itertools import count
-from sympy.ntheory.primetest import is_square
+from collections import UserList
+from itertools import islice
+from math import isqrt, prod
 from pathlib import Path
+from random import choice, randrange
 
-from .bailliepsw_helper import LucasPseudoPrime, D_chooser
+from cryptography318.prime.bailliepsw_helper import D_chooser, LucasPseudoPrime
+from cryptography318.utils.utils import binary_search, Details
 
 
-module = Path(__file__).parent.absolute()
-if module.joinpath("primes.txt").is_file():
-    primesIO = open(str(module.joinpath("primes.txt")), "r")
-else:
-    primesIO = None
+isprime_details = Details(**{
+    "Miller-Rabin": None,
+    "Baillie-PSW": None,
+    "Direct": None,
+})
 
 
-class Sieve(object):
+def get_details():
+    global isprime_details
+    return str(isprime_details)
+
+
+class Sieve(UserList[int]):
     """
     Unbound list of primes starting at 2. Object is iterable, index-able, print-able, searchable,
     and extendable. Unless another specific use is required, import primesieve object as a global
     variable for use. Intended to help with primality tests and factoring integers.
     """
 
-    def __init__(self):
-        self._list = [2, 3, 5, 7, 11, 13]
-
-    def __repr__(self):
-        return repr(self._list)
+    def __init__(self, data=None):
+        if data is None:
+            data = [2, 3, 5, 7, 11, 13]
+        super().__init__(data)
+
+    def search(self, value, *args):
+        """
+        Search for one or more values in the list. This is essentially
+        list.index() except when our list does not contain the value,
+        we will return the indices of the bordering primes.
+
+        :param value:
+        :param args:
+        :return:
+        """
 
-    def __getitem__(self, item):
-        return self._list[item]
-
-    def __contains__(self, item):
-        return self._list.__contains__(item)
+        # If we are just searching for the one value, much easier
+        if not args:
+            try:
+                # Try to just find it in the list
+                return self.data.index(value)
+            except ValueError:
+                # We either got a value error because the data is within the bounds of the list
+                # but not a prime OR it is outside the bounds of the list and possibly prime.
+                # If outside the bounds, we can't do anything so raise a ValueError
+                if value > self.data[-1] or value < self.data[0]:
+                    raise ValueError(f"{{{value}}} is not contained within the primesieve")
+
+                # Otherwise we know the value was within the bounds of the list but composite
+                # so lets find and return the indices of the bordering primes
+                i = binary_search(self.data, value, exist=False)
+                if i is None:
+                    raise ValueError(f"{{{value}}} is not contained within the primesieve")
+                return i - 1, i
+
+        # sorted() gets it back into a list, but now we've made sure to remove duplicates and add value
+        values = sorted({value, *args})
+
+        # If the largest value is larger than our upper bound or the smallest value is smaller than our
+        # lower bound then we cannot return information for all values so raise an error
+        if values[-1] > self.data[-1] or values[0] < self.data[0]:
+            raise ValueError(f"{set(values)} are not contained within the primesieve")
 
-    def __len__(self):
-        return len(self._list)
+        indices = []
+        composite = []
+        comp_indices = []
 
-    def __iter__(self):
-        nprimes = len(self._list) + 1
-        for i in count(1):
-            if i == nprimes:
-                return
-            yield self._list[i - 1]
+        last_index = 0
 
-    def search(self, *args):
-        if len(args) == 1:
-            item = args[0]
+        # Try to get indices using index, add all that fail to our list, as well as the last prime
+        # we saw before the fail
+        for j, v in enumerate(values):
             try:
-                return self._list.index(item)
+                last_index = self.data.index(v)
+                indices.append(last_index)
             except ValueError:
-                if item > self._list[-1] or item < self._list[0]:
-                    raise ValueError(f"{item} is not in the sieve list")
+                # Keep track of where we should insert this into indices
+                comp_indices.append(j)
+                # Add the composite value and the index of the last prime before we searched for this one
+                composite.append((v, last_index))
+
+        # If all values being searched for were primes, just return the values
+        if len(composite) == 0:
+            return tuple(indices)
+
+        for k, (v, j) in enumerate(composite):
+            i = binary_search(self.data, v, start=j, exist=False)
+            if i is None:
+                raise ValueError(f"{{{value}}} is not contained within the primesieve")
+            indices.insert(comp_indices[k], (i - 1, i))
 
-                start_idx = 0
-                for p in primesieve:
-                    if p > item:
-                        break
-                    start_idx += 1
-                return start_idx - 1, start_idx
-
-        args = sorted(set(args))  # in case args aren't sorted, they need to be, set call removes duplicates
-        if args[-1] > self._list[-1] or args[0] < self._list[0]:
-            raise ValueError(f"one (or more) of {args} is not in the sieve list")
-
-        indices = []
-        nargs = len(args)
-        i = 0
-        curr = args[0]
-        max_idx = -1
-
-        # try to get indices using index, if any fail, start from there
-        try:
-            while 1:
-                max_idx = self._list.index(curr)
-                indices.append(max_idx)
-                i += 1
-                if i == nargs:
-                    return tuple(*indices)
-                curr = args[i]
-        except ValueError:
-            pass
-
-        start_idx = max_idx + 1
-
-        # start at max_idx + 1, 0 if none were indexed, or index + 1 of last found prime
-        for p in self._list[start_idx:]:
-            if p == curr:
-                indices.append(start_idx)
-                i += 1
-                if i == nargs:
-                    return tuple(*indices)
-                curr = args[i]
-            elif p > curr:
-                indices.append((start_idx - 1, start_idx))
-                i += 1
-                if i == nargs:
-                    return tuple(*indices)
-                curr = args[i]
-            start_idx += 1
+        return tuple(indices)
 
     def extend(self, n):
+        """
+        Extends the list to include all primes up to ``n`` inclusive.
+        If ``n`` is composite, list extends to include the smallest
+        prime larger than ``n``.
+
+        :param n: upper bound
+        :return: None
+        """
         if n <= self.tail:
             return
-        elif primesIO is not None:
-            primesIO.seek(0)
-            add = False
-            while line := primesIO.readline():
-                p = int(line.strip("\n"))
-                if p >= n:
-                    return
-                elif add:
-                    self._list.append(p)
-                elif p > self.tail:
-                    add = True
-                    self._list.append(p)
 
         p = self.tail
-        while (p := next_prime(p)) <= n:
-            self._list.append(p)
+        while True:
+            p = next_prime(p)
+            self.data.append(p)
+            if p > n:
+                return
+
+    def load(self, file=None, overwrite=False):
+        """
+        Loads primes from text file into sieve.
+        :param file: Reads from primes.txt local to project
+        :param overwrite: If provided list of primes should replace existing list
+        """
+
+        if file is None:
+            fp = Path(__file__).parent.absolute().joinpath("primes.txt")
+        else:
+            fp = Path(file)
+
+        if not fp.is_file():
+            raise FileNotFoundError(f"Unable to locate file {fp}")
+
+        with open(fp, "r") as infile:
+
+            # If we are overwriting and just accepting this as the list
+            if overwrite:
+                self.data = []
+                for line in infile:
+                    self.data.append(int(line.strip()))
+                return
+
+            first_prime = int(infile.readline().strip())
+
+            # If we are starting from first prime, read all and then check to see if it read a higher prime
+            if first_prime == 2:
+                data = [2]
+                for line in infile:
+                    data.append(int(line.strip()))
+                if data[-1] > self.data[-1]:
+                    self.data = data
+                return
+
+            # If first prime is somewhere in list, find where it is and start adding from there
+            if first_prime < self.data[-1]:
+                # If this throws error then first_prime is not real prime
+                start_index = self.data.index(first_prime)
+                data = [first_prime]
+                for line in infile:
+                    data.append(int(line.strip()))
+
+                if data[-1] > self.data[-1]:
+                    self.data = self.data[:start_index] + data
+                return
+
+            # If first prime is our last prime, simple, just start appending to our list
+            if first_prime == self.data[-1]:
+                for line in infile:
+                    self.data.append(int(line.strip()))
+                return
+
+            # If first prime read is next sequentially, we can accept it
+            if next_prime(self.data[-1]) == first_prime:
+                self.data.append(first_prime)
+                for line in infile:
+                    self.data.append(int(line.strip()))
+                return
+
+            # Otherwise we have discontinuous list and have to throw error
+            raise ValueError(f"List of primes starting with {first_prime} is not continuous with current primesieve")
 
     def range(self, a, b=None):
+        """
+        Returns all primes within the given range. If a lower bound is not given
+        the range starts at 2.
+
+        :param a: first bound
+        :param b: upper bound
+        :return: all primes in range [a, b)
+        """
         if b is None:
             b = a
             a = 2
 
+        # Make sure that we've got a valid sized range
         if b <= a:
-            return
+            return None
 
-        if b > self._list[-1]:
-            self.extend(b)
+        # Extend sieve up to upper bound inclusive
+        self.extend(b)
 
-        i = self.search(a)
+        # Get indices of upper and lower bounds
+        i, j = self.search(a, b)
         if isinstance(i, tuple):
             i = i[1]
 
-        nprimes = len(self._list)
-        while i < nprimes:
-            n = self._list[i]
-            i += 1
-            if n <= b:
-                yield n
-            else:
-                return
+        # If it's a tuple, lets take the lower since we need to add 1 later since if it's not a tuple
+        # we want to make sure we include that prime
+        if isinstance(j, tuple):
+            j = j[0]
+
+        return islice(self.data, i, j + 1)
 
     @property
     def list(self):
-        return self._list
+        return self.data
 
     @property
     def tail(self):
-        return self._list[-1]
+        return self.data[-1]
 
 
 primesieve = Sieve()
 
 
-def miller_rabin(n, k=40):
-    """MRPrimality test reduces n - 1 to a power of 2 and an odd number, then
-    tests if random a is a witness of n's composite-ness, testing with
-    k random a's"""
+def is_square(n):
+    """
+    Replacement for Sympy's is_square function that follows almost
+    explicitly the routine outlined in the link. The major difference
+    is that due to the speed of Python's integer, we don't need
+    to pre-mod our value to increase the speed of future mods, for each
+    test we can mod n directly.
+
+    References
+    ----------
+    https://mersenneforum.org/showpost.php?p=110896
 
-    if (res := known_prime(n)) is not None:
-        return res
+    :param n: integer
+    :return: if a * a == n for some integer a
+    """
+    if n < 0:
+        return False
+    elif n in (0, 1):
+        return True
+    elif n & 1:
+        return False
+
+    m = n & 127  # n % 128
+    if (m * 0x8bc40d7d) & (m * 0xa1e2f5d1) & 0x14020a:
+        return False
+
+    m = n % 63
+    if (m * 0x3d491df7) & (m * 0xc824a9f9) & 0x10f14008:
+        return False
+
+    m = n % 25
+    if (m * 0x1929fc1b) & (m * 0x4c9ea3b2) & 0x51001005:
+        return False
+
+    m = 0xd10d829a * (n % 31)
+    if m & (m + 0x672a5354) & 0x21025115:
+        return False
+
+    m = n % 23
+    if (m * 0x7bd28629) & (m * 0xe7180889) & 0xf8300:
+        return False
+
+    m = n % 19
+    if (m * 0x1b8bead3) & (m * 0x4d75a124) & 0x4280082b:
+        return False
+
+    m = n % 17
+    if (m * 0x6736f323) & (m * 0x9b1d499) & 0xc0000300:
+        return False
+
+    m = n % 11
+    if (m * 0xabf1a3a7) & (m * 0x2612bf93) & 0x45854000:
+        return False
+
+    m = isqrt(n)
+    return m * m == n
+
+
+def miller_rabin(n, k=40, *, details=False):
+    """
+    MRPrimality test reduces n - 1 to a power of 2 and an odd number, then
+    tests if random `a` is a witness of n's composite-ness, testing with
+    k random a's
+    """
 
     d = n - 1
     r = 0
     while not d & 1:
         r += 1
         d >>= 1
 
     for _ in range(k):
         if not _mr_test(d, n):
+            if details:
+                global isprime_details
+                isprime_details.add_details("Miller-Rabin", f"{d} is a witness to {n}'s composite-ness")
             return False
 
     return True
 
 
 def _mr_test(d, n):
     """Helper function for miller_rabin which uses previously found d to
-    check if random a is a witness to n's composite-ness"""
+    check if random `a` is a witness to n's composite-ness"""
 
     a = randrange(2, n - 1)
     x = pow(a, d, n)
     if x == 1 or x == n - 1:
         return True
 
     # doubles d every time until d returns to original n-1 value
@@ -212,39 +343,53 @@
         q >>= 1
         k += 1
 
     a = pow(a, q, n)
     if a == 1 or a == n - 1:
         return True
     for _ in range(k):
+        # If we found any a^2 = -1 mod n then we know `a` is not a witness to n's compositeness
         if a == -1 or a == n - 1:
             return True
+
+        # If we found an a^2 = 1 mod n where a != +/- 1 then a is definitely composite
         elif a == 1:
             return False
         a = pow(a, 2, n)
 
     return False
 
 
-def miller_rabin_bases(bases, n):
+def miller_rabin_bases(bases, n, *, details=False):
     """Helper function that allows for a list of witnesses to be tested
     using MillerRabin_base_a function"""
+    global isprime_details
 
     for a in bases:
         if not _miller_rabin_base_a(a, n):
+            if details:
+                isprime_details.add_details("Miller-Rabin", f"{a} is witness to {n}'s compositeness")
             return False
+    if details:
+        isprime_details.add_details("Miller-Rabin", f"{n} is probably prime")
     return True
 
 
 def baillie_psw(n, mr=True):
-    """Perform the Baillie-PSW probabilistic primality test on candidate."""
+    """
+    Perform the Baillie-PSW probabilistic primality test on candidate.
+
+    :param n: prime candidate
+    :param mr: if Miller-Rabin test base 2 should be used
+    :return:
+    """
 
     # Check divisibility by a short list of primes less than 50
-    if known_prime(n) is not None:
-        return known_prime(n)
+    if (res := known_prime(n)) is not None:
+        return res
 
     # Now perform the Miller-Rabin primality test base 2
     if mr and not _miller_rabin_base_a(2, n):
         return False
 
     # Checks if number has square root
     if is_square(n):
@@ -272,111 +417,147 @@
         if n == p:
             return True
         elif n % p == 0:
             return False
     return None
 
 
-def isprime(n):
+def isprime(n, *, details=False):
     """
     IsPrime function returns False iff the prime-candidate is composite, and True
     if the prime-candidate is probably prime.
 
     Uses deterministic variants of the Miller-Rabin Primality test, which, through
     the use of specific bases and ranges, can deterministically return True iff
     candidate is prime for n < 3317044064679887385961981. For all larger n,
-    there is no  known set of bases that makes the MR test deterministic. Thus a
+    there is no  known set of bases that makes the MR test deterministic. Thus, a
     SPRP-test consisting of a Strong Lucas Pseudo-prime test and a Miller-Rabin
-    test with 20 random bases a, s.t. 1 < a < n is used to determine if candidate is
+    test with 20 random bases `a`, s.t. 1 < a < n is used to determine if candidate is
     probably prime.
     """
 
+    global isprime_details
+    if details:
+        isprime_details.clear_details()
+
     if n < 2:
+        if details:
+            isprime_details.add_details("Direct", f"{n} < 2")
         return False
 
     elif n < 10:
+        if details:
+            isprime_details.add_details("Direct", f"{n} < 10")
         return bool([0, 0, 1, 1, 0, 1, 0, 1, 0, 0, 0][n])
 
     # check for odds
     elif not n & 1:
+        if details:
+            isprime_details.add_details("Direct", f"{n} is even")
         return False
 
     # check for all other instances n != 6k +/- 1
     elif not n % 3:
+        if details:
+            isprime_details.add_details("Direct", f"{n} is divisible by 3")
         return False
 
     # This step is pretty useless unless primesieve is being used for something else or is
     # being purposefully generated, since it is constructed only with first 6 primes
     global primesieve
     if n in primesieve:
+        if details:
+            isprime_details.add_details("Direct", f"{n} is known prime")
         return True
     elif n < 2047:
-        return miller_rabin_bases([2], n)
+        return miller_rabin_bases([2], n, details=details)
     elif n < 1373653:
-        return miller_rabin_bases([2, 3], n)
+        return miller_rabin_bases([2, 3], n, details=details)
     elif n < 9080191:
-        return miller_rabin_bases([31, 73], n)
+        return miller_rabin_bases([31, 73], n, details=details)
     elif n < 1050535501:
-        return miller_rabin_bases([336781006125, 9639812373923155], n)
+        return miller_rabin_bases([336781006125, 9639812373923155], n, details=details)
     elif n < 3215031751:
-        return miller_rabin_bases([2, 3, 5, 7], n)
+        return miller_rabin_bases([2, 3, 5, 7], n, details=details)
     elif n < 4759123141:
-        return miller_rabin_bases([2, 7, 61], n)
+        return miller_rabin_bases([2, 7, 61], n, details=details)
     elif n < 1122004669633:
-        return miller_rabin_bases([2, 13, 23, 1662803], n)
+        return miller_rabin_bases([2, 13, 23, 1662803], n, details=details)
     elif n < 55245642489451:
-        return miller_rabin_bases([2, 141889084524735, 1199124725622454117, 11096072698276303650], n)
+        return miller_rabin_bases([2, 141889084524735, 1199124725622454117, 11096072698276303650], n, details=details)
     elif n < 7999252175582851:
-        return miller_rabin_bases([2, 4130806001517, 149795463772692060, 186635894390467037, 3967304179347715805], n)
+        return miller_rabin_bases([2, 4130806001517, 149795463772692060, 186635894390467037, 3967304179347715805], n, details=details)
     elif n < 18446744073709551616:
-        return miller_rabin_bases([2, 325, 9375, 28178, 450775, 9780504, 1795265022], n)
+        return miller_rabin_bases([2, 325, 9375, 28178, 450775, 9780504, 1795265022], n, details=details)
     elif n < 318665857834031151167461:
-        return miller_rabin_bases([2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37], n)
+        return miller_rabin_bases([2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37], n, details=details)
     elif n < 3317044064679887385961981:
-        return miller_rabin_bases([2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41], n)
+        return miller_rabin_bases([2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41], n, details=details)
     else:
-        return miller_rabin(n, k=40) and baillie_psw(n, mr=False)
+        res = miller_rabin(n, k=40, details=details)
+        if not res:
+            return False
+
+        # If miller rabin didn't say it was composite, then we should note that we used Baillie-PSW
+        if details:
+            isprime_details.add_details("Baillie-PSW", True)
+        return baillie_psw(n, mr=False)
 
 
 def randprime(a: int, b: int = None):
     """Uses combination of Miller-Rabin and Baillie-PSW primality tests to generate random prime
 
+    Note
+    ----
+    If no lower bound is specified, 2 will never be generated, since bounds of sampling are set [3, b)
+
     :param a: integer starting point of range for random prime
     :param b: integer stopping point of range for random prime (exclusive)
     """
 
     # determines if user entered a lower and upper limit or just an upper
     if b is None:
-        b = a
-        a = 3
+        b, a = a, 3
 
     base_2 = a == 2
-    a = a | 1  # if base_2, a isn't used, if not base 2 then even a is not prime so adjust to odd affects nothing
+    a = a | 1  # If base_2, `a` isn't used, if not base 2 then even `a` is not prime so adjust to odd affects nothing
 
     global primesieve
     if b <= primesieve.tail:
         start, stop = primesieve.search(a), primesieve.search(b)
         if isinstance(start, tuple):
             start = start[1]
         if isinstance(stop, tuple):
             stop = stop[0]
         return choice(primesieve[start:stop])
 
-    # if base_2, uses 2 as a base and increments by 1 (default) for generating random int
-    # if base != 2, generates random int starting at lower limit, incrementing by 2
-    while 1:
-        prime = randrange(2, b) if base_2 else randrange(a, b, 2)
+    # If base_2 is True then it uses 2 as a base and increments by 1 (default) for generating random int
+    # If base != 2, generates random int starting at lower limit, incrementing by 2
+    if base_2:
+        def rprime():
+            return randrange(2, b)
+    else:
+        def rprime():
+            return randrange(a, b, 2)
+
+    while True:
+        prime = rprime()
         if isprime(prime):
             return prime
 
 
 def confirm_prime(n):
-    """Uses infinitely deterministic AKS (Agrawal-Kayal-Saxena) primality test which
+    """Uses deterministic AKS (Agrawal-Kayal-Saxena) primality test which
     returns True if-and-only-if n is prime"""
 
+    if n < 2:
+        return False
+    elif n == 2:
+        return True
+
     global primesieve
     if n in primesieve:
         return True
 
     # generates the n-th row of Pascal's triangle, if any of the coefficients != 0 mod n, n is not prime
     for k in range(1, (n + 1) // 2):
         res = 1
@@ -403,24 +584,24 @@
             i = i[1]
         else:
             i += 1
         return primesieve[i]
 
     # Ensures that n starts at the nearest 6k + 1
 
-    # a is the closest 6k + 1 to n
+    # `a` is the closest 6k + 1 to n
     a = n - (n % 6) + 1
     if a <= n:
 
         # If a <= n, try 6k + 5, only return if that's greater than n
         a += 4
         if a > n and isprime(a):
             return a
 
-        # Otherwise, get a to 6k + 1, if this is prime, it's guaranteed > n so return
+        # Otherwise, get `a` to 6k + 1, if this is prime, it's guaranteed > n so return
         a += 2
         if isprime(a):
             return a
 
         # Otherwise, since 6k + 1 above n didn't work, set n to 6k + 5 for below loop
         n = a + 4
     elif isprime(a):
@@ -431,15 +612,15 @@
 
         # Otherwise, start off n at a + 4 which is (6k + 1) + 4
         n = a + 4
 
     assert n % 6 == 5
 
     # Iterate up through each 6k +/- 1
-    while 1:
+    while True:
         if isprime(n):
             return n
         n += 2
         if isprime(n):
             return n
         n += 4
 
@@ -482,14 +663,18 @@
         if isprime(n):
             return n
         n -= 4
         if isprime(n):
             return n
         n -= 2
 
+        # If we are sure that n passed was larger than 2, and we somehow end up below 2, just return 2
+        if n < 2:
+            return 2
+
 
 def prime_range(a, b=None):
     """Constructs list of a <= primes < b"""
     if b is None:
         b = a
         a = 1
```

### Comparing `cryptography318-0.3.2/cryptography318.egg-info/PKG-INFO` & `cryptography318-0.4.0/cryptography318.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: cryptography318
-Version: 0.3.2
+Version: 0.4.0
 Summary: A set of functions useful in cryptography and linear algebra
 Home-page: https://github.com/aarpyy/Cryptography
 Author: Andrew Carpenter
-Author-email: acarpent@oberlin.edu
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: andrewcarp00@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: License :: Public Domain
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
@@ -34,9 +32,8 @@
 
 ## Install
 ```angular2html
 $ pip install cryptography318
 ```
 
 ### License
-This package is unlicensed and not intended for public use.
-
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `cryptography318-0.3.2/cryptography318.egg-info/SOURCES.txt` & `cryptography318-0.4.0/cryptography318.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -12,14 +12,12 @@
 cryptography318/factor/__init__.py
 cryptography318/factor/curve.py
 cryptography318/factor/elliptic.py
 cryptography318/factor/factor.py
 cryptography318/factor/siqs.py
 cryptography318/linalg/__init__.py
 cryptography318/linalg/linalg.py
-cryptography318/linalg/matrix.py
-cryptography318/linalg/vector.py
 cryptography318/prime/__init__.py
 cryptography318/prime/bailliepsw_helper.py
 cryptography318/prime/prime.py
 cryptography318/utils/__init__.py
 cryptography318/utils/utils.py
```

### Comparing `cryptography318-0.3.2/setup.py` & `cryptography318-0.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         name='cryptography318',
         long_description=long_description,
         long_description_content_type='text/markdown',
         version=version,
         description='A set of functions useful in cryptography and linear algebra',
         url='https://github.com/aarpyy/Cryptography',
         author='Andrew Carpenter',
-        author_email='acarpent@oberlin.edu',
+        author_email='andrewcarp00@gmail.com',
         packages=["cryptography318"] + modules,
         install_requires=requirements,
         python_requires=">=3.10",   # Python 3.10 now required since zip(*, strict=True) is used
         classifiers=[
             'Development Status :: 2 - Pre-Alpha',
             'Intended Audience :: Education',
             'License :: Public Domain',
```

