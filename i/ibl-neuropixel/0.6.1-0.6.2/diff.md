# Comparing `tmp/ibl-neuropixel-0.6.1.tar.gz` & `tmp/ibl-neuropixel-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibl-neuropixel-0.6.1.tar", last modified: Tue Jun  6 14:33:25 2023, max compression
+gzip compressed data, was "ibl-neuropixel-0.6.2.tar", last modified: Mon Jun 19 11:04:55 2023, max compression
```

## Comparing `ibl-neuropixel-0.6.1.tar` & `ibl-neuropixel-0.6.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-06 14:33:25.236391 ibl-neuropixel-0.6.1/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1087 2022-04-18 09:47:34.000000 ibl-neuropixel-0.6.1/LICENSE
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       25 2022-04-18 12:17:34.000000 ibl-neuropixel-0.6.1/MANIFEST.in
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1910 2023-06-06 14:33:25.236391 ibl-neuropixel-0.6.1/PKG-INFO
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1369 2022-06-01 09:21:00.000000 ibl-neuropixel-0.6.1/README.md
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       38 2023-06-06 14:33:25.236391 ibl-neuropixel-0.6.1/setup.cfg
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1072 2023-06-06 14:06:55.000000 ibl-neuropixel-0.6.1/setup.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-06 14:33:25.232391 ibl-neuropixel-0.6.1/src/
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-06 14:33:25.236391 ibl-neuropixel-0.6.1/src/ibl_neuropixel.egg-info/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1910 2023-06-06 14:33:25.000000 ibl-neuropixel-0.6.1/src/ibl_neuropixel.egg-info/PKG-INFO
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      590 2023-06-06 14:33:25.000000 ibl-neuropixel-0.6.1/src/ibl_neuropixel.egg-info/SOURCES.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)        1 2023-06-06 14:33:25.000000 ibl-neuropixel-0.6.1/src/ibl_neuropixel.egg-info/dependency_links.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       57 2023-06-06 14:33:25.000000 ibl-neuropixel-0.6.1/src/ibl_neuropixel.egg-info/requires.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       44 2023-06-06 14:33:25.000000 ibl-neuropixel-0.6.1/src/ibl_neuropixel.egg-info/top_level.txt
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-06 14:33:25.236391 ibl-neuropixel-0.6.1/src/neurodsp/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)        0 2022-04-18 12:01:15.000000 ibl-neuropixel-0.6.1/src/neurodsp/__init__.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     6071 2023-03-07 11:56:59.000000 ibl-neuropixel-0.6.1/src/neurodsp/cadzow.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     2371 2022-04-18 10:38:28.000000 ibl-neuropixel-0.6.1/src/neurodsp/cuda_tools.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     2763 2022-04-20 07:48:28.000000 ibl-neuropixel-0.6.1/src/neurodsp/destripe_gpu.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     5838 2022-04-18 09:54:14.000000 ibl-neuropixel-0.6.1/src/neurodsp/filter_gpu.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    10529 2022-04-18 10:39:58.000000 ibl-neuropixel-0.6.1/src/neurodsp/fourier.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     7947 2022-04-18 14:10:58.000000 ibl-neuropixel-0.6.1/src/neurodsp/smooth.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     8976 2022-09-07 17:44:13.000000 ibl-neuropixel-0.6.1/src/neurodsp/utils.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    33322 2023-06-05 17:01:59.000000 ibl-neuropixel-0.6.1/src/neurodsp/voltage.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)    18164 2023-06-06 14:29:50.000000 ibl-neuropixel-0.6.1/src/neurodsp/waveforms.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    35717 2023-06-06 14:06:55.000000 ibl-neuropixel-0.6.1/src/neuropixel.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-06 14:33:25.236391 ibl-neuropixel-0.6.1/src/neurowaveforms/
--rw-r--r--   0 olivier   (1000) olivier   (1000)        0 2023-06-06 14:06:55.000000 ibl-neuropixel-0.6.1/src/neurowaveforms/__init__.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     4692 2023-06-06 14:06:55.000000 ibl-neuropixel-0.6.1/src/neurowaveforms/model.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    33746 2023-05-15 12:25:43.000000 ibl-neuropixel-0.6.1/src/spikeglx.py
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-19 11:04:55.461601 ibl-neuropixel-0.6.2/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1087 2022-04-18 09:47:34.000000 ibl-neuropixel-0.6.2/LICENSE
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       25 2022-04-18 12:17:34.000000 ibl-neuropixel-0.6.2/MANIFEST.in
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1910 2023-06-19 11:04:55.461601 ibl-neuropixel-0.6.2/PKG-INFO
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1369 2022-06-01 09:21:00.000000 ibl-neuropixel-0.6.2/README.md
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       38 2023-06-19 11:04:55.461601 ibl-neuropixel-0.6.2/setup.cfg
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1072 2023-06-19 10:31:03.000000 ibl-neuropixel-0.6.2/setup.py
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-19 11:04:55.457601 ibl-neuropixel-0.6.2/src/
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-19 11:04:55.457601 ibl-neuropixel-0.6.2/src/ibl_neuropixel.egg-info/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1910 2023-06-19 11:04:55.000000 ibl-neuropixel-0.6.2/src/ibl_neuropixel.egg-info/PKG-INFO
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      590 2023-06-19 11:04:55.000000 ibl-neuropixel-0.6.2/src/ibl_neuropixel.egg-info/SOURCES.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)        1 2023-06-19 11:04:55.000000 ibl-neuropixel-0.6.2/src/ibl_neuropixel.egg-info/dependency_links.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       57 2023-06-19 11:04:55.000000 ibl-neuropixel-0.6.2/src/ibl_neuropixel.egg-info/requires.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       44 2023-06-19 11:04:55.000000 ibl-neuropixel-0.6.2/src/ibl_neuropixel.egg-info/top_level.txt
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-19 11:04:55.461601 ibl-neuropixel-0.6.2/src/neurodsp/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)        0 2022-04-18 12:01:15.000000 ibl-neuropixel-0.6.2/src/neurodsp/__init__.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     6071 2023-03-07 11:56:59.000000 ibl-neuropixel-0.6.2/src/neurodsp/cadzow.py
+-rw-r--r--   0 olivier   (1000) olivier   (1000)     2371 2022-04-18 10:38:28.000000 ibl-neuropixel-0.6.2/src/neurodsp/cuda_tools.py
+-rw-r--r--   0 olivier   (1000) olivier   (1000)     2763 2022-04-20 07:48:28.000000 ibl-neuropixel-0.6.2/src/neurodsp/destripe_gpu.py
+-rw-r--r--   0 olivier   (1000) olivier   (1000)     5838 2022-04-18 09:54:14.000000 ibl-neuropixel-0.6.2/src/neurodsp/filter_gpu.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    10529 2022-04-18 10:39:58.000000 ibl-neuropixel-0.6.2/src/neurodsp/fourier.py
+-rw-r--r--   0 olivier   (1000) olivier   (1000)     7947 2022-04-18 14:10:58.000000 ibl-neuropixel-0.6.2/src/neurodsp/smooth.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     8976 2022-09-07 17:44:13.000000 ibl-neuropixel-0.6.2/src/neurodsp/utils.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    33322 2023-06-05 17:01:59.000000 ibl-neuropixel-0.6.2/src/neurodsp/voltage.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    20258 2023-06-14 09:51:06.000000 ibl-neuropixel-0.6.2/src/neurodsp/waveforms.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    35717 2023-06-06 14:06:55.000000 ibl-neuropixel-0.6.2/src/neuropixel.py
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-19 11:04:55.461601 ibl-neuropixel-0.6.2/src/neurowaveforms/
+-rw-r--r--   0 olivier   (1000) olivier   (1000)        0 2023-06-06 14:06:55.000000 ibl-neuropixel-0.6.2/src/neurowaveforms/__init__.py
+-rw-r--r--   0 olivier   (1000) olivier   (1000)     4692 2023-06-06 14:06:55.000000 ibl-neuropixel-0.6.2/src/neurowaveforms/model.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    33750 2023-06-19 10:26:14.000000 ibl-neuropixel-0.6.2/src/spikeglx.py
```

### Comparing `ibl-neuropixel-0.6.1/LICENSE` & `ibl-neuropixel-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.1/PKG-INFO` & `ibl-neuropixel-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibl-neuropixel
-Version: 0.6.1
+Version: 0.6.2
 Summary: Collection of tools for Neuropixel 1.0 and 2.0 probes data
 Home-page: https://github.com/int-brain-lab/ibl-neuropixel
 Author: The International Brain Laboratory
 Project-URL: Bug Tracker, https://github.com/int-brain-lab/ibl-neuropixel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ibl-neuropixel-0.6.1/README.md` & `ibl-neuropixel-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.1/setup.py` & `ibl-neuropixel-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     require = [x.strip() for x in f.readlines() if not x.startswith('git+')]
 
 setuptools.setup(
     name="ibl-neuropixel",
-    version="0.6.1",
+    version="0.6.2",
     author="The International Brain Laboratory",
     description="Collection of tools for Neuropixel 1.0 and 2.0 probes data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/int-brain-lab/ibl-neuropixel",
     project_urls={
         "Bug Tracker": "https://github.com/int-brain-lab/ibl-neuropixel/issues",
```

### Comparing `ibl-neuropixel-0.6.1/src/ibl_neuropixel.egg-info/PKG-INFO` & `ibl-neuropixel-0.6.2/src/ibl_neuropixel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibl-neuropixel
-Version: 0.6.1
+Version: 0.6.2
 Summary: Collection of tools for Neuropixel 1.0 and 2.0 probes data
 Home-page: https://github.com/int-brain-lab/ibl-neuropixel
 Author: The International Brain Laboratory
 Project-URL: Bug Tracker, https://github.com/int-brain-lab/ibl-neuropixel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ibl-neuropixel-0.6.1/src/ibl_neuropixel.egg-info/SOURCES.txt` & `ibl-neuropixel-0.6.2/src/ibl_neuropixel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.1/src/neurodsp/cadzow.py` & `ibl-neuropixel-0.6.2/src/neurodsp/cadzow.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.1/src/neurodsp/cuda_tools.py` & `ibl-neuropixel-0.6.2/src/neurodsp/cuda_tools.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.1/src/neurodsp/destripe_gpu.py` & `ibl-neuropixel-0.6.2/src/neurodsp/destripe_gpu.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.1/src/neurodsp/filter_gpu.py` & `ibl-neuropixel-0.6.2/src/neurodsp/filter_gpu.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.1/src/neurodsp/fourier.py` & `ibl-neuropixel-0.6.2/src/neurodsp/fourier.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.1/src/neurodsp/smooth.py` & `ibl-neuropixel-0.6.2/src/neurodsp/smooth.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.1/src/neurodsp/utils.py` & `ibl-neuropixel-0.6.2/src/neurodsp/utils.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.1/src/neurodsp/voltage.py` & `ibl-neuropixel-0.6.2/src/neurodsp/voltage.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.1/src/neurodsp/waveforms.py` & `ibl-neuropixel-0.6.2/src/neurodsp/waveforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,33 +115,38 @@
     df = pd.DataFrame()
     df['peak_trace_idx'] = indx_trace
     df['peak_time_idx'] = indx_peak
     df['peak_val'] = val_peak
     return df
 
 
-def find_tip_trough(arr_peak, df):
-    '''
-    :param arr_in: inverted
-    :param df:
-    :return:
-    '''
-    # 2. Find trough and tip (at peak waveform)
+def find_trough(arr_peak, df):
+    # Find tip (at peak waveform)
+
     # Create masks pre/post
     arr_pre, arr_post = arr_pre_post(arr_peak, df['peak_time_idx'].to_numpy())
 
     # Find trough
     # indx_trough = np.nanargmin(arr_post * np.sign(val_peak)[:, np.newaxis], axis=1)
     indx_trough = np.nanargmax(arr_post, axis=1)
     val_trough = arr_peak[np.arange(0, arr_peak.shape[0], 1), indx_trough] * df['invert_sign_peak'].to_numpy()
-    del arr_post
-    # TODO spin function above into a function
-    #  if ratio or diff peak/trough smaller than x AND time diff is smaller than xx :
-    #  Assign trough as peak
-    #  Call this function again to compute trough with new peak assigned
+
+    # Put values into df
+    df['trough_time_idx'] = indx_trough
+    df['trough_val'] = val_trough
+
+    return df
+
+
+def find_tip(arr_peak, df):
+    # Find tip (at peak waveform)
+
+    # Create masks pre/post
+    arr_pre, arr_post = arr_pre_post(arr_peak, df['peak_time_idx'].to_numpy())
+
     # Find tip
     '''
     # 02-06-2023 ; Decided not to use the inflection point but rather maximum
     # Leaving code for now commented as legacy example
 
     # Inflection point
     y_dif1 = np.diff(arr_pre, axis=1)
@@ -152,26 +157,68 @@
     indx_tip = np.argmax(np.cumsum(arr_cs, axis=1), axis=1) + 1
     val_tip = arr_peak[np.arange(0, arr_peak.shape[0], 1), indx_tip] * df['invert_sign_peak'].to_numpy()
     del arr_cs
     '''
     # Maximum
     indx_tip = np.nanargmax(arr_pre, axis=1)
     val_tip = arr_peak[np.arange(0, arr_peak.shape[0], 1), indx_tip] * df['invert_sign_peak'].to_numpy()
-    del arr_pre
 
     # Put values into df
-    df['trough_time_idx'] = indx_trough
-    df['trough_val'] = val_trough
-
     df['tip_time_idx'] = indx_tip
     df['tip_val'] = val_tip
 
     return df
 
 
+def find_tip_trough(arr_peak, arr_peak_real, df):
+    '''
+    :param arr_in: inverted
+    :param df:
+    :return:
+    '''
+    # 2. Find trough and tip (at peak waveform)
+
+    # Find trough
+    df = find_trough(arr_peak, df)
+    df = peak_to_trough_ratio(df)
+    # If ratio of peak/trough is near 1, and peak is positive :
+    # Assign trough as peak on same waveform channel
+    # Call the function again to compute trough etc. with new peak assigned
+
+    # Find df rows to be changed
+    df_index = df.index[(df['peak_val'] > 0) & (df['peak_to_trough_ratio'] <= 1.5)]
+    df_rows = df.iloc[df_index]
+    if len(df_index) > 0:
+        # New peak - Swap peak for trough values
+        df_rows = df_rows.drop(['peak_val', 'peak_time_idx'], axis=1)
+        df_rows['peak_val'] = df_rows['trough_val']
+        df_rows['peak_time_idx'] = df_rows['trough_time_idx']
+
+        # df_trials.loc[iss, f] = predicted[f].values
+
+        # Drop trough columns
+        df_rows = df_rows.drop(['trough_time_idx', 'trough_val'], axis=1)
+        # Create mini arr_peak for those rows uniquely (take the real waveforms value in, not inverted ones)
+        arr_peak_rows = arr_peak_real[df_index, :]
+        # Place into "inverted" array peak for return
+        arr_peak[df_index, :] = arr_peak_rows
+        # Get new sign for the peak
+        arr_peak_rows, df_rows = invert_peak_waveform(arr_peak_rows, df_rows)
+        # New trough
+        df_rows = find_trough(arr_peak_rows, df_rows)
+        # New peak-trough ratio
+        df_rows = peak_to_trough_ratio(df_rows)
+        # Assign back into the dataframe
+        df.loc[df_index] = df_rows
+    # Find tip
+    df = find_tip(arr_peak, df)
+
+    return df, arr_peak
+
+
 def plot_peaktiptrough(df, arr, ax, nth_wav=0, plot_grey=True):
     if plot_grey:
         ax.plot(arr[nth_wav], c='gray', alpha=0.5)
     # Peak channel
     ax.plot(arr[nth_wav][:, int(df.iloc[nth_wav].peak_trace_idx)], marker=".", c='blue')
     # Peak point
     ax.plot(df.iloc[nth_wav].peak_time_idx, df.iloc[nth_wav].peak_val, 'r*')
@@ -235,25 +282,37 @@
     :param fs:  sampling rate (Hz)
     :return: dataframe wirth added column
     '''
     df['half_peak_duration'] = (df['half_peak_post_time_idx'] - df['half_peak_pre_time_idx']) / fs
     return df
 
 
-def peak_to_trough(df, fs=30000):
+def peak_to_trough_duration(df, fs=30000):
     '''
-    Compute the duration (second) and ratio of the peak-to-trough
+    Compute the duration (second) of the peak-to-trough
     :param df: dataframe of waveforms features
     :param fs: sampling rate (Hz)
-    :return:
+    :return: df
     '''
     # Duration
     df['peak_to_trough_duration'] = (df['trough_time_idx'] - df['peak_time_idx']) / fs
+    return df
+
+
+def peak_to_trough_ratio(df):
+    '''
+    Compute the ratio of the peak-to-trough
+    :param df: dataframe of waveforms features
+    :param fs: sampling rate (Hz)
+    :return:
+    '''
     # Ratio
-    df['peak_to_trough_ratio'] = np.log(np.abs(df['peak_val'] / df['trough_val']))
+    df['peak_to_trough_ratio'] = np.abs(df['peak_val'] / df['trough_val'])  # Division by 0 returns NaN
+    # Ratio log-scale
+    df['peak_to_trough_ratio_log'] = np.log(df['peak_to_trough_ratio'])
     return df
 
 
 def polarisation_slopes(df, fs=30000):
     '''
     Computes the depolarisation and repolarisation slopes as the difference between tip-peak
     and peak-trough respectively.
@@ -414,25 +473,28 @@
     :recovery_duration_ms: in ms, the duration from the trough to the recovery point
     :param return_peak_channel: if True, return the peak channel traces
     :return: dataframe of spikes with all features,
     Returns:
     """
     df = find_peak(arr_in)
     # Per waveform, keep only trace that contains the peak
-    arr_peak = get_array_peak(arr_in, df)
+    arr_peak_real = get_array_peak(arr_in, df)
     # Invert positive spikes
-    arr_peak, df = invert_peak_waveform(arr_peak, df)
-    # Tip-trough
-    df = find_tip_trough(arr_peak, df)
+    arr_peak, df = invert_peak_waveform(arr_peak_real.copy(), df)  # Copy otherwise overwrite the variable in memory
+    # Tip-trough (this also computes the peak_to_trough_ratio)
+    df, arr_peak = find_tip_trough(arr_peak, arr_peak_real, df)
+    # Peak to trough duration
+    df = peak_to_trough_duration(df, fs=30000)
     # Half peak points
     df = half_peak_point(arr_peak, df)
     # Half peak duration
     df = half_peak_duration(df, fs=fs)
     # Recovery point
     df = recovery_point(arr_peak, df, idx_from_trough=int(round(recovery_duration_ms * fs / 1000)))
     # Slopes
     df = polarisation_slopes(df, fs=fs)
     df = recovery_slope(df, fs=fs)
+
     if return_peak_channel:
-        return df, arr_peak
+        return df, arr_peak_real
     else:
         return df
```

### Comparing `ibl-neuropixel-0.6.1/src/neuropixel.py` & `ibl-neuropixel-0.6.2/src/neuropixel.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.1/src/neurowaveforms/model.py` & `ibl-neuropixel-0.6.2/src/neurowaveforms/model.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.1/src/spikeglx.py` & `ibl-neuropixel-0.6.2/src/spikeglx.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,33 +35,33 @@
         s2mv = 2.34375e-06 (NP1 ap banc) : default value used
         s2mv = 4.6875e-06 (NP1 lfp band)
 
     Note: To release system resources the close method must be called
     """
 
     def __init__(self, sglx_file, open=True, nc=None, ns=None, fs=None, dtype='int16', s2v=None,
-                 nsync=None, ignore_warnings=False):
+                 nsync=None, ignore_warnings=False, meta_file=None):
         """
         An interface for reading data from a SpikeGLX file
         :param sglx_file: Path to a SpikeGLX file (compressed or otherwise), or to a meta-data file
         :param open: when True the file is opened
         """
         self.ignore_warnings = ignore_warnings
         sglx_file = Path(sglx_file)
-        file_meta_data = sglx_file.with_suffix('.meta')
-        if file_meta_data == sglx_file:
+        meta_file = meta_file or sglx_file.with_suffix('.meta')
+        if meta_file == sglx_file:
             # if a meta-data file is provided, try to get the binary file
             self.file_bin = sglx_file.with_suffix('.cbin') if sglx_file.with_suffix('.cbin').exists() else None
             self.file_bin = sglx_file.with_suffix('.bin') if sglx_file.with_suffix('.bin').exists() else None
         else:
             self.file_bin = sglx_file
         self.nbytes = self.file_bin.stat().st_size if self.file_bin else None
         self.dtype = np.dtype(dtype)
 
-        if not file_meta_data.exists():
+        if not meta_file.exists():
             # if no meta-data file is provided, try to get critical info from the binary file
             # by seeing if filesize checks out with neuropixel 384 channels
             if self.file_bin.stat().st_size / 384 % 2 == 0:
                 nc = nc or 384
                 ns = ns or self.file_bin.stat().st_size / 2 / 384
                 fs = fs or 30000
             elif self.file_bin.stat().st_size / 385 % 2 == 0:
@@ -81,16 +81,16 @@
             if s2v is None:
                 s2v = neuropixel.S2V_AP if self.dtype == np.dtype('int16') else 1.0
             self.channel_conversion_sample2v = {'samples': np.ones(nc) * s2v}
             if self._nsync > 0:
                 self.channel_conversion_sample2v['samples'][-nsync:] = 1
         else:
             # normal case we continue reading and interpreting the metadata file
-            self.file_meta_data = file_meta_data
-            self.meta = read_meta_data(file_meta_data)
+            self.file_meta_data = meta_file
+            self.meta = read_meta_data(meta_file)
             self.channel_conversion_sample2v = _conversion_sample2v_from_meta(self.meta)
             self._raw = None
         if open and self.file_bin:
             self.open()
 
     def open(self):
         # if we are not looking at a compressed file, use a memmap, otherwise instantiate mtscomp
```

