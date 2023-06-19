# Comparing `tmp/solo_epd_loader-0.2.3.tar.gz` & `tmp/solo_epd_loader-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/gieseler/uni/solo/solo-epd-loader/dist/.tmp-6qydycbe/solo_epd_loader-0.2.3.tar", last modified: Mon Jun  5 09:24:51 2023, max compression
+gzip compressed data, was "/home/gieseler/uni/solo/solo-epd-loader/dist/.tmp-j6ozfh3i/solo_epd_loader-0.2.4.tar", last modified: Mon Jun 19 07:28:16 2023, max compression
```

## Comparing `solo_epd_loader-0.2.3.tar` & `solo_epd_loader-0.2.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 09:24:51.788886 solo_epd_loader-0.2.3/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.3/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.3/MANIFEST.in
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    17529 2023-06-05 09:24:51.788886 solo_epd_loader-0.2.3/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16581 2023-05-23 14:42:04.000000 solo_epd_loader-0.2.3/README.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.2.3/code_of_conduct.md
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 09:24:51.780886 solo_epd_loader-0.2.3/docs/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.3/docs/Makefile
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.3/docs/conf.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.2.3/docs/index.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.3/docs/make.bat
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 09:24:51.780886 solo_epd_loader-0.2.3/examples/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.2.3/examples/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.2.3/examples/ws2021_fig_2d.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.2.3/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.2.3/gh2021_fig_2a.png
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 09:24:51.784886 solo_epd_loader-0.2.3/licenses/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.3/licenses/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.3/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.3/pyproject.toml
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2306 2023-06-05 09:24:51.788886 solo_epd_loader-0.2.3/setup.cfg
--rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.3/setup.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 09:24:51.784886 solo_epd_loader-0.2.3/solo_epd_loader/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    37798 2022-11-16 14:15:40.000000 solo_epd_loader-0.2.3/solo_epd_loader/__init__ (STEP UPDATE).py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    44832 2023-05-25 07:34:00.000000 solo_epd_loader-0.2.3/solo_epd_loader/__init__.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 09:24:51.788886 solo_epd_loader-0.2.3/solo_epd_loader/tests/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.3/solo_epd_loader/tests/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-06-05 09:24:51.000000 solo_epd_loader-0.2.3/solo_epd_loader/version.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 09:24:51.788886 solo_epd_loader-0.2.3/solo_epd_loader.egg-info/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    17529 2023-06-05 09:24:51.000000 solo_epd_loader-0.2.3/solo_epd_loader.egg-info/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      653 2023-06-05 09:24:51.000000 solo_epd_loader-0.2.3/solo_epd_loader.egg-info/SOURCES.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-06-05 09:24:51.000000 solo_epd_loader-0.2.3/solo_epd_loader.egg-info/dependency_links.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.2.3/solo_epd_loader.egg-info/not-zip-safe
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      192 2023-06-05 09:24:51.000000 solo_epd_loader-0.2.3/solo_epd_loader.egg-info/requires.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-06-05 09:24:51.000000 solo_epd_loader-0.2.3/solo_epd_loader.egg-info/top_level.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.2.3/tox.ini
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 07:28:16.060250 solo_epd_loader-0.2.4/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.4/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.4/MANIFEST.in
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    17529 2023-06-19 07:28:16.060250 solo_epd_loader-0.2.4/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16581 2023-05-23 14:42:04.000000 solo_epd_loader-0.2.4/README.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.2.4/code_of_conduct.md
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 07:28:16.052250 solo_epd_loader-0.2.4/docs/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.4/docs/Makefile
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.4/docs/conf.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.2.4/docs/index.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.4/docs/make.bat
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 07:28:16.056250 solo_epd_loader-0.2.4/examples/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.2.4/examples/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.2.4/examples/ws2021_fig_2d.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.2.4/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.2.4/gh2021_fig_2a.png
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 07:28:16.056250 solo_epd_loader-0.2.4/licenses/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.4/licenses/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.4/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.4/pyproject.toml
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2306 2023-06-19 07:28:16.060250 solo_epd_loader-0.2.4/setup.cfg
+-rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.4/setup.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 07:28:16.056250 solo_epd_loader-0.2.4/solo_epd_loader/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    37798 2022-11-16 14:15:40.000000 solo_epd_loader-0.2.4/solo_epd_loader/__init__ (STEP UPDATE).py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    54378 2023-06-19 07:20:29.000000 solo_epd_loader-0.2.4/solo_epd_loader/__init__.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 07:28:16.060250 solo_epd_loader-0.2.4/solo_epd_loader/tests/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.4/solo_epd_loader/tests/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-06-19 07:28:15.000000 solo_epd_loader-0.2.4/solo_epd_loader/version.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 07:28:16.056250 solo_epd_loader-0.2.4/solo_epd_loader.egg-info/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    17529 2023-06-19 07:28:15.000000 solo_epd_loader-0.2.4/solo_epd_loader.egg-info/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      653 2023-06-19 07:28:16.000000 solo_epd_loader-0.2.4/solo_epd_loader.egg-info/SOURCES.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-06-19 07:28:15.000000 solo_epd_loader-0.2.4/solo_epd_loader.egg-info/dependency_links.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.2.4/solo_epd_loader.egg-info/not-zip-safe
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      192 2023-06-19 07:28:15.000000 solo_epd_loader-0.2.4/solo_epd_loader.egg-info/requires.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-06-19 07:28:15.000000 solo_epd_loader-0.2.4/solo_epd_loader.egg-info/top_level.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.2.4/tox.ini
```

### Comparing `solo_epd_loader-0.2.3/LICENSE.rst` & `solo_epd_loader-0.2.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.3/PKG-INFO` & `solo_epd_loader-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo_epd_loader
-Version: 0.2.3
+Version: 0.2.4
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `solo_epd_loader-0.2.3/README.rst` & `solo_epd_loader-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.3/code_of_conduct.md` & `solo_epd_loader-0.2.4/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.3/docs/Makefile` & `solo_epd_loader-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.3/docs/conf.py` & `solo_epd_loader-0.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.3/docs/make.bat` & `solo_epd_loader-0.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.3/examples/gh2021_fig_2.png` & `solo_epd_loader-0.2.4/examples/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.3/examples/ws2021_fig_2d.png` & `solo_epd_loader-0.2.4/examples/ws2021_fig_2d.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.3/gh2021_fig_2.png` & `solo_epd_loader-0.2.4/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.3/gh2021_fig_2a.png` & `solo_epd_loader-0.2.4/gh2021_fig_2a.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.3/licenses/LICENSE.rst` & `solo_epd_loader-0.2.4/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.3/licenses/TEMPLATE_LICENSE.rst` & `solo_epd_loader-0.2.4/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.3/setup.cfg` & `solo_epd_loader-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.3/setup.py` & `solo_epd_loader-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.3/solo_epd_loader/__init__ (STEP UPDATE).py` & `solo_epd_loader-0.2.4/solo_epd_loader/__init__ (STEP UPDATE).py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.3/solo_epd_loader/__init__.py` & `solo_epd_loader-0.2.4/solo_epd_loader/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -972,102 +972,289 @@
     Function that reads in new format (since Oct 2021) STEP CDF 'files'.
     EPOCH_X dependent data is obtained as Pandas Dataframe via sunpy.
     Time-independent meta data is read in from the first cdf file via cdflib.
     """
     # read electron correction factors and meta data via cdflib
     cdf = cdflib.CDF(files[0])
     Electron_Flux_Mult = {'Electron_Avg_Flux_Mult': cdf['Electron_Avg_Flux_Mult']}
-    if not only_averages:
-        for i in range(1, 16):
-            Electron_Flux_Mult['Electron_'+str(i).rjust(2, '0')+'_Flux_Mult'] = cdf['Electron_'+str(i).rjust(2, '0')+'_Flux_Mult']
-        # df_Electron_Flux_Mult = pd.DataFrame(Electron_Flux_Mult)  # get dataframe from dict - not needed atm.
+    # if not only_averages:
+    for i in range(1, 16):
+        Electron_Flux_Mult['Electron_'+str(i).rjust(2, '0')+'_Flux_Mult'] = cdf['Electron_'+str(i).rjust(2, '0')+'_Flux_Mult']
+    # df_Electron_Flux_Mult = pd.DataFrame(Electron_Flux_Mult)  # get dataframe from dict - not needed atm.
 
     meta = {'Bins_Low_Energy': cdf['Bins_Low_Energy']}
     for i in ['Bins_Width', 'Bins_Text', 'Electron_Bins_Low_Energy', 'Electron_Bins_Width', 'Electron_Bins_Text', 'XYZ', 'XYZ_Pixels', 'XYZ_Labels', 'RTN_Labels']:
         meta[i] = cdf[i]
 
+    meta['Electron_Flux_Mult'] = Electron_Flux_Mult
+
     meta['df_rtn_desc'] = cdf.varattsget('RTN')['CATDESC']
     # TODO: add to meta: 'Sector_Bins_Text', 'Sector_Bins_Low_Energy', 'Sector_Bins_Width' -- don't exist in new data product?
 
-    del(cdf)
+    del cdf
 
     # use sunpy to get Pandas DataFrame of EPOCH_X-dependent variables
     # data = TimeSeries(files, concatenate=True)
     # df = data.to_dataframe()
     # del(data)
 
     df = pd.DataFrame()
     for f in files:
         print('Loading', f)
         data = TimeSeries(f, concatenate=True)
-        # print('convert to temporary dataframe (tdf)...')
         tdf = data.to_dataframe()
-        # drop 'Rate's from tdf
         all_columns = False
         if not all_columns:
             # print('dropping Rates from tdf')
             tdf.drop(columns=tdf.filter(like='Rate').columns, inplace=True)
         # drop per-Pixel data from tdf
         if only_averages:
             # print('dropping Pixels from tdf')
             drop_cols = ['Integral_0', 'Integral_1', 'Magnet_0', 'Magnet_1']
             for col in drop_cols:
                 tdf.drop(columns=tdf.filter(like=col).columns, inplace=True)
         # print('merge dataframes...')
         df = pd.concat([df, tdf])
-        del(data, tdf)
+        del (data, tdf)
 
     # move RTN and HCI to different df's because they have different time indices
     # print('move RTN')
     df_rtn = df[['RTN_0', 'RTN_1', 'RTN_2']].dropna(how='all')
     df = df.drop(columns=['RTN_0', 'RTN_1', 'RTN_2']).dropna(how='all')  # remove lines only containing NaN's (all)
     # print('move HCI')
     df_hci = df[['HCI_Lat', 'HCI_Lon', 'HCI_R']].dropna(how='all')
     df = df.drop(columns=['HCI_Lat', 'HCI_Lon', 'HCI_R']).dropna(how='all')  # remove lines only containing NaN's (all)
     meta['df_rtn'] = df_rtn
-    del(df_rtn)
+    del df_rtn
     meta['df_hci'] = df_hci
-    del(df_hci)
+    del df_hci
 
     """
     # what to do with this? not read in by sunpy because of multi-dimensionality. skip for now
     RTN_Pixels              (EPOCH_1, Pixels, dim1) float32 0.8412 ... -0.2708
                             CATDESC: 'Particle flow direction (unit vector) in RTN coordinates for each pixel'
     """
     meta['RTN_Pixels'] = 'CDF var RTN_Pixels (Particle flow direction (unit vector) in RTN coordinates for each pixel) left out as of now because it is multidimensional'
 
-    # calculate electron fluxes from Magnet and Integral Fluxes using correction factors
-    for i in range(len(Electron_Flux_Mult['Electron_Avg_Flux_Mult'])):  # 32 energy channels
-        df[f'Electron_Avg_Flux_{i}'] = Electron_Flux_Mult['Electron_Avg_Flux_Mult'][i] * (df[f'Integral_Avg_Flux_{i}'] - df[f'Magnet_Avg_Flux_{i}'])
-        df[f'Electron_Avg_Uncertainty_{i}'] = \
-            Electron_Flux_Mult['Electron_Avg_Flux_Mult'][i] * np.sqrt(df[f'Integral_Avg_Uncertainty_{i}']**2 + df[f'Magnet_Avg_Uncertainty_{i}']**2)
-        if type(contamination_threshold) == int:
-            clean = (df[f'Integral_Avg_Flux_{i}'] - df[f'Magnet_Avg_Flux_{i}']) > contamination_threshold*df[f'Integral_Avg_Uncertainty_{i}']
-            # mask non-clean data
-            df[f'Electron_Avg_Flux_{i}'] = df[f'Electron_Avg_Flux_{i}'].mask(~clean)
-            df[f'Electron_Avg_Uncertainty_{i}'] = df[f'Electron_Avg_Uncertainty_{i}'].mask(~clean)
-
-        if not only_averages:
-            for pix in [str(n).rjust(2, '0') for n in range(1, 16)]:  # pixel 01 - 15 (00 is background pixel)
-                # print(f'Electron_{pix}_Flux_{i}', f"Electron_Flux_Mult['Electron_{pix}_Flux_Mult'][i]", f'Integral_{pix}_Flux_{i}', f'Magnet_{pix}_Flux_{i}')
-                df[f'Electron_{pix}_Flux_{i}'] = Electron_Flux_Mult[f'Electron_{pix}_Flux_Mult'][i] * (df[f'Integral_{pix}_Flux_{i}'] - df[f'Magnet_{pix}_Flux_{i}'])
-
-                df[f'Electron_{pix}_Uncertainty_{i}'] = \
-                    Electron_Flux_Mult[f'Electron_{pix}_Flux_Mult'][i] * np.sqrt(df[f'Integral_{pix}_Uncertainty_{i}']**2 + df[f'Magnet_{pix}_Uncertainty_{i}']**2)
-
-                if type(contamination_threshold) == int:
-                    clean = (df[f'Integral_{pix}_Flux_{i}'] - df[f'Magnet_{pix}_Flux_{i}']) > contamination_threshold*df[f'Integral_{pix}_Uncertainty_{i}']
-                    # mask non-clean data
-                    df[f'Electron_{pix}_Flux_{i}'] = df[f'Electron_{pix}_Flux_{i}'].mask(~clean)
-                    df[f'Electron_{pix}_Uncertainty_{i}'] = df[f'Electron_{pix}_Uncertainty_{i}'].mask(~clean)
+    """
+    Electron_Flux calculation moved to own function that includes correct resampling. For Now, it should be called independently.
+    df = calc_electrons(df, meta, contamination_threshold=contamination_threshold, only_averages=only_averages, resample=False)
+    """
 
     # TODO: replace all negative values in dataframe with np.nan (applies for electron fluxes that get negative in their calculation)
     # ==> not needed any more after masking above?
     # df = df.mask(df <= 0)
 
     # TODO: multi-index (or rather multi-column) dataframe like previous product?
 
     # df3['QUALITY_FLAG'] = df['QUALITY_FLAG']
     # df3['QUALITY_BITMASK'] = df['QUALITY_BITMASK']
     # df3['SMALL_PIXELS_FLAG'] = df['SMALL_PIXELS_FLAG']
 
     return df, meta
+
+
+def calc_electrons(df, meta, contamination_threshold=2, only_averages=False, resample=False):
+    df = df.copy()
+
+    Electron_Flux_Mult = meta['Electron_Flux_Mult']
+
+    if resample:
+        # for all Integral and Magnet Uncertainties:
+        col_uncertainties = df.filter(like=f'_Uncertainty_').columns.tolist()
+        for delta_flux in col_uncertainties:
+            # overwrite x_Uncertainty with temp. variable x_Uncertainty**2 * dt**2 that is summed in the resampling
+            df[delta_flux] = df[delta_flux]**2 * df['DELTA_EPOCH']**2
+
+        # select columns that should be summed in the resampling process (instead of calculating the mean)
+        col_sum = col_uncertainties.copy()
+        col_sum.insert(0, 'DELTA_EPOCH')  # same as append, but puts it to the start of the list (not really necessary)
+
+        # select columns for which the mean should be calculated in the resampling process.
+        # do this by removing "to be summed" columns from the list of all columns.
+        col_mean = df.columns.drop(col_sum).tolist()
+
+        # build dictionary for agg function that defines how columns should be aggregated
+        dict_agg = {}
+        for c in col_sum:
+            dict_agg[c] = 'sum'
+        for c in col_mean:
+            dict_agg[c] = 'mean'
+
+        # resample with the timestamps at the beginning of the interval (like in original data!)
+        df = df.resample(resample, origin='start', label="left").agg(dict_agg)
+
+        # move timestamp to the center of each interval
+        df.index = df.index + pd.tseries.frequencies.to_offset(pd.Timedelta(resample)/2)
+
+        # calculate correctly resampled Uncertainties:
+        for delta_flux in col_uncertainties:
+            # delta_flux_resampled = np.sqrt( delta_flux_temp / dt^2 )  # delta_flux_temp and dt are resampled sums here!
+            df[delta_flux] = np.sqrt(df[delta_flux] / df['DELTA_EPOCH']**2)
+
+    # create list of electron fluxes to be calculated: only average or average + all individual pixels:
+    if only_averages:
+        pix_list = ['Avg']
+    else:
+        pix_list = ['Avg']+[str(n).rjust(2, '0') for n in range(1, 16)]
+
+    # calculate electron fluxes from Magnet and Integral Fluxes using correction factors
+    for i in range(len(Electron_Flux_Mult['Electron_Avg_Flux_Mult'])):  # 32 energy channels
+        for pix in pix_list:  # Avg, pixel 01 - 15 (00 is background pixel)
+            df[f'Electron_{pix}_Flux_{i}'] = Electron_Flux_Mult[f'Electron_{pix}_Flux_Mult'][i] * (df[f'Integral_{pix}_Flux_{i}'] - df[f'Magnet_{pix}_Flux_{i}'])
+            df[f'Electron_{pix}_Uncertainty_{i}'] = \
+                Electron_Flux_Mult[f'Electron_{pix}_Flux_Mult'][i] * np.sqrt(df[f'Integral_{pix}_Uncertainty_{i}']**2 + df[f'Magnet_{pix}_Uncertainty_{i}']**2)
+
+            if type(contamination_threshold) == int:
+                clean = (df[f'Integral_{pix}_Flux_{i}'] - df[f'Magnet_{pix}_Flux_{i}']) > contamination_threshold*df[f'Integral_{pix}_Uncertainty_{i}']
+                # clean = (df[f'Integral_{pix}_Rate_{i}'] - df[f'Magnet_{pix}_Rate_{i}']) > contamination_threshold*np.sqrt(df[f'Integral_{pix}_Rate_{i}'])/np.sqrt(df['DELTA_EPOCH'])
+                # clean = (df[f'Integral_{pix}_Rate_{i}'] - df[f'Magnet_{pix}_Rate_{i}']) > contamination_threshold*np.sqrt(df[f'Integral_{pix}_Counts_{i}'])/df['DELTA_EPOCH']
+
+                # mask non-clean data
+                df[f'Electron_{pix}_Flux_{i}'] = df[f'Electron_{pix}_Flux_{i}'].mask(~clean)
+                df[f'Electron_{pix}_Uncertainty_{i}'] = df[f'Electron_{pix}_Uncertainty_{i}'].mask(~clean)
+
+    return df
+
+
+def _calc_electrons_rates(df, meta, contamination_threshold=2, only_averages=False, resample=False):
+    """
+    Outdated version of calc_electrons() that used rates to calculate counts, which are then used to calculate resampled uncertainties
+    """
+    df = df.copy()
+
+    Electron_Flux_Mult = meta['Electron_Flux_Mult']
+
+    for i in range(len(Electron_Flux_Mult['Electron_Avg_Flux_Mult'])):  # 32 energy channels
+        # calculate Integral_xx_Counts_i (to be used with contamination threshold later)
+        for pix in [str(n).rjust(2, '0') for n in range(1, 16)]:  # pixel 01 - 15 (00 is background pixel)
+            df[f'Integral_{pix}_Counts_{i}'] = df[f'Integral_{pix}_Rate_{i}'] * df['DELTA_EPOCH']
+            df[f'Magnet_{pix}_Counts_{i}'] = df[f'Magnet_{pix}_Rate_{i}'] * df['DELTA_EPOCH']
+
+        # calculate Integral_Avg_Counts_i from sum of Integral_xx_Counts_i
+        df[f'Integral_Avg_Counts_{i}'] = df.filter(like='Integral_').filter(like=f'_Counts_{i}').sum(axis=1)
+        df[f'Magnet_Avg_Counts_{i}'] = df.filter(like='Magnet_').filter(like=f'_Counts_{i}').sum(axis=1)
+
+        # calculate Integral_Avg_Rate_i from Integral_Avg_Counts_i and integration time
+        df[f'Integral_Avg_Rate_{i}'] = df[f'Integral_Avg_Counts_{i}'] / df['DELTA_EPOCH']
+        df[f'Magnet_Avg_Rate_{i}'] = df[f'Magnet_Avg_Counts_{i}'] / df['DELTA_EPOCH']
+
+    if resample:
+        # select columns that should be summed in the resampling process (instead of calculating the mean)
+        col_sum = df.filter(like=f'_Counts_').columns.tolist()
+        col_sum.insert(0, 'DELTA_EPOCH')  # same as append, but puts it to the start of the list (not really necessary)
+
+        # select columns for which the mean should be calculated in the resampling process.
+        # do this by removing "to be summed" columns from the list of all columns.
+        col_mean = df.columns.drop(col_sum).tolist()
+
+        # build dictionary for agg function that defines how columns should be aggregated
+        dict_agg = {}
+        for c in col_sum:
+            dict_agg[c] = 'sum'
+        for c in col_mean:
+            dict_agg[c] = 'mean'
+
+        # resample with the timestamps at the beginning of the interval (like in original data!)
+        df = df.resample(resample, origin='start', label="left").agg(dict_agg)
+
+        # move timestamp to the center of each interval
+        df.index = df.index + pd.tseries.frequencies.to_offset(pd.Timedelta(resample)/2)
+
+    # create list of electron fluxes to be calculated: only average or average + all individual pixels:
+    if only_averages:
+        pix_list = ['Avg']
+    else:
+        pix_list = ['Avg']+[str(n).rjust(2, '0') for n in range(1, 16)]
+
+    # calculate electron fluxes from Magnet and Integral Fluxes using correction factors
+    for i in range(len(Electron_Flux_Mult['Electron_Avg_Flux_Mult'])):  # 32 energy channels
+        for pix in pix_list:  # Avg, pixel 01 - 15 (00 is background pixel)
+            # print(f'Electron_{pix}_Flux_{i}', f"Electron_Flux_Mult['Electron_{pix}_Flux_Mult'][i]", f'Integral_{pix}_Flux_{i}', f'Magnet_{pix}_Flux_{i}')
+            df[f'Electron_{pix}_Flux_{i}'] = Electron_Flux_Mult[f'Electron_{pix}_Flux_Mult'][i] * (df[f'Integral_{pix}_Flux_{i}'] - df[f'Magnet_{pix}_Flux_{i}'])
+
+            df[f'Electron_{pix}_Uncertainty_{i}'] = \
+                Electron_Flux_Mult[f'Electron_{pix}_Flux_Mult'][i] * np.sqrt(df[f'Integral_{pix}_Uncertainty_{i}']**2 + df[f'Magnet_{pix}_Uncertainty_{i}']**2)
+
+            if type(contamination_threshold) == int:
+                # clean = (df[f'Integral_{pix}_Flux_{i}'] - df[f'Magnet_{pix}_Flux_{i}']) > contamination_threshold*df[f'Integral_{pix}_Uncertainty_{i}']
+                # clean = (df[f'Integral_{pix}_Rate_{i}'] - df[f'Magnet_{pix}_Rate_{i}']) > contamination_threshold*np.sqrt(df[f'Integral_{pix}_Rate_{i}'])/np.sqrt(df['DELTA_EPOCH'])
+                clean = (df[f'Integral_{pix}_Rate_{i}'] - df[f'Magnet_{pix}_Rate_{i}']) > contamination_threshold*np.sqrt(df[f'Integral_{pix}_Counts_{i}'])/df['DELTA_EPOCH']
+
+                # mask non-clean data
+                df[f'Electron_{pix}_Flux_{i}'] = df[f'Electron_{pix}_Flux_{i}'].mask(~clean)
+                df[f'Electron_{pix}_Uncertainty_{i}'] = df[f'Electron_{pix}_Uncertainty_{i}'].mask(~clean)
+
+    # drop columns Rate and Counts from final df
+    all_columns = False
+    if not all_columns:
+        df.drop(columns=df.filter(like='Rate').columns, inplace=True)
+        df.drop(columns=df.filter(like='Counts').columns, inplace=True)
+    return df
+
+
+def _calc_electrons_old(df, meta, contamination_threshold=2, only_averages=False, resample=False):
+    """
+    Outdated original functionality to derive Electron Fluxes. Mask too many data when using contamination threshold because the Integral_Uncertainties are not calculated correctly in the resampling.
+    """
+    df = df.copy()
+
+    # create list of electron fluxes to be calculated: only average or average + all individual pixels:
+    if only_averages:
+        pix_list = ['Avg']
+    else:
+        pix_list = ['Avg']+[str(n).rjust(2, '0') for n in range(1, 16)]
+
+    Electron_Flux_Mult = meta['Electron_Flux_Mult']
+
+    if resample:
+        df = _resample_df_old(df=df, resample=resample)
+
+    # calculate electron fluxes from Magnet and Integral Fluxes using correction factors
+    for i in range(len(Electron_Flux_Mult['Electron_Avg_Flux_Mult'])):  # 32 energy channels
+        for pix in pix_list:  # Avg, pixel 01 - 15 (00 is background pixel)
+            # print(f'Electron_{pix}_Flux_{i}', f"Electron_Flux_Mult['Electron_{pix}_Flux_Mult'][i]", f'Integral_{pix}_Flux_{i}', f'Magnet_{pix}_Flux_{i}')
+            df[f'Electron_{pix}_Flux_{i}'] = Electron_Flux_Mult[f'Electron_{pix}_Flux_Mult'][i] * (df[f'Integral_{pix}_Flux_{i}'] - df[f'Magnet_{pix}_Flux_{i}'])
+
+            df[f'Electron_{pix}_Uncertainty_{i}'] = \
+                Electron_Flux_Mult[f'Electron_{pix}_Flux_Mult'][i] * np.sqrt(df[f'Integral_{pix}_Uncertainty_{i}']**2 + df[f'Magnet_{pix}_Uncertainty_{i}']**2)
+
+            if type(contamination_threshold) == int:
+                clean = (df[f'Integral_{pix}_Flux_{i}'] - df[f'Magnet_{pix}_Flux_{i}']) > contamination_threshold*df[f'Integral_{pix}_Uncertainty_{i}']
+                # mask non-clean data
+                df[f'Electron_{pix}_Flux_{i}'] = df[f'Electron_{pix}_Flux_{i}'].mask(~clean)
+                df[f'Electron_{pix}_Uncertainty_{i}'] = df[f'Electron_{pix}_Uncertainty_{i}'].mask(~clean)
+    return df
+
+
+def _resample_df_old(df, resample, pos_timestamp="center", origin="start"):
+    """
+    Resamples a Pandas Dataframe or Series to a new frequency.
+
+    Parameters:
+    -----------
+    df : pd.DataFrame or pd.Series
+            The dataframe or series to resample
+    resample : str
+            pandas-compatible time string, e.g., '1min', '2H' or '25s'
+    pos_timestamp : str, default 'center'
+            Controls if the timestamp is at the center of the time bin, or at the start of it
+    origin : str, default 'start'
+            Controls if the origin of resampling is at the start of the day (midnight) or at the first
+            entry of the input dataframe/series
+
+    Returns:
+    ----------
+    df : pd.DataFrame or Series, depending on the input
+    """
+    try:
+        df = df.resample(resample, origin=origin, label="left").mean()
+        if pos_timestamp == 'start':
+            df.index = df.index
+        else:
+            df.index = df.index + pd.tseries.frequencies.to_offset(pd.Timedelta(resample)/2)
+        # if pos_timestamp == 'stop' or pos_timestamp == 'end':
+        #     df.index = df.index + pd.tseries.frequencies.to_offset(pd.Timedelta(resample))
+    except ValueError:
+        raise ValueError(f"Your 'resample' option of [{resample}] doesn't seem to be a proper Pandas frequency!")
+
+    return df
```

### Comparing `solo_epd_loader-0.2.3/solo_epd_loader.egg-info/PKG-INFO` & `solo_epd_loader-0.2.4/solo_epd_loader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo-epd-loader
-Version: 0.2.3
+Version: 0.2.4
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `solo_epd_loader-0.2.3/solo_epd_loader.egg-info/SOURCES.txt` & `solo_epd_loader-0.2.4/solo_epd_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.3/tox.ini` & `solo_epd_loader-0.2.4/tox.ini`

 * *Files identical despite different names*

