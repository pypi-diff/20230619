# Comparing `tmp/xpublish_wms-0.1.dev73.tar.gz` & `tmp/xpublish_wms-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpublish_wms-0.1.dev73.tar", last modified: Mon May 15 17:11:08 2023, max compression
+gzip compressed data, was "xpublish_wms-0.2.0.tar", last modified: Mon Jun 19 18:08:55 2023, max compression
```

## Comparing `xpublish_wms-0.1.dev73.tar` & `xpublish_wms-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,30 @@
-drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-15 17:11:08.650133 xpublish_wms-0.1.dev73/
--rw-r--r--   0 akerney    (502) staff       (20)       34 2023-05-15 13:25:07.000000 xpublish_wms-0.1.dev73/.gitattributes
-drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-15 17:11:08.639731 xpublish_wms-0.1.dev73/.github/
-drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-15 17:11:08.645990 xpublish_wms-0.1.dev73/.github/workflows/
--rw-r--r--   0 akerney    (502) staff       (20)     1766 2023-05-15 15:28:34.000000 xpublish_wms-0.1.dev73/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 akerney    (502) staff       (20)      956 2023-05-15 13:28:23.000000 xpublish_wms-0.1.dev73/.github/workflows/tests.yml
--rw-r--r--   0 akerney    (502) staff       (20)     1432 2023-05-15 13:37:44.000000 xpublish_wms-0.1.dev73/.pre-commit-config.yaml
--rw-r--r--   0 akerney    (502) staff       (20)     1472 2023-05-15 12:15:12.000000 xpublish_wms-0.1.dev73/LICENSE.txt
--rw-r--r--   0 akerney    (502) staff       (20)      220 2023-05-15 12:15:12.000000 xpublish_wms-0.1.dev73/MANIFEST.in
--rw-r--r--   0 akerney    (502) staff       (20)     3995 2023-05-15 17:11:08.650659 xpublish_wms-0.1.dev73/PKG-INFO
--rw-r--r--   0 akerney    (502) staff       (20)     1451 2023-05-15 15:33:21.000000 xpublish_wms-0.1.dev73/README.md
--rw-r--r--   0 akerney    (502) staff       (20)     1759 2023-05-15 17:10:52.000000 xpublish_wms-0.1.dev73/pyproject.toml
--rw-r--r--   0 akerney    (502) staff       (20)      256 2023-05-15 13:25:07.000000 xpublish_wms-0.1.dev73/requirements-dev.txt
--rw-r--r--   0 akerney    (502) staff       (20)       85 2023-05-15 13:25:07.000000 xpublish_wms-0.1.dev73/requirements.txt
--rw-r--r--   0 akerney    (502) staff       (20)      201 2023-05-15 17:11:08.651527 xpublish_wms-0.1.dev73/setup.cfg
-drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-15 17:11:08.649518 xpublish_wms-0.1.dev73/xpublish_wms/
--rw-r--r--   0 akerney    (502) staff       (20)      235 2023-05-15 13:34:24.000000 xpublish_wms-0.1.dev73/xpublish_wms/__init__.py
--rw-r--r--   0 akerney    (502) staff       (20)      170 2023-05-15 17:11:08.000000 xpublish_wms-0.1.dev73/xpublish_wms/_version.py
--rw-r--r--   0 akerney    (502) staff       (20)    16205 2023-05-15 13:34:24.000000 xpublish_wms-0.1.dev73/xpublish_wms/cf_wms.py
--rw-r--r--   0 akerney    (502) staff       (20)    11193 2023-05-15 13:34:24.000000 xpublish_wms-0.1.dev73/xpublish_wms/getmap.py
--rw-r--r--   0 akerney    (502) staff       (20)      987 2023-05-15 13:34:24.000000 xpublish_wms-0.1.dev73/xpublish_wms/plugin.py
--rw-r--r--   0 akerney    (502) staff       (20)     1726 2023-05-15 13:34:24.000000 xpublish_wms-0.1.dev73/xpublish_wms/utils.py
-drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-15 17:11:08.649896 xpublish_wms-0.1.dev73/xpublish_wms.egg-info/
--rw-r--r--   0 akerney    (502) staff       (20)      342 2023-05-15 17:11:08.000000 xpublish_wms-0.1.dev73/xpublish_wms.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:08:55.710201 xpublish_wms-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:08:55.702201 xpublish_wms-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:08:55.706200 xpublish_wms-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-06-19 18:08:55.710201 xpublish_wms-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-19 18:08:55.710201 xpublish_wms-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:08:55.710201 xpublish_wms-0.2.0/xpublish_wms/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/xpublish_wms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 18:08:55.000000 xpublish_wms-0.2.0/xpublish_wms/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/xpublish_wms/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/xpublish_wms/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/xpublish_wms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:08:55.710201 xpublish_wms-0.2.0/xpublish_wms/wms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/xpublish_wms/wms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/xpublish_wms/wms/get_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/xpublish_wms/wms/get_feature_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/xpublish_wms/wms/get_legend_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/xpublish_wms/wms/get_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-19 18:08:09.000000 xpublish_wms-0.2.0/xpublish_wms/wms/get_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:08:55.710201 xpublish_wms-0.2.0/xpublish_wms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-19 18:08:55.000000 xpublish_wms-0.2.0/xpublish_wms.egg-info/SOURCES.txt
```

### Comparing `xpublish_wms-0.1.dev73/.github/workflows/publish-to-pypi.yml` & `xpublish_wms-0.2.0/.github/workflows/publish-to-pypi.yml`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,18 @@
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.x"
 
       # - name: Get tags
       #   run: git fetch --depth=1 origin +refs/tags/*:refs/tags/*
+      - name: Install native dependencies
+        run: |
+          sudo apt-get update
+          sudo apt-get install -y libgeos-dev
 
       - name: Install build tools
         run: |
           python -m pip install --upgrade build
 
       - name: Build binary wheel
         run: python -m build --sdist --wheel . --outdir dist
```

### Comparing `xpublish_wms-0.1.dev73/.github/workflows/tests.yml` & `xpublish_wms-0.2.0/.github/workflows/tests.yml`

 * *Files 22% similar despite different names*

```diff
@@ -12,25 +12,29 @@
       matrix:
         python-version: ["3.9", "3.10", "3.11"]
         os: [windows-latest, ubuntu-latest, macos-latest]
 
     steps:
       - uses: actions/checkout@v2
 
-      - name: Setup Micromamba
-        uses: mamba-org/provision-with-micromamba@main
+      - name: Setup Micromamba ${{ matrix.python-version }}
+        uses: mamba-org/setup-micromamba@v1
         with:
-          environment-file: false
+          environment-name: TEST
+          init-shell: bash
+          create-args: >-
+            python=${{ matrix.python-version }} pip
+            --file requirements.txt
+            --file requirements-dev.txt
+            --channel conda-forge
 
-      - name: Python ${{ matrix.python-version }}
+      - name: Install xpublish-opendap
         shell: bash -l {0}
-        run: |
-          micromamba create --name TEST python=${{ matrix.python-version }} --file requirements.txt --file requirements-dev.txt --channel conda-forge
-          micromamba activate TEST
-          pip install -e . --no-deps --force-reinstall
-          micromamba info --all
-          micromamba list
+        run: >
+          python -m pip install -e . --no-deps --force-reinstall
+          && micromamba info
+          && micromamba list
+
       - name: Tests
         shell: bash -l {0}
         run: |
-          micromamba activate TEST
-          pytest -rxs --cov=xpublish_wms tests
+          python -m pytest -rxs --cov=xpublish_wms tests
```

### Comparing `xpublish_wms-0.1.dev73/.pre-commit-config.yaml` & `xpublish_wms-0.2.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -50,17 +50,17 @@
   rev: v2.2.4
   hooks:
     - id: codespell
       args:
         - --quiet-level=2
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.4.0
+  rev: v3.6.0
   hooks:
     - id: pyupgrade
       args:
         - --py36-plus
 
 - repo: https://github.com/asottile/add-trailing-comma
-  rev: v2.4.0
+  rev: v2.5.1
   hooks:
     - id: add-trailing-comma
```

### Comparing `xpublish_wms-0.1.dev73/LICENSE.txt` & `xpublish_wms-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xpublish_wms-0.1.dev73/pyproject.toml` & `xpublish_wms-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 packages = ["xpublish_wms"]
 
 [tool.setuptools.dynamic]
 dependencies = { file = ["requirements.txt"] }
 
 [tool.setuptools_scm]
 write_to = "xpublish_wms/_version.py"
-local_scheme = "no-local-version"
 
 [tool.check-manifest]
 ignore = [
     "*.yml",
     "*.yaml",
     ".coveragerc",
     "docs",
```

### Comparing `xpublish_wms-0.1.dev73/xpublish_wms/getmap.py` & `xpublish_wms-0.2.0/xpublish_wms/wms/get_map.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,167 @@
 import io
 import logging
-import time
 from datetime import datetime
-from typing import List
+from typing import List, Union
 
 import cachey
+import cartopy.crs as ccrs
 import cf_xarray  # noqa
+import matplotlib.tri as tri
 import numpy as np
 import pandas as pd
 import xarray as xr
 from fastapi.responses import StreamingResponse
 from matplotlib import cm
+from matplotlib.figure import Figure
 from PIL import Image
-from pykdtree.kdtree import KDTree
 from rasterio.enums import Resampling
 from rasterio.transform import from_bounds
 
-from xpublish_wms.utils import lnglat_to_cartesian, to_lnglat
+from xpublish_wms.grid import GridType
+from xpublish_wms.utils import to_lnglat
 
 logger = logging.getLogger(__name__)
 
 
-class OgcWmsGetMap:
+class GetMap:
+    """
+    TODO - Add docstring
+    """
+
     TIME_CF_NAME: str = "time"
-    DEFAULT_CRS: str = "4326"
+    ELEVATION_CF_NAME: str = "vertical"
+    DEFAULT_CRS: str = "EPSG:3857"
     DEFAULT_STYLE: str = "raster/default"
+    DEFAULT_PALETTE: str = "turbo"
 
     cache: cachey.Cache
 
     # Data selection
     parameter: str
     time: datetime = None
+    has_time: bool
+    elevation: float = None
+    has_elevation: bool
 
     # Grid
+    grid_type: GridType
     crs: str
     bbox = List[float]
     width: int
     height: int
 
     # Output style
     style: str
     colorscalerange: List[float]
-    colorbaronly: bool
     autoscale: bool
 
-    def get_map(self, ds: xr.Dataset, query: dict):
+    def __init__(self, cache: cachey.Cache):
+        self.cache = cache
+
+    def get_map(self, ds: xr.Dataset, query: dict) -> StreamingResponse:
         """
         Return the WMS map for the dataset and given parameters
         """
         # Decode request params
-        self.ensure_query_types(query)
+        self.ensure_query_types(ds, query)
 
         # Select data according to request
         da = self.select_layer(ds)
         da = self.select_time(da)
+        da = self.select_elevation(da)
         da = self.select_custom_dim(da)
-        da_bbox = self.select_grid(da)
 
-        # Generate output
-        image_bytes = self.draw(da, da_bbox)
+        # Render the data using the render that matches the dataset type
+        # The data selection and render are coupled because they are both driven by
+        # The grid type for now. This can be revisited if we choose to interpolate or
+        # use the contoured renderer for regular grid datasets
+        image_buffer = io.BytesIO()
+        render_result = self.render(da, image_buffer, False)
+        if render_result:
+            image_buffer.seek(0)
+
+        return StreamingResponse(image_buffer, media_type="image/png")
+
+    def get_minmax(self, ds: xr.Dataset, query: dict) -> dict:
+        """
+        Return the range of values for the dataset and given parameters
+        """
+        entire_layer = False
+        if "bbox" not in query:
+            # When BBOX is not specified, we are just going to slice the layer in time and elevation
+            # and return the min and max values for the entire layer so bbox can just be the whoel world
+            entire_layer = True
+            query["bbox"] = "-180,-90,180,90"
+            query["width"] = 1
+            query["height"] = 1
+
+        # Decode request params
+        self.ensure_query_types(ds, query)
+
+        # Select data according to request
+        da = self.select_layer(ds)
+        da = self.select_time(da)
+        da = self.select_elevation(da)
 
-        return StreamingResponse(image_bytes, media_type="image/png")
+        # Prepare the data as if we are going to render it, but instead grab the min and max
+        # values from the data to represent the range of values in the given area
+        if entire_layer:
+            return {"min": float(da.min()), "max": float(da.max())}
+        else:
+            return self.render(da, None, minmax_only=True)
 
-    def ensure_query_types(self, query: dict):
+    def ensure_query_types(self, ds: xr.Dataset, query: dict):
         """
         Decode request params
 
         :param query:
         :return:
         """
+        self.grid_type = GridType.from_ds(ds)
+
         # Data selection
         self.parameter = query["layers"]
-        time_str = query.get("time", None)
-        if time_str:
-            self.time = pd.to_datetime(time_str).tz_localize(None)
+        self.time_str = query.get("time", None)
+        if self.time_str:
+            self.time = pd.to_datetime(self.time_str).tz_localize(None)
+        else:
+            self.time = None
+        self.has_time = "time" in ds[self.parameter].cf.coordinates
+
+        self.elevation_str = query.get("elevation", None)
+        if self.elevation_str:
+            self.elevation = float(self.elevation_str)
+        else:
+            self.elevation = None
+        self.has_elevation = "vertical" in ds[self.parameter].cf.coordinates
 
         # Grid
         self.crs = query.get("crs", None) or query.get("srs")
         self.bbox = [float(x) for x in query["bbox"].split(",")]
         self.width = int(query["width"])
         self.height = int(query["height"])
 
         # Output style
         self.style = query.get("styles", self.DEFAULT_STYLE)
+        # Let user pick cm from here https://predictablynoisy.com/matplotlib/gallery/color/colormap_reference.html#sphx-glr-gallery-color-colormap-reference-py
+        # Otherwise default to rainbow
+        try:
+            self.stylename, self.palettename = self.style.split("/")
+        except Exception:
+            self.stylename = "raster"
+            self.palettename = "default"
+        finally:
+            if self.palettename == "default":
+                self.palettename = self.DEFAULT_PALETTE
+
         self.colorscalerange = [
             float(x) for x in query.get("colorscalerange", "nan,nan").split(",")
         ]
-        self.autoscale = query.get("autoscale", "true") == "true"
+        self.autoscale = query.get("autoscale", "false") == "true"
 
     def select_layer(self, ds: xr.Dataset) -> xr.DataArray:
         """
         Select Dataset variable, according to WMS layers request
         :param ds:
         :return:
         """
@@ -114,62 +185,92 @@
         if self.time is not None:
             da = da.cf.sel({self.TIME_CF_NAME: self.time}, method="nearest")
         else:
             da = da.cf.isel({self.TIME_CF_NAME: -1})
 
         return da
 
+    def select_elevation(self, da: xr.DataArray) -> xr.DataArray:
+        """
+        Ensure elevation selection
+
+        If elevation is provided :
+            - use cf_xarray to access vertical coord
+            - by default use ELEVATION_CF_NAME
+            - method nearest to ensure at least one result
+
+        Otherwise:
+            - Get latest one
+
+        :param da:
+        :return:
+        """
+        if self.elevation is not None and self.has_elevation:
+            da = da.cf.sel({self.ELEVATION_CF_NAME: self.elevation}, method="nearest")
+        elif self.has_elevation:
+            da = da.cf.isel({self.ELEVATION_CF_NAME: 0})
+
+        return da
+
     def select_custom_dim(self, da: xr.DataArray) -> xr.DataArray:
         """
         Select other dimension, ensuring a 2D array
         :param da:
         :return:
         """
         # Squeeze single value dimensions
         da = da.squeeze()
 
         # TODO: Filter dimension from custom query, if any
 
         # Squeeze multiple values dimensions, by selecting the last value
-        for coord_name in da.cf.coords:
-            if coord_name in ("latitude", "longitude", "X", "Y"):
+        for key in da.cf.coordinates.keys():
+            if key in ("latitude", "longitude", "X", "Y"):
                 continue
-            coord = da.cf.coords[coord_name]
+
+            coord = da.cf.coords[key]
             if coord.size > 1:
-                da = da.cf.isel({coord_name: -1})
+                da = da.cf.isel({key: -1})
 
         return da
 
-    def select_grid(self, da: xr.DataArray) -> xr.DataArray:
+    def render(
+        self,
+        da: xr.DataArray,
+        buffer: io.BytesIO,
+        minmax_only: bool,
+    ) -> Union[bool, dict]:
         """
-        Select grid and reproject if needed
+        Render the data array into an image buffer
         :param da:
         :return:
         """
-        # Some basic check for dataset
-        if not da.rio.crs:
-            da = da.rio.write_crs(self.DEFAULT_CRS)
-
-        if self.grid_is_regular(da):
-            da = self.select_regular_grid(da)
+        if self.grid_type == GridType.REGULAR:
+            return self.render_regular_grid(da, buffer, minmax_only)
+        elif self.grid_type == GridType.SGRID:
+            return self.render_sgrid(da, buffer, minmax_only)
         else:
-            da = self.select_irregular_grid(da)
-        return da
-
-    def grid_is_regular(self, da: xr.DataArray) -> bool:
-        return da.cf.coords["longitude"].dims[0] == da.cf.coords["longitude"].name
+            return False
 
-    def select_regular_grid(self, da: xr.DataArray) -> xr.DataArray:
+    def render_regular_grid(
+        self,
+        da: xr.DataArray,
+        buffer: io.BytesIO,
+        minmax_only: bool,
+    ) -> Union[bool, dict]:
         """
-        Filter regular grid according to WMS request :
-            - bbox
-            - width and height
+        Render the data array into an image buffer when the dataset is using a
+        regularly spaced rectangular grid
         :param da:
         :return:
         """
+        # Some basic check for dataset
+        if not da.rio.crs:
+            da = da.rio.write_crs(self.DEFAULT_CRS)
+
         minx, miny, maxx, maxy = self.bbox
 
         transform = from_bounds(
             west=minx,
             south=miny,
             east=maxx,
             north=maxy,
@@ -186,188 +287,144 @@
         resampled_data = clipped.rio.reproject(
             dst_crs=self.crs,
             shape=(self.width, self.height),
             resampling=Resampling.nearest,
             transform=transform,
         )
 
-        return resampled_data
+        if minmax_only:
+            return {
+                "min": float(resampled_data.min()),
+                "max": float(resampled_data.max()),
+            }
 
-    def select_irregular_grid(self, da: xr.DataArray) -> xr.DataArray:
-        """
-        Filter irregular grid according to WMS request :
-            - bbox
-            - width and height
-        :param da:
-        :return:
-        """
-        ds = da
-        bbox, width, height = self.bbox, self.width, self.height
-
-        start = time.time()
-        min_lng = ds.cf.coords["longitude"].min().values.item()
-        min_lat = ds.cf.coords["latitude"].min().values.item()
-        max_lng = ds.cf.coords["longitude"].max().values.item()
-        max_lat = ds.cf.coords["latitude"].max().values.item()
-
-        # Check if we need to project the bounding box
-        if self.crs == "EPSG:3857":
-            t_lng, t_lat = to_lnglat.transform([bbox[0], bbox[2]], [bbox[1], bbox[3]])
-        else:
-            t_lng = [bbox[0], bbox[2]]
-            t_lat = [bbox[1], bbox[3]]
-
-        lngs = np.linspace(t_lng[0], t_lng[1], width)
-        lats = np.linspace(t_lat[0], t_lat[1], height)
-
-        grid_lngs, grid_lats = np.meshgrid(lngs, lats)
-
-        pts = lnglat_to_cartesian(grid_lngs.ravel(), grid_lats.ravel())
-
-        # Need ll version for masking outside dataset bounds
-        pts_ll = np.column_stack((grid_lngs.ravel(), grid_lats.ravel()))
-        pts_ll_mask = np.array(
-            [
-                x[0] >= min_lng
-                and x[0] <= max_lng
-                and x[1] >= min_lat
-                and x[1] <= max_lat
-                for x in pts_ll
-            ],
-        )
-
-        if np.any(pts_ll_mask):
-            kd = get_spatial_kdtree(ds, self.cache)
-            dist, n = kd.query(pts)
-
-            d_lng = pts[1][0] - pts[0][0]
-            d_lat = pts[1][1] - pts[0][1]
-            d_ele = pts[1][2] - pts[0][2]
-            max_dist = np.sqrt((2 * d_lng) ** 2 + (2 * d_lat) ** 2 + (2 * d_ele))
-            dist_mask = np.where(dist > max_dist)
-
-            logger.info(f"Calculated max dist: {max_dist}")
-            logger.info(f"max dist: {np.max(dist)}")
-            logger.info(f"min dist: {np.min(dist)}")
-            logger.info(f"mean dist: {np.mean(dist)}")
-            logger.info(f"median dist: {np.median(dist)}")
-            logger.info(f"stdev dist: {np.std(dist)}")
-            logger.info("-----------------")
-
-            ni = n.argsort()
-            pp = n[ni]
-
-            index_time = time.time()
-            logger.info(f"index and kdtree irregular: {index_time - start}")
-
-            # This is slow because it has to pull into numpy array, can we do better?
-            # TODO: Can we avoid pulling down fully masked chunks???
-            z = ds.zeta[0][pp].values
-            z = z[ni.argsort()]
-            z[~pts_ll_mask] = np.nan
-            z[dist_mask] = np.nan
-
-            z = z.reshape((height, width))
-
-            extraction_time = time.time()
-            logger.info(f"extract data irregular: {extraction_time - index_time}")
-
-            rds = xr.Dataset(
-                data_vars=dict(
-                    z=(["y", "x"], z),
-                ),
-                coords=dict(
-                    x=(["x"], lngs),
-                    y=(["y"], lats),
-                ),
-            )
-            rds.rio.write_crs(4326, inplace=True)
-            resampled_data = rds.z.rio.reproject(
-                dst_crs=self.crs,
-                shape=(width, height),
-                resampling=Resampling.nearest,
-                transform=from_bounds(*bbox, width=width, height=height),
-            )
-
-            reproject_time = time.time()
-            logger.info(
-                f"clip and reproject irregular: {reproject_time - extraction_time}",
-            )
+        if self.autoscale:
+            min_value = float(resampled_data.min())
+            max_value = float(resampled_data.max())
         else:
-            resampled_data = np.empty((width, height))
-            resampled_data[:] = np.nan
-
-        reproject_time = time.time()
-        logger.info(f"clip and reproject irregular: {reproject_time - extraction_time}")
-        return resampled_data
+            min_value = self.colorscalerange[0]
+            max_value = self.colorscalerange[1]
 
-    def draw(self, da: xr.DataArray, da_bbox: xr.DataArray) -> io.BytesIO:
-        """
-        Generate drawing, could be easily overridden
+        da_scaled = (resampled_data - min_value) / (max_value - min_value)
+        im = Image.fromarray(np.uint8(cm.get_cmap(self.palettename)(da_scaled) * 255))
+        im.save(buffer, format="PNG")
 
-        :param da:
-        :param da_bbox:
-        :return:
-        """
-        da_scaled = self.draw_pil_get_colormap_scaled_data(da, da_bbox)
-        return self.draw_pil_generate_map(da_scaled)
+        return True
 
-    def draw_pil_get_colormap_scaled_data(
+    def render_sgrid(
         self,
         da: xr.DataArray,
-        da_bbox: xr.DataArray,
-    ) -> xr.DataArray:
+        buffer: io.BytesIO,
+        minmax_only: bool,
+    ) -> Union[bool, dict]:
         """
-        Generate numpy array from our datasset, ensuring colormap is computed from the
-        non-clipped data
+        Render the data array into an image buffer when the dataset is using a
+        staggered (ala ROMS) grid
         :param da:
-        :param da_bbox:
         :return:
         """
-        if self.autoscale:
-            min_value = float(da.min())
-            max_value = float(da.max())
+        # TODO: Make this based on the actual chunks of the dataset, for now brute forcing to time and variable
+        if self.has_time:
+            cache_key = f"{self.parameter}_{self.time_str}"
         else:
-            min_value = self.colorscalerange[0]
-            max_value = self.colorscalerange[1]
-
-        return (da_bbox - min_value) / (max_value - min_value)
-
-    def draw_pil_generate_map(self, da: xr.DataArray) -> io.BytesIO:
-        """
-        Draw as PIL.Image
-        :param da:
-        :return:
-        """
-        try:
-            stylename, palettename = self.style.split("/")
-        except:  # noqa: E722
-            palettename = "default"
-
-        # Let user pick cm from here https://predictablynoisy.com/matplotlib/gallery/color/colormap_reference.html#sphx-glr-gallery-color-colormap-reference-py
-        # Otherwise default to rainbow
-        if palettename == "default":
-            palettename = "rainbow"
-        im = Image.fromarray(np.uint8(cm.get_cmap(palettename)(da) * 255))
-
-        image_bytes = io.BytesIO()
-        im.save(image_bytes, format="PNG")
-        image_bytes.seek(0)
+            cache_key = f"{self.parameter}"
+        cache_coord_key = f"{self.parameter}_coords"
 
-        return image_bytes
+        data_cache_key = f"{cache_key}_data"
+        x_cache_key = f"{cache_coord_key}_x"
+        y_cache_key = f"{cache_coord_key}_y"
 
+        if self.crs == "EPSG:3857":
+            bbox_lng, bbox_lat = to_lnglat.transform(
+                [self.bbox[0], self.bbox[2]],
+                [self.bbox[1], self.bbox[3]],
+            )
+            bbox = [*bbox_lng, *bbox_lat]
+        else:
+            bbox = [self.bbox[0], self.bbox[2], self.bbox[1], self.bbox[3]]
 
-def get_spatial_kdtree(ds: xr.Dataset, cache: cachey.Cache) -> KDTree:
-    cache_key = f"dataset-kdtree-{ds.attrs['title']}"
-    kd = cache.get(cache_key)
-    if kd:
-        return kd
-
-    lng = ds.cf["longitude"]
-    lat = ds.cf["latitude"]
-
-    verts = lnglat_to_cartesian(lng, lat)
-    kd = KDTree(verts)
+        data = self.cache.get(data_cache_key, None)
+        if data is None:
+            data = np.array(da.values)
+            self.cache.put(data_cache_key, data, cost=50)
+
+        x = self.cache.get(x_cache_key, None)
+        if x is None:
+            x = np.array(da.cf["longitude"].values)
+            self.cache.put(x_cache_key, x, cost=50)
+
+        y = self.cache.get(y_cache_key, None)
+        if y is None:
+            y = np.array(da.cf["latitude"].values)
+            self.cache.put(y_cache_key, y, cost=50)
+
+        inds = np.where(
+            (x >= (bbox[0] - 0.18))
+            & (x <= (bbox[1] + 0.18))
+            & (y >= (bbox[2] - 0.18))
+            & (y <= (bbox[3] + 0.18)),
+        )
+        x_sel = x[inds]
+        y_sel = y[inds]
+        data_sel = data[inds]
+        if minmax_only:
+            return {
+                "min": float(data_sel.min()),
+                "max": float(data_sel.max()),
+            }
+
+        tris = tri.Triangulation(x_sel, y_sel)
+        data_tris = data_sel[tris.triangles]
+        mask = np.where(np.isnan(data_tris), [True], [False])
+        triangle_mask = np.any(mask, axis=1)
+        tris.set_mask(triangle_mask)
+
+        projection = ccrs.Mercator() if self.crs == "EPSG:3857" else ccrs.PlateCarree()
+
+        dpi = 80
+        fig = Figure(dpi=dpi, facecolor="none", edgecolor="none")
+        fig.set_alpha(0)
+        fig.set_figheight(self.height / dpi)
+        fig.set_figwidth(self.width / dpi)
+        ax = fig.add_axes(
+            [0.0, 0.0, 1.0, 1.0],
+            xticks=[],
+            yticks=[],
+            projection=projection,
+        )
+        ax.set_axis_off()
+        ax.set_frame_on(False)
+        ax.set_clip_on(False)
+        ax.set_position([0, 0, 1, 1])
 
-    cache.put(cache_key, kd, 5)
+        if not self.autoscale:
+            vmin, vmax = self.colorscalerange
+        else:
+            vmin, vmax = [None, None]
 
-    return kd
+        try:
+            # ax.tripcolor(tris, data_sel, transform=ccrs.PlateCarree(), cmap=cmap, shading='flat', vmin=vmin, vmax=vmax)
+            ax.tricontourf(
+                tris,
+                data_sel,
+                transform=ccrs.PlateCarree(),
+                cmap=self.palettename,
+                vmin=vmin,
+                vmax=vmax,
+                levels=80,
+            )
+            # ax.pcolormesh(x, y, data, transform=ccrs.PlateCarree(), cmap=cmap, vmin=vmin, vmax=vmax)
+        except Exception as e:
+            print(e)
+            print(bbox)
+
+        ax.set_extent(bbox, crs=ccrs.PlateCarree())
+        ax.axis("off")
+
+        fig.savefig(
+            buffer,
+            format="png",
+            transparent=True,
+            pad_inches=0,
+            bbox_inches="tight",
+        )
+        return True
```

### Comparing `xpublish_wms-0.1.dev73/xpublish_wms/utils.py` & `xpublish_wms-0.2.0/xpublish_wms/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
-from typing import Union
+from typing import Tuple, Union
 
 import numpy as np
 import xarray as xr
 from pyproj import Transformer
 
+from xpublish_wms.grid import GridType
+
 logger = logging.getLogger(__name__)
 
 
 def lower_case_keys(d: dict) -> dict:
     return {k.lower(): v for k, v in d.items()}
 
 
@@ -59,15 +61,45 @@
 def lnglat_to_cartesian(longitude, latitude):
     """
     Converts latitude and longitude to cartesian coordinates
     """
     lng_rad = np.deg2rad(longitude)
     lat_rad = np.deg2rad(latitude)
 
+    logger.warning(lng_rad)
+
     R = 6371
     x = R * np.cos(lat_rad) * np.cos(lng_rad)
     y = R * np.cos(lat_rad) * np.sin(lng_rad)
     z = R * np.sin(lat_rad)
     return np.column_stack((x, y, z))
 
 
 to_lnglat = Transformer.from_crs(3857, 4326, always_xy=True)
+
+
+def ds_bbox(ds: xr.Dataset) -> Tuple[float, float, float, float]:
+    """
+    Return the bounding box of the dataset
+    :param ds:
+    :return:
+    """
+    grid_type = GridType.from_ds(ds)
+
+    if grid_type == GridType.REGULAR:
+        bbox = [
+            ds.cf.coords["longitude"].min().values.item(),
+            ds.cf.coords["latitude"].min().values.item(),
+            ds.cf.coords["longitude"].max().values.item(),
+            ds.cf.coords["latitude"].max().values.item(),
+        ]
+    elif grid_type == GridType.SGRID:
+        topology = ds.cf["grid_topology"]
+        lng_coord, lat_coord = topology.attrs["face_coordinates"].split(" ")
+        bbox = [
+            ds[lng_coord].min().values.item(),
+            ds[lat_coord].min().values.item(),
+            ds[lng_coord].max().values.item(),
+            ds[lat_coord].max().values.item(),
+        ]
+
+    return bbox
```

