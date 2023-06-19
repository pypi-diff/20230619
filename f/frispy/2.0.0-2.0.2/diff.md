# Comparing `tmp/frispy-2.0.0.tar.gz` & `tmp/frispy-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frispy-2.0.0.tar", max compression
+gzip compressed data, was "frispy-2.0.2.tar", max compression
```

## Comparing `frispy-2.0.0.tar` & `frispy-2.0.2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1071 2022-11-28 00:04:09.049683 frispy-2.0.0/LICENSE
--rw-r--r--   0        0        0     2606 2022-11-28 00:04:09.049683 frispy-2.0.0/README.rst
--rw-r--r--   0        0        0      140 2022-11-28 00:04:09.049683 frispy-2.0.0/frispy/__init__.py
--rw-r--r--   0        0        0     5039 2022-11-28 00:04:09.049683 frispy-2.0.0/frispy/disc.py
--rw-r--r--   0        0        0     8479 2022-11-28 00:04:09.049683 frispy-2.0.0/frispy/equations_of_motion.py
--rw-r--r--   0        0        0     3499 2022-11-28 00:04:09.049683 frispy-2.0.0/frispy/model.py
--rw-r--r--   0        0        0     1368 2022-11-28 00:04:09.053684 frispy-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3344 1970-01-01 00:00:00.000000 frispy-2.0.0/setup.py
--rw-r--r--   0        0        0     3134 1970-01-01 00:00:00.000000 frispy-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-19 13:56:00.617025 frispy-2.0.2/LICENSE
+-rw-r--r--   0        0        0     2607 2023-06-19 13:56:00.617025 frispy-2.0.2/README.rst
+-rw-r--r--   0        0        0      140 2023-06-19 13:56:00.617025 frispy-2.0.2/frispy/__init__.py
+-rw-r--r--   0        0        0     5111 2023-06-19 13:56:00.617025 frispy-2.0.2/frispy/disc.py
+-rw-r--r--   0        0        0     8479 2023-06-19 13:56:00.617025 frispy-2.0.2/frispy/equations_of_motion.py
+-rw-r--r--   0        0        0     3499 2023-06-19 13:56:00.617025 frispy-2.0.2/frispy/model.py
+-rw-r--r--   0        0        0     1368 2023-06-19 13:56:00.621025 frispy-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3092 1970-01-01 00:00:00.000000 frispy-2.0.2/PKG-INFO
```

### Comparing `frispy-2.0.0/LICENSE` & `frispy-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `frispy-2.0.0/README.rst` & `frispy-2.0.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 for their 2003 Masters thesis for UC Davis.  You can find the document in full
 `on this page <https://morleyfielddgc.files.wordpress.com/2009/04/hummelthesis.pdf>`_.
 
 Installation
 ------------
 
 The easiest way to install this package is with ``pip``. The PyPI package can
-be viewed `here <https://pypi.org/project/frispy/>`_.
+be viewed `here <https://pypi.org/project/frispy/>`_. 
 
 .. code-block:: bash
 
    pip install frispy
 
 
 For developers
```

### Comparing `frispy-2.0.0/frispy/disc.py` & `frispy-2.0.2/frispy/disc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Disc class."""
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Dict, Tuple, Type
 
 import numpy as np
 from scipy.integrate import solve_ivp
 from scipy.optimize import OptimizeResult
 
 from frispy.equations_of_motion import EOM
@@ -59,15 +59,16 @@
     dgamma: float = 62.0  # rad / sec
     area: float = 0.058556  # m ^ 2
     I_xx: float = 0.001219  # kg * m ^ 2
     I_zz: float = 0.002352  # kg * m ^ 2
     mass: float = 0.175  # kg
     air_density: float = 1.225  # kg / m ^ 3
     g: float = 9.81  # m / s ^ 2
-    model: Model = Model()
+    model: Model = field(default_factory=Model)
+    eom: EOM = None
     eom_class: Type = EOM
 
     def compute_trajectory(
         self,
         flight_time: float = 3.0,
         n_times: int = 100,
         **solver_kwargs,
@@ -134,14 +135,16 @@
                 self.dtheta,
                 self.dgamma,
             ],
             t_eval=t_eval,
             **solver_kwargs,
         )
 
+        self.eom = eom
+
         return (
             {
                 "times": result.t,
                 "x": result.y[0],
                 "y": result.y[1],
                 "z": result.y[2],
                 "vx": result.y[3],
```

### Comparing `frispy-2.0.0/frispy/equations_of_motion.py` & `frispy-2.0.2/frispy/equations_of_motion.py`

 * *Files identical despite different names*

### Comparing `frispy-2.0.0/frispy/model.py` & `frispy-2.0.2/frispy/model.py`

 * *Files identical despite different names*

### Comparing `frispy-2.0.0/pyproject.toml` & `frispy-2.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "frispy"
-version = "2.0.0"
+version = "2.0.2"
 description = "Frisbee simulation."
 authors = ["Tom McClintock <thmsmcclintock@gmail.com>"]
 readme = "README.rst"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.23.5"
 scipy = "^1.9.3"
-matplotlib = "^3.6.2"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.10.1"
 black = "^22.10.0"
 flake8 = "^6.0.0"
 pre-commit = "^2.20.0"
 pytest = "^7.2.0"
 coverage = "^6.5.0"
 sphinx-rtd-theme = "^1.1.1"
 sphinx-autoapi = "^2.0.0"
 interrogate = "^1.5.0"
 pydocstyle = "^6.1.1"
+matplotlib = "^3.6.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
```

### Comparing `frispy-2.0.0/PKG-INFO` & `frispy-2.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: frispy
-Version: 2.0.0
+Version: 2.0.2
 Summary: Frisbee simulation.
 Author: Tom McClintock
 Author-email: thmsmcclintock@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
 Description-Content-Type: text/x-rst
 
 .. |TRAVIS| image:: https://github.com/tmcclintock/FrisPy/workflows/Build%20Status/badge.svg?branch=master
 	    :target: https://github.com/tmcclintock/FrisPy/actions
 .. |COVERALLS| image:: https://coveralls.io/repos/github/tmcclintock/FrisPy/badge.svg?branch=master
@@ -44,15 +43,15 @@
 for their 2003 Masters thesis for UC Davis.  You can find the document in full
 `on this page <https://morleyfielddgc.files.wordpress.com/2009/04/hummelthesis.pdf>`_.
 
 Installation
 ------------
 
 The easiest way to install this package is with ``pip``. The PyPI package can
-be viewed `here <https://pypi.org/project/frispy/>`_.
+be viewed `here <https://pypi.org/project/frispy/>`_. 
 
 .. code-block:: bash
 
    pip install frispy
 
 
 For developers
```

