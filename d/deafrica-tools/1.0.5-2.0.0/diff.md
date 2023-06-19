# Comparing `tmp/deafrica-tools-1.0.5.tar.gz` & `tmp/deafrica_tools-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deafrica-tools-1.0.5.tar", last modified: Mon Jun 12 14:48:47 2023, max compression
+gzip compressed data, was "deafrica_tools-2.0.0.tar", max compression
```

## Comparing `deafrica-tools-1.0.5.tar` & `deafrica_tools-2.0.0.tar`

### file list

```diff
@@ -1,43 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:47.283860 deafrica-tools-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-12 14:48:47.283860 deafrica-tools-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:47.279860 deafrica-tools-1.0.5/deafrica_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:47.283860 deafrica-tools-1.0.5/deafrica_tools/app/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31281 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/app/animations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/app/changefilmstrips.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/app/crophealth.py
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/app/deacoastlines.py
--rw-r--r--   0 runner    (1001) docker     (123)    37648 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/app/forestmonitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/app/geomedian.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/app/imageexport.py
--rw-r--r--   0 runner    (1001) docker     (123)    12980 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/app/wetlandsinsighttool.py
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/app/widgetconstructors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/areaofinterest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/bandindices.py
--rw-r--r--   0 runner    (1001) docker     (123)    61473 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    23347 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/coastal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)    35752 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/datahandling.py
--rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/load_era5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/load_isda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:47.279860 deafrica-tools-1.0.5/deafrica_tools/locales/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:47.279860 deafrica-tools-1.0.5/deafrica_tools/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:47.283860 deafrica-tools-1.0.5/deafrica_tools/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po
--rw-r--r--   0 runner    (1001) docker     (123)    50494 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    36679 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)    25800 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/wetlands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:47.279860 deafrica-tools-1.0.5/deafrica_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-12 14:48:47.000000 deafrica-tools-1.0.5/deafrica_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-12 14:48:47.000000 deafrica-tools-1.0.5/deafrica_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:48:47.000000 deafrica-tools-1.0.5/deafrica_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-12 14:48:47.000000 deafrica-tools-1.0.5/deafrica_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 14:48:47.000000 deafrica-tools-1.0.5/deafrica_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 14:48:47.283860 deafrica-tools-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/setup.py
+-rw-r--r--   0        0        0    11357 2023-06-19 06:48:50.178113 deafrica_tools-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2587 2023-06-19 06:48:50.178113 deafrica_tools-2.0.0/README.md
+-rw-r--r--   0        0        0      676 2023-06-19 06:48:50.178113 deafrica_tools-2.0.0/deafrica_tools/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/app/__init__.py
+-rw-r--r--   0        0        0    31449 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/app/animations.py
+-rw-r--r--   0        0        0    10984 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/app/changefilmstrips.py
+-rw-r--r--   0        0        0    10494 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/app/crophealth.py
+-rw-r--r--   0        0        0    20287 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/app/deacoastlines.py
+-rw-r--r--   0        0        0    37843 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/app/forestmonitoring.py
+-rw-r--r--   0        0        0     8673 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/app/geomedian.py
+-rw-r--r--   0        0        0    13383 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/app/imageexport.py
+-rw-r--r--   0        0        0    13148 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/app/wetlandsinsighttool.py
+-rw-r--r--   0        0        0     9882 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/app/widgetconstructors.py
+-rw-r--r--   0        0        0     2043 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/areaofinterest.py
+-rw-r--r--   0        0        0    24548 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/bandindices.py
+-rw-r--r--   0        0        0    61473 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/classification.py
+-rw-r--r--   0        0        0    23515 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/coastal.py
+-rw-r--r--   0        0        0     3404 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/dask.py
+-rw-r--r--   0        0        0    35752 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/datahandling.py
+-rw-r--r--   0        0        0    14369 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/load_era5.py
+-rw-r--r--   0        0        0     2793 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/load_isda.py
+-rw-r--r--   0        0        0     2027 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/load_soil_moisture.py
+-rw-r--r--   0        0        0     1783 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo
+-rw-r--r--   0        0        0     2841 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po
+-rw-r--r--   0        0        0    50697 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/plotting.py
+-rw-r--r--   0        0        0    36957 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/spatial.py
+-rw-r--r--   0        0        0    17245 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/temporal.py
+-rw-r--r--   0        0        0    25961 2023-06-19 06:48:50.182113 deafrica_tools-2.0.0/deafrica_tools/wetlands.py
+-rw-r--r--   0        0        0     3310 2023-06-19 06:48:50.186113 deafrica_tools-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5067 1970-01-01 00:00:00.000000 deafrica_tools-2.0.0/PKG-INFO
```

### Comparing `deafrica-tools-1.0.5/LICENSE` & `deafrica_tools-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.5/PKG-INFO` & `deafrica_tools-2.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: deafrica-tools
-Version: 1.0.5
-Summary: Functions and algorithms for analysing Digital Earth Africa data.
-Home-page: https://github.com/digitalearthafrica/deafrica-sandbox-notebooks
-Author: Digital Earth Africa
-Author-email: systems@digitalearthafrica.org
-License: Apache License 2.0
-Project-URL: Bug Tracker, https://github.com/digitalearthafrica/deafrica-sandbox-notebooks/issues
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <img align="centre" src="https://github.com/digitalearthafrica/deafrica-sandbox-notebooks/blob/main/Supplementary_data/Github_banner.jpg?raw=true" width="100%">
 
 # Digital Earth Africa Tools Package
 
 Python functions and algorithms developed to assist in analysing Digital Earth Africa data (e.g. loading data, plotting, spatial analysis, machine learning).
 
 ## Installation
```

### Comparing `deafrica-tools-1.0.5/deafrica_tools/__init__.py` & `deafrica_tools-2.0.0/deafrica_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.5"
+__version__ = "2.0.0"
 
 __locales__ = __path__[0] + '/locales'
 
 
 def set_lang(lang=None):
     if lang is None:
         import os
```

### Comparing `deafrica-tools-1.0.5/deafrica_tools/app/animations.py` & `deafrica_tools-2.0.0/deafrica_tools/app/animations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # -*- coding: utf-8 -*-
 """
 Satellite imagery animation widget, which can be used to interactively 
 produce animations for multiple DE Africa products.
 """
 
 # Import required packages
+
+# Force GeoPandas to use Shapely instead of PyGEOS
+# In a future release, GeoPandas will switch to using Shapely by default.
+import os
+os.environ['USE_PYGEOS'] = '0'
+
 import fiona
 import sys
 import datacube
 import warnings
 import matplotlib.pyplot as plt
 from datacube.utils.geometry import CRS
 from ipyleaflet import (
```

### Comparing `deafrica-tools-1.0.5/deafrica_tools/app/changefilmstrips.py` & `deafrica_tools-2.0.0/deafrica_tools/app/changefilmstrips.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.5/deafrica_tools/app/crophealth.py` & `deafrica_tools-2.0.0/deafrica_tools/app/crophealth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # crophealth.py
 '''
 Functions for loading and interacting with data in the crop health notebook,
  inside the Real_world_examples folder.
 '''
 
 # Load modules
+
+# Force GeoPandas to use Shapely instead of PyGEOS
+# In a future release, GeoPandas will switch to using Shapely by default.
+import os
+os.environ['USE_PYGEOS'] = '0'
+
 from ipyleaflet import (
     Map,
     GeoJSON,
     DrawControl,
     basemaps
 )
 import datetime as dt
```

### Comparing `deafrica-tools-1.0.5/deafrica_tools/app/deacoastlines.py` & `deafrica_tools-2.0.0/deafrica_tools/app/deacoastlines.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 """
 Digital Earth Africa Coastline widget, which can be used to 
 interactively extract shoreline data using transects.
 """
 
 # Import required packages
-import fiona
+
+# Force GeoPandas to use Shapely instead of PyGEOS
+# In a future release, GeoPandas will switch to using Shapely by default.
 import os
+os.environ['USE_PYGEOS'] = '0'
+
+import fiona
 import sys
 import datacube
 import warnings
 import matplotlib.pyplot as plt
 from datacube.utils.geometry import CRS
 from ipyleaflet import (
     WMSLayer,
```

### Comparing `deafrica-tools-1.0.5/deafrica_tools/app/forestmonitoring.py` & `deafrica_tools-2.0.0/deafrica_tools/app/forestmonitoring.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 '''
 Functions for loading and interacting with Global Forest Change data in the forest monitoring notebook, inside the Real_world_examples folder.
 '''
 
+# Import required packages
+
+# Force GeoPandas to use Shapely instead of PyGEOS
+# In a future release, GeoPandas will switch to using Shapely by default.
+import os
+os.environ['USE_PYGEOS'] = '0'
+
 import json
 import warnings
 from io import BytesIO
 
 import deafrica_tools.app.widgetconstructors as deawidgets
 import geopandas as gpd
 import ipywidgets as widgets
```

### Comparing `deafrica-tools-1.0.5/deafrica_tools/app/geomedian.py` & `deafrica_tools-2.0.0/deafrica_tools/app/geomedian.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.5/deafrica_tools/app/imageexport.py` & `deafrica_tools-2.0.0/deafrica_tools/app/imageexport.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.5/deafrica_tools/app/wetlandsinsighttool.py` & `deafrica_tools-2.0.0/deafrica_tools/app/wetlandsinsighttool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 """
 Wetlands insight tool widget, which can be used to run an interactive
 version of the wetlands insight tool.
 """
 
 # Import required packages
+
+# Force GeoPandas to use Shapely instead of PyGEOS
+# In a future release, GeoPandas will switch to using Shapely by default.
+import os
+os.environ['USE_PYGEOS'] = '0'
+
 import datacube
 import warnings
 import seaborn as sns
 import matplotlib.pyplot as plt
 from datacube.utils.geometry import CRS
 from ipyleaflet import (
     WMSLayer,
```

### Comparing `deafrica-tools-1.0.5/deafrica_tools/app/widgetconstructors.py` & `deafrica_tools-2.0.0/deafrica_tools/app/widgetconstructors.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.5/deafrica_tools/areaofinterest.py` & `deafrica_tools-2.0.0/deafrica_tools/areaofinterest.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 """
 Function for defining an area of interest using either a point and buffer or a shapefile file. 
 """
 
+# Import required packages
+
+# Force GeoPandas to use Shapely instead of PyGEOS
+# In a future release, GeoPandas will switch to using Shapely by default.
+import os
+os.environ['USE_PYGEOS'] = '0'
+
 import geopandas as gpd
 from shapely.geometry import box
 from geojson import Feature, Point, FeatureCollection
 
 def define_area(lat=None, lon=None, buffer=None, shapefile_path=None):
     '''
     Define an area of interest using either a point and buffer or a shapefile.
```

### Comparing `deafrica-tools-1.0.5/deafrica_tools/bandindices.py` & `deafrica_tools-2.0.0/deafrica_tools/bandindices.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.5/deafrica_tools/classification.py` & `deafrica_tools-2.0.0/deafrica_tools/classification.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.5/deafrica_tools/coastal.py` & `deafrica_tools-2.0.0/deafrica_tools/coastal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 """
 Coastal analyses on Digital Earth Africa data.
 """
 
 # Import required packages
+
+# Force GeoPandas to use Shapely instead of PyGEOS
+# In a future release, GeoPandas will switch to using Shapely by default.
+import os
+os.environ['USE_PYGEOS'] = '0'
+
 import requests
 import numpy as np
 import xarray as xr
 import pandas as pd
 import geopandas as gpd
 import matplotlib.pyplot as plt
 from scipy import stats
```

### Comparing `deafrica-tools-1.0.5/deafrica_tools/dask.py` & `deafrica_tools-2.0.0/deafrica_tools/dask.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.5/deafrica_tools/datahandling.py` & `deafrica_tools-2.0.0/deafrica_tools/datahandling.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.5/deafrica_tools/load_era5.py` & `deafrica_tools-2.0.0/deafrica_tools/load_era5.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         # re-order along longitude to go from -180 to 180 if needed
         if min(lon) < 0:
             ds = ds.assign_coords({"lon": (((ds.lon + 180) % 360) - 180)})
             ds = ds.reindex({"lon": np.sort(ds.lon)})
 
         if lat_range is None:
             # find the nearest lat lon boundary points
-            test = ds.sel(lat=lat, lon=lon, method="nearest")
+            test = ds.sel(lat=list(lat), lon=list(lon), method="nearest")
             # define the lat/lon grid
             lat_range = slice(test.lat.max().values, test.lat.min().values)
             lon_range = slice(test.lon.min().values, test.lon.max().values)
        
         if "time0" in ds.dims:
             ds = ds.rename({"time0": "time"})
         if "time1" in ds.dims:
```

### Comparing `deafrica-tools-1.0.5/deafrica_tools/load_isda.py` & `deafrica_tools-2.0.0/deafrica_tools/load_isda.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.5/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo` & `deafrica_tools-2.0.0/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.5/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po` & `deafrica_tools-2.0.0/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.5/deafrica_tools/plotting.py` & `deafrica_tools-2.0.0/deafrica_tools/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 """
 Functions for plotting Digital Earth Africa data.
 """
 
 # Import required packages
+
+# Force GeoPandas to use Shapely instead of PyGEOS
+# In a future release, GeoPandas will switch to using Shapely by default.
+import os
+os.environ['USE_PYGEOS'] = '0'
+
 import math
 import folium
 import ipywidgets
 import branca
 import numpy as np
 import geopandas as gpd
 import matplotlib as mpl
 import matplotlib.patheffects as PathEffects
 import matplotlib.pyplot as plt
 import matplotlib.animation as animation
 from datetime import datetime
 import matplotlib.cm as cm
 from matplotlib import colors as mcolours
-from pyproj import Proj, transform
+from pyproj import Transformer
 from IPython.display import display
 from matplotlib.colors import ListedColormap
 from mpl_toolkits.axes_grid1.inset_locator import inset_axes
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from ipyleaflet import Map, Marker, Popup, GeoJSON, basemaps, Choropleth
 from skimage import exposure
 from branca.colormap import linear
@@ -277,15 +283,16 @@
     viewport is the closest it can possibly get to the centered
     bounding rectangle without clipping it.
     """
 
     # Convert each corner coordinates to lat-lon
     all_x = (x[0], x[1], x[0], x[1])
     all_y = (y[0], y[0], y[1], y[1])
-    all_longitude, all_latitude = transform(Proj(crs), Proj("EPSG:4326"), all_x, all_y)
+    transformer = Transformer.from_crs(crs, "EPSG:4326")
+    all_longitude, all_latitude = transformer.transform(all_x, all_y)
 
     # Calculate zoom level based on coordinates
     lat_zoom_level = (
         _degree_to_zoom_level(min(all_latitude), max(all_latitude), margin=margin)
         + zoom_bias
     )
     lon_zoom_level = (
```

### Comparing `deafrica-tools-1.0.5/deafrica_tools/spatial.py` & `deafrica_tools-2.0.0/deafrica_tools/spatial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 '''
 Spatial analyses functions for Digital Earth Africa data.
 '''
 
 # Import required packages
+
+# Force GeoPandas to use Shapely instead of PyGEOS
+# In a future release, GeoPandas will switch to using Shapely by default.
+import os
+os.environ['USE_PYGEOS'] = '0'
+
 import fiona
 import collections
 import numpy as np
 import xarray as xr
 from osgeo import osr
 from osgeo import ogr
 import geopandas as gpd
@@ -665,14 +671,16 @@
         
     Returns
     -------
     A numpy array with three columns giving the X, Y and Z coordinates 
     of each vertex in the input GeoDataFrame.
         
     """        
+    # Explode multi-part geometries into multiple single geometries.
+    gdf = gdf.explode(ignore_index=True)
 
     coords_zvals = []
 
     for i in range(0, len(gdf)):
 
         val = gdf.iloc[i][col]
```

### Comparing `deafrica-tools-1.0.5/deafrica_tools/temporal.py` & `deafrica_tools-2.0.0/deafrica_tools/temporal.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
     if method_sos == "first":
         # find index (argmin) where distance is most negative
         idx = allNaN_arg(distance, "time", "min").astype("int16")
 
     if method_sos == "median":
         # find index (argmin) where distance is smallest absolute value
-        idx = allNaN_arg(xr.ufuncs.fabs(distance), "time", "min").astype("int16")
+        idx = allNaN_arg(np.fabs(distance), "time", "min").astype("int16")
 
     return pos_greenup.isel(time=idx)
 
 
 def _sos(vsos):
     """
     SOS = DOY for start of season
@@ -161,15 +161,15 @@
 
     if method_eos == "last":
         # index where last negative slope occurs
         idx = allNaN_arg(distance, "time", "min").astype("int16")
 
     if method_eos == "median":
         # index where median occurs
-        idx = allNaN_arg(xr.ufuncs.fabs(distance), "time", "min").astype("int16")
+        idx = allNaN_arg(np.fabs(distance), "time", "min").astype("int16")
 
     return neg_senesce.isel(time=idx)
 
 
 def _eos(veos):
     """
     EOS = DOY for end of seasonn
```

### Comparing `deafrica-tools-1.0.5/deafrica_tools/wetlands.py` & `deafrica_tools-2.0.0/deafrica_tools/wetlands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 """
 Functions for working with the Wetlands Insight Tool (WIT)
 """
 
 # Import required packages
+
+# Force GeoPandas to use Shapely instead of PyGEOS
+# In a future release, GeoPandas will switch to using Shapely by default.
+import os
+os.environ['USE_PYGEOS'] = '0'
+
 import warnings
 import numpy as np
 import pandas as pd
 import geopandas as gpd
 import seaborn as sns
 import xarray as xr
 import matplotlib.pyplot as plt
@@ -207,15 +213,15 @@
     # seem to handle floats the way we want it to
     fc_int = fc_ds_noTCW.astype("int8")
 
     # use nanargmax to get the index of the maximum value
     BSPVNPV = fc_int.argmax(dim="variable")
     
     #int dytype remocves NaNs so we need to create mask again
-    FC_mask = xr.ufuncs.isfinite(fc_ds_noTCW).all(dim="variable")
+    FC_mask = np.isfinite(fc_ds_noTCW).all(dim="variable")
     BSPVNPV = BSPVNPV.where(FC_mask)
 
     # Restack the Fractional cover dataset all together
     # CAUTION:ARGMAX DEPENDS ON ORDER OF VARIABALES IN
     # DATASET. NEED TO ADJUST BELOW DEPENDING ON ORDER OF FC VARIABLES
     
     FC_dominant = xr.Dataset(
```

