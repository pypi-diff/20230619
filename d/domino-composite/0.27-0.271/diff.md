# Comparing `tmp/domino-composite-0.27.tar.gz` & `tmp/domino-composite-0.271.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domino-composite-0.27.tar", last modified: Mon Jun 19 15:39:14 2023, max compression
+gzip compressed data, was "domino-composite-0.271.tar", last modified: Mon Jun 19 15:46:24 2023, max compression
```

## Comparing `domino-composite-0.27.tar` & `domino-composite-0.271.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-06-19 15:39:14.273861 domino-composite-0.27/
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1212 2023-06-19 15:39:14.273861 domino-composite-0.27/PKG-INFO
-drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-06-19 15:39:14.273861 domino-composite-0.27/domino/
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       62 2022-11-23 14:01:08.000000 domino-composite-0.27/domino/__init__.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1034 2023-06-19 15:18:52.000000 domino-composite-0.27/domino/agg.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     2702 2022-11-23 14:10:17.000000 domino-composite-0.27/domino/categorical_analysis.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)    50731 2023-06-19 15:18:52.000000 domino-composite-0.27/domino/core.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     4248 2023-01-30 10:05:05.000000 domino-composite-0.27/domino/deseasonaliser.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     3810 2023-06-19 15:18:52.000000 domino-composite-0.27/domino/filtering.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     4784 2023-04-03 16:12:11.000000 domino-composite-0.27/domino/plsr.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)    14070 2023-04-12 16:04:19.000000 domino-composite-0.27/domino/prediction.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     5814 2023-06-19 15:18:52.000000 domino-composite-0.27/domino/util.py
-drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-06-19 15:39:14.273861 domino-composite-0.27/domino_composite.egg-info/
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1212 2023-06-19 15:39:14.000000 domino-composite-0.27/domino_composite.egg-info/PKG-INFO
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      382 2023-06-19 15:39:14.000000 domino-composite-0.27/domino_composite.egg-info/SOURCES.txt
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)        1 2023-06-19 15:39:14.000000 domino-composite-0.27/domino_composite.egg-info/dependency_links.txt
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       62 2023-06-19 15:39:14.000000 domino-composite-0.27/domino_composite.egg-info/requires.txt
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)        7 2023-06-19 15:39:14.000000 domino-composite-0.27/domino_composite.egg-info/top_level.txt
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       38 2023-06-19 15:39:14.273861 domino-composite-0.27/setup.cfg
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      727 2023-06-19 15:39:03.000000 domino-composite-0.27/setup.py
+drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-06-19 15:46:24.223301 domino-composite-0.271/
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1213 2023-06-19 15:46:24.223301 domino-composite-0.271/PKG-INFO
+drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-06-19 15:46:24.223301 domino-composite-0.271/domino/
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       62 2022-11-23 14:01:08.000000 domino-composite-0.271/domino/__init__.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1034 2023-06-19 15:18:52.000000 domino-composite-0.271/domino/agg.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     2702 2022-11-23 14:10:17.000000 domino-composite-0.271/domino/categorical_analysis.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)    50731 2023-06-19 15:18:52.000000 domino-composite-0.271/domino/core.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     4248 2023-01-30 10:05:05.000000 domino-composite-0.271/domino/deseasonaliser.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     3846 2023-06-19 15:45:24.000000 domino-composite-0.271/domino/filtering.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     4784 2023-04-03 16:12:11.000000 domino-composite-0.271/domino/plsr.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)    14070 2023-04-12 16:04:19.000000 domino-composite-0.271/domino/prediction.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     5814 2023-06-19 15:18:52.000000 domino-composite-0.271/domino/util.py
+drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-06-19 15:46:24.223301 domino-composite-0.271/domino_composite.egg-info/
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1213 2023-06-19 15:46:24.000000 domino-composite-0.271/domino_composite.egg-info/PKG-INFO
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      382 2023-06-19 15:46:24.000000 domino-composite-0.271/domino_composite.egg-info/SOURCES.txt
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)        1 2023-06-19 15:46:24.000000 domino-composite-0.271/domino_composite.egg-info/dependency_links.txt
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       62 2023-06-19 15:46:24.000000 domino-composite-0.271/domino_composite.egg-info/requires.txt
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)        7 2023-06-19 15:46:24.000000 domino-composite-0.271/domino_composite.egg-info/top_level.txt
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       38 2023-06-19 15:46:24.223301 domino-composite-0.271/setup.cfg
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      728 2023-06-19 15:46:01.000000 domino-composite-0.271/setup.py
```

### Comparing `domino-composite-0.27/PKG-INFO` & `domino-composite-0.271/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-composite
-Version: 0.27
+Version: 0.271
 Summary: A package for compositing atmospheric datasets
 Home-page: https://github.com/joshdorrington/domino
 Author: Josh Dorrington
 Author-email: joshua.dorrington@kit.edu
 License: bsd-3-clause
 Description-Content-Type: text/markdown
```

### Comparing `domino-composite-0.27/domino/agg.py` & `domino-composite-0.271/domino/agg.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.27/domino/categorical_analysis.py` & `domino-composite-0.271/domino/categorical_analysis.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.27/domino/core.py` & `domino-composite-0.271/domino/core.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.27/domino/deseasonaliser.py` & `domino-composite-0.271/domino/deseasonaliser.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.27/domino/filtering.py` & `domino-composite-0.271/domino/filtering.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,28 +10,25 @@
     dtheta=lat1-lat0
     A=r2*np.abs(np.cos(theta))*dtheta*dphi #in km**2
     return A
 
 def grid_area(da,lat_coord='lat',lon_coord='lon',r=6371):
     lat=da[lat_coord].values
     lon=da[lon_coord].values
-    
-    #If coords are descending, we sort that out by
-    #just taking absolute value of the final area
-    dlon=(lon[1:]-lon[:-1])/2 
+    dlon=(lon[1:]-lon[:-1])/2
     dlat=(lat[1:]-lat[:-1])/2
     dlon=[np.median(dlon),*dlon]
     dlat=[np.median(dlat),*dlat]
     areas=np.array([[\
         latlonarea(la-dla,la+dla,lo-dlo,lo+dlo,r=r)\
         for la,dla in zip(lat,dlat)]\
         for lo,dlo in zip(lon,dlon)])
     area=xr.DataArray(data=areas.T,\
-        coords={lat_coord:lat,lon_coord:lon},dims=[lat_coord,lon_coord])
-    return np.abs(area)
+        coords={lat_coord:lat,lon_coord:lon})
+    return area
 
 
 def apply_2d_func_to_da(da,func,*args,dims=None):
     da=da.copy(deep=True)
     da_dim=None    
     if dims is not None:
         #if dims is specified, ignore da's without all dims
@@ -95,15 +92,19 @@
         return apply_2d_func_to_da(da,get_area_regions,n,area,dims=dims)
     else:
         return apply_2d_func_to_da(da,get_large_regions,n,dims=dims)
 
 def ds_large_regions(mask_ds,n,dims,area_based=False):
         ds=mask_ds.copy()
         for var in list(ds.data_vars):
-            ds[var]=da_large_regions(ds[var],n,dims,area_based=area_based)
+            
+            if (dims is not None) and (not np.all([d in mask_ds.dims for d in dims])):
+                pass #ignore variables with missing dims
+            else:
+                ds[var]=da_large_regions(ds[var],n,dims,area_based=area_based)
         return ds
 
 def convolve_pad(x,N):
     Y=np.array([np.convolve(y,np.ones(np.min([N,len(y)])),mode='same') for y in x])
     Y=np.array([np.convolve(y,np.ones(np.min([N,len(y)])),mode='same') for y in Y.T]).T
     Y[Y>0]=1
     return Y
@@ -114,8 +115,8 @@
 def convolve_pad_ds(ds,n,dims):
     ds=ds.copy()
     for var in list(ds.data_vars):
         ds[var]=convolve_pad_da(ds[var],n,dims=dims)
     return ds
 
 def std_filter(val_ds,std,frac):
-    return np.abs(val_ds)>=frac*std
+    return np.abs(val_ds)>=frac*std
```

### Comparing `domino-composite-0.27/domino/plsr.py` & `domino-composite-0.271/domino/plsr.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.27/domino/prediction.py` & `domino-composite-0.271/domino/prediction.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.27/domino/util.py` & `domino-composite-0.271/domino/util.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.27/domino_composite.egg-info/PKG-INFO` & `domino-composite-0.271/domino_composite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-composite
-Version: 0.27
+Version: 0.271
 Summary: A package for compositing atmospheric datasets
 Home-page: https://github.com/joshdorrington/domino
 Author: Josh Dorrington
 Author-email: joshua.dorrington@kit.edu
 License: bsd-3-clause
 Description-Content-Type: text/markdown
```

### Comparing `domino-composite-0.27/setup.py` & `domino-composite-0.271/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("/data/ox5324/Domino/readme.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='domino-composite',
-    version='0.27',
+    version='0.271',
     author='Josh Dorrington',
     author_email='joshua.dorrington@kit.edu',
     description='A package for compositing atmospheric datasets',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/joshdorrington/domino',
     license='bsd-3-clause',
```

