# Comparing `tmp/bayesmsd-0.1.2.tar.gz` & `tmp/bayesmsd-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/simongh/gitlibs/bayesmsd/dist/.tmp-agz2ngjs/bayesmsd-0.1.2.tar", last modified: Fri Feb 10 20:55:30 2023, max compression
+gzip compressed data, was "/home/simongh/gitlibs/bayesmsd/dist/.tmp-5qcqv3ov/bayesmsd-0.1.3.tar", last modified: Mon Jun 19 19:35:30 2023, max compression
```

## Comparing `bayesmsd-0.1.2.tar` & `bayesmsd-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 simongh   (8090) simongh   (8090)        0 2023-02-10 20:55:30.000000 bayesmsd-0.1.2/
--rw-rw-r--   0 simongh   (8090) simongh   (8090)     1074 2023-02-10 17:39:20.000000 bayesmsd-0.1.2/LICENSE
--rw-rw-r--   0 simongh   (8090) simongh   (8090)     4238 2023-02-10 20:55:30.000000 bayesmsd-0.1.2/PKG-INFO
--rw-rw-r--   0 simongh   (8090) simongh   (8090)     2394 2023-02-10 17:40:19.000000 bayesmsd-0.1.2/README.md
-drwxrwxr-x   0 simongh   (8090) simongh   (8090)        0 2023-02-10 20:55:30.000000 bayesmsd-0.1.2/bayesmsd/
--rw-rw-r--   0 simongh   (8090) simongh   (8090)     3125 2023-02-10 17:39:20.000000 bayesmsd-0.1.2/bayesmsd/__init__.py
--rw-rw-r--   0 simongh   (8090) simongh   (8090)      395 2023-02-10 17:39:20.000000 bayesmsd-0.1.2/bayesmsd/cython_imports.py
--rw-rw-r--   0 simongh   (8090) simongh   (8090)     6418 2023-02-10 17:39:20.000000 bayesmsd-0.1.2/bayesmsd/deco.py
--rw-rw-r--   0 simongh   (8090) simongh   (8090)    27426 2023-02-10 17:39:20.000000 bayesmsd-0.1.2/bayesmsd/fit.py
--rw-rw-r--   0 simongh   (8090) simongh   (8090)     8697 2023-02-10 17:39:20.000000 bayesmsd-0.1.2/bayesmsd/gp.py
--rw-rw-r--   0 simongh   (8090) simongh   (8090)    34190 2023-02-10 17:39:20.000000 bayesmsd-0.1.2/bayesmsd/lib.py
--rw-rw-r--   0 simongh   (8090) simongh   (8090)     8204 2023-02-10 17:39:20.000000 bayesmsd-0.1.2/bayesmsd/parameters.py
--rw-rw-r--   0 simongh   (8090) simongh   (8090)    27952 2023-02-10 17:39:20.000000 bayesmsd-0.1.2/bayesmsd/profiler.py
-drwxrwxr-x   0 simongh   (8090) simongh   (8090)        0 2023-02-10 20:55:30.000000 bayesmsd-0.1.2/bayesmsd/src/
--rw-rw-r--   0 simongh   (8090) simongh   (8090)   935878 2023-02-10 17:39:20.000000 bayesmsd-0.1.2/bayesmsd/src/gp.c
--rw-rw-r--   0 simongh   (8090) simongh   (8090)     3562 2023-02-10 17:39:20.000000 bayesmsd-0.1.2/bayesmsd/src/gp_py.py
-drwxrwxr-x   0 simongh   (8090) simongh   (8090)        0 2023-02-10 20:55:30.000000 bayesmsd-0.1.2/bayesmsd.egg-info/
--rw-rw-r--   0 simongh   (8090) simongh   (8090)     4238 2023-02-10 20:55:30.000000 bayesmsd-0.1.2/bayesmsd.egg-info/PKG-INFO
--rw-rw-r--   0 simongh   (8090) simongh   (8090)      450 2023-02-10 20:55:30.000000 bayesmsd-0.1.2/bayesmsd.egg-info/SOURCES.txt
--rw-rw-r--   0 simongh   (8090) simongh   (8090)        1 2023-02-10 20:55:30.000000 bayesmsd-0.1.2/bayesmsd.egg-info/dependency_links.txt
--rw-rw-r--   0 simongh   (8090) simongh   (8090)        1 2023-02-10 17:39:51.000000 bayesmsd-0.1.2/bayesmsd.egg-info/not-zip-safe
--rw-rw-r--   0 simongh   (8090) simongh   (8090)       53 2023-02-10 20:55:30.000000 bayesmsd-0.1.2/bayesmsd.egg-info/requires.txt
--rw-rw-r--   0 simongh   (8090) simongh   (8090)        9 2023-02-10 20:55:30.000000 bayesmsd-0.1.2/bayesmsd.egg-info/top_level.txt
--rw-rw-r--   0 simongh   (8090) simongh   (8090)      816 2023-02-10 20:54:43.000000 bayesmsd-0.1.2/pyproject.toml
--rw-rw-r--   0 simongh   (8090) simongh   (8090)       38 2023-02-10 20:55:30.000000 bayesmsd-0.1.2/setup.cfg
--rw-rw-r--   0 simongh   (8090) simongh   (8090)     1937 2023-02-10 17:39:20.000000 bayesmsd-0.1.2/setup.py
-drwxrwxr-x   0 simongh   (8090) simongh   (8090)        0 2023-02-10 20:55:30.000000 bayesmsd-0.1.2/tests/
--rw-rw-r--   0 simongh   (8090) simongh   (8090)    21232 2023-02-10 17:39:20.000000 bayesmsd-0.1.2/tests/test_bayesmsd.py
+drwxrwxr-x   0 simongh   (8090) simongh   (8090)        0 2023-06-19 19:35:30.000000 bayesmsd-0.1.3/
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)     1074 2023-02-10 17:39:20.000000 bayesmsd-0.1.3/LICENSE
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)     4238 2023-06-19 19:35:30.000000 bayesmsd-0.1.3/PKG-INFO
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)     2394 2023-02-12 18:07:24.000000 bayesmsd-0.1.3/README.md
+drwxrwxr-x   0 simongh   (8090) simongh   (8090)        0 2023-06-19 19:35:30.000000 bayesmsd-0.1.3/bayesmsd/
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)     3125 2023-02-12 18:07:24.000000 bayesmsd-0.1.3/bayesmsd/__init__.py
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)      395 2023-02-12 18:07:24.000000 bayesmsd-0.1.3/bayesmsd/cython_imports.py
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)     6882 2023-02-16 19:38:42.000000 bayesmsd-0.1.3/bayesmsd/deco.py
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)    27427 2023-06-19 19:34:34.000000 bayesmsd-0.1.3/bayesmsd/fit.py
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)     8697 2023-02-12 18:07:24.000000 bayesmsd-0.1.3/bayesmsd/gp.py
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)    34878 2023-02-16 19:38:39.000000 bayesmsd-0.1.3/bayesmsd/lib.py
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)     8204 2023-02-12 18:07:24.000000 bayesmsd-0.1.3/bayesmsd/parameters.py
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)    27952 2023-02-13 19:17:44.000000 bayesmsd-0.1.3/bayesmsd/profiler.py
+drwxrwxr-x   0 simongh   (8090) simongh   (8090)        0 2023-06-19 19:35:30.000000 bayesmsd-0.1.3/bayesmsd/src/
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)   937877 2023-02-17 17:08:53.000000 bayesmsd-0.1.3/bayesmsd/src/gp.c
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)     3562 2023-02-12 18:07:24.000000 bayesmsd-0.1.3/bayesmsd/src/gp_py.py
+drwxrwxr-x   0 simongh   (8090) simongh   (8090)        0 2023-06-19 19:35:30.000000 bayesmsd-0.1.3/bayesmsd.egg-info/
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)     4238 2023-06-19 19:35:30.000000 bayesmsd-0.1.3/bayesmsd.egg-info/PKG-INFO
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)      450 2023-06-19 19:35:30.000000 bayesmsd-0.1.3/bayesmsd.egg-info/SOURCES.txt
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)        1 2023-06-19 19:35:30.000000 bayesmsd-0.1.3/bayesmsd.egg-info/dependency_links.txt
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)        1 2023-02-10 17:39:51.000000 bayesmsd-0.1.3/bayesmsd.egg-info/not-zip-safe
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)       53 2023-06-19 19:35:30.000000 bayesmsd-0.1.3/bayesmsd.egg-info/requires.txt
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)        9 2023-06-19 19:35:30.000000 bayesmsd-0.1.3/bayesmsd.egg-info/top_level.txt
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)      816 2023-06-19 19:34:34.000000 bayesmsd-0.1.3/pyproject.toml
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)       38 2023-06-19 19:35:30.000000 bayesmsd-0.1.3/setup.cfg
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)     1937 2023-02-12 18:07:24.000000 bayesmsd-0.1.3/setup.py
+drwxrwxr-x   0 simongh   (8090) simongh   (8090)        0 2023-06-19 19:35:30.000000 bayesmsd-0.1.3/tests/
+-rw-rw-r--   0 simongh   (8090) simongh   (8090)    21247 2023-02-16 19:38:39.000000 bayesmsd-0.1.3/tests/test_bayesmsd.py
```

### Comparing `bayesmsd-0.1.2/LICENSE` & `bayesmsd-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bayesmsd-0.1.2/PKG-INFO` & `bayesmsd-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayesmsd
-Version: 0.1.2
+Version: 0.1.3
 Summary: Bayesian MSD fitting
 Author-email: Simon Grosse-Holz <sgh256@mit.edu>
 License: MIT License
         
         Copyright (c) 2022 Simon Grosse-Holz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bayesmsd-0.1.2/README.md` & `bayesmsd-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `bayesmsd-0.1.2/bayesmsd/__init__.py` & `bayesmsd-0.1.3/bayesmsd/__init__.py`

 * *Files identical despite different names*

### Comparing `bayesmsd-0.1.2/bayesmsd/deco.py` & `bayesmsd-0.1.3/bayesmsd/deco.py`

 * *Files 3% similar despite different names*

```diff
@@ -156,15 +156,25 @@
             phi = f/dt
             b = np.empty(len(phi), dtype=float)
             ind = phi > 0
             phi = phi[ind]
             b[ind] = ( (1+phi)**(a+2) + (1-phi)**(a+2) - 2 ) / ( phi**2 * (a+1) * (a+2) )
             b[~ind] = 1
 
-            return b*msdfun(dt, **kwargs) - 2*B + 2*noise2
+            out = b*msdfun(dt, **kwargs) - 2*B + 2*noise2
+
+            # In some edge cases, the MSD can get close to zero, i.e.
+            # numerically potentially negative.
+            if np.any(out < 0): # pragma: no cover
+                if np.min(out) > -1e-10:
+                    out[out < 0] = 0
+                else:
+                    raise ValueError("MSD became significantly (by more than 1e-10) negative during imaging correction. This is probably due to a bug; please report it.")
+
+            return out
 
         # Assemble a useful docstring
         try:
             fun_kwargstring = msdfun._kwargstring
         except AttributeError:
             params = inspect.signature(msdfun).parameters
             arglist = list(params)
```

### Comparing `bayesmsd-0.1.2/bayesmsd/fit.py` & `bayesmsd-0.1.3/bayesmsd/fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -644,15 +644,15 @@
             try:
                 initial_offset = -init_from['logL']
             except KeyError:
                 initial_offset = 0
 
         # Set up the minimization target
         # also allows us to convert initial_params to appropriate array
-        min_target = Fit.MinTarget(self, fix_values, initial_offset)
+        min_target = self.MinTarget(self, fix_values, initial_offset)
 
         p0 = min_target.params_dict2array(initial_params)
         bounds = [self.parameters[name].bounds for name in min_target.param_names]
         
         # Set up progress bar
         bar = tqdm(disable = not show_progress)
         def callback(x):
```

### Comparing `bayesmsd-0.1.2/bayesmsd/gp.py` & `bayesmsd-0.1.3/bayesmsd/gp.py`

 * *Files identical despite different names*

### Comparing `bayesmsd-0.1.2/bayesmsd/lib.py` & `bayesmsd-0.1.3/bayesmsd/lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 import rouse
 from noctiluca.analysis import MSD
 
 from . import deco
 from .fit import Fit
 from .parameters import Parameter, Linearize
 
+_MAX_LOG = 500
+
 class SplineFit(Fit):
     """
     Fit a spline MSD
 
     The MSD in this case is parametrized by the positions of a few spline
     points, between which we interpolate with cubic splines. The boundary
     conditions for the splines are set such that the fitted MSD extrapolates
@@ -141,15 +143,15 @@
         # x lives in the compactified interval [0, 1] (or [0, 2]), while y =
         # log(MSD) can be any real number.
         self.parameters = {}
         for i in range(self.n):
             self.parameters[f"x{i}"] = Parameter((0, self.x_max),
                                                  linearization=Linearize.Bounded(),
                                                  )
-            self.parameters[f"y{i}"] = Parameter((-np.inf, np.inf),
+            self.parameters[f"y{i}"] = Parameter((-np.inf, _MAX_LOG),
                                                  linearization=Linearize.Exponential(),
                                                  )
 
         self.constraints = [self.constraint_dx,
                             self.constraint_logmsd,
                             self.constraint_Cpositive,
                            ]
@@ -240,16 +242,17 @@
         alpha0 = csp(0, nu=1) / self.logT
         if self.ss_order == 0:
             alpha0 *= 4/np.pi
 
         @deco.MSDfun
         @deco.imaging(f=self.motion_blur_f, alpha0=alpha0)
         def msd(dt, csp=csp):
-            # dt == 0 is filtered out by MSDfun
-            return np.exp(csp(self.compactify(dt))) / self.d
+            with np.errstate(under='ignore'):
+                # dt == 0 is filtered out by MSDfun
+                return np.exp(csp(self.compactify(dt))) / self.d
 
         return self.d*[(msd, 0)]
             
     def initial_params(self):
         """
         Give suitable initial parameters for the spline
 
@@ -364,15 +367,15 @@
             the constraint score
 
         See also
         --------
         Fit
         """
         start_penalizing = 200
-        full_penalty = 500
+        full_penalty = _MAX_LOG
         
         csp = self._params2csp(params)
         x_full = self.compactify(np.arange(1, self.T))
         return (full_penalty - np.max(np.abs(csp(x_full))))/start_penalizing
 
 class NPXFit(Fit): # NPX = Noise + Powerlaw + X (i.e. spline)
     """
@@ -428,14 +431,21 @@
 
     Technically, the spline used to extend the MSD has ``n+1`` nodes, since of
     course there has to be one at the transition from powerlaw to spline.
 
     The vertical position of the first, and horizontal position of the last
     spline points are fixed. So the parameters for the spline are ``x0``
     through ``x(n-1)`` and ``y1`` through ``yn``.
+
+    The theoretical upper bound for the exponent of the powerlaw part is 2; at
+    this point the covariance matrix of the process stops being positive
+    definite. Due to numerical inaccuracies, this can start being an issue for
+    exponents close to (but smaller than) 2 as well. Thus, the upper bound for
+    these exponents is set to 1.99, i.e. if a fit returns 1.99 this is just the
+    upper bound of the parameter space and not a precise estimate.
     """
     def __init__(self, data, ss_order, n=0,
                  previous_NPXFit_and_result=None,
                  motion_blur_f=0,
                 ):
         super().__init__(data)
         self.motion_blur_f = motion_blur_f
@@ -464,26 +474,26 @@
         # 1.99
         self.x_max = min(self.x_last, self.compactify(sys.float_info.max/2))
 
         # Set up parameters
         # Populate with templates -> expand dimensions -> remove templates
         # The powerlaw stops being positive definite at α = 2, so stay away from that
         self.parameters = {
-            'log(σ²)' : Parameter((-np.inf, np.inf),
+            'log(σ²)' : Parameter((-np.inf, _MAX_LOG),
                                   linearization=Linearize.Exponential()),
-            'log(Γ)'  : Parameter((-np.inf, np.inf),
+            'log(Γ)'  : Parameter((-np.inf, _MAX_LOG),
                                   linearization=Linearize.Exponential()),
-            'α'       : Parameter((0, 2-1e-10), # stay away from upper bound
+            'α'       : Parameter((0.01, 1.99), # stay away from bounds, since covariance becomes singular, leading to numerical issues when getting close
                                   linearization=Linearize.Bounded()),
         }
 
         for i in range(self.n+1):
             self.parameters[f"x{i}"] = Parameter((0, self.x_max),
                                                  linearization=Linearize.Bounded())
-            self.parameters[f"y{i}"] = Parameter((-np.inf, np.inf),
+            self.parameters[f"y{i}"] = Parameter((-np.inf, _MAX_LOG),
                                                  linearization=Linearize.Exponential())
 
         # For the spline, y0 and xn are fixed
         del self.parameters["y0"]
         del self.parameters[f"x{self.n}"]
 
         # Expand dimensions and remove templates
@@ -662,15 +672,16 @@
                 t0 = np.exp(self.decompactify_log(params[f"x0 (dim {dim})"]))
 
                 def msd(dt, G=G, alpha=alpha, csp=csp, t0=t0):
                     out = G*(dt**alpha)
                     ind = dt > t0
                     if np.any(ind):
                         x = self.compactify(dt[ind])
-                        out[ind] = np.exp(csp(x))
+                        with np.errstate(under='ignore'):
+                            out[ind] = np.exp(csp(x))
                     return out
 
             # Apply MSD function decorators
             msd = deco.imaging(noise2=noise2, f=self.motion_blur_f, alpha0=alpha)(msd)
             msd = deco.MSDfun(msd)
 
             msdm.append((msd, 0))
@@ -812,15 +823,15 @@
 
         See also
         --------
         Fit
         """
         # constraints are not applied if n == 0, so we can safely assume n > 0
         start_penalizing = 200
-        full_penalty = 500
+        full_penalty = _MAX_LOG
 
         csps = self._params2csp(params)
         x_full = self.compactify(np.arange(1, self.T))
         xs = [x_full[x_full >= params[f"x0 (dim {dim})"]] for dim in range(self.d)]
 
         if all(len(x) == 0 for x in xs): # pragma: no cover
             return np.inf
@@ -856,15 +867,15 @@
         
         self.ss_order = 0
         
         self.parameters = {}
         for name in ['log(σ²)', 'log(Γ)', 'log(J)']:
             for dim in range(self.d):
                 dim_name = f"{name} (dim {dim})"
-                self.parameters[f"{name} (dim {dim})"] = Parameter((-np.inf, np.inf),
+                self.parameters[f"{name} (dim {dim})"] = Parameter((-np.inf, _MAX_LOG),
                                                                    linearization=Linearize.Exponential())
 
                 if name != 'log(σ²)' and dim > 0:
                     self.parameters[dim_name].fix_to = f"{name} (dim 0)"
 
         self.constraints = [] # Don't need to check Cpositive, will always be true for Rouse MSDs
```

### Comparing `bayesmsd-0.1.2/bayesmsd/parameters.py` & `bayesmsd-0.1.3/bayesmsd/parameters.py`

 * *Files identical despite different names*

### Comparing `bayesmsd-0.1.2/bayesmsd/profiler.py` & `bayesmsd-0.1.3/bayesmsd/profiler.py`

 * *Files identical despite different names*

### Comparing `bayesmsd-0.1.2/bayesmsd/src/gp.c` & `bayesmsd-0.1.3/bayesmsd/src/gp.c`

 * *Files 0% similar despite different names*

```diff
@@ -1336,24 +1336,24 @@
  * ctypedef float s
  * ctypedef double d             # <<<<<<<<<<<<<<
  * ctypedef float complex c
  * ctypedef double complex z
  */
 typedef double __pyx_t_5scipy_6linalg_13cython_lapack_d;
 
-/* "bayesmsd/src/gp.pyx":14
+/* "bayesmsd/src/gp.pyx":26
  * from ..src.gp_py import BadCovarianceError
  * 
  * ctypedef double FLOAT_t             # <<<<<<<<<<<<<<
  * ctypedef unsigned long SIZE_t
  * 
  */
 typedef double __pyx_t_8bayesmsd_3bin_2gp_FLOAT_t;
 
-/* "bayesmsd/src/gp.pyx":15
+/* "bayesmsd/src/gp.pyx":27
  * 
  * ctypedef double FLOAT_t
  * ctypedef unsigned long SIZE_t             # <<<<<<<<<<<<<<
  * 
  * @cython.boundscheck(False)
  */
 typedef unsigned long __pyx_t_8bayesmsd_3bin_2gp_SIZE_t;
@@ -2861,15 +2861,15 @@
 static PyObject *__pyx_tuple__27;
 static PyObject *__pyx_tuple__28;
 static PyObject *__pyx_tuple__29;
 static PyObject *__pyx_codeobj__23;
 static PyObject *__pyx_codeobj__30;
 /* Late includes */
 
-/* "bayesmsd/src/gp.pyx":19
+/* "bayesmsd/src/gp.pyx":31
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cdef void msd2C_ss0(FLOAT_t[::1]    msd,             # <<<<<<<<<<<<<<
  *                     SIZE_t[::1]     ti,
  *                     FLOAT_t[:, ::1] C,
  */
 
@@ -2880,170 +2880,182 @@
   __pyx_t_8bayesmsd_3bin_2gp_SIZE_t __pyx_v_maxti;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   __pyx_t_8bayesmsd_3bin_2gp_SIZE_t __pyx_t_3;
   size_t __pyx_t_4;
   int __pyx_t_5;
-  Py_ssize_t __pyx_t_6;
-  Py_ssize_t __pyx_t_7;
-  __pyx_t_8bayesmsd_3bin_2gp_SIZE_t __pyx_t_8;
-  size_t __pyx_t_9;
-  size_t __pyx_t_10;
+  size_t __pyx_t_6;
+  size_t __pyx_t_7;
+  Py_ssize_t __pyx_t_8;
+  Py_ssize_t __pyx_t_9;
+  __pyx_t_8bayesmsd_3bin_2gp_SIZE_t __pyx_t_10;
   Py_ssize_t __pyx_t_11;
   size_t __pyx_t_12;
   size_t __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("msd2C_ss0", 0);
 
-  /* "bayesmsd/src/gp.pyx":36
+  /* "bayesmsd/src/gp.pyx":48
  *         part and diagonal (i.e. FORTRAN lower triangular)
  *     """
  *     cdef SIZE_t m, n, T=msd.shape[0], maxti=0             # <<<<<<<<<<<<<<
  * 
  *     for m in range(ti.shape[0]):
  */
   __pyx_v_T = (__pyx_v_msd.shape[0]);
   __pyx_v_maxti = 0;
 
-  /* "bayesmsd/src/gp.pyx":38
+  /* "bayesmsd/src/gp.pyx":50
  *     cdef SIZE_t m, n, T=msd.shape[0], maxti=0
  * 
  *     for m in range(ti.shape[0]):             # <<<<<<<<<<<<<<
  *         if ti[m] > maxti:
  *             maxti = ti[m]
  */
   __pyx_t_1 = (__pyx_v_ti.shape[0]);
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_m = __pyx_t_3;
 
-    /* "bayesmsd/src/gp.pyx":39
+    /* "bayesmsd/src/gp.pyx":51
  * 
  *     for m in range(ti.shape[0]):
  *         if ti[m] > maxti:             # <<<<<<<<<<<<<<
  *             maxti = ti[m]
  * 
  */
     __pyx_t_4 = __pyx_v_m;
     __pyx_t_5 = (((*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_4)) ))) > __pyx_v_maxti) != 0);
     if (__pyx_t_5) {
 
-      /* "bayesmsd/src/gp.pyx":40
+      /* "bayesmsd/src/gp.pyx":52
  *     for m in range(ti.shape[0]):
  *         if ti[m] > maxti:
  *             maxti = ti[m]             # <<<<<<<<<<<<<<
  * 
  *     assert C.shape[0] >= ti.shape[0]
  */
       __pyx_t_4 = __pyx_v_m;
       __pyx_v_maxti = (*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_4)) )));
 
-      /* "bayesmsd/src/gp.pyx":39
+      /* "bayesmsd/src/gp.pyx":51
  * 
  *     for m in range(ti.shape[0]):
  *         if ti[m] > maxti:             # <<<<<<<<<<<<<<
  *             maxti = ti[m]
  * 
  */
     }
   }
 
-  /* "bayesmsd/src/gp.pyx":42
+  /* "bayesmsd/src/gp.pyx":54
  *             maxti = ti[m]
  * 
  *     assert C.shape[0] >= ti.shape[0]             # <<<<<<<<<<<<<<
  *     assert C.shape[1] >= ti.shape[0]
  *     assert msd.shape[0] > maxti-1
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!(((__pyx_v_C.shape[0]) >= (__pyx_v_ti.shape[0])) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 42, __pyx_L1_error)
+      __PYX_ERR(0, 54, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "bayesmsd/src/gp.pyx":43
+  /* "bayesmsd/src/gp.pyx":55
  * 
  *     assert C.shape[0] >= ti.shape[0]
  *     assert C.shape[1] >= ti.shape[0]             # <<<<<<<<<<<<<<
  *     assert msd.shape[0] > maxti-1
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!(((__pyx_v_C.shape[1]) >= (__pyx_v_ti.shape[0])) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 43, __pyx_L1_error)
+      __PYX_ERR(0, 55, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "bayesmsd/src/gp.pyx":44
+  /* "bayesmsd/src/gp.pyx":56
  *     assert C.shape[0] >= ti.shape[0]
  *     assert C.shape[1] >= ti.shape[0]
  *     assert msd.shape[0] > maxti-1             # <<<<<<<<<<<<<<
  * 
  *     for m in range(ti.shape[0]):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!(((__pyx_v_msd.shape[0]) > (__pyx_v_maxti - 1)) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 44, __pyx_L1_error)
+      __PYX_ERR(0, 56, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "bayesmsd/src/gp.pyx":46
+  /* "bayesmsd/src/gp.pyx":58
  *     assert msd.shape[0] > maxti-1
  * 
  *     for m in range(ti.shape[0]):             # <<<<<<<<<<<<<<
+ *         C[m, m] = 0.5*msd[T-1]
  *         for n in range(m, ti.shape[0]):
- *             C[m, n] = 0.5*( msd[T-1] - msd[abs(ti[m] - ti[n])] )
  */
   __pyx_t_1 = (__pyx_v_ti.shape[0]);
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_m = __pyx_t_3;
 
-    /* "bayesmsd/src/gp.pyx":47
+    /* "bayesmsd/src/gp.pyx":59
  * 
  *     for m in range(ti.shape[0]):
+ *         C[m, m] = 0.5*msd[T-1]             # <<<<<<<<<<<<<<
+ *         for n in range(m, ti.shape[0]):
+ *             C[m, n] = 0.5*( msd[T-1] - msd[abs(ti[m] - ti[n])] )
+ */
+    __pyx_t_4 = (__pyx_v_T - 1);
+    __pyx_t_6 = __pyx_v_m;
+    __pyx_t_7 = __pyx_v_m;
+    *((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=1 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ (__pyx_v_C.data + __pyx_t_6 * __pyx_v_C.strides[0]) )) + __pyx_t_7)) )) = (0.5 * (*((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) __pyx_v_msd.data) + __pyx_t_4)) ))));
+
+    /* "bayesmsd/src/gp.pyx":60
+ *     for m in range(ti.shape[0]):
+ *         C[m, m] = 0.5*msd[T-1]
  *         for n in range(m, ti.shape[0]):             # <<<<<<<<<<<<<<
  *             C[m, n] = 0.5*( msd[T-1] - msd[abs(ti[m] - ti[n])] )
  * 
  */
-    __pyx_t_6 = (__pyx_v_ti.shape[0]);
-    __pyx_t_7 = __pyx_t_6;
-    for (__pyx_t_8 = __pyx_v_m; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
-      __pyx_v_n = __pyx_t_8;
+    __pyx_t_8 = (__pyx_v_ti.shape[0]);
+    __pyx_t_9 = __pyx_t_8;
+    for (__pyx_t_10 = __pyx_v_m; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
+      __pyx_v_n = __pyx_t_10;
 
-      /* "bayesmsd/src/gp.pyx":48
- *     for m in range(ti.shape[0]):
+      /* "bayesmsd/src/gp.pyx":61
+ *         C[m, m] = 0.5*msd[T-1]
  *         for n in range(m, ti.shape[0]):
  *             C[m, n] = 0.5*( msd[T-1] - msd[abs(ti[m] - ti[n])] )             # <<<<<<<<<<<<<<
  * 
  * @cython.boundscheck(False)
  */
       __pyx_t_4 = (__pyx_v_T - 1);
-      __pyx_t_9 = __pyx_v_m;
-      __pyx_t_10 = __pyx_v_n;
-      __pyx_t_11 = abs(((*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_9)) ))) - (*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_10)) )))));
+      __pyx_t_7 = __pyx_v_m;
+      __pyx_t_6 = __pyx_v_n;
+      __pyx_t_11 = abs(((*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_7)) ))) - (*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_6)) )))));
       __pyx_t_12 = __pyx_v_m;
       __pyx_t_13 = __pyx_v_n;
       *((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=1 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ (__pyx_v_C.data + __pyx_t_12 * __pyx_v_C.strides[0]) )) + __pyx_t_13)) )) = (0.5 * ((*((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) __pyx_v_msd.data) + __pyx_t_4)) ))) - (*((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) __pyx_v_msd.data) + __pyx_t_11)) )))));
     }
   }
 
-  /* "bayesmsd/src/gp.pyx":19
+  /* "bayesmsd/src/gp.pyx":31
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cdef void msd2C_ss0(FLOAT_t[::1]    msd,             # <<<<<<<<<<<<<<
  *                     SIZE_t[::1]     ti,
  *                     FLOAT_t[:, ::1] C,
  */
 
@@ -3051,15 +3063,15 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("bayesmsd.bin.gp.msd2C_ss0", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "bayesmsd/src/gp.pyx":52
+/* "bayesmsd/src/gp.pyx":65
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cdef void msd2C_ss1(FLOAT_t[::1]    msd,             # <<<<<<<<<<<<<<
  *                     SIZE_t[::1]     ti,
  *                     FLOAT_t[:, ::1] C,
  */
 
@@ -3069,217 +3081,231 @@
   __pyx_t_8bayesmsd_3bin_2gp_SIZE_t __pyx_v_maxti;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   __pyx_t_8bayesmsd_3bin_2gp_SIZE_t __pyx_t_3;
   size_t __pyx_t_4;
   int __pyx_t_5;
-  Py_ssize_t __pyx_t_6;
+  size_t __pyx_t_6;
   Py_ssize_t __pyx_t_7;
-  __pyx_t_8bayesmsd_3bin_2gp_SIZE_t __pyx_t_8;
+  size_t __pyx_t_8;
   size_t __pyx_t_9;
   Py_ssize_t __pyx_t_10;
-  size_t __pyx_t_11;
-  size_t __pyx_t_12;
+  Py_ssize_t __pyx_t_11;
+  __pyx_t_8bayesmsd_3bin_2gp_SIZE_t __pyx_t_12;
   Py_ssize_t __pyx_t_13;
   size_t __pyx_t_14;
   size_t __pyx_t_15;
   Py_ssize_t __pyx_t_16;
   size_t __pyx_t_17;
   size_t __pyx_t_18;
   Py_ssize_t __pyx_t_19;
   size_t __pyx_t_20;
   size_t __pyx_t_21;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("msd2C_ss1", 0);
 
-  /* "bayesmsd/src/gp.pyx":68
+  /* "bayesmsd/src/gp.pyx":81
  *         part and diagonal (i.e. FORTRAN lower triangular)
  *     """
  *     cdef SIZE_t m, n, maxti=0             # <<<<<<<<<<<<<<
  * 
  *     for m in range(ti.shape[0]):
  */
   __pyx_v_maxti = 0;
 
-  /* "bayesmsd/src/gp.pyx":70
+  /* "bayesmsd/src/gp.pyx":83
  *     cdef SIZE_t m, n, maxti=0
  * 
  *     for m in range(ti.shape[0]):             # <<<<<<<<<<<<<<
  *         if ti[m] > maxti:
  *             maxti = ti[m]
  */
   __pyx_t_1 = (__pyx_v_ti.shape[0]);
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_m = __pyx_t_3;
 
-    /* "bayesmsd/src/gp.pyx":71
+    /* "bayesmsd/src/gp.pyx":84
  * 
  *     for m in range(ti.shape[0]):
  *         if ti[m] > maxti:             # <<<<<<<<<<<<<<
  *             maxti = ti[m]
  * 
  */
     __pyx_t_4 = __pyx_v_m;
     __pyx_t_5 = (((*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_4)) ))) > __pyx_v_maxti) != 0);
     if (__pyx_t_5) {
 
-      /* "bayesmsd/src/gp.pyx":72
+      /* "bayesmsd/src/gp.pyx":85
  *     for m in range(ti.shape[0]):
  *         if ti[m] > maxti:
  *             maxti = ti[m]             # <<<<<<<<<<<<<<
  * 
  *     assert C.shape[0] >= ti.shape[0]-1
  */
       __pyx_t_4 = __pyx_v_m;
       __pyx_v_maxti = (*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_4)) )));
 
-      /* "bayesmsd/src/gp.pyx":71
+      /* "bayesmsd/src/gp.pyx":84
  * 
  *     for m in range(ti.shape[0]):
  *         if ti[m] > maxti:             # <<<<<<<<<<<<<<
  *             maxti = ti[m]
  * 
  */
     }
   }
 
-  /* "bayesmsd/src/gp.pyx":74
+  /* "bayesmsd/src/gp.pyx":87
  *             maxti = ti[m]
  * 
  *     assert C.shape[0] >= ti.shape[0]-1             # <<<<<<<<<<<<<<
  *     assert C.shape[1] >= ti.shape[0]-1
  *     assert msd.shape[0] > maxti
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!(((__pyx_v_C.shape[0]) >= ((__pyx_v_ti.shape[0]) - 1)) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 74, __pyx_L1_error)
+      __PYX_ERR(0, 87, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "bayesmsd/src/gp.pyx":75
+  /* "bayesmsd/src/gp.pyx":88
  * 
  *     assert C.shape[0] >= ti.shape[0]-1
  *     assert C.shape[1] >= ti.shape[0]-1             # <<<<<<<<<<<<<<
  *     assert msd.shape[0] > maxti
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!(((__pyx_v_C.shape[1]) >= ((__pyx_v_ti.shape[0]) - 1)) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 75, __pyx_L1_error)
+      __PYX_ERR(0, 88, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "bayesmsd/src/gp.pyx":76
+  /* "bayesmsd/src/gp.pyx":89
  *     assert C.shape[0] >= ti.shape[0]-1
  *     assert C.shape[1] >= ti.shape[0]-1
  *     assert msd.shape[0] > maxti             # <<<<<<<<<<<<<<
  * 
- *     for m in range(ti.shape[0]-1):
+ *     # ti should be ordered
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!(((__pyx_v_msd.shape[0]) > __pyx_v_maxti) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 76, __pyx_L1_error)
+      __PYX_ERR(0, 89, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "bayesmsd/src/gp.pyx":78
- *     assert msd.shape[0] > maxti
- * 
+  /* "bayesmsd/src/gp.pyx":94
+ *     # populate only upper triangle
+ *     # benchmarking showed no speedup for precalculating msd[ti-tj]
  *     for m in range(ti.shape[0]-1):             # <<<<<<<<<<<<<<
- *         for n in range(m, ti.shape[0]-1):
- *             # Note: if ti are unevenly spaced (i.e. missing data, this is the
+ *         C[m, m] = msd[abs(ti[m+1]-ti[m])]
+ *         for n in range(m+1, ti.shape[0]-1):
  */
   __pyx_t_1 = ((__pyx_v_ti.shape[0]) - 1);
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_m = __pyx_t_3;
 
-    /* "bayesmsd/src/gp.pyx":79
- * 
+    /* "bayesmsd/src/gp.pyx":95
+ *     # benchmarking showed no speedup for precalculating msd[ti-tj]
+ *     for m in range(ti.shape[0]-1):
+ *         C[m, m] = msd[abs(ti[m+1]-ti[m])]             # <<<<<<<<<<<<<<
+ *         for n in range(m+1, ti.shape[0]-1):
+ *             C[m, n] = 0.5*(  msd[abs(ti[n+1]-ti[m])]
+ */
+    __pyx_t_4 = (__pyx_v_m + 1);
+    __pyx_t_6 = __pyx_v_m;
+    __pyx_t_7 = abs(((*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_4)) ))) - (*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_6)) )))));
+    __pyx_t_8 = __pyx_v_m;
+    __pyx_t_9 = __pyx_v_m;
+    *((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=1 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ (__pyx_v_C.data + __pyx_t_8 * __pyx_v_C.strides[0]) )) + __pyx_t_9)) )) = (*((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) __pyx_v_msd.data) + __pyx_t_7)) )));
+
+    /* "bayesmsd/src/gp.pyx":96
  *     for m in range(ti.shape[0]-1):
- *         for n in range(m, ti.shape[0]-1):             # <<<<<<<<<<<<<<
- *             # Note: if ti are unevenly spaced (i.e. missing data, this is the
- *             # usual case), then C is not strictly Toeplitz
- */
-    __pyx_t_6 = ((__pyx_v_ti.shape[0]) - 1);
-    __pyx_t_7 = __pyx_t_6;
-    for (__pyx_t_8 = __pyx_v_m; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
-      __pyx_v_n = __pyx_t_8;
-
-      /* "bayesmsd/src/gp.pyx":82
- *             # Note: if ti are unevenly spaced (i.e. missing data, this is the
- *             # usual case), then C is not strictly Toeplitz
- *             C[m, n] = 0.5*(  msd[abs(ti[m+1]-ti[n])]             # <<<<<<<<<<<<<<
- *                            + msd[abs(ti[m]  -ti[n+1])]
- *                            - msd[abs(ti[m+1]-ti[n+1])]
+ *         C[m, m] = msd[abs(ti[m+1]-ti[m])]
+ *         for n in range(m+1, ti.shape[0]-1):             # <<<<<<<<<<<<<<
+ *             C[m, n] = 0.5*(  msd[abs(ti[n+1]-ti[m])]
+ *                            + msd[abs(ti[n]  -ti[m+1])]
+ */
+    __pyx_t_10 = ((__pyx_v_ti.shape[0]) - 1);
+    __pyx_t_11 = __pyx_t_10;
+    for (__pyx_t_12 = (__pyx_v_m + 1); __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
+      __pyx_v_n = __pyx_t_12;
+
+      /* "bayesmsd/src/gp.pyx":97
+ *         C[m, m] = msd[abs(ti[m+1]-ti[m])]
+ *         for n in range(m+1, ti.shape[0]-1):
+ *             C[m, n] = 0.5*(  msd[abs(ti[n+1]-ti[m])]             # <<<<<<<<<<<<<<
+ *                            + msd[abs(ti[n]  -ti[m+1])]
+ *                            - msd[abs(ti[n+1]-ti[m+1])]
  */
-      __pyx_t_4 = (__pyx_v_m + 1);
-      __pyx_t_9 = __pyx_v_n;
-      __pyx_t_10 = abs(((*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_4)) ))) - (*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_9)) )))));
+      __pyx_t_6 = (__pyx_v_n + 1);
+      __pyx_t_4 = __pyx_v_m;
+      __pyx_t_7 = abs(((*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_6)) ))) - (*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_4)) )))));
 
-      /* "bayesmsd/src/gp.pyx":83
- *             # usual case), then C is not strictly Toeplitz
- *             C[m, n] = 0.5*(  msd[abs(ti[m+1]-ti[n])]
- *                            + msd[abs(ti[m]  -ti[n+1])]             # <<<<<<<<<<<<<<
- *                            - msd[abs(ti[m+1]-ti[n+1])]
- *                            - msd[abs(ti[m]  -ti[n])]
- */
-      __pyx_t_11 = __pyx_v_m;
-      __pyx_t_12 = (__pyx_v_n + 1);
-      __pyx_t_13 = abs(((*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_11)) ))) - (*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_12)) )))));
+      /* "bayesmsd/src/gp.pyx":98
+ *         for n in range(m+1, ti.shape[0]-1):
+ *             C[m, n] = 0.5*(  msd[abs(ti[n+1]-ti[m])]
+ *                            + msd[abs(ti[n]  -ti[m+1])]             # <<<<<<<<<<<<<<
+ *                            - msd[abs(ti[n+1]-ti[m+1])]
+ *                            - msd[abs(ti[n]  -ti[m])]
+ */
+      __pyx_t_9 = __pyx_v_n;
+      __pyx_t_8 = (__pyx_v_m + 1);
+      __pyx_t_13 = abs(((*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_9)) ))) - (*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_8)) )))));
 
-      /* "bayesmsd/src/gp.pyx":84
- *             C[m, n] = 0.5*(  msd[abs(ti[m+1]-ti[n])]
- *                            + msd[abs(ti[m]  -ti[n+1])]
- *                            - msd[abs(ti[m+1]-ti[n+1])]             # <<<<<<<<<<<<<<
- *                            - msd[abs(ti[m]  -ti[n])]
+      /* "bayesmsd/src/gp.pyx":99
+ *             C[m, n] = 0.5*(  msd[abs(ti[n+1]-ti[m])]
+ *                            + msd[abs(ti[n]  -ti[m+1])]
+ *                            - msd[abs(ti[n+1]-ti[m+1])]             # <<<<<<<<<<<<<<
+ *                            - msd[abs(ti[n]  -ti[m])]
  *                           )
  */
-      __pyx_t_14 = (__pyx_v_m + 1);
-      __pyx_t_15 = (__pyx_v_n + 1);
+      __pyx_t_14 = (__pyx_v_n + 1);
+      __pyx_t_15 = (__pyx_v_m + 1);
       __pyx_t_16 = abs(((*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_14)) ))) - (*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_15)) )))));
 
-      /* "bayesmsd/src/gp.pyx":85
- *                            + msd[abs(ti[m]  -ti[n+1])]
- *                            - msd[abs(ti[m+1]-ti[n+1])]
- *                            - msd[abs(ti[m]  -ti[n])]             # <<<<<<<<<<<<<<
+      /* "bayesmsd/src/gp.pyx":100
+ *                            + msd[abs(ti[n]  -ti[m+1])]
+ *                            - msd[abs(ti[n+1]-ti[m+1])]
+ *                            - msd[abs(ti[n]  -ti[m])]             # <<<<<<<<<<<<<<
  *                           )
  * 
  */
-      __pyx_t_17 = __pyx_v_m;
-      __pyx_t_18 = __pyx_v_n;
+      __pyx_t_17 = __pyx_v_n;
+      __pyx_t_18 = __pyx_v_m;
       __pyx_t_19 = abs(((*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_17)) ))) - (*((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_SIZE_t *) __pyx_v_ti.data) + __pyx_t_18)) )))));
 
-      /* "bayesmsd/src/gp.pyx":82
- *             # Note: if ti are unevenly spaced (i.e. missing data, this is the
- *             # usual case), then C is not strictly Toeplitz
- *             C[m, n] = 0.5*(  msd[abs(ti[m+1]-ti[n])]             # <<<<<<<<<<<<<<
- *                            + msd[abs(ti[m]  -ti[n+1])]
- *                            - msd[abs(ti[m+1]-ti[n+1])]
+      /* "bayesmsd/src/gp.pyx":97
+ *         C[m, m] = msd[abs(ti[m+1]-ti[m])]
+ *         for n in range(m+1, ti.shape[0]-1):
+ *             C[m, n] = 0.5*(  msd[abs(ti[n+1]-ti[m])]             # <<<<<<<<<<<<<<
+ *                            + msd[abs(ti[n]  -ti[m+1])]
+ *                            - msd[abs(ti[n+1]-ti[m+1])]
  */
       __pyx_t_20 = __pyx_v_m;
       __pyx_t_21 = __pyx_v_n;
-      *((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=1 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ (__pyx_v_C.data + __pyx_t_20 * __pyx_v_C.strides[0]) )) + __pyx_t_21)) )) = (0.5 * ((((*((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) __pyx_v_msd.data) + __pyx_t_10)) ))) + (*((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) __pyx_v_msd.data) + __pyx_t_13)) )))) - (*((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) __pyx_v_msd.data) + __pyx_t_16)) )))) - (*((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) __pyx_v_msd.data) + __pyx_t_19)) )))));
+      *((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=1 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ (__pyx_v_C.data + __pyx_t_20 * __pyx_v_C.strides[0]) )) + __pyx_t_21)) )) = (0.5 * ((((*((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) __pyx_v_msd.data) + __pyx_t_7)) ))) + (*((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) __pyx_v_msd.data) + __pyx_t_13)) )))) - (*((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) __pyx_v_msd.data) + __pyx_t_16)) )))) - (*((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) __pyx_v_msd.data) + __pyx_t_19)) )))));
     }
   }
 
-  /* "bayesmsd/src/gp.pyx":52
+  /* "bayesmsd/src/gp.pyx":65
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cdef void msd2C_ss1(FLOAT_t[::1]    msd,             # <<<<<<<<<<<<<<
  *                     SIZE_t[::1]     ti,
  *                     FLOAT_t[:, ::1] C,
  */
 
@@ -3287,15 +3313,15 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("bayesmsd.bin.gp.msd2C_ss1", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "bayesmsd/src/gp.pyx":97
+/* "bayesmsd/src/gp.pyx":112
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cdef FLOAT_t _core_logL(FLOAT_t[:, ::1] C, # will be overwritten             # <<<<<<<<<<<<<<
  *                         FLOAT_t[::1]    x,
  *                         FLOAT_t[::1]    y, # copy of x
  */
 
@@ -3321,110 +3347,110 @@
   PyObject *__pyx_t_10 = NULL;
   Py_ssize_t __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_core_logL", 0);
 
-  /* "bayesmsd/src/gp.pyx":107
+  /* "bayesmsd/src/gp.pyx":122
  *     #   necessary; c.f. Fit.constraint_Cpositive
  *     cdef FLOAT_t logdet, xCx
  *     cdef int i, N=C.shape[0], info, inc=1             # <<<<<<<<<<<<<<
  *     cdef double one=1.
  * 
  */
   __pyx_v_N = (__pyx_v_C.shape[0]);
   __pyx_v_inc = 1;
 
-  /* "bayesmsd/src/gp.pyx":108
+  /* "bayesmsd/src/gp.pyx":123
  *     cdef FLOAT_t logdet, xCx
  *     cdef int i, N=C.shape[0], info, inc=1
  *     cdef double one=1.             # <<<<<<<<<<<<<<
  * 
  *     # Cholesky factorization
  */
   __pyx_v_one = 1.;
 
-  /* "bayesmsd/src/gp.pyx":111
+  /* "bayesmsd/src/gp.pyx":126
  * 
  *     # Cholesky factorization
  *     dpotrf('l', &N, &C[0, 0], &N, &info)             # <<<<<<<<<<<<<<
  * 
  *     # logdet from cholesky
  */
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_f_5scipy_6linalg_13cython_lapack_dpotrf(((char *)"l"), (&__pyx_v_N), (&(*((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=1 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ (__pyx_v_C.data + __pyx_t_1 * __pyx_v_C.strides[0]) )) + __pyx_t_2)) )))), (&__pyx_v_N), (&__pyx_v_info));
 
-  /* "bayesmsd/src/gp.pyx":114
+  /* "bayesmsd/src/gp.pyx":129
  * 
  *     # logdet from cholesky
  *     if info == 0:             # <<<<<<<<<<<<<<
  *         logdet = 0.
  *         for i in range(N):
  */
   __pyx_t_3 = ((__pyx_v_info == 0) != 0);
   if (likely(__pyx_t_3)) {
 
-    /* "bayesmsd/src/gp.pyx":115
+    /* "bayesmsd/src/gp.pyx":130
  *     # logdet from cholesky
  *     if info == 0:
  *         logdet = 0.             # <<<<<<<<<<<<<<
  *         for i in range(N):
  *             logdet += log(fabs(C[i, i]))
  */
     __pyx_v_logdet = 0.;
 
-    /* "bayesmsd/src/gp.pyx":116
+    /* "bayesmsd/src/gp.pyx":131
  *     if info == 0:
  *         logdet = 0.
  *         for i in range(N):             # <<<<<<<<<<<<<<
  *             logdet += log(fabs(C[i, i]))
  *     else:
  */
     __pyx_t_4 = __pyx_v_N;
     __pyx_t_5 = __pyx_t_4;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       __pyx_v_i = __pyx_t_6;
 
-      /* "bayesmsd/src/gp.pyx":117
+      /* "bayesmsd/src/gp.pyx":132
  *         logdet = 0.
  *         for i in range(N):
  *             logdet += log(fabs(C[i, i]))             # <<<<<<<<<<<<<<
  *     else:
  *         raise BadCovarianceError(f"Cholesky factorization failed, dpotrf returned {info}")
  */
       __pyx_t_2 = __pyx_v_i;
       __pyx_t_1 = __pyx_v_i;
       __pyx_v_logdet = (__pyx_v_logdet + log(fabs((*((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=1 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ (__pyx_v_C.data + __pyx_t_2 * __pyx_v_C.strides[0]) )) + __pyx_t_1)) ))))));
     }
 
-    /* "bayesmsd/src/gp.pyx":114
+    /* "bayesmsd/src/gp.pyx":129
  * 
  *     # logdet from cholesky
  *     if info == 0:             # <<<<<<<<<<<<<<
  *         logdet = 0.
  *         for i in range(N):
  */
     goto __pyx_L3;
   }
 
-  /* "bayesmsd/src/gp.pyx":119
+  /* "bayesmsd/src/gp.pyx":134
  *             logdet += log(fabs(C[i, i]))
  *     else:
  *         raise BadCovarianceError(f"Cholesky factorization failed, dpotrf returned {info}")             # <<<<<<<<<<<<<<
  * 
  *     logdet *= 2
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_BadCovarianceError); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 119, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_BadCovarianceError); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_9 = __Pyx_PyUnicode_From_int(__pyx_v_info, 0, ' ', 'd'); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 119, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyUnicode_From_int(__pyx_v_info, 0, ' ', 'd'); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_10 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Cholesky_factorization_failed_dp, __pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 119, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Cholesky_factorization_failed_dp, __pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_t_9 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
       if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
@@ -3432,131 +3458,131 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_8, function);
       }
     }
     __pyx_t_7 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_9, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_10);
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 119, __pyx_L1_error)
+    if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_Raise(__pyx_t_7, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __PYX_ERR(0, 119, __pyx_L1_error)
+    __PYX_ERR(0, 134, __pyx_L1_error)
   }
   __pyx_L3:;
 
-  /* "bayesmsd/src/gp.pyx":121
+  /* "bayesmsd/src/gp.pyx":136
  *         raise BadCovarianceError(f"Cholesky factorization failed, dpotrf returned {info}")
  * 
  *     logdet *= 2             # <<<<<<<<<<<<<<
  * 
  *     # Compute xCx = x @ inv(C) @ x = x @ y with C @ y = x
  */
   __pyx_v_logdet = (__pyx_v_logdet * 2.0);
 
-  /* "bayesmsd/src/gp.pyx":128
+  /* "bayesmsd/src/gp.pyx":143
  *     dtrsm('l', 'l', 'n', 'n',       # L @ b = x
  *           &N, &inc, &one,
  *           &C[0, 0], &N,             # <<<<<<<<<<<<<<
  *           &y[0], &N,
  *          )
  */
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
 
-  /* "bayesmsd/src/gp.pyx":129
+  /* "bayesmsd/src/gp.pyx":144
  *           &N, &inc, &one,
  *           &C[0, 0], &N,
  *           &y[0], &N,             # <<<<<<<<<<<<<<
  *          )
  *     dtrsm('l', 'l', 't', 'n',       # L.T @ y = b
  */
   __pyx_t_11 = 0;
 
-  /* "bayesmsd/src/gp.pyx":126
+  /* "bayesmsd/src/gp.pyx":141
  *     # solve with cholesky: L @ L.T @ y = x
  *     # dcopy(&x[0], &inc, &y[0], &inc) # copy x --> y # is now required as parameter
  *     dtrsm('l', 'l', 'n', 'n',       # L @ b = x             # <<<<<<<<<<<<<<
  *           &N, &inc, &one,
  *           &C[0, 0], &N,
  */
   __pyx_f_5scipy_6linalg_11cython_blas_dtrsm(((char *)"l"), ((char *)"l"), ((char *)"n"), ((char *)"n"), (&__pyx_v_N), (&__pyx_v_inc), (&__pyx_v_one), (&(*((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=1 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ (__pyx_v_C.data + __pyx_t_1 * __pyx_v_C.strides[0]) )) + __pyx_t_2)) )))), (&__pyx_v_N), (&(*((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) __pyx_v_y.data) + __pyx_t_11)) )))), (&__pyx_v_N));
 
-  /* "bayesmsd/src/gp.pyx":133
+  /* "bayesmsd/src/gp.pyx":148
  *     dtrsm('l', 'l', 't', 'n',       # L.T @ y = b
  *           &N, &inc, &one,
  *           &C[0, 0], &N,             # <<<<<<<<<<<<<<
  *           &y[0], &N,
  *          )
  */
   __pyx_t_11 = 0;
   __pyx_t_2 = 0;
 
-  /* "bayesmsd/src/gp.pyx":134
+  /* "bayesmsd/src/gp.pyx":149
  *           &N, &inc, &one,
  *           &C[0, 0], &N,
  *           &y[0], &N,             # <<<<<<<<<<<<<<
  *          )
  *     xCx = <FLOAT_t> ddot(&N, &x[0], &inc, &y[0], &inc)
  */
   __pyx_t_1 = 0;
 
-  /* "bayesmsd/src/gp.pyx":131
+  /* "bayesmsd/src/gp.pyx":146
  *           &y[0], &N,
  *          )
  *     dtrsm('l', 'l', 't', 'n',       # L.T @ y = b             # <<<<<<<<<<<<<<
  *           &N, &inc, &one,
  *           &C[0, 0], &N,
  */
   __pyx_f_5scipy_6linalg_11cython_blas_dtrsm(((char *)"l"), ((char *)"l"), ((char *)"t"), ((char *)"n"), (&__pyx_v_N), (&__pyx_v_inc), (&__pyx_v_one), (&(*((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=1 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ (__pyx_v_C.data + __pyx_t_11 * __pyx_v_C.strides[0]) )) + __pyx_t_2)) )))), (&__pyx_v_N), (&(*((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) __pyx_v_y.data) + __pyx_t_1)) )))), (&__pyx_v_N));
 
-  /* "bayesmsd/src/gp.pyx":136
+  /* "bayesmsd/src/gp.pyx":151
  *           &y[0], &N,
  *          )
  *     xCx = <FLOAT_t> ddot(&N, &x[0], &inc, &y[0], &inc)             # <<<<<<<<<<<<<<
  * 
  *     return -0.5*( xCx + logdet + N*LOG_2PI )
  */
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_v_xCx = ((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t)__pyx_f_5scipy_6linalg_11cython_blas_ddot((&__pyx_v_N), (&(*((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) __pyx_v_x.data) + __pyx_t_1)) )))), (&__pyx_v_inc), (&(*((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) ( /* dim=0 */ ((char *) (((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t *) __pyx_v_y.data) + __pyx_t_2)) )))), (&__pyx_v_inc)));
 
-  /* "bayesmsd/src/gp.pyx":138
+  /* "bayesmsd/src/gp.pyx":153
  *     xCx = <FLOAT_t> ddot(&N, &x[0], &inc, &y[0], &inc)
  * 
  *     return -0.5*( xCx + logdet + N*LOG_2PI )             # <<<<<<<<<<<<<<
  * 
  * def logL(trace, ss_order, msd, mean=0):
  */
   __pyx_r = (-0.5 * ((__pyx_v_xCx + __pyx_v_logdet) + (__pyx_v_N * __pyx_v_8bayesmsd_3bin_2gp_LOG_2PI)));
   goto __pyx_L0;
 
-  /* "bayesmsd/src/gp.pyx":97
+  /* "bayesmsd/src/gp.pyx":112
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cdef FLOAT_t _core_logL(FLOAT_t[:, ::1] C, # will be overwritten             # <<<<<<<<<<<<<<
  *                         FLOAT_t[::1]    x,
  *                         FLOAT_t[::1]    y, # copy of x
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_WriteUnraisable("bayesmsd.bin.gp._core_logL", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
-  __pyx_r = 0;
+  __Pyx_AddTraceback("bayesmsd.bin.gp._core_logL", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 1e300;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bayesmsd/src/gp.pyx":140
+/* "bayesmsd/src/gp.pyx":155
  *     return -0.5*( xCx + logdet + N*LOG_2PI )
  * 
  * def logL(trace, ss_order, msd, mean=0):             # <<<<<<<<<<<<<<
  *     """
  *     Gaussian process likelihood for a given trace
  */
 
@@ -3599,31 +3625,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_trace)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ss_order)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("logL", 0, 3, 4, 1); __PYX_ERR(0, 140, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("logL", 0, 3, 4, 1); __PYX_ERR(0, 155, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_msd)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("logL", 0, 3, 4, 2); __PYX_ERR(0, 140, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("logL", 0, 3, 4, 2); __PYX_ERR(0, 155, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mean);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "logL") < 0)) __PYX_ERR(0, 140, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "logL") < 0)) __PYX_ERR(0, 155, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -3635,15 +3661,15 @@
     __pyx_v_trace = values[0];
     __pyx_v_ss_order = values[1];
     __pyx_v_msd = values[2];
     __pyx_v_mean = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("logL", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 140, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("logL", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 155, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("bayesmsd.bin.gp.logL", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8bayesmsd_3bin_2gp_logL(__pyx_self, __pyx_v_trace, __pyx_v_ss_order, __pyx_v_msd, __pyx_v_mean);
 
@@ -3666,52 +3692,53 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   Py_ssize_t __pyx_t_7;
   int __pyx_t_8;
   __Pyx_memviewslice __pyx_t_9 = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_t_10 = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_t_11 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __pyx_t_8bayesmsd_3bin_2gp_FLOAT_t __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("logL", 0);
 
-  /* "bayesmsd/src/gp.pyx":172
+  /* "bayesmsd/src/gp.pyx":187
  *     cdef FLOAT_t[::1]    X
  * 
  *     ti = np.nonzero(~np.isnan(trace))[0].astype(np.uint)             # <<<<<<<<<<<<<<
  *     N = len(ti)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_nonzero); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_nonzero); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_isnan); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_isnan); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_5, __pyx_v_trace) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_trace);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 172, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyNumber_Invert(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_6 = PyNumber_Invert(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -3719,26 +3746,26 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_astype); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_astype); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_uint); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_uint); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -3746,315 +3773,316 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_ti = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "bayesmsd/src/gp.pyx":173
+  /* "bayesmsd/src/gp.pyx":188
  * 
  *     ti = np.nonzero(~np.isnan(trace))[0].astype(np.uint)
  *     N = len(ti)             # <<<<<<<<<<<<<<
  * 
  *     if ss_order == 0:
  */
-  __pyx_t_7 = PyObject_Length(__pyx_v_ti); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 173, __pyx_L1_error)
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_t_7 = PyObject_Length(__pyx_v_ti); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_N = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "bayesmsd/src/gp.pyx":175
+  /* "bayesmsd/src/gp.pyx":190
  *     N = len(ti)
  * 
  *     if ss_order == 0:             # <<<<<<<<<<<<<<
  *         X = trace[ti] - mean
  *         C = np.empty((N, N), dtype=float)
  */
-  __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_ss_order, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_ss_order, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_8) {
 
-    /* "bayesmsd/src/gp.pyx":176
+    /* "bayesmsd/src/gp.pyx":191
  * 
  *     if ss_order == 0:
  *         X = trace[ti] - mean             # <<<<<<<<<<<<<<
  *         C = np.empty((N, N), dtype=float)
  *         msd2C_ss0(msd, ti, C)
  */
-    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_trace, __pyx_v_ti); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_trace, __pyx_v_ti); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = PyNumber_Subtract(__pyx_t_1, __pyx_v_mean); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Subtract(__pyx_t_1, __pyx_v_mean); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_8bayesmsd_3bin_2gp_FLOAT_t(__pyx_t_2, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_8bayesmsd_3bin_2gp_FLOAT_t(__pyx_t_2, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 191, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_X = __pyx_t_9;
     __pyx_t_9.memview = NULL;
     __pyx_t_9.data = NULL;
 
-    /* "bayesmsd/src/gp.pyx":177
+    /* "bayesmsd/src/gp.pyx":192
  *     if ss_order == 0:
  *         X = trace[ti] - mean
  *         C = np.empty((N, N), dtype=float)             # <<<<<<<<<<<<<<
  *         msd2C_ss0(msd, ti, C)
  *     elif ss_order == 1:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 192, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_v_N);
     __Pyx_GIVEREF(__pyx_v_N);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_N);
     __Pyx_INCREF(__pyx_v_N);
     __Pyx_GIVEREF(__pyx_v_N);
     PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_N);
-    __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 192, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_2);
     __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, ((PyObject *)(&PyFloat_Type))) < 0) __PYX_ERR(0, 177, __pyx_L1_error)
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 177, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, ((PyObject *)(&PyFloat_Type))) < 0) __PYX_ERR(0, 192, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 192, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_8bayesmsd_3bin_2gp_FLOAT_t(__pyx_t_4, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_8bayesmsd_3bin_2gp_FLOAT_t(__pyx_t_4, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 192, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_C = __pyx_t_10;
     __pyx_t_10.memview = NULL;
     __pyx_t_10.data = NULL;
 
-    /* "bayesmsd/src/gp.pyx":178
+    /* "bayesmsd/src/gp.pyx":193
  *         X = trace[ti] - mean
  *         C = np.empty((N, N), dtype=float)
  *         msd2C_ss0(msd, ti, C)             # <<<<<<<<<<<<<<
  *     elif ss_order == 1:
  *         X = np.diff(trace[ti]) - mean*np.diff(ti)
  */
-    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_8bayesmsd_3bin_2gp_FLOAT_t(__pyx_v_msd, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 178, __pyx_L1_error)
-    __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_8bayesmsd_3bin_2gp_SIZE_t(__pyx_v_ti, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 178, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_8bayesmsd_3bin_2gp_FLOAT_t(__pyx_v_msd, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 193, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_8bayesmsd_3bin_2gp_SIZE_t(__pyx_v_ti, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 193, __pyx_L1_error)
     __pyx_f_8bayesmsd_3bin_2gp_msd2C_ss0(__pyx_t_9, __pyx_t_11, __pyx_v_C);
     __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
     __pyx_t_9.memview = NULL;
     __pyx_t_9.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_11, 1);
     __pyx_t_11.memview = NULL;
     __pyx_t_11.data = NULL;
 
-    /* "bayesmsd/src/gp.pyx":175
+    /* "bayesmsd/src/gp.pyx":190
  *     N = len(ti)
  * 
  *     if ss_order == 0:             # <<<<<<<<<<<<<<
  *         X = trace[ti] - mean
  *         C = np.empty((N, N), dtype=float)
  */
     goto __pyx_L3;
   }
 
-  /* "bayesmsd/src/gp.pyx":179
+  /* "bayesmsd/src/gp.pyx":194
  *         C = np.empty((N, N), dtype=float)
  *         msd2C_ss0(msd, ti, C)
  *     elif ss_order == 1:             # <<<<<<<<<<<<<<
  *         X = np.diff(trace[ti]) - mean*np.diff(ti)
  *         C = np.empty((N-1, N-1), dtype=float)
  */
-  __pyx_t_4 = __Pyx_PyInt_EqObjC(__pyx_v_ss_order, __pyx_int_1, 1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 179, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_EqObjC(__pyx_v_ss_order, __pyx_int_1, 1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 179, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (likely(__pyx_t_8)) {
 
-    /* "bayesmsd/src/gp.pyx":180
+    /* "bayesmsd/src/gp.pyx":195
  *         msd2C_ss0(msd, ti, C)
  *     elif ss_order == 1:
  *         X = np.diff(trace[ti]) - mean*np.diff(ti)             # <<<<<<<<<<<<<<
  *         C = np.empty((N-1, N-1), dtype=float)
  *         msd2C_ss1(msd, ti, C)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_diff); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_diff); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_trace, __pyx_v_ti); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_trace, __pyx_v_ti); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_1, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_2);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 180, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_diff); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_diff); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_6 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_2, __pyx_v_ti) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_ti);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 180, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_Multiply(__pyx_v_mean, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Multiply(__pyx_v_mean, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = PyNumber_Subtract(__pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __pyx_t_6 = PyNumber_Subtract(__pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_8bayesmsd_3bin_2gp_FLOAT_t(__pyx_t_6, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_8bayesmsd_3bin_2gp_FLOAT_t(__pyx_t_6, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_v_X = __pyx_t_9;
     __pyx_t_9.memview = NULL;
     __pyx_t_9.data = NULL;
 
-    /* "bayesmsd/src/gp.pyx":181
+    /* "bayesmsd/src/gp.pyx":196
  *     elif ss_order == 1:
  *         X = np.diff(trace[ti]) - mean*np.diff(ti)
  *         C = np.empty((N-1, N-1), dtype=float)             # <<<<<<<<<<<<<<
  *         msd2C_ss1(msd, ti, C)
  *     else: # pragma: no cover
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 196, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_N, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_N, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 196, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_v_N, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_v_N, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 196, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 196, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_4);
     __pyx_t_6 = 0;
     __pyx_t_4 = 0;
-    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 196, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
     __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 196, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, ((PyObject *)(&PyFloat_Type))) < 0) __PYX_ERR(0, 181, __pyx_L1_error)
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 181, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, ((PyObject *)(&PyFloat_Type))) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 196, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_8bayesmsd_3bin_2gp_FLOAT_t(__pyx_t_6, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_8bayesmsd_3bin_2gp_FLOAT_t(__pyx_t_6, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 196, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_v_C = __pyx_t_10;
     __pyx_t_10.memview = NULL;
     __pyx_t_10.data = NULL;
 
-    /* "bayesmsd/src/gp.pyx":182
+    /* "bayesmsd/src/gp.pyx":197
  *         X = np.diff(trace[ti]) - mean*np.diff(ti)
  *         C = np.empty((N-1, N-1), dtype=float)
  *         msd2C_ss1(msd, ti, C)             # <<<<<<<<<<<<<<
  *     else: # pragma: no cover
  *         raise ValueError(f"Invalid steady state order: {ss_order}")
  */
-    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_8bayesmsd_3bin_2gp_FLOAT_t(__pyx_v_msd, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 182, __pyx_L1_error)
-    __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_8bayesmsd_3bin_2gp_SIZE_t(__pyx_v_ti, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 182, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_8bayesmsd_3bin_2gp_FLOAT_t(__pyx_v_msd, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_8bayesmsd_3bin_2gp_SIZE_t(__pyx_v_ti, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 197, __pyx_L1_error)
     __pyx_f_8bayesmsd_3bin_2gp_msd2C_ss1(__pyx_t_9, __pyx_t_11, __pyx_v_C);
     __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
     __pyx_t_9.memview = NULL;
     __pyx_t_9.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_11, 1);
     __pyx_t_11.memview = NULL;
     __pyx_t_11.data = NULL;
 
-    /* "bayesmsd/src/gp.pyx":179
+    /* "bayesmsd/src/gp.pyx":194
  *         C = np.empty((N, N), dtype=float)
  *         msd2C_ss0(msd, ti, C)
  *     elif ss_order == 1:             # <<<<<<<<<<<<<<
  *         X = np.diff(trace[ti]) - mean*np.diff(ti)
  *         C = np.empty((N-1, N-1), dtype=float)
  */
     goto __pyx_L3;
   }
 
-  /* "bayesmsd/src/gp.pyx":184
+  /* "bayesmsd/src/gp.pyx":199
  *         msd2C_ss1(msd, ti, C)
  *     else: # pragma: no cover
  *         raise ValueError(f"Invalid steady state order: {ss_order}")             # <<<<<<<<<<<<<<
  * 
  *     return _core_logL(C, X, X.copy())
  */
   /*else*/ {
-    __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_v_ss_order, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_v_ss_order, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Invalid_steady_state_order, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Invalid_steady_state_order, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 184, __pyx_L1_error)
+    __PYX_ERR(0, 199, __pyx_L1_error)
   }
   __pyx_L3:;
 
-  /* "bayesmsd/src/gp.pyx":186
+  /* "bayesmsd/src/gp.pyx":201
  *         raise ValueError(f"Invalid steady state order: {ss_order}")
  * 
  *     return _core_logL(C, X, X.copy())             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_9 = __pyx_memoryview_copy_slice_dc_nn___pyx_t_8bayesmsd_3bin_2gp_FLOAT_t_c(__pyx_v_X); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 186, __pyx_L1_error)
-  __pyx_t_6 = PyFloat_FromDouble(__pyx_f_8bayesmsd_3bin_2gp__core_logL(__pyx_v_C, __pyx_v_X, __pyx_t_9)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 186, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_9 = __pyx_memoryview_copy_slice_dc_nn___pyx_t_8bayesmsd_3bin_2gp_FLOAT_t_c(__pyx_v_X); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_t_12 = __pyx_f_8bayesmsd_3bin_2gp__core_logL(__pyx_v_C, __pyx_v_X, __pyx_t_9); if (unlikely(__pyx_t_12 == ((__pyx_t_8bayesmsd_3bin_2gp_FLOAT_t)1e300) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L1_error)
   __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
   __pyx_t_9.memview = NULL;
   __pyx_t_9.data = NULL;
+  __pyx_t_6 = PyFloat_FromDouble(__pyx_t_12); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "bayesmsd/src/gp.pyx":140
+  /* "bayesmsd/src/gp.pyx":155
  *     return -0.5*( xCx + logdet + N*LOG_2PI )
  * 
  * def logL(trace, ss_order, msd, mean=0):             # <<<<<<<<<<<<<<
  *     """
  *     Gaussian process likelihood for a given trace
  */
 
@@ -19026,16 +19054,16 @@
   {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 38, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 199, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 149, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 152, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 834, __pyx_L1_error)
@@ -19261,25 +19289,25 @@
   __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
   __pyx_tuple__21 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
 
-  /* "bayesmsd/src/gp.pyx":140
+  /* "bayesmsd/src/gp.pyx":155
  *     return -0.5*( xCx + logdet + N*LOG_2PI )
  * 
  * def logL(trace, ss_order, msd, mean=0):             # <<<<<<<<<<<<<<
  *     """
  *     Gaussian process likelihood for a given trace
  */
-  __pyx_tuple__22 = PyTuple_Pack(8, __pyx_n_s_trace, __pyx_n_s_ss_order, __pyx_n_s_msd, __pyx_n_s_mean, __pyx_n_s_C, __pyx_n_s_X, __pyx_n_s_ti, __pyx_n_s_N); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 140, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(8, __pyx_n_s_trace, __pyx_n_s_ss_order, __pyx_n_s_msd, __pyx_n_s_mean, __pyx_n_s_C, __pyx_n_s_X, __pyx_n_s_ti, __pyx_n_s_N); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(4, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bayesmsd_src_gp_pyx, __pyx_n_s_logL, 140, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 140, __pyx_L1_error)
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(4, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bayesmsd_src_gp_pyx, __pyx_n_s_logL, 155, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 155, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
@@ -19758,98 +19786,100 @@
   (void)__Pyx_modinit_variable_import_code();
   if (unlikely(__Pyx_modinit_function_import_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "bayesmsd/src/gp.pyx":1
+  /* "bayesmsd/src/gp.pyx":13
+ * #       assembling, 90% on computation
+ * 
  * import numpy as np             # <<<<<<<<<<<<<<
  * cimport numpy as np
  * np.import_array()
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "bayesmsd/src/gp.pyx":3
+  /* "bayesmsd/src/gp.pyx":15
  * import numpy as np
  * cimport numpy as np
  * np.import_array()             # <<<<<<<<<<<<<<
  * 
  * import cython
  */
-  __pyx_t_2 = __pyx_f_5numpy_import_array(); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_5numpy_import_array(); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 15, __pyx_L1_error)
 
-  /* "bayesmsd/src/gp.pyx":12
+  /* "bayesmsd/src/gp.pyx":24
  * from scipy.linalg.cython_lapack cimport dpotrf
  * 
  * from ..src.gp_py import BadCovarianceError             # <<<<<<<<<<<<<<
  * 
  * ctypedef double FLOAT_t
  */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_BadCovarianceError);
   __Pyx_GIVEREF(__pyx_n_s_BadCovarianceError);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_BadCovarianceError);
-  __pyx_t_3 = __Pyx_Import(__pyx_n_s_src_gp_py, __pyx_t_1, 2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Import(__pyx_n_s_src_gp_py, __pyx_t_1, 2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_BadCovarianceError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_BadCovarianceError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_BadCovarianceError, __pyx_t_1) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_BadCovarianceError, __pyx_t_1) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "bayesmsd/src/gp.pyx":93
+  /* "bayesmsd/src/gp.pyx":108
  * # use dscal for 0.5*
  * 
  * cdef FLOAT_t LOG_2PI = np.log(2*np.pi)             # <<<<<<<<<<<<<<
  * 
  * @cython.boundscheck(False)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_log); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_log); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_pi); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_pi); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_Multiply(__pyx_int_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_int_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_8bayesmsd_3bin_2gp_LOG_2PI = __pyx_t_5;
 
-  /* "bayesmsd/src/gp.pyx":140
+  /* "bayesmsd/src/gp.pyx":155
  *     return -0.5*( xCx + logdet + N*LOG_2PI )
  * 
  * def logL(trace, ss_order, msd, mean=0):             # <<<<<<<<<<<<<<
  *     """
  *     Gaussian process likelihood for a given trace
  */
-  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_8bayesmsd_3bin_2gp_1logL, NULL, __pyx_n_s_bayesmsd_bin_gp); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 140, __pyx_L1_error)
+  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_8bayesmsd_3bin_2gp_1logL, NULL, __pyx_n_s_bayesmsd_bin_gp); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_logL, __pyx_t_4) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_logL, __pyx_t_4) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "bayesmsd/src/gp.pyx":1
- * import numpy as np             # <<<<<<<<<<<<<<
- * cimport numpy as np
- * np.import_array()
+ * ## cython: profiling=True             # <<<<<<<<<<<<<<
+ * # ^ remove second # to compile for profiler
+ * ## cython: linetrace=True
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_4) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "View.MemoryView":210
```

### Comparing `bayesmsd-0.1.2/bayesmsd/src/gp_py.py` & `bayesmsd-0.1.3/bayesmsd/src/gp_py.py`

 * *Files identical despite different names*

### Comparing `bayesmsd-0.1.2/bayesmsd.egg-info/PKG-INFO` & `bayesmsd-0.1.3/bayesmsd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayesmsd
-Version: 0.1.2
+Version: 0.1.3
 Summary: Bayesian MSD fitting
 Author-email: Simon Grosse-Holz <sgh256@mit.edu>
 License: MIT License
         
         Copyright (c) 2022 Simon Grosse-Holz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bayesmsd-0.1.2/pyproject.toml` & `bayesmsd-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel", "numpy>=1.20"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bayesmsd"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Simon Grosse-Holz", email="sgh256@mit.edu" }
 ]
 description = "Bayesian MSD fitting"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `bayesmsd-0.1.2/setup.py` & `bayesmsd-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `bayesmsd-0.1.2/tests/test_bayesmsd.py` & `bayesmsd-0.1.3/tests/test_bayesmsd.py`

 * *Files 0% similar despite different names*

```diff
@@ -946,382 +946,383 @@
 00003b10: 6d63 6920 3d20 7072 6f66 696c 6572 2e66  mci = profiler.f
 00003b20: 696e 645f 4d43 4928 290a 0a20 2020 2020  ind_MCI()..     
 00003b30: 2020 2066 6f72 206e 616d 6520 696e 206e     for name in n
 00003b40: 616d 6573 3a0a 2020 2020 2020 2020 2020  ames:.          
 00003b50: 2020 7365 6c66 2e61 7373 6572 745f 6172    self.assert_ar
 00003b60: 7261 795f 6571 7561 6c28 6d63 695b 6e61  ray_equal(mci[na
 00003b70: 6d65 5d5b 315d 2c20 5b2d 6e70 2e69 6e66  me][1], [-np.inf
-00003b80: 2c20 6e70 2e69 6e66 5d29 0a20 2020 200a  , np.inf]).    .
-00003b90: 2020 2020 6465 6620 7465 7374 5f73 696e      def test_sin
-00003ba0: 676c 6570 6172 616d 5f6e 6f5f 7072 6f66  gleparam_no_prof
-00003bb0: 696c 696e 6728 7365 6c66 293a 0a20 2020  iling(self):.   
-00003bc0: 2020 2020 2073 656c 662e 6669 742e 7061       self.fit.pa
-00003bd0: 7261 6d65 7465 7273 5b27 7930 275d 2e66  rameters['y0'].f
-00003be0: 6978 5f74 6f20 3d20 300a 2020 2020 2020  ix_to = 0.      
-00003bf0: 2020 7072 6f66 696c 6572 203d 2062 6179    profiler = bay
-00003c00: 6573 6d73 642e 5072 6f66 696c 6572 2873  esmsd.Profiler(s
-00003c10: 656c 662e 6669 742c 2070 726f 6669 6c69  elf.fit, profili
-00003c20: 6e67 3d54 7275 652c 2076 6572 626f 7369  ng=True, verbosi
-00003c30: 7479 3d30 290a 2020 2020 2020 2020 7365  ty=0).        se
-00003c40: 6c66 2e61 7373 6572 7446 616c 7365 2870  lf.assertFalse(p
-00003c50: 726f 6669 6c65 722e 7072 6f66 696c 696e  rofiler.profilin
-00003c60: 6729 0a0a 2020 2020 6465 6620 7465 7374  g)..    def test
-00003c70: 436c 6f73 6573 7452 6573 2873 656c 6629  ClosestRes(self)
-00003c80: 3a0a 2020 2020 2020 2020 7072 6f66 696c  :.        profil
-00003c90: 6572 203d 2062 6179 6573 6d73 642e 5072  er = bayesmsd.Pr
-00003ca0: 6f66 696c 6572 2873 656c 662e 6669 7429  ofiler(self.fit)
-00003cb0: 0a20 2020 2020 2020 2070 726f 6669 6c65  .        profile
-00003cc0: 722e 7275 6e5f 6669 7428 290a 2020 2020  r.run_fit().    
-00003cd0: 2020 2020 7265 7320 3d20 7072 6f66 696c      res = profil
-00003ce0: 6572 2e70 6f69 6e74 5f65 7374 696d 6174  er.point_estimat
-00003cf0: 650a 2020 2020 2020 2020 7072 6f66 696c  e.        profil
-00003d00: 6572 2e63 7572 5f70 6172 616d 203d 2022  er.cur_param = "
-00003d10: 7930 220a 0a20 2020 2020 2020 2063 6c6f  y0"..        clo
-00003d20: 7365 7374 203d 2070 726f 6669 6c65 722e  sest = profiler.
-00003d30: 6669 6e64 5f63 6c6f 7365 7374 5f72 6573  find_closest_res
-00003d40: 2872 6573 5b27 7061 7261 6d73 275d 5b22  (res['params']["
-00003d50: 7930 225d 290a 2020 2020 2020 2020 7365  y0"]).        se
-00003d60: 6c66 2e61 7373 6572 7449 7328 636c 6f73  lf.assertIs(clos
-00003d70: 6573 742c 2072 6573 290a 0a20 2020 2020  est, res)..     
-00003d80: 2020 2077 6974 6820 7365 6c66 2e61 7373     with self.ass
-00003d90: 6572 7452 6169 7365 7328 5275 6e74 696d  ertRaises(Runtim
-00003da0: 6545 7272 6f72 293a 0a20 2020 2020 2020  eError):.       
-00003db0: 2020 2020 2063 6c6f 7365 7374 203d 2070       closest = p
-00003dc0: 726f 6669 6c65 722e 6669 6e64 5f63 6c6f  rofiler.find_clo
-00003dd0: 7365 7374 5f72 6573 2872 6573 5b27 7061  sest_res(res['pa
-00003de0: 7261 6d73 275d 5b22 7930 225d 202b 2031  rams']["y0"] + 1
-00003df0: 2c20 6469 7265 6374 696f 6e3d 3129 0a0a  , direction=1)..
-00003e00: 2020 2020 6465 6620 7465 7374 4c69 6b65      def testLike
-00003e10: 6c69 686f 6f64 5368 6170 6573 2873 656c  lihoodShapes(sel
-00003e20: 6629 3a0a 2020 2020 2020 2020 7072 6f66  f):.        prof
-00003e30: 696c 6572 203d 2062 6179 6573 6d73 642e  iler = bayesmsd.
-00003e40: 5072 6f66 696c 6572 2873 656c 662e 6669  Profiler(self.fi
-00003e50: 742c 2070 726f 6669 6c69 6e67 3d46 616c  t, profiling=Fal
-00003e60: 7365 290a 0a20 2020 2020 2020 2023 2048  se)..        # H
-00003e70: 6974 2062 6f75 6e64 7320 7768 696c 6520  it bounds while 
-00003e80: 6272 6163 6b65 7469 6e67 2028 6c65 6674  bracketing (left
-00003e90: 7761 7264 7329 0a20 2020 2020 2020 2023  wards).        #
-00003ea0: 2048 6974 206a 756d 7020 7768 696c 6520   Hit jump while 
-00003eb0: 6269 7365 6374 696e 6720 2020 2028 7269  bisecting    (ri
-00003ec0: 6768 7477 6172 6473 290a 2020 2020 2020  ghtwards).      
-00003ed0: 2020 7072 6f66 696c 6572 2e66 6974 2e70    profiler.fit.p
-00003ee0: 6172 616d 6574 6572 735b 2779 3027 5d2e  arameters['y0'].
-00003ef0: 626f 756e 6473 203d 2028 302c 2031 290a  bounds = (0, 1).
-00003f00: 2020 2020 2020 2020 7072 6f66 696c 6572          profiler
-00003f10: 2e66 6974 2e70 6172 616d 6574 6572 735b  .fit.parameters[
-00003f20: 2779 3127 5d2e 626f 756e 6473 203d 2028  'y1'].bounds = (
-00003f30: 302c 2031 290a 2020 2020 2020 2020 7072  0, 1).        pr
-00003f40: 6f66 696c 6572 2e70 6f69 6e74 5f65 7374  ofiler.point_est
-00003f50: 696d 6174 6520 3d20 7b27 7061 7261 6d73  imate = {'params
-00003f60: 2720 3a20 7b27 7930 2720 3a20 302e 352c  ' : {'y0' : 0.5,
-00003f70: 2027 7931 2720 3a20 302e 357d 2c0a 2020   'y1' : 0.5},.  
-00003f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b80: 2c20 6261 7965 736d 7364 2e6c 6962 2e5f  , bayesmsd.lib._
+00003b90: 4d41 585f 4c4f 475d 290a 2020 2020 0a20  MAX_LOG]).    . 
+00003ba0: 2020 2064 6566 2074 6573 745f 7369 6e67     def test_sing
+00003bb0: 6c65 7061 7261 6d5f 6e6f 5f70 726f 6669  leparam_no_profi
+00003bc0: 6c69 6e67 2873 656c 6629 3a0a 2020 2020  ling(self):.    
+00003bd0: 2020 2020 7365 6c66 2e66 6974 2e70 6172      self.fit.par
+00003be0: 616d 6574 6572 735b 2779 3027 5d2e 6669  ameters['y0'].fi
+00003bf0: 785f 746f 203d 2030 0a20 2020 2020 2020  x_to = 0.       
+00003c00: 2070 726f 6669 6c65 7220 3d20 6261 7965   profiler = baye
+00003c10: 736d 7364 2e50 726f 6669 6c65 7228 7365  smsd.Profiler(se
+00003c20: 6c66 2e66 6974 2c20 7072 6f66 696c 696e  lf.fit, profilin
+00003c30: 673d 5472 7565 2c20 7665 7262 6f73 6974  g=True, verbosit
+00003c40: 793d 3029 0a20 2020 2020 2020 2073 656c  y=0).        sel
+00003c50: 662e 6173 7365 7274 4661 6c73 6528 7072  f.assertFalse(pr
+00003c60: 6f66 696c 6572 2e70 726f 6669 6c69 6e67  ofiler.profiling
+00003c70: 290a 0a20 2020 2064 6566 2074 6573 7443  )..    def testC
+00003c80: 6c6f 7365 7374 5265 7328 7365 6c66 293a  losestRes(self):
+00003c90: 0a20 2020 2020 2020 2070 726f 6669 6c65  .        profile
+00003ca0: 7220 3d20 6261 7965 736d 7364 2e50 726f  r = bayesmsd.Pro
+00003cb0: 6669 6c65 7228 7365 6c66 2e66 6974 290a  filer(self.fit).
+00003cc0: 2020 2020 2020 2020 7072 6f66 696c 6572          profiler
+00003cd0: 2e72 756e 5f66 6974 2829 0a20 2020 2020  .run_fit().     
+00003ce0: 2020 2072 6573 203d 2070 726f 6669 6c65     res = profile
+00003cf0: 722e 706f 696e 745f 6573 7469 6d61 7465  r.point_estimate
+00003d00: 0a20 2020 2020 2020 2070 726f 6669 6c65  .        profile
+00003d10: 722e 6375 725f 7061 7261 6d20 3d20 2279  r.cur_param = "y
+00003d20: 3022 0a0a 2020 2020 2020 2020 636c 6f73  0"..        clos
+00003d30: 6573 7420 3d20 7072 6f66 696c 6572 2e66  est = profiler.f
+00003d40: 696e 645f 636c 6f73 6573 745f 7265 7328  ind_closest_res(
+00003d50: 7265 735b 2770 6172 616d 7327 5d5b 2279  res['params']["y
+00003d60: 3022 5d29 0a20 2020 2020 2020 2073 656c  0"]).        sel
+00003d70: 662e 6173 7365 7274 4973 2863 6c6f 7365  f.assertIs(close
+00003d80: 7374 2c20 7265 7329 0a0a 2020 2020 2020  st, res)..      
+00003d90: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
+00003da0: 7274 5261 6973 6573 2852 756e 7469 6d65  rtRaises(Runtime
+00003db0: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
+00003dc0: 2020 2020 636c 6f73 6573 7420 3d20 7072      closest = pr
+00003dd0: 6f66 696c 6572 2e66 696e 645f 636c 6f73  ofiler.find_clos
+00003de0: 6573 745f 7265 7328 7265 735b 2770 6172  est_res(res['par
+00003df0: 616d 7327 5d5b 2279 3022 5d20 2b20 312c  ams']["y0"] + 1,
+00003e00: 2064 6972 6563 7469 6f6e 3d31 290a 0a20   direction=1).. 
+00003e10: 2020 2064 6566 2074 6573 744c 696b 656c     def testLikel
+00003e20: 6968 6f6f 6453 6861 7065 7328 7365 6c66  ihoodShapes(self
+00003e30: 293a 0a20 2020 2020 2020 2070 726f 6669  ):.        profi
+00003e40: 6c65 7220 3d20 6261 7965 736d 7364 2e50  ler = bayesmsd.P
+00003e50: 726f 6669 6c65 7228 7365 6c66 2e66 6974  rofiler(self.fit
+00003e60: 2c20 7072 6f66 696c 696e 673d 4661 6c73  , profiling=Fals
+00003e70: 6529 0a0a 2020 2020 2020 2020 2320 4869  e)..        # Hi
+00003e80: 7420 626f 756e 6473 2077 6869 6c65 2062  t bounds while b
+00003e90: 7261 636b 6574 696e 6720 286c 6566 7477  racketing (leftw
+00003ea0: 6172 6473 290a 2020 2020 2020 2020 2320  ards).        # 
+00003eb0: 4869 7420 6a75 6d70 2077 6869 6c65 2062  Hit jump while b
+00003ec0: 6973 6563 7469 6e67 2020 2020 2872 6967  isecting    (rig
+00003ed0: 6874 7761 7264 7329 0a20 2020 2020 2020  htwards).       
+00003ee0: 2070 726f 6669 6c65 722e 6669 742e 7061   profiler.fit.pa
+00003ef0: 7261 6d65 7465 7273 5b27 7930 275d 2e62  rameters['y0'].b
+00003f00: 6f75 6e64 7320 3d20 2830 2c20 3129 0a20  ounds = (0, 1). 
+00003f10: 2020 2020 2020 2070 726f 6669 6c65 722e         profiler.
+00003f20: 6669 742e 7061 7261 6d65 7465 7273 5b27  fit.parameters['
+00003f30: 7931 275d 2e62 6f75 6e64 7320 3d20 2830  y1'].bounds = (0
+00003f40: 2c20 3129 0a20 2020 2020 2020 2070 726f  , 1).        pro
+00003f50: 6669 6c65 722e 706f 696e 745f 6573 7469  filer.point_esti
+00003f60: 6d61 7465 203d 207b 2770 6172 616d 7327  mate = {'params'
+00003f70: 203a 207b 2779 3027 203a 2030 2e35 2c20   : {'y0' : 0.5, 
+00003f80: 2779 3127 203a 2030 2e35 7d2c 0a20 2020  'y1' : 0.5},.   
 00003f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003fa0: 2027 6c6f 674c 2720 3a20 302e 2c0a 2020   'logL' : 0.,.  
-00003fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fb0: 276c 6f67 4c27 203a 2030 2e2c 0a20 2020  'logL' : 0.,.   
 00003fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003fd0: 7d0a 0a20 2020 2020 2020 2023 203c 736f  }..        # <so
-00003fe0: 6d65 2075 676c 7920 6861 636b 696e 6720  me ugly hacking 
-00003ff0: 746f 2067 6574 2061 2075 7365 722d 6465  to get a user-de
-00004000: 6669 6e65 6420 6c69 6b65 6c69 686f 6f64  fined likelihood
-00004010: 2066 756e 6374 696f 6e3e 0a20 2020 2020   function>.     
-00004020: 2020 206d 696e 5f74 6172 6765 7420 3d20     min_target = 
-00004030: 7365 6c66 2e66 6974 2e4d 696e 5461 7267  self.fit.MinTarg
-00004040: 6574 2873 656c 662e 6669 7429 0a20 2020  et(self.fit).   
-00004050: 2020 2020 2064 6566 205f 6d69 6e5f 7461       def _min_ta
-00004060: 7267 6574 2873 656c 662c 2070 6172 616d  rget(self, param
-00004070: 735f 6172 7261 7929 3a0a 2020 2020 2020  s_array):.      
-00004080: 2020 2020 2020 7061 7261 6d73 203d 206d        params = m
-00004090: 696e 5f74 6172 6765 742e 7061 7261 6d73  in_target.params
-000040a0: 5f61 7272 6179 3264 6963 7428 7061 7261  _array2dict(para
-000040b0: 6d73 5f61 7272 6179 290a 2020 2020 2020  ms_array).      
-000040c0: 2020 2020 2020 7265 7475 726e 2030 2069        return 0 i
-000040d0: 6620 7061 7261 6d73 5b27 7930 275d 203c  f params['y0'] <
-000040e0: 2030 2e37 3320 656c 7365 2031 6531 300a   0.73 else 1e10.
-000040f0: 0a23 2076 7676 7676 7676 7676 7676 7676  .# vvvvvvvvvvvvv
-00004100: 7676 7676 7676 7676 0a20 2020 2020 2020  vvvvvvvv.       
-00004110: 204d 696e 5461 7267 6574 5f5f 6361 6c6c   MinTarget__call
-00004120: 5f5f 203d 2074 7970 6528 6d69 6e5f 7461  __ = type(min_ta
-00004130: 7267 6574 292e 5f5f 6361 6c6c 5f5f 0a20  rget).__call__. 
-00004140: 2020 2020 2020 2074 7970 6528 6d69 6e5f         type(min_
-00004150: 7461 7267 6574 292e 5f5f 6361 6c6c 5f5f  target).__call__
-00004160: 203d 205f 6d69 6e5f 7461 7267 6574 0a23   = _min_target.#
-00004170: 205e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e   ^^^^^^^^^^^^^^^
-00004180: 5e5e 5e5e 5e5e 0a0a 2020 2020 2020 2020  ^^^^^^..        
-00004190: 7072 6f66 696c 6572 2e6d 696e 5f74 6172  profiler.min_tar
-000041a0: 6765 745f 6672 6f6d 5f66 6974 203d 206d  get_from_fit = m
-000041b0: 696e 5f74 6172 6765 740a 0a20 2020 2020  in_target..     
-000041c0: 2020 206d 2c20 726f 6f74 7320 3d20 7072     m, roots = pr
-000041d0: 6f66 696c 6572 2e66 696e 645f 4d43 4928  ofiler.find_MCI(
-000041e0: 2279 3022 295b 2279 3022 5d0a 2020 2020  "y0")["y0"].    
-000041f0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00004200: 7175 616c 2872 6f6f 7473 5b30 5d2c 2030  qual(roots[0], 0
-00004210: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00004220: 7373 6572 7441 6c6d 6f73 7445 7175 616c  ssertAlmostEqual
-00004230: 2872 6f6f 7473 5b31 5d2c 2030 2e37 3329  (roots[1], 0.73)
-00004240: 0a0a 2320 7676 7676 7676 7676 7676 7676  ..# vvvvvvvvvvvv
-00004250: 7676 7676 7676 7676 760a 2020 2020 2020  vvvvvvvvv.      
-00004260: 2020 7479 7065 286d 696e 5f74 6172 6765    type(min_targe
-00004270: 7429 2e5f 5f63 616c 6c5f 5f20 3d20 4d69  t).__call__ = Mi
-00004280: 6e54 6172 6765 745f 5f63 616c 6c5f 5f0a  nTarget__call__.
-00004290: 2320 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  # ^^^^^^^^^^^^^^
-000042a0: 5e5e 5e5e 5e5e 5e0a 0a63 6c61 7373 2054  ^^^^^^^..class T
-000042b0: 6573 7452 616e 646f 6d53 7475 6666 286d  estRandomStuff(m
-000042c0: 7954 6573 7443 6173 6529 3a0a 2020 2020  yTestCase):.    
-000042d0: 6465 6620 7465 7374 5f4d 5344 2873 656c  def test_MSD(sel
-000042e0: 6629 3a0a 2020 2020 2020 2020 6461 7461  f):.        data
-000042f0: 203d 206e 6c2e 5461 6767 6564 5365 7428   = nl.TaggedSet(
-00004300: 5b6e 6c2e 5472 616a 6563 746f 7279 285b  [nl.Trajectory([
-00004310: 5b31 2c20 322c 2033 5d2c 205b 342c 2035  [1, 2, 3], [4, 5
-00004320: 2c20 365d 5d29 5d2c 2068 6173 5461 6773  , 6]])], hasTags
-00004330: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
-00004340: 6669 7420 3d20 6261 7965 736d 7364 2e6c  fit = bayesmsd.l
-00004350: 6962 2e4e 5058 4669 7428 6461 7461 2c20  ib.NPXFit(data, 
-00004360: 7373 5f6f 7264 6572 3d31 2c20 6e3d 3029  ss_order=1, n=0)
-00004370: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
-00004380: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-00004390: 276c 6f67 28cf 83c2 b229 2028 6469 6d20  'log(....) (dim 
-000043a0: 3029 2720 3a20 2d6e 702e 696e 662c 0a20  0)' : -np.inf,. 
-000043b0: 2020 2020 2020 2020 2020 2020 276c 6f67              'log
-000043c0: 28ce 9329 2028 6469 6d20 3029 2720 3a20  (..) (dim 0)' : 
-000043d0: 302e 3338 372c 0a20 2020 2020 2020 2020  0.387,.         
-000043e0: 2020 2020 2020 2020 2027 ceb1 2028 6469           '.. (di
-000043f0: 6d20 3029 2720 3a20 302e 3839 2c0a 2020  m 0)' : 0.89,.  
-00004400: 2020 2020 2020 2020 2020 276c 6f67 28cf            'log(.
-00004410: 83c2 b229 2028 6469 6d20 3129 2720 3a20  ...) (dim 1)' : 
-00004420: 2d6e 702e 696e 662c 0a20 2020 2020 2020  -np.inf,.       
-00004430: 2020 2020 2020 276c 6f67 28ce 9329 2028        'log(..) (
-00004440: 6469 6d20 3129 2720 3a20 302e 3338 372c  dim 1)' : 0.387,
-00004450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004460: 2020 2027 ceb1 2028 6469 6d20 3129 2720     '.. (dim 1)' 
-00004470: 3a20 302e 3839 2c0a 2020 2020 2020 2020  : 0.89,.        
-00004480: 2020 2020 276c 6f67 28cf 83c2 b229 2028      'log(....) (
-00004490: 6469 6d20 3229 2720 3a20 2d6e 702e 696e  dim 2)' : -np.in
-000044a0: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
-000044b0: 276c 6f67 28ce 9329 2028 6469 6d20 3229  'log(..) (dim 2)
-000044c0: 2720 3a20 302e 3338 372c 0a20 2020 2020  ' : 0.387,.     
-000044d0: 2020 2020 2020 2020 2020 2020 2027 ceb1               '..
-000044e0: 2028 6469 6d20 3229 2720 3a20 302e 3839   (dim 2)' : 0.89
-000044f0: 2c0a 2020 2020 2020 2020 7d0a 0a20 2020  ,.        }..   
-00004500: 2020 2020 206d 7364 203d 2066 6974 2e4d       msd = fit.M
-00004510: 5344 2870 6172 616d 7329 0a20 2020 2020  SD(params).     
-00004520: 2020 2064 6f63 7374 7269 6e67 203d 206d     docstring = m
-00004530: 7364 2e5f 5f64 6f63 5f5f 0a20 2020 2020  sd.__doc__.     
-00004540: 2020 2073 656c 662e 6173 7365 7274 496e     self.assertIn
-00004550: 2866 2228 6474 2c22 2c20 646f 6373 7472  (f"(dt,", docstr
-00004560: 696e 6729 0a20 2020 2020 2020 2073 656c  ing).        sel
-00004570: 662e 6173 7365 7274 496e 2866 227b 7061  f.assertIn(f"{pa
-00004580: 7261 6d73 5b27 ceb1 2028 6469 6d20 3029  rams['.. (dim 0)
-00004590: 275d 7d22 2c20 646f 6373 7472 696e 6729  ']}", docstring)
-000045a0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-000045b0: 7365 7274 496e 2866 227b 6e70 2e65 7870  sertIn(f"{np.exp
-000045c0: 2870 6172 616d 735b 276c 6f67 28ce 9329  (params['log(..)
-000045d0: 2028 6469 6d20 3029 275d 293a 2e34 667d   (dim 0)']):.4f}
-000045e0: 225b 3a2d 315d 2c20 646f 6373 7472 696e  "[:-1], docstrin
-000045f0: 6729 2023 2070 7265 7665 6e74 2072 6f75  g) # prevent rou
-00004600: 6e64 696e 672c 206a 7573 7420 7472 756e  nding, just trun
-00004610: 6361 7465 0a0a 2020 2020 2020 2020 6474  cate..        dt
-00004620: 203d 206e 702e 6172 616e 6765 2831 2c20   = np.arange(1, 
-00004630: 3130 290a 2020 2020 2020 2020 6c6f 6747  10).        logG
-00004640: 2020 3d20 7061 7261 6d73 5b27 6c6f 6728    = params['log(
-00004650: ce93 2920 2864 696d 2030 2927 5d0a 2020  ..) (dim 0)'].  
-00004660: 2020 2020 2020 616c 7068 6120 3d20 7061        alpha = pa
-00004670: 7261 6d73 5b20 2020 2020 27ce b120 2864  rams[     '.. (d
-00004680: 696d 2030 2927 5d0a 2020 2020 2020 2020  im 0)'].        
-00004690: 7365 6c66 2e61 7373 6572 745f 6172 7261  self.assert_arra
-000046a0: 795f 616c 6d6f 7374 5f65 7175 616c 286d  y_almost_equal(m
-000046b0: 7364 2864 7429 2c20 6461 7461 5b30 5d2e  sd(dt), data[0].
-000046c0: 642a 6e70 2e65 7870 2861 6c70 6861 2a6e  d*np.exp(alpha*n
-000046d0: 702e 6c6f 6728 6474 2920 2b20 6c6f 6747  p.log(dt) + logG
-000046e0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-000046f0: 6173 7365 7274 5f61 7272 6179 5f61 6c6d  assert_array_alm
-00004700: 6f73 745f 6571 7561 6c28 6d73 6428 6474  ost_equal(msd(dt
-00004710: 292c 2066 6974 2e4d 5344 2870 6172 616d  ), fit.MSD(param
-00004720: 732c 2064 7429 290a 0a20 2020 2064 6566  s, dt))..    def
-00004730: 2074 6573 745f 6765 6e65 7261 7465 2873   test_generate(s
-00004740: 656c 6629 3a0a 2020 2020 2020 2020 6461  elf):.        da
-00004750: 7461 203d 206e 6c2e 5461 6767 6564 5365  ta = nl.TaggedSe
-00004760: 7428 5b6e 6c2e 5472 616a 6563 746f 7279  t([nl.Trajectory
-00004770: 285b 5b31 2c20 322c 2033 5d2c 205b 342c  ([[1, 2, 3], [4,
-00004780: 2035 2c20 365d 5d29 5d2c 2068 6173 5461   5, 6]])], hasTa
-00004790: 6773 3d46 616c 7365 290a 2020 2020 2020  gs=False).      
-000047a0: 2020 6669 7420 3d20 6261 7965 736d 7364    fit = bayesmsd
-000047b0: 2e6c 6962 2e4e 5058 4669 7428 6461 7461  .lib.NPXFit(data
-000047c0: 2c20 7373 5f6f 7264 6572 3d31 2c20 6e3d  , ss_order=1, n=
-000047d0: 3029 0a20 2020 2020 2020 2070 6172 616d  0).        param
-000047e0: 7320 3d20 7b0a 2020 2020 2020 2020 2020  s = {.          
-000047f0: 2020 276c 6f67 28cf 83c2 b229 2028 6469    'log(....) (di
-00004800: 6d20 3029 2720 3a20 2d6e 702e 696e 662c  m 0)' : -np.inf,
-00004810: 0a20 2020 2020 2020 2020 2020 2020 276c  .             'l
-00004820: 6f67 28ce 9329 2028 6469 6d20 3029 2720  og(..) (dim 0)' 
-00004830: 3a20 302e 3338 372c 0a20 2020 2020 2020  : 0.387,.       
-00004840: 2020 2020 2020 2020 2020 2027 ceb1 2028             '.. (
-00004850: 6469 6d20 3029 2720 3a20 302e 3839 2c0a  dim 0)' : 0.89,.
-00004860: 2020 2020 2020 2020 2020 2020 276c 6f67              'log
-00004870: 28cf 83c2 b229 2028 6469 6d20 3129 2720  (....) (dim 1)' 
-00004880: 3a20 2d6e 702e 696e 662c 0a20 2020 2020  : -np.inf,.     
-00004890: 2020 2020 2020 2020 276c 6f67 28ce 9329          'log(..)
-000048a0: 2028 6469 6d20 3129 2720 3a20 302e 3338   (dim 1)' : 0.38
-000048b0: 372c 0a20 2020 2020 2020 2020 2020 2020  7,.             
-000048c0: 2020 2020 2027 ceb1 2028 6469 6d20 3129       '.. (dim 1)
-000048d0: 2720 3a20 302e 3839 2c0a 2020 2020 2020  ' : 0.89,.      
-000048e0: 2020 2020 2020 276c 6f67 28cf 83c2 b229        'log(....)
-000048f0: 2028 6469 6d20 3229 2720 3a20 2d6e 702e   (dim 2)' : -np.
-00004900: 696e 662c 0a20 2020 2020 2020 2020 2020  inf,.           
-00004910: 2020 276c 6f67 28ce 9329 2028 6469 6d20    'log(..) (dim 
-00004920: 3229 2720 3a20 302e 3338 372c 0a20 2020  2)' : 0.387,.   
-00004930: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00004940: ceb1 2028 6469 6d20 3229 2720 3a20 302e  .. (dim 2)' : 0.
-00004950: 3839 2c0a 2020 2020 2020 2020 7d0a 0a20  89,.        }.. 
-00004960: 2020 2020 2020 2064 6174 615f 7361 6d70         data_samp
-00004970: 6c65 203d 2062 6179 6573 6d73 642e 6770  le = bayesmsd.gp
-00004980: 2e67 656e 6572 6174 6528 2866 6974 2c20  .generate((fit, 
-00004990: 6469 6374 2870 6172 616d 733d 7061 7261  dict(params=para
-000049a0: 6d73 2929 2c20 3130 2c20 6e3d 3229 0a20  ms)), 10, n=2). 
-000049b0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000049c0: 7274 4571 7561 6c28 6c65 6e28 6461 7461  rtEqual(len(data
-000049d0: 5f73 616d 706c 6529 2c20 3229 0a20 2020  _sample), 2).   
-000049e0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000049f0: 4571 7561 6c28 6c65 6e28 6461 7461 5f73  Equal(len(data_s
-00004a00: 616d 706c 655b 305d 292c 2031 3029 0a20  ample[0]), 10). 
-00004a10: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00004a20: 7274 4571 7561 6c28 6461 7461 5f73 616d  rtEqual(data_sam
-00004a30: 706c 655b 305d 2e64 2c20 3329 0a20 2020  ple[0].d, 3).   
-00004a40: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00004a50: 5472 7565 286e 702e 616c 6c28 6e70 2e61  True(np.all(np.a
-00004a60: 7272 6179 285b 7472 616a 5b30 5d20 666f  rray([traj[0] fo
-00004a70: 7220 7472 616a 2069 6e20 6461 7461 5f73  r traj in data_s
-00004a80: 616d 706c 655d 2920 3d3d 2030 2929 0a0a  ample]) == 0))..
-00004a90: 2020 2020 2020 2020 6669 7420 3d20 6261          fit = ba
-00004aa0: 7965 736d 7364 2e6c 6962 2e4e 5058 4669  yesmsd.lib.NPXFi
-00004ab0: 7428 6461 7461 2c20 7373 5f6f 7264 6572  t(data, ss_order
-00004ac0: 3d30 2c20 6e3d 3129 0a20 2020 2020 2020  =0, n=1).       
-00004ad0: 2070 6172 616d 7320 3d20 7b27 6c6f 6728   params = {'log(
-00004ae0: cf83 c2b2 2927 203a 202d 6e70 2e69 6e66  ....)' : -np.inf
-00004af0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00004b00: 2020 2020 276c 6f67 28ce 9329 2720 3a20      'log(..)' : 
-00004b10: 302e 3338 372c 2027 ceb1 2720 3a20 302e  0.387, '..' : 0.
-00004b20: 3839 2c0a 2020 2020 2020 2020 2020 2020  89,.            
-00004b30: 2020 2020 2020 2778 3027 203a 2030 2e35        'x0' : 0.5
-00004b40: 2c20 2779 3127 203a 2031 2c0a 2020 2020  , 'y1' : 1,.    
-00004b50: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00004b60: 2020 2020 2020 2020 666f 7220 6e61 6d65          for name
-00004b70: 2069 6e20 6c69 7374 2870 6172 616d 732e   in list(params.
-00004b80: 6b65 7973 2829 293a 0a20 2020 2020 2020  keys()):.       
-00004b90: 2020 2020 2070 6172 616d 732e 7570 6461       params.upda
-00004ba0: 7465 287b 6622 7b6e 616d 657d 2028 6469  te({f"{name} (di
-00004bb0: 6d20 7b64 696d 7d29 2220 3a20 7061 7261  m {dim})" : para
-00004bc0: 6d73 5b6e 616d 655d 2066 6f72 2064 696d  ms[name] for dim
-00004bd0: 2069 6e20 7261 6e67 6528 6669 742e 6429   in range(fit.d)
-00004be0: 7d29 0a20 2020 2020 2020 2020 2020 2064  }).            d
-00004bf0: 656c 2070 6172 616d 735b 6e61 6d65 5d0a  el params[name].
-00004c00: 2020 2020 2020 2020 6461 7461 5f73 616d          data_sam
-00004c10: 706c 6520 3d20 6261 7965 736d 7364 2e67  ple = bayesmsd.g
-00004c20: 702e 6765 6e65 7261 7465 2828 6669 742c  p.generate((fit,
-00004c30: 2064 6963 7428 7061 7261 6d73 3d70 6172   dict(params=par
-00004c40: 616d 7329 292c 2031 302c 206e 3d32 290a  ams)), 10, n=2).
-00004c50: 0a20 2020 2020 2020 2066 6974 203d 2062  .        fit = b
-00004c60: 6179 6573 6d73 642e 6c69 622e 5477 6f4c  ayesmsd.lib.TwoL
-00004c70: 6f63 7573 526f 7573 6546 6974 2864 6174  ocusRouseFit(dat
-00004c80: 6129 0a20 2020 2020 2020 2070 6172 616d  a).        param
-00004c90: 7320 3d20 7b27 6c6f 6728 cf83 c2b2 2927  s = {'log(....)'
-00004ca0: 203a 202d 6e70 2e69 6e66 2c0a 2020 2020   : -np.inf,.    
-00004cb0: 2020 2020 2020 2020 2020 2020 2020 276c                'l
-00004cc0: 6f67 28ce 9329 2720 3a20 302e 2c0a 2020  og(..)' : 0.,.  
-00004cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ce0: 276c 6f67 284a 2927 203a 2031 2e2c 0a20  'log(J)' : 1.,. 
-00004cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d00: 207d 0a20 2020 2020 2020 2066 6f72 206e   }.        for n
-00004d10: 616d 6520 696e 206c 6973 7428 7061 7261  ame in list(para
-00004d20: 6d73 2e6b 6579 7328 2929 3a0a 2020 2020  ms.keys()):.    
-00004d30: 2020 2020 2020 2020 7061 7261 6d73 2e75          params.u
-00004d40: 7064 6174 6528 7b66 227b 6e61 6d65 7d20  pdate({f"{name} 
-00004d50: 2864 696d 207b 6469 6d7d 2922 203a 2070  (dim {dim})" : p
-00004d60: 6172 616d 735b 6e61 6d65 5d20 666f 7220  arams[name] for 
-00004d70: 6469 6d20 696e 2072 616e 6765 2866 6974  dim in range(fit
-00004d80: 2e64 297d 290a 2020 2020 2020 2020 2020  .d)}).          
-00004d90: 2020 6465 6c20 7061 7261 6d73 5b6e 616d    del params[nam
-00004da0: 655d 0a20 2020 2020 2020 2064 6174 615f  e].        data_
-00004db0: 7361 6d70 6c65 203d 2062 6179 6573 6d73  sample = bayesms
-00004dc0: 642e 6770 2e67 656e 6572 6174 6528 2866  d.gp.generate((f
-00004dd0: 6974 2e4d 5344 2870 6172 616d 7329 2c20  it.MSD(params), 
-00004de0: 302c 2031 292c 2031 302c 206e 3d32 290a  0, 1), 10, n=2).
-00004df0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00004e00: 6572 7445 7175 616c 286c 656e 2864 6174  ertEqual(len(dat
-00004e10: 615f 7361 6d70 6c65 292c 2032 290a 2020  a_sample), 2).  
-00004e20: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00004e30: 7445 7175 616c 286c 656e 2864 6174 615f  tEqual(len(data_
-00004e40: 7361 6d70 6c65 5b30 5d29 2c20 3130 290a  sample[0]), 10).
-00004e50: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00004e60: 6572 7445 7175 616c 2864 6174 615f 7361  ertEqual(data_sa
-00004e70: 6d70 6c65 5b30 5d2e 642c 2031 290a 0a20  mple[0].d, 1).. 
-00004e80: 2020 2020 2020 2064 6174 615f 7361 6d70         data_samp
-00004e90: 6c65 203d 2062 6179 6573 6d73 642e 6770  le = bayesmsd.gp
-00004ea0: 2e67 656e 6572 6174 6528 2866 6974 2e4d  .generate((fit.M
-00004eb0: 5344 2870 6172 616d 7329 2c20 312c 2031  SD(params), 1, 1
-00004ec0: 292c 2031 302c 206e 3d32 290a 0a20 2020  ), 10, n=2)..   
-00004ed0: 2064 6566 2074 6573 745f 6765 6e65 7261   def test_genera
-00004ee0: 7465 5f64 735f 6c69 6b65 2873 656c 6629  te_ds_like(self)
-00004ef0: 3a0a 2020 2020 2020 2020 6461 7461 203d  :.        data =
-00004f00: 206e 6c2e 5461 6767 6564 5365 7428 5b28   nl.TaggedSet([(
-00004f10: 6e6c 2e54 7261 6a65 6374 6f72 7928 5b31  nl.Trajectory([1
-00004f20: 2c20 322c 206e 702e 6e61 6e2c 2034 5d29  , 2, np.nan, 4])
-00004f30: 2c20 7b27 666f 6f27 7d29 2c0a 2020 2020  , {'foo'}),.    
-00004f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f50: 2020 2020 2020 2020 2028 6e6c 2e54 7261           (nl.Tra
-00004f60: 6a65 6374 6f72 7928 5b6e 702e 6e61 6e2c  jectory([np.nan,
-00004f70: 2032 2c20 332c 2034 5d29 2c20 7b27 6261   2, 3, 4]), {'ba
-00004f80: 7227 2c20 2762 617a 277d 295d 290a 0a20  r', 'baz'})]).. 
-00004f90: 2020 2020 2020 2040 6261 7965 736d 7364         @bayesmsd
-00004fa0: 2e64 6563 6f2e 4d53 4466 756e 0a20 2020  .deco.MSDfun.   
-00004fb0: 2020 2020 2064 6566 206d 7364 2864 7429       def msd(dt)
-00004fc0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00004fd0: 7475 726e 2064 740a 0a20 2020 2020 2020  turn dt..       
-00004fe0: 2064 6174 615f 6e65 7720 3d20 6261 7965   data_new = baye
-00004ff0: 736d 7364 2e67 702e 6765 6e65 7261 7465  smsd.gp.generate
-00005000: 5f64 6174 6173 6574 5f6c 696b 6528 6461  _dataset_like(da
-00005010: 7461 2c20 286d 7364 2c20 312c 2031 2929  ta, (msd, 1, 1))
-00005020: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-00005030: 7373 6572 7445 7175 616c 2864 6174 612e  ssertEqual(data.
-00005040: 5f74 6167 735b 305d 2c20 6461 7461 5f6e  _tags[0], data_n
-00005050: 6577 2e5f 7461 6773 5b30 5d29 0a20 2020  ew._tags[0]).   
-00005060: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00005070: 4973 4e6f 7428 6461 7461 2e5f 7461 6773  IsNot(data._tags
-00005080: 5b30 5d2c 2064 6174 615f 6e65 772e 5f74  [0], data_new._t
-00005090: 6167 735b 305d 290a 2020 2020 2020 2020  ags[0]).        
-000050a0: 6461 7461 5f6e 6577 2e5f 7461 6773 5b30  data_new._tags[0
-000050b0: 5d2e 6164 6428 276d 6f6f 2729 0a20 2020  ].add('moo').   
-000050c0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000050d0: 4e6f 7445 7175 616c 2864 6174 612e 5f74  NotEqual(data._t
-000050e0: 6167 735b 305d 2c20 6461 7461 5f6e 6577  ags[0], data_new
-000050f0: 2e5f 7461 6773 5b30 5d29 0a0a 2020 2020  ._tags[0])..    
-00005100: 2020 2020 7365 6c66 2e61 7373 6572 745f      self.assert_
-00005110: 6172 7261 795f 6571 7561 6c28 6e70 2e69  array_equal(np.i
-00005120: 736e 616e 2864 6174 615f 6e65 775b 315d  snan(data_new[1]
-00005130: 5b3a 5d5b 3a2c 2030 5d29 2c0a 2020 2020  [:][:, 0]),.    
-00005140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005150: 2020 2020 2020 2020 2020 2020 6e70 2e61              np.a
-00005160: 7272 6179 285b 5472 7565 2c20 4661 6c73  rray([True, Fals
-00005170: 652c 2046 616c 7365 2c20 4661 6c73 655d  e, False, False]
-00005180: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00005190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051a0: 2020 2029 0a0a 636c 6173 7320 5465 7374     )..class Test
-000051b0: 4e65 7749 6d70 6c65 6d65 6e74 6174 696f  NewImplementatio
-000051c0: 6e28 6d79 5465 7374 4361 7365 293a 0a20  n(myTestCase):. 
-000051d0: 2020 2064 6566 2074 6573 745f 4d53 4466     def test_MSDf
-000051e0: 756e 2873 656c 6629 3a0a 2020 2020 2020  un(self):.      
-000051f0: 2020 4062 6179 6573 6d73 642e 6465 636f    @bayesmsd.deco
-00005200: 2e4d 5344 6675 6e0a 2020 2020 2020 2020  .MSDfun.        
-00005210: 6465 6620 6e6f 6e5f 696d 6167 696e 675f  def non_imaging_
-00005220: 6675 6e28 6172 673d 3529 3a0a 2020 2020  fun(arg=5):.    
-00005230: 2020 2020 2020 2020 7061 7373 2023 2070          pass # p
-00005240: 7261 676d 613a 206e 6f20 636f 7665 720a  ragma: no cover.
-00005250: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00005260: 2073 656c 662e 6173 7365 7274 496e 2827   self.assertIn('
-00005270: 5f6b 7761 7267 7374 7269 6e67 272c 206e  _kwargstring', n
-00005280: 6f6e 5f69 6d61 6769 6e67 5f66 756e 2e5f  on_imaging_fun._
-00005290: 5f64 6963 745f 5f29 0a0a 6966 205f 5f6e  _dict__)..if __n
-000052a0: 616d 655f 5f20 3d3d 2027 5f5f 6d61 696e  ame__ == '__main
-000052b0: 5f5f 273a 2023 2070 7261 676d 613a 206e  __': # pragma: n
-000052c0: 6f20 636f 7665 720a 2020 2020 756e 6974  o cover.    unit
-000052d0: 7465 7374 2e6d 6169 6e28 6d6f 6475 6c65  test.main(module
-000052e0: 3d5f 5f66 696c 655f 5f5b 3a2d 335d 290a  =__file__[:-3]).
+00003fd0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00003fe0: 0a0a 2020 2020 2020 2020 2320 3c73 6f6d  ..        # <som
+00003ff0: 6520 7567 6c79 2068 6163 6b69 6e67 2074  e ugly hacking t
+00004000: 6f20 6765 7420 6120 7573 6572 2d64 6566  o get a user-def
+00004010: 696e 6564 206c 696b 656c 6968 6f6f 6420  ined likelihood 
+00004020: 6675 6e63 7469 6f6e 3e0a 2020 2020 2020  function>.      
+00004030: 2020 6d69 6e5f 7461 7267 6574 203d 2073    min_target = s
+00004040: 656c 662e 6669 742e 4d69 6e54 6172 6765  elf.fit.MinTarge
+00004050: 7428 7365 6c66 2e66 6974 290a 2020 2020  t(self.fit).    
+00004060: 2020 2020 6465 6620 5f6d 696e 5f74 6172      def _min_tar
+00004070: 6765 7428 7365 6c66 2c20 7061 7261 6d73  get(self, params
+00004080: 5f61 7272 6179 293a 0a20 2020 2020 2020  _array):.       
+00004090: 2020 2020 2070 6172 616d 7320 3d20 6d69       params = mi
+000040a0: 6e5f 7461 7267 6574 2e70 6172 616d 735f  n_target.params_
+000040b0: 6172 7261 7932 6469 6374 2870 6172 616d  array2dict(param
+000040c0: 735f 6172 7261 7929 0a20 2020 2020 2020  s_array).       
+000040d0: 2020 2020 2072 6574 7572 6e20 3020 6966       return 0 if
+000040e0: 2070 6172 616d 735b 2779 3027 5d20 3c20   params['y0'] < 
+000040f0: 302e 3733 2065 6c73 6520 3165 3130 0a0a  0.73 else 1e10..
+00004100: 2320 7676 7676 7676 7676 7676 7676 7676  # vvvvvvvvvvvvvv
+00004110: 7676 7676 7676 760a 2020 2020 2020 2020  vvvvvvv.        
+00004120: 4d69 6e54 6172 6765 745f 5f63 616c 6c5f  MinTarget__call_
+00004130: 5f20 3d20 7479 7065 286d 696e 5f74 6172  _ = type(min_tar
+00004140: 6765 7429 2e5f 5f63 616c 6c5f 5f0a 2020  get).__call__.  
+00004150: 2020 2020 2020 7479 7065 286d 696e 5f74        type(min_t
+00004160: 6172 6765 7429 2e5f 5f63 616c 6c5f 5f20  arget).__call__ 
+00004170: 3d20 5f6d 696e 5f74 6172 6765 740a 2320  = _min_target.# 
+00004180: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
+00004190: 5e5e 5e5e 5e0a 0a20 2020 2020 2020 2070  ^^^^^..        p
+000041a0: 726f 6669 6c65 722e 6d69 6e5f 7461 7267  rofiler.min_targ
+000041b0: 6574 5f66 726f 6d5f 6669 7420 3d20 6d69  et_from_fit = mi
+000041c0: 6e5f 7461 7267 6574 0a0a 2020 2020 2020  n_target..      
+000041d0: 2020 6d2c 2072 6f6f 7473 203d 2070 726f    m, roots = pro
+000041e0: 6669 6c65 722e 6669 6e64 5f4d 4349 2822  filer.find_MCI("
+000041f0: 7930 2229 5b22 7930 225d 0a20 2020 2020  y0")["y0"].     
+00004200: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00004210: 7561 6c28 726f 6f74 735b 305d 2c20 3029  ual(roots[0], 0)
+00004220: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00004230: 7365 7274 416c 6d6f 7374 4571 7561 6c28  sertAlmostEqual(
+00004240: 726f 6f74 735b 315d 2c20 302e 3733 290a  roots[1], 0.73).
+00004250: 0a23 2076 7676 7676 7676 7676 7676 7676  .# vvvvvvvvvvvvv
+00004260: 7676 7676 7676 7676 0a20 2020 2020 2020  vvvvvvvv.       
+00004270: 2074 7970 6528 6d69 6e5f 7461 7267 6574   type(min_target
+00004280: 292e 5f5f 6361 6c6c 5f5f 203d 204d 696e  ).__call__ = Min
+00004290: 5461 7267 6574 5f5f 6361 6c6c 5f5f 0a23  Target__call__.#
+000042a0: 205e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e   ^^^^^^^^^^^^^^^
+000042b0: 5e5e 5e5e 5e5e 0a0a 636c 6173 7320 5465  ^^^^^^..class Te
+000042c0: 7374 5261 6e64 6f6d 5374 7566 6628 6d79  stRandomStuff(my
+000042d0: 5465 7374 4361 7365 293a 0a20 2020 2064  TestCase):.    d
+000042e0: 6566 2074 6573 745f 4d53 4428 7365 6c66  ef test_MSD(self
+000042f0: 293a 0a20 2020 2020 2020 2064 6174 6120  ):.        data 
+00004300: 3d20 6e6c 2e54 6167 6765 6453 6574 285b  = nl.TaggedSet([
+00004310: 6e6c 2e54 7261 6a65 6374 6f72 7928 5b5b  nl.Trajectory([[
+00004320: 312c 2032 2c20 335d 2c20 5b34 2c20 352c  1, 2, 3], [4, 5,
+00004330: 2036 5d5d 295d 2c20 6861 7354 6167 733d   6]])], hasTags=
+00004340: 4661 6c73 6529 0a20 2020 2020 2020 2066  False).        f
+00004350: 6974 203d 2062 6179 6573 6d73 642e 6c69  it = bayesmsd.li
+00004360: 622e 4e50 5846 6974 2864 6174 612c 2073  b.NPXFit(data, s
+00004370: 735f 6f72 6465 723d 312c 206e 3d30 290a  s_order=1, n=0).
+00004380: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
+00004390: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
+000043a0: 6c6f 6728 cf83 c2b2 2920 2864 696d 2030  log(....) (dim 0
+000043b0: 2927 203a 202d 6e70 2e69 6e66 2c0a 2020  )' : -np.inf,.  
+000043c0: 2020 2020 2020 2020 2020 2027 6c6f 6728             'log(
+000043d0: ce93 2920 2864 696d 2030 2927 203a 2030  ..) (dim 0)' : 0
+000043e0: 2e33 3837 2c0a 2020 2020 2020 2020 2020  .387,.          
+000043f0: 2020 2020 2020 2020 27ce b120 2864 696d          '.. (dim
+00004400: 2030 2927 203a 2030 2e38 392c 0a20 2020   0)' : 0.89,.   
+00004410: 2020 2020 2020 2020 2027 6c6f 6728 cf83           'log(..
+00004420: c2b2 2920 2864 696d 2031 2927 203a 202d  ..) (dim 1)' : -
+00004430: 6e70 2e69 6e66 2c0a 2020 2020 2020 2020  np.inf,.        
+00004440: 2020 2020 2027 6c6f 6728 ce93 2920 2864       'log(..) (d
+00004450: 696d 2031 2927 203a 2030 2e33 3837 2c0a  im 1)' : 0.387,.
+00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004470: 2020 27ce b120 2864 696d 2031 2927 203a    '.. (dim 1)' :
+00004480: 2030 2e38 392c 0a20 2020 2020 2020 2020   0.89,.         
+00004490: 2020 2027 6c6f 6728 cf83 c2b2 2920 2864     'log(....) (d
+000044a0: 696d 2032 2927 203a 202d 6e70 2e69 6e66  im 2)' : -np.inf
+000044b0: 2c0a 2020 2020 2020 2020 2020 2020 2027  ,.             '
+000044c0: 6c6f 6728 ce93 2920 2864 696d 2032 2927  log(..) (dim 2)'
+000044d0: 203a 2030 2e33 3837 2c0a 2020 2020 2020   : 0.387,.      
+000044e0: 2020 2020 2020 2020 2020 2020 27ce b120              '.. 
+000044f0: 2864 696d 2032 2927 203a 2030 2e38 392c  (dim 2)' : 0.89,
+00004500: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
+00004510: 2020 2020 6d73 6420 3d20 6669 742e 4d53      msd = fit.MS
+00004520: 4428 7061 7261 6d73 290a 2020 2020 2020  D(params).      
+00004530: 2020 646f 6373 7472 696e 6720 3d20 6d73    docstring = ms
+00004540: 642e 5f5f 646f 635f 5f0a 2020 2020 2020  d.__doc__.      
+00004550: 2020 7365 6c66 2e61 7373 6572 7449 6e28    self.assertIn(
+00004560: 6622 2864 742c 222c 2064 6f63 7374 7269  f"(dt,", docstri
+00004570: 6e67 290a 2020 2020 2020 2020 7365 6c66  ng).        self
+00004580: 2e61 7373 6572 7449 6e28 6622 7b70 6172  .assertIn(f"{par
+00004590: 616d 735b 27ce b120 2864 696d 2030 2927  ams['.. (dim 0)'
+000045a0: 5d7d 222c 2064 6f63 7374 7269 6e67 290a  ]}", docstring).
+000045b0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000045c0: 6572 7449 6e28 6622 7b6e 702e 6578 7028  ertIn(f"{np.exp(
+000045d0: 7061 7261 6d73 5b27 6c6f 6728 ce93 2920  params['log(..) 
+000045e0: 2864 696d 2030 2927 5d29 3a2e 3466 7d22  (dim 0)']):.4f}"
+000045f0: 5b3a 2d31 5d2c 2064 6f63 7374 7269 6e67  [:-1], docstring
+00004600: 2920 2320 7072 6576 656e 7420 726f 756e  ) # prevent roun
+00004610: 6469 6e67 2c20 6a75 7374 2074 7275 6e63  ding, just trunc
+00004620: 6174 650a 0a20 2020 2020 2020 2064 7420  ate..        dt 
+00004630: 3d20 6e70 2e61 7261 6e67 6528 312c 2031  = np.arange(1, 1
+00004640: 3029 0a20 2020 2020 2020 206c 6f67 4720  0).        logG 
+00004650: 203d 2070 6172 616d 735b 276c 6f67 28ce   = params['log(.
+00004660: 9329 2028 6469 6d20 3029 275d 0a20 2020  .) (dim 0)'].   
+00004670: 2020 2020 2061 6c70 6861 203d 2070 6172       alpha = par
+00004680: 616d 735b 2020 2020 2027 ceb1 2028 6469  ams[     '.. (di
+00004690: 6d20 3029 275d 0a20 2020 2020 2020 2073  m 0)'].        s
+000046a0: 656c 662e 6173 7365 7274 5f61 7272 6179  elf.assert_array
+000046b0: 5f61 6c6d 6f73 745f 6571 7561 6c28 6d73  _almost_equal(ms
+000046c0: 6428 6474 292c 2064 6174 615b 305d 2e64  d(dt), data[0].d
+000046d0: 2a6e 702e 6578 7028 616c 7068 612a 6e70  *np.exp(alpha*np
+000046e0: 2e6c 6f67 2864 7429 202b 206c 6f67 4729  .log(dt) + logG)
+000046f0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00004700: 7373 6572 745f 6172 7261 795f 616c 6d6f  ssert_array_almo
+00004710: 7374 5f65 7175 616c 286d 7364 2864 7429  st_equal(msd(dt)
+00004720: 2c20 6669 742e 4d53 4428 7061 7261 6d73  , fit.MSD(params
+00004730: 2c20 6474 2929 0a0a 2020 2020 6465 6620  , dt))..    def 
+00004740: 7465 7374 5f67 656e 6572 6174 6528 7365  test_generate(se
+00004750: 6c66 293a 0a20 2020 2020 2020 2064 6174  lf):.        dat
+00004760: 6120 3d20 6e6c 2e54 6167 6765 6453 6574  a = nl.TaggedSet
+00004770: 285b 6e6c 2e54 7261 6a65 6374 6f72 7928  ([nl.Trajectory(
+00004780: 5b5b 312c 2032 2c20 335d 2c20 5b34 2c20  [[1, 2, 3], [4, 
+00004790: 352c 2036 5d5d 295d 2c20 6861 7354 6167  5, 6]])], hasTag
+000047a0: 733d 4661 6c73 6529 0a20 2020 2020 2020  s=False).       
+000047b0: 2066 6974 203d 2062 6179 6573 6d73 642e   fit = bayesmsd.
+000047c0: 6c69 622e 4e50 5846 6974 2864 6174 612c  lib.NPXFit(data,
+000047d0: 2073 735f 6f72 6465 723d 312c 206e 3d30   ss_order=1, n=0
+000047e0: 290a 2020 2020 2020 2020 7061 7261 6d73  ).        params
+000047f0: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+00004800: 2027 6c6f 6728 cf83 c2b2 2920 2864 696d   'log(....) (dim
+00004810: 2030 2927 203a 202d 6e70 2e69 6e66 2c0a   0)' : -np.inf,.
+00004820: 2020 2020 2020 2020 2020 2020 2027 6c6f               'lo
+00004830: 6728 ce93 2920 2864 696d 2030 2927 203a  g(..) (dim 0)' :
+00004840: 2030 2e33 3837 2c0a 2020 2020 2020 2020   0.387,.        
+00004850: 2020 2020 2020 2020 2020 27ce b120 2864            '.. (d
+00004860: 696d 2030 2927 203a 2030 2e38 392c 0a20  im 0)' : 0.89,. 
+00004870: 2020 2020 2020 2020 2020 2027 6c6f 6728             'log(
+00004880: cf83 c2b2 2920 2864 696d 2031 2927 203a  ....) (dim 1)' :
+00004890: 202d 6e70 2e69 6e66 2c0a 2020 2020 2020   -np.inf,.      
+000048a0: 2020 2020 2020 2027 6c6f 6728 ce93 2920         'log(..) 
+000048b0: 2864 696d 2031 2927 203a 2030 2e33 3837  (dim 1)' : 0.387
+000048c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000048d0: 2020 2020 27ce b120 2864 696d 2031 2927      '.. (dim 1)'
+000048e0: 203a 2030 2e38 392c 0a20 2020 2020 2020   : 0.89,.       
+000048f0: 2020 2020 2027 6c6f 6728 cf83 c2b2 2920       'log(....) 
+00004900: 2864 696d 2032 2927 203a 202d 6e70 2e69  (dim 2)' : -np.i
+00004910: 6e66 2c0a 2020 2020 2020 2020 2020 2020  nf,.            
+00004920: 2027 6c6f 6728 ce93 2920 2864 696d 2032   'log(..) (dim 2
+00004930: 2927 203a 2030 2e33 3837 2c0a 2020 2020  )' : 0.387,.    
+00004940: 2020 2020 2020 2020 2020 2020 2020 27ce                '.
+00004950: b120 2864 696d 2032 2927 203a 2030 2e38  . (dim 2)' : 0.8
+00004960: 392c 0a20 2020 2020 2020 207d 0a0a 2020  9,.        }..  
+00004970: 2020 2020 2020 6461 7461 5f73 616d 706c        data_sampl
+00004980: 6520 3d20 6261 7965 736d 7364 2e67 702e  e = bayesmsd.gp.
+00004990: 6765 6e65 7261 7465 2828 6669 742c 2064  generate((fit, d
+000049a0: 6963 7428 7061 7261 6d73 3d70 6172 616d  ict(params=param
+000049b0: 7329 292c 2031 302c 206e 3d32 290a 2020  s)), 10, n=2).  
+000049c0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000049d0: 7445 7175 616c 286c 656e 2864 6174 615f  tEqual(len(data_
+000049e0: 7361 6d70 6c65 292c 2032 290a 2020 2020  sample), 2).    
+000049f0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00004a00: 7175 616c 286c 656e 2864 6174 615f 7361  qual(len(data_sa
+00004a10: 6d70 6c65 5b30 5d29 2c20 3130 290a 2020  mple[0]), 10).  
+00004a20: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00004a30: 7445 7175 616c 2864 6174 615f 7361 6d70  tEqual(data_samp
+00004a40: 6c65 5b30 5d2e 642c 2033 290a 2020 2020  le[0].d, 3).    
+00004a50: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+00004a60: 7275 6528 6e70 2e61 6c6c 286e 702e 6172  rue(np.all(np.ar
+00004a70: 7261 7928 5b74 7261 6a5b 305d 2066 6f72  ray([traj[0] for
+00004a80: 2074 7261 6a20 696e 2064 6174 615f 7361   traj in data_sa
+00004a90: 6d70 6c65 5d29 203d 3d20 3029 290a 0a20  mple]) == 0)).. 
+00004aa0: 2020 2020 2020 2066 6974 203d 2062 6179         fit = bay
+00004ab0: 6573 6d73 642e 6c69 622e 4e50 5846 6974  esmsd.lib.NPXFit
+00004ac0: 2864 6174 612c 2073 735f 6f72 6465 723d  (data, ss_order=
+00004ad0: 302c 206e 3d31 290a 2020 2020 2020 2020  0, n=1).        
+00004ae0: 7061 7261 6d73 203d 207b 276c 6f67 28cf  params = {'log(.
+00004af0: 83c2 b229 2720 3a20 2d6e 702e 696e 662c  ...)' : -np.inf,
+00004b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004b10: 2020 2027 6c6f 6728 ce93 2927 203a 2030     'log(..)' : 0
+00004b20: 2e33 3837 2c20 27ce b127 203a 2030 2e38  .387, '..' : 0.8
+00004b30: 392c 0a20 2020 2020 2020 2020 2020 2020  9,.             
+00004b40: 2020 2020 2027 7830 2720 3a20 302e 352c       'x0' : 0.5,
+00004b50: 2027 7931 2720 3a20 312c 0a20 2020 2020   'y1' : 1,.     
+00004b60: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00004b70: 2020 2020 2020 2066 6f72 206e 616d 6520         for name 
+00004b80: 696e 206c 6973 7428 7061 7261 6d73 2e6b  in list(params.k
+00004b90: 6579 7328 2929 3a0a 2020 2020 2020 2020  eys()):.        
+00004ba0: 2020 2020 7061 7261 6d73 2e75 7064 6174      params.updat
+00004bb0: 6528 7b66 227b 6e61 6d65 7d20 2864 696d  e({f"{name} (dim
+00004bc0: 207b 6469 6d7d 2922 203a 2070 6172 616d   {dim})" : param
+00004bd0: 735b 6e61 6d65 5d20 666f 7220 6469 6d20  s[name] for dim 
+00004be0: 696e 2072 616e 6765 2866 6974 2e64 297d  in range(fit.d)}
+00004bf0: 290a 2020 2020 2020 2020 2020 2020 6465  ).            de
+00004c00: 6c20 7061 7261 6d73 5b6e 616d 655d 0a20  l params[name]. 
+00004c10: 2020 2020 2020 2064 6174 615f 7361 6d70         data_samp
+00004c20: 6c65 203d 2062 6179 6573 6d73 642e 6770  le = bayesmsd.gp
+00004c30: 2e67 656e 6572 6174 6528 2866 6974 2c20  .generate((fit, 
+00004c40: 6469 6374 2870 6172 616d 733d 7061 7261  dict(params=para
+00004c50: 6d73 2929 2c20 3130 2c20 6e3d 3229 0a0a  ms)), 10, n=2)..
+00004c60: 2020 2020 2020 2020 6669 7420 3d20 6261          fit = ba
+00004c70: 7965 736d 7364 2e6c 6962 2e54 776f 4c6f  yesmsd.lib.TwoLo
+00004c80: 6375 7352 6f75 7365 4669 7428 6461 7461  cusRouseFit(data
+00004c90: 290a 2020 2020 2020 2020 7061 7261 6d73  ).        params
+00004ca0: 203d 207b 276c 6f67 28cf 83c2 b229 2720   = {'log(....)' 
+00004cb0: 3a20 2d6e 702e 696e 662c 0a20 2020 2020  : -np.inf,.     
+00004cc0: 2020 2020 2020 2020 2020 2020 2027 6c6f               'lo
+00004cd0: 6728 ce93 2927 203a 2030 2e2c 0a20 2020  g(..)' : 0.,.   
+00004ce0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00004cf0: 6c6f 6728 4a29 2720 3a20 312e 2c0a 2020  log(J)' : 1.,.  
+00004d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d10: 7d0a 2020 2020 2020 2020 666f 7220 6e61  }.        for na
+00004d20: 6d65 2069 6e20 6c69 7374 2870 6172 616d  me in list(param
+00004d30: 732e 6b65 7973 2829 293a 0a20 2020 2020  s.keys()):.     
+00004d40: 2020 2020 2020 2070 6172 616d 732e 7570         params.up
+00004d50: 6461 7465 287b 6622 7b6e 616d 657d 2028  date({f"{name} (
+00004d60: 6469 6d20 7b64 696d 7d29 2220 3a20 7061  dim {dim})" : pa
+00004d70: 7261 6d73 5b6e 616d 655d 2066 6f72 2064  rams[name] for d
+00004d80: 696d 2069 6e20 7261 6e67 6528 6669 742e  im in range(fit.
+00004d90: 6429 7d29 0a20 2020 2020 2020 2020 2020  d)}).           
+00004da0: 2064 656c 2070 6172 616d 735b 6e61 6d65   del params[name
+00004db0: 5d0a 2020 2020 2020 2020 6461 7461 5f73  ].        data_s
+00004dc0: 616d 706c 6520 3d20 6261 7965 736d 7364  ample = bayesmsd
+00004dd0: 2e67 702e 6765 6e65 7261 7465 2828 6669  .gp.generate((fi
+00004de0: 742e 4d53 4428 7061 7261 6d73 292c 2030  t.MSD(params), 0
+00004df0: 2c20 3129 2c20 3130 2c20 6e3d 3229 0a20  , 1), 10, n=2). 
+00004e00: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00004e10: 7274 4571 7561 6c28 6c65 6e28 6461 7461  rtEqual(len(data
+00004e20: 5f73 616d 706c 6529 2c20 3229 0a20 2020  _sample), 2).   
+00004e30: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00004e40: 4571 7561 6c28 6c65 6e28 6461 7461 5f73  Equal(len(data_s
+00004e50: 616d 706c 655b 305d 292c 2031 3029 0a20  ample[0]), 10). 
+00004e60: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00004e70: 7274 4571 7561 6c28 6461 7461 5f73 616d  rtEqual(data_sam
+00004e80: 706c 655b 305d 2e64 2c20 3129 0a0a 2020  ple[0].d, 1)..  
+00004e90: 2020 2020 2020 6461 7461 5f73 616d 706c        data_sampl
+00004ea0: 6520 3d20 6261 7965 736d 7364 2e67 702e  e = bayesmsd.gp.
+00004eb0: 6765 6e65 7261 7465 2828 6669 742e 4d53  generate((fit.MS
+00004ec0: 4428 7061 7261 6d73 292c 2031 2c20 3129  D(params), 1, 1)
+00004ed0: 2c20 3130 2c20 6e3d 3229 0a0a 2020 2020  , 10, n=2)..    
+00004ee0: 6465 6620 7465 7374 5f67 656e 6572 6174  def test_generat
+00004ef0: 655f 6473 5f6c 696b 6528 7365 6c66 293a  e_ds_like(self):
+00004f00: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+00004f10: 6e6c 2e54 6167 6765 6453 6574 285b 286e  nl.TaggedSet([(n
+00004f20: 6c2e 5472 616a 6563 746f 7279 285b 312c  l.Trajectory([1,
+00004f30: 2032 2c20 6e70 2e6e 616e 2c20 345d 292c   2, np.nan, 4]),
+00004f40: 207b 2766 6f6f 277d 292c 0a20 2020 2020   {'foo'}),.     
+00004f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f60: 2020 2020 2020 2020 286e 6c2e 5472 616a          (nl.Traj
+00004f70: 6563 746f 7279 285b 6e70 2e6e 616e 2c20  ectory([np.nan, 
+00004f80: 322c 2033 2c20 345d 292c 207b 2762 6172  2, 3, 4]), {'bar
+00004f90: 272c 2027 6261 7a27 7d29 5d29 0a0a 2020  ', 'baz'})])..  
+00004fa0: 2020 2020 2020 4062 6179 6573 6d73 642e        @bayesmsd.
+00004fb0: 6465 636f 2e4d 5344 6675 6e0a 2020 2020  deco.MSDfun.    
+00004fc0: 2020 2020 6465 6620 6d73 6428 6474 293a      def msd(dt):
+00004fd0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00004fe0: 7572 6e20 6474 0a0a 2020 2020 2020 2020  urn dt..        
+00004ff0: 6461 7461 5f6e 6577 203d 2062 6179 6573  data_new = bayes
+00005000: 6d73 642e 6770 2e67 656e 6572 6174 655f  msd.gp.generate_
+00005010: 6461 7461 7365 745f 6c69 6b65 2864 6174  dataset_like(dat
+00005020: 612c 2028 6d73 642c 2031 2c20 3129 290a  a, (msd, 1, 1)).
+00005030: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00005040: 7365 7274 4571 7561 6c28 6461 7461 2e5f  sertEqual(data._
+00005050: 7461 6773 5b30 5d2c 2064 6174 615f 6e65  tags[0], data_ne
+00005060: 772e 5f74 6167 735b 305d 290a 2020 2020  w._tags[0]).    
+00005070: 2020 2020 7365 6c66 2e61 7373 6572 7449      self.assertI
+00005080: 734e 6f74 2864 6174 612e 5f74 6167 735b  sNot(data._tags[
+00005090: 305d 2c20 6461 7461 5f6e 6577 2e5f 7461  0], data_new._ta
+000050a0: 6773 5b30 5d29 0a20 2020 2020 2020 2064  gs[0]).        d
+000050b0: 6174 615f 6e65 772e 5f74 6167 735b 305d  ata_new._tags[0]
+000050c0: 2e61 6464 2827 6d6f 6f27 290a 2020 2020  .add('moo').    
+000050d0: 2020 2020 7365 6c66 2e61 7373 6572 744e      self.assertN
+000050e0: 6f74 4571 7561 6c28 6461 7461 2e5f 7461  otEqual(data._ta
+000050f0: 6773 5b30 5d2c 2064 6174 615f 6e65 772e  gs[0], data_new.
+00005100: 5f74 6167 735b 305d 290a 0a20 2020 2020  _tags[0])..     
+00005110: 2020 2073 656c 662e 6173 7365 7274 5f61     self.assert_a
+00005120: 7272 6179 5f65 7175 616c 286e 702e 6973  rray_equal(np.is
+00005130: 6e61 6e28 6461 7461 5f6e 6577 5b31 5d5b  nan(data_new[1][
+00005140: 3a5d 5b3a 2c20 305d 292c 0a20 2020 2020  :][:, 0]),.     
+00005150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005160: 2020 2020 2020 2020 2020 206e 702e 6172             np.ar
+00005170: 7261 7928 5b54 7275 652c 2046 616c 7365  ray([True, False
+00005180: 2c20 4661 6c73 652c 2046 616c 7365 5d29  , False, False])
+00005190: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000051a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051b0: 2020 290a 0a63 6c61 7373 2054 6573 744e    )..class TestN
+000051c0: 6577 496d 706c 656d 656e 7461 7469 6f6e  ewImplementation
+000051d0: 286d 7954 6573 7443 6173 6529 3a0a 2020  (myTestCase):.  
+000051e0: 2020 6465 6620 7465 7374 5f4d 5344 6675    def test_MSDfu
+000051f0: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
+00005200: 2040 6261 7965 736d 7364 2e64 6563 6f2e   @bayesmsd.deco.
+00005210: 4d53 4466 756e 0a20 2020 2020 2020 2064  MSDfun.        d
+00005220: 6566 206e 6f6e 5f69 6d61 6769 6e67 5f66  ef non_imaging_f
+00005230: 756e 2861 7267 3d35 293a 0a20 2020 2020  un(arg=5):.     
+00005240: 2020 2020 2020 2070 6173 7320 2320 7072         pass # pr
+00005250: 6167 6d61 3a20 6e6f 2063 6f76 6572 0a20  agma: no cover. 
+00005260: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00005270: 7365 6c66 2e61 7373 6572 7449 6e28 275f  self.assertIn('_
+00005280: 6b77 6172 6773 7472 696e 6727 2c20 6e6f  kwargstring', no
+00005290: 6e5f 696d 6167 696e 675f 6675 6e2e 5f5f  n_imaging_fun.__
+000052a0: 6469 6374 5f5f 290a 0a69 6620 5f5f 6e61  dict__)..if __na
+000052b0: 6d65 5f5f 203d 3d20 275f 5f6d 6169 6e5f  me__ == '__main_
+000052c0: 5f27 3a20 2320 7072 6167 6d61 3a20 6e6f  _': # pragma: no
+000052d0: 2063 6f76 6572 0a20 2020 2075 6e69 7474   cover.    unitt
+000052e0: 6573 742e 6d61 696e 286d 6f64 756c 653d  est.main(module=
+000052f0: 5f5f 6669 6c65 5f5f 5b3a 2d33 5d29 0a    __file__[:-3]).
```

