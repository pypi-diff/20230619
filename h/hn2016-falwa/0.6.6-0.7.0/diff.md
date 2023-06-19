# Comparing `tmp/hn2016_falwa-0.6.6.tar.gz` & `tmp/hn2016_falwa-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hn2016_falwa-0.6.6.tar", last modified: Sun Apr  9 19:51:08 2023, max compression
+gzip compressed data, was "hn2016_falwa-0.7.0.tar", last modified: Mon Jun 19 03:13:28 2023, max compression
```

## Comparing `hn2016_falwa-0.6.6.tar` & `hn2016_falwa-0.7.0.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-04-09 19:51:08.770943 hn2016_falwa-0.6.6/
--rw-r--r--   0 claresyhuang   (501) staff       (20)     1065 2020-03-01 18:38:08.000000 hn2016_falwa-0.6.6/LICENSE.txt
--rw-r--r--   0 claresyhuang   (501) staff       (20)     1320 2023-04-09 19:51:08.770639 hn2016_falwa-0.6.6/PKG-INFO
-drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-04-09 19:51:08.558964 hn2016_falwa-0.6.6/hn2016_falwa/
--rw-r--r--   0 claresyhuang   (501) staff       (20)      679 2023-04-09 19:49:59.000000 hn2016_falwa-0.6.6/hn2016_falwa/__init__.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)     4834 2022-08-28 04:26:39.000000 hn2016_falwa-0.6.6/hn2016_falwa/barotropic_field.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)     4853 2022-08-28 04:26:28.000000 hn2016_falwa-0.6.6/hn2016_falwa/basis.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)      335 2023-01-17 16:56:08.000000 hn2016_falwa-0.6.6/hn2016_falwa/constant.py
-drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-04-09 19:51:08.647229 hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/
--rw-r--r--   0 claresyhuang   (501) staff       (20)     5000 2023-02-14 04:53:29.000000 hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/compute_flux_dirinv.f90
--rw-r--r--   0 claresyhuang   (501) staff       (20)     5819 2023-02-14 04:53:29.000000 hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/compute_lwa_and_barotropic_fluxes.f90
--rw-r--r--   0 claresyhuang   (501) staff       (20)     4592 2023-01-17 16:56:08.000000 hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/compute_qref_and_fawa_first.f90
--rw-r--r--   0 claresyhuang   (501) staff       (20)     7231 2022-08-28 03:20:26.000000 hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/compute_reference_states.f90
--rw-r--r--   0 claresyhuang   (501) staff       (20)     6105 2022-08-28 03:20:26.000000 hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/interpolate_fields.f90
--rw-r--r--   0 claresyhuang   (501) staff       (20)     5625 2023-01-17 16:56:08.000000 hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/interpolate_fields_dirinv.f90
--rw-r--r--   0 claresyhuang   (501) staff       (20)      905 2022-08-28 03:20:26.000000 hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/matrix_after_inversion.f90
--rw-r--r--   0 claresyhuang   (501) staff       (20)     2353 2023-01-17 16:56:08.000000 hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/matrix_b4_inversion.f90
--rw-r--r--   0 claresyhuang   (501) staff       (20)     2288 2022-08-28 03:20:26.000000 hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/upward_sweep.f90
-drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-04-09 19:51:08.662719 hn2016_falwa-0.6.6/hn2016_falwa/legacy/
--rw-r--r--   0 claresyhuang   (501) staff       (20)        0 2021-08-14 20:06:09.000000 hn2016_falwa-0.6.6/hn2016_falwa/legacy/__init__.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)    20729 2021-08-14 20:06:33.000000 hn2016_falwa-0.6.6/hn2016_falwa/legacy/beta_version.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)    50300 2023-01-17 16:56:40.000000 hn2016_falwa-0.6.6/hn2016_falwa/oopinterface.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)     1161 2023-01-17 16:56:08.000000 hn2016_falwa-0.6.6/hn2016_falwa/plot_utilities.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)     3346 2022-08-30 03:28:00.000000 hn2016_falwa-0.6.6/hn2016_falwa/qgformalism.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)     9932 2022-08-28 04:25:37.000000 hn2016_falwa-0.6.6/hn2016_falwa/utilities.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)    23544 2022-08-28 04:25:29.000000 hn2016_falwa-0.6.6/hn2016_falwa/wrapper.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)    28059 2023-01-17 16:56:08.000000 hn2016_falwa-0.6.6/hn2016_falwa/xarrayinterface.py
-drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-04-09 19:51:08.561802 hn2016_falwa-0.6.6/hn2016_falwa.egg-info/
--rw-r--r--   0 claresyhuang   (501) staff       (20)     1320 2023-04-09 19:51:08.000000 hn2016_falwa-0.6.6/hn2016_falwa.egg-info/PKG-INFO
--rw-r--r--   0 claresyhuang   (501) staff       (20)     1214 2023-04-09 19:51:08.000000 hn2016_falwa-0.6.6/hn2016_falwa.egg-info/SOURCES.txt
--rw-r--r--   0 claresyhuang   (501) staff       (20)        1 2023-04-09 19:51:08.000000 hn2016_falwa-0.6.6/hn2016_falwa.egg-info/dependency_links.txt
--rw-r--r--   0 claresyhuang   (501) staff       (20)        1 2023-04-09 19:51:08.000000 hn2016_falwa-0.6.6/hn2016_falwa.egg-info/not-zip-safe
--rw-r--r--   0 claresyhuang   (501) staff       (20)       19 2023-04-09 19:51:08.000000 hn2016_falwa-0.6.6/hn2016_falwa.egg-info/requires.txt
--rw-r--r--   0 claresyhuang   (501) staff       (20)       19 2023-04-09 19:51:08.000000 hn2016_falwa-0.6.6/hn2016_falwa.egg-info/top_level.txt
--rw-r--r--   0 claresyhuang   (501) staff       (20)       38 2023-04-09 19:51:08.771025 hn2016_falwa-0.6.6/setup.cfg
--rw-r--r--   0 claresyhuang   (501) staff       (20)     3511 2023-04-09 19:49:59.000000 hn2016_falwa-0.6.6/setup.py
-drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-04-09 19:51:08.761498 hn2016_falwa-0.6.6/tests/
--rw-r--r--   0 claresyhuang   (501) staff       (20)        0 2020-03-01 18:39:03.000000 hn2016_falwa-0.6.6/tests/__init__.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)        1 2020-03-01 18:39:03.000000 hn2016_falwa-0.6.6/tests/conftest.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)     3839 2021-08-15 20:17:11.000000 hn2016_falwa-0.6.6/tests/test_barotropic_field.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)     2063 2020-03-01 18:39:03.000000 hn2016_falwa-0.6.6/tests/test_basis.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)    10170 2023-04-07 01:45:01.000000 hn2016_falwa-0.6.6/tests/test_oopinterface.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)     1167 2020-03-01 18:39:03.000000 hn2016_falwa-0.6.6/tests/test_utilities.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)     5643 2022-08-28 03:20:26.000000 hn2016_falwa-0.6.6/tests/test_xarrayinterface.py
+drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-06-19 03:13:28.580021 hn2016_falwa-0.7.0/
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     1065 2020-03-01 18:38:08.000000 hn2016_falwa-0.7.0/LICENSE.txt
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     1320 2023-06-19 03:13:28.579745 hn2016_falwa-0.7.0/PKG-INFO
+drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-06-19 03:13:28.361217 hn2016_falwa-0.7.0/hn2016_falwa/
+-rw-r--r--   0 claresyhuang   (501) staff       (20)      685 2023-06-19 02:58:19.000000 hn2016_falwa-0.7.0/hn2016_falwa/__init__.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     4912 2023-06-19 02:58:19.000000 hn2016_falwa-0.7.0/hn2016_falwa/barotropic_field.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     7483 2023-06-19 02:58:19.000000 hn2016_falwa-0.7.0/hn2016_falwa/basis.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)      336 2023-06-19 02:58:19.000000 hn2016_falwa-0.7.0/hn2016_falwa/constant.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)    10177 2023-06-19 02:58:19.000000 hn2016_falwa-0.7.0/hn2016_falwa/data_storage.py
+drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-06-19 03:13:28.482504 hn2016_falwa-0.7.0/hn2016_falwa/f90_modules/
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     6915 2023-06-19 02:58:19.000000 hn2016_falwa-0.7.0/hn2016_falwa/f90_modules/compute_flux_dirinv.f90
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     6915 2023-06-19 02:58:19.000000 hn2016_falwa-0.7.0/hn2016_falwa/f90_modules/compute_flux_dirinv_nshem.f90
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     5819 2023-06-10 16:30:20.000000 hn2016_falwa-0.7.0/hn2016_falwa/f90_modules/compute_lwa_and_barotropic_fluxes.f90
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     4592 2023-01-17 16:56:08.000000 hn2016_falwa-0.7.0/hn2016_falwa/f90_modules/compute_qref_and_fawa_first.f90
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     7231 2022-08-28 03:20:26.000000 hn2016_falwa-0.7.0/hn2016_falwa/f90_modules/compute_reference_states.f90
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     6105 2022-08-28 03:20:26.000000 hn2016_falwa-0.7.0/hn2016_falwa/f90_modules/interpolate_fields.f90
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     5625 2023-01-17 16:56:08.000000 hn2016_falwa-0.7.0/hn2016_falwa/f90_modules/interpolate_fields_dirinv.f90
+-rw-r--r--   0 claresyhuang   (501) staff       (20)      920 2023-06-19 02:58:19.000000 hn2016_falwa-0.7.0/hn2016_falwa/f90_modules/matrix_after_inversion.f90
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     2298 2023-06-19 02:58:19.000000 hn2016_falwa-0.7.0/hn2016_falwa/f90_modules/matrix_b4_inversion.f90
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     2288 2023-06-19 02:58:19.000000 hn2016_falwa-0.7.0/hn2016_falwa/f90_modules/upward_sweep.f90
+drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-06-19 03:13:28.483492 hn2016_falwa-0.7.0/hn2016_falwa/legacy/
+-rw-r--r--   0 claresyhuang   (501) staff       (20)        0 2021-08-14 20:06:09.000000 hn2016_falwa-0.7.0/hn2016_falwa/legacy/__init__.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)    20729 2021-08-14 20:06:33.000000 hn2016_falwa-0.7.0/hn2016_falwa/legacy/beta_version.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)    59143 2023-06-19 02:58:19.000000 hn2016_falwa-0.7.0/hn2016_falwa/oopinterface.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     3921 2023-06-19 02:58:19.000000 hn2016_falwa-0.7.0/hn2016_falwa/plot_utils.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     9932 2022-08-28 04:25:37.000000 hn2016_falwa-0.7.0/hn2016_falwa/utilities.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)    23366 2023-06-19 02:58:19.000000 hn2016_falwa-0.7.0/hn2016_falwa/wrapper.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)    26415 2023-06-19 02:58:19.000000 hn2016_falwa-0.7.0/hn2016_falwa/xarrayinterface.py
+drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-06-19 03:13:28.382618 hn2016_falwa-0.7.0/hn2016_falwa.egg-info/
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     1320 2023-06-19 03:13:28.000000 hn2016_falwa-0.7.0/hn2016_falwa.egg-info/PKG-INFO
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     1295 2023-06-19 03:13:28.000000 hn2016_falwa-0.7.0/hn2016_falwa.egg-info/SOURCES.txt
+-rw-r--r--   0 claresyhuang   (501) staff       (20)        1 2023-06-19 03:13:28.000000 hn2016_falwa-0.7.0/hn2016_falwa.egg-info/dependency_links.txt
+-rw-r--r--   0 claresyhuang   (501) staff       (20)        1 2023-04-09 19:51:08.000000 hn2016_falwa-0.7.0/hn2016_falwa.egg-info/not-zip-safe
+-rw-r--r--   0 claresyhuang   (501) staff       (20)       19 2023-06-19 03:13:28.000000 hn2016_falwa-0.7.0/hn2016_falwa.egg-info/requires.txt
+-rw-r--r--   0 claresyhuang   (501) staff       (20)       19 2023-06-19 03:13:28.000000 hn2016_falwa-0.7.0/hn2016_falwa.egg-info/top_level.txt
+-rw-r--r--   0 claresyhuang   (501) staff       (20)       38 2023-06-19 03:13:28.580105 hn2016_falwa-0.7.0/setup.cfg
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     3511 2023-06-19 02:58:19.000000 hn2016_falwa-0.7.0/setup.py
+drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-06-19 03:13:28.578339 hn2016_falwa-0.7.0/tests/
+-rw-r--r--   0 claresyhuang   (501) staff       (20)        0 2020-03-01 18:39:03.000000 hn2016_falwa-0.7.0/tests/__init__.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)        1 2020-03-01 18:39:03.000000 hn2016_falwa-0.7.0/tests/conftest.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     3839 2021-08-15 20:17:11.000000 hn2016_falwa-0.7.0/tests/test_barotropic_field.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     2081 2023-06-19 02:58:20.000000 hn2016_falwa-0.7.0/tests/test_basis.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)    13679 2023-06-19 02:58:20.000000 hn2016_falwa-0.7.0/tests/test_oopinterface.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     8782 2023-06-19 02:58:20.000000 hn2016_falwa-0.7.0/tests/test_output_results.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     1167 2020-03-01 18:39:03.000000 hn2016_falwa-0.7.0/tests/test_utilities.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     8113 2023-06-19 02:58:20.000000 hn2016_falwa-0.7.0/tests/test_xarrayinterface.py
```

### Comparing `hn2016_falwa-0.6.6/LICENSE.txt` & `hn2016_falwa-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.6/PKG-INFO` & `hn2016_falwa-0.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hn2016_falwa
-Version: 0.6.6
+Version: 0.7.0
 Summary: python package to compute finite-amplitude local wave activity (Huang and Nakamura 2016, JAS)
 Home-page: https://github.com/csyhuang/hn2016_falwa
 Author: Clare S. Y. Huang
 Author-email: csyhuang@uchicago.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `hn2016_falwa-0.6.6/hn2016_falwa/__init__.py` & `hn2016_falwa-0.7.0/hn2016_falwa/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 ------------------------------------------
 File name: __init__.py
 Author: Clare Huang, Christopher Polster
 """
 
-__version__ = "0.6.6"
+__version__ = "0.7.0"
 from .interpolate_fields import interpolate_fields
 from .interpolate_fields_direct_inv import interpolate_fields_direct_inv
 from .compute_qref_and_fawa_first import compute_qref_and_fawa_first
 from .matrix_b4_inversion import matrix_b4_inversion
 from .matrix_after_inversion import matrix_after_inversion
 from .upward_sweep import upward_sweep
 from .compute_reference_states import compute_reference_states
-from .compute_flux_dirinv import compute_flux_dirinv
+from .compute_flux_dirinv import compute_flux_dirinv_nshem
 from .compute_lwa_and_barotropic_fluxes import compute_lwa_and_barotropic_fluxes
```

### Comparing `hn2016_falwa-0.6.6/hn2016_falwa/barotropic_field.py` & `hn2016_falwa-0.7.0/hn2016_falwa/barotropic_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,18 @@
         dphi : np.array
             Differential length element along the lat grid with dimension = nlat.
 
         pv_field : np.ndarray
             Absolute vorticity field with dimension [nlat x nlon]. If 'pv_field=None': pv_field is expected to be computed with u,v,t field.
 
 
-    Example
-    ---------
+    Examples
+    --------
+    :doc:`Example Notebook <notebooks/Example_qgpv>`
+
     >>> barofield1 = BarotropicField(xlon, ylat, pv_field=abs_vorticity)
 
     """
 
     def __init__(self, xlon, ylat, pv_field, area=None, dphi=None,
                  n_partitions=None, planet_radius=6.378e+6):
 
@@ -94,17 +96,17 @@
         self._eqvlat = None
         self._lwa = None
 
     def _compute_eqvlat(self):
         """
         Private function. Compute equivalent latitude if it has not been computed yet.
         """
-        self.eqvlat, _ = basis.eqvlat(
+        self.eqvlat, _ = basis.eqvlat_fawa(
             self.ylat, self.pv_field, self.area, self.n_partitions,
-            planet_radius=self.planet_radius
+            planet_radius=self.planet_radius, output_fawa=False
         )
         return self.eqvlat
 
     def _compute_lwa(self):
         """
         Private function. Compute equivalent latitude if it has not been computed yet.
         """
```

### Comparing `hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/compute_flux_dirinv.f90` & `hn2016_falwa-0.7.0/hn2016_falwa/f90_modules/compute_flux_dirinv.f90`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-SUBROUTINE compute_flux_dirinv(pv,uu,vv,pt,tn0,qref,uref,tref,&
-        imax, JMAX, kmax, nd, jb, jd, &
+SUBROUTINE compute_flux_dirinv_nshem(pv,uu,vv,pt,tn0,qref,uref,tref,&
+        imax, JMAX, kmax, nd, jb, jd, is_nhem, &
         a, om, dz, h, rr, cp, prefac,&
         astarbaro,ubaro,urefbaro,ua1baro,ua2baro,ep1baro,ep2baro,ep3baro,ep4,astar1,astar2)
 
-  INTEGER, INTENT(IN) :: imax, JMAX, kmax, nd, jb, jd
   REAL, INTENT(IN) :: pv(imax,jmax,kmax),uu(imax,jmax,kmax),vv(imax,jmax,kmax),pt(imax,jmax,kmax),&
           tn0(kmax),qref(nd,kmax),uref(jd,kmax),tref(jd,kmax)
+  INTEGER, INTENT(IN) :: imax, JMAX, kmax, nd, jb, jd
+  LOGICAL, INTENT(IN) :: is_nhem
   REAL, INTENT(IN) :: a, om, dz, h, rr, cp, prefac
   REAL, INTENT(OUT) :: astarbaro(imax,nd),ubaro(imax,nd),urefbaro(nd),ua1baro(imax,nd),ua2baro(imax,nd),&
           ep1baro(imax,nd),ep2baro(imax,nd),ep3baro(imax,nd),ep4(imax,nd),astar1(imax,nd,kmax),astar2(imax,nd,kmax)
 
   REAL :: tg(kmax)
   REAL :: ua1(imax,nd),ua2(imax,nd),ep1(imax,nd)
   REAL :: ep2(imax,nd),ep3(imax,nd)
   REAL :: qe(imax,nd),ue(imax,nd)
   REAL :: z(kmax)
+  INTEGER :: jstart, jend
 
   !a = 6378000.
   pi = acos(-1.)
   !om = 7.29e-5
   dp = pi/float(jmax-1)
   !dz = 500.
   !h = 7000.
@@ -47,69 +49,117 @@
   ua2baro(:,:) = 0.
   ep1baro(:,:) = 0.
   ep2baro(:,:) = 0.
   ep3baro(:,:) = 0.
   ep4(:,:) = 0.
   dc = dz/prefac
 
+  ! Bounds of y-indices in N/SHem
+  if (is_nhem) then  ! 5N and higher latitude
+    jstart = jb+1  ! 6
+    jend = nd-1
+  else
+    jstart = 2
+    jend = nd-jb   ! nd - 5
+  endif
+
   do k = 2,kmax-1
     zk = dz*float(k-1)
     do i = 1,imax
-      do j = jb+1,nd-1            ! 5N and higher latitude
+      do j = jstart, jend
         astar1(i,j,k) = 0.       ! LWA*cos(phi)
         astar2(i,j,k) = 0.       ! LWA*cos(phi)
         ua2(i,j) = 0.          !F2
-        phi0 = dp*float(j-1)           !latitude
+        if (is_nhem) then        !latitude
+          phi0 = dp*float(j-1)
+        else
+          phi0 = dp*float(j-1)-0.5*pi
+        endif
         cor = 2.*om*sin(phi0)          !Coriolis parameter
         do jj = 1,nd
-          phi1 = dp*float(jj-1)
-          qe(i,jj) = pv(i,jj+nd-1,k)-qref(j,k)   !qe; Q = qref
-          ue(i,jj) = uu(i,jj+nd-1,k)-uref(j-jb,k)   !ue; shift uref 5N
+          if (is_nhem) then
+            phi1 = dp*float(jj-1)
+            qe(i,jj) = pv(i,jj+nd-1,k)-qref(j,k)    !qe; Q = qref
+            ue(i,jj) = uu(i,jj+nd-1,k)-uref(j-jb,k) !ue; shift uref 5N
+          else
+            phi1 = dp*float(jj-1)-0.5*pi
+            qe(i,jj) = pv(i,jj,k)-qref(j,k)     !qe; Q = qref
+            ue(i,jj) = uu(i,jj,k)-uref(j-jb,k)  !ue;
+          endif
           aa = a*dp*cos(phi1)                      !length element
           if((qe(i,jj).le.0.).and.(jj.ge.j)) then  !LWA*cos and F2
-            astar2(i,j,k)=astar2(i,j,k)-qe(i,jj)*aa  !anticyclonic
+            if (is_nhem) then
+              astar2(i,j,k)=astar2(i,j,k)-qe(i,jj)*aa  !anticyclonic
+            else
+              astar1(i,j,k)=astar1(i,j,k)-qe(i,jj)*aa  !cyclonic
+            endif
             ua2(i,j) = ua2(i,j)-qe(i,jj)*ue(i,jj)*aa
           endif
           if((qe(i,jj).gt.0.).and.(jj.lt.j)) then
-            astar1(i,j,k)=astar1(i,j,k)+qe(i,jj)*aa  !cyclonic
+            if (is_nhem) then
+              astar1(i,j,k)=astar1(i,j,k)+qe(i,jj)*aa  !cyclonic
+            else
+              astar2(i,j,k)=astar2(i,j,k)+qe(i,jj)*aa  !anticyclonic
+            endif
             ua2(i,j) = ua2(i,j)+qe(i,jj)*ue(i,jj)*aa
           endif
         enddo
 
         !  ******** Other fluxes ******
-
-        ua1(i,j) = uref(j-jb,k)*(astar1(i,j,k) +  &
-        astar2(i,j,k))            !F1
-        ep1(i,j) = -0.5*(uu(i,j+nd-1,k)-uref(j-jb,k))**2  !F3a
-        ep1(i,j) = ep1(i,j)+0.5*vv(i,j+nd-1,k)**2    !F3a+b
-        ep11 = 0.5*(pt(i,j+nd-1,k)-tref(j-jb,k))**2         !F3c
+        if (is_nhem) then
+          ua1(i,j) = uref(j-jb,k)*(astar1(i,j,k) + astar2(i,j,k))  !F1
+          ep1(i,j) = -0.5*(uu(i,j+nd-1,k)-uref(j-jb,k))**2         !F3a
+          ep1(i,j) = ep1(i,j)+0.5*vv(i,j+nd-1,k)**2                !F3a+b
+          ep11 = 0.5*(pt(i,j+nd-1,k)-tref(j-jb,k))**2              !F3c
+        else
+          ua1(i,j) = uref(j,k)*(astar1(i,j,k) + astar2(i,j,k))     !F1
+          ep1(i,j) = -0.5*(uu(i,j,k)-uref(j,k))**2                 !F3a
+          ep1(i,j) = ep1(i,j)+0.5*vv(i,j,k)**2                     !F3a+b
+          ep11 = 0.5*(pt(i,j,k)-tref(j,k))**2               !F3c
+        endif
         zz = dz*float(k-1)
         ep11 = ep11*(rr/h)*exp(-rkappa*zz/h)
         ep11 = ep11*2.*dz/(tg(k+1)-tg(k-1))
         ep1(i,j) = ep1(i,j)-ep11                   !F3
-        phip = dp*float(j)
-        phi0 = dp*float(j-1)
-        phim = dp*float(j-2)
+        if (is_nhem) then
+          phip = dp*float(j)
+          phi0 = dp*float(j-1)
+          phim = dp*float(j-2)
+        else
+          phip = dp*float(j) - 0.5*pi
+          phi0 = dp*float(j-1) - 0.5*pi
+          phim = dp*float(j-2) - 0.5*pi
+        endif
         cosp = cos(phip)          ! cosine for one grid north
         cos0 = cos(phi0)          ! cosine for latitude grid
         cosm = cos(phim)          ! cosine for one grid south
         sin0 = sin(phi0)          ! sine for latitude grid
         ep1(i,j) = ep1(i,j)*cos0 ! correct for cosine factor
 
 
         ! meridional eddy momentum flux one grid north and south
-        ep2(i,j) = (uu(i,j+nd,k)-uref(j-jb+1,k))*cosp*cosp * vv(i,j+nd,k)
-        ep3(i,j) = (uu(i,j+nd-2,k)-uref(j-jb-1,k))*cosm*cosm * vv(i,j+nd-2,k)
+        if (is_nhem) then
+          ep2(i,j) = (uu(i,j+nd,k)-uref(j-jb+1,k))*cosp*cosp * vv(i,j+nd,k)
+          ep3(i,j) = (uu(i,j+nd-2,k)-uref(j-jb-1,k))*cosm*cosm * vv(i,j+nd-2,k)
+        else
+          ! TODO: double check.
+          ep2(i,j) = (uu(i,j+1,k)-uref(j+1,k))*cosp*cosp * vv(i,j+1,k)
+          ep3(i,j) = (uu(i,j-1,k)-uref(j-1,k))*cosm*cosm * vv(i,j-1,k)
+        endif
 
         ! low-level meridional eddy heat flux
         if(k.eq.2) then     ! (26) of SI-HN17
           ep41 = 2.*om*sin0*cos0*dz/prefac       ! prefactor
-          ep42 = exp(-dz/h)*vv(i,j+nd-1,2)*(pt(i,j+nd-1,2)-tref(j-jb,2))
-          ep42 = ep42/(tg(3)-tg(1))
-          ep43 = vv(i,j+nd-1,1)*(pt(i,j+nd-1,1)-tref(j-jb,1))
+          if (is_nhem) then
+            ep42 = exp(-dz/h)*vv(i,j+nd-1,2)*(pt(i,j+nd-1,2)-tref(j-jb,2))/(tg(3)-tg(1))
+            ep43 = vv(i,j+nd-1,1)*(pt(i,j+nd-1,1)-tref(j-jb,1))
+          else
+            ep42 = exp(-dz/h)*vv(i,j,2)*(pt(i,j,2)-tref(j,2))/(tg(3)-tg(1))
+            ep43 = vv(i,j,1)*(pt(i,j,1)-tref(j,1))
+          endif
           ep43 = 0.5*ep43/(tg(2)-tg(1))
           ep4(i,j) = ep41*(ep42+ep43)   ! low-level heat flux
         endif
       enddo
       phip = dp*jb
       phi0 = dp*(jb-1)
       cosp = cos(phip)          ! cosine for one grid north
@@ -123,14 +173,24 @@
     astarbaro(:,:) = astarbaro(:,:)+(astar1(:,:,k)    &
     + astar2(:,:,k))*exp(-zk/h)*dc
     ua1baro(:,:) = ua1baro(:,:)+ua1(:,:)*exp(-zk/h)*dc
     ua2baro(:,:) = ua2baro(:,:)+ua2(:,:)*exp(-zk/h)*dc
     ep1baro(:,:) = ep1baro(:,:)+ep1(:,:)*exp(-zk/h)*dc
     ep2baro(:,:) = ep2baro(:,:)+ep2(:,:)*exp(-zk/h)*dc
     ep3baro(:,:) = ep3baro(:,:)+ep3(:,:)*exp(-zk/h)*dc
-    do j = jb+1,nd  ! ### yet to be multiplied by cosine
+
+    ! Bounds of y-indices in N/SHem
+    if (is_nhem) then  ! 5N and higher latitude
+      jstart = jb+1  ! 6
+      jend = nd
+    else
+      jstart = 1
+      jend = nd-jb   ! nd - 5
+    endif
+
+    do j = jstart,jend  ! ### yet to be multiplied by cosine
       ubaro(:,j) = ubaro(:,j)+uu(:,j+nd-1,k)*exp(-zk/h)*dc
       urefbaro(j) = urefbaro(j)+uref(j-jb,k)*exp(-zk/h)*dc
     enddo
   enddo
 
 END SUBROUTINE
```

### Comparing `hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/compute_lwa_and_barotropic_fluxes.f90` & `hn2016_falwa-0.7.0/hn2016_falwa/f90_modules/compute_lwa_and_barotropic_fluxes.f90`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/compute_qref_and_fawa_first.f90` & `hn2016_falwa-0.7.0/hn2016_falwa/f90_modules/compute_qref_and_fawa_first.f90`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/compute_reference_states.f90` & `hn2016_falwa-0.7.0/hn2016_falwa/f90_modules/compute_reference_states.f90`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/interpolate_fields.f90` & `hn2016_falwa-0.7.0/hn2016_falwa/f90_modules/interpolate_fields.f90`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/interpolate_fields_dirinv.f90` & `hn2016_falwa-0.7.0/hn2016_falwa/f90_modules/interpolate_fields_dirinv.f90`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/matrix_after_inversion.f90` & `hn2016_falwa-0.7.0/hn2016_falwa/f90_modules/matrix_after_inversion.f90`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-SUBROUTINE matrix_after_inversion(k,kmax,jd,qjj,djj,cjj,tj,rj,sjk,tjk)
+SUBROUTINE matrix_after_inversion(k,kmax,jd,qjj,djj,cjj,rj,sjk,tjk)
 
   INTEGER, INTENT(in) :: k, kmax, jd
   REAL, INTENT(in) :: qjj(jd-2,jd-2),djj(jd-2,jd-2),cjj(jd-2,jd-2),rj(jd-2)
-  REAL, INTENT(INOUT) :: sjk(jd-2,jd-2,kmax-1),tjk(jd-2,kmax-1),tj(jd-2)  ! Note that tj is not used in subsequent modules
+  REAL, INTENT(INOUT) :: sjk(jd-2,jd-2,kmax-1),tjk(jd-2,kmax-1)  ! Note that tj is not used in subsequent modules
 
   integer :: i, j
-  real :: xjj(jd-2,jd-2),yj(jd-2)
-
+  real :: xjj(jd-2,jd-2),yj(jd-2),tj(jd-2)
 
+  tj(:) = tjk(:,k)
   do i = 1,jd-2
     do j = 1,jd-2
     xjj(i,j) = 0.
     do kk = 1,jd-2
       xjj(i,j) = xjj(i,j)+qjj(i,kk)*djj(kk,j)
     enddo
     sjk(i,j,k-1) = -xjj(i,j)
```

### Comparing `hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/matrix_b4_inversion.f90` & `hn2016_falwa-0.7.0/hn2016_falwa/f90_modules/matrix_b4_inversion.f90`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-SUBROUTINE matrix_b4_inversion(k,jmax,kmax,nd,jb,jd,z,statn,qref,ckref,&
+SUBROUTINE matrix_b4_inversion(k,jmax,kmax,nd,jb,jd,z,statn,qref,ckref,sjk,&
         a, om, dz, h, rr, cp, &
-        qjj,djj,cjj,rj,tj,sjk,tjk)
+        qjj,djj,cjj,rj)
 
   integer, INTENT(in) :: k, jmax, kmax, nd, jb, jd
   REAL, INTENT(in) :: z(kmax),statn(kmax),qref(nd,kmax),ckref(nd,kmax)
+  REAL, INTENT(IN) :: sjk(jd-2,jd-2,kmax-1)
   REAL, INTENT(in) :: a, om, dz, h, rr, cp
-  REAL, INTENT(OUT) :: qjj(jd-2,jd-2),djj(jd-2,jd-2),cjj(jd-2,jd-2),rj(jd-2),tj(jd-2)
-  REAL, INTENT(INOUT) :: sjk(jd-2,jd-2,kmax-1),tjk(jd-2,kmax-1)
+  REAL, INTENT(OUT) :: qjj(jd-2,jd-2),djj(jd-2,jd-2),cjj(jd-2,jd-2),rj(jd-2)
   REAL :: xjj(jd-2,jd-2), u(jd,kmax)
   REAL :: sjj(jd-2,jd-2)
 
   rkappa = rr/cp
   pi = acos(-1.)
   dp = pi/float(jmax-1)
 
@@ -18,15 +18,14 @@
   zm = 0.5*(z(k-1)+z(k))
   statp = 0.5*(statn(k+1)+statn(k))
   statm = 0.5*(statn(k-1)+statn(k))
   cjj(:,:) = 0.
   djj(:,:) = 0.
   qjj(:,:) = 0.
   sjj(:,:) = sjk(:,:,k)
-  tj(:) = tjk(:,k)
   do jj = jb+2,(nd-1)
     j = jj - jb
     phi0 = float(jj-1)*dp
     phip = (float(jj)-0.5)*dp
     phim = (float(jj)-1.5)*dp
     cos0 = cos(phi0)
     cosp = cos(phip)
```

### Comparing `hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/upward_sweep.f90` & `hn2016_falwa-0.7.0/hn2016_falwa/f90_modules/upward_sweep.f90`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
   ! *** Corner boundary conditions ***
   u(1,1) = 0.
   u(jd,1) = 0.
   !        u(1,kmax) = ubar(1+jb,kmax)*cos(dp*float(jb))
   u(1,kmax) = ckref(1+jb,kmax)/(2.*pi*a)-om*a*cos(dp*float(jb))
   u(jd,kmax) = 0.
 
-  ! *** Divide by cos phi to revover Uref ****
+  ! *** Divide by cos phi to recover Uref ****
   do jj = jb+1,nd-1
     j = jj-jb
     phi0 = dp*float(jj-1)
     u(j,:) = u(j,:)/cos(phi0)
   enddo
   u(jd,:) = 2.*u(jd-1,:)-u(jd-2,:)
```

### Comparing `hn2016_falwa-0.6.6/hn2016_falwa/legacy/beta_version.py` & `hn2016_falwa-0.7.0/hn2016_falwa/legacy/beta_version.py`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.6/hn2016_falwa/oopinterface.py` & `hn2016_falwa-0.7.0/hn2016_falwa/oopinterface.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 """
 ------------------------------------------
 File name: oopinterface.py
 Author: Clare Huang
 """
-from typing import Optional
+from typing import Tuple, Optional, Union, NamedTuple
+from abc import ABC, abstractmethod
 import math
 import warnings
 import numpy as np
 from scipy.interpolate import interp1d
 from scipy.linalg.lapack import dgetrf, dgetri
 
 from hn2016_falwa import utilities
 from hn2016_falwa.constant import P_GROUND, SCALE_HEIGHT, CP, DRY_GAS_CONSTANT, EARTH_RADIUS, EARTH_OMEGA
+from hn2016_falwa.data_storage import InterpolatedFieldsStorage, DomainAverageStorage, ReferenceStatesStorage, \
+    LWAStorage, BarotropicFluxTermsStorage, OutputBarotropicFluxTermsStorage
 
+# *** Import f2py modules ***
 from hn2016_falwa import interpolate_fields, interpolate_fields_direct_inv, compute_qref_and_fawa_first,\
-    matrix_b4_inversion, matrix_after_inversion, upward_sweep, compute_flux_dirinv, compute_reference_states,\
+    matrix_b4_inversion, matrix_after_inversion, upward_sweep, compute_flux_dirinv_nshem, compute_reference_states,\
     compute_lwa_and_barotropic_fluxes
 from collections import namedtuple
 
 
-class QGField(object):
+class QGFieldBase(ABC):
 
     """
-    Local wave activity and flux analysis in quasi-geostrophic framework
-    that can be used to reproduce the results in:
-    Nakamura and Huang, Atmospheric Blocking as a Traffic Jam in the Jet Stream, Science (2018).
-    Note that topography is assumed flat in this object.
+    Local wave activity and flux analysis in the quasi-geostrophic framework.
+
+    .. warning::
+        This is an abstract class that defines the public interface but does
+        not define any boundary conditions for the reference state computation.
+        Instanciate via the specific child classes :py:class:`QGFieldNH18` or
+        :py:class:`QGFieldNHN22` to select the desired boundary conditions.
+
+    Topography is assumed flat in this object.
 
     .. versionadded:: 0.3.0
 
     Parameters
     ----------
     xlon : numpy.array
            Array of evenly-spaced longitude (in degree) of size nlon.
@@ -67,28 +76,21 @@
     dry_gas_constant : float, optional
            Gas constant for dry air in J/kg-K. Default = 287.
     omega : float, optional
            Rotation rate of the earth in 1/s. Default = 7.29e-5.
     planet_radius : float, optional
            Radius of the planet in meters.
            Default = 6.378e+6 (Earth's radius).
-    eq_boundary_index: int, optional
-           The improved inversion algorithm of reference states allow modification of equatorward boundary
-           to be the absolute vorticity. This parameter specify the location of grid point (from equator)
-           which will be used as boundary. Default = 5.
-
-    Examples
-    --------
-    >>> test_object = QGField(xlon, ylat, plev, u_field, v_field, t_field)
-
+    northern_hemisphere_results_only : bool, optional
+           whether only to return northern hemispheric results. Default = False
     """
 
     def __init__(self, xlon, ylat, plev, u_field, v_field, t_field, kmax=49, maxit=100000, dz=1000., npart=None,
                  tol=1.e-5, rjac=0.95, scale_height=SCALE_HEIGHT, cp=CP, dry_gas_constant=DRY_GAS_CONSTANT,
-                 omega=EARTH_OMEGA, planet_radius=EARTH_RADIUS, prefactor=None, eq_boundary_index=5):
+                 omega=EARTH_OMEGA, planet_radius=EARTH_RADIUS, northern_hemisphere_results_only=False):
 
         """
         Create a QGField object.
         This only initialize the attributes of the object. Analysis and
         computation are done by calling various methods.
         """
 
@@ -144,90 +146,87 @@
             self.v_field = interp_v(self.ylat)
             self.t_field = interp_t(self.ylat)
         else:
             self.u_field = u_field
             self.v_field = v_field
             self.t_field = t_field
 
-        # === To be computed ===
+        # === Coordinate-related ===
         self.dphi = np.deg2rad(180./(self.nlat-1))
         self.dlambda = np.deg2rad(self.xlon[1] - self.xlon[0])
-
-        if npart is None:
-            self.npart = self.nlat
-        else:
-            self.npart = npart
+        self.slat = np.sin(np.deg2rad(ylat))  # sin latitude
+        self.clat = np.cos(np.deg2rad(ylat))  # sin latitude
+        self.npart = npart if npart is not None else self.nlat
+        self.kmax = kmax
         self.height = np.array([i * dz for i in range(kmax)])
 
-        # === Parameters ===
-        self.kmax = kmax
+        # === Moved here in v0.7.0 ===
+        self._northern_hemisphere_results_only = northern_hemisphere_results_only
+
+        # === Other parameters ===
         self.maxit = maxit
         self.dz = dz
         self.tol = tol
         self.rjac = rjac
-        self.eq_boundary_index = eq_boundary_index
 
         # === Constants ===
         self.scale_height = scale_height
         self.cp = cp
         self.dry_gas_constant = dry_gas_constant
         self.omega = omega
         self.planet_radius = planet_radius
         self._compute_prefactor()  # Compute normalization prefactor
 
-        # Modification on Oct 19, 2021 - deprecation of prefactor (it should be computed from kmax and dz)
-        if prefactor is not None:
-            warnings.warn(
-                "The optional input prefactor will be deprecated since it can be determined directly from " +
-                "kmax and dz. Given your input kmax = {kmax} and dz = {dz}, ".format(kmax=self.kmax, dz=self.dz) +
-                "the computed normalization prefactor is {prefactor}. ".format(prefactor=self.prefactor) +
-                "Your input value {input} would be ignored.".format(input=prefactor))
-
-        # === Variables that will be computed in methods ===
-        self._qgpv_temp = None
-        self._interpolated_u_temp = None
-        self._interpolated_v_temp = None
-        self._interpolated_avort_temp = None
-        self._interpolated_theta_temp = None
-        self._static_stability = None
-        self._static_stability_n = None
-        self._static_stability_s = None
-        self._tn0 = None
-        self._ts0 = None
-
-        # === Temporary solution for direct inv routine
-        self._f_qref, self._f_u, self._f_tref, self._f_ubar, self._f_tbar, self._f_fawa, self._f_ckref = \
-            None, None, None, None, None, None, None
-
-        # Computation from computer_reference_states
-        self._qref_stemp = None
-        self._uref_stemp = None
-        self._ptref_stemp = None
-        self._qref_ntemp = None
-        self._uref_ntemp = None
-        self._ptref_ntemp = None
-        self._qref = None
-        self._uref = None
-        self._ptref = None
-        self._qgpv = None
-        self._interpolated_u = None
-        self._interpolated_v = None
-        self._interpolated_theta = None
-        self._northern_hemisphere_results_only: Optional[bool] = None  # Leave it uninitialized first.
-
-        # Computation from compute_lwa_and_barotropic_fluxes
-        self._adv_flux_f1 = None
-        self._adv_flux_f2 = None
-        self._adv_flux_f3 = None
-        self._convergence_zonal_advective_flux = None
-        self._meridional_heat_flux = None
-        self._lwa_baro = None
-        self._u_baro = None
-        self._lwa = None
-        self._divergence_eddy_momentum_flux = None
+        # === qgpv, u, v, avort, theta encapsulated in InterpolatedFieldsStorage ===
+        self._interpolated_field_storage = InterpolatedFieldsStorage(
+            pydim=(self.kmax, self.nlat, self.nlon),
+            fdim=(self.nlon, self.nlat, self.kmax),
+            swapaxis_1=0,
+            swapaxis_2=2,
+            northern_hemisphere_results_only=self.northern_hemisphere_results_only)
+        # Global averaged quantities (TODO: encalsulate them later)
+        self._domain_average_storage = DomainAverageStorage(
+            pydim=self.kmax,
+            fdim=self.kmax,
+            swapaxis_1=0,
+            swapaxis_2=2,
+            northern_hemisphere_results_only=self.northern_hemisphere_results_only)
+
+        # Reference states
+        lat_dim = self.nlat // 2 + 1 if self.northern_hemisphere_results_only else self.nlat
+        self._reference_states_storage = ReferenceStatesStorage(
+            pydim=(self.kmax, lat_dim),
+            fdim=(lat_dim, self.kmax),
+            swapaxis_1=0,
+            swapaxis_2=1,
+            northern_hemisphere_results_only=self.northern_hemisphere_results_only)
+
+        # LWA storage (3D)
+        self._lwa_storage = LWAStorage(
+            pydim=(self.kmax, lat_dim, self.nlon),
+            fdim=(self.nlon, lat_dim, self.kmax),
+            swapaxis_1=0,
+            swapaxis_2=2,
+            northern_hemisphere_results_only=self.northern_hemisphere_results_only)
+
+        # barotropic flux term storage (2D)
+        self._barotropic_flux_terms_storage = BarotropicFluxTermsStorage(
+            pydim=(lat_dim, self.nlon),
+            fdim=(self.nlon, lat_dim),
+            swapaxis_1=0,
+            swapaxis_2=1,
+            northern_hemisphere_results_only=self.northern_hemisphere_results_only)
+
+        # output barotropic flux term storage (2D)
+        self._output_barotropic_flux_terms_storage = OutputBarotropicFluxTermsStorage(
+            pydim=(lat_dim, self.nlon),
+            fdim=(self.nlon, lat_dim),
+            swapaxis_1=0,
+            swapaxis_2=1,
+            northern_hemisphere_results_only=self.northern_hemisphere_results_only)
 
         # Temporary solution for GRL computation
         self._ua1baro_nhem = None
         self._ua2baro_nhem = None
         self._ep1baro_nhem = None
         self._ep2baro_nhem = None
         self._ep3baro_nhem = None
@@ -238,18 +237,14 @@
         Private function. Compute prefactor for normalization by evaluating
             int^{z=kmax*dz}_0 e^{-z/H} dz
         using rectangular rule consistent with the integral evaluation in compute_lwa_and_barotropic_fluxes.f90.
         TODO: evaluate numerical integration scheme used in the fortran module.
         """
         self._prefactor = sum([math.exp(-k * self.dz / self.scale_height) * self.dz for k in range(1, self.kmax-1)])
 
-    @property
-    def prefactor(self):
-        return self._prefactor
-
     def _check_valid_plev(self, plev, scale_height, kmax, dz):
         """
         Private function. Check the validity of plev to see
             1. if plev is in decending order
             2. if kmax is valid given the max pseudoheight in the input data
 
         Parameters
@@ -262,16 +257,16 @@
                Dimension of uniform pseudoheight grids used for interpolation.
         dz : float, optional
                Size of uniform pseudoheight grids (in meters).
         """
         # Check if plev is in decending order
         if np.diff(plev)[0] > 0:
             raise TypeError("plev must be in decending order (i.e. from ground level to aloft)")
-        else:
-            self.plev = plev
+        self.plev = plev
+        self.zlev = -scale_height * np.log(plev/P_GROUND)
 
         # Check if kmax is valid given the max pseudoheight in the input data
         hmax = -scale_height*np.log(plev[-1]/P_GROUND)
         if hmax < (kmax-1) * dz:
             raise ValueError('Input kmax = {} but the maximum valid kmax'.format(kmax) +
                              '(constrainted by the vertical grid of your input data) is {}'.format(int(hmax//dz)+1))
 
@@ -328,15 +323,15 @@
             raise TypeError("No need for such interpolation.")
         else:
             return interp1d(
                 interp_from, field, axis=which_axis, bounds_error=False,
                 fill_value='extrapolate'
             )(interp_to)
 
-    def _return_interp_variables(self, variable, interp_axis, northern_hemisphere_results_only=True):
+    def _return_interp_variables(self, variable, interp_axis):
         """
         Private function to return interpolated variables from odd grid back to even grid if originally
         the data was given on an odd grid.
 
         Parameters
         ----------
             variable(numpy.ndarray): the variable to be interpolated
@@ -347,80 +342,46 @@
                 Will be deprecated in upcoming release.
 
         Returns
         -------
             The interpolated variable(numpy.ndarray)
         """
         if self.need_latitude_interpolation:
-            if northern_hemisphere_results_only:
+            if self.northern_hemisphere_results_only:
                 return self._interp_back(
                     variable, self.ylat[-(self.nlat//2+1):],
                     self.ylat_no_equator[-(self.nlat//2):],
                     which_axis=interp_axis)
             else:
                 return self._interp_back(variable, self.ylat, self.ylat_no_equator, which_axis=interp_axis)
         else:
             return variable
 
-    def _compute_reference_state_wrapper(self, qgpv, u, theta):
-        """
-        Private function to call the fortran subroutine compute_reference_states that returns variable of
-        dimension [nlat, kmax]. Swapping of axes is needed for other computation.
-
-        Parameters
-        ----------
-            qgpv(numpy.ndarray): QGPV
-
-            u(numpy.ndarray): 3D zonal wind
-
-            theta(numpy.ndarray): 3D potential temperature
-
-            num_of_iter(int): number of iteration when solving the eliptic equation
-
-        Returns
-        -------
-            Qref(numpy.ndarray): Reference state of QGPV of dimension [nlat, kmax]
-
-            Uref(numpy.ndarray): Reference state of zonal wind of dimension [nlat, kmax]
-
-            PTref(numpy.ndarray): Reference state of potential temperature of dimension [nlat, kmax]
-        """
-        return compute_reference_states(
-            qgpv,
-            u,
-            theta,
-            self._static_stability,
-            self.equator_idx,
-            self.npart,
-            self.maxit,
-            self.planet_radius,
-            self.omega,
-            self.dz,
-            self.tol,
-            self.scale_height,
-            self.dry_gas_constant,
-            self.cp,
-            self.rjac,
-        )
-
     def _compute_lwa_and_barotropic_fluxes_wrapper(self, qgpv, u, v, theta, qref_temp, uref_temp, ptref_temp):
         """
         Private function. Wrapper to call the fortran subroutine compute_lwa_and_barotropic_fluxes.
         """
         return compute_lwa_and_barotropic_fluxes(
             qgpv, u, v, theta, qref_temp, uref_temp, ptref_temp,
             self.planet_radius, self.omega, self.dz, self.scale_height, self.dry_gas_constant, self.cp, self.prefactor)
 
-    def interpolate_fields(self):
+    def interpolate_fields(self, return_named_tuple: bool = True) -> Optional[NamedTuple]:
 
         """
         Interpolate zonal wind, maridional wind, and potential temperature field onto the uniform pseudoheight grids,
         and compute QGPV on the same grids. This returns named tuple called "Interpolated_fields" that consists of
         5 elements as listed below.
 
+        Parameters
+        ----------
+        return_named_tuple : bool
+           Whether to returned a named tuple with variables in python indexing. Default: True. If False, nothing will be
+           returned from this method. The variables can be retrieved from the QGField object after all computation is
+           finished. This may save run time in some use case.
+
         Returns
         -------
         QGPV : numpy.ndarray
             Three-dimensional array of quasi-geostrophic potential vorticity (QGPV) with dimension = [kmax, nlat, nlon]
 
         U : numpy.ndarray
             Three-dimensional array of interpolated zonal wind with dimension = [kmax, nlat, nlon]
@@ -439,68 +400,45 @@
         --------
 
         >>> interpolated_fields = test_object.interpolate_fields()
         >>> interpolated_fields.QGPV  # This is to access the QGPV field
 
         """
 
-        if self._qref_ntemp is None:
+        # Return a named tuple
+        Interpolated_fields_to_return = namedtuple(
+            'Interpolated_fields', ['QGPV', 'U', 'V', 'Theta', 'Static_stability'])
 
-            # === Interpolate fields and obtain qgpv ===
-            self._qgpv_temp, \
-                self._interpolated_u_temp, \
-                self._interpolated_v_temp, \
-                self._interpolated_avort_temp, \
-                self._interpolated_theta_temp, \
-                self._static_stability = \
-                interpolate_fields(
-                    np.swapaxes(self.u_field, 0, 2),
-                    np.swapaxes(self.v_field, 0, 2),
-                    np.swapaxes(self.t_field, 0, 2),
-                    self.plev,
-                    self.height,
-                    self.planet_radius,
-                    self.omega,
-                    self.dz,
-                    self.scale_height,
-                    self.dry_gas_constant,
-                    self.cp
-                )
-
-            self._qgpv = np.swapaxes(self._qgpv_temp, 0, 2)
-            self._interpolated_u = np.swapaxes(self._interpolated_u_temp, 0, 2)
-            self._interpolated_v = np.swapaxes(self._interpolated_v_temp, 0, 2)
-            self._interpolated_theta = np.swapaxes(
-                self._interpolated_theta_temp, 0, 2
-            )
+        interpolated_fields_tuple = self._interpolate_fields(Interpolated_fields_to_return, return_named_tuple)
+
+        # TODO: warn that for NHN22, static stability returned would be a tuple of ndarray
+        if return_named_tuple:
+            return interpolated_fields_tuple
 
-        # Construct a named tuple # TODO: add absolute vorticity here? But only after testing
-        Interpolated_fields = namedtuple('Interpolated_fields', ['QGPV', 'U', 'V', 'Theta', 'Static_stability'])
-        interpolated_fields = Interpolated_fields(
-            self.qgpv,
-            self.interpolated_u,
-            self.interpolated_v,
-            self.interpolated_theta,
-            self.static_stability)
-        return interpolated_fields
+    @abstractmethod
+    def _interpolate_fields(self, Interpolated_fields_to_return: NamedTuple, return_named_tuple: bool) -> Optional[NamedTuple]:
+        """
+        The specific interpolation procedures w.r.t the particular procedures in the paper will be implemented here.
+        """
 
-    def compute_reference_states(self, northern_hemisphere_results_only=False):
+    def compute_reference_states(self, return_named_tuple: bool = True, northern_hemisphere_results_only=None) -> Optional[NamedTuple]:
 
         """
         Compute the local wave activity and reference states of QGPV, zonal wind and potential temperature using a more
         stable inversion algorithm applied in Nakamura and Huang (2018, Science). The equation to be invert is
         equation (22) in supplementary materials of Huang and Nakamura (2017, GRL).
 
-        This function returns named tuple called "Reference_states" that consists of 3 elements:
+        The parameter `northern_hemisphere_results_only` is deprecated and has no effect.
 
         Parameters
         ----------
-        northern_hemisphere_results_only : bool
-           If true, arrays of size [kmax, nlat//2+1] will be returned. Otherwise, arrays of size [kmax, nlat] will be
-           returned. Default: False.
+        return_named_tuple : bool
+           Whether to returned a named tuple with variables in python indexing. Default: True. If False, nothing will be
+           returned from this method. The variables can be retrieved from the QGField object after all computation is
+           finished. This may save run time in some use case.
 
         Returns
         -------
         Qref : numpy.ndarray
             Two-dimensional array of reference state of quasi-geostrophic potential vorticity (QGPV) with
             dimension = [kmax, nlat, nlon] if northern_hemisphere_results_only=False, or
             dimension = [kmax, nlat//2+1, nlon] if northern_hemisphere_results_only=True
@@ -517,86 +455,63 @@
 
         Examples
         --------
 
         >>> qref, uref, ptref = test_object.compute_reference_states()
 
         """
-        if self._northern_hemisphere_results_only is None:
-            self._northern_hemisphere_results_only = northern_hemisphere_results_only
-        else:
-            if northern_hemisphere_results_only != self._northern_hemisphere_results_only:
-                warnings.warn(
-                    f"In compute_reference_states, input argument northern_hemisphere_results_only = " +
-                    f"{northern_hemisphere_results_only} but self._northern_hemisphere_results_only has been " +
-                    f"initialized to {self._northern_hemisphere_results_only} already. The following computation will " +
-                    f"use self._northern_hemisphere_results_only = {self._northern_hemisphere_results_only}.")
 
-        if self._qgpv_temp is None:
-            self.interpolate_fields()
-
-        # === Compute reference states in Northern Hemisphere ===
-        self._qref_ntemp, self._uref_ntemp, self._ptref_ntemp, num_of_iter = self._compute_reference_state_wrapper(
-            qgpv=self._qgpv_temp, u=self._interpolated_u_temp, theta=self._interpolated_theta_temp)
-        if num_of_iter >= self.maxit:
-            raise ValueError("The reference state does not converge for Northern Hemisphere.")
-        # *** Convert Qref to the right unit
-        qref_ntemp_right_unit = \
-            self._qref_ntemp * 2 * self.omega * np.sin(np.deg2rad(self.ylat[(self.equator_idx - 1):, np.newaxis]))
-
-        # === Compute reference states in Southern Hemisphere ===
-        if not self._northern_hemisphere_results_only:
-            self._qref_stemp, self._uref_stemp, self._ptref_stemp, num_of_iter = self._compute_reference_state_wrapper(
-                qgpv=-self._qgpv_temp[:, ::-1, :],
-                u=self._interpolated_u_temp[:, ::-1, :],
-                theta=self._interpolated_theta_temp[:, ::-1, :])
-            if num_of_iter >= self.maxit:
-                raise ValueError("The reference state does not converge for Southern Hemisphere.")
+        if northern_hemisphere_results_only:
+            warnings.warn(
+                f"""
+                Since v0.7.0, northern_hemisphere_results_only is initialized at the creation of QGField instance.
+                The value of self.northern_hemisphere_results_only = {self.northern_hemisphere_results_only} but
+                your input here is northern_hemisphere_results_only = {northern_hemisphere_results_only}. 
+                Please remove this input argument from the method 'compute_reference_states'.
+                """)
+
+        if self.qgpv is None:
+            raise ValueError("QGField.interpolate_fields has to be called before QGField.compute_reference_states.")
+
+        self._compute_reference_states()
+
+        # *** Return a named tuple ***
+        if return_named_tuple:
+            Reference_states = namedtuple('Reference_states', ['Qref', 'Uref', 'PTref'])
+            reference_states = Reference_states(
+                self.qref,
+                self.uref,
+                self.ptref)
+            return reference_states
 
-            # *** Convert Qref to the right unit
-            qref_stemp_right_unit = self._qref_stemp[::-1, :] * 2 * self.omega * np.sin(
-                np.deg2rad(self.ylat[:self.equator_idx, np.newaxis]))
-
-        if self._northern_hemisphere_results_only:
-            self._qref = np.swapaxes(qref_ntemp_right_unit, 0, 1)
-            self._uref = np.swapaxes(self._uref_ntemp, 0, 1)
-            self._ptref = np.swapaxes(self._ptref_ntemp, 0, 1)
-        else:
-            self._qref = \
-                np.hstack((np.swapaxes(qref_stemp_right_unit[:, :], 0, 1),
-                           np.swapaxes(qref_ntemp_right_unit[1:, :], 0, 1)))
-            self._uref = \
-                np.hstack((np.swapaxes(self._uref_stemp[::-1, :], 0, 1),
-                           np.swapaxes(self._uref_ntemp[1:, :], 0, 1)))
-            self._ptref = \
-                np.hstack((np.swapaxes(self._ptref_stemp[::-1, :], 0, 1),
-                           np.swapaxes(self._ptref_ntemp[1:, :], 0, 1)))
-
-        # Construct a named tuple
-        Reference_states = namedtuple('Reference_states', ['Qref', 'Uref', 'PTref'])
-        reference_states = Reference_states(
-            self.qref,
-            self.uref,
-            self.ptref)
-        return reference_states
+    @abstractmethod
+    def _compute_reference_states(self):
+        """
+        Reference state computation with boundary conditions and procedures specified in the paper will be
+        implemented here.
+        """
 
-    def compute_lwa_and_barotropic_fluxes(self, northern_hemisphere_results_only=False):
+    def compute_lwa_and_barotropic_fluxes(self, return_named_tuple: bool = True, northern_hemisphere_results_only=None):
 
         """
         Compute barotropic components of local wave activity and flux terms in eqs.(2) and (3) in
         Nakamura and Huang (Science, 2018). It returns a named tuple called "LWA_and_fluxes" that consists of
         9 elements as listed below. The discretization scheme that is used in the numerical integration is outlined
         in the Supplementary materials of Huang and Nakamura (GRL, 2017).
 
+        The parameter `northern_hemisphere_results_only` is deprecated and has no effect.
+
+        Note that flux computation for NHN22 is still experimental.
+
         Parameters
         ----------
-        northern_hemisphere_results_only : bool
-           If true, arrays of size [kmax, nlat//2+1] will be returned. Otherwise, arrays of size [kmax, nlat] will be
-           returned. Default: False. If this variable has been initialized when calling compute_reference_states,
-           the initialized value will be used. This variable will be deprecated in the next major release.
+        return_named_tuple : bool
+           Whether to returned a named tuple with variables in python indexing. Default: True. If False, nothing will be
+           returned from this method. The variables can be retrieved from the QGField object after all computation is
+           finished. This may save run time in some use case.
 
         Returns
         -------
         adv_flux_f1 : numpy.ndarray
             Two-dimensional array of the second-order eddy term in zonal advective flux,
             i.e. F1 in equation 3 of NH18, with dimension = [nlat//2+1, nlon] if northern_hemisphere_results_only=True,
             or dimension = [nlat, nlon] if northern_hemisphere_results_only=False.
@@ -643,473 +558,763 @@
         --------
 
         >>> adv_flux_f1, adv_flux_f2, adv_flux_f3, convergence_zonal_advective_flux,
             divergence_eddy_momentum_flux, meridional_heat_flux,
             lwa_baro, u_baro, lwa = test_object.compute_lwa_and_barotropic_fluxes()
         """
 
-        # Check if previous steps have been done.
-        if self._qgpv_temp is None:
-            self.interpolate_fields()
-
-        if self._uref_ntemp is None:
-            self.compute_reference_states(northern_hemisphere_results_only)
-
-        if northern_hemisphere_results_only != self._northern_hemisphere_results_only:
+        if northern_hemisphere_results_only:
             warnings.warn(
-                f"In compute_lwa_and_barotropic_fluxes, input argument northern_hemisphere_results_only = " +
-                f"{northern_hemisphere_results_only} but self._northern_hemisphere_results_only has been " +
-                f"initialized to {self._northern_hemisphere_results_only} already. The following computation will " +
-                f"use self._northern_hemisphere_results_only = {self._northern_hemisphere_results_only}.")
+                f"""
+                Since v0.7.0, northern_hemisphere_results_only is initialized at the creation of QGField instance.
+                The value of self.northern_hemisphere_results_only = {self.northern_hemisphere_results_only} but
+                your input here is northern_hemisphere_results_only = {northern_hemisphere_results_only}. 
+                Please remove this input argument from the method 'compute_lwa_and_barotropic_fluxes'.
+                """)
 
-        # === Compute barotropic flux terms (NHem) ===
-        lwa_nhem, astarbaro_nhem, ua1baro_nhem, ubaro_nhem, ua2baro_nhem,\
-            ep1baro_nhem, ep2baro_nhem, ep3baro_nhem, ep4_nhem = \
-            self._compute_lwa_and_barotropic_fluxes_wrapper(
-                self._qgpv_temp,
-                self._interpolated_u_temp,
-                self._interpolated_v_temp,
-                self._interpolated_theta_temp,
-                self._qref_ntemp,
-                self._uref_ntemp,
-                self._ptref_ntemp)
-
-        # === Access barotropic components of ua1, ua2, ep1, ep2, ep3, ep4: for the use of nhn GLR paper only ===
-        self._ua1baro_nhem = ua1baro_nhem
-        self._ua2baro_nhem = ua2baro_nhem
-        self._ep1baro_nhem = ep1baro_nhem
-        self._ep2baro_nhem = ep2baro_nhem
-        self._ep3baro_nhem = ep3baro_nhem
-        self._ep4_nhem = ep4_nhem
+        # Check if previous steps have been done.
+        if self.qgpv is None:
+            raise ValueError("QGField.interpolate_fields has to be called before QGField.compute_reference_states.")
 
-        # === Compute barotropic flux terms (SHem) ===
-        if not self._northern_hemisphere_results_only:
-            lwa_shem, astarbaro_shem, ua1baro_shem, ubaro_shem, ua2baro_shem,\
-                ep1baro_shem, ep2baro_shem, ep3baro_shem, ep4_shem = \
-                self._compute_lwa_and_barotropic_fluxes_wrapper(
-                    -self._qgpv_temp[:, ::-1, :],
-                    self._interpolated_u_temp[:, ::-1, :],
-                    self._interpolated_v_temp[:, ::-1, :],
-                    self._interpolated_theta_temp[:, ::-1, :],
-                    self._qref_stemp,
-                    self._uref_stemp,
-                    self._ptref_stemp)
-
-        # *** Northern Hemisphere ***
-        # Compute divergence of the meridional eddy momentum flux
-        meri_flux_nhem_temp = np.zeros_like(ep2baro_nhem)
-        meri_flux_nhem_temp[:, 1:-1] = (ep2baro_nhem[:, 1:-1] - ep3baro_nhem[:, 1:-1]) / \
-            (2 * self.planet_radius * self.dphi *
-             np.cos(np.deg2rad(self.ylat[-self.equator_idx + 1:-1])))
-        # Compute convergence of the zonal LWA flux
-        zonal_adv_flux_nhem_sum = np.swapaxes((ua1baro_nhem + ua2baro_nhem + ep1baro_nhem), 0, 1)
-        convergence_zonal_advective_flux_nhem = \
+        # TODO: need a check for reference states computed. If not, throw an error.
+        self._compute_intermediate_flux_terms()
+
+        # *** Compute named fluxes in NH18 ***
+        clat = self.clat[-self.equator_idx:] if self.northern_hemisphere_results_only else self.clat
+        self._output_barotropic_flux_terms_storage.divergence_eddy_momentum_flux = \
+            np.swapaxes(
+                (self._barotropic_flux_terms_storage.ep2baro - self._barotropic_flux_terms_storage.ep3baro) / \
+                (2 * self.planet_radius * self.dphi * clat), 0, 1)
+
+        zonal_adv_flux_sum = np.swapaxes((
+            self._barotropic_flux_terms_storage.ua1baro
+            + self._barotropic_flux_terms_storage.ua2baro
+            + self._barotropic_flux_terms_storage.ep1baro), 0, 1)
+        self._output_barotropic_flux_terms_storage.convergence_zonal_advective_flux = \
             utilities.zonal_convergence(
-                zonal_adv_flux_nhem_sum,
-                np.cos(np.deg2rad(self.ylat[-self.equator_idx:])),
-                self.dlambda,
-                planet_radius=self.planet_radius
-            )
+                field=zonal_adv_flux_sum,
+                clat=clat,
+                dlambda=self.dlambda,
+                planet_radius=self.planet_radius)
+        self._output_barotropic_flux_terms_storage.adv_flux_f1 = \
+            self._barotropic_flux_terms_storage.fortran_to_python(self._barotropic_flux_terms_storage.ua1baro)
+        self._output_barotropic_flux_terms_storage.adv_flux_f2 = \
+            self._barotropic_flux_terms_storage.fortran_to_python(self._barotropic_flux_terms_storage.ua2baro)
+        self._output_barotropic_flux_terms_storage.adv_flux_f3 = \
+            self._barotropic_flux_terms_storage.fortran_to_python(self._barotropic_flux_terms_storage.ep1baro)
+        self._output_barotropic_flux_terms_storage.meridional_heat_flux = \
+            self._barotropic_flux_terms_storage.fortran_to_python(self._barotropic_flux_terms_storage.ep4)
+
+        # *** Return the named tuple ***
+        if return_named_tuple:
+            LWA_and_fluxes = namedtuple(
+                'LWA_and_fluxes',
+                ['adv_flux_f1', 'adv_flux_f2', 'adv_flux_f3', 'convergence_zonal_advective_flux',
+                 'divergence_eddy_momentum_flux', 'meridional_heat_flux', 'lwa_baro', 'u_baro', 'lwa'])
+            lwa_and_fluxes = LWA_and_fluxes(
+                self._output_barotropic_flux_terms_storage.adv_flux_f1,
+                self._output_barotropic_flux_terms_storage.adv_flux_f2,
+                self._output_barotropic_flux_terms_storage.adv_flux_f3,
+                self._output_barotropic_flux_terms_storage.convergence_zonal_advective_flux,
+                self._output_barotropic_flux_terms_storage.divergence_eddy_momentum_flux,
+                self._output_barotropic_flux_terms_storage.meridional_heat_flux,
+                self._barotropic_flux_terms_storage.fortran_to_python(self._barotropic_flux_terms_storage.lwa_baro),
+                self._barotropic_flux_terms_storage.fortran_to_python(self._barotropic_flux_terms_storage.u_baro),
+                self._lwa_storage.fortran_to_python(self._lwa_storage.lwa))
+            return lwa_and_fluxes
 
-        # *** Southern Hemisphere ***
-        # Compute divergence of the meridional eddy momentum flux
-        if not self._northern_hemisphere_results_only:
-            meri_flux_shem_temp = np.zeros_like(ep2baro_shem)
-            meri_flux_shem_temp[:, 1:-1] = (ep2baro_shem[:, 1:-1] - ep3baro_shem[:, 1:-1]) / \
-                (2 * self.planet_radius * self.dphi *
-                 np.cos(np.deg2rad(self.ylat[-self.equator_idx + 1:-1])))
-
-            # Compute convergence of the zonal LWA flux
-            zonal_adv_flux_shem_sum = np.swapaxes((ua1baro_shem + ua2baro_shem + ep1baro_shem), 0, 1)  # axes swapped
-            convergence_zonal_advective_flux_shem = \
-                utilities.zonal_convergence(
-                    zonal_adv_flux_shem_sum,
-                    np.cos(np.deg2rad(self.ylat[-self.equator_idx:])),
-                    self.dlambda,
-                    planet_radius=self.planet_radius
-                )
-
-        if self._northern_hemisphere_results_only:
-            self._adv_flux_f1 = np.swapaxes(ua1baro_nhem, 0, 1)
-            self._adv_flux_f2 = np.swapaxes(ua2baro_nhem, 0, 1)
-            self._adv_flux_f3 = np.swapaxes(ep1baro_nhem, 0, 1)
-            self._convergence_zonal_advective_flux = convergence_zonal_advective_flux_nhem
-            self._meridional_heat_flux = np.swapaxes(ep4_nhem, 0, 1)
-            self._lwa_baro = np.swapaxes(astarbaro_nhem, 0, 1)
-            self._u_baro = np.swapaxes(ubaro_nhem, 0, 1)
-            self._lwa = np.swapaxes(lwa_nhem, 0, 2)
-            self._divergence_eddy_momentum_flux = \
-                np.swapaxes(meri_flux_nhem_temp, 0, 1)
-        else:
-            # Flip component in southern hemisphere
-            self._adv_flux_f1 = np.vstack((np.swapaxes(ua1baro_shem[:, ::-1], 0, 1),
-                                           np.swapaxes(ua1baro_nhem[:, 1:], 0, 1)))
-
-            self._adv_flux_f2 = np.vstack((np.swapaxes(ua2baro_shem[:, ::-1], 0, 1),
-                                           np.swapaxes(ua2baro_nhem[:, 1:], 0, 1)))
-
-            self._adv_flux_f3 = np.vstack((np.swapaxes(ep1baro_shem[:, ::-1], 0, 1),
-                                           np.swapaxes(ep1baro_nhem[:, 1:], 0, 1)))
-
-            # Axes already swapped for convergence zonal advective flux
-            self._convergence_zonal_advective_flux = np.vstack((convergence_zonal_advective_flux_shem[::-1, :],
-                                                                convergence_zonal_advective_flux_nhem[1:, :]))
-
-            # Negative sign for southern hemisphere upon flipping (via Coriolis parameter)
-            self._meridional_heat_flux = \
-                np.vstack((np.swapaxes(-ep4_shem[:, ::-1], 0, 1),
-                           np.swapaxes(ep4_nhem[:, 1:], 0, 1)))
-
-            self._lwa_baro = \
-                np.vstack((np.swapaxes(astarbaro_shem[:, ::-1], 0, 1),
-                           np.swapaxes(astarbaro_nhem[:, 1:], 0, 1)))
-
-            self._u_baro = np.vstack((np.swapaxes(ubaro_shem[:, ::-1], 0, 1),
-                                      np.swapaxes(ubaro_nhem[:, 1:], 0, 1)))
-
-            self._lwa = np.concatenate((np.swapaxes(lwa_shem[:, ::-1], 0, 2),
-                                        np.swapaxes(lwa_nhem[:, 1:], 0, 2)), axis=1)
-
-            self._divergence_eddy_momentum_flux = np.vstack((np.swapaxes(-meri_flux_shem_temp[:, ::-1], 0, 1),
-                                                             np.swapaxes(meri_flux_nhem_temp[:, 1:], 0, 1)))
-
-        # Construct a named tuple
-        LWA_and_fluxes = namedtuple(
-            'LWA_and_fluxes',
-            ['adv_flux_f1', 'adv_flux_f2', 'adv_flux_f3', 'convergence_zonal_advective_flux',
-             'divergence_eddy_momentum_flux', 'meridional_heat_flux', 'lwa_baro', 'u_baro', 'lwa'])
-        lwa_and_fluxes = LWA_and_fluxes(
-            self.adv_flux_f1, self.adv_flux_f2, self.adv_flux_f3, self.convergence_zonal_advective_flux,
-            self.divergence_eddy_momentum_flux, self.meridional_heat_flux, self.lwa_baro, self.u_baro, self.lwa)
-        return lwa_and_fluxes
-
-    # *** Added in Release 0.6.0 ***
-    # The following internal functions are used to compute results in NHN (2022, GRL):
-    # - _interpolate_field_dirinv
-    # - _compute_qref_fawa_and_bc
-    # - _compute_lwa_flux_dirinv
-    # They will be refactored in the upcoming releases.
-    def _interpolate_field_dirinv(self):
+    @abstractmethod
+    def _compute_intermediate_flux_terms(self):
         """
-        Added for NHN 2022 GRL
-
-        .. versionadded:: 0.6.0
+        Compute ua1, ua2, ep1, ep2, ep3, ep4 depending on which BC protocol to use.
         """
-        self._qgpv_temp, \
-        self._interpolated_u_temp, \
-        self._interpolated_v_temp, \
-        self._interpolated_avort_temp, \
-        self._interpolated_theta_temp, \
-        self._static_stability_n, \
-        self._static_stability_s,\
-        self._tn0, self._ts0 = \
-            interpolate_fields_direct_inv(
-                self.kmax,
-                self.nlat // 2 + self.nlat % 2,
-                np.swapaxes(self.u_field, 0, 2),
-                np.swapaxes(self.v_field, 0, 2),
-                np.swapaxes(self.t_field, 0, 2),
-                self.plev,
-                self.planet_radius,
-                self.omega,
-                self.dz,
-                self.scale_height,
-                self.dry_gas_constant,
-                self.cp)
-
-        self._check_nan("self._qgpv_temp", self._qgpv_temp)
-        self._check_nan("self._interpolated_u_temp", self._interpolated_u_temp)
-        self._check_nan("self._interpolated_v_temp", self._interpolated_v_temp)
-        self._check_nan("self._interpolated_avort_temp", self._interpolated_avort_temp)
-        self._check_nan("self._interpolated_theta_temp", self._interpolated_theta_temp)
-        self._check_nan("self._static_stability_n", self._static_stability_n)
-        self._check_nan("self._static_stability_s", self._static_stability_s)
-        self._check_nan("self._tn0", self._tn0)
-        self._check_nan("self._ts0", self._ts0)
-
-        return self._qgpv_temp, self._interpolated_u_temp, self._interpolated_v_temp,  self._interpolated_avort_temp, \
-        self._interpolated_theta_temp, self._static_stability_n, self._static_stability_s, self._tn0, self._ts0
 
     @staticmethod
     def _check_nan(name, var):
         nan_num = np.count_nonzero(np.isnan(var))
         if nan_num > 0:
             print(f"num of nan in {name}: {np.count_nonzero(np.isnan(var))}.")
 
-    def _compute_qref_fawa_and_bc(self):
-        """
-        Added for NHN 2022 GRL
+    # *** Fixed properties (since creation of instance) ***
+    @property
+    def prefactor(self):
+        """Normalization constant for vertical weighted-averaged integration"""
+        return self._prefactor
 
-        .. versionadded:: 0.6.0
+    @property
+    def ylat_ref_states(self) -> np.array:
         """
-        # ans = compute_qref_and_fawa_first(
-            # pv, uu, vort, pt, nd, nnd, jb, jd, aa, omega, dz, h, rr, cp)
-        ans = compute_qref_and_fawa_first(
-            pv=self._qgpv_temp,
-            uu=self._interpolated_u_temp,
-            vort=self._interpolated_avort_temp,
-            pt=self._interpolated_theta_temp,
-            tn0=self._tn0,
-            nd=self.nlat//2 + self.nlat % 2,  # 91
-            nnd=self.nlat,                    # 181
-            jb=self.eq_boundary_index,        # 5
-            jd=self.nlat//2 + self.nlat % 2 - self.eq_boundary_index,  # 86 TODO fix its formula
-            a=self.planet_radius,
-            omega=self.omega,
-            dz=self.dz,
-            h=self.scale_height,
-            rr=self.dry_gas_constant,
-            cp=self.cp)
-
-        qref_over_cor, ubar, tbar, fawa, ckref, tjk, sjk = ans  # unpack tuple
-
-        self._check_nan("qref_over_cor", qref_over_cor)
-        self._check_nan("ubar", ubar)
-        self._check_nan("tbar", tbar)
-        self._check_nan("fawa", fawa)
-        self._check_nan("ckref", ckref)
-        self._check_nan("tjk", tjk)
-        self._check_nan("sjk", sjk)
-
-        for k in range(self.kmax-1, 1, -1):  # Fortran indices
-            ans = matrix_b4_inversion(
-                k=k,
-                jmax=self.nlat,
-                jb=self.eq_boundary_index,  # 5
-                jd=self.nlat // 2 + self.nlat % 2 - self.eq_boundary_index,  # 86
-                z=np.arange(0, self.kmax*self.dz, self.dz),
-                statn=self._static_stability_n,
-                qref=qref_over_cor,
-                ckref=ckref,
-                a=self.planet_radius,
-                om=self.omega,
-                dz=self.dz,
-                h=self.scale_height,
-                rr=self.dry_gas_constant,
-                cp=self.cp,
-                sjk=sjk,
-                tjk=tjk)
-            qjj, djj, cjj, rj, tj = ans
-
-            # TODO: The inversion algorithm  is the bottleneck of the computation
-            # SciPy is very slow compared to MKL in Fortran...
-            lu, piv, info = dgetrf(qjj)
-            qjj, info = dgetri(lu, piv)
-
-            _ = matrix_after_inversion(
-                k=k,
-                qjj=qjj,
-                djj=djj,
-                cjj=cjj,
-                tj=tj,
-                rj=rj,
-                sjk=sjk,
-                tjk=tjk)
-
-        tref, qref, u = upward_sweep(
-            jmax=self.nlat,
-            jb=self.eq_boundary_index,
-            sjk=sjk,
-            tjk=tjk,
-            ckref=ckref,
-            tb=self._tn0,
-            qref_over_cor=qref_over_cor,
-            a=self.planet_radius,
-            om=self.omega,
-            dz=self.dz,
-            h=self.scale_height,
-            rr=self.dry_gas_constant,
-            cp=self.cp)
-
-        return qref, u, tref, fawa, ubar, tbar  # uref = u
-
-    def _compute_lwa_flux_dirinv(self, qref, uref, tref):
+        Latitude dimension of reference state
         """
-        Added for NHN 2022 GRL
+        if self.northern_hemisphere_results_only:
+            return self.ylat[-(self.nlat//2+1):]
+        return self.ylat
 
-        .. versionadded:: 0.6.0
+    @property
+    def northern_hemisphere_results_only(self) -> bool:
         """
-        ans = compute_flux_dirinv(pv=self._qgpv_temp, uu=self._interpolated_u_temp, vv=self._interpolated_v_temp,
-                                  pt=self._interpolated_theta_temp, tn0=self._tn0,
-                                  qref=qref, uref=uref, tref=tref,
-                                  jb=self.eq_boundary_index, a=self.planet_radius, om=self.omega,
-                                  dz=self.dz, h=self.scale_height, rr=self.dry_gas_constant, cp=self.cp,
-                                  prefac=self.prefactor)
-        # astarbaro, ubaro, urefbaro, ua1baro, ua2baro, ep1baro, ep2baro, ep3baro, ep4, astar1, astar2 = ans
-        return ans
+        Even though a global field is required for input, whether ref state and fluxes are computed for
+        northern hemisphere only
+        """
+        return self._northern_hemisphere_results_only
 
+    # *** Derived physical quantities ***
     @property
     def qgpv(self):
         """
         Quasi-geostrophic potential vorticity on the regular pseudoheight grids.
         """
-        if self._qgpv is None:
+        if self._interpolated_field_storage.qgpv is None:
             raise ValueError('QGPV field is not present in the QGField object.')
-        return self._return_interp_variables(
-            variable=self._qgpv, interp_axis=1, northern_hemisphere_results_only=False)
+        return self._return_interp_variables(variable=self._interpolated_field_storage.fortran_to_python(
+            self._interpolated_field_storage.qgpv), interp_axis=1)
 
     @property
     def interpolated_u(self):
         """
         Zonal wind on the regular pseudoheight grids.
         """
-        if self._interpolated_u is None:
+        if self._interpolated_field_storage.interpolated_u is None:
             raise ValueError('interpolated_u is not present in the QGField object.')
-        return self._return_interp_variables(
-            variable=self._interpolated_u, interp_axis=1, northern_hemisphere_results_only=False)
+        return self._return_interp_variables(variable=self._interpolated_field_storage.fortran_to_python(
+            self._interpolated_field_storage.interpolated_u), interp_axis=1)
 
     @property
     def interpolated_v(self):
         """
         Meridional wind on the regular pseudoheight grids.
         """
-        if self._interpolated_v is None:
+        if self._interpolated_field_storage.interpolated_v is None:
             raise ValueError('interpolated_v is not present in the QGField object.')
-        return self._return_interp_variables(
-            variable=self._interpolated_v, interp_axis=1, northern_hemisphere_results_only=False)
+        return self._return_interp_variables(variable=self._interpolated_field_storage.fortran_to_python(
+            self._interpolated_field_storage.interpolated_v), interp_axis=1)
 
     @property
     def interpolated_theta(self):
         """
         Potential temperature on the regular pseudoheight grids.
         """
-        if self._interpolated_theta is None:
+        if self._interpolated_field_storage.interpolated_theta is None:
             raise ValueError('interpolated_theta is not present in the QGField object.')
-        return self._return_interp_variables(
-            variable=self._interpolated_theta, interp_axis=1, northern_hemisphere_results_only=False)
+        return self._return_interp_variables(variable=self._interpolated_field_storage.fortran_to_python(
+            self._interpolated_field_storage.interpolated_theta), interp_axis=1)
 
     @property
-    def static_stability(self):
+    @abstractmethod
+    def static_stability(self) -> Union[np.array, Tuple[np.array, np.array]]:
         """
         The interpolated static stability.
         """
-        return self._static_stability
 
     @property
     def qref(self):
         """
         Reference state of QGPV (Qref).
         """
-        if self._qref is None:
+        if self._reference_states_storage.qref is None:
             raise ValueError('qref is not computed yet.')
-        return self._return_interp_variables(variable=self._qref, interp_axis=1,
-                                             northern_hemisphere_results_only=self._northern_hemisphere_results_only)
+        return self._return_interp_variables(
+            variable=self._reference_states_storage.qref_correct_unit(
+                self.ylat_ref_states, self.omega), interp_axis=1)
 
     @property
     def uref(self):
         """
         Reference state of zonal wind (Uref).
         """
-        if self._uref is None:
-            raise ValueError('uref field is not computed yet.')
-        return self._return_interp_variables(variable=self._uref, interp_axis=1,
-                                             northern_hemisphere_results_only=self._northern_hemisphere_results_only)
+        if self._reference_states_storage.uref is None:
+            raise ValueError('uref is not computed yet.')
+        return self._return_interp_variables(
+            variable=self._reference_states_storage.fortran_to_python(self._reference_states_storage.uref), interp_axis=1)
 
     @property
     def ptref(self):
         """
         Reference state of potential temperature (\\Theta_ref).
         """
-        if self._ptref is None:
-            raise ValueError('ptref field is not computed yet.')
-        return self._return_interp_variables(variable=self._ptref, interp_axis=1,
-                                             northern_hemisphere_results_only=self._northern_hemisphere_results_only)
+        if self._reference_states_storage.ptref is None:
+            raise ValueError('ptref is not computed yet.')
+        return self._return_interp_variables(
+            variable=self._reference_states_storage.fortran_to_python(self._reference_states_storage.ptref), interp_axis=1)
 
     @property
     def adv_flux_f1(self):
         """
         Two-dimensional array of the second-order eddy term in zonal advective flux, i.e. F1 in equation 3 of NH18
         """
-        if self._adv_flux_f1 is None:
-            raise ValueError('adv_flux_f1 is not computed yet.')
-        return self._return_interp_variables(variable=self._adv_flux_f1, interp_axis=0,
-                                             northern_hemisphere_results_only=self._northern_hemisphere_results_only)
+        return self._return_interp_variables(
+            variable=self._output_barotropic_flux_terms_storage.adv_flux_f1,
+            interp_axis=0)
 
     @property
     def adv_flux_f2(self):
         """
         Two-dimensional array of the third-order eddy term in zonal advective flux, i.e. F2 in equation 3 of NH18
         """
-        if self._adv_flux_f2 is None:
-            raise ValueError('adv_flux_f2 is not computed yet.')
-        return self._return_interp_variables(variable=self._adv_flux_f2, interp_axis=0,
-                                             northern_hemisphere_results_only=self._northern_hemisphere_results_only)
+        return self._return_interp_variables(
+            variable=self._output_barotropic_flux_terms_storage.adv_flux_f2,
+            interp_axis=0)
 
     @property
     def adv_flux_f3(self):
         """
         Two-dimensional array of the remaining term in zonal advective flux, i.e. F3 in equation 3 of NH18
         """
-        if self._adv_flux_f3 is None:
-            raise ValueError('adv_flux_f3 is not computed yet.')
-        return self._return_interp_variables(variable=self._adv_flux_f3, interp_axis=0,
-                                             northern_hemisphere_results_only=self._northern_hemisphere_results_only)
+        return self._return_interp_variables(
+            variable=self._output_barotropic_flux_terms_storage.adv_flux_f3,
+            interp_axis=0)
 
     @property
     def convergence_zonal_advective_flux(self):
         """
         Two-dimensional array of the convergence of zonal advective flux, i.e. -div(F1+F2+F3) in equation 3 of NH18
         """
-        if self._convergence_zonal_advective_flux is None:
-            raise ValueError('convergence_zonal_advective_flux is not computed yet.')
-        return self._return_interp_variables(variable=self._convergence_zonal_advective_flux, interp_axis=0,
-                                             northern_hemisphere_results_only=self._northern_hemisphere_results_only)
+        return self._return_interp_variables(
+            variable=self._output_barotropic_flux_terms_storage.convergence_zonal_advective_flux,
+            interp_axis=0)
 
     @property
     def divergence_eddy_momentum_flux(self):
         """
         Two-dimensional array of the divergence of eddy momentum flux, i.e. (II) in equation 2 of NH18
         """
-        if self._divergence_eddy_momentum_flux is None:
-            raise ValueError('divergence_eddy_momentum_flux is not computed yet.')
-        return self._return_interp_variables(variable=self._divergence_eddy_momentum_flux, interp_axis=0,
-                                             northern_hemisphere_results_only=self._northern_hemisphere_results_only)
+        return self._return_interp_variables(
+            variable=self._output_barotropic_flux_terms_storage.divergence_eddy_momentum_flux,
+            interp_axis=0)
 
     @property
     def meridional_heat_flux(self):
         """
         Two-dimensional array of the low-level meridional heat flux, i.e. (III) in equation 2 of NH18
         """
-        if self._meridional_heat_flux is None:
-            raise ValueError('meridional_heat_flux is not computed yet.')
-        return self._return_interp_variables(variable=self._meridional_heat_flux, interp_axis=0,
-                                             northern_hemisphere_results_only=self._northern_hemisphere_results_only)
+        return self._return_interp_variables(
+            variable=self._output_barotropic_flux_terms_storage.meridional_heat_flux,
+            interp_axis=0)
 
     @property
     def lwa_baro(self):
         """
         Two-dimensional array of barotropic local wave activity (with cosine weighting).
         """
-        if self._lwa_baro is None:
+        if self._barotropic_flux_terms_storage.lwa_baro is None:
             raise ValueError('lwa_baro is not computed yet.')
-        return self._return_interp_variables(variable=self._lwa_baro, interp_axis=0,
-                                             northern_hemisphere_results_only=self._northern_hemisphere_results_only)
+        return self._return_interp_variables(
+            variable=self._barotropic_flux_terms_storage.fortran_to_python(
+                self._barotropic_flux_terms_storage.lwa_baro),
+            interp_axis=0)
 
     @property
     def u_baro(self):
         """
         Two-dimensional array of barotropic zonal wind (without cosine weighting).
         """
-        if self._u_baro is None:
+        if self._barotropic_flux_terms_storage.u_baro is None:
             raise ValueError('u_baro is not computed yet.')
-        return self._return_interp_variables(variable=self._u_baro, interp_axis=0,
-                                             northern_hemisphere_results_only=self._northern_hemisphere_results_only)
+        return self._return_interp_variables(
+            variable=self._barotropic_flux_terms_storage.fortran_to_python(
+                self._barotropic_flux_terms_storage.u_baro),
+            interp_axis=0)
 
     @property
     def lwa(self):
         """
-        Three-dimensional array of barotropic local wave activity
+        Three-dimensional array of local wave activity
         """
-        if self._lwa is None:
+        if self._lwa_storage.lwa is None:
             raise ValueError('lwa is not computed yet.')
-        return self._return_interp_variables(variable=self._lwa, interp_axis=1,
-                                             northern_hemisphere_results_only=self._northern_hemisphere_results_only)
+        return self._return_interp_variables(
+            variable=self._lwa_storage.fortran_to_python(self._lwa_storage.lwa),
+            interp_axis=1)
 
     def get_latitude_dim(self):
         """
         Return the latitude dimension of the input data.
         """
         if self.need_latitude_interpolation:
             return self.ylat_no_equator.size
         else:
             return self.nlat
 
+
+class QGFieldNH18(QGFieldBase):
+    """
+    Procedures and reference state computation with the set of boundary conditions of NH18:
+
+        Nakamura, N., & Huang, C. S. (2018). Atmospheric blocking as a traffic jam in the jet stream. Science, 361(6397), 42-47.
+        https://www.science.org/doi/10.1126/science.aat0721
+
+    See the documentation of :py:class:`QGField` for the public interface.
+    There are no additional arguments for this class.
+
+    .. versionadded:: 0.7.0
+
+    Examples
+    --------
+    :doc:`notebooks/demo_script_for_nh2018`
+    """
+
+    def _interpolate_fields(self, Interpolated_fields_to_return, return_named_tuple) -> Optional[NamedTuple]:
+        """
+        .. versionadded:: 0.7.0
+        """
+        self._interpolated_field_storage.qgpv, \
+            self._interpolated_field_storage.interpolated_u, \
+            self._interpolated_field_storage.interpolated_v, \
+            self._interpolated_field_storage.interpolated_avort, \
+            self._interpolated_field_storage.interpolated_theta, \
+            self._domain_average_storage.static_stability = interpolate_fields(  # f2py module
+                np.swapaxes(self.u_field, 0, 2),
+                np.swapaxes(self.v_field, 0, 2),
+                np.swapaxes(self.t_field, 0, 2),
+                self.plev,
+                self.height,
+                self.planet_radius,
+                self.omega,
+                self.dz,
+                self.scale_height,
+                self.dry_gas_constant,
+                self.cp)
+
+        if return_named_tuple:
+            interpolated_fields = Interpolated_fields_to_return(
+                self.qgpv,
+                self.interpolated_u,
+                self.interpolated_v,
+                self.interpolated_theta,
+                self._domain_average_storage.static_stability)
+            return interpolated_fields
+
+    def _compute_reference_states(self):
+        """
+        .. versionadded:: 0.7.0
+        """
+        # *** Compute reference states in Northern Hemisphere using SOR ***
+        self._reference_states_storage.qref_nhem, \
+            self._reference_states_storage.uref_nhem, \
+            self._reference_states_storage.ptref_nhem, num_of_iter = \
+            self._compute_reference_state_wrapper(
+                qgpv=self._interpolated_field_storage.qgpv,
+                u=self._interpolated_field_storage.interpolated_u,
+                theta=self._interpolated_field_storage.interpolated_theta)
+
+        if num_of_iter >= self.maxit:
+            raise ValueError("The reference state does not converge for Northern Hemisphere.")
+
+        # === Compute reference states in Southern Hemisphere ===
+        if not self.northern_hemisphere_results_only:
+            self._reference_states_storage.qref_shem, \
+                self._reference_states_storage.uref_shem, \
+                self._reference_states_storage.ptref_shem, num_of_iter = \
+                self._compute_reference_state_wrapper(
+                    qgpv=-self._interpolated_field_storage.qgpv[:, ::-1, :],
+                    u=self._interpolated_field_storage.interpolated_u[:, ::-1, :],
+                    theta=self._interpolated_field_storage.interpolated_theta[:, ::-1, :])
+
+            if num_of_iter >= self.maxit:
+                raise ValueError("The reference state does not converge for Southern Hemisphere.")
+
+    def _compute_reference_state_wrapper(self, qgpv, u, theta):
+        """
+        Private function to call the fortran subroutine compute_reference_states that returns variable of
+        dimension [nlat, kmax]. Swapping of axes is needed for other computation.
+
+        Parameters
+        ----------
+            qgpv(numpy.ndarray): QGPV
+
+            u(numpy.ndarray): 3D zonal wind
+
+            theta(numpy.ndarray): 3D potential temperature
+
+            num_of_iter(int): number of iteration when solving the eliptic equation
+
+        Returns
+        -------
+            Qref(numpy.ndarray): Reference state of QGPV of dimension [nlat, kmax]
+
+            Uref(numpy.ndarray): Reference state of zonal wind of dimension [nlat, kmax]
+
+            PTref(numpy.ndarray): Reference state of potential temperature of dimension [nlat, kmax]
+        """
+        return compute_reference_states(
+            qgpv,
+            u,
+            theta,
+            self._domain_average_storage.static_stability,
+            self.equator_idx,
+            self.npart,
+            self.maxit,
+            self.planet_radius,
+            self.omega,
+            self.dz,
+            self.tol,
+            self.scale_height,
+            self.dry_gas_constant,
+            self.cp,
+            self.rjac,
+        )
+
+    def _compute_intermediate_flux_terms(self):
+        """
+        The flux term computation from NH18 is currently shared by both interface.
+        .. versionadded:: 0.7.0
+        """
+        # === Compute barotropic flux terms (NHem) ===
+        self._lwa_storage.lwa_nhem, \
+            self._barotropic_flux_terms_storage.lwa_baro_nhem, \
+            self._barotropic_flux_terms_storage.ua1baro_nhem, \
+            self._barotropic_flux_terms_storage.u_baro_nhem, \
+            self._barotropic_flux_terms_storage.ua2baro_nhem, \
+            self._barotropic_flux_terms_storage.ep1baro_nhem, \
+            self._barotropic_flux_terms_storage.ep2baro_nhem, \
+            self._barotropic_flux_terms_storage.ep3baro_nhem, \
+            self._barotropic_flux_terms_storage.ep4_nhem = \
+            self._compute_lwa_and_barotropic_fluxes_wrapper(
+                self._interpolated_field_storage.qgpv,
+                self._interpolated_field_storage.interpolated_u,
+                self._interpolated_field_storage.interpolated_v,
+                self._interpolated_field_storage.interpolated_theta,
+                self._reference_states_storage.qref_nhem,
+                self._reference_states_storage.uref_nhem,
+                self._reference_states_storage.ptref_nhem)
+
+        # === Compute barotropic flux terms (SHem) ===
+        # TODO: check signs!
+        if not self.northern_hemisphere_results_only:
+            self._lwa_storage.lwa_shem, \
+                self._barotropic_flux_terms_storage.lwa_baro_shem, \
+                self._barotropic_flux_terms_storage.ua1baro_shem, \
+                self._barotropic_flux_terms_storage.u_baro_shem, \
+                self._barotropic_flux_terms_storage.ua2baro_shem, \
+                self._barotropic_flux_terms_storage.ep1baro_shem, \
+                self._barotropic_flux_terms_storage.ep2baro_shem, \
+                self._barotropic_flux_terms_storage.ep3baro_shem, \
+                ep4_shem = \
+                self._compute_lwa_and_barotropic_fluxes_wrapper(
+                    -self._interpolated_field_storage.qgpv[:, ::-1, :],
+                    self._interpolated_field_storage.interpolated_u[:, ::-1, :],
+                    self._interpolated_field_storage.interpolated_v[:, ::-1, :],
+                    self._interpolated_field_storage.interpolated_theta[:, ::-1, :],
+                    self._reference_states_storage.qref_shem[::-1, :],
+                    self._reference_states_storage.uref_shem[::-1, :],
+                    self._reference_states_storage.ptref_shem[::-1, :])
+            self._barotropic_flux_terms_storage.ep4_shem = -ep4_shem
+
+    @property
+    def static_stability(self) -> np.array:
+        """
+        The interpolated static stability.
+        """
+        return self._domain_average_storage.static_stability
+
+
+class QGField(QGFieldNH18):
+    """
+    This class is equivalent to `QGFieldNH18` for backward compatibility.
+    `QGField` will be deprecated in upcoming release. See documentation in `QGFieldNH18`.
+    """
+
+
+class QGFieldNHN22(QGFieldBase):
+    """
+    Procedures and reference state computation with the set of boundary conditions of NHN22:
+
+        Neal et al (2022). The 2021 Pacific Northwest heat wave and associated blocking: meteorology and the role of an
+        upstream cyclone as a diabatic source of wave activity.
+        https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2021GL097699
+
+    Note that barotropic flux term computation from this class occasionally experience numerical instability, so
+    please use with caution.
+
+    See the documentation of :py:class:`QGField` for the public interface.
+
+    .. versionadded:: 0.7.0
+
+    Parameters
+    ----------
+    eq_boundary_index: int, optional
+        The improved inversion algorithm of reference states allow modification of equatorward boundary
+        to be the absolute vorticity. This parameter specify the location of grid point (from equator)
+        which will be used as boundary. The results in NHN22 is produced by using 1 deg latitude data and
+        eq_boundary_index = 5, i.e. using a latitude domain from 5 deg to the pole. Default = 5 here.
+
+    Examples
+    --------
+    Notebook: :doc:`notebooks/nhn22_reference_states`
+    """
+    def __init__(self, xlon, ylat, plev, u_field, v_field, t_field, kmax=49, maxit=100000, dz=1000., npart=None,
+                 tol=1.e-5, rjac=0.95, scale_height=SCALE_HEIGHT, cp=CP, dry_gas_constant=DRY_GAS_CONSTANT,
+                 omega=EARTH_OMEGA, planet_radius=EARTH_RADIUS,
+                 northern_hemisphere_results_only=False, eq_boundary_index=5):
+        super().__init__(xlon, ylat, plev, u_field, v_field, t_field, kmax, maxit, dz, npart, tol, rjac, scale_height,
+                         cp, dry_gas_constant, omega, planet_radius, northern_hemisphere_results_only)
+
+        # === Latitude domain boundary ===
+        self._eq_boundary_index = eq_boundary_index
+        self._jd = self.nlat // 2 + self.nlat % 2 - self.eq_boundary_index
+
+    def _interpolate_fields(self, Interpolated_fields_to_return, return_named_tuple) -> Optional[NamedTuple]:
+        """
+        .. versionadded:: 0.7.0
+        """
+        self._interpolated_field_storage.qgpv, \
+            self._interpolated_field_storage.interpolated_u, \
+            self._interpolated_field_storage.interpolated_v, \
+            self._interpolated_field_storage.interpolated_avort, \
+            self._interpolated_field_storage.interpolated_theta, \
+            self._domain_average_storage.static_stability_n, \
+            self._domain_average_storage.static_stability_s, \
+            self._domain_average_storage.tn0, self._domain_average_storage.ts0 = interpolate_fields_direct_inv(  # f2py module
+                self.kmax,
+                self.nlat // 2 + self.nlat % 2,
+                np.swapaxes(self.u_field, 0, 2),
+                np.swapaxes(self.v_field, 0, 2),
+                np.swapaxes(self.t_field, 0, 2),
+                self.plev,
+                self.planet_radius,
+                self.omega,
+                self.dz,
+                self.scale_height,
+                self.dry_gas_constant,
+                self.cp)
+
+        if return_named_tuple:
+            interpolated_fields = Interpolated_fields_to_return(
+                self.qgpv,
+                self.interpolated_u,
+                self.interpolated_v,
+                self.interpolated_theta,
+                (self._domain_average_storage.static_stability_s, self._domain_average_storage.static_stability_n))
+            return interpolated_fields
+
+    def _compute_reference_states(self):
+        """
+        Added for NHN 2022 GRL
+
+        .. versionadded:: 0.6.0
+        """
+
+        # === Compute reference states in Northern Hemisphere ===
+        self._reference_states_storage.qref_nhem, \
+            self._reference_states_storage.uref_nhem, \
+            self._reference_states_storage.ptref_nhem, \
+                fawa, ubar, tbar = \
+            self._compute_reference_states_nhn22_hemispheric_wrapper(
+                qgpv=self._interpolated_field_storage.qgpv,
+                u=self._interpolated_field_storage.interpolated_u,
+                avort=self._interpolated_field_storage.interpolated_avort,
+                theta=self._interpolated_field_storage.interpolated_theta,
+                t0=self._domain_average_storage.tn0)
+
+        if not self.northern_hemisphere_results_only:
+            # === Compute reference states in Southern Hemisphere ===
+            self._reference_states_storage.qref_shem, \
+                self._reference_states_storage.uref_shem, \
+                self._reference_states_storage.ptref_shem, \
+                fawa, ubar, tbar = \
+                self._compute_reference_states_nhn22_hemispheric_wrapper(
+                    qgpv=-self._interpolated_field_storage.qgpv[:, ::-1, :],
+                    u=self._interpolated_field_storage.interpolated_u[:, ::-1, :],
+                    avort=self._interpolated_field_storage.interpolated_avort[:, ::-1, :],
+                    theta=self._interpolated_field_storage.interpolated_theta[:, ::-1, :],
+                    t0=self._domain_average_storage.ts0)
+
+    def _compute_reference_states_nhn22_hemispheric_wrapper(self, qgpv, u, avort, theta, t0):
+        """
+        Wrapper to a series of operation using direct inversion algorithm to solve reference state.
+        """
+        qref_over_sin, ubar, tbar, fawa, ckref, tjk, sjk = compute_qref_and_fawa_first(
+            pv=qgpv,
+            uu=u,
+            vort=avort,
+            pt=theta,
+            tn0=t0,
+            nd=self.nlat//2 + self.nlat % 2,  # 91
+            nnd=self.nlat,                    # 181
+            jb=self.eq_boundary_index,        # 5
+            jd=self.jd,
+            a=self.planet_radius,
+            omega=self.omega,
+            dz=self.dz,
+            h=self.scale_height,
+            rr=self.dry_gas_constant,
+            cp=self.cp)
+
+        self._check_nan("qref_over_sin", qref_over_sin)
+        self._check_nan("ubar", ubar)
+        self._check_nan("tbar", tbar)
+        self._check_nan("fawa", fawa)
+        self._check_nan("ckref", ckref)
+        self._check_nan("tjk", tjk)
+        self._check_nan("sjk", sjk)
+
+        for k in range(self.kmax-1, 1, -1):  # Fortran indices
+            ans = matrix_b4_inversion(
+                k=k,
+                jmax=self.nlat,
+                jb=self.eq_boundary_index,  # 5
+                jd=self.jd,
+                z=np.arange(0, self.kmax*self.dz, self.dz),
+                statn=self._domain_average_storage.static_stability_n,
+                qref=qref_over_sin,
+                ckref=ckref,
+                sjk=sjk,
+                a=self.planet_radius,
+                om=self.omega,
+                dz=self.dz,
+                h=self.scale_height,
+                rr=self.dry_gas_constant,
+                cp=self.cp)
+            qjj, djj, cjj, rj = ans
+
+            # TODO: The inversion algorithm  is the bottleneck of the computation
+            # SciPy is very slow compared to MKL in Fortran...
+            lu, piv, info = dgetrf(qjj)
+            qjj, info = dgetri(lu, piv)
+
+            _ = matrix_after_inversion(
+                k=k,
+                qjj=qjj,
+                djj=djj,
+                cjj=cjj,
+                rj=rj,
+                sjk=sjk,
+                tjk=tjk)
+
+        tref, qref, uref = upward_sweep(
+            jmax=self.nlat,
+            jb=self.eq_boundary_index,
+            sjk=sjk,
+            tjk=tjk,
+            ckref=ckref,
+            tb=self._domain_average_storage.tn0,
+            qref_over_cor=qref_over_sin,
+            a=self.planet_radius,
+            om=self.omega,
+            dz=self.dz,
+            h=self.scale_height,
+            rr=self.dry_gas_constant,
+            cp=self.cp)
+
+        # return qref, uref, tref, fawa, ubar, tbar
+        return qref_over_sin / (2. * self.omega), uref, tref, fawa, ubar, tbar
+
+    @property
+    def static_stability(self) -> Tuple[np.array, np.array]:
+        """
+        The interpolated static stability.
+        """
+        if self.northern_hemisphere_results_only:
+            return self._domain_average_storage.static_stability_n
+        else:
+            return self._domain_average_storage.static_stability_s, self._domain_average_storage.static_stability_n
+
+    @property
+    def eq_boundary_index(self):
+        return self._eq_boundary_index
+
+    @property
+    def jd(self):
+        return self._jd
+
+    def _compute_intermediate_flux_terms(self):
+        """
+        Intermediate flux term computation for NHN 2022 GRL. Note that numerical instability is observed occasionally,
+        so please used with caution.
+
+        .. versionadded:: 0.7.0
+        """
+
+        # Turn qref back to correct unit
+
+        ylat_input = self.ylat[-self.equator_idx:] if self.northern_hemisphere_results_only else self.ylat
+        qref_correct_unit = self._reference_states_storage.qref_correct_unit(
+            ylat=ylat_input, omega=self.omega, python_indexing=False)
+
+        # === Compute barotropic flux terms (NHem) ===
+        self._barotropic_flux_terms_storage.lwa_baro_nhem, \
+            self._barotropic_flux_terms_storage.u_baro_nhem, \
+            urefbaro, \
+            self._barotropic_flux_terms_storage.ua1baro_nhem, \
+            self._barotropic_flux_terms_storage.ua2baro_nhem, \
+            self._barotropic_flux_terms_storage.ep1baro_nhem, \
+            self._barotropic_flux_terms_storage.ep2baro_nhem, \
+            self._barotropic_flux_terms_storage.ep3baro_nhem, \
+            self._barotropic_flux_terms_storage.ep4_nhem, \
+            astar1, \
+            astar2 = \
+            compute_flux_dirinv_nshem(
+                pv=self._interpolated_field_storage.qgpv,
+                uu=self._interpolated_field_storage.interpolated_u,
+                vv=self._interpolated_field_storage.interpolated_v,
+                pt=self._interpolated_field_storage.interpolated_theta,
+                tn0=self._domain_average_storage.tn0,
+                qref=qref_correct_unit[-self.equator_idx:],
+                uref=self._reference_states_storage.uref_nhem,
+                tref=self._reference_states_storage.ptref_nhem,
+                jb=self.eq_boundary_index,
+                is_nhem=True,
+                a=self.planet_radius,
+                om=self.omega,
+                dz=self.dz,
+                h=self.scale_height,
+                rr=self.dry_gas_constant,
+                cp=self.cp,
+                prefac=self.prefactor)
+        self._lwa_storage.lwa_nhem = np.abs(astar1 + astar2)
+
+        # === Compute barotropic flux terms (SHem) ===
+        # TODO: check signs!
+        if not self.northern_hemisphere_results_only:
+            self._barotropic_flux_terms_storage.lwa_baro[:, :self.equator_idx], \
+                self._barotropic_flux_terms_storage.u_baro[:, :self.equator_idx], \
+                urefbaro, \
+                self._barotropic_flux_terms_storage.ua1baro[:, :self.equator_idx], \
+                self._barotropic_flux_terms_storage.ua2baro[:, :self.equator_idx], \
+                self._barotropic_flux_terms_storage.ep1baro[:, :self.equator_idx], \
+                self._barotropic_flux_terms_storage.ep2baro[:, :self.equator_idx], \
+                self._barotropic_flux_terms_storage.ep3baro[:, :self.equator_idx], \
+                self._barotropic_flux_terms_storage.ep4[:, :self.equator_idx], \
+                astar1, \
+                astar2 = \
+                compute_flux_dirinv_nshem(
+                    pv=self._interpolated_field_storage.qgpv,
+                    uu=self._interpolated_field_storage.interpolated_u,
+                    vv=self._interpolated_field_storage.interpolated_v,
+                    pt=self._interpolated_field_storage.interpolated_theta,
+                    tn0=self._domain_average_storage.ts0,
+                    qref=qref_correct_unit[:self.equator_idx],
+                    uref=self._reference_states_storage.uref_shem,
+                    tref=self._reference_states_storage.ptref_shem,
+                    jb=self.eq_boundary_index,
+                    is_nhem=False,
+                    a=self.planet_radius,
+                    om=self.omega,
+                    dz=self.dz,
+                    h=self.scale_height,
+                    rr=self.dry_gas_constant,
+                    cp=self.cp,
+                    prefac=self.prefactor)
+            self._lwa_storage.lwa[:, :self.equator_idx, :] = np.abs(astar1 + astar2)
+
+    def _compute_lwa_flux_dirinv(self, qref, uref, tref):
+        """
+        Added for NHN 2022 GRL
+
+        .. versionadded:: 0.6.0
+        """
+        ans = compute_flux_dirinv_nshem(
+            pv=self._interpolated_field_storage.qgpv,
+            uu=self._interpolated_field_storage.interpolated_u,
+            vv=self._interpolated_field_storage.interpolated_v,
+            pt=self._interpolated_field_storage.interpolated_theta,
+            tn0=self._domain_average_storage.tn0,
+            qref=qref,
+            uref=uref,
+            tref=tref,
+            jb=self.eq_boundary_index,
+            is_nhem=True,
+            a=self.planet_radius,
+            om=self.omega,
+            dz=self.dz, h=self.scale_height, rr=self.dry_gas_constant, cp=self.cp, prefac=self.prefactor)
+        # astarbaro, u_baro, urefbaro, ua1baro, ua2baro, ep1baro, ep2baro, ep3baro, ep4baro, astar1, astar2 = ans
+        return ans
```

### Comparing `hn2016_falwa-0.6.6/hn2016_falwa/utilities.py` & `hn2016_falwa-0.7.0/hn2016_falwa/utilities.py`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.6/hn2016_falwa/wrapper.py` & `hn2016_falwa-0.7.0/hn2016_falwa/wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 ------------------------------------------
 File name: wrapper.py
 Author: Clare Huang
 """
 import numpy as np
 from hn2016_falwa.constant import EARTH_RADIUS
+from hn2016_falwa import basis
 
 
 def barotropic_eqlat_lwa(ylat, vort, area, dmu, n_points, planet_radius=EARTH_RADIUS):
     """
     Compute equivalent latitude and wave activity on a barotropic sphere.
 
     Parameters
@@ -29,26 +30,27 @@
     Returns
     -------
     qref : numpy.array
         1-d numpy array of value Q(y) where latitude y is given by ylat; dimension = (nlat).
     lwa_result : numpy.ndarray
         2-d numpy array of local wave activity values;
                     dimension = [nlat_s x nlon]
-    """
-
-    from hn2016_falwa import basis
 
+    Examples
+    --------
+    :doc:`Example Notebook <notebooks/Example_barotropic>`
+    """
     nlat = vort.shape[0]
     nlon = vort.shape[1]
     if n_points is None:
         n_points = nlat
 
-    qref, dummy = basis.eqvlat(ylat, vort, area, n_points,
-                               planet_radius=planet_radius)
-    lwa_result, dummy = basis.lwa(nlon, nlat, vort, qref, dmu)
+    qref, fawa = basis.eqvlat_fawa(
+        ylat, vort, area, n_points)
+    lwa_result, _ = basis.lwa(nlon, nlat, vort, qref, dmu)
 
     return qref, lwa_result
 
 
 def barotropic_input_qref_to_compute_lwa(ylat, qref, vort, area, dmu, planet_radius=EARTH_RADIUS):
 
     """
@@ -70,15 +72,14 @@
         radius of spherical planet of interest consistent with input 'area'.
 
     Returns
     -------
     lwa_result : numpy.ndarray
         2-d numpy array of local wave activity values; dimension = [nlat_s x nlon]
     """
-    from hn2016_falwa import basis
     nlat = vort.shape[0]
     nlon = vort.shape[1]
     lwa_result = basis.lwa(nlon, nlat, vort, qref, dmu)
     return lwa_result
 
 
 def eqvlat_hemispheric(ylat, vort, area, nlat_s=None, n_points=None, planet_radius=EARTH_RADIUS):
@@ -103,33 +104,31 @@
 
     Returns
     -------
     q_part : numpy.ndarray
         1-d numpy array of value Q(y) where latitude y is given by ylat; dimension = (nlat).
 
     """
-    from hn2016_falwa import basis
-
     nlat = vort.shape[0]
     qref = np.zeros(nlat)
 
     if nlat_s is None:
         nlat_s = nlat // 2
 
     if n_points is None:
         n_points = nlat_s
 
     # --- Southern Hemisphere ---
-    qref1, _ = basis.eqvlat(ylat[:nlat_s], vort[:nlat_s, :], area[:nlat_s, :],
+    qref1, _ = basis.eqvlat_fawa(ylat[:nlat_s], vort[:nlat_s, :], area[:nlat_s, :],
                             n_points, planet_radius=planet_radius)
     qref[:nlat_s] = qref1
 
     # --- Northern Hemisphere ---
     vort2 = -vort[::-1, :]
-    qref2, _ = basis.eqvlat(ylat[:nlat_s], vort2[:nlat_s, :], area[:nlat_s, :],
+    qref2, _ = basis.eqvlat_fawa(ylat[:nlat_s], vort2[:nlat_s, :], area[:nlat_s, :],
                             n_points, planet_radius=planet_radius)
     qref[-nlat_s:] = qref2[::-1]
 
     return qref
 
 
 def eqvlat_bracket_hemispheric(ylat, vort, area, nlat_s=None, n_points=None, planet_radius=EARTH_RADIUS, vgrad=None):
@@ -159,36 +158,34 @@
     q_part : numpy.ndarray
         1-d numpy array of value Q(y) where latitude y is given by ylat; dimension = (nlat).
     brac : numpy.ndarray or None
         1-d numpy array of averaged vgrad in the square bracket.
         If *vgrad* = None, *brac* = None.
 
     """
-    from hn2016_falwa import basis
-
     nlat = vort.shape[0]
     qref = np.zeros(nlat)
     brac = np.zeros(nlat)
 
     if nlat_s is None:
         nlat_s = nlat // 2
 
     if n_points is None:
         n_points = nlat_s
 
     # --- Southern Hemisphere ---
-    qref1, brac1 = basis.eqvlat(ylat[:nlat_s], vort[:nlat_s, :],
+    qref1, brac1 = basis.eqvlat_fawa(ylat[:nlat_s], vort[:nlat_s, :],
                                 area[:nlat_s, :],
                                 n_points, planet_radius=planet_radius,
                                 vgrad=vgrad)
     qref[:nlat_s] = qref1
 
     # --- Northern Hemisphere ---
     vort2 = -vort[::-1, :]
-    qref2, brac2 = basis.eqvlat(ylat[:nlat_s], vort2[:nlat_s, :],
+    qref2, brac2 = basis.eqvlat_fawa(ylat[:nlat_s], vort2[:nlat_s, :],
                                 area[:nlat_s, :],
                                 n_points, planet_radius=planet_radius,
                                 vgrad=vgrad)
 
     qref[-nlat_s:] = qref2[::-1]
 
     brac[:nlat_s] = brac1
@@ -225,44 +222,43 @@
     -------
     qref : numpy.ndarray
         1-d numpy array of value Q(y) where latitude y is given by ylat; dimension = (nlat).
     lwa_result : numpy.ndarray
         2-d numpy array of local wave activity values;
                     dimension = [nlat_s x nlon]
 
+    Examples
+    --------
+    :doc:`Example Notebook <notebooks/Example_qgpv>`
     """
-
-    from hn2016_falwa import basis
-
     nlat = vort.shape[0]
     nlon = vort.shape[1]
 
     if nlat_s is None:
         nlat_s = nlat // 2
 
     if n_points is None:
         n_points = nlat_s
 
     qref = np.zeros(nlat)
     lwa_result = np.zeros((nlat, nlon))
 
     # --- Southern Hemisphere ---
-    qref1, _ = basis.eqvlat(ylat[:nlat_s], vort[:nlat_s, :],
-                            area[:nlat_s, :],
-                            n_points, planet_radius=planet_radius)
+    qref1, _ = basis.eqvlat_fawa(
+        ylat[:nlat_s], vort[:nlat_s, :], area[:nlat_s, :], n_points, planet_radius=planet_radius)
     qref[:nlat_s] = qref1
     lwa_result[:nlat_s, :], _ = basis.lwa(nlon, nlat_s,
                                           vort[:nlat_s, :],
                                           qref1, dmu[:nlat_s])
 
     # --- Northern Hemisphere ---
     vort2 = -vort[::-1, :]
     # Added the minus sign, but gotta see if NL_North is affected
-    qref2, _ = basis.eqvlat(ylat[:nlat_s], vort2[:nlat_s, :], area[:nlat_s, :],
-                            n_points, planet_radius=planet_radius)
+    qref2, _ = basis.eqvlat_fawa(
+        ylat[:nlat_s], vort2[:nlat_s, :], area[:nlat_s, :], n_points, planet_radius=planet_radius)
     qref[-nlat_s:] = -qref2[::-1]
     lwa_result[-nlat_s:, :], _ = basis.lwa(nlon, nlat_s,
                                            vort[-nlat_s:, :],
                                            qref[-nlat_s:],
                                            dmu[-nlat_s:])
     return qref, lwa_result
 
@@ -301,44 +297,41 @@
         1-d numpy array of value Q(y) where latitude y is given by ylat; dimension = (nlat).
     lwa_result : numpy.ndarray
         2-d numpy array of local wave activity values; dimension = (nlat, nlon).
     capsigma: numpy.ndarray
         2-d numpy array of non-conservative force contribution value; dimension = (nlat, nlon).
 
     """
-
-    from hn2016_falwa import basis
-
     nlat = vort.shape[0]
     nlon = vort.shape[1]
 
     if nlat_s is None:
         nlat_s = nlat // 2
 
     if n_points is None:
         n_points = nlat_s
 
     qref = np.zeros(nlat)
     lwa_result = np.zeros((nlat, nlon))
     capsigma = np.zeros((nlat, nlon))
 
     # --- Southern Hemisphere ---
-    qref1, _ = basis.eqvlat(ylat[:nlat_s],
+    qref1, _ = basis.eqvlat_fawa(ylat[:nlat_s],
                             vort[:nlat_s, :], area[:nlat_s, :],
                             n_points, planet_radius=planet_radius)
     qref[:nlat_s] = qref1
     lwa_result[:nlat_s, :], \
     capsigma[:nlat_s, :] = basis.lwa(nlon, nlat_s, vort[:nlat_s, :],
                                      qref1, dmu[:nlat_s],
                                      ncforce=ncforce[:nlat_s, :])
 
     # --- Northern Hemisphere ---
     vort2 = -vort[::-1, :]
     # Added the minus sign, but gotta see if NL_North is affected
-    qref2, _ = basis.eqvlat(ylat[:nlat_s], vort2[:nlat_s, :], area[:nlat_s, :],
+    qref2, _ = basis.eqvlat_fawa(ylat[:nlat_s], vort2[:nlat_s, :], area[:nlat_s, :],
                             n_points, planet_radius=planet_radius)
     qref[-nlat_s:] = -qref2[::-1]
     lwa_result[-nlat_s:, :], \
     capsigma[-nlat_s:, :] = basis.lwa(nlon, nlat_s, vort[-nlat_s:, :],
                                       qref[-nlat_s:], dmu[-nlat_s:],
                                       ncforce=ncforce[-nlat_s:, :])
     return qref, lwa_result, capsigma
@@ -383,17 +376,14 @@
         1-d numpy array of <...>_Q(y) in NZ10 where latitude y is given by ylat; dimension = (nlat).
     (3) lwa_result : numpy.ndarray
         2-d numpy array of local wave activity values; dimension = (nlat, nlon).
     (4) capsigma: numpy.ndarray
         2-d numpy array of non-conservative force contribution value; dimension = (nlat, nlon).
 
     """
-
-    from hn2016_falwa import basis
-
     nlat = vort.shape[0]
     nlon = vort.shape[1]
 
     if nlat_s is None:
         nlat_s = nlat // 2
 
     if n_points is None:
@@ -404,19 +394,19 @@
     if ncforce is not None:
         capsigma = np.zeros((nlat, nlon))
     if vgrad is not None:
         brac_result = np.zeros(nlat)
 
     # --- Southern Hemisphere ---
     if vgrad is None:
-        qref1, brac = basis.eqvlat(ylat[:nlat_s], vort[:nlat_s, :],
+        qref1, brac = basis.eqvlat_fawa(ylat[:nlat_s], vort[:nlat_s, :],
                                    area[:nlat_s, :],
                                    n_points, planet_radius=planet_radius)
     else:
-        qref1, brac = basis.eqvlat(ylat[:nlat_s], vort[:nlat_s, :],
+        qref1, brac = basis.eqvlat_fawa(ylat[:nlat_s], vort[:nlat_s, :],
                                    area[:nlat_s, :],
                                    n_points, planet_radius=planet_radius,
                                    vgrad=vgrad[:nlat_s, :])
 
     qref[:nlat_s] = qref1
     if vgrad is not None:
         brac_result[:nlat_s] = brac
@@ -432,20 +422,20 @@
                                               qref1, dmu[:nlat_s])
 
     # --- Northern Hemisphere ---
     vort2 = -vort[::-1, :]
     # Added the minus sign, but gotta see if NL_North is affected
 
     if vgrad is None:
-        qref2, brac = basis.eqvlat(ylat[:nlat_s], vort2[:nlat_s, :],
+        qref2, brac = basis.eqvlat_fawa(ylat[:nlat_s], vort2[:nlat_s, :],
                                    area[:nlat_s, :],
                                    n_points, planet_radius=planet_radius)
     else:
         vgrad2 = -vgrad[::-1, :]  # Is this correct?
-        qref2, brac = basis.eqvlat(ylat[:nlat_s], vort2[:nlat_s, :],
+        qref2, brac = basis.eqvlat_fawa(ylat[:nlat_s], vort2[:nlat_s, :],
                                    area[:nlat_s, :],
                                    n_points, planet_radius=planet_radius,
                                    vgrad=vgrad2[:nlat_s, :])
 
     qref[-nlat_s:] = -qref2[::-1]
     if vgrad is not None:
         brac_result[-nlat_s:] = -brac[::-1]
@@ -498,16 +488,14 @@
         radius of spherical planet of interest consistent with input 'area'.
 
     Returns
     -------
     lwa_result : numpy.ndarray
         2-d numpy array of local wave activity values; dimension = (nlat, nlon).
     """
-    from hn2016_falwa import basis
-
     nlat = vort.shape[0]
     nlon = vort.shape[1]
     if nlat_s is None:
         nlat_s = nlat // 2
 
     lwa_result = np.zeros((nlat, nlon))
 
@@ -546,37 +534,35 @@
     -------
     qref : numpy.array
         1-d numpy array of value reference potential temperature *Theta(y)* approximated by box counting method, where latitude y is given by ylat; dimension = (nlat).
     lwa_result : numpy.ndarray
         2-d numpy array of local surface wave activity values; dimension = (nlat, nlon).
 
     """
-    from hn2016_falwa import basis
-
     nlat = theta.shape[0]
     nlon = theta.shape[1]
     if nlat_s is None:
         nlat_s = nlat // 2
     if n_points is None:
         n_points = nlat_s
 
     qref = np.zeros(nlat)
     lwa_result = np.zeros((nlat, nlon))
 
     # --- southern Hemisphere ---
-    qref[:nlat_s], brac = basis.eqvlat(ylat[:nlat_s], theta[:nlat_s, :],
+    qref[:nlat_s], brac = basis.eqvlat_fawa(ylat[:nlat_s], theta[:nlat_s, :],
                                        area[:nlat_s, :], n_points,
                                        planet_radius=planet_radius)
     lwa_result[:nlat_s, :], dummy = basis.lwa(nlon, nlat_s, theta[:nlat_s, :],
                                               qref[:nlat_s], dmu[:nlat_s])
 
     # --- northern Hemisphere ---
     theta2 = theta[::-1, :]
     # Added the minus sign, but gotta see if NL_north is affected
-    qref2, brac = basis.eqvlat(ylat[:nlat_s], theta2[:nlat_s, :],
+    qref2, brac = basis.eqvlat_fawa(ylat[:nlat_s], theta2[:nlat_s, :],
                                area[:nlat_s, :],
                                n_points, planet_radius=planet_radius)
     qref[-nlat_s:] = qref2[::-1]
     lwa_result[-nlat_s:, :], dummy = basis.lwa(nlon, nlat_s,
                                                theta[-nlat_s:, :],
                                                qref[-nlat_s:],
                                                dmu[-nlat_s:])
```

### Comparing `hn2016_falwa-0.6.6/hn2016_falwa/xarrayinterface.py` & `hn2016_falwa-0.7.0/hn2016_falwa/xarrayinterface.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Author: Christopher Polster
 """
 import functools
 import numpy as np
 import xarray as xr
 
 from hn2016_falwa import __version__
-from hn2016_falwa.oopinterface import QGField
+from hn2016_falwa.oopinterface import QGFieldNH18
 
 
 def _is_ascending(arr):
     return np.all(np.diff(arr) > 0)
 
 def _is_descending(arr):
     return np.all(np.diff(arr) < 0)
@@ -31,142 +31,210 @@
 _NAMES_T = ["t", "T"]
 # Budget terms name lookup
 _NAMES_LWA  = ["lwa_baro"]
 _NAMES_CZAF = ["convergence_zonal_advective_flux"]
 _NAMES_DEMF = ["divergence_eddy_momentum_flux"]
 _NAMES_MHF  = ["meridional_heat_flux"]
 
+
+def _get_dataarray(data, names, user_names=None):
+    name = _get_name(data, names, user_names=None)
+    return data[name]
+
+
 def _get_name(ds, names, user_names=None):
     # If the first name from the list of defaults is in the user-provided
     # dictionary, use the name provided there
     if user_names is not None and names[0] in user_names:
         name = user_names[names[0]]
         if name not in ds:
             raise KeyError(f"specified variable '{name}' not found")
         return name
     # Else, search in default list of names
     for name in names:
         if name in ds:
             return name
     raise KeyError(f"no matching variable for '{names[0]}' found")
 
+
 def _map_collect(f, xs, names, postprocess=None):
     out = { name: [] for name in names }
     for x in xs:
         for name, y in zip(names, f(x)):
             out[name].append(y)
     if postprocess is not None:
         for name in names:
             out[name] = postprocess(out[name])
     return out
 
 
+class _DataArrayCollector(property):
+    # Getter properties for DataArray-based access to QGField properties.
+    # Inherits from property, so instances are recognized as properties by
+    # sphinx for the docs.
+
+    def __init__(self, name, dimnames, dimvars=None):
+        self.name = name
+        self.dimnames = dimnames
+        self.dimvars = dimvars if dimvars is not None else dimnames
+        self.__doc__ = (
+            f"See :py:attr:`oopinterface.QGField.{name}`."
+            "\n\nReturns\n-------\nxarray.DataArray"
+        )
+
+    def __get__(self, obj, objtype=None):
+        fields = obj.fields
+        data = np.asarray([getattr(field, self.name) for field in fields])
+        coords = ({
+            coord: getattr(fields[0], var)
+            for coord, var in zip(self.dimnames, self.dimvars)
+        })
+        coords.update(obj._other_coords)
+        dims = (*obj._other_dims, *self.dimnames)
+        shape = (*obj._other_shape, *(getattr(fields[0], var).size for var in self.dimvars))
+        return xr.DataArray(data.reshape(shape), coords, dims, self.name, obj.attrs)
+
+
 class QGDataset:
     """A wrapper for multiple QGField objects with xarray in- and output.
 
-    Examines the given dataset and tries to extract `u`, `v`, and `T` fields
-    based on the names of coordinates in the dataset. For each combination of
-    timestep, ensemble member, etc., a :py:class:`oopinterface.QGField` object
-    is instanciated. The constructor will automatically flip latitude and
-    pressure dimensions of the input data if necessary to meet the requirements
-    of QGField.
+    For each combination of timestep, ensemble member, etc. in the input data,
+    a :py:class:`oopinterface.QGField` object is instanciated. The constructor
+    will automatically flip latitude and pressure dimensions of the input data
+    if necessary to meet the requirements of QGField.
 
     This wrapper class imitates the methods of QGField (but not the
     properties/attributes) and collects and re-organizes output data in xarray
     Datasets for convenience. All calculations are performed by the QGField
     routines.
 
     .. versionadded:: 0.6.1
 
     Parameters
     ----------
-    ds : xarray.Dataset
-        Input dataset. Must contain 3D fields of zonal wind, meridional wind
-        and temperature. The 3D fields's dimensions must end with height,
-        latitude and longitude. Other dimensions (e.g. time, ensemble member
-        id) are preserved in the output datasets.
-    qgfield_args : tuple, optional
-        Positional arguments given to the QGField constructor.
-    qgfield_kwargs : dict, optional
-        Keyword arguments given to the QGField constructor.
+    da_u : xarray.DataArray | xarray.Dataset
+        Input 3D fields of zonal wind. The 3D fields's dimensions must end with
+        height, latitude and longitude. Other dimensions (e.g. time, ensemble
+        member id) are preserved in the output datasets.
+        Alternatively, a dataset can be given, from which `u`, `v` and `T`
+        fields are then extracted. The `da_v` and `da_t` arguments can then be
+        omitted or used as an override.
+    da_v : xarray.DataArray, optional
+        Input 3D fields of meridional wind. The 3D fields's dimensions must end
+        with height, latitude and longitude. Other dimensions (e.g. time,
+        ensemble member id) are preserved in the output datasets.
+    da_t : xarray.DataArray, optional
+        Input 3D fields of temperature. The 3D fields's dimensions must end
+        with height, latitude and longitude. Other dimensions (e.g. time,
+        ensemble member id) are preserved in the output datasets.
     var_names : dict, optional
         If the auto-detection of variable or coordinate names fails, provide
         a lookup table that maps `plev`, `ylat`, `xlon`, `u`, `v` and/or `t` to
         the names used in the dataset.
+    qgfield : QGField class, optional
+        The QGField class to use in the computation. Default:
+        :py:class:`oopinterface.QGFieldNH18`.
+    qgfield_args : tuple, optional
+        Positional arguments given to the QGField constructor.
+    qgfield_kwargs : dict, optional
+        Keyword arguments given to the QGField constructor.
 
-    Example
+    Examples
     -------
-    >>> data = xarray.load_dataset("path/to/some/uvt-data.nc")
+    >>> data = xarray.open_dataset("path/to/some/uvt-data.nc")
     >>> qgds = QGDataset(data)
+    >>> qgds.interpolate_fields()
+    <xarray.Dataset> ...
+
+    :doc:`notebooks/demo_script_for_nh2018_with_xarray`
+
+    >>> data_u = xarray.load_dataset("path/to/some/u-data.nc")
+    >>> data_v = xarray.load_dataset("path/to/some/v-data.nc")
+    >>> data_t = xarray.load_dataset("path/to/some/t-data.nc")
+    >>> qgds = QGDataset(data_u, data_v, data_t)
     """
 
-    def __init__(self, ds, qgfield_args=None, qgfield_kwargs=None, var_names=None):
+    def __init__(self, da_u, da_v=None, da_t=None, *, var_names=None,
+                 qgfield=QGFieldNH18, qgfield_args=None, qgfield_kwargs=None):
         if var_names is None:
             var_names = dict()
-        self._ds = ds
-        self._qgfield_args   = list() if qgfield_args   is None else qgfield_args
+        # Also support construction from single-arg and mixed variants
+        if isinstance(da_u, xr.Dataset):
+            # Fill up missing DataArrays for v and t from the Dataset but give
+            # priority to existing v and t fields from the args
+            if da_v is None:
+                da_v = _get_dataarray(da_u, _NAMES_V, var_names)
+            if da_t is None:
+                da_t = _get_dataarray(da_u, _NAMES_T, var_names)
+            # Always take u
+            da_u = _get_dataarray(da_u, _NAMES_U, var_names)
+        # Assertions about da_u, da_v, da_t
+        assert da_u is not None, "missing u field"
+        assert da_v is not None, "missing v field"
+        assert da_t is not None, "missing t field"
+        # Assign standard names to the input fields
+        da_u = da_u.rename("u")
+        da_v = da_v.rename("v")
+        da_t = da_t.rename("t")
+        # Merge into one dataset and keep the reference. xarray will avoid
+        # copying the data in the merge, so the operation should be relatively
+        # cheap and fast. The merge further verifies that the coordinates of
+        # the three DataArrays match.
+        self._ds = xr.merge([da_u, da_v, da_t], join="exact", compat="equals")
+        # QGField* configuration
+        self._qgfield = qgfield
+        self._qgfield_args = list() if qgfield_args is None else qgfield_args
         self._qgfield_kwargs = dict() if qgfield_kwargs is None else qgfield_kwargs
-        # Find names of spatial coordinates
-        self._plev_name = _get_name(ds, _NAMES_PLEV, var_names)
-        self._ylat_name = _get_name(ds, _NAMES_YLAT, var_names)
-        self._xlon_name = _get_name(ds, _NAMES_XLON, var_names)
-        # Find names of wind and temperature fields
-        self._u_name = _get_name(ds, _NAMES_U, var_names)
-        self._v_name = _get_name(ds, _NAMES_V, var_names)
-        self._t_name = _get_name(ds, _NAMES_T, var_names)
-        # Shorthands for data arrays
-        plev = ds[self._plev_name]
-        ylat = ds[self._ylat_name]
-        xlon = ds[self._xlon_name]
-        u = ds[self._u_name]
-        v = ds[self._v_name]
-        t = ds[self._t_name]
+        # Extract spatial coordinates
+        da_plev = _get_dataarray(self._ds.coords, _NAMES_PLEV, var_names)
+        da_ylat = _get_dataarray(self._ds.coords, _NAMES_YLAT, var_names)
+        da_xlon = _get_dataarray(self._ds.coords, _NAMES_XLON, var_names)
         # Check that field coordinates end in lev, lat, lon
-        assert u.dims[-3] == plev.name, f"dimension -3 of input fields must be '{plev.name}' (plev)"
-        assert u.dims[-2] == ylat.name, f"dimension -2 of input fields must be '{ylat.name}' (ylat)"
-        assert u.dims[-1] == xlon.name, f"dimension -1 of input fields must be '{xlon.name}' (xlon)"
-        assert u.dims == v.dims, f"dimensions of fields '{u.name}' (u) and '{v.name}' (v) don't match"
-        assert u.dims == t.dims, f"dimensions of fields '{u.name}' (u) and '{t.name}' (t) don't match"
+        assert da_u.dims[-3] == da_plev.name, f"dimension -3 of input fields must be '{da_plev.name}' (plev)"
+        assert da_u.dims[-2] == da_ylat.name, f"dimension -2 of input fields must be '{da_ylat.name}' (ylat)"
+        assert da_u.dims[-1] == da_xlon.name, f"dimension -1 of input fields must be '{da_xlon.name}' (xlon)"
+        assert da_u.dims == da_v.dims, f"dimensions of fields '{da_u.name}' (u) and '{da_v.name}' (v) don't match"
+        assert da_u.dims == da_t.dims, f"dimensions of fields '{da_u.name}' (u) and '{da_t.name}' (t) don't match"
         # The input data may contain multiple time steps, ensemble members etc.
         # Flatten all these other dimensions so a single loop covers all
         # fields. These dimensions are restored in the output datasets.
-        self._other_dims = u.dims[:-3]
-        self._other_shape = tuple(ds[dim].size for dim in self._other_dims)
+        self._other_dims = da_u.dims[:-3]
+        self._other_shape = tuple(da_u[dim].size for dim in self._other_dims)
         self._other_size = np.product(self._other_shape, dtype=np.int64)
-        _shape = (self._other_size, *u.shape[-3:])
+        _shape = (self._other_size, *da_u.shape[-3:])
         # Extract value arrays and collapse all additional dimensions
-        u = u.data.reshape(_shape)
-        v = v.data.reshape(_shape)
-        t = t.data.reshape(_shape)
+        u = da_u.data.reshape(_shape)
+        v = da_v.data.reshape(_shape)
+        t = da_t.data.reshape(_shape)
         # Automatically determine how fields need to be flipped so they match
         # the requirements of QGField and extract coordinate values
         flip = []
         # Ensure that ylat is ascending
-        ylat = ylat.values
+        ylat = da_ylat.values
         if not _is_ascending(ylat):
             ylat = np.flip(ylat)
             flip.append(-2)
         # Ensure that plev is descending
-        plev = plev.values
+        plev = da_plev.values
         if not _is_descending(plev):
             plev = np.flip(plev)
             flip.append(-3)
         # Ordering of xlon doesn't matter here
-        xlon = xlon.values
+        xlon = da_xlon.values
         # Create a QGField object for each combination of timestep, ensemble
         # member, etc.
         self._fields = []
         for u_field, v_field, t_field in zip(u, v, t):
             # Apply reordering to fields
             if flip:
                 u_field = np.flip(u_field, axis=flip)
                 v_field = np.flip(v_field, axis=flip)
                 t_field = np.flip(t_field, axis=flip)
-            field = QGField(xlon, ylat, plev, u_field, v_field, t_field,
-                            *self._qgfield_args, **self._qgfield_kwargs)
+            field = self._qgfield(xlon, ylat, plev, u_field, v_field, t_field,
+                                  *self._qgfield_args, **self._qgfield_kwargs)
             self._fields.append(field)
         # Make sure there is at least one field in the dataset
         assert self._fields, "empty input"
 
     @property
     def fields(self):
         """Access to the QGField objects created by the QGDataset.
@@ -174,15 +242,15 @@
         The :py:class:`.oopinterface.QGField` objects are stored in a flattened
         list.
         """
         return self._fields
 
     @property
     def _other_coords(self):
-        return { dim: self._ds[dim] for dim in self._other_dims}
+        return {dim: self._ds[dim] for dim in self._other_dims}
 
     @property
     def attrs(self):
         """Metadata dictionary that is attached to output datasets."""
         field = self._fields[0]
         return {
             "kmax": field.kmax,
@@ -193,82 +261,118 @@
             "rjac": field.rjac,
             "scale_height": field.scale_height,
             "cp": field.cp,
             "dry_gas_constant": field.dry_gas_constant,
             "omega": field.omega,
             "planet_radius": field.planet_radius,
             "prefactor": field.prefactor,
+            "protocol": self._qgfield.__name__,
             "package": f"hn2016_falwa {__version__}"
         }
 
     def interpolate_fields(self):
         """Collect the output of `interpolate_fields` in a dataset.
 
         See :py:meth:`.oopinterface.QGField.interpolate_fields`.
 
+        .. note::
+            A QGField class may define static stability globally or
+            hemispherically on each level. The output dataset contains a single
+            variable for static stability in case of a global definition and
+            two variables for static stability for a hemispheric definition
+            (suffix ``_n`` for the northern hemisphere and ``_s`` for the
+            southern hemisphere).
+
         Returns
         -------
         xarray.Dataset
         """
         # Call interpolate_fields on all QGField objects
         out_fields = _map_collect(
             lambda field: field.interpolate_fields(),
             self._fields,
-            ["qgpv", "interpolated_u", "interpolated_v", "theta", "static_stability"],
+            ["qgpv", "interpolated_u", "interpolated_v", "interpolated_theta", "static_stability"],
             postprocess=np.asarray
         )
         # Take the first field to extract coordinates and metadata
         _field = self.fields[0]
         # Prepare coordinate-related data for the output: interpolated data is
         # transferred onto the QG height grid, fields are functions of height,
         # latitude, longitude
         out_dims = (*self._other_dims, "height", "ylat", "xlon")
         out_shape = (*self._other_shape, _field.height.size, _field.ylat.size, _field.xlon.size)
+        # Special case: static stability (global for NH18, hemispheric for NHN22)
+        stability = out_fields["static_stability"]
+        data_vars_stability = {}
+        if stability.ndim == 2:
+            # One vertical profile of static stability per field: global
+            data_vars_stability["static_stability"] = (out_dims[:-2], stability.reshape(out_shape[:-2]))
+        elif stability.ndim == 3 and stability.shape[-2] == 2:
+            # Two vertical profiles of static stability per field: hemispheric
+            data_vars_stability["static_stability_n"] = (out_dims[:-2], stability[:,0,:].reshape(out_shape[:-2]))
+            data_vars_stability["static_stability_s"] = (out_dims[:-2], stability[:,1,:].reshape(out_shape[:-2]))
+        else:
+            raise ValueError(f"cannot process shape of returned static stability field: {stability.shape}")
         # Combine all outputs into a dataset, reshape to restore the original
         # other dimensions that were flattened earlier
         return xr.Dataset(
             data_vars={
                 "qgpv": (out_dims, out_fields["qgpv"].reshape(out_shape)),
                 "interpolated_u": (out_dims, out_fields["interpolated_u"].reshape(out_shape)),
                 "interpolated_v": (out_dims, out_fields["interpolated_v"].reshape(out_shape)),
-                "theta": (out_dims, out_fields["theta"].reshape(out_shape)),
-                "static_stability": (out_dims[:-2], out_fields["static_stability"].reshape(out_shape[:-2]))
+                "interpolated_theta": (out_dims, out_fields["interpolated_theta"].reshape(out_shape)),
+                **data_vars_stability
             },
             coords={
                 **self._other_coords,
                 "height": _field.height,
                 "ylat": _field.ylat,
                 "xlon": _field.xlon,
             },
             attrs=self.attrs
         )
 
-    def compute_reference_states(self, northern_hemisphere_results_only=False):
+    # Accessors for individual field properties computed in interpolate_fields
+    qgpv = _DataArrayCollector(
+        "qgpv",
+        ["height", "ylat", "xlon"]
+    )
+    interpolated_u = _DataArrayCollector(
+        "interpolated_u",
+        ["height", "ylat", "xlon"]
+    )
+    interpolated_v = _DataArrayCollector(
+        "interpolated_v",
+        ["height", "ylat", "xlon"]
+    )
+    interpolated_theta = _DataArrayCollector(
+        "interpolated_theta",
+        ["height", "ylat", "xlon"]
+    )
+
+    def compute_reference_states(self):
         """Collect the output of `compute_reference_states` in a dataset.
 
         See :py:meth:`.oopinterface.QGField.compute_reference_states`.
 
         Returns
         -------
         xarray.Dataset
         """
         # Call compute_reference_states on all QGField objects
         out_fields = _map_collect(
-            lambda field: field.compute_reference_states(northern_hemisphere_results_only),
+            lambda field: field.compute_reference_states(),
             self._fields,
             ["qref", "uref", "ptref"],
             postprocess=np.asarray
         )
         # Take the first field to extract coordinates and metadata
         _field = self.fields[0]
         # Prepare coordinate-related data for the output
-        if northern_hemisphere_results_only:
-            _ylat = _field.ylat[(_field.equator_idx - 1):]            
-        else:
-            _ylat = _field.ylat
+        _ylat = _field.ylat_ref_states
         # 2D data, function of height and latitude
         out_dims = (*self._other_dims, "height", "ylat")
         out_shape = (*self._other_shape, _field.height.size, _ylat.size)
         # Combine all outputs into a dataset, reshape to restore the original
         # other dimensions that were flattened earlier
         return xr.Dataset(
             data_vars={
@@ -280,39 +384,53 @@
                 **self._other_coords,
                 "height": _field.height,
                 "ylat": _ylat,
             },
             attrs=self.attrs
         )
 
-    def compute_lwa_and_barotropic_fluxes(self, northern_hemisphere_results_only=False):
+    # Accessors for individual field properties computed in compute_reference_states
+    qref = _DataArrayCollector(
+        "qref",
+        ["height", "ylat"],
+        ["height", "ylat_ref_states"]
+    )
+    uref = _DataArrayCollector(
+        "uref",
+        ["height", "ylat"],
+        ["height", "ylat_ref_states"]
+    )
+    ptref = _DataArrayCollector(
+        "ptref",
+        ["height", "ylat"],
+        ["height", "ylat_ref_states"]
+    )
+
+    def compute_lwa_and_barotropic_fluxes(self):
         """Collect the output of `compute_lwa_and_barotropic_fluxes` in a dataset.
 
         See :py:meth:`.oopinterface.QGField.compute_lwa_and_barotropic_fluxes`.
 
         Returns
         -------
         xarray.Dataset
         """
         # Call compute_lwa_and_barotropic_fluxes on all QGField objects
         out_fields = _map_collect(
-            lambda field: field.compute_lwa_and_barotropic_fluxes(northern_hemisphere_results_only),
+            lambda field: field.compute_lwa_and_barotropic_fluxes(),
             self._fields,
             ["adv_flux_f1", "adv_flux_f2", "adv_flux_f3", "convergence_zonal_advective_flux",
                 "divergence_eddy_momentum_flux", "meridional_heat_flux", "lwa_baro", "u_baro",
                 "lwa"],
             postprocess=np.asarray
         )
         # Take the first field to extract coordinates and metadata
         _field = self.fields[0]
         # Prepare coordinate-related data for the output
-        if northern_hemisphere_results_only:
-            _ylat = _field.ylat[(_field.equator_idx - 1):]            
-        else:
-            _ylat = _field.ylat
+        _ylat = _field.ylat_ref_states
         # 2D data, function of latitude and longitude
         out_dims_2d = (*self._other_dims, "ylat", "xlon")
         out_shape_2d = (*self._other_shape, _ylat.size, _field.xlon.size)
         # 3D data, function of height, latitude and longitude
         out_dims_3d = (*self._other_dims, "height", "ylat", "xlon")
         out_shape_3d = (*self._other_shape, _field.height.size, _ylat.size, _field.xlon.size)
         # Combine all outputs into a dataset, reshape to restore the original
@@ -334,163 +452,61 @@
                 "height": _field.height,
                 "ylat": _ylat,
                 "xlon": _field.xlon,
             },
             attrs=self.attrs
         )
 
-    # The new routines so far only seem to work for 1°-resolution data and the northern hemisphere
-
-    def _interpolate_field_dirinv(self):
-        # Call interpolate_field_dirinv on all QGField objects
-        out_fields = _map_collect(
-            lambda field: field._interpolate_field_dirinv(),
-            self._fields,
-            ["qgpv", "interpolated_u", "interpolated_v", "interpolated_avort",
-                "interpolated_theta", "static_stability_n", "static_stability_s",
-                "tn0", "ts0"],
-            postprocess=np.asarray
-        )
-        # Take the first field to extract coordinates and metadata
-        _field = self.fields[0]
-        # Prepare coordinate-related data for the output: interpolated data is
-        # transferred onto the QG height grid.
-        # 1D data, function of height only
-        out_dims_h = (*self._other_dims, "height")
-        out_shape_h = (*self._other_shape, _field.height.size)
-        # 3D data, function of longitude, latitude and height (plev and xlon
-        # dimensions are not swapped back in the dirinv routines currently)
-        out_dims_xyh = (*self._other_dims, "xlon", "ylat", "height")
-        out_shape_xyh = (*self._other_shape, _field.xlon.size, _field.ylat.size, _field.height.size)
-        # Combine all outputs into a dataset, reshape to restore the original
-        # other dimensions that were flattened earlier
-        return xr.Dataset(
-            data_vars={
-                "qgpv": (out_dims_xyh, out_fields["qgpv"].reshape(out_shape_xyh)),
-                "interpolated_u": (out_dims_xyh, out_fields["interpolated_u"].reshape(out_shape_xyh)),
-                "interpolated_v": (out_dims_xyh, out_fields["interpolated_v"].reshape(out_shape_xyh)),
-                "interpolated_avort": (out_dims_xyh, out_fields["interpolated_avort"].reshape(out_shape_xyh)),
-                "interpolated_theta": (out_dims_xyh, out_fields["interpolated_theta"].reshape(out_shape_xyh)),
-                "static_stability_n": (out_dims_h, out_fields["static_stability_n"].reshape(out_shape_h)),
-                "static_stability_s": (out_dims_h, out_fields["static_stability_s"].reshape(out_shape_h)),
-                "tn0": (out_dims_h, out_fields["tn0"].reshape(out_shape_h)),
-                "ts0": (out_dims_h, out_fields["ts0"].reshape(out_shape_h)),
-            },
-            coords={
-                **self._other_coords,
-                "height": _field.height,
-                "ylat": _field.ylat,
-                "xlon": _field.xlon,
-            },
-            attrs=self.attrs
-        )
-
-    def _compute_qref_fawa_and_bc(self):
-        # Call _compute_qref_fawa_and_bc on all QGField objects
-        out_fields = _map_collect(
-            lambda field: field._compute_qref_fawa_and_bc(),
-            self._fields,
-            ["qref", "u", "tref", "fawa", "ubar", "tbar"],
-            postprocess=np.asarray
-        )
-        # The output of _compute_qref_fawa_and_bc is currently not stored in
-        # the QGField object and must be given to _compute_lwa_flux_dirinv
-        # explicitly. Until a better solution is found in the QGField
-        # implementation, apply a monkey patch here: add the outputs of
-        # _compute_qref_fawa_and_bc as underscore-attributes to the QGField
-        # objects so they can be retrieved later.
-        for name, arrs in out_fields.items():
-            for field, arr in zip(self._fields, arrs):
-                setattr(field, "_temp_dirinv_" + name, arr)
-        # Take the first field to extract coordinates and metadata
-        _field = self.fields[0]
-        _nlat = _field.nlat // 2 + _field.nlat % 2
-        # Prepare coordinate-related data for the output: all outputs are
-        # functions of latitude and height
-        out_dims_yh = (*self._other_dims, "ylat", "height")
-        out_shape_yh = (*self._other_shape, _nlat, _field.height.size)
-        # Output fields u (=uref) and tref currently exclude the equator
-        # boundary points and are padded here for more convenient, consistent
-        # output array shapes.
-        _pad = functools.partial(
-            np.pad,
-            pad_width=[(0, 0), (_field.eq_boundary_index, 0), (0, 0)],
-            mode="constant",
-            constant_values=np.nan
-        )
-        # Combine all outputs into a dataset, reshape to restore the original
-        # other dimensions that were flattened earlier. u is returned under the
-        # name uref to avoid confusion about the content.
-        return xr.Dataset(
-            data_vars={
-                "qref": (out_dims_yh, out_fields["qref"].reshape(out_shape_yh)),
-                "uref": (out_dims_yh, _pad(out_fields["u"]).reshape(out_shape_yh)),
-                "tref": (out_dims_yh, _pad(out_fields["tref"]).reshape(out_shape_yh)),
-                "fawa": (out_dims_yh, out_fields["fawa"].reshape(out_shape_yh)),
-                "ubar": (out_dims_yh, out_fields["ubar"].reshape(out_shape_yh)),
-                "tbar": (out_dims_yh, out_fields["tbar"].reshape(out_shape_yh)),
-            },
-            coords={
-                **self._other_coords,
-                "height": _field.height,
-                "ylat": _field.ylat[-_nlat:],
-            },
-            attrs=self.attrs
-        )
-        return out_fields
+    # Accessors for individual field properties computed in compute_lwa_and_barotropic_fluxes
+    adv_flux_f1 = _DataArrayCollector(
+        "adv_flux_f1",
+        ["ylat", "xlon"],
+        ["ylat_ref_states", "xlon"]
+    )
+    adv_flux_f2 = _DataArrayCollector(
+        "adv_flux_f2",
+        ["ylat", "xlon"],
+        ["ylat_ref_states", "xlon"]
+    )
+    adv_flux_f3 = _DataArrayCollector(
+        "adv_flux_f3",
+        ["ylat", "xlon"],
+        ["ylat_ref_states", "xlon"]
+    )
+    convergence_zonal_advective_flux = _DataArrayCollector(
+        "convergence_zonal_advective_flux",
+        ["ylat", "xlon"],
+        ["ylat_ref_states", "xlon"]
+    )
+    divergence_eddy_momentum_flux = _DataArrayCollector(
+        "divergence_eddy_momentum_flux",
+        ["ylat", "xlon"],
+        ["ylat_ref_states", "xlon"]
+    )
+    meridional_heat_flux = _DataArrayCollector(
+        "meridional_heat_flux",
+        ["ylat", "xlon"],
+        ["ylat_ref_states", "xlon"]
+    )
+    lwa_baro = _DataArrayCollector(
+        "lwa_baro",
+        ["ylat", "xlon"],
+        ["ylat_ref_states", "xlon"]
+    )
+    u_baro = _DataArrayCollector(
+        "u_baro",
+        ["ylat", "xlon"],
+        ["ylat_ref_states", "xlon"]
+    )
+    lwa = _DataArrayCollector(
+        "lwa",
+        ["height", "ylat", "xlon"],
+        ["height", "ylat_ref_states", "xlon"]
+    )
 
-    def _compute_lwa_flux_dirinv(self):
-        # Call _compute_lwa_flux_dirinv on all QGField objects, use the monkey
-        # patched attributes added in _compute_qref_fawa_and_bc
-        out_fields = _map_collect(
-            lambda field: field._compute_lwa_flux_dirinv(qref=field._temp_dirinv_qref, uref=field._temp_dirinv_u,
-                                                         tref=field._temp_dirinv_tref),
-            self._fields,
-            ["astarbaro", "ubaro", "urefbaro", "ua1baro", "ua2baro", "ep1baro",
-                "ep2baro", "ep3baro", "ep4", "astar1", "astar2"],
-            postprocess=np.asarray
-        )
-        # Take the first field to extract coordinates and metadata
-        _field = self.fields[0]
-        _nlat = _field.nlat // 2 + _field.nlat % 2
-        # Prepare coordinate-related data for the output:
-        # 1D data, function of latitude only
-        out_dims_y = (*self._other_dims, "ylat")
-        out_shape_y = (*self._other_shape, _nlat)
-        # 2D data, function of longitude and latitude
-        out_dims_xy = (*self._other_dims, "xlon", "ylat")
-        out_shape_xy = (*self._other_shape, _field.xlon.size, _nlat)
-        # 3D data, function of longitude, latitude and height (again, xlon and
-        # plev are currently not swapped back in the dirinv routines)
-        out_dims_xyh = (*self._other_dims, "xlon", "ylat", "height")
-        out_shape_xyh = (*self._other_shape, _field.xlon.size, _nlat, _field.height.size)
-        # Combine all outputs into a dataset, reshape to restore the original
-        # other dimensions that were flattened earlier
-        return xr.Dataset(
-            data_vars={
-                "astarbaro": (out_dims_xy, out_fields["astarbaro"].reshape(out_shape_xy)),
-                "ubaro": (out_dims_xy, out_fields["ubaro"].reshape(out_shape_xy)),
-                "urefbaro": (out_dims_y, out_fields["urefbaro"].reshape(out_shape_y)),
-                "ua1baro": (out_dims_xy, out_fields["ua1baro"].reshape(out_shape_xy)),
-                "ua2baro": (out_dims_xy, out_fields["ua2baro"].reshape(out_shape_xy)),
-                "ep1baro": (out_dims_xy, out_fields["ep1baro"].reshape(out_shape_xy)),
-                "ep2baro": (out_dims_xy, out_fields["ep2baro"].reshape(out_shape_xy)),
-                "ep3baro": (out_dims_xy, out_fields["ep3baro"].reshape(out_shape_xy)),
-                "ep4": (out_dims_xy, out_fields["ep4"].reshape(out_shape_xy)),
-                "astar1": (out_dims_xyh, out_fields["astar1"].reshape(out_shape_xyh)),
-                "astar2": (out_dims_xyh, out_fields["astar2"].reshape(out_shape_xyh)),
-            },
-            coords={
-                **self._other_coords,
-                "height": _field.height,
-                "ylat": _field.ylat[-_nlat:],
-                "xlon": _field.xlon,
-            },
-            attrs=self.attrs
-        )
 
 
 def integrate_budget(ds, var_names=None):
     """Compute the integrated LWA budget terms for the given data.
 
     Integrates the LWA tendencies from equation (2) of `NH18
     <https://doi.org/10.1126/science.aat0721>`_ in time (over the time interval
@@ -517,15 +533,15 @@
         `divergence_eddy_momentum_flux`, and/or `meridional_heat_flux` to the
         names used in the input dataset.
 
     Returns
     -------
     xarray.Dataset
 
-    Example
+    Examples
     -------
     >>> qgds = QGDataset(data)
     >>> terms = qgds.compute_lwa_and_barotropic_fluxes()
     >>> compute_budget(terms.isel({ "time": slice(5, 10) }))
     """
     name_time = _get_name(ds, _NAMES_TIME, var_names)
     name_lwa  = _get_name(ds, _NAMES_LWA,  var_names)
```

### Comparing `hn2016_falwa-0.6.6/hn2016_falwa.egg-info/PKG-INFO` & `hn2016_falwa-0.7.0/hn2016_falwa.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hn2016-falwa
-Version: 0.6.6
+Version: 0.7.0
 Summary: python package to compute finite-amplitude local wave activity (Huang and Nakamura 2016, JAS)
 Home-page: https://github.com/csyhuang/hn2016_falwa
 Author: Clare S. Y. Huang
 Author-email: csyhuang@uchicago.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `hn2016_falwa-0.6.6/hn2016_falwa.egg-info/SOURCES.txt` & `hn2016_falwa-0.7.0/hn2016_falwa.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 LICENSE.txt
 setup.py
 hn2016_falwa/__init__.py
 hn2016_falwa/barotropic_field.py
 hn2016_falwa/basis.py
 hn2016_falwa/constant.py
+hn2016_falwa/data_storage.py
 hn2016_falwa/oopinterface.py
-hn2016_falwa/plot_utilities.py
-hn2016_falwa/qgformalism.py
+hn2016_falwa/plot_utils.py
 hn2016_falwa/utilities.py
 hn2016_falwa/wrapper.py
 hn2016_falwa/xarrayinterface.py
 hn2016_falwa.egg-info/PKG-INFO
 hn2016_falwa.egg-info/SOURCES.txt
 hn2016_falwa.egg-info/dependency_links.txt
 hn2016_falwa.egg-info/not-zip-safe
 hn2016_falwa.egg-info/requires.txt
 hn2016_falwa.egg-info/top_level.txt
 hn2016_falwa/f90_modules/compute_flux_dirinv.f90
+hn2016_falwa/f90_modules/compute_flux_dirinv_nshem.f90
 hn2016_falwa/f90_modules/compute_lwa_and_barotropic_fluxes.f90
 hn2016_falwa/f90_modules/compute_qref_and_fawa_first.f90
 hn2016_falwa/f90_modules/compute_reference_states.f90
 hn2016_falwa/f90_modules/interpolate_fields.f90
 hn2016_falwa/f90_modules/interpolate_fields_dirinv.f90
 hn2016_falwa/f90_modules/matrix_after_inversion.f90
 hn2016_falwa/f90_modules/matrix_b4_inversion.f90
@@ -28,9 +29,10 @@
 hn2016_falwa/legacy/__init__.py
 hn2016_falwa/legacy/beta_version.py
 tests/__init__.py
 tests/conftest.py
 tests/test_barotropic_field.py
 tests/test_basis.py
 tests/test_oopinterface.py
+tests/test_output_results.py
 tests/test_utilities.py
 tests/test_xarrayinterface.py
```

### Comparing `hn2016_falwa-0.6.6/setup.py` & `hn2016_falwa-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 ext9 = Extension(name='hn2016_falwa.compute_flux_dirinv',
                  sources=['hn2016_falwa/f90_modules/compute_flux_dirinv.f90'],
                  f2py_options=['--quiet'])
 
 setup(
     name='hn2016_falwa',
-    version='0.6.6',
+    version='0.7.0',
     description='python package to compute finite-amplitude local wave activity (Huang and Nakamura 2016, JAS)',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     url='https://github.com/csyhuang/hn2016_falwa',
     author='Clare S. Y. Huang',
     author_email='csyhuang@uchicago.edu',
     license='MIT',
```

### Comparing `hn2016_falwa-0.6.6/tests/test_barotropic_field.py` & `hn2016_falwa-0.7.0/tests/test_barotropic_field.py`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.6/tests/test_basis.py` & `hn2016_falwa-0.7.0/tests/test_basis.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,37 +21,37 @@
 dphi = np.deg2rad(np.diff(ylat)[0])
 area = 2. * pi * planet_radius ** 2 \
             * (np.cos(np.deg2rad(ylat[:, np.newaxis])) * dphi) \
             / float(nlon) * np.ones((nlat, nlon))
 
 
 def test_lwa():
-    '''
+    """
     To assert that the lwa function in basis.py produce the expect results -
     lwa shall be all zero when the there is no meridional component in the
     wind field.
-    '''
+    """
 
     test_vort = (np.ones((5, 5)) * np.array([1, 2, 3, 4, 5]))\
         .swapaxes(0, 1)
     test_q_part = np.array([1, 2, 3, 4, 5])
     input_result, _ = basis.lwa(5, 5, test_vort, test_q_part, np.ones(5))
     assert np.array_equal(input_result, np.zeros((5, 5)))
 
 
-def test_eqvlat():
-    '''
+def test_eqvlat_vgrad():
+    """
     To test whether the eqvlat function in basis.py produce a reference state of vorticity non-decreasing with latitude, given a random vorticity field.
-    '''
-    q_part1, vgrad = basis.eqvlat(
+    """
+    q_part1, vgrad = basis.eqvlat_vgrad(
         ylat, vort, area, nlat,
         planet_radius=EARTH_RADIUS,
         vgrad=dummy_vgrad
     )
-    q_part2, _ = basis.eqvlat(
+    q_part2, _ = basis.eqvlat_vgrad(
         ylat, vort, area, nlat,
         planet_radius=EARTH_RADIUS,
         vgrad=None
     )
     assert np.all(np.diff(q_part1) >= 0.)
     assert q_part1.tolist() == q_part2.tolist()
     assert vgrad is not None
```

### Comparing `hn2016_falwa-0.6.6/tests/test_utilities.py` & `hn2016_falwa-0.7.0/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.6/tests/test_xarrayinterface.py` & `hn2016_falwa-0.7.0/tests/test_xarrayinterface.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,59 +2,78 @@
 
 import numpy as np
 try:
     import xarray as xr
 except ImportError:
     pytest.skip("Optional package Xarray is not installed.", allow_module_level=True)
 
+from hn2016_falwa.oopinterface import QGFieldNH18, QGFieldNHN22
 from hn2016_falwa.xarrayinterface import QGDataset
 from hn2016_falwa.xarrayinterface import _is_ascending, _is_descending, _is_equator
 from hn2016_falwa.xarrayinterface import _get_name, _map_collect
 
 
 def _generate_test_dataset(**additional_coords):
     from .test_oopinterface import xlon, ylat, plev, u_field, v_field, t_field
     dims = ("plev", "ylat", "xlon")
     return xr.Dataset(
         data_vars={ "u": (dims, u_field), "v": (dims, v_field), "t": (dims, t_field) },
         coords={ "plev": plev, "ylat": ylat, "xlon": xlon, **additional_coords }
     )
 
-def test_qgdataset():
+
+def test_qgdataset_with_dataset():
     data = _generate_test_dataset()
     qgds = QGDataset(data)
     # Make sure all computation functions run
     qgds.interpolate_fields()
     qgds.compute_reference_states()
     qgds.compute_lwa_and_barotropic_fluxes()
 
-def test_qgdataset_flips_ylat():
+def test_qgdataset_with_dataarray():
     data = _generate_test_dataset()
-    interp1 = QGDataset(data).interpolate_fields()
-    interp2 = QGDataset(data.reindex({ "ylat": data["ylat"][::-1] })).interpolate_fields()
-    assert np.allclose(interp1["ylat"], interp2["ylat"])
+    QGDataset(data["u"], data["v"], data["t"])
 
-def test_qgdataset_flips_plev():
+def test_qgdataset_with_mixed_args():
     data = _generate_test_dataset()
-    interp1 = QGDataset(data).interpolate_fields()
-    interp2 = QGDataset(data.reindex({ "plev": data["plev"][::-1] })).interpolate_fields()
-    assert np.allclose(interp1["height"], interp2["height"])
+    QGDataset(data[["u", "t"]], da_v=data["v"])
 
 def test_qgdataset_rejects_incomplete():
     data = _generate_test_dataset()
     for var in data:
         with pytest.raises(KeyError):
             QGDataset(data.drop_vars([var]))
 
+def test_qgdataset_with_coordinate_mismatch():
+    data = _generate_test_dataset()
+    with pytest.raises(AssertionError):
+        QGDataset(data["u"], data["v"], data["t"].rename({ "ylat": "latitude" }))
+
 def test_qgdataset_rejects_transposed():
     data = _generate_test_dataset()
     with pytest.raises(AssertionError):
-        QGDataset(data.transpose("xlon", "plev", "ylat"))
+        transposed_data = data.transpose("xlon", "plev", "ylat")
+        QGDataset(transposed_data)
     with pytest.raises(AssertionError):
-        QGDataset(data.transpose("ylat", "xlon", "plev"))
+        transposed_data = data.transpose("ylat", "xlon", "plev")
+        QGDataset(transposed_data)
+
+
+def test_qgdataset_flips_ylat():
+    data = _generate_test_dataset()
+    interp1 = QGDataset(data).interpolate_fields()
+    interp2 = QGDataset(data.reindex({"ylat": data["ylat"][::-1]})).interpolate_fields()
+    assert np.allclose(interp1["ylat"], interp2["ylat"])
+
+def test_qgdataset_flips_plev():
+    data = _generate_test_dataset()
+    interp1 = QGDataset(data).interpolate_fields()
+    interp2 = QGDataset(data.reindex({"plev": data["plev"][::-1]})).interpolate_fields()
+    assert np.allclose(interp1["height"], interp2["height"])
+
 
 def test_qgdataset_4d():
     data = xr.concat([_generate_test_dataset(time=t) for t in range(3)], dim="time")
     qgds = QGDataset(data)
     interp = qgds.interpolate_fields()
     # Verify that time dimension is preserved
     assert "time" in interp.coords
@@ -82,14 +101,48 @@
         data["time"].size,
         qgds.attrs["kmax"],
         data["ylat"].size,
         data["xlon"].size
     )
 
 
+@pytest.mark.parametrize("nh_only", [False, True])
+@pytest.mark.parametrize("QGField", [QGFieldNH18, QGFieldNHN22])
+def test_basic_qgdataset_calls(QGField, nh_only):
+    data = _generate_test_dataset()
+    qgds = QGDataset(data, qgfield=QGField, qgfield_kwargs={
+        "northern_hemisphere_results_only": nh_only
+    })
+    # Step 1: basic output verification
+    out1 = qgds.interpolate_fields()
+    np.testing.assert_allclose(out1["qgpv"], qgds.qgpv)
+    np.testing.assert_allclose(out1["interpolated_u"], qgds.interpolated_u)
+    np.testing.assert_allclose(out1["interpolated_v"], qgds.interpolated_v)
+    np.testing.assert_allclose(out1["interpolated_theta"], qgds.interpolated_theta)
+    assert "static_stability" in out1 or ("static_stability_n" in out1 and "static_stability_s" in out1)
+    # Step 2: basic output verification
+    out2 = qgds.compute_reference_states()
+    np.testing.assert_allclose(out2["qref"], qgds.qref)
+    np.testing.assert_allclose(out2["uref"], qgds.uref)
+    np.testing.assert_allclose(out2["ptref"], qgds.ptref)
+    # Step 3: basic output verification
+    out3 = qgds.compute_lwa_and_barotropic_fluxes()
+    np.testing.assert_allclose(out3["adv_flux_f1"], qgds.adv_flux_f1)
+    np.testing.assert_allclose(out3["adv_flux_f2"], qgds.adv_flux_f2)
+    np.testing.assert_allclose(out3["adv_flux_f3"], qgds.adv_flux_f3)
+    np.testing.assert_allclose(out3["convergence_zonal_advective_flux"], qgds.convergence_zonal_advective_flux)
+    np.testing.assert_allclose(out3["divergence_eddy_momentum_flux"], qgds.divergence_eddy_momentum_flux)
+    np.testing.assert_allclose(out3["meridional_heat_flux"], qgds.meridional_heat_flux)
+    np.testing.assert_allclose(out3["lwa_baro"], qgds.lwa_baro)
+    np.testing.assert_allclose(out3["u_baro"], qgds.u_baro)
+    np.testing.assert_allclose(out3["lwa"], qgds.lwa)
+
+
+# Tests for internals
+
 def test_is_ascending():
     assert _is_ascending([4])
     assert _is_ascending([0, 1, 2, 3, 4, 5])
     assert _is_ascending([-2.0, 0.3, 0.5, 1.2])
     assert not _is_ascending([0, -1])
     assert not _is_ascending([0, 2, 3, 3, 3, 2.9])
     assert not _is_ascending([-1, -2., -3.])
```

