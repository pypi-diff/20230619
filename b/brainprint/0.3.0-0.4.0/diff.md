# Comparing `tmp/brainprint-0.3.0.tar.gz` & `tmp/brainprint-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainprint-0.3.0.tar", last modified: Wed May 17 16:30:48 2023, max compression
+gzip compressed data, was "brainprint-0.4.0.tar", last modified: Mon Jun 19 18:30:28 2023, max compression
```

## Comparing `brainprint-0.3.0.tar` & `brainprint-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:30:48.413168 brainprint-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-17 16:29:54.000000 brainprint-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-05-17 16:30:48.413168 brainprint-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-17 16:29:54.000000 brainprint-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:30:48.409168 brainprint-0.3.0/brainprint/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-17 16:29:54.000000 brainprint-0.3.0/brainprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-17 16:29:54.000000 brainprint-0.3.0/brainprint/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-17 16:29:54.000000 brainprint-0.3.0/brainprint/asymmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-05-17 16:29:54.000000 brainprint-0.3.0/brainprint/brainprint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:30:48.409168 brainprint-0.3.0/brainprint/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-17 16:29:54.000000 brainprint-0.3.0/brainprint/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-05-17 16:29:54.000000 brainprint-0.3.0/brainprint/cli/help_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-17 16:29:54.000000 brainprint-0.3.0/brainprint/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-17 16:29:54.000000 brainprint-0.3.0/brainprint/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:30:48.409168 brainprint-0.3.0/brainprint/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:29:54.000000 brainprint-0.3.0/brainprint/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-17 16:29:54.000000 brainprint-0.3.0/brainprint/commands/sys_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-17 16:29:54.000000 brainprint-0.3.0/brainprint/surfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:30:48.413168 brainprint-0.3.0/brainprint/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-17 16:29:54.000000 brainprint-0.3.0/brainprint/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-17 16:29:54.000000 brainprint-0.3.0/brainprint/utils/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-05-17 16:29:54.000000 brainprint-0.3.0/brainprint/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:30:48.409168 brainprint-0.3.0/brainprint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-05-17 16:30:48.000000 brainprint-0.3.0/brainprint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-17 16:30:48.000000 brainprint-0.3.0/brainprint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:30:48.000000 brainprint-0.3.0/brainprint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-17 16:30:48.000000 brainprint-0.3.0/brainprint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-17 16:30:48.000000 brainprint-0.3.0/brainprint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 16:30:48.000000 brainprint-0.3.0/brainprint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-17 16:29:54.000000 brainprint-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 16:30:48.413168 brainprint-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 16:29:54.000000 brainprint-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:30:28.781467 brainprint-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-19 18:29:45.000000 brainprint-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-06-19 18:30:28.781467 brainprint-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-06-19 18:29:45.000000 brainprint-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:30:28.781467 brainprint-0.4.0/brainprint/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-19 18:29:45.000000 brainprint-0.4.0/brainprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-19 18:29:45.000000 brainprint-0.4.0/brainprint/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-06-19 18:29:45.000000 brainprint-0.4.0/brainprint/asymmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-06-19 18:29:45.000000 brainprint-0.4.0/brainprint/brainprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:30:28.781467 brainprint-0.4.0/brainprint/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-19 18:29:45.000000 brainprint-0.4.0/brainprint/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-06-19 18:29:45.000000 brainprint-0.4.0/brainprint/cli/help_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-19 18:29:45.000000 brainprint-0.4.0/brainprint/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-19 18:29:45.000000 brainprint-0.4.0/brainprint/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:30:28.781467 brainprint-0.4.0/brainprint/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 18:29:45.000000 brainprint-0.4.0/brainprint/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-19 18:29:45.000000 brainprint-0.4.0/brainprint/commands/sys_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-06-19 18:29:45.000000 brainprint-0.4.0/brainprint/surfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:30:28.781467 brainprint-0.4.0/brainprint/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-19 18:29:45.000000 brainprint-0.4.0/brainprint/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-19 18:29:45.000000 brainprint-0.4.0/brainprint/utils/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-06-19 18:29:45.000000 brainprint-0.4.0/brainprint/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:30:28.781467 brainprint-0.4.0/brainprint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-06-19 18:30:28.000000 brainprint-0.4.0/brainprint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-19 18:30:28.000000 brainprint-0.4.0/brainprint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 18:30:28.000000 brainprint-0.4.0/brainprint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-19 18:30:28.000000 brainprint-0.4.0/brainprint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-19 18:30:28.000000 brainprint-0.4.0/brainprint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-19 18:30:28.000000 brainprint-0.4.0/brainprint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-06-19 18:29:45.000000 brainprint-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 18:30:28.781467 brainprint-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 18:29:45.000000 brainprint-0.4.0/setup.py
```

### Comparing `brainprint-0.3.0/LICENSE` & `brainprint-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brainprint-0.3.0/PKG-INFO` & `brainprint-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainprint
-Version: 0.3.0
+Version: 0.4.0
 Summary: A package to compute BrainPrint (shape descriptors) from FastSurfer/FreeSurfer MRI segmentations
 Author-email: Martin Reuter <martin.reuter@dzne.de>, Kersten Diers <kersten.diers@dzne.de>
 Maintainer-email: Martin Reuter <martin.reuter@dzne.de>
 License: MIT License
         
         Copyright (c) 2019 Image Analysis, DZNE e.V.
         
@@ -38,23 +38,24 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.4
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: style
 Provides-Extra: test
 Provides-Extra: all
 Provides-Extra: full
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/brainprint.svg)](https://pypi.org/project/brainprint/)
 # BrainPrint
 
 This is the `brainprint` python package, a derivative of the original
 [BrainPrint-legacy](https://github.com/Deep-MI/BrainPrint-legacy) scripts,
 with the primary goal to provide a Python-only version, to integrate the
 [LaPy](https://github.com/Deep-MI/LaPy) package, and to remove dependencies
 on third-party software (shapeDNA-* binaries, gmsh, meshfix). As a result,
```

### Comparing `brainprint-0.3.0/README.md` & `brainprint-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+[![PyPI version](https://badge.fury.io/py/brainprint.svg)](https://pypi.org/project/brainprint/)
 # BrainPrint
 
 This is the `brainprint` python package, a derivative of the original
 [BrainPrint-legacy](https://github.com/Deep-MI/BrainPrint-legacy) scripts,
 with the primary goal to provide a Python-only version, to integrate the
 [LaPy](https://github.com/Deep-MI/LaPy) package, and to remove dependencies
 on third-party software (shapeDNA-* binaries, gmsh, meshfix). As a result,
```

### Comparing `brainprint-0.3.0/brainprint/asymmetry.py` & `brainprint-0.4.0/brainprint/asymmetry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Contains asymmetry estimation functionality.
 """
 from typing import Dict
 
 import numpy as np
-from lapy import ShapeDNA
+from lapy import shapedna
 
 
 def compute_asymmetry(
     eigenvalues, distance: str = "euc", skip_cortex: bool = False
 ) -> Dict[str, float]:
     """
     Computes lateral shape distances from BrainPrint analysis results.
@@ -70,19 +70,22 @@
         left_eigenvalues, right_eigenvalues = (
             eigenvalues[left_label][2:],
             eigenvalues[right_label][2:],
         )
         has_nan = np.isnan(left_eigenvalues).any() or np.isnan(right_eigenvalues).any()
         key = f"{left_label}_{right_label}"
         if has_nan:
-            message = "NaNs found for {left_label} or {right_label}, skipping asymmetry computation...".format(
-                left_label=left_label, right_label=right_label
+            message = (
+                "NaNs found for {left_label} or {right_label}, "
+                "skipping asymmetry computation...".format(
+                    left_label=left_label, right_label=right_label
+                )
             )
             print(message)
             distances[key] = np.nan
         else:
-            distances[key] = ShapeDNA.compute_distance(
+            distances[key] = shapedna.compute_distance(
                 left_eigenvalues,
                 right_eigenvalues,
                 dist=distance,
             )
     return distances
```

### Comparing `brainprint-0.3.0/brainprint/brainprint.py` & `brainprint-0.4.0/brainprint/brainprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 Definition of the brainprint analysis execution functions.
 """
+
 import shutil
 import warnings
 from pathlib import Path
 from typing import Dict, Tuple, Union
 
 import numpy as np
-from lapy import ShapeDNA, TriaMesh
+from lapy import TriaMesh, shapedna
 
 from . import __version__
 from .asymmetry import compute_asymmetry
 from .surfaces import create_surfaces, read_vtk
 from .utils.utils import (
     create_output_paths,
     export_brainprint_results,
@@ -48,21 +49,21 @@
     -------
     np.ndarray
         Fixed eigenvalues
     """
     if not triangular_mesh.is_oriented():
         triangular_mesh.orient_()
     if norm != "none":
-        eigenvalues = ShapeDNA.normalize_ev(
+        eigenvalues = shapedna.normalize_ev(
             geom=triangular_mesh,
             evals=eigenvalues,
             method=norm,
         )
     if reweight:
-        eigenvalues = ShapeDNA.reweight_ev(eigenvalues)
+        eigenvalues = shapedna.reweight_ev(eigenvalues)
     return eigenvalues
 
 
 def compute_surface_brainprint(
     path: Path,
     return_eigenvectors: bool = True,
     num: int = 50,
@@ -93,16 +94,21 @@
 
     Returns
     -------
     Tuple[np.ndarray, Union[np.ndarray, None]]
         Eigenvalues, eigenvectors (if returned)
     """
     triangular_mesh = read_vtk(path)
-    shape_dna = ShapeDNA.compute_shapedna(
-        triangular_mesh, k=num, lump=False, aniso=None, aniso_smooth=10, use_cholmod=use_cholmod
+    shape_dna = shapedna.compute_shapedna(
+        triangular_mesh,
+        k=num,
+        lump=False,
+        aniso=None,
+        aniso_smooth=10,
+        use_cholmod=use_cholmod,
     )
 
     eigenvectors = None
     if return_eigenvectors:
         eigenvectors = shape_dna["Eigenvectors"]
 
     eigenvalues = shape_dna["Eigenvalues"]
@@ -153,25 +159,29 @@
         Surface label to eigenvalues, surface label to eigenvectors (if
         *keep_eigenvectors* is True)
     """
     eigenvalues = dict()
     eigenvectors = dict() if keep_eigenvectors else None
     for surface_label, surface_path in surfaces.items():
         try:
-            (surface_eigenvalues, surface_eigenvectors,) = compute_surface_brainprint(
+            (
+                surface_eigenvalues,
+                surface_eigenvectors,
+            ) = compute_surface_brainprint(
                 surface_path,
                 num=num,
                 norm=norm,
                 reweight=reweight,
                 return_eigenvectors=keep_eigenvectors,
                 use_cholmod=use_cholmod,
             )
         except Exception as e:
-            message = "BrainPrint analysis raised the following exception:\n{exception}".format(
-                exception=e
+            message = (
+                "BrainPrint analysis raised the following exception:\n"
+                "{exception}".format(exception=e)
             )
             warnings.warn(message)
             eigenvalues[surface_label] = ["NaN"] * (num + 2)
         else:
             if len(surface_eigenvalues) == 0:
                 eigenvalues[surface_label] = ["NaN"] * (num + 2)
             else:
@@ -313,20 +323,20 @@
         asymmetry : bool, optional
             Whether to calculate asymmetry between lateral structures, by
             default False
         asymmetry_distance : str, optional
             Distance measurement to use if *asymmetry* is set to True, by
             default "euc"
         keep_temp : bool, optional
-            Whether to keep the temporary files directory or not, by default
-            False
+            Whether to keep the temporary files directory or not, by default False
         use_cholmod : bool, optional
             If True, attempts to use the Cholesky decomposition for improved execution
-            speed. Requires the ``scikit-sparse`` library. If it can not be found, an error
-            will be thrown. If False, will use slower LU decomposition. This is the default.
+            speed. Requires the ``scikit-sparse`` library. If it can not be found, an
+            error will be thrown. If False, will use slower LU decomposition. This is
+            the default.
         """
         self.subjects_dir = subjects_dir
         self.num = num
         self.norm = norm
         self.skip_cortex = skip_cortex
         self.reweight = reweight
         self.keep_eigenvectors = keep_eigenvectors
```

### Comparing `brainprint-0.3.0/brainprint/cli/help_text.py` & `brainprint-0.4.0/brainprint/cli/help_text.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 SKIP_CORTEX: str = "Skip cortical surfaces (default: off)"
 NORM: str = "Eigenvalues normalization method (default: none)"
 REWEIGHT: str = "Switch on eigenvalue reweighting (default: off)"
 ASYM: str = "Switch on additional asymmetry calculation (default: off)"
 ASYM_DISTANCE: str = (
     "Distance measurement to use for asymmetry calculation (default: euc)"
 )
-CHOLMOD: str = (
-    "Use cholesky decomposition (faster) instead of LU decompostion (slower). May require manual install of scikit-sparse library. Default is LU decomposition."
-)
+CHOLMOD: str = "Use cholesky decomposition (faster) instead of LU decomposition (slower). May require manual install of scikit-sparse library. Default is LU decomposition."
 KEEP_TEMP: str = (
     "Whether to keep the temporary files directory or not, by default False"
 )
 HELP: str = "Display this help message and exit"
 MORE_HELP: str = "Display extensive help message and exit"
 
 HELPTEXT: str = """
@@ -125,15 +123,15 @@
     --norm <surface|volume|geometry|none>
                      Switch on eigenvalue normalization; will be either surface,
                      volume, or determined by the geometry of the object. Use
                      "none" or leave out entirely to skip normalization.
     --reweight       Switch on eigenvalue reweighting (default: off)
     --asymmetry      Perform left-right asymmetry calculation (default: off)
     --cholmod        Use cholesky decomposition (faster) instead of LU 
-                     decompostion (slower). May require manual install of the
+                     decomposition (slower). May require manual install of the
                      scikit-sparse library. Default is LU decomposition.
 
 Output parameters:
     --outdir=OUTDIR  Output directory (default: <sdir>/<sid>/brainprint)
 
 ============
 PYTHON USAGE
@@ -145,29 +143,21 @@
 import lapy
 from brainprint import brainprint
 brainprint.run_brainprint(subjects_dir="/my/subjects/directory", subject_id="my_subject_id")
 
 Additional options are num=<int>, evec=<bool>, skipcortex=<bool>,
 norm=<"surface"|"volume"|"geometry"|"none">, reweight=<bool>, and outdir=<string>.
 
-=============
-REQUIREMENTS
-============
-
-The script requires the lapy package, which can be installed from
-https://github.com/Deep-MI/LaPy using
-pip3 install --user git+https://github.com/Deep-MI/LaPy.git.
-
 ==========
 REFERENCES
 ==========
 
 If used for a publication, please cite both [1] for the shape
 descriptor method and [2] for the application to brain MRI and
-definiton of the BrainPrint.
+definition of the BrainPrint.
 
 [1] M. Reuter, F.-E. Wolter and N. Peinecke.
 Laplace-Beltrami spectra as "Shape-DNA" of surfaces and solids.
 Computer-Aided Design 38 (4), pp.342-366, 2006.
 http://dx.doi.org/10.1016/j.cad.2005.10.011
 
 [2] C. Wachinger, P. Golland, W. Kremen, B. Fischl, M. Reuter.
```

### Comparing `brainprint-0.3.0/brainprint/cli/parser.py` & `brainprint-0.4.0/brainprint/cli/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         default="euc",
         metavar="<euc>",
         choices=["euc"],
         required=False,
     )
     optional.add_argument(
         "--cholmod",
-        dest="cholmod",
+        dest="use_cholmod",
         help=help_text.CHOLMOD,
         default=False,
         action="store_true",
         required=False,
     )
 
     # Output options
```

### Comparing `brainprint-0.3.0/brainprint/surfaces.py` & `brainprint-0.4.0/brainprint/surfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
-Utilty module holding surface generation related functions.
+Utility module holding surface generation related functions.
 """
 import uuid
 from pathlib import Path
 from typing import Dict, List
 
-from lapy import TriaIO, TriaMesh
-from lapy.read_geometry import read_geometry
+from lapy import TriaMesh
 
 from .utils.utils import run_shell_command
 
 
 def create_aseg_surface(
     subject_dir: Path, destination: Path, indices: List[int]
 ) -> Path:
@@ -64,15 +63,14 @@
     )
     run_shell_command(conversion_command)
 
     return conversion_destination
 
 
 def create_aseg_surfaces(subject_dir: Path, destination: Path) -> Dict[str, Path]:
-
     # Define aseg labels
 
     # combined and individual aseg labels:
     # - Left  Striatum: left  Caudate + Putamen + Accumbens
     # - Right Striatum: right Caudate + Putamen + Accumbens
     # - CorpusCallosum: 5 subregions combined
     # - Cerebellum: brainstem + (left+right) cerebellum WM and GM
@@ -142,15 +140,15 @@
         cortical_surfaces = create_cortical_surfaces(subject_dir, destination)
         surfaces.update(cortical_surfaces)
     return surfaces
 
 
 def read_vtk(path: Path):
     try:
-        triangular_mesh = TriaIO.import_vtk(path)
+        triangular_mesh = TriaMesh.read_vtk(path)
     except Exception:
         message = "Failed to read VTK from the following path: {path}!".format(
             path=path
         )
         raise RuntimeError(message)
     else:
         if triangular_mesh is None:
@@ -173,10 +171,9 @@
         Equivalent *.vtk* file
 
     Returns
     -------
     Path
         Resulting *.vtk* file
     """
-    surface = read_geometry(source)
-    TriaIO.export_vtk(TriaMesh(v=surface[0], t=surface[1]), destination)
+    TriaMesh.read_fssurf(source).write_vtk(destination)
     return destination
```

### Comparing `brainprint-0.3.0/brainprint/utils/_config.py` & `brainprint-0.4.0/brainprint/utils/_config.py`

 * *Files identical despite different names*

### Comparing `brainprint-0.3.0/brainprint/utils/utils.py` & `brainprint-0.4.0/brainprint/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 
 def validate_environment() -> None:
     """
     Checks whether required environment variables are set.
     """
     if not os.getenv("FREESURFER_HOME"):
         raise RuntimeError(
-            "FreeSurfer root directory must be set as the $FREESURFER_HOME environment variable!"
+            "FreeSurfer root directory must be set as the $FREESURFER_HOME "
+            "environment variable!"
         )
 
 
 def test_freesurfer() -> None:
     """
     Tests FreeSurfer binarize are accessible and executable.
 
@@ -31,15 +32,16 @@
         Failed to execute test FreeSurfer command
     """
     command = "mri_binarize -version"
     try:
         run_shell_command(command)
     except FileNotFoundError:
         raise RuntimeError(
-            "Failed to run FreeSurfer command, please check the required binaries are included in your $PATH."
+            "Failed to run FreeSurfer command, please check the required binaries "
+            "are included in your $PATH."
         )
 
 
 def run_shell_command(command: str, verbose: bool = False):
     """
     Execute shell command.
 
@@ -55,22 +57,26 @@
     """
     if verbose:
         print(f"Executing command:\t{command}", end="\n")
     args = shlex.split(command)
     try:
         return_code = subprocess.call(args)
     except Exception as e:
-        message = "Failed to execute the following command:\n{command}\nThe following exception was raised:\n{exception}".format(
-            command=command, exception=e
+        message = (
+            "Failed to execute the following command:\n{command}\n"
+            "The following exception was raised:\n{exception}".format(
+                command=command, exception=e
+            )
         )
         print(message)
         raise
     if return_code != 0:
-        message = "Execution of the following command:\n{command}\nReturned non-zero exit code!".format(
-            command=command
+        message = (
+            "Execution of the following command:\n{command}\n"
+            "Returned non-zero exit code!".format(command=command)
         )
         raise RuntimeError(message)
 
 
 def validate_subject_dir(subjects_dir: Path, subject_id: str) -> Path:
     """
     Checks the input FreeSurfer preprocessing results directory exists.
```

### Comparing `brainprint-0.3.0/brainprint.egg-info/PKG-INFO` & `brainprint-0.4.0/brainprint.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainprint
-Version: 0.3.0
+Version: 0.4.0
 Summary: A package to compute BrainPrint (shape descriptors) from FastSurfer/FreeSurfer MRI segmentations
 Author-email: Martin Reuter <martin.reuter@dzne.de>, Kersten Diers <kersten.diers@dzne.de>
 Maintainer-email: Martin Reuter <martin.reuter@dzne.de>
 License: MIT License
         
         Copyright (c) 2019 Image Analysis, DZNE e.V.
         
@@ -38,23 +38,24 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.4
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: style
 Provides-Extra: test
 Provides-Extra: all
 Provides-Extra: full
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/brainprint.svg)](https://pypi.org/project/brainprint/)
 # BrainPrint
 
 This is the `brainprint` python package, a derivative of the original
 [BrainPrint-legacy](https://github.com/Deep-MI/BrainPrint-legacy) scripts,
 with the primary goal to provide a Python-only version, to integrate the
 [LaPy](https://github.com/Deep-MI/LaPy) package, and to remove dependencies
 on third-party software (shapeDNA-* binaries, gmsh, meshfix). As a result,
```

### Comparing `brainprint-0.3.0/brainprint.egg-info/SOURCES.txt` & `brainprint-0.4.0/brainprint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brainprint-0.3.0/pyproject.toml` & `brainprint-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ['setuptools >= 61.0.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'brainprint'
-version = '0.3.0'
+version = '0.4.0'
 description = 'A package to compute BrainPrint (shape descriptors) from FastSurfer/FreeSurfer MRI segmentations'
 readme = 'README.md'
 license = {file = 'LICENSE'}
-requires-python = '>=3.4'
+requires-python = '>=3.8'
 authors = [
     {name = 'Martin Reuter', email = 'martin.reuter@dzne.de'},
     {name = 'Kersten Diers', email = 'kersten.diers@dzne.de'},
 ]
 maintainers = [
     {name = 'Martin Reuter', email = 'martin.reuter@dzne.de'},
 ]
@@ -34,29 +34,30 @@
     'License :: OSI Approved :: MIT License',
     'Intended Audience :: Science/Research',
 ]
 dependencies = [
     'numpy',
     'scipy',
     'pandas',
-    'lapy'
+    'lapy >= 1.0.0, <2',
+    'psutil'
 ]
 
 [project.optional-dependencies]
 build = [
     'build',
     'twine',
 ]
 style = [
     'bibclean',
     'black',
     'codespell',
     'isort',
-    'flake8',
     'pydocstyle[toml]',
+    'ruff',
 ]
 test = [
     'pytest',
     'pytest-cov',
     'pytest-timeout',
 ]
 all = [
@@ -89,15 +90,15 @@
 [tool.black]
 line-length = 88
 target-version = ['py38']
 include = '\.pyi?$'
 extend-exclude = '''
 (
       __pycache__
-    | \.github
+    | .github
     | setup.py
     | data/
     | examples/
 )
 '''
 
 [tool.isort]
@@ -114,14 +115,24 @@
 [tool.pydocstyle]
 convention = 'numpy'
 ignore-decorators = '(copy_doc|property|.*setter|.*getter|pyqtSlot|Slot)'
 match = '^(?!setup|__init__|test_).*\.py'
 match-dir = '^brainprint.*'
 add_ignore = 'D100,D104,D107'
 
+[tool.ruff]
+line-length = 88
+extend-exclude = [
+    "doc",
+    "setup.py",
+]
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = ["F401"]
+
 [tool.pytest.ini_options]
 minversion = '6.0'
 addopts = '--durations 20 --junit-xml=junit-results.xml --verbose'
 filterwarnings = []
 
 [tool.coverage.run]
 branch = true
```

