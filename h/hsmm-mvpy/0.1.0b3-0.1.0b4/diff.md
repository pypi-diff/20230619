# Comparing `tmp/hsmm_mvpy-0.1.0b3.tar.gz` & `tmp/hsmm_mvpy-0.1.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsmm_mvpy-0.1.0b3.tar", last modified: Mon Jun 19 15:42:44 2023, max compression
+gzip compressed data, was "hsmm_mvpy-0.1.0b4.tar", last modified: Mon Jun 19 15:52:21 2023, max compression
```

## Comparing `hsmm_mvpy-0.1.0b3.tar` & `hsmm_mvpy-0.1.0b4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:42:44.580909 hsmm_mvpy-0.1.0b3/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.1.0b3/LICENSE.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    25106 2023-06-19 15:42:44.580909 hsmm_mvpy-0.1.0b3/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22740 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b3/README.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      830 2023-06-19 15:42:17.000000 hsmm_mvpy-0.1.0b3/pyproject.toml
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2023-06-19 15:42:44.580909 hsmm_mvpy-0.1.0b3/setup.cfg
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:42:44.580909 hsmm_mvpy-0.1.0b3/src/
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:42:44.580909 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      194 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/__init__.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    57323 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/models.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     5735 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/resample.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    11044 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/simulations.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    41499 2023-06-19 15:42:15.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/utils.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22654 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/visu.py
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:42:44.580909 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy.egg-info/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    25106 2023-06-19 15:42:44.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy.egg-info/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      369 2023-06-19 15:42:44.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy.egg-info/SOURCES.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2023-06-19 15:42:44.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy.egg-info/dependency_links.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       71 2023-06-19 15:42:44.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy.egg-info/requires.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2023-06-19 15:42:44.000000 hsmm_mvpy-0.1.0b3/src/hsmm_mvpy.egg-info/top_level.txt
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:52:21.029332 hsmm_mvpy-0.1.0b4/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.1.0b4/LICENSE.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    25106 2023-06-19 15:52:21.029332 hsmm_mvpy-0.1.0b4/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22740 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b4/README.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      830 2023-06-19 15:51:42.000000 hsmm_mvpy-0.1.0b4/pyproject.toml
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2023-06-19 15:52:21.029332 hsmm_mvpy-0.1.0b4/setup.cfg
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:52:21.029332 hsmm_mvpy-0.1.0b4/src/
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:52:21.029332 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      194 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/__init__.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    57323 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/models.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     5735 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/resample.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    11044 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/simulations.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    41493 2023-06-19 15:51:30.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/utils.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22654 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/visu.py
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:52:21.029332 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy.egg-info/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    25106 2023-06-19 15:52:21.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy.egg-info/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      369 2023-06-19 15:52:21.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2023-06-19 15:52:21.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       71 2023-06-19 15:52:21.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy.egg-info/requires.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2023-06-19 15:52:21.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy.egg-info/top_level.txt
```

### Comparing `hsmm_mvpy-0.1.0b3/LICENSE.md` & `hsmm_mvpy-0.1.0b4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b3/PKG-INFO` & `hsmm_mvpy-0.1.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmm_mvpy
-Version: 0.1.0b3
+Version: 0.1.0b4
 Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
 Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
         All rights reserved.
```

### Comparing `hsmm_mvpy-0.1.0b3/README.md` & `hsmm_mvpy-0.1.0b4/README.md`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b3/pyproject.toml` & `hsmm_mvpy-0.1.0b4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "hsmm_mvpy"
-version = "0.1.0-beta3"
+version = "0.1.0-beta4"
 authors = [
   { name="Gabriel Weindel", email="gabriel.weindel@gmail.com" },
   { name="Leendert van Maanen", email="e@mail.com" },
   { name="Jelmer Borst", email="e@mail.com" },
 ]
 description = "Package for fitting Hidden Semi-Markov Models to electro-encephalographic data"
 readme = "README.md"
```

### Comparing `hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/models.py` & `hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/models.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/resample.py` & `hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/resample.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/simulations.py` & `hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/simulations.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/utils.py` & `hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,18 +357,18 @@
     for epoch in np.arange(len(data)):
         #Crops the epochs up to RT
         cropped_data_epoch[j,:,:rts[epoch]+offset_after_resp_samples] = \
         (data[epoch,:,:rts[epoch]+offset_after_resp_samples])
         j += 1
     print(f'Totaling {len(cropped_data_epoch)} valid trials')
 
-    data_xr = hmp_data_format(cropped_data_epoch, sfreq, conditions, offset_after_resp_samples, epochs=epochs, electrodes = electrode_columns)
+    data_xr = hmp_data_format(cropped_data_epoch, sfreq, conditions, offset_after_resp_samples, epochs=epochs, channels = channel_columns)
     return data_xr
 
-def hmp_data_format(data, sfreq, events=None, offset=0, participants=[], epochs=None, electrodes=None, metadata=None):
+def hmp_data_format(data, sfreq, events=None, offset=0, participants=[], epochs=None, channels=None, metadata=None):
 
     '''
     Converting 3D matrix with dimensions (participant) * trials * channels * sample into xarray Dataset
     
     Parameters
     ----------
     data : ndarray
```

### Comparing `hsmm_mvpy-0.1.0b3/src/hsmm_mvpy/visu.py` & `hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/visu.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b3/src/hsmm_mvpy.egg-info/PKG-INFO` & `hsmm_mvpy-0.1.0b4/src/hsmm_mvpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmm-mvpy
-Version: 0.1.0b3
+Version: 0.1.0b4
 Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
 Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
         All rights reserved.
```

