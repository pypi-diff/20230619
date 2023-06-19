# Comparing `tmp/Sella-2.3.1.tar.gz` & `tmp/Sella-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sella-2.3.1.tar", last modified: Thu Jun 15 23:06:39 2023, max compression
+gzip compressed data, was "Sella-2.3.2.tar", last modified: Mon Jun 19 19:22:05 2023, max compression
```

## Comparing `Sella-2.3.1.tar` & `Sella-2.3.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:06:39.955768 Sella-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-06-15 23:06:09.000000 Sella-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-15 23:06:09.000000 Sella-2.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-15 23:06:39.955768 Sella-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-15 23:06:09.000000 Sella-2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:06:39.951768 Sella-2.3.1/Sella.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-15 23:06:39.000000 Sella-2.3.1/Sella.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-15 23:06:39.000000 Sella-2.3.1/Sella.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 23:06:39.000000 Sella-2.3.1/Sella.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 23:06:39.000000 Sella-2.3.1/Sella.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 23:06:39.000000 Sella-2.3.1/Sella.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-15 23:06:09.000000 Sella-2.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 23:06:09.000000 Sella-2.3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:06:39.955768 Sella-2.3.1/sella/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/eigensolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    21272 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/force_match.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/hessian_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    56197 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:06:39.955768 Sella-2.3.1/sella/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/optimize/irc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/optimize/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/optimize/restricted_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/optimize/stepper.py
--rw-r--r--   0 runner    (1001) docker     (123)    20857 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/peswrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/samd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:06:39.955768 Sella-2.3.1/sella/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/utilities/blas.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/utilities/math.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 23:06:39.955768 Sella-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-15 23:06:09.000000 Sella-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:22:05.837957 Sella-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-06-19 19:21:35.000000 Sella-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-19 19:21:35.000000 Sella-2.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-19 19:22:05.837957 Sella-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-19 19:21:35.000000 Sella-2.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:22:05.833957 Sella-2.3.2/Sella.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-19 19:22:05.000000 Sella-2.3.2/Sella.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-19 19:22:05.000000 Sella-2.3.2/Sella.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:22:05.000000 Sella-2.3.2/Sella.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-19 19:22:05.000000 Sella-2.3.2/Sella.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 19:22:05.000000 Sella-2.3.2/Sella.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-19 19:21:35.000000 Sella-2.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-19 19:21:35.000000 Sella-2.3.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:22:05.833957 Sella-2.3.2/sella/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-19 19:21:35.000000 Sella-2.3.2/sella/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-06-19 19:21:35.000000 Sella-2.3.2/sella/eigensolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21272 2023-06-19 19:21:35.000000 Sella-2.3.2/sella/force_match.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-19 19:21:35.000000 Sella-2.3.2/sella/hessian_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56197 2023-06-19 19:21:35.000000 Sella-2.3.2/sella/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-06-19 19:21:35.000000 Sella-2.3.2/sella/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:22:05.837957 Sella-2.3.2/sella/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-19 19:21:35.000000 Sella-2.3.2/sella/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-06-19 19:21:35.000000 Sella-2.3.2/sella/optimize/irc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-06-19 19:21:35.000000 Sella-2.3.2/sella/optimize/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-06-19 19:21:35.000000 Sella-2.3.2/sella/optimize/restricted_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-19 19:21:35.000000 Sella-2.3.2/sella/optimize/stepper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20803 2023-06-19 19:21:35.000000 Sella-2.3.2/sella/peswrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-19 19:21:35.000000 Sella-2.3.2/sella/samd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:22:05.837957 Sella-2.3.2/sella/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 19:21:35.000000 Sella-2.3.2/sella/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-19 19:21:35.000000 Sella-2.3.2/sella/utilities/blas.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-06-19 19:21:35.000000 Sella-2.3.2/sella/utilities/math.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-19 19:22:05.837957 Sella-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-19 19:21:35.000000 Sella-2.3.2/setup.py
```

### Comparing `Sella-2.3.1/LICENSE` & `Sella-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Sella-2.3.1/PKG-INFO` & `Sella-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sella
-Version: 2.3.1
+Version: 2.3.2
 Author: Eric Hermes
 Author-email: ehermes@sandia.gov
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
```

### Comparing `Sella-2.3.1/README.md` & `Sella-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `Sella-2.3.1/Sella.egg-info/PKG-INFO` & `Sella-2.3.2/Sella.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sella
-Version: 2.3.1
+Version: 2.3.2
 Author: Eric Hermes
 Author-email: ehermes@sandia.gov
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
```

### Comparing `Sella-2.3.1/Sella.egg-info/SOURCES.txt` & `Sella-2.3.2/Sella.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Sella-2.3.1/sella/eigensolvers.py` & `Sella-2.3.2/sella/eigensolvers.py`

 * *Files identical despite different names*

### Comparing `Sella-2.3.1/sella/force_match.pyx` & `Sella-2.3.2/sella/force_match.pyx`

 * *Files identical despite different names*

### Comparing `Sella-2.3.1/sella/hessian_update.py` & `Sella-2.3.2/sella/hessian_update.py`

 * *Files identical despite different names*

### Comparing `Sella-2.3.1/sella/internal.py` & `Sella-2.3.2/sella/internal.py`

 * *Files identical despite different names*

### Comparing `Sella-2.3.1/sella/linalg.py` & `Sella-2.3.2/sella/linalg.py`

 * *Files identical despite different names*

### Comparing `Sella-2.3.1/sella/optimize/irc.py` & `Sella-2.3.2/sella/optimize/irc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,52 @@
 import warnings
+from typing import Optional, Union, Dict, Any
 
 import numpy as np
 from scipy.linalg import eigh
 
-from sella.peswrapper import PES
-
+from ase import Atoms
+from ase.io.trajectory import Trajectory, TrajectoryWriter
 from ase.optimize.optimize import Optimizer
+
+from sella.peswrapper import PES
 from .restricted_step import IRCTrustRegion
 from .stepper import QuasiNewtonIRC
 
+
 class IRCInnerLoopConvergenceFailure(RuntimeError):
     pass
 
 
 class IRC(Optimizer):
     def __init__(
         self,
-        atoms,
-        restart=None,
-        logfile='-',
-        trajectory=None,
-        master=None,
-        force_consistent=False,
-        ninner_iter=10,
-        irctol=1e-2,
-        dx=0.1,
-        eta=1e-4,
-        gamma=0.1,
-        peskwargs=None,
+        atoms: Atoms,
+        logfile: str = '-',
+        trajectory: Optional[Union[str, TrajectoryWriter]] = None,
+        master: Optional[bool] = None,
+        force_consistent: bool = False,
+        ninner_iter: int = 10,
+        irctol: float = 1e-2,
+        dx: float = 0.1,
+        eta: float = 1e-4,
+        gamma: float = 0.1,
+        peskwargs: Optional[Dict[str, Any]] = None,
+        keep_going: bool = False,
         **kwargs
     ):
-        Optimizer.__init__(self, atoms, restart, logfile, trajectory, master,
-                           force_consistent)
+        Optimizer.__init__(
+            self,
+            atoms,
+            None,
+            logfile,
+            trajectory,
+            master,
+            force_consistent,
+        )
         self.ninner_iter = ninner_iter
         self.irctol = irctol
         self.dx = dx
         if peskwargs is None:
             self.peskwargs = dict(gamma=gamma)
 
         if 'masses' not in self.atoms.arrays:
@@ -46,43 +57,50 @@
                               "contain the most common isotope masses, so "
                               "Earth-abundance-averaged masses will be used "
                               "instead!")
                 self.atoms.set_masses('defaults')
 
         self.sqrtm = np.repeat(np.sqrt(self.atoms.get_masses()), 3)
 
-        def get_W(self):
-            return np.diag(1. / np.sqrt(np.repeat(self.atoms.get_masses(), 3)))
-
-        PES.get_W = get_W
         self.pes = PES(atoms, eta=eta, proj_trans=False, proj_rot=False,
                        **kwargs)
 
         self.lastrun = None
         self.x0 = self.pes.get_x().copy()
-        self.v0ts = None
-        self.H0 = None
+        self.v0ts: Optional[np.ndarray] = None
+        self.H0: Optional[np.ndarray] = None
         self.peslast = None
         self.xi = 1.
         self.first = True
+        self.keep_going = keep_going
 
-    def irun(self, fmax=0.05, fmax_inner=0.01, steps=None, direction='forward'):
+    def irun(
+        self,
+        fmax: float = 0.05,
+        fmax_inner: float = 0.01,
+        steps: Optional[int] = None,
+        direction: str = 'forward',
+    ):
         if direction not in ['forward', 'reverse']:
             raise ValueError('direction must be one of "forward" or '
                              '"reverse"!')
 
         if self.v0ts is None:
             # Initial diagonalization
             self.pes.kick(0, True, **self.peskwargs)
             self.H0 = self.pes.get_H().asarray().copy()
             Hw = self.H0 / np.outer(self.sqrtm, self.sqrtm)
             _, vecs = eigh(Hw)
             self.v0ts = self.dx * vecs[:, 0] / self.sqrtm
-            if self.v0ts[np.nonzero(self.v0ts)[0][0]] < 0: 
-                self.v0ts *= -1 #force v0ts to be the direction where the first non-zero component is positive
+
+            # force v0ts to be the direction where the first non-zero
+            # component is positive
+            if self.v0ts[np.nonzero(self.v0ts)[0][0]] < 0:
+                self.v0ts *= -1
+
             self.pescurr = self.pes.curr.copy()
             self.peslast = self.pes.last.copy()
         else:
             # Or, restore from last diagonalization for new direction
             self.pes.set_x(self.x0)
             self.pes.curr = self.pescurr.copy()
             self.pes.last = self.peslast.copy()
@@ -93,51 +111,63 @@
         elif direction == 'reverse':
             self.d1 = -self.v0ts.copy()
 
         self.first = True
         self.fmax_inner = min(fmax, fmax_inner)
         return Optimizer.irun(self, fmax, steps)
 
-    def run(self, fmax=0.05, fmax_inner=0.01, steps=None, direction='forward'):
-        for converged in self.irun(fmax, fmax_inner, steps, direction):
+    def run(self, *args, **kwargs):
+        for converged in self.irun(*args, **kwargs):
             pass
         return converged
 
     def step(self):
-        x0 = self.pes.get_x()
         if self.first:
             self.pes.kick(self.d1)
             self.first = False
         for n in range(self.ninner_iter):
             s, smag = IRCTrustRegion(
-                self.pes, 0, self.dx, method=QuasiNewtonIRC, sqrtm=self.sqrtm,
-                d1=self.d1
+                self.pes,
+                0,
+                self.dx,
+                method=QuasiNewtonIRC,
+                sqrtm=self.sqrtm,
+                d1=self.d1,
+                W=self.get_W(),
             ).get_s()
 
             bound_clip = abs(smag - self.dx) < 1e-8
             self.d1 += s
 
             self.pes.kick(s)
             g1 = self.pes.get_g()
 
             d1m = self.d1 * self.sqrtm
             d1m /= np.linalg.norm(d1m)
             g1m = g1 / self.sqrtm
 
             g1m_proj = g1m - d1m * (d1m @ g1m)
-            fmax = np.linalg.norm((g1m_proj * self.sqrtm).reshape((-1, 3)), axis=1).max()
+            fmax = np.linalg.norm(
+                (g1m_proj * self.sqrtm).reshape((-1, 3)), axis=1
+            ).max()
 
             g1m /= np.linalg.norm(g1m)
-            dot = np.abs(d1m @ g1m)
-            snorm = np.linalg.norm(s)
-            #print(bound_clip, snorm, dot, fmax)
             if bound_clip and fmax < self.fmax_inner:
                 break
             elif self.converged():
                 break
         else:
-            raise IRCInnerLoopConvergenceFailure
+            if self.keep_going:
+                warnings.warn(
+                    'IRC inner loop failed to converge! The trajectory is no '
+                    'longer a trustworthy IRC.'
+                )
+            else:
+                raise IRCInnerLoopConvergenceFailure
 
         self.d1 *= 0.
 
     def converged(self, forces=None):
         return self.pes.converged(self.fmax)[0] and self.pes.H.evals[0] > 0
+
+    def get_W(self):
+        return np.diag(1. / np.sqrt(np.repeat(self.atoms.get_masses(), 3)))
```

### Comparing `Sella-2.3.1/sella/optimize/optimize.py` & `Sella-2.3.2/sella/optimize/optimize.py`

 * *Files identical despite different names*

### Comparing `Sella-2.3.1/sella/optimize/restricted_step.py` & `Sella-2.3.2/sella/optimize/restricted_step.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,39 @@
+from typing import Optional, Union, List
+
 import numpy as np
 import inspect
 
+from sella.peswrapper import PES, InternalPES
 from .stepper import get_stepper, BaseStepper, NaiveStepper
 
 
 # Classes for restricted step (e.g. trust radius, max atom displacement, etc)
 class BaseRestrictedStep:
-    synonyms = None
+    synonyms: List[str] = []
 
-    def __init__(self, pes, order, delta, method='qn',
-                 tol=1e-15, maxiter=1000, d1=None):
+    def __init__(
+        self,
+        pes: Union[PES, InternalPES],
+        order: int,
+        delta: float,
+        method: str = 'qn',
+        tol: float = 1e-15,
+        maxiter: int = 1000,
+        d1: Optional[np.ndarray] = None,
+        W: Optional[np.ndarray] = None,
+    ):
         self.pes = pes
         self.delta = delta
         self.d1 = d1
         g0 = self.pes.get_g()
 
+        if W is None:
+            W = np.eye(len(g0))
+
         self.scons = self.pes.get_scons()
         # TODO: Should this be HL instead of H?
         g = g0 + self.pes.get_H() @ self.scons
 
         if inspect.isclass(method) and issubclass(method, BaseStepper):
             stepper = method
         else:
@@ -26,21 +41,24 @@
 
         if self.cons(self.scons) - self.delta > 1e-8:
             self.P = self.pes.get_Unred().T
             dx = self.P @ self.scons
             self.stepper = NaiveStepper(dx)
             self.scons[:] *= 0
         else:
-            self.P = self.pes.get_Ufree().T @ self.pes.get_W()
+            self.P = self.pes.get_Ufree().T @ W
             d1 = self.d1
             if d1 is not None:
                 d1 = np.linalg.lstsq(self.P.T, d1, rcond=None)[0]
-            self.stepper = stepper(self.P @ g,
-                                   self.pes.get_HL().project(self.P.T),
-                                   order, d1=d1)
+            self.stepper = stepper(
+                self.P @ g,
+                self.pes.get_HL().project(self.P.T),
+                order,
+                d1=d1,
+            )
 
         self.tol = tol
         self.maxiter = maxiter
 
     def cons(self, s, dsda=None):
         raise NotImplementedError
 
@@ -94,16 +112,21 @@
 
     @classmethod
     def match(cls, name):
         return name in cls.synonyms
 
 
 class TrustRegion(BaseRestrictedStep):
-    synonyms = ['tr', 'trust region', 'trust-region', 'trust radius',
-                'trust-radius']
+    synonyms = [
+        'tr',
+        'trust region',
+        'trust-region',
+        'trust radius',
+        'trust-radius',
+    ]
 
     def cons(self, s, dsda=None):
         val = np.linalg.norm(s)
         if dsda is None:
             return val
 
         dval = dsda @ s / val
@@ -127,17 +150,18 @@
 
 
 class RestrictedAtomicStep(BaseRestrictedStep):
     synonyms = ['ras', 'restricted atomic step']
 
     def __init__(self, pes, *args, **kwargs):
         if pes.int is not None:
-            raise ValueError("Internal coordinates are not compatible with "
-                             "the {} trust region method."
-                             .format(self.__class__.__name__))
+            raise ValueError(
+                "Internal coordinates are not compatible with "
+                f"the {self.__class__.__name__} trust region method."
+            )
         BaseRestrictedStep.__init__(self, pes, *args, **kwargs)
 
     def cons(self, s, dsda=None):
         s_mat = s.reshape((-1, 3))
         s_norms = np.linalg.norm(s_mat, axis=1)
         index = np.argmax(s_norms)
         val = s_norms[index]
@@ -153,17 +177,18 @@
 class MaxInternalStep(BaseRestrictedStep):
     synonyms = ['mis', 'max internal step']
 
     def __init__(
         self, pes, *args, wx=1., wb=1., wa=1., wd=1., wo=1., **kwargs
     ):
         if pes.int is None:
-            raise ValueError("Internal coordinates are required for the "
-                             "{} trust region method"
-                             .format(self.__class__.__name__))
+            raise ValueError(
+                "Internal coordinates are required for the "
+                "{self.__class__.__name__} trust region method"
+            )
         self.wx = wx
         self.wb = wb
         self.wa = wa
         self.wd = wd
         self.wo = wo
         BaseRestrictedStep.__init__(self, pes, *args, **kwargs)
```

### Comparing `Sella-2.3.1/sella/optimize/stepper.py` & `Sella-2.3.2/sella/optimize/stepper.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,106 +1,126 @@
+from typing import Optional, Tuple, Type, List
+
 import numpy as np
 from scipy.linalg import eigh
 
+from sella.linalg import ApproximateHessian
+
 
 # Classes for optimization algorithms (e.g. MMF, Newton, RFO)
 class BaseStepper:
-    alpha0 = None
-    alphamin = None
-    alphamax = None
+    alpha0: Optional[float] = None
+    alphamin: Optional[float] = None
+    alphamax: Optional[float] = None
     # Whether the step size increases or decreases with increasing alpha
-    slope = None
-    synonyms = None
+    slope: Optional[float] = None
+    synonyms: List[str] = []
 
-    def __init__(self, g, H, order=0, d1=None):
+    def __init__(
+        self,
+        g: np.ndarray,
+        H: ApproximateHessian,
+        order: int = 0,
+        d1: Optional[np.ndarray] = None,
+    ) -> None:
         self.g = g
         self.H = H
         self.order = order
         self.d1 = d1
         self._stepper_init()
 
     @classmethod
-    def match(cls, name):
+    def match(cls, name: str) -> bool:
         return name in cls.synonyms
 
-    def _stepper_init(self):
+    def _stepper_init(self) -> None:
         raise NotImplementedError  # pragma: no cover
 
-    def get_s(self, alpha):
+    def get_s(self, alpha: float) -> Tuple[np.ndarray, np.ndarray]:
         raise NotImplementedError  # pragma: no cover
 
 
 class NaiveStepper(BaseStepper):
     synonyms = []  # No synonyms, we don't want someone using this accidentally
     alpha0 = 0.5
     alphamin = 0.
     alphamax = 1.
     slope = 1.
 
-    def __init__(self, dx):
+    def __init__(self, dx: np.ndarray) -> None:
         self.dx = dx
 
-    def get_s(self, alpha):
+    def get_s(self, alpha: float) -> Tuple[np.ndarray, np.ndarray]:
         return alpha * self.dx, self.dx
 
 
 class QuasiNewton(BaseStepper):
     alpha0 = 0.
     alphamin = 0.
     alphamax = np.infty
     slope = -1
-    synonyms = ['qn', 'quasi-newton', 'quasi newton', 'quasi-newton',
-                'newton', 'mmf', 'minimum mode following',
-                'minimum-mode following', 'dimer']
+    synonyms = [
+        'qn',
+        'quasi-newton',
+        'quasi newton',
+        'quasi-newton',
+        'newton',
+        'mmf',
+        'minimum mode following',
+        'minimum-mode following',
+        'dimer',
+    ]
 
-    def _stepper_init(self):
+    def _stepper_init(self) -> None:
         self.L = np.abs(self.H.evals)
         self.L[:self.order] *= -1
 
         self.V = self.H.evecs
         self.Vg = self.V.T @ self.g
 
         self.ones = np.ones_like(self.L)
         self.ones[:self.order] = -1
 
-    def get_s(self, alpha):
+    def get_s(self, alpha: float) -> Tuple[np.ndarray, np.ndarray]:
         denom = self.L + alpha * self.ones
         sproj = self.Vg / denom
         s = -self.V @ sproj
         dsda = self.V @ (sproj / denom)
         return s, dsda
 
 
 class QuasiNewtonIRC(QuasiNewton):
     synonyms = []
 
-    def _stepper_init(self):
+    def _stepper_init(self) -> None:
         QuasiNewton._stepper_init(self)
         self.Vd1 = self.V.T @ self.d1
 
-    def get_s(self, alpha):
+    def get_s(self, alpha: float) -> Tuple[np.ndarray, np.ndarray]:
         denom = np.abs(self.L) + alpha
         sproj = -(self.Vg + alpha * self.Vd1) / denom
         s = self.V @ sproj
         dsda = -self.V @ ((sproj + self.Vd1) / denom)
         return s, dsda
 
 
 class RationalFunctionOptimization(BaseStepper):
     alpha0 = 1.
     alphamin = 0.
     alphamax = 1.
     slope = 1.
     synonyms = ['rfo', 'rational function optimization']
 
-    def _stepper_init(self):
-        self.A = np.block([[self.H.asarray(), self.g[:, np.newaxis]],
-                           [self.g, 0]])
+    def _stepper_init(self) -> None:
+        self.A = np.block([
+            [self.H.asarray(), self.g[:, np.newaxis]],
+            [self.g, 0]
+        ])
 
-    def get_s(self, alpha):
+    def get_s(self, alpha: float) -> Tuple[np.ndarray, np.ndarray]:
         A = self.A * alpha
         A[:-1, :-1] *= alpha
         L, V = eigh(A)
         s = V[:-1, self.order] * alpha / V[-1, self.order]
 
         dAda = self.A.copy()
         dAda[:-1, :-1] *= 2 * alpha
@@ -116,37 +136,44 @@
                    / V[-1, self.order]**2) * dVda[-1])
         return s, dsda
 
 
 class PartitionedRationalFunctionOptimization(RationalFunctionOptimization):
     synonyms = ['prfo', 'p-rfo', 'partitioned rational function optimization']
 
-    def _stepper_init(self):
+    def _stepper_init(self) -> None:
         self.Vmax = self.H.evecs[:, :self.order]
         self.Vmin = self.H.evecs[:, self.order:]
 
-        self.max = RationalFunctionOptimization(self.Vmax.T @ self.g,
-                                                self.H.project(self.Vmax),
-                                                order=self.Vmax.shape[1])
-
-        self.min = RationalFunctionOptimization(self.Vmin.T @ self.g,
-                                                self.H.project(self.Vmin),
-                                                order=0)
+        self.max = RationalFunctionOptimization(
+            self.Vmax.T @ self.g,
+            self.H.project(self.Vmax),
+            order=self.Vmax.shape[1],
+        )
+
+        self.min = RationalFunctionOptimization(
+            self.Vmin.T @ self.g,
+            self.H.project(self.Vmin),
+            order=0,
+        )
 
-    def get_s(self, alpha):
+    def get_s(self, alpha: float) -> Tuple[np.ndarray, np.ndarray]:
         smax, dsmaxda = self.max.get_s(alpha)
         smin, dsminda = self.min.get_s(alpha)
 
         s = self.Vmax @ smax + self.Vmin @ smin
         dsda = self.Vmax @ dsmaxda + self.Vmin @ dsminda
         return s, dsda
 
 
-_all_steppers = [QuasiNewton, RationalFunctionOptimization,
-                 PartitionedRationalFunctionOptimization]
+_all_steppers = [
+    QuasiNewton,
+    RationalFunctionOptimization,
+    PartitionedRationalFunctionOptimization,
+]
 
 
-def get_stepper(name):
+def get_stepper(name: str) -> Type[BaseStepper]:
     for stepper in _all_steppers:
         if stepper.match(name):
             return stepper
     raise ValueError("Unknown stepper name: {}".format(name))
```

### Comparing `Sella-2.3.1/sella/peswrapper.py` & `Sella-2.3.2/sella/peswrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,17 +296,14 @@
 
     def converged(self, fmax, cmax=1e-5):
         fmax1 = np.linalg.norm(self.get_projected_forces(), axis=1).max()
         cmax1 = np.linalg.norm(self.get_res())
         conv = (fmax1 < fmax) and (cmax1 < cmax)
         return conv, fmax1, cmax1
 
-    def get_W(self):
-        return np.eye(self.dim)
-
     def wrap_dx(self, dx):
         return dx
 
     def get_df_pred(self, dx, g, H):
         if H is None:
             return None
         return g.T @ dx + (dx.T @ H @ dx) / 2.
```

### Comparing `Sella-2.3.1/sella/samd.py` & `Sella-2.3.2/sella/samd.py`

 * *Files identical despite different names*

### Comparing `Sella-2.3.1/sella/utilities/blas.pyx` & `Sella-2.3.2/sella/utilities/blas.pyx`

 * *Files identical despite different names*

### Comparing `Sella-2.3.1/sella/utilities/math.pyx` & `Sella-2.3.2/sella/utilities/math.pyx`

 * *Files identical despite different names*

### Comparing `Sella-2.3.1/setup.py` & `Sella-2.3.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import os
 
 import numpy as np
 
 from setuptools import setup, Extension, find_packages
 
-VERSION = '2.3.1'
+VERSION = '2.3.2'
 
 debug = '--debug' in sys.argv or '-g' in sys.argv
 
 try:
     from Cython.Build import cythonize
 except ImportError:
     use_cython = False
```

