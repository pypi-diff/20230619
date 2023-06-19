# Comparing `tmp/domino-composite-0.271.tar.gz` & `tmp/domino-composite-0.272.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domino-composite-0.271.tar", last modified: Mon Jun 19 15:46:24 2023, max compression
+gzip compressed data, was "domino-composite-0.272.tar", last modified: Mon Jun 19 15:48:06 2023, max compression
```

## Comparing `domino-composite-0.271.tar` & `domino-composite-0.272.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-06-19 15:46:24.223301 domino-composite-0.271/
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1213 2023-06-19 15:46:24.223301 domino-composite-0.271/PKG-INFO
-drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-06-19 15:46:24.223301 domino-composite-0.271/domino/
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       62 2022-11-23 14:01:08.000000 domino-composite-0.271/domino/__init__.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1034 2023-06-19 15:18:52.000000 domino-composite-0.271/domino/agg.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     2702 2022-11-23 14:10:17.000000 domino-composite-0.271/domino/categorical_analysis.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)    50731 2023-06-19 15:18:52.000000 domino-composite-0.271/domino/core.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     4248 2023-01-30 10:05:05.000000 domino-composite-0.271/domino/deseasonaliser.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     3846 2023-06-19 15:45:24.000000 domino-composite-0.271/domino/filtering.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     4784 2023-04-03 16:12:11.000000 domino-composite-0.271/domino/plsr.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)    14070 2023-04-12 16:04:19.000000 domino-composite-0.271/domino/prediction.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     5814 2023-06-19 15:18:52.000000 domino-composite-0.271/domino/util.py
-drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-06-19 15:46:24.223301 domino-composite-0.271/domino_composite.egg-info/
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1213 2023-06-19 15:46:24.000000 domino-composite-0.271/domino_composite.egg-info/PKG-INFO
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      382 2023-06-19 15:46:24.000000 domino-composite-0.271/domino_composite.egg-info/SOURCES.txt
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)        1 2023-06-19 15:46:24.000000 domino-composite-0.271/domino_composite.egg-info/dependency_links.txt
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       62 2023-06-19 15:46:24.000000 domino-composite-0.271/domino_composite.egg-info/requires.txt
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)        7 2023-06-19 15:46:24.000000 domino-composite-0.271/domino_composite.egg-info/top_level.txt
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       38 2023-06-19 15:46:24.223301 domino-composite-0.271/setup.cfg
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      728 2023-06-19 15:46:01.000000 domino-composite-0.271/setup.py
+drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-06-19 15:48:06.718695 domino-composite-0.272/
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1213 2023-06-19 15:48:06.718695 domino-composite-0.272/PKG-INFO
+drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-06-19 15:48:06.718695 domino-composite-0.272/domino/
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       62 2022-11-23 14:01:08.000000 domino-composite-0.272/domino/__init__.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1034 2023-06-19 15:18:52.000000 domino-composite-0.272/domino/agg.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     2702 2022-11-23 14:10:17.000000 domino-composite-0.272/domino/categorical_analysis.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)    50731 2023-06-19 15:18:52.000000 domino-composite-0.272/domino/core.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     4248 2023-01-30 10:05:05.000000 domino-composite-0.272/domino/deseasonaliser.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     3851 2023-06-19 15:47:52.000000 domino-composite-0.272/domino/filtering.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     4784 2023-04-03 16:12:11.000000 domino-composite-0.272/domino/plsr.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)    14070 2023-04-12 16:04:19.000000 domino-composite-0.272/domino/prediction.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     5814 2023-06-19 15:18:52.000000 domino-composite-0.272/domino/util.py
+drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-06-19 15:48:06.718695 domino-composite-0.272/domino_composite.egg-info/
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1213 2023-06-19 15:48:06.000000 domino-composite-0.272/domino_composite.egg-info/PKG-INFO
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      382 2023-06-19 15:48:06.000000 domino-composite-0.272/domino_composite.egg-info/SOURCES.txt
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)        1 2023-06-19 15:48:06.000000 domino-composite-0.272/domino_composite.egg-info/dependency_links.txt
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       62 2023-06-19 15:48:06.000000 domino-composite-0.272/domino_composite.egg-info/requires.txt
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)        7 2023-06-19 15:48:06.000000 domino-composite-0.272/domino_composite.egg-info/top_level.txt
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       38 2023-06-19 15:48:06.718695 domino-composite-0.272/setup.cfg
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      728 2023-06-19 15:47:59.000000 domino-composite-0.272/setup.py
```

### Comparing `domino-composite-0.271/PKG-INFO` & `domino-composite-0.272/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-composite
-Version: 0.271
+Version: 0.272
 Summary: A package for compositing atmospheric datasets
 Home-page: https://github.com/joshdorrington/domino
 Author: Josh Dorrington
 Author-email: joshua.dorrington@kit.edu
 License: bsd-3-clause
 Description-Content-Type: text/markdown
```

### Comparing `domino-composite-0.271/domino/agg.py` & `domino-composite-0.272/domino/agg.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.271/domino/categorical_analysis.py` & `domino-composite-0.272/domino/categorical_analysis.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.271/domino/core.py` & `domino-composite-0.272/domino/core.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.271/domino/deseasonaliser.py` & `domino-composite-0.272/domino/deseasonaliser.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.271/domino/filtering.py` & `domino-composite-0.272/domino/filtering.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     else:
         return apply_2d_func_to_da(da,get_large_regions,n,dims=dims)
 
 def ds_large_regions(mask_ds,n,dims,area_based=False):
         ds=mask_ds.copy()
         for var in list(ds.data_vars):
             
-            if (dims is not None) and (not np.all([d in mask_ds.dims for d in dims])):
+            if (dims is not None) and (not np.all([d in mask_ds[var].dims for d in dims])):
                 pass #ignore variables with missing dims
             else:
                 ds[var]=da_large_regions(ds[var],n,dims,area_based=area_based)
         return ds
 
 def convolve_pad(x,N):
     Y=np.array([np.convolve(y,np.ones(np.min([N,len(y)])),mode='same') for y in x])
```

### Comparing `domino-composite-0.271/domino/plsr.py` & `domino-composite-0.272/domino/plsr.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.271/domino/prediction.py` & `domino-composite-0.272/domino/prediction.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.271/domino/util.py` & `domino-composite-0.272/domino/util.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.271/domino_composite.egg-info/PKG-INFO` & `domino-composite-0.272/domino_composite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-composite
-Version: 0.271
+Version: 0.272
 Summary: A package for compositing atmospheric datasets
 Home-page: https://github.com/joshdorrington/domino
 Author: Josh Dorrington
 Author-email: joshua.dorrington@kit.edu
 License: bsd-3-clause
 Description-Content-Type: text/markdown
```

### Comparing `domino-composite-0.271/setup.py` & `domino-composite-0.272/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("/data/ox5324/Domino/readme.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='domino-composite',
-    version='0.271',
+    version='0.272',
     author='Josh Dorrington',
     author_email='joshua.dorrington@kit.edu',
     description='A package for compositing atmospheric datasets',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/joshdorrington/domino',
     license='bsd-3-clause',
```

