# Comparing `tmp/seiscat-0.1.tar.gz` & `tmp/seiscat-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seiscat-0.1.tar", last modified: Mon Jun 19 14:32:22 2023, max compression
+gzip compressed data, was "seiscat-0.2.tar", last modified: Mon Jun 19 15:28:25 2023, max compression
```

## Comparing `seiscat-0.1.tar` & `seiscat-0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:32:22.605365 seiscat-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-19 14:32:12.000000 seiscat-0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-19 14:32:12.000000 seiscat-0.1/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-19 14:32:12.000000 seiscat-0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-19 14:32:12.000000 seiscat-0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-19 14:32:22.605365 seiscat-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-19 14:32:12.000000 seiscat-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:32:22.605365 seiscat-0.1/seiscat/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-19 14:32:12.000000 seiscat-0.1/seiscat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-19 14:32:22.605365 seiscat-0.1/seiscat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:32:22.605365 seiscat-0.1/seiscat/conf/
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-19 14:32:12.000000 seiscat-0.1/seiscat/conf/configspec.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:32:22.605365 seiscat-0.1/seiscat/configobj/
--rw-r--r--   0 runner    (1001) docker     (123)    88030 2023-06-19 14:32:12.000000 seiscat-0.1/seiscat/configobj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-19 14:32:12.000000 seiscat-0.1/seiscat/configobj/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    46990 2023-06-19 14:32:12.000000 seiscat-0.1/seiscat/configobj/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-19 14:32:12.000000 seiscat-0.1/seiscat/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-19 14:32:12.000000 seiscat-0.1/seiscat/fdsnws.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-06-19 14:32:12.000000 seiscat-0.1/seiscat/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:32:22.605365 seiscat-0.1/seiscat/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-19 14:32:12.000000 seiscat-0.1/seiscat/scripts/seiscat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-19 14:32:12.000000 seiscat-0.1/seiscat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:32:22.601365 seiscat-0.1/seiscat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-19 14:32:22.000000 seiscat-0.1/seiscat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-19 14:32:22.000000 seiscat-0.1/seiscat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 14:32:22.000000 seiscat-0.1/seiscat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-19 14:32:22.000000 seiscat-0.1/seiscat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-19 14:32:22.000000 seiscat-0.1/seiscat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 14:32:22.000000 seiscat-0.1/seiscat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-19 14:32:22.605365 seiscat-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-19 14:32:12.000000 seiscat-0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-06-19 14:32:12.000000 seiscat-0.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:28:25.750739 seiscat-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-19 15:28:14.000000 seiscat-0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-19 15:28:14.000000 seiscat-0.2/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-19 15:28:14.000000 seiscat-0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-19 15:28:14.000000 seiscat-0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-19 15:28:25.750739 seiscat-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-19 15:28:14.000000 seiscat-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:28:25.750739 seiscat-0.2/seiscat/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-19 15:28:14.000000 seiscat-0.2/seiscat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-19 15:28:25.750739 seiscat-0.2/seiscat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:28:25.746739 seiscat-0.2/seiscat/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-19 15:28:14.000000 seiscat-0.2/seiscat/conf/configspec.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:28:25.750739 seiscat-0.2/seiscat/configobj/
+-rw-r--r--   0 runner    (1001) docker     (123)    88030 2023-06-19 15:28:14.000000 seiscat-0.2/seiscat/configobj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-19 15:28:14.000000 seiscat-0.2/seiscat/configobj/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46990 2023-06-19 15:28:14.000000 seiscat-0.2/seiscat/configobj/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-19 15:28:14.000000 seiscat-0.2/seiscat/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-19 15:28:14.000000 seiscat-0.2/seiscat/fdsnws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-06-19 15:28:14.000000 seiscat-0.2/seiscat/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:28:25.750739 seiscat-0.2/seiscat/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-19 15:28:14.000000 seiscat-0.2/seiscat/scripts/seiscat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-19 15:28:14.000000 seiscat-0.2/seiscat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:28:25.746739 seiscat-0.2/seiscat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-19 15:28:25.000000 seiscat-0.2/seiscat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-19 15:28:25.000000 seiscat-0.2/seiscat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:28:25.000000 seiscat-0.2/seiscat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-19 15:28:25.000000 seiscat-0.2/seiscat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-19 15:28:25.000000 seiscat-0.2/seiscat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 15:28:25.000000 seiscat-0.2/seiscat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-19 15:28:25.750739 seiscat-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-19 15:28:14.000000 seiscat-0.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-06-19 15:28:14.000000 seiscat-0.2/versioneer.py
```

### Comparing `seiscat-0.1/LICENSE.txt` & `seiscat-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seiscat-0.1/PKG-INFO` & `seiscat-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seiscat
-Version: 0.1
+Version: 0.2
 Summary: Keep a local seismic catalog
 Home-page: https://github.com/SeismicSource/SeisCat
 Author: Claudio Satriano
 Author-email: satriano@ipgp.fr
 License: GNU General Public License v3 or later (GPLv3+)
 Platform: OS Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `seiscat-0.1/README.md` & `seiscat-0.2/README.md`

 * *Files identical despite different names*

### Comparing `seiscat-0.1/seiscat/conf/configspec.conf` & `seiscat-0.2/seiscat/conf/configspec.conf`

 * *Files identical despite different names*

### Comparing `seiscat-0.1/seiscat/configobj/__init__.py` & `seiscat-0.2/seiscat/configobj/__init__.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.1/seiscat/configobj/validate.py` & `seiscat-0.2/seiscat/configobj/validate.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.1/seiscat/db.py` & `seiscat-0.2/seiscat/db.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.1/seiscat/fdsnws.py` & `seiscat-0.2/seiscat/fdsnws.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.1/seiscat/plot.py` & `seiscat-0.2/seiscat/plot.py`

 * *Files 18% similar despite different names*

```diff
@@ -47,15 +47,22 @@
 def _get_map_extent(config):
     """
     Get the map extent from the config file.
 
     :param config: config object
     :returns: lon_min, lon_max, lat_min, lat_max
     """
-    lon_min, lon_max, lat_min, lat_max = _get_map_extent_for_suffix(config)
+    ret = _get_map_extent_for_suffix(config)
+    if ret is None:
+        lon_min = -179
+        lon_max = 180
+        lat_min = -75
+        lat_max = 80
+    else:
+        lon_min, lon_max, lat_min, lat_max = ret
     # see if there are additional limits in the config file
     n = 1
     while True:
         ret = _get_map_extent_for_suffix(config, suffix=f'_{n}')
         if ret is None:
             break
         lon_min_, lon_max_, lat_min_, lat_max_ = ret
@@ -63,28 +70,32 @@
         lon_max = max(lon_max, lon_max_)
         lat_min = min(lat_min, lat_min_)
         lat_max = max(lat_max, lat_max_)
         n += 1
     return lon_min, lon_max, lat_min, lat_max
 
 
-def _get_tile_zoom_level(ax):
+def _get_tile_scale(extent):
     """
-    Empirical formula to get the zoom level for a tile.
+    Get the tile scale for a given extent.
 
     :param extent: tuple (lon_min, lon_max, lat_min, lat_max)
-    :returns: zoom level
+    :returns: tile scale
     """
-    extent = ax.get_extent()
-    area = (extent[1] - extent[0]) * (extent[3] - extent[2])
-    levels = [1e14, 1e13, 1e12, 1e11, 1e9, 1e8, 1e7, 1e6, 1e5]
-    zoom_level = np.argmin(np.abs(np.array(levels) - area)) + 6
-    # uncomment to debug
-    # print(f'area: {area:.1e}, zoom_level: {zoom_level:d}')
-    return int(zoom_level)
+    from cartopy.feature import AdaptiveScaler
+    tile_autoscaler = AdaptiveScaler(
+        default_scale=4,
+        limits=(
+            (4, 180), (5, 90), (6, 45), (7, 25), (8, 15), (9, 5),
+            (10, 2), (11, 1),
+        )
+    )
+    tile_scale = tile_autoscaler.scale_from_extent(extent)
+    # print(f'tile_scale: {tile_scale}')
+    return int(tile_scale)
 
 
 def _read_event_db(config):
     """
     Read event database. Return a list of events.
 
     :param config: config object
@@ -139,14 +150,15 @@
         '', xy=(0, 0), xytext=(5, 5),
         textcoords='offset points',
         bbox=dict(boxstyle='round', fc='w'),
         zorder=20
     )
     annot.set_visible(False)
     fig = ax.get_figure()
+
     def hover(event):
         vis = annot.get_visible()
         if vis:
             annot.set_visible(False)
             fig.canvas.draw_idle()
         if event.inaxes != ax:
             return
@@ -161,15 +173,14 @@
                 annot.set_visible(True)
             else:
                 marker.set_linewidth(1)
         fig.canvas.draw_idle()
     fig.canvas.mpl_connect('motion_notify_event', hover)
 
 
-
 def plot_catalog_map(config):
     """
     Plot the catalog map.
 
     :param config: config object
     """
     # lazy import cartopy, since it's not an install requirement
@@ -183,19 +194,22 @@
             'See https://scitools.org.uk/cartopy/docs/latest/installing.html'
         )
     fig = plt.figure(figsize=(10, 10))
     stamen_terrain = cimgt.Stamen('terrain-background')
     ax = fig.add_subplot(1, 1, 1, projection=stamen_terrain.crs)
     extent = _get_map_extent(config)
     ax.set_extent(extent)
-    ax.add_image(stamen_terrain, _get_tile_zoom_level(ax))
+    tile_scale = _get_tile_scale(extent)
+    ax.add_image(stamen_terrain, tile_scale)
     ax.coastlines(resolution='10m', edgecolor='black', linewidth=1)
-    ax.add_feature(ccrs.cartopy.feature.BORDERS, edgecolor='black', linewidth=1)
+    ax.add_feature(
+        ccrs.cartopy.feature.BORDERS, edgecolor='black', linewidth=1)
     g_kwargs = dict(draw_labels=True, dms=True, x_inline=False, y_inline=False)
     ax.gridlines(**g_kwargs)
+
     def redraw_gridlines(ax):
         ax.gridlines(**g_kwargs)
     ax.callbacks.connect('xlim_changed', lambda ax: redraw_gridlines(ax))
     events = _read_event_db(config)
     _plot_events(events, ax)
     nevents = len(events)
     tmin = min(event['time'] for event in events)
```

### Comparing `seiscat-0.1/seiscat/scripts/seiscat.py` & `seiscat-0.2/seiscat/scripts/seiscat.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.1/seiscat/utils.py` & `seiscat-0.2/seiscat/utils.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.1/seiscat.egg-info/PKG-INFO` & `seiscat-0.2/seiscat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seiscat
-Version: 0.1
+Version: 0.2
 Summary: Keep a local seismic catalog
 Home-page: https://github.com/SeismicSource/SeisCat
 Author: Claudio Satriano
 Author-email: satriano@ipgp.fr
 License: GNU General Public License v3 or later (GPLv3+)
 Platform: OS Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `seiscat-0.1/seiscat.egg-info/SOURCES.txt` & `seiscat-0.2/seiscat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seiscat-0.1/setup.py` & `seiscat-0.2/setup.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.1/versioneer.py` & `seiscat-0.2/versioneer.py`

 * *Files identical despite different names*

