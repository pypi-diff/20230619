# Comparing `tmp/solo_epd_loader-0.2.5.tar.gz` & `tmp/solo_epd_loader-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solo_epd_loader-0.2.5.tar", last modified: Mon Jun 19 08:26:15 2023, max compression
+gzip compressed data, was "/home/gieseler/uni/solo/solo-epd-loader/dist/.tmp-2t8k6eda/solo_epd_loader-0.2.6.tar", last modified: Mon Jun 19 16:38:58 2023, max compression
```

## Comparing `solo_epd_loader-0.2.5.tar` & `solo_epd_loader-0.2.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 08:26:15.181496 solo_epd_loader-0.2.5/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.5/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.5/MANIFEST.in
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16795 2023-06-19 08:26:15.181496 solo_epd_loader-0.2.5/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15847 2023-06-19 08:20:58.000000 solo_epd_loader-0.2.5/README.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.2.5/code_of_conduct.md
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 08:26:15.173496 solo_epd_loader-0.2.5/docs/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.5/docs/Makefile
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.5/docs/conf.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.2.5/docs/index.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.5/docs/make.bat
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 08:26:15.177496 solo_epd_loader-0.2.5/examples/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.2.5/examples/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.2.5/examples/ws2021_fig_2d.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.2.5/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.2.5/gh2021_fig_2a.png
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 08:26:15.177496 solo_epd_loader-0.2.5/licenses/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.5/licenses/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.5/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.5/pyproject.toml
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2306 2023-06-19 08:26:15.185496 solo_epd_loader-0.2.5/setup.cfg
--rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.5/setup.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 08:26:15.177496 solo_epd_loader-0.2.5/solo_epd_loader/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    54423 2023-06-19 08:10:34.000000 solo_epd_loader-0.2.5/solo_epd_loader/__init__.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 08:26:15.181496 solo_epd_loader-0.2.5/solo_epd_loader/tests/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.5/solo_epd_loader/tests/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-06-19 08:26:15.000000 solo_epd_loader-0.2.5/solo_epd_loader/version.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 08:26:15.181496 solo_epd_loader-0.2.5/solo_epd_loader.egg-info/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16795 2023-06-19 08:26:15.000000 solo_epd_loader-0.2.5/solo_epd_loader.egg-info/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      611 2023-06-19 08:26:15.000000 solo_epd_loader-0.2.5/solo_epd_loader.egg-info/SOURCES.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-06-19 08:26:15.000000 solo_epd_loader-0.2.5/solo_epd_loader.egg-info/dependency_links.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.2.5/solo_epd_loader.egg-info/not-zip-safe
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      192 2023-06-19 08:26:15.000000 solo_epd_loader-0.2.5/solo_epd_loader.egg-info/requires.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-06-19 08:26:15.000000 solo_epd_loader-0.2.5/solo_epd_loader.egg-info/top_level.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.2.5/tox.ini
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 16:38:58.250460 solo_epd_loader-0.2.6/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.6/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.6/MANIFEST.in
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16795 2023-06-19 16:38:58.250460 solo_epd_loader-0.2.6/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15847 2023-06-19 08:20:58.000000 solo_epd_loader-0.2.6/README.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.2.6/code_of_conduct.md
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 16:38:58.242460 solo_epd_loader-0.2.6/docs/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.6/docs/Makefile
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.6/docs/conf.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.2.6/docs/index.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.6/docs/make.bat
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 16:38:58.242460 solo_epd_loader-0.2.6/examples/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.2.6/examples/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.2.6/examples/ws2021_fig_2d.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.2.6/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.2.6/gh2021_fig_2a.png
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 16:38:58.246460 solo_epd_loader-0.2.6/licenses/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.6/licenses/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.6/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.6/pyproject.toml
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2306 2023-06-19 16:38:58.250460 solo_epd_loader-0.2.6/setup.cfg
+-rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.6/setup.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 16:38:58.246460 solo_epd_loader-0.2.6/solo_epd_loader/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    54968 2023-06-19 12:20:19.000000 solo_epd_loader-0.2.6/solo_epd_loader/__init__.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 16:38:58.246460 solo_epd_loader-0.2.6/solo_epd_loader/tests/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.6/solo_epd_loader/tests/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-06-19 16:38:58.000000 solo_epd_loader-0.2.6/solo_epd_loader/version.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 16:38:58.246460 solo_epd_loader-0.2.6/solo_epd_loader.egg-info/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16795 2023-06-19 16:38:58.000000 solo_epd_loader-0.2.6/solo_epd_loader.egg-info/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      611 2023-06-19 16:38:58.000000 solo_epd_loader-0.2.6/solo_epd_loader.egg-info/SOURCES.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-06-19 16:38:58.000000 solo_epd_loader-0.2.6/solo_epd_loader.egg-info/dependency_links.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.2.6/solo_epd_loader.egg-info/not-zip-safe
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      192 2023-06-19 16:38:58.000000 solo_epd_loader-0.2.6/solo_epd_loader.egg-info/requires.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-06-19 16:38:58.000000 solo_epd_loader-0.2.6/solo_epd_loader.egg-info/top_level.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.2.6/tox.ini
```

### Comparing `solo_epd_loader-0.2.5/LICENSE.rst` & `solo_epd_loader-0.2.6/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.5/PKG-INFO` & `solo_epd_loader-0.2.6/solo_epd_loader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: solo_epd_loader
-Version: 0.2.5
+Name: solo-epd-loader
+Version: 0.2.6
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `solo_epd_loader-0.2.5/README.rst` & `solo_epd_loader-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.5/code_of_conduct.md` & `solo_epd_loader-0.2.6/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.5/docs/Makefile` & `solo_epd_loader-0.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.5/docs/conf.py` & `solo_epd_loader-0.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.5/docs/make.bat` & `solo_epd_loader-0.2.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.5/examples/gh2021_fig_2.png` & `solo_epd_loader-0.2.6/examples/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.5/examples/ws2021_fig_2d.png` & `solo_epd_loader-0.2.6/examples/ws2021_fig_2d.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.5/gh2021_fig_2.png` & `solo_epd_loader-0.2.6/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.5/gh2021_fig_2a.png` & `solo_epd_loader-0.2.6/gh2021_fig_2a.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.5/licenses/LICENSE.rst` & `solo_epd_loader-0.2.6/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.5/licenses/TEMPLATE_LICENSE.rst` & `solo_epd_loader-0.2.6/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.5/setup.cfg` & `solo_epd_loader-0.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.5/setup.py` & `solo_epd_loader-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.5/solo_epd_loader/__init__.py` & `solo_epd_loader-0.2.6/solo_epd_loader/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1039,15 +1039,15 @@
     """
     Electron_Flux calculation moved to own function that includes correct resampling. For Now, it should be called independently.
     df = calc_electrons(df, meta, contamination_threshold=contamination_threshold, only_averages=only_averages, resample=False)
     """
 
     # TODO: replace all negative values in dataframe with np.nan (applies for electron fluxes that get negative in their calculation)
     # ==> not needed any more after masking above?
-    # df = df.mask(df <= 0)
+    # df = df.mask(df < 0)
 
     # TODO: multi-index (or rather multi-column) dataframe like previous product?
 
     # df3['QUALITY_FLAG'] = df['QUALITY_FLAG']
     # df3['QUALITY_BITMASK'] = df['QUALITY_BITMASK']
     # df3['SMALL_PIXELS_FLAG'] = df['SMALL_PIXELS_FLAG']
 
@@ -1102,21 +1102,31 @@
     for i in range(len(Electron_Flux_Mult['Electron_Avg_Flux_Mult'])):  # 32 energy channels
         for pix in pix_list:  # Avg, pixel 01 - 15 (00 is background pixel)
             df[f'Electron_{pix}_Flux_{i}'] = Electron_Flux_Mult[f'Electron_{pix}_Flux_Mult'][i] * (df[f'Integral_{pix}_Flux_{i}'] - df[f'Magnet_{pix}_Flux_{i}'])
             df[f'Electron_{pix}_Uncertainty_{i}'] = \
                 Electron_Flux_Mult[f'Electron_{pix}_Flux_Mult'][i] * np.sqrt(df[f'Integral_{pix}_Uncertainty_{i}']**2 + df[f'Magnet_{pix}_Uncertainty_{i}']**2)
 
             if type(contamination_threshold) == int:
-                clean = (df[f'Integral_{pix}_Flux_{i}'] - df[f'Magnet_{pix}_Flux_{i}']) > contamination_threshold*df[f'Integral_{pix}_Uncertainty_{i}']
-                # clean = (df[f'Integral_{pix}_Rate_{i}'] - df[f'Magnet_{pix}_Rate_{i}']) > contamination_threshold*np.sqrt(df[f'Integral_{pix}_Rate_{i}'])/np.sqrt(df['DELTA_EPOCH'])
-                # clean = (df[f'Integral_{pix}_Rate_{i}'] - df[f'Magnet_{pix}_Rate_{i}']) > contamination_threshold*np.sqrt(df[f'Integral_{pix}_Counts_{i}'])/df['DELTA_EPOCH']
-
-                # mask non-clean data
-                df[f'Electron_{pix}_Flux_{i}'] = df[f'Electron_{pix}_Flux_{i}'].mask(~clean)
-                df[f'Electron_{pix}_Uncertainty_{i}'] = df[f'Electron_{pix}_Uncertainty_{i}'].mask(~clean)
+                if contamination_threshold != 0:
+                    clean = (df[f'Integral_{pix}_Flux_{i}'] - df[f'Magnet_{pix}_Flux_{i}']) > contamination_threshold*df[f'Integral_{pix}_Uncertainty_{i}']
+                    # clean = (df[f'Integral_{pix}_Rate_{i}'] - df[f'Magnet_{pix}_Rate_{i}']) > contamination_threshold*np.sqrt(df[f'Integral_{pix}_Rate_{i}'])/np.sqrt(df['DELTA_EPOCH'])
+                    # clean = (df[f'Integral_{pix}_Rate_{i}'] - df[f'Magnet_{pix}_Rate_{i}']) > contamination_threshold*np.sqrt(df[f'Integral_{pix}_Counts_{i}'])/df['DELTA_EPOCH']
+
+                    # mask non-clean data
+                    df[f'Electron_{pix}_Flux_{i}'] = df[f'Electron_{pix}_Flux_{i}'].mask(~clean)
+                    df[f'Electron_{pix}_Uncertainty_{i}'] = df[f'Electron_{pix}_Uncertainty_{i}'].mask(~clean)
+
+    if contamination_threshold == 0:
+        print("contamination_threshold has been set to 0. Ignoring the contamination_threshold (i.e., NOT calculating it for 0)!")
+
+    if type(contamination_threshold) != int:
+        print("conatmination_threshold will only be applied if it is an integer. Otherwise only negative fluxes are removed.")
+
+    # remove negative fluxes (probably not needed for masked data, but for contamination_threshold=None)
+    df = df.mask(df < 0)
 
     return df
 
 
 def _calc_electrons_rates(df, meta, contamination_threshold=2, only_averages=False, resample=False):
     """
     Outdated version of calc_electrons() that used rates to calculate counts, which are then used to calculate resampled uncertainties
```

### Comparing `solo_epd_loader-0.2.5/solo_epd_loader.egg-info/PKG-INFO` & `solo_epd_loader-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: solo-epd-loader
-Version: 0.2.5
+Name: solo_epd_loader
+Version: 0.2.6
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `solo_epd_loader-0.2.5/solo_epd_loader.egg-info/SOURCES.txt` & `solo_epd_loader-0.2.6/solo_epd_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.5/tox.ini` & `solo_epd_loader-0.2.6/tox.ini`

 * *Files identical despite different names*

