# Comparing `tmp/hsmm_mvpy-0.1.0b4.tar.gz` & `tmp/hsmm_mvpy-0.1.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsmm_mvpy-0.1.0b4.tar", last modified: Mon Jun 19 15:52:21 2023, max compression
+gzip compressed data, was "hsmm_mvpy-0.1.0b5.tar", last modified: Mon Jun 19 15:59:38 2023, max compression
```

## Comparing `hsmm_mvpy-0.1.0b4.tar` & `hsmm_mvpy-0.1.0b5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:52:21.029332 hsmm_mvpy-0.1.0b4/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.1.0b4/LICENSE.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    25106 2023-06-19 15:52:21.029332 hsmm_mvpy-0.1.0b4/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22740 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b4/README.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      830 2023-06-19 15:51:42.000000 hsmm_mvpy-0.1.0b4/pyproject.toml
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2023-06-19 15:52:21.029332 hsmm_mvpy-0.1.0b4/setup.cfg
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:52:21.029332 hsmm_mvpy-0.1.0b4/src/
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:52:21.029332 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      194 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/__init__.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    57323 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/models.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     5735 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/resample.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    11044 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/simulations.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    41493 2023-06-19 15:51:30.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/utils.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22654 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/visu.py
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:52:21.029332 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy.egg-info/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    25106 2023-06-19 15:52:21.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy.egg-info/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      369 2023-06-19 15:52:21.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy.egg-info/SOURCES.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2023-06-19 15:52:21.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy.egg-info/dependency_links.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       71 2023-06-19 15:52:21.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy.egg-info/requires.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2023-06-19 15:52:21.000000 hsmm_mvpy-0.1.0b4/src/hsmm_mvpy.egg-info/top_level.txt
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:59:38.521545 hsmm_mvpy-0.1.0b5/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.1.0b5/LICENSE.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    25106 2023-06-19 15:59:38.521545 hsmm_mvpy-0.1.0b5/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22740 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b5/README.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      830 2023-06-19 15:59:27.000000 hsmm_mvpy-0.1.0b5/pyproject.toml
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2023-06-19 15:59:38.521545 hsmm_mvpy-0.1.0b5/setup.cfg
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:59:38.521545 hsmm_mvpy-0.1.0b5/src/
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:59:38.521545 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      194 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/__init__.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    57323 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/models.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     5735 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/resample.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    11044 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/simulations.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    41485 2023-06-19 15:59:14.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/utils.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22654 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/visu.py
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 15:59:38.521545 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy.egg-info/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    25106 2023-06-19 15:59:38.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy.egg-info/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      369 2023-06-19 15:59:38.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2023-06-19 15:59:38.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       71 2023-06-19 15:59:38.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy.egg-info/requires.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2023-06-19 15:59:38.000000 hsmm_mvpy-0.1.0b5/src/hsmm_mvpy.egg-info/top_level.txt
```

### Comparing `hsmm_mvpy-0.1.0b4/LICENSE.md` & `hsmm_mvpy-0.1.0b5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b4/PKG-INFO` & `hsmm_mvpy-0.1.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmm_mvpy
-Version: 0.1.0b4
+Version: 0.1.0b5
 Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
 Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
         All rights reserved.
```

### Comparing `hsmm_mvpy-0.1.0b4/README.md` & `hsmm_mvpy-0.1.0b5/README.md`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b4/pyproject.toml` & `hsmm_mvpy-0.1.0b5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "hsmm_mvpy"
-version = "0.1.0-beta4"
+version = "0.1.0-beta5"
 authors = [
   { name="Gabriel Weindel", email="gabriel.weindel@gmail.com" },
   { name="Leendert van Maanen", email="e@mail.com" },
   { name="Jelmer Borst", email="e@mail.com" },
 ]
 description = "Package for fitting Hidden Semi-Markov Models to electro-encephalographic data"
 readme = "README.md"
```

### Comparing `hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/models.py` & `hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/models.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/resample.py` & `hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/resample.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/simulations.py` & `hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/simulations.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/utils.py` & `hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,15 +250,15 @@
             x += 1
         if x > 0:
             print(f'RTs > 0 longer than expected ({x})')
         print(f'{len(cropped_data_epoch)} trials were retained for participant {participant}')
         if verbose:
             print(f'End sampling frequency is {sfreq} Hz')
 
-        epoch_data.append(hmp_data_format(cropped_data_epoch, epochs.info['sfreq'], None, offset_after_resp_samples, epochs=[int(x) for x in epochs_idx], electrodes = epochs.ch_names, metadata = metadata_i))
+        epoch_data.append(hmp_data_format(cropped_data_epoch, epochs.info['sfreq'], None, offset_after_resp_samples, epochs=[int(x) for x in epochs_idx], channels = epochs.ch_names, metadata = metadata_i))
 
         y += 1
     epoch_data = xr.concat(epoch_data, dim = xr.DataArray(subj_idx, dims='participant'),
                           fill_value={'event':'', 'data':np.nan})
     return epoch_data
 
 def _pick_channels(pick_channels,data,stim=True):
@@ -388,16 +388,16 @@
     if len(np.shape(data)) == 4:#means group
         n_subj, n_epochs, n_channels, n_samples = np.shape(data)
     elif len(np.shape(data)) == 3:
         n_epochs, n_channels, n_samples = np.shape(data)
         n_subj = 1
     else:
         raise ValueError(f'Unknown data format with dimensions {np.shape(data)}')
-    if electrodes is None:
-        electrodes = np.arange(n_electrodes)
+    if channels is None:
+        channels = np.arange(n_channels)
     if epochs is None:
          epochs = np.arange(n_epochs)
     if n_subj < 2:
         data = xr.Dataset(
                 {
                     "data": (["epochs", "channels", "samples"],data),
                 },
```

### Comparing `hsmm_mvpy-0.1.0b4/src/hsmm_mvpy/visu.py` & `hsmm_mvpy-0.1.0b5/src/hsmm_mvpy/visu.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b4/src/hsmm_mvpy.egg-info/PKG-INFO` & `hsmm_mvpy-0.1.0b5/src/hsmm_mvpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmm-mvpy
-Version: 0.1.0b4
+Version: 0.1.0b5
 Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
 Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
         All rights reserved.
```

