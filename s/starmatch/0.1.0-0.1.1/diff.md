# Comparing `tmp/starmatch-0.1.0-py3-none-any.whl.zip` & `tmp/starmatch-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 31317 bytes, number of entries: 13
+Zip file size: 31322 bytes, number of entries: 13
 -rw-r--r--  2.0 unx       41 b- defN 23-May-30 10:47 starmatch/__init__.py
 -rw-r--r--  2.0 unx    22310 b- defN 23-Jun-12 11:07 starmatch/astroalign.py
 -rw-r--r--  2.0 unx    41872 b- defN 23-Jun-16 03:10 starmatch/classes.py
 -rw-r--r--  2.0 unx     5958 b- defN 23-Jun-12 13:07 starmatch/orientation.py
 -rw-r--r--  2.0 unx     3078 b- defN 23-Jun-12 11:33 starmatch/plot.py
 -rw-r--r--  2.0 unx     1976 b- defN 23-Jun-12 11:32 starmatch/wcs.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-30 11:01 starmatch/distortion/__init__.py
 -rw-r--r--  2.0 unx    11236 b- defN 23-Jun-15 03:24 starmatch/distortion/distortion_model.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jun-16 07:41 starmatch-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    24023 b- defN 23-Jun-16 07:41 starmatch-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 07:41 starmatch-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-16 07:41 starmatch-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1044 b- defN 23-Jun-16 07:41 starmatch-0.1.0.dist-info/RECORD
-13 files, 112708 bytes uncompressed, 29583 bytes compressed:  73.8%
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jun-19 06:35 starmatch-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    24093 b- defN 23-Jun-19 06:35 starmatch-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 06:35 starmatch-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-19 06:35 starmatch-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1044 b- defN 23-Jun-19 06:35 starmatch-0.1.1.dist-info/RECORD
+13 files, 112778 bytes uncompressed, 29588 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: starmatch/distortion/__init__.py
 Comment: 
 
 Filename: starmatch/distortion/distortion_model.py
 Comment: 
 
-Filename: starmatch-0.1.0.dist-info/LICENSE
+Filename: starmatch-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: starmatch-0.1.0.dist-info/METADATA
+Filename: starmatch-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: starmatch-0.1.0.dist-info/WHEEL
+Filename: starmatch-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: starmatch-0.1.0.dist-info/top_level.txt
+Filename: starmatch-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: starmatch-0.1.0.dist-info/RECORD
+Filename: starmatch-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `starmatch-0.1.0.dist-info/LICENSE` & `starmatch-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `starmatch-0.1.0.dist-info/METADATA` & `starmatch-0.1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starmatch
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to handle the Star map matching and astronomical positioning
 Home-page: https://github.com/lcx366/STARMATCH
 Author: Chunxiao Li
 Author-email: lcx366@126.com
 License: MIT
 Keywords: Star Map Matching,Astronomical positioning,Distortion Correction,pointing calibration
 Classifier: Development Status :: 4 - Beta
@@ -20,15 +20,15 @@
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
 Requires-Dist: scikit-image
 Requires-Dist: photutils
 Requires-Dist: astropy (>=4.3.1)
 Requires-Dist: GPy
-Requires-Dist: PIL
+Requires-Dist: Pillow
 Requires-Dist: colorama
 Requires-Dist: starcatalogquery
 
 # Welcome to the STARMATCH package
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/starmatch.svg)](https://pypi.python.org/pypi/starmatch/) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/starmatch.svg)](https://pypi.python.org/pypi/starmatch/) [![PyPI status](https://img.shields.io/pypi/status/starmatch.svg)](https://pypi.python.org/pypi/starmatch/) [![GitHub contributors](https://img.shields.io/github/contributors/lcx366/STARMATCH.svg)](https://GitHub.com/lcx366/STARMATCH/graphs/contributors/) [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/lcx366/STARMATCH/graphs/commit-activity) [![GitHub license](https://img.shields.io/github/license/lcx366/STARMATCH.svg)](https://github.com/lcx366/STARMATCH/blob/master/LICENSE) [![Documentation Status](https://readthedocs.org/projects/starmatch/badge/?version=latest)](http://starmatch.readthedocs.io/?badge=latest) [![Build Status](https://travis-ci.org/lcx366/starmatch.svg?branch=master)](https://travis-ci.org/lcx366/starmatch)
 
@@ -182,17 +182,17 @@
 
 #### Example: Tangential Distortion Model(TDM)
 
 The Tangential Distortion Model(also known as the de-centering distortion) is defined by the distortion center and the distortion coefficients.
 
 Basic formulas are as follows:
 
-$x_u = x_d + (P_1 * (r_d^2 + 2*(x_d-x_c)^2) + 2*P_2 * (x_d-x_c)*(y_d-y_c))*(1 + P_3*r_d^2 + P_4*r_d^4 + ...)$
+$x_u = x_d + (P_1 * (r_d^2 + 2*(x_d-x_c)^2) + 2*P_2 * (x_d-x_c)*(y_d-y_c))*(1 + P_3 * r_d^2 + P_4*r_d^4 + ...)$
 
-$y_u = y_d + (P_2 * (r_d^2 + 2*(y_d-y_c)^2) + 2*P_1 * (x_d-x_c)*(y_d-y_c))*(1 + P_3*r_d^2 + P_4*r_d^4 + ...)$
+$y_u = y_d + (P_2 * (r_d^2 + 2*(y_d-y_c)^2) + 2*P_1 * (x_d-x_c)*(y_d-y_c))*(1 + P_3 * r_d^2 + P_4*r_d^4 + ...)$
 
 ##### Construct a Tangential Distortion Model
 
 ```python
 from starmatch.classes import Distortion
 model = 'Tangential' # Type of distortion model
 coeffs = [-1e-4,1e-4] # Coefficients of 2nd order SRDM in form of [P1,P2]
@@ -326,55 +326,55 @@
     - _fov -> Field of View of camera in [deg]
     - _pixel_width -> Pixel width of camera in [deg]
     - _res -> Resolution of camera
 ```
 
 #### Estimate the center pointing of the camera
 
-We use the HYG v3.0 star catalog(Thanks to [David Nash](https://www.astronexus.com/hyg)) to genarate the h5-format index file according to the camera parameters(field of view, detected magnitude, observation time) with the python package starcatalogquery, which can be installed by `pip install starcatalogquery`. The h5-format index file records the center pointing of each sky area, the pixel coordinates, the triangle invariants and the asterism indices of the stars.
+We use the HYG v3.5 star catalog(Thanks to [David Nash](https://www.astronexus.com/hyg)) to genarate the h5-format index file according to the camera parameters(field of view, detected magnitude, observation time) with the python package starcatalogquery, which can be installed by `pip install starcatalogquery`. The h5-format index file records the center pointing of each sky area, the pixel coordinates, the triangle invariants and the asterism indices of the stars.
 
 ##### Blind matching over star maps
 
 ```python
-catalogfile_h5 = 'starcatalogs/indices/hygv3/fov10_mag9.0_mcp20_2022.0.h5'
+catalogfile_h5 = 'starcatalogs/indices/hygv35/fov10_mag9.0_mcp20_2022.0.h5'
 fp_radec = sources1.center_pointing(catalogfile_h5)
 print(fp_radec)
 ```
 
-    (204.01793337608683, 36.24740259697955)m of 192
+    (204.01793337608683, 36.24740259697955)
 
 ##### Blind matching over star maps with the multi-core parallel computing
 
 ```python
-catalogfile_h5 = 'starcatalogs/indices/hygv3/fov10_mag9.0_mcp20_2022.0.h5'
+catalogfile_h5 = 'starcatalogs/indices/hygv35/fov10_mag9.0_mcp20_2022.0.h5'
 fp_radec = sources1.center_pointing_mp(catalogfile_h5)
 print(fp_radec) # (Ra,Dec) in [deg]
 ```
 
     (204.01793337608683, 36.24740259697955)
 
 ### Star Map Matching
 
-Load the simplified HYG v3.0 star catalog.
+Load the simplified HYG v3.5 star catalog.
 
 ```python
 from starcatalogquery import StarCatalog
 # The following starcatalog path stores the tile files with size of 5 deg, stars magnitude less than 9.0, and proper motion correction to epoch of 2022.0.
-dir_from_simplified = 'starcatalogs/simplified/hygv3/res5/mag9.0/epoch2022.0/'
-hygv3_simplified = StarCatalog.load(dir_from_simplified)
+dir_from_simplified = 'starcatalogs/simplified/hygv35/res5/mag9.0/epoch2022.0/'
+hygv35_simplified = StarCatalog.load(dir_from_simplified)
 ```
 
 The actual center pointing of the camera is (204.01706216087143, 36.25274704575726), in order to test the tolerance ability of star map matching, we set the pointing point to [200,30]. 
 
 Note: in process of star map matching, we set **L**(default=32) as the normalized length scale, namely, number of pixels in a unit length. It controls the tolerance of the 3D-Tree composed of (x,y,mag) of sources from camera and stars from catalog. For example, if the tolerance is set to 0.2(default), it means the difference within 0.2\*32=6.4 for pixel coordinates and 0.2 for magnitude is regarded as the correct matching.
 Another use of L is associated with the GPR(Gaussian Process Regression)-based distortion correction bellow. Experience has shown that normalizing the pixel coordinates by L is beneficial to the operation of GPR.
 
 ```python
 fp_radec = [201,31]
-sources1.align(fp_radec,hygv3_simplified,L=32)
+sources1.align(fp_radec,hygv35_simplified,L=32)
 ```
 
     Instance of class Sources
 
 We get object `sources1` updated with new attributes added:
 
 ```
@@ -434,15 +434,19 @@
 sources1.show_starmatch(image_raw,offset)
 ```
 
 <p align="middle">
   <img src="readme_figs/output_52_0.png" width="500" />
 </p>
 
-The asterisks on the graph are consistent with the  `catalog_df`.
+The asterisks on the graph are consistent with the `catalog_df`.
+
+<p align="middle">
+  <img src="readme_figs/catalog_df.png" width="700" />
+</p>
 
 ### Calibrate the orientation of the camera center
 
 ```python
 sources1.fp_calibrate()
 print(sources1.fp_radec_calibrated)
 # [[204.01747112  36.25112389]]
@@ -453,16 +457,16 @@
 
 ### Astronomical Positioning and Apparent Magnitude Estimation
 
 Estimate the celestial coordinates and magnitudes of unknown targets.
 
 ```python
 xy_target,flux_target = [345,678],1e3 # [[345,678],[-278,521]],[1e3,2e4]
-radec,M_affine,M_uncalibrated = sources1.apply(xy_target,flux_target)
-print(radec,M_affine,M_uncalibrated)
+radec,M_affine,M_match = sources1.apply(xy_target,flux_target)
+print(radec,M_affine,M_match)
 print(sources1.affine_results.mag_rms,sources1.match_results.mag_rms)
 ```
 
     [[199.83995525  31.44951982]] 8.036101294387004 8.011023843192229
     0.08052914228287848 0.10371476611720697
 
 ### Star Map Matching with geometric distortion considered
@@ -486,15 +490,15 @@
 # sources2 = StarMatch.from_sources(xy_distorted,flux,camera_params,20,distortion_correction_model)
 sources2 = StarMatch.from_sources(xy_distorted,flux,camera_params,20)
 ```
 
 #### Star Map Matching
 
 ```python
-sources2.align(fp_radec,hygv3_simplified,L=32,calibrate=True) 
+sources2.align(fp_radec,hygv35_simplified,L=32,calibrate=True) 
 ```
 
     Instance of class Sources
 
 We get object `sources2` updated with new attributes added:
 
 ```
```

## Comparing `starmatch-0.1.0.dist-info/RECORD` & `starmatch-0.1.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 starmatch/astroalign.py,sha256=OymKBKAHvw7_IvlC4mpnTYnQKg987sh0g7TGO17GgYg,22310
 starmatch/classes.py,sha256=Dshs0hnoRCf-zA6Rnqoxa5w7S1TSvbM-h2cPJHrJj-Y,41872
 starmatch/orientation.py,sha256=DRkmfMEd4n8eeqG1daIuN_-5pXunIdLgrglt0wprkL4,5958
 starmatch/plot.py,sha256=K9BIOSlRT7gcO-oiix-4vFwKnTUwNMrBDU8epDa40RE,3078
 starmatch/wcs.py,sha256=jq5mmLYtXeVbdL7MuBTUEQnwX-FuTn_jcU7KqMaHYOA,1976
 starmatch/distortion/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 starmatch/distortion/distortion_model.py,sha256=bZ05MifpnbIuHE_eVa-0XErwpmZZ_rVZC9QDmmQWQds,11236
-starmatch-0.1.0.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
-starmatch-0.1.0.dist-info/METADATA,sha256=QKDzLSNCvww2EYMU1937kFRqFQNGd8vy3SNJOyApZro,24023
-starmatch-0.1.0.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-starmatch-0.1.0.dist-info/top_level.txt,sha256=yxZNa5SKsmUHcbN_hI9Aa5_mi6QfdMxAorjQUYkiMiA,10
-starmatch-0.1.0.dist-info/RECORD,,
+starmatch-0.1.1.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
+starmatch-0.1.1.dist-info/METADATA,sha256=VTXp45OVukPFI4HRn11BJxAuMZyc38h-tZu0jPa6X5s,24093
+starmatch-0.1.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+starmatch-0.1.1.dist-info/top_level.txt,sha256=yxZNa5SKsmUHcbN_hI9Aa5_mi6QfdMxAorjQUYkiMiA,10
+starmatch-0.1.1.dist-info/RECORD,,
```

