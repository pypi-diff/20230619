# Comparing `tmp/cmyt-1.2.0.tar.gz` & `tmp/cmyt-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmyt-1.2.0.tar", last modified: Sun Apr 16 18:27:36 2023, max compression
+gzip compressed data, was "cmyt-1.2.1.tar", last modified: Mon Jun 19 12:04:50 2023, max compression
```

## Comparing `cmyt-1.2.0.tar` & `cmyt-1.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:27:36.192787 cmyt-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-16 18:27:24.000000 cmyt-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-16 18:27:36.192787 cmyt-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-16 18:27:24.000000 cmyt-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:27:36.188787 cmyt-1.2.0/cmyt/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/cm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:27:36.192787 cmyt-1.2.0/cmyt/colormaps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/algae.py
--rw-r--r--   0 runner    (1001) docker     (123)    17723 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/apricity.py
--rw-r--r--   0 runner    (1001) docker     (123)    19063 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/arbre.py
--rw-r--r--   0 runner    (1001) docker     (123)    19345 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/dusk.py
--rw-r--r--   0 runner    (1001) docker     (123)    19006 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/kelp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19059 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/octarine.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/pastel.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/pixel_blue.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/pixel_green.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/pixel_red.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/xray.py
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:27:36.188787 cmyt-1.2.0/cmyt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-16 18:27:36.000000 cmyt-1.2.0/cmyt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-16 18:27:36.000000 cmyt-1.2.0/cmyt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 18:27:36.000000 cmyt-1.2.0/cmyt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-16 18:27:36.000000 cmyt-1.2.0/cmyt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-16 18:27:36.000000 cmyt-1.2.0/cmyt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-16 18:27:24.000000 cmyt-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 18:27:36.192787 cmyt-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:27:36.192787 cmyt-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-16 18:27:24.000000 cmyt-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-16 18:27:24.000000 cmyt-1.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-16 18:27:24.000000 cmyt-1.2.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-16 18:27:24.000000 cmyt-1.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:04:50.358384 cmyt-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-19 12:04:40.000000 cmyt-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-06-19 12:04:50.358384 cmyt-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-19 12:04:40.000000 cmyt-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:04:50.354384 cmyt-1.2.1/cmyt/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/cm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:04:50.354384 cmyt-1.2.1/cmyt/colormaps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/algae.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/apricity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19009 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/arbre.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/dusk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/kelp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19005 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/octarine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/pastel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/pixel_blue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/pixel_green.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/pixel_red.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/colormaps/xray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-19 12:04:40.000000 cmyt-1.2.1/cmyt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:04:50.354384 cmyt-1.2.1/cmyt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-06-19 12:04:50.000000 cmyt-1.2.1/cmyt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-19 12:04:50.000000 cmyt-1.2.1/cmyt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 12:04:50.000000 cmyt-1.2.1/cmyt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-19 12:04:50.000000 cmyt-1.2.1/cmyt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-19 12:04:50.000000 cmyt-1.2.1/cmyt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-19 12:04:40.000000 cmyt-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 12:04:50.358384 cmyt-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:04:50.358384 cmyt-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-19 12:04:40.000000 cmyt-1.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-19 12:04:40.000000 cmyt-1.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-19 12:04:40.000000 cmyt-1.2.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-19 12:04:40.000000 cmyt-1.2.1/tests/test_utils.py
```

### Comparing `cmyt-1.2.0/LICENSE` & `cmyt-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmyt-1.2.0/PKG-INFO` & `cmyt-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmyt
-Version: 1.2.0
+Version: 1.2.1
 Summary: A collection of Matplotlib colormaps from the yt project
 Author-email: The yt project <yt-dev@python.org>
 License: BSD 3-Clause
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Source, https://github.com/yt-project/cmyt/
 Project-URL: Tracker, https://github.com/yt-project/cmyt/issues
 Keywords: visualization
@@ -31,15 +31,15 @@
 
 [![CI](https://github.com/yt-project/cmyt/actions/workflows/ci.yml/badge.svg)](https://github.com/yt-project/cmyt/actions/workflows/ci.yml)
 [![CI (bleeding edge)](https://github.com/yt-project/cmyt/actions/workflows/bleeding-edge.yaml/badge.svg)](https://github.com/yt-project/cmyt/actions/workflows/bleeding-edge.yaml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/yt-project/cmyt/main.svg)](https://results.pre-commit.ci/latest/github/yt-project/cmyt/main)
 
 [![yt-project](https://img.shields.io/static/v1?label="works%20with"&message="yt"&color="blueviolet")](https://yt-project.org)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 <a href="http://yt-project.org"><img src="https://raw.githubusercontent.com/yt-project/yt/main/doc/source/_static/yt_logo.png" width="150"></a>
 
 Matplotlib colormaps from the yt project !
 
 ## Colormaps overview
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cmyt Version: 1.2.0 Summary: A collection of
+Metadata-Version: 2.1 Name: cmyt Version: 1.2.1 Summary: A collection of
 Matplotlib colormaps from the yt project Author-email: The yt project
 python.org> License: BSD 3-Clause Project-URL: Homepage, https://yt-
 project.org/ Project-URL: Source, https://github.com/yt-project/cmyt/ Project-
 URL: Tracker, https://github.com/yt-project/cmyt/issues Keywords: visualization
 Classifier: Development Status :: 5 - Production/Stable Classifier: Framework
 :: Matplotlib Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: MacOS ::
@@ -24,15 +24,15 @@
 bleeding-edge.yaml) [![pre-commit.ci status](https://results.pre-commit.ci/
 badge/github/yt-project/cmyt/main.svg)](https://results.pre-commit.ci/latest/
 github/yt-project/cmyt/main) [![yt-project](https://img.shields.io/static/
 v1?label="works%20with"&message="yt"&color="blueviolet")](https://yt-
 project.org) [![Code style: black](https://img.shields.io/badge/code%20style-
 black-000000.svg)](https://github.com/psf/black) [![Ruff](https://
 img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/
-ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff) [https:
+ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff) [https:
 //raw.githubusercontent.com/yt-project/yt/main/doc/source/_static/yt_logo.png]
 Matplotlib colormaps from the yt project ! ## Colormaps overview The following
 colormaps, as well as their respective reversed (`*_r`) versions are available
 ### Perceptually uniform sequential colormaps
          [https://raw.githubusercontent.com/yt-project/cmyt/main/doc/
                       overview_perceptually_uniform.png]
 ### Monochromatic sequential colormaps
```

### Comparing `cmyt-1.2.0/README.md` & `cmyt-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [![CI](https://github.com/yt-project/cmyt/actions/workflows/ci.yml/badge.svg)](https://github.com/yt-project/cmyt/actions/workflows/ci.yml)
 [![CI (bleeding edge)](https://github.com/yt-project/cmyt/actions/workflows/bleeding-edge.yaml/badge.svg)](https://github.com/yt-project/cmyt/actions/workflows/bleeding-edge.yaml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/yt-project/cmyt/main.svg)](https://results.pre-commit.ci/latest/github/yt-project/cmyt/main)
 
 [![yt-project](https://img.shields.io/static/v1?label="works%20with"&message="yt"&color="blueviolet")](https://yt-project.org)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 <a href="http://yt-project.org"><img src="https://raw.githubusercontent.com/yt-project/yt/main/doc/source/_static/yt_logo.png" width="150"></a>
 
 Matplotlib colormaps from the yt project !
 
 ## Colormaps overview
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
 bleeding-edge.yaml) [![pre-commit.ci status](https://results.pre-commit.ci/
 badge/github/yt-project/cmyt/main.svg)](https://results.pre-commit.ci/latest/
 github/yt-project/cmyt/main) [![yt-project](https://img.shields.io/static/
 v1?label="works%20with"&message="yt"&color="blueviolet")](https://yt-
 project.org) [![Code style: black](https://img.shields.io/badge/code%20style-
 black-000000.svg)](https://github.com/psf/black) [![Ruff](https://
 img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/
-ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff) [https:
+ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff) [https:
 //raw.githubusercontent.com/yt-project/yt/main/doc/source/_static/yt_logo.png]
 Matplotlib colormaps from the yt project ! ## Colormaps overview The following
 colormaps, as well as their respective reversed (`*_r`) versions are available
 ### Perceptually uniform sequential colormaps
          [https://raw.githubusercontent.com/yt-project/cmyt/main/doc/
                       overview_perceptually_uniform.png]
 ### Monochromatic sequential colormaps
```

### Comparing `cmyt-1.2.0/cmyt/cm.py` & `cmyt-1.2.1/cmyt/cm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,21 @@
 from importlib import import_module
 
-import numpy as np
-
-from cmyt.utils import ColorDict, cmyt_cmaps, register_colormap
-
-
-def _luts_to_cdict(luts: np.ndarray) -> ColorDict:
-    _vs = np.linspace(0, 1, 256)
-
-    return {
-        "red": np.transpose([_vs, luts[0], luts[0]]),
-        "green": np.transpose([_vs, luts[1], luts[1]]),
-        "blue": np.transpose([_vs, luts[2], luts[2]]),
-    }
-
+from cmyt.utils import cmyt_cmaps, register_colormap
 
 for name in cmyt_cmaps:
     # register to MPL
     mod = import_module(f"cmyt.colormaps.{name}")
     if hasattr(mod, "data"):
-        data = mod.data
+        cmap, cmap_r = register_colormap(name, color_dict=mod.data)
     elif hasattr(mod, "luts"):
-        data = _luts_to_cdict(mod.luts)
+        cmap, cmap_r = register_colormap(name, colors=mod.luts)
     else:
         raise RuntimeError(
             f"colormap module '{name}' doesn't contain necessary data for registration."
         )
-    cmap, cmap_r = register_colormap(name, data)
 
     globals()[cmap.name] = cmap
     globals()[cmap_r.name] = cmap_r
 
 
 __all__ = tuple(cmyt_cmaps) + tuple(f"{name}_r" for name in cmyt_cmaps)
```

### Comparing `cmyt-1.2.0/cmyt/colormaps/algae.py` & `cmyt-1.2.1/cmyt/colormaps/algae.py`

 * *Files identical despite different names*

### Comparing `cmyt-1.2.0/cmyt/colormaps/apricity.py` & `cmyt-1.2.1/cmyt/colormaps/apricity.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     "fixed": -1,
     "filter_k": 100,
     "cmtype": "linear",
     "uniform_colorspace": "CAM02-UCS",
     "spline_method": "CatmulClark",
 }
 
-luts = (
-    np.array(
+luts = np.transpose(
+    (
         [
             0.349019,
             0.349019,
             0.349019,
             0.349019,
             0.352941,
             0.352941,
@@ -284,17 +284,15 @@
             0.929411,
             0.933333,
             0.941176,
             0.945098,
             0.952941,
             0.956862,
             0.964705,
-        ]
-    ),
-    np.array(
+        ],
         [
             0.411764,
             0.4156864,
             0.419607,
             0.423529,
             0.423529,
             0.4274504,
@@ -544,17 +542,15 @@
             0.956862,
             0.960784,
             0.960784,
             0.960784,
             0.964705,
             0.964705,
             0.964705,
-        ]
-    ),
-    np.array(
+        ],
         [
             0.686274,
             0.682352,
             0.682352,
             0.678431,
             0.678431,
             0.674509,
@@ -804,11 +800,10 @@
             0.258823,
             0.250980,
             0.247058,
             0.239215,
             0.231372,
             0.223529,
             0.215686,
-        ]
-    ),
-    np.ones(256),
+        ],
+    )
 )
```

### Comparing `cmyt-1.2.0/cmyt/colormaps/arbre.py` & `cmyt-1.2.1/cmyt/colormaps/arbre.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
         41.007532956685509,
         31.532485875706215,
     ],
     "min_Jp": 27.2243940579,
     "max_Jp": 94.7771696638,
 }
 
-luts = (
-    np.array(
+luts = np.transpose(
+    (
         [
             0.44131774,
             0.44370177,
             0.44605933,
             0.44839054,
             0.45067478,
             0.45293504,
@@ -276,17 +276,15 @@
             0.933148,
             0.94530521,
             0.95690622,
             0.96783447,
             0.97790967,
             0.986926,
             0.99464852,
-        ]
-    ),
-    np.array(
+        ],
         [
             0.05626182,
             0.06063603,
             0.06486246,
             0.06895821,
             0.07296132,
             0.0768539,
@@ -536,17 +534,15 @@
             0.94487644,
             0.94486297,
             0.94496862,
             0.9452415,
             0.94575723,
             0.94660423,
             0.94788672,
-        ]
-    ),
-    np.array(
+        ],
         [
             0.04951266,
             0.06083219,
             0.07165053,
             0.08210915,
             0.09247329,
             0.10260581,
@@ -796,11 +792,10 @@
             0.18441057,
             0.19343386,
             0.2047358,
             0.21833687,
             0.2341978,
             0.25223614,
             0.2722682,
-        ]
-    ),
-    np.ones(256),
+        ],
+    )
 )
```

### Comparing `cmyt-1.2.0/cmyt/colormaps/dusk.py` & `cmyt-1.2.1/cmyt/colormaps/dusk.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         58.514492753623216,
         0.1811594202898732,
     ],
     "min_Jp": 3.96624472574,
     "max_Jp": 96.5975103734,
 }
 
-luts = (
-    np.array(
+luts = np.transpose(
+    (
         [
             0.02379297,
             0.0261157,
             0.02850455,
             0.03095137,
             0.0334476,
             0.0360304,
@@ -286,17 +286,15 @@
             0.96735109,
             0.96853232,
             0.96975252,
             0.97100046,
             0.9722811,
             0.97360166,
             0.97499094,
-        ]
-    ),
-    np.array(
+        ],
         [
             0.01131879,
             0.01391783,
             0.01674789,
             0.01980761,
             0.02309557,
             0.02659703,
@@ -546,17 +544,15 @@
             0.91230608,
             0.91806899,
             0.9238354,
             0.92961071,
             0.93539672,
             0.94119732,
             0.94701577,
-        ]
-    ),
-    np.array(
+        ],
         [
             0.02001135,
             0.02410049,
             0.0285127,
             0.03327199,
             0.03840892,
             0.04377278,
@@ -806,11 +802,10 @@
             0.89277169,
             0.90169092,
             0.91054951,
             0.91934683,
             0.92805132,
             0.93660318,
             0.9448656,
-        ]
-    ),
-    np.ones(256),
+        ],
+    )
 )
```

### Comparing `cmyt-1.2.0/cmyt/colormaps/kelp.py` & `cmyt-1.2.1/cmyt/colormaps/kelp.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
         -13.6284722222222,
         23.4375,
     ],
     "min_Jp": 15,
     "max_Jp": 95,
 }
 
-luts = (
-    np.array(
+luts = np.transpose(
+    (
         [
             0.07873808,
             0.08503098,
             0.09119215,
             0.09725944,
             0.10324966,
             0.10914691,
@@ -276,17 +276,15 @@
             0.93489628,
             0.94222522,
             0.94961559,
             0.95703072,
             0.96451696,
             0.97201416,
             0.97959794,
-        ]
-    ),
-    np.array(
+        ],
         [
             0.02380049,
             0.02762946,
             0.0314955,
             0.03538367,
             0.03929263,
             0.04314916,
@@ -536,17 +534,15 @@
             0.92900992,
             0.93214934,
             0.93527665,
             0.93840226,
             0.94151285,
             0.9446259,
             0.94771918,
-        ]
-    ),
-    np.array(
+        ],
         [
             0.45890713,
             0.46137905,
             0.46384563,
             0.46630529,
             0.46875421,
             0.4711862,
@@ -796,11 +792,10 @@
             0.53904386,
             0.53620824,
             0.53329363,
             0.53036982,
             0.52734442,
             0.52433316,
             0.52118636,
-        ]
-    ),
-    np.ones(256),
+        ],
+    )
 )
```

### Comparing `cmyt-1.2.0/cmyt/colormaps/octarine.py` & `cmyt-1.2.1/cmyt/colormaps/octarine.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
         -23.958333333333314,
         -16.059027777777771,
     ],
     "min_Jp": 17.1875,
     "max_Jp": 82.1875,
 }
 
-luts = (
-    np.array(
+luts = np.transpose(
+    (
         [
             0.01845663,
             0.01940818,
             0.02066025,
             0.02218966,
             0.02395409,
             0.02595033,
@@ -277,17 +277,15 @@
             0.90556318,
             0.90603649,
             0.90695623,
             0.90913313,
             0.91657895,
             0.92518702,
             0.93347579,
-        ]
-    ),
-    np.array(
+        ],
         [
             0.14549808,
             0.14959758,
             0.15353745,
             0.15733732,
             0.1610376,
             0.16463933,
@@ -537,17 +535,15 @@
             0.66421949,
             0.66770704,
             0.67086745,
             0.67317041,
             0.67282641,
             0.67266658,
             0.67286793,
-        ]
-    ),
-    np.array(
+        ],
         [
             0.31784919,
             0.31399639,
             0.31040105,
             0.30704607,
             0.30380333,
             0.30070875,
@@ -797,11 +793,10 @@
             0.94285311,
             0.95166927,
             0.96090167,
             0.97095595,
             0.97849108,
             0.98057884,
             0.98147471,
-        ]
-    ),
-    np.ones(256),
+        ],
+    )
 )
```

### Comparing `cmyt-1.2.0/cmyt/colormaps/pastel.py` & `cmyt-1.2.1/cmyt/colormaps/pastel.py`

 * *Files identical despite different names*

### Comparing `cmyt-1.2.0/cmyt/colormaps/xray.py` & `cmyt-1.2.1/cmyt/colormaps/xray.py`

 * *Files identical despite different names*

### Comparing `cmyt-1.2.0/cmyt/utils.py` & `cmyt-1.2.1/cmyt/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import re
 import sys
 from typing import TYPE_CHECKING, Dict, Final, Iterable, Literal, Optional, Tuple
 
 import matplotlib
 import numpy as np
-from matplotlib.colors import Colormap, LinearSegmentedColormap
+from matplotlib.colors import Colormap, LinearSegmentedColormap, ListedColormap
 from more_itertools import always_iterable
 
 # type aliases
 
 if TYPE_CHECKING:
     from matplotlib.axes import Axes
     from matplotlib.figure import Figure
@@ -91,28 +91,42 @@
         from matplotlib.cm import register_cmap
 
         register_cmap(cmap=cmap)
 
 
 def register_colormap(
     name: str,
-    color_dict: ColorDict,
+    *,
+    color_dict: Optional[ColorDict] = None,
+    colors: Optional[np.ndarray] = None,
 ) -> Tuple[LinearSegmentedColormap, LinearSegmentedColormap]:
     name = prefix_name(name)
 
+    if color_dict is not None and colors is not None:
+        raise TypeError("Either color_dict or colors must be provided, but not both")
     # register to MPL
-    mpl_cmap = LinearSegmentedColormap(name=name, segmentdata=color_dict, N=256)
+    if color_dict is not None:
+        mpl_cmap = LinearSegmentedColormap(name=name, segmentdata=color_dict, N=256)
+    elif colors is not None:
+        mpl_cmap = ListedColormap(colors, name=name, N=256)
+    else:
+        raise TypeError("color_dict or colors must be provided")
     mpl_cmap_r = mpl_cmap.reversed()
     _register_mpl_cmap(mpl_cmap)
     _register_mpl_cmap(mpl_cmap_r)
 
     # return cmaps with unprefixed names for registration as importable objects
-    cmap = LinearSegmentedColormap(
-        name=unprefix_name(name), segmentdata=color_dict, N=256
-    )
+    if MPL_VERSION >= (3, 4):
+        cmap = mpl_cmap.copy()
+    else:
+        if color_dict is not None:
+            cmap = LinearSegmentedColormap(name=name, segmentdata=color_dict, N=256)
+        elif colors is not None:
+            cmap = ListedColormap(colors, name=name, N=256)
+    cmap.name = unprefix_name(name)
     cmap_r = cmap.reversed()
 
     return cmap, cmap_r
 
 
 graySCALE_CONVERSION_SPACE = "JCh"
```

### Comparing `cmyt-1.2.0/cmyt.egg-info/PKG-INFO` & `cmyt-1.2.1/cmyt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmyt
-Version: 1.2.0
+Version: 1.2.1
 Summary: A collection of Matplotlib colormaps from the yt project
 Author-email: The yt project <yt-dev@python.org>
 License: BSD 3-Clause
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Source, https://github.com/yt-project/cmyt/
 Project-URL: Tracker, https://github.com/yt-project/cmyt/issues
 Keywords: visualization
@@ -31,15 +31,15 @@
 
 [![CI](https://github.com/yt-project/cmyt/actions/workflows/ci.yml/badge.svg)](https://github.com/yt-project/cmyt/actions/workflows/ci.yml)
 [![CI (bleeding edge)](https://github.com/yt-project/cmyt/actions/workflows/bleeding-edge.yaml/badge.svg)](https://github.com/yt-project/cmyt/actions/workflows/bleeding-edge.yaml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/yt-project/cmyt/main.svg)](https://results.pre-commit.ci/latest/github/yt-project/cmyt/main)
 
 [![yt-project](https://img.shields.io/static/v1?label="works%20with"&message="yt"&color="blueviolet")](https://yt-project.org)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 <a href="http://yt-project.org"><img src="https://raw.githubusercontent.com/yt-project/yt/main/doc/source/_static/yt_logo.png" width="150"></a>
 
 Matplotlib colormaps from the yt project !
 
 ## Colormaps overview
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cmyt Version: 1.2.0 Summary: A collection of
+Metadata-Version: 2.1 Name: cmyt Version: 1.2.1 Summary: A collection of
 Matplotlib colormaps from the yt project Author-email: The yt project
 python.org> License: BSD 3-Clause Project-URL: Homepage, https://yt-
 project.org/ Project-URL: Source, https://github.com/yt-project/cmyt/ Project-
 URL: Tracker, https://github.com/yt-project/cmyt/issues Keywords: visualization
 Classifier: Development Status :: 5 - Production/Stable Classifier: Framework
 :: Matplotlib Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: MacOS ::
@@ -24,15 +24,15 @@
 bleeding-edge.yaml) [![pre-commit.ci status](https://results.pre-commit.ci/
 badge/github/yt-project/cmyt/main.svg)](https://results.pre-commit.ci/latest/
 github/yt-project/cmyt/main) [![yt-project](https://img.shields.io/static/
 v1?label="works%20with"&message="yt"&color="blueviolet")](https://yt-
 project.org) [![Code style: black](https://img.shields.io/badge/code%20style-
 black-000000.svg)](https://github.com/psf/black) [![Ruff](https://
 img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/
-ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff) [https:
+ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff) [https:
 //raw.githubusercontent.com/yt-project/yt/main/doc/source/_static/yt_logo.png]
 Matplotlib colormaps from the yt project ! ## Colormaps overview The following
 colormaps, as well as their respective reversed (`*_r`) versions are available
 ### Perceptually uniform sequential colormaps
          [https://raw.githubusercontent.com/yt-project/cmyt/main/doc/
                       overview_perceptually_uniform.png]
 ### Monochromatic sequential colormaps
```

### Comparing `cmyt-1.2.0/cmyt.egg-info/SOURCES.txt` & `cmyt-1.2.1/cmyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmyt-1.2.0/pyproject.toml` & `cmyt-1.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cmyt"
-version = "1.2.0"
+version = "1.2.1"
 description = "A collection of Matplotlib colormaps from the yt project"
 authors = [
     { name = "The yt project", email = "yt-dev@python.org" },
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Matplotlib",
@@ -57,17 +57,19 @@
 [tool.ruff]
 exclude = ["*__init__.py"]
 ignore = ["E501"]
 select = [
     "E",
     "F",
     "W",
-    "B",
-    "I",
-    "UP",
+    "C4",  # flake8-comprehensions
+    "B",   # flake8-bugbear
+    "YTT", # flake8-2020
+    "I",   # isort
+    "UP",  # pyupgrade
 ]
 
 [tool.ruff.isort]
 combine-as-imports = true
 
 [tool.mypy]
 python_version = "3.8"
```

### Comparing `cmyt-1.2.0/tests/test_integration.py` & `cmyt-1.2.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `cmyt-1.2.0/tests/test_utils.py` & `cmyt-1.2.1/tests/test_utils.py`

 * *Files identical despite different names*

