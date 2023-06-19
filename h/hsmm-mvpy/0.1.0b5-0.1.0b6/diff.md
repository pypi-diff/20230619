# Comparing `tmp/hsmm_mvpy-0.1.0b5.tar.gz` & `tmp/hsmm_mvpy-0.1.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsmm_mvpy-0.1.0b5.tar", last modified: Mon Jun 19 15:59:38 2023, max compression
+gzip compressed data, was "hsmm_mvpy-0.1.0b6.tar", last modified: Mon Jun 19 16:17:59 2023, max compression
```

## Comparing `hsmm_mvpy-0.1.0b5.tar` & `hsmm_mvpy-0.1.0b6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:59:38.521545 hsmm_mvpy-0.1.0b5/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.1.0b5/LICENSE.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    25106 2023-06-19 15:59:38.521545 hsmm_mvpy-0.1.0b5/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22740 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b5/README.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      830 2023-06-19 15:59:27.000000 hsmm_mvpy-0.1.0b5/pyproject.toml
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2023-06-19 15:59:38.521545 hsmm_mvpy-0.1.0b5/setup.cfg
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:59:38.521545 hsmm_mvpy-0.1.0b5/src/
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:59:38.521545 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      194 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/__init__.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    57323 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/models.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     5735 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/resample.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    11044 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/simulations.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    41485 2023-06-19 15:59:14.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/utils.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22654 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/visu.py
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:59:38.521545 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy.egg-info/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    25106 2023-06-19 15:59:38.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy.egg-info/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      369 2023-06-19 15:59:38.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy.egg-info/SOURCES.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2023-06-19 15:59:38.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy.egg-info/dependency_links.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       71 2023-06-19 15:59:38.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy.egg-info/requires.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2023-06-19 15:59:38.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy.egg-info/top_level.txt
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 16:17:59.581714 hsmm_mvpy-0.1.0b6/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.1.0b6/LICENSE.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    25106 2023-06-19 16:17:59.577715 hsmm_mvpy-0.1.0b6/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22740 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b6/README.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      830 2023-06-19 16:17:20.000000 hsmm_mvpy-0.1.0b6/pyproject.toml
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2023-06-19 16:17:59.581714 hsmm_mvpy-0.1.0b6/setup.cfg
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 16:17:59.577715 hsmm_mvpy-0.1.0b6/src/
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 16:17:59.577715 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      194 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/__init__.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    57323 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/models.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     5735 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/resample.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    11044 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/simulations.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    41525 2023-06-19 16:15:32.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/utils.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22654 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/visu.py
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 16:17:59.577715 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy.egg-info/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    25106 2023-06-19 16:17:59.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy.egg-info/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      369 2023-06-19 16:17:59.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2023-06-19 16:17:59.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       71 2023-06-19 16:17:59.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy.egg-info/requires.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2023-06-19 16:17:59.000000 hsmm_mvpy-0.1.0b6/src/hsmm_mvpy.egg-info/top_level.txt
```

### Comparing `hsmm_mvpy-0.1.0b5/LICENSE.md` & `hsmm_mvpy-0.1.0b6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b5/PKG-INFO` & `hsmm_mvpy-0.1.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmm_mvpy
-Version: 0.1.0b5
+Version: 0.1.0b6
 Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
 Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
         All rights reserved.
```

### Comparing `hsmm_mvpy-0.1.0b5/README.md` & `hsmm_mvpy-0.1.0b6/README.md`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b5/pyproject.toml` & `hsmm_mvpy-0.1.0b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "hsmm_mvpy"
-version = "0.1.0-beta5"
+version = "0.1.0-beta6"
 authors = [
   { name="Gabriel Weindel", email="gabriel.weindel@gmail.com" },
   { name="Leendert van Maanen", email="e@mail.com" },
   { name="Jelmer Borst", email="e@mail.com" },
 ]
 description = "Package for fitting Hidden Semi-Markov Models to electro-encephalographic data"
 readme = "README.md"
```

### Comparing `hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/models.py` & `hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/models.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/resample.py` & `hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/resample.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/simulations.py` & `hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/simulations.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/utils.py` & `hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,14 +418,15 @@
                     "epochs" :epochs,
                     "channels":  channels,
                     "samples": np.arange(n_samples)
                 },
                 attrs={'sfreq':sfreq,'offset':offset}
                 )
     if metadata is not None:
+        metadata = metadata.loc[epochs]
         metadata = metadata.to_xarray()
         metadata = metadata.rename_dims({'index':'epochs'})
         metadata = metadata.rename_vars({'index':'epochs'})
         data = data.merge(metadata)
         data = data.set_coords(list(metadata.data_vars))
     if events is not None:
         data['events'] = xr.DataArray(
```

### Comparing `hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/visu.py` & `hsmm_mvpy-0.1.0b6/src/hsmm_mvpy/visu.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b5/src/hsmm_mvpy.egg-info/PKG-INFO` & `hsmm_mvpy-0.1.0b6/src/hsmm_mvpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmm-mvpy
-Version: 0.1.0b5
+Version: 0.1.0b6
 Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
 Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
         All rights reserved.
```

