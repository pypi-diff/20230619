# Comparing `tmp/trianglechain-0.4.1.tar.gz` & `tmp/trianglechain-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trianglechain-0.4.1.tar", last modified: Fri Jun  9 15:12:25 2023, max compression
+gzip compressed data, was "trianglechain-0.4.2.tar", last modified: Mon Jun 19 13:43:18 2023, max compression
```

## Comparing `trianglechain-0.4.1.tar` & `trianglechain-0.4.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-09 15:12:25.094668 trianglechain-0.4.1/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      201 2023-05-04 11:29:54.000000 trianglechain-0.4.1/AUTHORS.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1708 2023-05-04 11:29:54.000000 trianglechain-0.4.1/CONTRIBUTING.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1670 2023-06-09 15:11:54.000000 trianglechain-0.4.1/HISTORY.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1116 2023-05-04 11:29:54.000000 trianglechain-0.4.1/LICENSE
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)       99 2023-05-04 11:29:54.000000 trianglechain-0.4.1/MANIFEST.in
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-06-09 15:12:25.094738 trianglechain-0.4.1/PKG-INFO
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1594 2023-05-04 11:29:54.000000 trianglechain-0.4.1/README.md
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      735 2023-05-04 11:29:54.000000 trianglechain-0.4.1/pyproject.toml
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1385 2023-06-09 15:12:25.095086 trianglechain-0.4.1/setup.cfg
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-09 15:12:25.088569 trianglechain-0.4.1/src/
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-09 15:12:25.092606 trianglechain-0.4.1/src/trianglechain/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     8714 2023-05-04 11:29:54.000000 trianglechain-0.4.1/src/trianglechain/BaseChain.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13478 2023-05-04 11:29:54.000000 trianglechain-0.4.1/src/trianglechain/LineChain.py
--rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)    28003 2023-06-05 12:25:46.000000 trianglechain-0.4.1/src/trianglechain/TriangleChain.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      319 2023-06-09 15:11:46.000000 trianglechain-0.4.1/src/trianglechain/__init__.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13417 2023-05-04 11:29:54.000000 trianglechain-0.4.1/src/trianglechain/bestfit.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     9932 2023-06-05 12:25:46.000000 trianglechain-0.4.1/src/trianglechain/density_estimation.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     7853 2023-05-04 11:29:54.000000 trianglechain-0.4.1/src/trianglechain/limits.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    16854 2023-06-09 15:08:20.000000 trianglechain-0.4.1/src/trianglechain/make_subplots.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     4349 2023-05-04 11:29:54.000000 trianglechain-0.4.1/src/trianglechain/params.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     3024 2023-05-04 11:29:54.000000 trianglechain-0.4.1/src/trianglechain/utils_pj_hpd.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    19680 2023-06-05 12:25:46.000000 trianglechain-0.4.1/src/trianglechain/utils_plots.py
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-09 15:12:25.093653 trianglechain-0.4.1/src/trianglechain.egg-info/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-06-09 15:12:25.000000 trianglechain-0.4.1/src/trianglechain.egg-info/PKG-INFO
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      809 2023-06-09 15:12:25.000000 trianglechain-0.4.1/src/trianglechain.egg-info/SOURCES.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-06-09 15:12:25.000000 trianglechain-0.4.1/src/trianglechain.egg-info/dependency_links.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-05-11 08:24:36.000000 trianglechain-0.4.1/src/trianglechain.egg-info/not-zip-safe
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      308 2023-06-09 15:12:25.000000 trianglechain-0.4.1/src/trianglechain.egg-info/requires.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)       14 2023-06-09 15:12:25.000000 trianglechain-0.4.1/src/trianglechain.egg-info/top_level.txt
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-09 15:12:25.094538 trianglechain-0.4.1/tests/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      674 2023-05-04 11:29:54.000000 trianglechain-0.4.1/tests/test_bestfit.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2013 2023-05-04 11:29:54.000000 trianglechain-0.4.1/tests/test_limits.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      748 2023-05-04 11:29:54.000000 trianglechain-0.4.1/tests/test_linechain.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2897 2023-05-04 11:29:54.000000 trianglechain-0.4.1/tests/test_params.py
--rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)     4006 2023-05-04 11:29:54.000000 trianglechain-0.4.1/tests/test_trianglechain.py
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-19 13:43:18.043530 trianglechain-0.4.2/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      201 2023-05-04 11:29:54.000000 trianglechain-0.4.2/AUTHORS.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1708 2023-05-04 11:29:54.000000 trianglechain-0.4.2/CONTRIBUTING.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1752 2023-06-19 13:42:54.000000 trianglechain-0.4.2/HISTORY.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1116 2023-05-04 11:29:54.000000 trianglechain-0.4.2/LICENSE
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)       99 2023-05-04 11:29:54.000000 trianglechain-0.4.2/MANIFEST.in
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-06-19 13:43:18.043597 trianglechain-0.4.2/PKG-INFO
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1594 2023-05-04 11:29:54.000000 trianglechain-0.4.2/README.md
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      735 2023-05-04 11:29:54.000000 trianglechain-0.4.2/pyproject.toml
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1385 2023-06-19 13:43:18.043939 trianglechain-0.4.2/setup.cfg
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-19 13:43:18.038831 trianglechain-0.4.2/src/
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-19 13:43:18.041632 trianglechain-0.4.2/src/trianglechain/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     8714 2023-05-04 11:29:54.000000 trianglechain-0.4.2/src/trianglechain/BaseChain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13478 2023-05-04 11:29:54.000000 trianglechain-0.4.2/src/trianglechain/LineChain.py
+-rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)    28041 2023-06-19 13:40:12.000000 trianglechain-0.4.2/src/trianglechain/TriangleChain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      319 2023-06-19 13:42:58.000000 trianglechain-0.4.2/src/trianglechain/__init__.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13417 2023-05-04 11:29:54.000000 trianglechain-0.4.2/src/trianglechain/bestfit.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     9932 2023-06-05 12:25:46.000000 trianglechain-0.4.2/src/trianglechain/density_estimation.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     7853 2023-05-04 11:29:54.000000 trianglechain-0.4.2/src/trianglechain/limits.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    16854 2023-06-09 15:08:20.000000 trianglechain-0.4.2/src/trianglechain/make_subplots.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     4349 2023-05-04 11:29:54.000000 trianglechain-0.4.2/src/trianglechain/params.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     3024 2023-05-04 11:29:54.000000 trianglechain-0.4.2/src/trianglechain/utils_pj_hpd.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    19680 2023-06-05 12:25:46.000000 trianglechain-0.4.2/src/trianglechain/utils_plots.py
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-19 13:43:18.042646 trianglechain-0.4.2/src/trianglechain.egg-info/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-06-19 13:43:17.000000 trianglechain-0.4.2/src/trianglechain.egg-info/PKG-INFO
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      809 2023-06-19 13:43:18.000000 trianglechain-0.4.2/src/trianglechain.egg-info/SOURCES.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-06-19 13:43:17.000000 trianglechain-0.4.2/src/trianglechain.egg-info/dependency_links.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-05-11 08:24:36.000000 trianglechain-0.4.2/src/trianglechain.egg-info/not-zip-safe
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      308 2023-06-19 13:43:17.000000 trianglechain-0.4.2/src/trianglechain.egg-info/requires.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)       14 2023-06-19 13:43:17.000000 trianglechain-0.4.2/src/trianglechain.egg-info/top_level.txt
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-19 13:43:18.043415 trianglechain-0.4.2/tests/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      674 2023-05-04 11:29:54.000000 trianglechain-0.4.2/tests/test_bestfit.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2013 2023-05-04 11:29:54.000000 trianglechain-0.4.2/tests/test_limits.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      748 2023-05-04 11:29:54.000000 trianglechain-0.4.2/tests/test_linechain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2897 2023-05-04 11:29:54.000000 trianglechain-0.4.2/tests/test_params.py
+-rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)     4006 2023-05-04 11:29:54.000000 trianglechain-0.4.2/tests/test_trianglechain.py
```

### Comparing `trianglechain-0.4.1/CONTRIBUTING.rst` & `trianglechain-0.4.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.1/HISTORY.rst` & `trianglechain-0.4.2/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 .. :changelog:
 
 History
 -------
 
+0.4.2 (2023-06-19)
+++++++++++++++++++
+
+* FIX: scatter_kwargs for scatter_density
+
 0.4.1 (2023-06-09)
 ++++++++++++++++++
 
 * FIX: RGB(A) colors in plt.contour
 
 0.4.0 (2023-06-05)
 ++++++++++++++++++
```

### Comparing `trianglechain-0.4.1/LICENSE` & `trianglechain-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.1/PKG-INFO` & `trianglechain-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trianglechain
-Version: 0.4.1
+Version: 0.4.2
 Summary: Code to plot multidimensional distributions
 Author: Silvan Fischbacher, Tomasz Kacprzak
 Author-email: silvanf@phys.ethz.ch, tomaszk@phys.ethz.ch
 License: MIT License
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/trianglechain
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `trianglechain-0.4.1/README.md` & `trianglechain-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.1/pyproject.toml` & `trianglechain-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.1/setup.cfg` & `trianglechain-0.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.1/src/trianglechain/BaseChain.py` & `trianglechain-0.4.2/src/trianglechain/BaseChain.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.1/src/trianglechain/LineChain.py` & `trianglechain-0.4.2/src/trianglechain/LineChain.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.1/src/trianglechain/TriangleChain.py` & `trianglechain-0.4.2/src/trianglechain/TriangleChain.py`

 * *Files 1% similar despite different names*

```diff
@@ -551,14 +551,15 @@
                     n_bins=n_bins,
                     lim1=current_ranges[columns[j]],
                     lim2=current_ranges[columns[i]],
                     norm_cols=False,
                     n_points_scatter=-1,
                     cmap=cmap,
                     label=label,
+                    **scatter_kwargs,
                 )
             set_limits(
                 axc,
                 ranges,
                 current_ranges,
                 columns[i],
                 columns[j],
```

### Comparing `trianglechain-0.4.1/src/trianglechain/bestfit.py` & `trianglechain-0.4.2/src/trianglechain/bestfit.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.1/src/trianglechain/density_estimation.py` & `trianglechain-0.4.2/src/trianglechain/density_estimation.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.1/src/trianglechain/limits.py` & `trianglechain-0.4.2/src/trianglechain/limits.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.1/src/trianglechain/make_subplots.py` & `trianglechain-0.4.2/src/trianglechain/make_subplots.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.1/src/trianglechain/params.py` & `trianglechain-0.4.2/src/trianglechain/params.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.1/src/trianglechain/utils_pj_hpd.py` & `trianglechain-0.4.2/src/trianglechain/utils_pj_hpd.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.1/src/trianglechain/utils_plots.py` & `trianglechain-0.4.2/src/trianglechain/utils_plots.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.1/src/trianglechain.egg-info/PKG-INFO` & `trianglechain-0.4.2/src/trianglechain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trianglechain
-Version: 0.4.1
+Version: 0.4.2
 Summary: Code to plot multidimensional distributions
 Author: Silvan Fischbacher, Tomasz Kacprzak
 Author-email: silvanf@phys.ethz.ch, tomaszk@phys.ethz.ch
 License: MIT License
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/trianglechain
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `trianglechain-0.4.1/src/trianglechain.egg-info/SOURCES.txt` & `trianglechain-0.4.2/src/trianglechain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.1/tests/test_bestfit.py` & `trianglechain-0.4.2/tests/test_bestfit.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.1/tests/test_limits.py` & `trianglechain-0.4.2/tests/test_limits.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.1/tests/test_linechain.py` & `trianglechain-0.4.2/tests/test_linechain.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.1/tests/test_params.py` & `trianglechain-0.4.2/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.1/tests/test_trianglechain.py` & `trianglechain-0.4.2/tests/test_trianglechain.py`

 * *Files identical despite different names*

