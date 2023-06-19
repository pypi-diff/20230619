# Comparing `tmp/iconarray-0.3.0.tar.gz` & `tmp/iconarray-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iconarray-0.3.0.tar", last modified: Mon Mar  6 10:51:51 2023, max compression
+gzip compressed data, was "iconarray-0.3.1.tar", last modified: Mon Jun 19 13:53:06 2023, max compression
```

## Comparing `iconarray-0.3.0.tar` & `iconarray-0.3.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 10:51:51.351282 iconarray-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-06 10:51:42.000000 iconarray-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-03-06 10:51:51.351282 iconarray-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-03-06 10:51:42.000000 iconarray-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 10:51:51.351282 iconarray-0.3.0/iconarray/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-06 10:51:42.000000 iconarray-0.3.0/iconarray/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 10:51:51.351282 iconarray-0.3.0/iconarray/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 10:51:42.000000 iconarray-0.3.0/iconarray/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26233 2023-03-06 10:51:42.000000 iconarray-0.3.0/iconarray/backend/grid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 10:51:51.351282 iconarray-0.3.0/iconarray/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 10:51:42.000000 iconarray-0.3.0/iconarray/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-03-06 10:51:42.000000 iconarray-0.3.0/iconarray/core/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-03-06 10:51:42.000000 iconarray-0.3.0/iconarray/core/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-03-06 10:51:42.000000 iconarray-0.3.0/iconarray/core/latlonhash.py
--rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-03-06 10:51:42.000000 iconarray-0.3.0/iconarray/core/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 10:51:51.351282 iconarray-0.3.0/iconarray/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-06 10:51:42.000000 iconarray-0.3.0/iconarray/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-03-06 10:51:42.000000 iconarray-0.3.0/iconarray/plot/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 10:51:51.351282 iconarray-0.3.0/iconarray/plot/formatoptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 10:51:42.000000 iconarray-0.3.0/iconarray/plot/formatoptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-03-06 10:51:42.000000 iconarray-0.3.0/iconarray/plot/formatoptions/borders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-03-06 10:51:42.000000 iconarray-0.3.0/iconarray/plot/formatoptions/customtext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-03-06 10:51:42.000000 iconarray-0.3.0/iconarray/plot/formatoptions/lakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-03-06 10:51:42.000000 iconarray-0.3.0/iconarray/plot/formatoptions/meanmaxwind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-03-06 10:51:42.000000 iconarray-0.3.0/iconarray/plot/formatoptions/rivers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-03-06 10:51:42.000000 iconarray-0.3.0/iconarray/plot/formatoptions/standardtitle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 10:51:51.351282 iconarray-0.3.0/iconarray/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 10:51:42.000000 iconarray-0.3.0/iconarray/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-03-06 10:51:42.000000 iconarray-0.3.0/iconarray/utils/get_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 10:51:51.351282 iconarray-0.3.0/iconarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-03-06 10:51:51.000000 iconarray-0.3.0/iconarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-06 10:51:51.000000 iconarray-0.3.0/iconarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 10:51:51.000000 iconarray-0.3.0/iconarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-06 10:51:51.000000 iconarray-0.3.0/iconarray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-06 10:51:51.000000 iconarray-0.3.0/iconarray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-03-06 10:51:51.355282 iconarray-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-06 10:51:42.000000 iconarray-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:06.588451 iconarray-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-19 13:52:57.000000 iconarray-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-06-19 13:53:06.588451 iconarray-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-06-19 13:52:57.000000 iconarray-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:06.584451 iconarray-0.3.1/iconarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:06.584451 iconarray-0.3.1/iconarray/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26233 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/backend/grid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:06.584451 iconarray-0.3.1/iconarray/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/core/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/core/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/core/latlonhash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/core/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:06.588451 iconarray-0.3.1/iconarray/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/plot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:06.588451 iconarray-0.3.1/iconarray/plot/formatoptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/plot/formatoptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/plot/formatoptions/borders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/plot/formatoptions/customtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/plot/formatoptions/lakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/plot/formatoptions/meanmaxwind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/plot/formatoptions/rivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/plot/formatoptions/standardtitle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:06.588451 iconarray-0.3.1/iconarray/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-19 13:52:57.000000 iconarray-0.3.1/iconarray/utils/get_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:06.584451 iconarray-0.3.1/iconarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-06-19 13:53:06.000000 iconarray-0.3.1/iconarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-19 13:53:06.000000 iconarray-0.3.1/iconarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:53:06.000000 iconarray-0.3.1/iconarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-19 13:53:06.000000 iconarray-0.3.1/iconarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-19 13:53:06.000000 iconarray-0.3.1/iconarray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-19 13:53:06.588451 iconarray-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-19 13:52:57.000000 iconarray-0.3.1/setup.py
```

### Comparing `iconarray-0.3.0/LICENSE` & `iconarray-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.0/PKG-INFO` & `iconarray-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: iconarray
-Version: 0.3.0
+Version: 0.3.1
 Summary: A package of modules for processing and plotting ICON data.
 Home-page: https://github.com/C2SM/iconarray
 Author: MeteoSwiss, C2SM
 Author-email: victoria.cherkas@meteoswiss.ch, annika.lauber@c2sm.ethz.ch
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # iconarray
 
 [![Available on pypi](https://badge.fury.io/py/iconarray.svg)](https://pypi.python.org/pypi/iconarray/)
-[![Docs](https://github.com/C2SM/iconarray/workflows/docs/badge.svg?branch=main)](https://c2sm.github.io/iconarray/)
+[![Docs](https://github.com/C2SM/iconarray/workflows/Documentation/badge.svg?branch=main)](https://c2sm.github.io/iconarray/)
 [![Build Status](https://jenkins-mch.cscs.ch/job/iconarray_testsuite/badge/icon?config=build)](https://jenkins-mch.cscs.ch/job/iconarray_testsuite/)
 [![Test Status](https://jenkins-mch.cscs.ch/job/iconarray_testsuite/badge/icon?config=test)](https://jenkins-mch.cscs.ch/job/iconarray_testsuite/)
 
 ## Introduction
 
 The iconarray python package contains various modules to facilitate working with ICON data with xarray or other xarray based tools (such as [psyplot](https://psyplot.github.io/) - a plotting package). The package was developed together with [icon-vis](https://github.com/C2SM/icon-vis).
```

### Comparing `iconarray-0.3.0/README.md` & `iconarray-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # iconarray
 
 [![Available on pypi](https://badge.fury.io/py/iconarray.svg)](https://pypi.python.org/pypi/iconarray/)
-[![Docs](https://github.com/C2SM/iconarray/workflows/docs/badge.svg?branch=main)](https://c2sm.github.io/iconarray/)
+[![Docs](https://github.com/C2SM/iconarray/workflows/Documentation/badge.svg?branch=main)](https://c2sm.github.io/iconarray/)
 [![Build Status](https://jenkins-mch.cscs.ch/job/iconarray_testsuite/badge/icon?config=build)](https://jenkins-mch.cscs.ch/job/iconarray_testsuite/)
 [![Test Status](https://jenkins-mch.cscs.ch/job/iconarray_testsuite/badge/icon?config=test)](https://jenkins-mch.cscs.ch/job/iconarray_testsuite/)
 
 ## Introduction
 
 The iconarray python package contains various modules to facilitate working with ICON data with xarray or other xarray based tools (such as [psyplot](https://psyplot.github.io/) - a plotting package). The package was developed together with [icon-vis](https://github.com/C2SM/icon-vis).
```

### Comparing `iconarray-0.3.0/iconarray/backend/grid.py` & `iconarray-0.3.1/iconarray/backend/grid.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.0/iconarray/core/crop.py` & `iconarray-0.3.1/iconarray/core/crop.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.0/iconarray/core/interpolate.py` & `iconarray-0.3.1/iconarray/core/interpolate.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.0/iconarray/core/latlonhash.py` & `iconarray-0.3.1/iconarray/core/latlonhash.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.0/iconarray/core/utilities.py` & `iconarray-0.3.1/iconarray/core/utilities.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """
 The utilities.py module contains various functions useful for analysing or plotting (ICON) data using xarray.
 
 Contains public functions: ind_from_latlon, add_coordinates, get_stats wilks, show_data_vars
 """
 
+from typing import List
+
 import numpy as np
 import six
-import xarray
+import xarray as xr
 from scipy import stats
+from sklearn.neighbors import BallTree
 
 
 def awhere_drop(ds, cond):
     """
-    xarray.Dataset.where equivalent that preserves the dtype of the array.
+    xr.Dataset.where equivalent that preserves the dtype of the array.
 
-    The xarray.Dataset.where in general will not preserve the value type of the array. In case of drop=False, elements of the array that do not satisfy the condition are set to np.NaN, which can only be stored on a float type. Therefore the return of xarray.Dataset.where will be of dtype float64. This function computes a where with drop=True, ensuring the dtype of the input xarray is preserved.
+    The xr.Dataset.where in general will not preserve the value type of the array. In case of drop=False, elements of the array that do not satisfy the condition are set to np.NaN, which can only be stored on a float type. Therefore the return of xarray.Dataset.where will be of dtype float64. This function computes a where with drop=True, ensuring the dtype of the input xarray is preserved.
 
     Parameters
     ----------
     ds : xr.Dataset
         Dataset such as ICON data
     cond
         A condition to apply to the data.
@@ -31,68 +34,142 @@
     ret = ds.where(cond, drop=True)
     for var in ds:
         ret[var] = ret[var].astype(ds[var].dtype)
 
     return ret
 
 
-def ind_from_latlon(lats, lons, lat, lon, verbose=False):
+def ind_from_latlon(
+    lon_array: xr.DataArray,
+    lat_array: xr.DataArray,
+    lon_point: float,
+    lat_point: float,
+    n: int = 1,
+    verbose: bool = False,
+) -> List[int]:
     """
-    Find the nearest neighbouring index to given location.
+    Find the indices of the n closest cells in a grid, relative to a given latitude/longitude point.
+
+    The function builds a BallTree from the provided 1D or 2D array of longitude and latitude coordinates,
+    and queries it to find the n nearest neighbors to the given point.
 
     Parameters
     ----------
-    lats : 2d array
-        Latitude grid
-    lons : 2d array
-        Longitude grid
-    lat : float
-        Latitude of location
-    lon : float
-        Longitude of location
-    verbose : bool
+    lon_array : xr.DataArray
+        A 1D or 2D xr of longitude values [degree].
+    lat_array : xr.DataArray
+        A 1D or 2D xr of latitude values [degree].
+    lon_point : float
+        The longitude value [degree] of the point to find the closest point(s) to.
+    lat_point : float
+        The latitude value [degree] of the point to find the closest point(s) to.
+    n : int, optional
+        The number of closest points to return. Default is 1.
+    verbose: bool, optional
         Print information. Defaults to False.
 
     Returns
-    ----------
-    index : int
-        Index of nearest grid point.
+    -------
+    List[int]
+        The indices of the closest n points to the given point.
 
-    See Also
-    ----------
-    iconarray.core.utilities
 
-    Examples
+    Example
     ----------
     >>> # Get values of grid cell closest to coordinate
     >>> # E.g. Zürich:
     >>> lon = 8.54
     >>> lat = 47.38
-    >>> lats = np.rad2deg(ds.clat.values[:])
-    >>> lons = np.rad2deg(ds.clon.values[:])
+    >>> lats = ds.clat
+    >>> lons = ds.clon
+    >>> if ds.clat.attrs.get('units') == 'radian':
+    >>>     lats = np.rad2deg(lats)
+    >>>     lons = np.rad2deg(lons)
     >>> ind = iconarray.ind_from_latlon(
-    ...         lats,lons,lat,lon,verbose=True
+    ...         lats,lons,lat,lon,
+    ...         verbose=True, n=1
     ...         )
 
     >>> ind
     3352
     # Closest ind: 3352
-    #  Given lat: 47.380 vs found lat: 47.372
-    #  Given lon: 8.540 vs found lon: 8.527
+    # Given lat: 47.380 deg. Closest 1 lat/s found: 47.372
+    # Given lon: 8.540 deg. Closest 1 lon/s found: 8.527
 
     """
-    dist = [
-        np.sqrt((lats[i] - lat) ** 2 + (lons[i] - lon) ** 2) for i in range(len(lats))
+    # Utility function
+    def get_innermost_element(indices):
+        """
+        Recursively traverses nested lists or arrays to obtain the innermost element.
+
+        Args:
+            indices: A nested list or numpy array.
+
+        Returns:
+            The innermost element of the nested structure.
+
+        """
+        if isinstance(indices, (list, tuple, np.ndarray)):
+            if len(indices) > 0:
+                if isinstance(indices[0], (list, tuple, np.ndarray)):
+                    return get_innermost_element(indices[0])
+                else:
+                    return indices
+            else:
+                return indices
+        return [indices]
+
+    # Convert Input to radians
+    lon_array, lat_array, lon_point, lat_point = [
+        np.deg2rad(arr) for arr in [lon_array, lat_array, lon_point, lat_point]
     ]
-    ind = np.where(dist == np.min(dist))[0][0]
+
+    # Create a 2D array of lon and lat coordinates
+    lon_lat_array = np.column_stack(
+        (lon_array.values.flatten(), lat_array.values.flatten())
+    )
+
+    # Build a BallTree from this 2D array using the Haversine distance
+    tree = BallTree(lon_lat_array, metric="haversine")
+
+    # Find the index of the nearest neighbor(s) of the given point
+    points = np.column_stack((lon_point, lat_point))
+    _, indices = tree.query(points, k=n)
+
+    # Convert index to 2D indices if applicable, e.g., when using output remapped to lat-lon grind
+    if n == 1:
+        indices = [np.unravel_index(indices, lon_array.shape)]
+    else:
+        indices = [np.unravel_index(index, lon_array.shape) for index in indices]
+
+    # Unpack indices list
+    indices = get_innermost_element(indices)
+
+    # Print verbose information if requested
     if verbose:
-        print(f"Closest ind: {ind}")
-        print(f" Given lat: {lat:.3f} vs found lat: {lats[ind]:.3f}")
-        print(f" Given lon: {lon:.3f} vs found lon: {lons[ind]:.3f}")
-    return ind
+        closest_lats = " ".join(
+            f"{num:.4f}" for num in np.rad2deg(lat_array.values[indices])
+        )
+        closest_lons = " ".join(
+            f"{num:.4f}" for num in np.rad2deg(lon_array.values[indices])
+        )
+
+        indices_str = " ".join(map(str, indices.tolist()))
+        given_lat_str = f"{np.rad2deg(lat_point):.4f}"
+        given_lon_str = f"{np.rad2deg(lon_point):.4f}"
+
+        print(f"Closest indices: {indices_str}")
+        print(
+            f"Given lat: {given_lat_str} deg. Closest {n} lat/s found: {closest_lats}"
+        )
+        print(
+            f"Given lon: {given_lon_str} deg. Closest {n} lon/s found: {closest_lons}"
+        )
+
+    return indices
 
 
 def add_coordinates(lon, lat, lonmin, lonmax, latmin, latmax):
     """
     Get the position of given lat/lon coordinates in relation to the bounds of regular lat/lon grid.
 
     This could be used for example to add a marker to a map plot by lat/lon coordinates.
@@ -230,22 +307,22 @@
     """
     Print a table with variables in dataset.
 
     The first column is the variable name chosen by cfgrib to use eg. when plotting with psyplot.
 
     Parameters
     ----------
-    ds : xarray.Dataset
+    ds : xr.Dataset
         Dataset of ICON GRIB data opened with cgrib engine or cfgrib.
     """
     if type(ds) is str:
         Exception(
             "Argument is not a Dataset. Please open the dataset via psy.open_dataset() and pass returned Dataset to this function."
         )
-    elif type(ds) is xarray.core.dataset.Dataset:
+    elif type(ds) is xr.core.dataset.Dataset:
         print(
             "{:<15} {:<32} {:<20} {:<20} {:<10}".format(
                 "psyplot name", "long_name", "GRIB_cfVarName", "GRIB_shortName", "units"
             )
         )
         for _k, v in six.iteritems(ds.data_vars):
             i = ds.data_vars[v.name]
```

### Comparing `iconarray-0.3.0/iconarray/plot/config.py` & `iconarray-0.3.1/iconarray/plot/config.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.0/iconarray/plot/formatoptions/borders.py` & `iconarray-0.3.1/iconarray/plot/formatoptions/borders.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.0/iconarray/plot/formatoptions/customtext.py` & `iconarray-0.3.1/iconarray/plot/formatoptions/customtext.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.0/iconarray/plot/formatoptions/lakes.py` & `iconarray-0.3.1/iconarray/plot/formatoptions/lakes.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.0/iconarray/plot/formatoptions/meanmaxwind.py` & `iconarray-0.3.1/iconarray/plot/formatoptions/meanmaxwind.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.0/iconarray/plot/formatoptions/rivers.py` & `iconarray-0.3.1/iconarray/plot/formatoptions/rivers.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.0/iconarray/plot/formatoptions/standardtitle.py` & `iconarray-0.3.1/iconarray/plot/formatoptions/standardtitle.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.0/iconarray/utils/get_data.py` & `iconarray-0.3.1/iconarray/utils/get_data.py`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.0/iconarray.egg-info/PKG-INFO` & `iconarray-0.3.1/iconarray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: iconarray
-Version: 0.3.0
+Version: 0.3.1
 Summary: A package of modules for processing and plotting ICON data.
 Home-page: https://github.com/C2SM/iconarray
 Author: MeteoSwiss, C2SM
 Author-email: victoria.cherkas@meteoswiss.ch, annika.lauber@c2sm.ethz.ch
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # iconarray
 
 [![Available on pypi](https://badge.fury.io/py/iconarray.svg)](https://pypi.python.org/pypi/iconarray/)
-[![Docs](https://github.com/C2SM/iconarray/workflows/docs/badge.svg?branch=main)](https://c2sm.github.io/iconarray/)
+[![Docs](https://github.com/C2SM/iconarray/workflows/Documentation/badge.svg?branch=main)](https://c2sm.github.io/iconarray/)
 [![Build Status](https://jenkins-mch.cscs.ch/job/iconarray_testsuite/badge/icon?config=build)](https://jenkins-mch.cscs.ch/job/iconarray_testsuite/)
 [![Test Status](https://jenkins-mch.cscs.ch/job/iconarray_testsuite/badge/icon?config=test)](https://jenkins-mch.cscs.ch/job/iconarray_testsuite/)
 
 ## Introduction
 
 The iconarray python package contains various modules to facilitate working with ICON data with xarray or other xarray based tools (such as [psyplot](https://psyplot.github.io/) - a plotting package). The package was developed together with [icon-vis](https://github.com/C2SM/icon-vis).
```

### Comparing `iconarray-0.3.0/iconarray.egg-info/SOURCES.txt` & `iconarray-0.3.1/iconarray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.0/setup.cfg` & `iconarray-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `iconarray-0.3.0/setup.py` & `iconarray-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name="iconarray",  # Required
-    version="v0.3.0",  # Required
+    version="v0.3.1",  # Required
     description="A package of modules for processing and plotting ICON data.",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional
     url="https://github.com/C2SM/iconarray",  # Optional
     author="MeteoSwiss, C2SM",  # Optional
     author_email="victoria.cherkas@meteoswiss.ch, annika.lauber@c2sm.ethz.ch",  # Optional
     # package_dir={"": "iconarray"},  # Optional
```

