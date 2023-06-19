# Comparing `tmp/lm_datahandler-0.1.3.tar.gz` & `tmp/lm_datahandler-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lm_datahandler-0.1.3.tar", last modified: Wed Jun 14 11:40:27 2023, max compression
+gzip compressed data, was "lm_datahandler-0.1.4.tar", last modified: Mon Jun 19 08:11:56 2023, max compression
```

## Comparing `lm_datahandler-0.1.3.tar` & `lm_datahandler-0.1.4.tar`

### file list

```diff
@@ -1,43 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 11:40:27.646879 lm_datahandler-0.1.3/
--rw-rw-rw-   0        0        0     1104 2023-06-14 03:54:04.000000 lm_datahandler-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       45 2023-06-14 10:58:27.000000 lm_datahandler-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      325 2023-06-14 11:40:27.646879 lm_datahandler-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 11:40:27.600663 lm_datahandler-0.1.3/lm_datahandler/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:11:31.000000 lm_datahandler-0.1.3/lm_datahandler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:40:27.615012 lm_datahandler-0.1.3/lm_datahandler/data_load/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:11:51.000000 lm_datahandler-0.1.3/lm_datahandler/data_load/__init__.py
--rw-rw-rw-   0        0        0     1674 2023-06-13 02:30:00.000000 lm_datahandler-0.1.3/lm_datahandler/data_load/data_loader.py
--rw-rw-rw-   0        0        0    10521 2023-06-13 02:44:38.000000 lm_datahandler-0.1.3/lm_datahandler/data_load/loaders.py
--rw-rw-rw-   0        0        0    24343 2023-06-14 03:57:25.000000 lm_datahandler-0.1.3/lm_datahandler/datahandler.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:40:27.618744 lm_datahandler-0.1.3/lm_datahandler/functions/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:02.000000 lm_datahandler-0.1.3/lm_datahandler/functions/__init__.py
--rw-rw-rw-   0        0        0    31179 2023-06-14 03:24:58.000000 lm_datahandler-0.1.3/lm_datahandler/functions/biomarker.py
--rw-rw-rw-   0        0        0    14569 2023-06-02 03:05:39.000000 lm_datahandler-0.1.3/lm_datahandler/functions/feature_extract.py
--rw-rw-rw-   0        0        0        0 2023-05-31 12:12:04.000000 lm_datahandler-0.1.3/lm_datahandler/functions/os_detect.py
--rw-rw-rw-   0        0        0     1556 2023-06-14 11:39:19.000000 lm_datahandler-0.1.3/lm_datahandler/functions/sleep_staging.py
--rw-rw-rw-   0        0        0     3240 2023-06-14 03:25:28.000000 lm_datahandler-0.1.3/lm_datahandler/functions/sleep_variable_compute.py
--rw-rw-rw-   0        0        0        0 2023-05-31 12:11:57.000000 lm_datahandler-0.1.3/lm_datahandler/functions/spindle_detect.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:40:27.618744 lm_datahandler-0.1.3/lm_datahandler/models/
--rw-rw-rw-   0        0        0   376172 2023-05-30 01:59:36.000000 lm_datahandler-0.1.3/lm_datahandler/models/wholenight_sleep_staging.txt
-drwxrwxrwx   0        0        0        0 2023-06-14 11:40:27.620267 lm_datahandler-0.1.3/lm_datahandler/plots/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:16.000000 lm_datahandler-0.1.3/lm_datahandler/plots/__init__.py
--rw-rw-rw-   0        0        0      625 2023-06-07 08:43:30.000000 lm_datahandler-0.1.3/lm_datahandler/plots/biomarker_plot.py
--rw-rw-rw-   0        0        0     5653 2023-06-14 05:56:16.000000 lm_datahandler-0.1.3/lm_datahandler/plots/sleep_staging_plot.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:40:27.643996 lm_datahandler-0.1.3/lm_datahandler/postprocess/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:28.000000 lm_datahandler-0.1.3/lm_datahandler/postprocess/__init__.py
--rw-rw-rw-   0        0        0     2358 2023-06-02 05:40:05.000000 lm_datahandler-0.1.3/lm_datahandler/postprocess/label_smooth.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:40:27.645436 lm_datahandler-0.1.3/lm_datahandler/preprocess/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:46.000000 lm_datahandler-0.1.3/lm_datahandler/preprocess/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-31 10:45:45.000000 lm_datahandler-0.1.3/lm_datahandler/preprocess/filter.py
--rw-rw-rw-   0        0        0        0 2023-05-31 10:48:56.000000 lm_datahandler-0.1.3/lm_datahandler/preprocess/tailor.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:40:27.646432 lm_datahandler-0.1.3/lm_datahandler/utils/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:57.000000 lm_datahandler-0.1.3/lm_datahandler/utils/__init__.py
--rw-rw-rw-   0        0        0     1734 2023-04-20 07:01:30.000000 lm_datahandler-0.1.3/lm_datahandler/utils/numba_func.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:40:27.614244 lm_datahandler-0.1.3/lm_datahandler.egg-info/
--rw-rw-rw-   0        0        0      325 2023-06-14 11:40:27.000000 lm_datahandler-0.1.3/lm_datahandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1106 2023-06-14 11:40:27.000000 lm_datahandler-0.1.3/lm_datahandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 11:40:27.000000 lm_datahandler-0.1.3/lm_datahandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      179 2023-06-14 11:40:27.000000 lm_datahandler-0.1.3/lm_datahandler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-14 11:40:27.000000 lm_datahandler-0.1.3/lm_datahandler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 11:40:27.646879 lm_datahandler-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      987 2023-06-14 11:40:22.000000 lm_datahandler-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:11:56.552041 lm_datahandler-0.1.4/
+-rw-rw-rw-   0        0        0     1104 2023-06-14 03:54:04.000000 lm_datahandler-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0       45 2023-06-14 10:58:27.000000 lm_datahandler-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      325 2023-06-19 08:11:56.551551 lm_datahandler-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 08:11:56.471544 lm_datahandler-0.1.4/lm_datahandler/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:11:31.000000 lm_datahandler-0.1.4/lm_datahandler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:11:56.488884 lm_datahandler-0.1.4/lm_datahandler/data_load/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:11:51.000000 lm_datahandler-0.1.4/lm_datahandler/data_load/__init__.py
+-rw-rw-rw-   0        0        0     2024 2023-06-15 10:20:25.000000 lm_datahandler-0.1.4/lm_datahandler/data_load/data_loader.py
+-rw-rw-rw-   0        0        0    12664 2023-06-15 09:43:32.000000 lm_datahandler-0.1.4/lm_datahandler/data_load/loaders.py
+-rw-rw-rw-   0        0        0    24102 2023-06-19 08:08:17.000000 lm_datahandler-0.1.4/lm_datahandler/datahandler.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:11:56.541721 lm_datahandler-0.1.4/lm_datahandler/functions/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:02.000000 lm_datahandler-0.1.4/lm_datahandler/functions/__init__.py
+-rw-rw-rw-   0        0        0    31179 2023-06-14 03:24:58.000000 lm_datahandler-0.1.4/lm_datahandler/functions/biomarker.py
+-rw-rw-rw-   0        0        0    29337 2023-06-16 07:10:08.000000 lm_datahandler-0.1.4/lm_datahandler/functions/feature_extract.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:12:04.000000 lm_datahandler-0.1.4/lm_datahandler/functions/os_detect.py
+-rw-rw-rw-   0        0        0      613 2023-06-16 08:37:12.000000 lm_datahandler-0.1.4/lm_datahandler/functions/posture_analyse.py
+-rw-rw-rw-   0        0        0     1510 2023-06-15 09:46:15.000000 lm_datahandler-0.1.4/lm_datahandler/functions/sleep_staging.py
+-rw-rw-rw-   0        0        0     3240 2023-06-14 03:25:28.000000 lm_datahandler-0.1.4/lm_datahandler/functions/sleep_variable_compute.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:11:57.000000 lm_datahandler-0.1.4/lm_datahandler/functions/spindle_detect.py
+-rw-rw-rw-   0        0        0      832 2023-06-16 07:21:59.000000 lm_datahandler-0.1.4/lm_datahandler/functions/wear_detect.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:11:56.542749 lm_datahandler-0.1.4/lm_datahandler/models/
+-rw-rw-rw-   0        0        0    59109 2023-03-31 05:25:34.000000 lm_datahandler-0.1.4/lm_datahandler/models/wear_detection_1s.txt
+-rw-rw-rw-   0        0        0   376172 2023-05-30 01:59:36.000000 lm_datahandler-0.1.4/lm_datahandler/models/wholenight_sleep_staging.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 08:11:56.548032 lm_datahandler-0.1.4/lm_datahandler/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:16.000000 lm_datahandler-0.1.4/lm_datahandler/plots/__init__.py
+-rw-rw-rw-   0        0        0      625 2023-06-07 08:43:30.000000 lm_datahandler-0.1.4/lm_datahandler/plots/biomarker_plot.py
+-rw-rw-rw-   0        0        0     6390 2023-06-16 05:16:37.000000 lm_datahandler-0.1.4/lm_datahandler/plots/sleep_staging_plot.py
+-rw-rw-rw-   0        0        0     3553 2023-06-19 08:09:09.000000 lm_datahandler-0.1.4/lm_datahandler/plots/stim_plot.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:11:56.548231 lm_datahandler-0.1.4/lm_datahandler/postprocess/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:28.000000 lm_datahandler-0.1.4/lm_datahandler/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     2358 2023-06-02 05:40:05.000000 lm_datahandler-0.1.4/lm_datahandler/postprocess/label_smooth.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:11:56.550400 lm_datahandler-0.1.4/lm_datahandler/preprocess/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:46.000000 lm_datahandler-0.1.4/lm_datahandler/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      865 2023-06-19 08:09:38.000000 lm_datahandler-0.1.4/lm_datahandler/preprocess/filter.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 10:48:56.000000 lm_datahandler-0.1.4/lm_datahandler/preprocess/tailor.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:11:56.550935 lm_datahandler-0.1.4/lm_datahandler/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:57.000000 lm_datahandler-0.1.4/lm_datahandler/utils/__init__.py
+-rw-rw-rw-   0        0        0     1734 2023-04-20 07:01:30.000000 lm_datahandler-0.1.4/lm_datahandler/utils/numba_func.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:11:56.487010 lm_datahandler-0.1.4/lm_datahandler.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-06-19 08:11:56.000000 lm_datahandler-0.1.4/lm_datahandler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1268 2023-06-19 08:11:56.000000 lm_datahandler-0.1.4/lm_datahandler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 08:11:56.000000 lm_datahandler-0.1.4/lm_datahandler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      179 2023-06-19 08:11:56.000000 lm_datahandler-0.1.4/lm_datahandler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-19 08:11:56.000000 lm_datahandler-0.1.4/lm_datahandler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 08:11:56.552041 lm_datahandler-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      987 2023-06-19 08:09:38.000000 lm_datahandler-0.1.4/setup.py
```

### Comparing `lm_datahandler-0.1.3/LICENSE` & `lm_datahandler-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.3/lm_datahandler/data_load/data_loader.py` & `lm_datahandler-0.1.4/lm_datahandler/data_load/data_loader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 import numpy as np
-from .loaders import EEGLoader, ACCLoader, BLELoader
+from .loaders import EEGLoader, ACCLoader, BLELoader, STILoader
 
-def load_data(eeg_path, acc_path, ble_path, sf_send):
-    raw_acc = raw_eeg = package_loss_rate = total_time = disconnections = disconnect_rate = None
+
+def load_data(eeg_path, acc_path, sti_path, ble_path, sf_send, logger):
+    raw_acc = raw_eeg = raw_sti = package_loss_rate = total_time = disconnections = disconnect_rate = None
     if acc_path is not None:
+        logger.info("ACC loading start...")
         acc_loader = ACCLoader(sf_send)
-        raw_acc, acc_loss_rate, total_time = acc_loader.load_data(acc_path)
+        raw_acc, acc, acc_loss_rate, total_time = acc_loader.load_data(acc_path)
+        logger.info("ACC loading finished.")
     if eeg_path is not None:
+        logger.info("EEG loading start...")
         eeg_loader = EEGLoader(sf_send)
-        raw_eeg, eeg_loss_rate, total_time = eeg_loader.load_data(eeg_path)
+        raw_eeg, eeg, eeg_loss_rate, total_time = eeg_loader.load_data(eeg_path)
+        logger.info("EEG loading finished.")
+    if sti_path is not None:
+        sti_loader = STILoader()
+        raw_sti = sti_loader.load_data(sti_path)
 
-    if raw_eeg is not None and raw_acc is not None:
-        assert raw_eeg.shape[0] != raw_acc.shape[0]
+    if eeg is not None and acc is not None:
+        assert eeg.shape[0] != acc.shape[0]
     if eeg_loss_rate is not None and acc_loss_rate is not None:
         assert eeg_loss_rate == acc_loss_rate
         package_loss_rate = eeg_loss_rate
 
     if ble_path is not None:
         ble_loader = BLELoader()
         disconnections = ble_loader.load_data(ble_path)
@@ -30,8 +38,8 @@
 
             # seg_gap = np.around(time_gap / 15).astype(np.int32)
             # disconnection_st = disconnections[:, 0]
             # disconnection_index = np.around((disconnection_st - st_time) / 15).astype(np.int32)
             #
             # disconnection_count = len(time_gap)
 
-    return raw_eeg, raw_acc, disconnections, total_time, package_loss_rate, disconnect_rate
+    return raw_eeg, eeg, raw_acc, acc, raw_sti, disconnections, total_time, package_loss_rate, disconnect_rate
```

### Comparing `lm_datahandler-0.1.3/lm_datahandler/data_load/loaders.py` & `lm_datahandler-0.1.4/lm_datahandler/data_load/loaders.py`

 * *Files 18% similar despite different names*

```diff
@@ -87,14 +87,18 @@
     #         et_datetime = et_datetime + timedelta(days=ET_D_more)
     #     total_time = (et_datetime - st_datetime).total_seconds()
 
 
 class EEGLoader(BaseLoader):
     def __init__(self, sf_send=10):
         super().__init__()
+        self.data_total = None
+        self.package_loss = None
+        self.time_length = None
+        self.raw_data = None
         if sf_send == 10:
             self.package_length = 208
             self.package_std_time_interval = [100 - 20, 100, 100 + 20]
         elif sf_send == 50:
             self.package_length = 48
             self.package_std_time_interval = [20-10, 20, 20+10]
 
@@ -105,46 +109,53 @@
         #     pass
         # else:
         #     self.package_std_time_interval = [70 - 20, 70, 70 + 20]
         self.file_data.seek(self.data_offSet, 0)
         all_packages = np.array(list(self.file_data.read(self.package_count * self.package_length))).reshape(
             [-1, self.package_length])
         all_package_data = all_packages[:, 8:]
+        raw_eeg = all_package_data.reshape([-1, self.resolution])
+        raw_eeg = raw_eeg[:, 0] + raw_eeg[:, 1] * 256
+        raw_eeg = np.squeeze(raw_eeg)
+        self.raw_data = np.transpose(np.copy(raw_eeg.reshape([-1, 2])))
+
 
         all_package_ids = all_packages[:, 0:8]
         all_package_ids = np.apply_along_axis(int_from_bytes_8bit, 1, all_package_ids)
         package_time_intervals = all_package_ids[1:] - all_package_ids[0:-1]
-
         package_time_intervals = np.round(package_time_intervals / self.package_std_time_interval[1])
         package_time_intervals = np.insert(package_time_intervals, 0, [1])
 
         package_repeats = package_time_intervals.astype(np.int32)
         package_repeats[package_repeats <= 0] = 1
 
         self.time_length = np.sum(package_repeats)*0.1
         self.package_loss = (np.sum(package_repeats) - package_repeats.__len__()) / np.sum(package_repeats) * 100
 
-        all_package_ids = np.repeat(all_package_ids, package_repeats, axis=0)
+        # all_package_ids = np.repeat(all_package_ids, package_repeats, axis=0)
         all_package_data = np.repeat(all_package_data, package_repeats, axis=0)
         all_package_data = all_package_data.reshape([-1, self.resolution])
 
-        # package_loss_new = all_package_ids.shape[0] / total_time*10
-
         all_package_data = all_package_data[:, 0] + all_package_data[:, 1] * 256
         all_package_data = np.squeeze(all_package_data)
 
+
+        # package_loss_new = all_package_ids.shape[0] / total_time*10
+
+
+
         data_total = all_package_data
         data_total = data_total[0:len(data_total) // 2 * 2]
         data_total_T = data_total.reshape(-1, 2)
         self.data_total = []
         self.data_total.append(data_total_T[:, 0])
         self.data_total.append(data_total_T[:, 1])
         self.data_total = np.asarray(self.data_total)
 
-        return self.data_total, self.package_loss, self.time_length
+        return self.raw_data, self.data_total, self.package_loss, self.time_length
 
 
 class ACCLoader(BaseLoader):
     def __init__(self, sf_send):
         super().__init__()
         if sf_send == 10:
             self.package_length = 38
@@ -159,14 +170,19 @@
         #     pass
         # else:
         #     self.package_std_time_interval = [70 - 20, 70, 70 + 20]
         self.file_data.seek(self.data_offSet, 0)
         all_packages = np.array(list(self.file_data.read(self.package_count * self.package_length))).reshape(
             [-1, self.package_length])
         all_package_data = all_packages[:, 8:]
+        raw_acc = all_package_data.reshape([-1, self.resolution])
+        raw_acc = raw_acc[:, 0] + raw_acc[:, 1] * 256
+        raw_acc = np.squeeze(raw_acc)
+        self.raw_data = np.transpose(np.copy(raw_acc.reshape([-1, 3])))
+
 
         all_package_ids = all_packages[:, 0:8]
         all_package_ids = np.apply_along_axis(int_from_bytes_8bit, 1, all_package_ids)
         package_time_intervals = all_package_ids[1:] - all_package_ids[0:-1]
 
         package_time_intervals = np.round(package_time_intervals / self.package_std_time_interval[1])
         package_time_intervals = np.insert(package_time_intervals, 0, [1])
@@ -191,17 +207,47 @@
         data_total_T = data_total.reshape(-1, 3)
         self.data_total = []
         self.data_total.append(data_total_T[:, 0])
         self.data_total.append(data_total_T[:, 1])
         self.data_total.append(data_total_T[:, 2])
         self.data_total = np.asarray(self.data_total)
 
-        return self.data_total, self.package_loss, self.time_length
+        return self.raw_data, self.data_total, self.package_loss, self.time_length
 
+class STILoader(BaseLoader):
+    def __init__(self):
+        super(STILoader, self).__init__()
+        self.package_length = 12
+    def load_data(self, data_path):
+        super(STILoader, self).load_data(data_path)
+
+        self.file_data.seek(self.data_offSet, 0)
+        all_packages = np.array(list(self.file_data.read(self.package_count * self.package_length))).reshape(
+            [-1, self.package_length])
+        all_package_data = all_packages[:, 8:]
+        all_package_ids = all_packages[:, 0:8]
+
+        all_package_data = all_package_data[:, 0] + all_package_data[:, 1] * 256 + all_package_data[:,
+                                                                                   2] * 256 * 256 + all_package_data[
+                                                                                                    :,
+                                                                                                    3] * 256 * 256 * 256
+        all_package_data = np.squeeze(all_package_data)
+        self.data_total = all_package_data
+        return self.data_total
 
+    def load_sti_log(self, data_path):
+        sti_index = []
+        with open(data_path) as f:
+            for line in f:
+                if line.startswith("point count: "):
+                    line = line.split("\t")[0]
+                    index_str = line[13:]
+                    sti_index.append(np.int32(index_str))
+        sti_index = np.asarray(sti_index)
+        return sti_index
 
 class BLELoader(BaseLoader):
     def __init__(self):
         super().__init__()
 
 
     def load_data(self, data_path):
```

### Comparing `lm_datahandler-0.1.3/lm_datahandler/datahandler.py` & `lm_datahandler-0.1.4/lm_datahandler/datahandler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,92 +1,98 @@
 import logging
 import os
-
+import sys
 import pandas as pd
 from scipy.io import savemat
 
 from lm_datahandler.data_load import data_loader
 from lm_datahandler.functions.biomarker import sw_detect, spindles_detect
-from lm_datahandler.functions.feature_extract import RSCFeature
-import scipy.signal as signal
+from lm_datahandler.functions.feature_extract import RSCFeature, WearDectectFeature
 from lm_datahandler.functions.sleep_staging import sleep_staging_with_features
+from lm_datahandler.functions.wear_detect import wear_detect_with_features
 import matplotlib.pyplot as plt
 import seaborn as sns
-from lm_datahandler.plots.sleep_staging_plot import plot_spectrogram, plot_avg_diff_acc, plot_sleep_staging_result
+from lm_datahandler.plots.sleep_staging_plot import plot_spectrogram, plot_avg_diff_acc, plot_sleep_staging_result, plot_sleep_posture
+from lm_datahandler.plots.stim_plot import plot_stim_sham_sw
 from lm_datahandler.functions.sleep_variable_compute import *
-
+from lm_datahandler.preprocess.filter import eeg_filter
+from lm_datahandler.functions.posture_analyse import sleep_posture_analyse
 
 class DataHandler(object):
     def __init__(self):
 
+        self.sleep_postures = None
+        self.raw_sti = None
         self.data_name = None
         self.logger = None
         self.sleep_variables = None
         self.seconds = None
         self.sp_df = None
         self.sleep_staging_result = None
-        self.raw_acc = None
-        self.raw_eeg = None
+        self.acc = None
+        self.eeg = None
         self.biomarker = None
         self.features = pd.DataFrame({})
         self.supported_features = {}
         self.sf_eeg = 500
         self.sf_acc = 50
         self.epoch_len = 15
         self.sw_df = None
 
         self.set_logger()
 
     def set_logger(self):
         self.logger = logging.getLogger("LM Data Handler")
         self.logger.setLevel("INFO")
         # 创建一个handler，用于输出日志到控制台
-        console_handler = logging.StreamHandler()
+        console_handler = logging.StreamHandler(stream=sys.stdout)
         console_handler.setLevel(logging.INFO)
 
-        # 创建一个formatter，定义日志的输出格式
-        formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-
+        formatter = logging.Formatter(
+            '%(asctime)s - %(levelname)s: %(message)s'
+        )
         # 将formatter添加到handler
         console_handler.setFormatter(formatter)
-
+        for handler in self.logger.handlers:
+            self.logger.removeHandler(handler)
         # 将handler添加到logger
         self.logger.addHandler(console_handler)
 
     def load_data_file(self, data_name, eeg_path, acc_path, ble_path, sti_path, sf_send, person_info=None):
-        assert data_name is not None, "Please check the data name and retry!"
+        assert data_name is not None, "Please check the data name and retry."
 
         self.data_name = data_name
-        self.raw_eeg, self.raw_acc, self.disconnections, self.total_time, self.package_loss_rate, self.disconnect_rate = data_loader.load_data(
-            eeg_path, acc_path, ble_path, sf_send)
-
-        self.raw_eeg = (self.raw_eeg[0] - 32767) / 65536 * 2.5 * 1000 * 1000 / 100
-        self.raw_eeg = np.squeeze(self.raw_eeg)
-        self.raw_acc = self.raw_acc - 32767
-        self.raw_acc = np.squeeze(self.raw_acc)
-
-        eeg_sec = self.raw_eeg.shape[0] // self.sf_eeg
-        if self.raw_acc is not None:
-            acc_sec = self.raw_acc.shape[1] // self.sf_acc
+        self.raw_eeg, self.eeg, self.raw_acc, self.acc, self.raw_sti, self.disconnections, self.total_time, self.package_loss_rate, self.disconnect_rate = data_loader.load_data(
+            eeg_path, acc_path, sti_path, ble_path, sf_send, logger=self.logger)
+        self.eeg = (self.eeg[0] - 32767) / 65536 * 2.5 * 1000 * 1000 / 100
+        self.raw_eeg = self.raw_eeg[0]
+        self.eeg = np.squeeze(self.eeg)
+        self.acc = self.acc - 32767
+        self.acc = np.squeeze(self.acc)
+
+        eeg_sec = self.eeg.shape[0] // self.sf_eeg
+        if self.acc is not None:
+            acc_sec = self.acc.shape[1] // self.sf_acc
             assert eeg_sec == acc_sec, "EEG length have to be consistent with ACC."
         self.seconds = eeg_sec
-        self.raw_eeg = self.raw_eeg[:self.seconds * self.sf_eeg]
-        self.raw_acc = self.raw_acc[:self.seconds * self.sf_acc]
+        self.eeg = self.eeg[:self.seconds * self.sf_eeg]
+        self.acc = self.acc[:self.seconds * self.sf_acc]
         self.logger.info("Data loaded, {} total seconds".format(self.seconds))
 
         self.features['meta'] = {'male': 1, 'age': 30, 'data_type': 0, 'h/w': 0}
         if person_info is not None:
             if person_info['male'] is not None:
                 self.features['meta']['male'] = person_info['male']
             if person_info['age'] is not None:
                 self.features['meta']['age'] = person_info['age']
             if person_info['data_type'] is not None:
                 self.features['meta']['data_type'] = person_info['data_type']
             if person_info['height'] is not None and person_info['weight'] is not None:
                 self.features['meta']['h/w'] = person_info['height'] / person_info['weight']
+        return self
 
     def load_data(self, data_name, data_path, sf_send=10, person_info=None):
         assert data_name is not None, "Please check the data name and retry!"
         self.data_name = data_name
         eeg_path = None
         acc_path = None
         sti_path = None
@@ -97,22 +103,23 @@
             if file.endswith(".acc"):
                 acc_path = os.path.join(data_path, file)
             if file.endswith(".sti"):
                 sti_path = os.path.join(data_path, file)
             if file.endswith(".ble"):
                 ble_path = os.path.join(data_path, file)
         self.load_data_file(data_name, eeg_path, acc_path, ble_path, sti_path, sf_send, person_info)
+        return self
 
     def save_data_to_mat(self, mat_path):
-        if self.raw_eeg is None:
+        if self.eeg is None:
             self.logger.info("Please load EEG data first.")
-        if self.raw_acc is None:
+        if self.acc is None:
             self.logger.info("Please load ACC data first.")
-        savemat(mat_path, {'EEG_total': self.raw_eeg, 'ACC': self.raw_acc, 'package_loss_rate': self.package_loss_rate,
-                           'disconnect_rate': self.disconnect_rate})
+        savemat(mat_path, {'EEG_total': self.eeg, 'ACC': self.acc, 'package_loss_rate': self.package_loss_rate,
+                           'disconnect_rate': -1 if self.disconnect_rate is None else self.disconnect_rate})
 
     def load_hypno(self, hypno):
         hypno = np.asarray(hypno)
         if np.shape(hypno.shape) != 1 or hypno.shape[0] <= 0:
             self.logger.error("Format of hypno is incorrect, please check hypno is one-dimension array!")
             return
         if self.sleep_staging_result is not None and hypno.shape[0] != self.sleep_staging_result.shape[0]:
@@ -131,100 +138,116 @@
             start_sec = 0
             end_sec = self.seconds // self.epoch_len * self.epoch_len
         if tailor_type == "custom" and tailor_param is not None:
             start_sec = tailor_param['start_sec']
             end_sec = tailor_param['end_sec']
             assert start_sec is not None and end_sec is not None, "tailor_param is a dict consist of start_sec and end_sec, please check!"
 
-        self.raw_eeg = self.raw_eeg[start_sec * self.sf_eeg:end_sec * self.sf_eeg]
-        self.raw_acc = self.raw_acc[:, start_sec * self.sf_acc:end_sec * self.sf_acc]
+        self.eeg = self.eeg[start_sec * self.sf_eeg:end_sec * self.sf_eeg]
+        self.acc = self.acc[:, start_sec * self.sf_acc:end_sec * self.sf_acc]
         self.seconds = end_sec - start_sec
         self.logger.info(
             "Loaded data is clipped to a multiple of the window length, {} total seconds".format(self.seconds))
 
     def preprocess(self, filter_param={'highpass': 0.5, 'lowpass': None, 'bandstop': [[49, 51]]},
                    tailor_type="drop_tail", tailor_param=None):
         self.tailor_operation(tailor_type, tailor_param)
 
         self.highpass = filter_param['highpass']
         self.bandstop = filter_param['bandstop']
         self.lowpass = filter_param['lowpass']
+
+        self.eeg = eeg_filter(self.eeg, self.sf_eeg, self.highpass, 3, self.lowpass, 3, self.bandstop, 3)
         log_info = "EEG filtered: "
         if self.highpass is not None:
-            wn = 2 * self.highpass / self.sf_eeg
-            b, a = signal.butter(3, wn, 'highpass', analog=False)
-            self.raw_eeg = signal.filtfilt(b, a, self.raw_eeg, axis=0)
             log_info += "Highpass: {} Hz".format(self.highpass)
         if self.lowpass is not None:
-            wn = 2 * self.lowpass / self.sf_eeg
-            b, a = signal.butter(3, wn, 'lowpass', analog=False)
-            self.raw_eeg = signal.filtfilt(b, a, self.raw_eeg, axis=0)
             log_info += ", Lowpass: {} Hz".format(self.lowpass)
         if self.bandstop is not None:
-            w0 = self.bandstop[0][0] / (self.sf_eeg / 2)
-            w1 = self.bandstop[0][1] / (self.sf_eeg / 2)
-            b, a = signal.butter(3, [w0, w1], btype='bandstop', analog=False)
-            self.raw_eeg = signal.filtfilt(b, a, self.raw_eeg, axis=0)
             log_info += ", Bandstop: {} Hz.".format(self.bandstop)
         self.logger.info(log_info)
         return self
 
     # def feature_extract(self, feature_names={}):
     #     unsupoort_features = feature_names - self.supported_features
     #     if len(unsupoort_features) > 0:
     #         self.logger.warning("{}/{} input features are not support: ".format(len(unsupoort_features), len(feature_names),
     #                                                                         unsupoort_features))
 
+    def wear_detect(self, model_path=None):
+        if model_path is not None:
+            self.logger.info("Wear detect model is set, please make sure the features are corresponded.")
+        person_info = dict(age=30, male=1, datatype=0)
+        epochs = self.eeg.shape[0] // (self.sf_eeg * self.epoch_len)
+        input_eeg = self.eeg[0:epochs * self.sf_eeg * self.epoch_len].reshape(-1, self.sf_eeg)
+        wear_detect_features = WearDectectFeature(person_info, input_eeg, self.sf_eeg, context_mode=3).get_features()
+        wear_detect_res = wear_detect_with_features(features=wear_detect_features, model_path=model_path)
+
+        wear_detect_res = wear_detect_res.reshape([-1, 15])
+        wear_detect_res = np.sum(wear_detect_res, axis=1)
+        wear_detect_res[wear_detect_res <= 15 * 0.5] = 0
+        wear_detect_res[wear_detect_res > 15 * 0.5] = 1
+
+        return wear_detect_res
+
+
     def sleep_staging(self, use_acc=False, use_time=False, context_mode=2, model_path=None):
-        if self.raw_eeg is None:
+        if self.eeg is None:
             self.logger.info("The EEG data is not loaded, please load EEG first.")
         self.logger.info("Sleep staging started.")
-        epochs = self.raw_eeg.shape[0] // (self.sf_eeg * self.epoch_len)
-        input_eeg = self.raw_eeg[0:epochs * self.sf_eeg * self.epoch_len].reshape(-1, self.sf_eeg * self.epoch_len)
+        epochs = self.eeg.shape[0] // (self.sf_eeg * self.epoch_len)
+        input_eeg = self.eeg[0:epochs * self.sf_eeg * self.epoch_len].reshape(-1, self.sf_eeg * self.epoch_len)
         # data = np.load('E:/dataset/x7_disorder/npzData/20230511_19145647867.npz')
         # input_eeg = data['x'].reshape(-1, 500*15)
         # epochs = 1800
-        acc = self.raw_acc[:, 0:epochs * self.sf_acc * self.epoch_len]
+        acc = self.acc[:, 0:epochs * self.sf_acc * self.epoch_len]
         # acc = data['acc']
         accx = acc[0, :].reshape(-1, 1, 750)
         accy = acc[1, :].reshape(-1, 1, 750)
         accz = acc[2, :].reshape(-1, 1, 750)
         input_acc = np.concatenate([accx, accy, accz], axis=1)
 
         self.features = RSCFeature(self.features['meta'], raw_eeg=input_eeg, raw_acc=input_acc,
                                    sf_eeg=self.sf_eeg, sf_acc=self.sf_acc).get_features()
         self.logger.info("Feature extraction finished.")
         predictions, pp_predictions = sleep_staging_with_features(self.features, use_acc=use_acc, use_time=use_time,
                                                                   context_mode=context_mode, model_path=model_path)
+
+        wear_detect_res = self.wear_detect()
+        pp_predictions[wear_detect_res == 0] = 4
         self.sleep_staging_result = pp_predictions
         self.logger.info("Sleep staging finished.")
         return self
 
     def plot_sleep_data(self, plot_spectral=True, plot_acc=True, plot_staging=True, plot_variables=True, savefig=None):
         if self.sleep_staging_result is None:
             self.logger.info("Sleep staging result is none, auto sleep staging will run first!")
 
-        if self.sleep_variables is None:
+        if plot_variables and self.sleep_variables is None:
             self.logger.info(
                 "Sleep variables is none, and will computed first. If you don't want it, just change \"plot_variables\" to False.")
             self.compute_sleep_variables()
 
-        subplot_count = 0 + plot_acc + plot_spectral + plot_staging
+        subplot_count = 0 + 2*plot_acc + plot_spectral + plot_staging
         fig, ax = plt.subplots(subplot_count, 1, figsize=(16, subplot_count * 4))
         fig.subplots_adjust(hspace=0.5)
         if subplot_count == 1:
             ax = [ax]
 
         i = 0
         if plot_spectral:
-            plot_spectrogram(fig, ax[i], self.raw_eeg, self.sf_eeg)
+            plot_spectrogram(fig, ax[i], self.eeg, self.sf_eeg)
 
         i += 1
         if plot_acc:
-            plot_avg_diff_acc(fig, ax[i], self.raw_acc, self.sf_acc)
+            plot_avg_diff_acc(fig, ax[i], self.acc, self.sf_acc)
+            i += 1
+            if self.sleep_postures is None:
+                self.sleep_postures = sleep_posture_analyse(self.acc)
+            plot_sleep_posture(fig, ax[i], self.sleep_postures, self.sf_acc)
 
         i += 1
         if plot_staging:
             if self.sleep_staging_result is None:
                 self.logger.info("The sleep staging result is None, auto sleep staging will run first!")
                 self.sleep_staging()
             variables = None
@@ -238,47 +261,47 @@
 
         if savefig is not None:
             plt.savefig(savefig, dpi=300, bbox_inches='tight')
             self.logger.info("The sleep data plot is saved as {}".format(savefig))
         return self
 
     def compute_sleep_variables(self, hypno=None):
-        """
-            compute multi sleep index
-            :rtype: object
-            :param hypno:
-            :param epoch_length:
-            :return: tst, sl, waso, se, arousal_time
-        """
+
         if hypno is not None:
             self.logger.info("Sleep variables will be computed by the giving hypno instead of the loaded data!")
         elif self.sleep_staging_result is None:
             self.logger.info("Sleep variables are based on sleep staging result, auto sleep staging will run first!")
 
         tst = tst_compute(self.sleep_staging_result, self.epoch_len)
         sl = sl_compute(self.sleep_staging_result, self.epoch_len)
-        # waso = waso_compute(self.sleep_staging_result, self.epoch_len)
-        se = se_compute(self.sleep_staging_result)
-        arousal_count, arousal_time = arousal_time_compute(self.sleep_staging_result, self.epoch_len)
-        waso = arousal_time.shape[0] * self.epoch_len
+        if sl == -1:
+            self.logger.info("No continuous sleep epochs are detected!")
+            se = 0.0
+            arousal_time = np.asarray([])
+            arousal_count = 0
+            waso = 0
+        else:
+            se = se_compute(self.sleep_staging_result)
+            arousal_count, arousal_time = arousal_time_compute(self.sleep_staging_result, self.epoch_len)
+            waso = arousal_time.shape[0] * self.epoch_len
         self.sleep_variables = {
             "TST": tst,
             "SOL": sl,
             "WASO": waso,
             "SE": se,
             "AR": arousal_count,
             "ART": arousal_time
         }
-        print("TST: {} s\nSOL: {} s\nSE: {}%\nWASO: {} s\nAR: {}".format(tst, sl, se * 100, waso, arousal_count))
+        print("TST:\t{} s\nSOL:\t{} s\nSE:\t\t{}%\nWASO:\t{} s\nAR:\t\t{}".format(tst, sl, se * 100, waso, arousal_count))
 
         return self
 
     def get_sleep_variables(self):
         if self.sleep_variables is None:
-            self.logger.info("Sleep variables are None, please run compute_sleep_variables first.")
+            self.logger.error("Sleep variables are None, please run compute_sleep_variables first.")
         return self.sleep_variables
 
     def spindle_detect(self, hypno_mask=(0, 1), freq_sp=(12, 15), freq_broad=(1, 30), duration=(0.5, 2),
                        min_distance=100,
                        thresh_rel_pow=0.2, thresh_corr=0.65, thresh_rms=1.5):
         self.logger.info("Spindle detect start.")
 
@@ -287,20 +310,21 @@
             if self.sleep_staging_result is None:
                 self.logger.info(
                     "Sleep staging result is need for spindle detection, auto sleep staging will run first!")
                 self.sleep_staging()
             mask = np.in1d(self.sleep_staging_result, hypno_mask)
             mask = np.repeat(mask, self.sf_eeg * self.epoch_len)
 
-        self.sp_df = spindles_detect(self.raw_eeg, mask=mask, freq_sp=freq_sp, freq_broad=freq_broad,
+        self.sp_df = spindles_detect(self.eeg, mask=mask, freq_sp=freq_sp, freq_broad=freq_broad,
                                      duration=duration,
                                      min_distance=min_distance, thresh_rel_pow=thresh_rel_pow, thresh_rms=thresh_rms,
                                      thresh_corr=thresh_corr)
+        logging.getLogger("").isEnabledFor(logging.WARNING)
         if self.biomarker is None:
-            self.biomarker = np.zeros(self.raw_eeg.shape[0])
+            self.biomarker = np.zeros(self.eeg.shape[0])
         for row in np.arange(self.sp_df.shape[0]):
             self.biomarker[self.sp_df['Start_Index'][row]:self.sp_df['End_Index'][row]] = 1
         self.logger.info("Spindle detect finished.")
         # print(self.sp_df)
         return self
 
     def sw_detect(self, hypno_mask=(0, 1), freq_sw=(0.3, 1.5), dur_neg=(0.3, 1.5), dur_pos=(0.1, 1), amp_neg=(40, 200),
@@ -311,29 +335,26 @@
             if self.sleep_staging_result is None:
                 self.logger.info(
                     "Sleep staging result is need for slow-wave detection, auto sleep staging will run first!")
                 self.sleep_staging()
             mask = np.in1d(self.sleep_staging_result, hypno_mask)
             mask = np.repeat(mask, self.sf_eeg * self.epoch_len)
 
-        self.sw_df = sw_detect(self.raw_eeg, sf=self.sf_eeg, mask=mask, freq_sw=freq_sw, dur_neg=dur_neg,
+        self.sw_df = sw_detect(self.eeg, sf=self.sf_eeg, mask=mask, freq_sw=freq_sw, dur_neg=dur_neg,
                                dur_pos=dur_pos,
                                amp_neg=amp_neg, amp_pos=amp_pos, amp_ptp=amp_ptp, coupling=coupling,
                                coupling_params=coupling_params)
         if self.biomarker is None:
-            self.biomarker = np.zeros(self.raw_eeg.shape[0])
+            self.biomarker = np.zeros(self.eeg.shape[0])
         for row in np.arange(self.sw_df.shape[0]):
             self.biomarker[self.sw_df['Start_Index'][row]:self.sw_df['End_Index'][row]] = 2
         self.logger.info("Slow-wave detect finished.")
         # print(self.sw_df)
         return self
 
-    def show_sp_results(self):
-        pass
-
     def export_sp_results(self, save_file=None):
         if self.sp_df is None:
             self.logger.info("The spindle detection result is None, spindle detection will run first.")
             self.spindle_detect()
         if save_file is None:
             self.logger.info("File save path is not configured, default saved to ./saved_files/{}".format(
                 "spindle_result_" + self.data_name + ".csv"))
@@ -366,32 +387,32 @@
             self.logger.info("You have not run spindle detect, spindle detect will run first!")
             self.spindle_detect()
         if self.sp_df.size < sp_index or sp_index <= 0:
             self.logger.error("The input sp_index is invalid, please check!")
         sp = self.sp_df.iloc[sp_index]
         mid = (sp["Start_Index"] + sp["End_Index"]) // 2
         min_index = max(mid - range / 2, 0)
-        max_index = min(mid + range / 2, self.raw_eeg.shape[0])
+        max_index = min(mid + range / 2, self.eeg.shape[0])
         self.plot_sp_results_by_range(start_index=min_index, end_index=max_index,
                                       title="spindle detection result: No.{}".format(sp_index), savefig=savefig)
         if savefig is not None:
             self.logger.info("The spindle plot is saved to {}".format(savefig))
         return self
 
     def plot_sp_results_by_range(self, start_index, end_index, title=None, savefig=None):
         if end_index - start_index > 8000:
-            self.logger.error("For best view, please make sure the sample size is around 5000!")
+            self.logger.error("For best view, please make sure the sample size is around 5000, plot is skipped.")
             return
         if self.sp_df is None:
             self.logger.info("You have not run spindle detect, spindle detect will run first!")
             self.spindle_detect()
         start_index = int(start_index)
         end_index = int(end_index)
         mask = self.biomarker[start_index: end_index]
-        data = self.raw_eeg[start_index: end_index]
+        data = self.eeg[start_index: end_index]
         mask[mask != 1] = np.nan
         times = np.arange(start_index, end_index) / self.sf_eeg
         plt.figure(figsize=(14, 4))
         plt.plot(times, data, 'k')
         plt.plot(times, mask * data, 'indianred')
         plt.xlabel('Time (seconds)')
         plt.ylabel('Amplitude (uV)')
@@ -411,15 +432,15 @@
             self.logger.info("You have not run slow wave detect, slow wave detect will run first!")
             self.sw_detect()
         if self.sw_df.size < sw_index or sw_index <= 0:
             self.logger.error("The input sp_index is invalid, please check!")
         sw = self.sw_df.iloc[sw_index]
         mid = (sw["Start_Index"] + sw["End_Index"]) // 2
         min_index = max(mid - range / 2, 0)
-        max_index = min(mid + range / 2, self.raw_eeg.shape[0])
+        max_index = min(mid + range / 2, self.eeg.shape[0])
         self.plot_sw_results_by_range(start_index=min_index, end_index=max_index,
                                       title="slow wave result: No.{}".format(sw_index), savefig=savefig)
         if savefig is not None:
             self.logger.info("The slow-wave plot is saved as {}".format(savefig))
         return self
 
     def plot_sw_results_by_range(self, start_index, end_index, title=None, savefig=None):
@@ -429,15 +450,15 @@
 
         if end_index - start_index > 8000:
             self.logger.error("For best view, please make sure the sample size is around 5000!")
             return
         start_index = int(start_index)
         end_index = int(end_index)
         mask = self.biomarker[start_index: end_index]
-        data = self.raw_eeg[start_index: end_index]
+        data = self.eeg[start_index: end_index]
         mask[mask != 2] = np.nan
         mask[mask == 2] = 1
         times = np.arange(start_index, end_index) / self.sf_eeg
         plt.figure(figsize=(14, 4))
         plt.plot(times, data, 'k')
         plt.plot(times, mask * data, 'indianred')
         plt.xlabel('Time (seconds)')
@@ -448,47 +469,31 @@
         else:
             plt.title(title)
         sns.despine()
         if savefig is not None:
             plt.savefig(savefig, dpi=300, bbox_inches='tight')
         return self
 
+    def plot_sw_stim_sham(self, savefig=None):
+        if self.raw_sti is None:
+            self.logger.error(
+                "The sti indexs is None, please make sure the .sti file is loaded before plot sw stim vs sham.")
+            return self
+        if self.raw_sti.shape[0] < 10:
+            self.logger.error("The count of stim/sham points is less than expected, slow-wave stim sham plot will be skipped.")
+            return self
+        eeg_copy = np.copy(self.raw_eeg)
+        plot_stim_sham_sw(eeg_copy, self.raw_sti, self.sf_eeg, savefig)
+
+    def show_plots(self):
+        plt.show()
+
 
 if __name__ == '__main__':
     data_handler = DataHandler()
-    data_handler.load_data(data_name="20230614_15663630175",
-                           data_path="E:/dataset/dev_test_data/x7_50Hz/20230614_15663630175", sf_send=50)
+    data_handler.load_data(data_name="20230614_15927226341", data_path=r"E:\dataset\dev_test_data\20230614_15927226341")
+
+    data_handler.plot_sw_stim_sham()
+    data_handler.preprocess().sleep_staging().compute_sleep_variables().plot_sleep_data()
+
+    data_handler.show_plots()
 
-    data_handler.save_data_to_mat('E:/dataset/dev_test_data/x7_50Hz/20230614_15663630175/Data.mat')
-    data_handler.preprocess().sleep_staging().compute_sleep_variables().plot_sleep_data().plot_sp_results_by_id(
-        16, savefig="E:\dataset\dev_test_data\sp_16.png").plot_sw_results_by_range(3685 * 500, 3695 * 500,
-                                                                                   savefig="E:\dataset\dev_test_data\sw1.png")
-
-    plt.show()
-    # print(data_handler.sleep_staging_result)
-    # data_handler.load_data_file(data_name="20230511_19145647867",
-    #                             eeg_path='E:/dataset/x7_disorder/matlabData/20230511_19145647867/eeg.eeg',
-    #                             acc_path='E:/dataset/x7_disorder/matlabData/20230511_19145647867/acc.acc',
-    #                             ble_path=None,
-    #                             sti_path='E:/dataset/x7_disorder/matlabData/20230511_19145647867/sti.sti')
-    # data_handler.preprocess(tailor_type="drop_tail", tailor_param=None)
-    # # data_handler.raw_eeg = data_handler.raw_eeg-32767
-    # sleep_staging_results = data_handler.sleep_staging()
-    # # print(sleep_staging_results)
-    # # data_handler.compute_sleep_variables()
-    # # data_handler.(plot_spectral=True, plot_acc=True, plot_staging=True, plot_variables=True)
-    # sp_df = data_handler.spindle_detect().plot_sp_results_by_id(16)
-    # # print(sp_df)
-    # # data_handler.export_sp_results()
-    # # data_handler
-    # # data_handler.plot_sp_results_by_range(start_index=7050 * 500, end_index=7060 * 500)
-    #
-    # data_handler.sw_detect().plot_sw_results_by_range(3685 * 500, 3695 * 500).export_sw_results()
-    # savemat("./20230511_19145647867_eeg.mat", {"eeg": data_handler.raw_eeg})
-    #
-    # mask = np.zeros(data_handler.raw_eeg.shape)
-    # for index, row in data_handler.sw_df.iterrows():
-    #     mask[int(row["Start_Index"]): int(row["End_Index"])] = 1
-    # mask = mask * data_handler.raw_eeg
-    # savemat("./20230511_19145647867_sw.mat", {"sw": mask})
-    # print(data_handler.sw_df)
-    # plt.show()
```

### Comparing `lm_datahandler-0.1.3/lm_datahandler/functions/biomarker.py` & `lm_datahandler-0.1.4/lm_datahandler/functions/biomarker.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.3/lm_datahandler/functions/feature_extract.py` & `lm_datahandler-0.1.4/lm_datahandler/functions/feature_extract.py`

 * *Files 23% similar despite different names*

```diff
@@ -357,7 +357,360 @@
             bp /= total_power
 
         all_freqs = all_freqs.reshape(-1, 2)
         total_bands = all_freqs[:, 1] - all_freqs[:, 0]
         total_bands = total_bands[..., np.newaxis]
         bp /= total_bands
         return bp
+
+
+
+class WearDectectFeature:
+    # bands = [
+    #     (0.4, 1, "sdelta"),
+    #     (1, 4, "fdelta"),
+    #     (0.4, 4, "delta"),
+    #     (4, 8, "theta"),
+    #     (8, 12, "alpha"),
+    #     (12, 16, "sigma"),
+    #     (16, 30, "beta"),
+    # ]
+
+    bands = [
+        (1, 2, "sdelta"),
+        (0, 4, "delta"),
+        (1, 4, "fdelta"),
+        (2, 3, "delta4"),
+
+        (4, 8, "theta"),
+        (4, 6, "theta2"),
+
+        (4, 12, "n_wave"),
+        (4, 10, "n_wave2"),
+
+        (8, 12, "alpha"),
+        (8, 10, "alpha2"),
+
+        (12, 16, "sigma"),
+        (12, 20, "sigma2"),
+        (14, 18, "sigma3"),
+
+        (12, 24, "rem_wave3"),
+        (12, 30, "rem_wave"),
+        (10, 16, "rem_wave2"),
+
+        (16, 30, "beta"),
+        (16, 23, "beta2"),
+        (23, 30, "beta3"),
+
+        (30, 35, "gama0"),
+        (35, 49, "gama"),
+        (49, 51, "gama2"),
+        (51, 60, "gama3"),
+        (60, 75, "gama4"),
+    ]
+
+    def __init__(self, person_info, raw_eeg, sf_eeg=500, raw_acc=None, sf_acc=50, context_mode=1, data_type=0):
+        super().__init__()
+        self.feature_name_ = None
+        self.raw_eeg = raw_eeg
+        self.sf_eeg = sf_eeg
+        self.raw_acc = raw_acc
+        self.sf_acc = sf_acc
+        self.feature_in_dataframe = None
+        self.person_info = person_info
+
+        self.fit(context_mode, data_type)
+
+    def fit(self, context_mode, data_type):
+        feature = {}
+
+        freq_feature, freqs, psd = self.generate_freq_feature(welch_window=1)
+        feature.update(freq_feature)
+
+        statistic_feature = self.generate_statistic_feature(self.raw_eeg, context_mode=context_mode)
+        feature.update(statistic_feature)
+
+        other_feature = self.generate_other_feature(freqs, psd, self.raw_eeg, context_mode=context_mode)
+        feature.update(other_feature)
+
+        self.feature_in_dataframe = pd.DataFrame(feature).add_prefix("eeg_")
+        if self.raw_acc is not None:
+            acc_feature = self.generate_acc_feature(raw_acc=self.raw_acc)
+            acc_feature_in_dataframe = pd.DataFrame(acc_feature).add_prefix("acc_")
+            self.feature_in_dataframe = self.feature_in_dataframe.join(acc_feature_in_dataframe)
+
+        self.feature_in_dataframe.index.name = "epoch"
+
+        # Apply centered rolling average (15 epochs = 7 min 30)
+        # Triang: [0.125, 0.25, 0.375, 0.5, 0.625, 0.75, 0.875, 1.,
+        #          0.875, 0.75, 0.625, 0.5, 0.375, 0.25, 0.125]
+        if context_mode == 2:
+            rollc = self.feature_in_dataframe.rolling(window=25, center=True, min_periods=1, win_type="triang").mean()
+            rollc[rollc.columns] = robust_scale(rollc, quantile_range=(5, 95))
+            rollc = rollc.add_suffix("_c6min_norm")
+
+            # Now look at the past 2 minutes
+            rollp = self.feature_in_dataframe.rolling(window=15, min_periods=1).mean()
+            rollp[rollp.columns] = robust_scale(rollp, quantile_range=(5, 95))
+            rollp = rollp.add_suffix("_p2min_norm")
+            self.feature_in_dataframe = self.feature_in_dataframe.join(rollp)
+            self.feature_in_dataframe = self.feature_in_dataframe.join(rollc)
+
+        if context_mode == 1:
+            rollp = self.feature_in_dataframe.rolling(window=15, min_periods=1).mean()
+            # rollp[rollp.columns] = robust_scale(rollp, quantile_range=(5, 95))
+            rollp = rollp.add_suffix("_p2min_norm")
+            self.feature_in_dataframe = self.feature_in_dataframe.join(rollp)
+
+        if context_mode == 3:
+            pass
+
+        #######################################################################
+        # TEMPORAL + METADATA FEATURES AND EXPORT
+        #######################################################################
+
+        # Add temporal features
+        epochs = self.raw_eeg.shape[0]
+        times = np.arange(0, epochs, 1) * 5
+
+        self.feature_in_dataframe["time_hour"] = times / 3600
+        self.feature_in_dataframe["time_norm"] = times / times[-1]
+
+        if self.person_info is not None:
+            for c in self.person_info.keys():
+                self.feature_in_dataframe[c] = self.person_info[c]
+
+        self.feature_in_dataframe["data_type"] = data_type
+
+        # Sort the column names here (same behavior as lightGBM)
+        self.feature_in_dataframe.sort_index(axis=1, inplace=True)
+        self.feature_name_ = self.feature_in_dataframe.columns.tolist()
+
+    def generate_other_feature(self, freqs, psd, epochs, context_mode):
+        freq_broad = (0, 75)
+        idx_broad = np.logical_and(freqs >= freq_broad[0], freqs <= freq_broad[1])
+        dx = freqs[1] - freqs[0]
+        # Calculate entropy and fractal dimension features
+        if context_mode == 2:
+            other_features = {
+                "abspow": np.trapz(psd[:, idx_broad], dx=dx),
+                "perm": np.apply_along_axis(ant.perm_entropy, axis=1, arr=epochs, normalize=True),
+                "higuchi": np.apply_along_axis(ant.higuchi_fd, axis=1, arr=epochs),
+                "petrosian": ant.petrosian_fd(epochs, axis=1)
+            }
+        elif context_mode == 1 or context_mode == 3:
+            other_features = {
+                "abspow": np.trapz(psd[:, idx_broad], dx=dx),
+                # "perm": np.apply_along_axis(ant.perm_entropy, axis=1, arr=epochs, normalize=True),
+                # "higuchi": np.apply_along_axis(ant.higuchi_fd, axis=1, arr=epochs),
+                "petrosian": ant.petrosian_fd(epochs, axis=1)
+            }
+        return other_features
+
+    def generate_freq_feature(self, welch_window=1):
+        win = int(welch_window * self.sf_eeg)
+        kwargs_welch = dict(window="hamming", nperseg=win, average="median")
+        freqs, psd = sp_sig.welch(self.raw_eeg, self.sf_eeg, **kwargs_welch)
+
+        feature = {}
+
+        bp = self.bandpower_from_psd_ndarray(psd, freqs, relative=False)
+        for j, (_, _, b) in enumerate(self.bands):
+            feature[b] = bp[j]
+
+        # zscore(a, axis=0, ddof=0, nan_policy='propagate')
+
+        delta = feature["delta"]
+        # band_ratio = {
+        #     "dt": delta / feature["theta"],
+        #     "ds": delta / feature["sigma"],
+        #     "db": delta / feature["beta"],
+        #     "at": feature["alpha"] / feature["theta"],
+        # }
+        band_ratio = {
+            "dt": feature["delta"] / feature["theta"] ,
+            "dn": feature["delta"] / feature["n_wave"] ,
+            "dr": feature["delta"] / feature["rem_wave"] ,
+            "ds": feature["delta"] / feature["sigma"] ,
+            "db": feature["delta"] / feature["beta"] ,
+            "da": feature["delta"] / feature["alpha"] ,
+            "at": feature["alpha"] / feature["theta"] ,
+            "as": feature["alpha"] / feature["sigma"] ,
+            "ar": feature["alpha"] / feature["rem_wave"] ,
+            "ab": feature["alpha"] / feature["beta"] ,
+            "rn": feature["rem_wave"] / feature["n_wave"],
+            "gr": feature["gama"] / feature["rem_wave"],
+            "gn": feature["gama"] / feature["n_wave"] ,
+            "g3n": feature["gama3"] / feature["n_wave"],
+            "g3a": feature["gama3"] / feature["alpha"],
+            "g3b": feature["gama3"] / feature["beta"] ,
+            "g3t": feature["gama3"] / feature["theta"],
+            "g3r": feature["gama3"] / feature["rem_wave"],
+            "g3d": feature["gama3"] / feature["delta"] ,
+        }
+
+
+        feature.update(band_ratio)
+        # feature = band_ratio
+
+        return feature, freqs, psd
+
+    def generate_statistic_feature(self, raw_eeg, context_mode):
+        if context_mode == 2:
+            hmob, hcomp = ant.hjorth_params(raw_eeg, axis=1)
+            feat = {
+                "std": np.std(raw_eeg, ddof=1, axis=1),
+                "iqr": sp_stats.iqr(raw_eeg, rng=(25, 75), axis=1),
+                "skew": sp_stats.skew(raw_eeg, axis=1),
+                "kurt": sp_stats.kurtosis(raw_eeg, axis=1),
+                "nzc": ant.num_zerocross(raw_eeg, axis=1),
+                "hmob": hmob,
+                "hcomp": hcomp,
+            }
+        elif context_mode == 1 or context_mode == 3:
+            feat = {
+                "std": np.std(raw_eeg, ddof=1, axis=1),
+                "iqr": sp_stats.iqr(raw_eeg, rng=(25, 75), axis=1),
+                "skew": sp_stats.skew(raw_eeg, axis=1),
+                "kurt": sp_stats.kurtosis(raw_eeg, axis=1),
+                "nzc": ant.num_zerocross(raw_eeg, axis=1),
+            }
+        return feat
+
+    def generate_acc_feature(self, raw_acc):
+        abs_acc = np.abs(raw_acc)
+        # abs_acc_avg = np.average(abs_acc, axis=2)
+        # abs_acc_std = np.std(abs_acc, axis=2)
+        # feat = {"x_abs_avg": abs_acc_avg[:, 0],
+        #         "y_abs_avg": abs_acc_avg[:, 1],
+        #         "z_abs_avg": abs_acc_avg[:, 2],
+        #         "x_abs_std": abs_acc_std[:, 0],
+        #         "y_abs_std": abs_acc_std[:, 1],
+        #         "z_abs_std": abs_acc_std[:, 2]
+        #         }
+        feat = {}
+        max_channel = np.zeros([abs_acc.shape[0], abs_acc.shape[2]])
+        max_channel[(abs_acc[:, 0, :] > abs_acc[:, 1, :]) & (abs_acc[:, 0, :] > abs_acc[:, 2, :])] = 1
+        feat["x_max_percentage"] = np.sum(max_channel, axis=1) / max_channel.shape[1]
+
+        max_channel = np.zeros([abs_acc.shape[0], abs_acc.shape[2]])
+        max_channel[(abs_acc[:, 1, :] > abs_acc[:, 2, :]) & (abs_acc[:, 1, :] > abs_acc[:, 0, :])] = 1
+        feat["y_max_percentage"] = np.sum(max_channel, axis=1) / max_channel.shape[1]
+
+        max_channel = np.zeros([abs_acc.shape[0], abs_acc.shape[2]])
+        max_channel[(abs_acc[:, 2, :] > abs_acc[:, 1, :]) & (abs_acc[:, 2, :] > abs_acc[:, 0, :])] = 1
+        feat["z_max_percentage"] = np.sum(max_channel, axis=1) / max_channel.shape[1]
+
+        diff_acc_x = np.abs(raw_acc[:, 0, 1:-2] - raw_acc[:, 0, 2:-1])
+        diff_acc_y = np.abs(raw_acc[:, 1, 1:-2] - raw_acc[:, 1, 2:-1])
+        diff_acc_z = np.abs(raw_acc[:, 2, 1:-2] - raw_acc[:, 2, 2:-1])
+        diff_acc = diff_acc_z + diff_acc_y + diff_acc_x
+        # feat["diff_sum"] = np.sum(diff_acc, axis=1)
+        feat["diff_avg"] = np.average(diff_acc, axis=1)
+        feat["diff_std"] = np.std(diff_acc, axis=1)
+        diff_global_avg = np.average(diff_acc)
+        diff_global_std = np.std(diff_acc)
+        feat["diff_avg_ratio"] = feat["diff_avg"] / diff_global_avg
+        feat["diff_std_ratio"] = feat["diff_std"] / diff_global_std
+
+        feat["diff_iqr"] = sp_stats.iqr(diff_acc, rng=(25, 75), axis=1)
+        feat["diff_median"] = np.median(diff_acc, axis=1)
+
+        max_channel = np.zeros(diff_acc.shape)
+        max_channel[(diff_acc_x > diff_acc_y) & (diff_acc_x > diff_acc_z)] = 1
+        feat["x_diff_max_percentage"] = np.sum(max_channel, axis=1) / max_channel.shape[1]
+
+        max_channel = np.zeros(diff_acc.shape)
+        max_channel[(diff_acc_y > diff_acc_x) & (diff_acc_y > diff_acc_z)] = 1
+        feat["y_diff_max_percentage"] = np.sum(max_channel, axis=1) / max_channel.shape[1]
+
+        max_channel = np.zeros(diff_acc.shape)
+        max_channel[(diff_acc_z > diff_acc_x) & (diff_acc_z > diff_acc_y)] = 1
+        feat["z_diff_max_percentage"] = np.sum(max_channel, axis=1) / max_channel.shape[1]
+
+        return feat
+
+    def get_features(self):
+        if not hasattr(self, "feature_in_dataframe"):
+            self.fit()
+        return self.feature_in_dataframe.copy()
+
+    def bandpower_from_psd_ndarray(self, psd, freqs, relative=True):
+        """Compute bandpowers in N-dimensional PSD.
+
+        This is a NumPy-only implementation of the :py:func:`yasa.bandpower_from_psd` function,
+        which supports 1-D arrays of shape (n_freqs), or N-dimensional arays (e.g. 2-D (n_chan,
+        n_freqs) or 3-D (n_chan, n_epochs, n_freqs))
+
+        .. versionadded:: 0.2.0
+
+        Parameters
+        ----------
+        psd : :py:class:`numpy.ndarray`
+            Power spectral density of data, in uV^2/Hz. Must be a N-D array of shape (..., n_freqs).
+            See :py:func:`scipy.signal.welch` for more details.
+        freqs : :py:class:`numpy.ndarray`
+            Array of frequencies. Must be a 1-D array of shape (n_freqs,)
+        bands : list of tuples
+            List of frequency bands of interests. Each tuple must contain the lower and upper
+            frequencies, as well as the band name (e.g. (0.5, 4, 'Delta')).
+        relative : boolean
+            If True, bandpower is divided by the total power between the min and
+            max frequencies defined in ``band`` (default 0.5 to 40 Hz).
+
+        Returns
+        -------
+        bandpowers : :py:class:`numpy.ndarray`
+            Bandpower array of shape *(n_bands, ...)*.
+        """
+        # Type checks
+        assert isinstance(self.bands, list), "bands must be a list of tuple(s)"
+        assert isinstance(relative, bool), "relative must be a boolean"
+
+        # Safety checks
+        freqs = np.asarray(freqs)
+        psd = np.asarray(psd)
+        assert freqs.ndim == 1, "freqs must be a 1-D array of shape (n_freqs,)"
+        assert psd.shape[-1] == freqs.shape[-1], "n_freqs must be last axis of psd"
+
+        # Extract frequencies of interest
+        all_freqs = np.hstack([[b[0], b[1]] for b in self.bands])
+        fmin, fmax = min(all_freqs), max(all_freqs)
+        idx_good_freq = np.logical_and(freqs >= fmin, freqs <= fmax)
+        freqs = freqs[idx_good_freq]
+        res = freqs[1] - freqs[0]
+
+        # Trim PSD to frequencies of interest
+        psd = psd[..., idx_good_freq]
+
+        # plt.imshow(psd.T[:50,:], cmap='jet')
+        # plt.show()
+        # assert 0
+
+        # Check if there are negative values in PSD
+        if (psd < 0).any():
+            pass
+
+        # Calculate total power
+        total_power = simps(psd, dx=res, axis=-1)
+        total_power = total_power[np.newaxis, ...]
+
+        # Initialize empty array
+        bp = np.zeros((len(self.bands), *psd.shape[:-1]), dtype=np.float64)
+
+        # Enumerate over the frequency bands
+        labels = []
+        for i, band in enumerate(self.bands):
+            b0, b1, la = band
+            labels.append(la)
+            idx_band = np.logical_and(freqs >= b0, freqs <= b1)
+            bp[i] = simps(psd[..., idx_band], dx=res, axis=-1)
+
+        if relative:
+            bp /= total_power
+
+        all_freqs = all_freqs.reshape(-1, 2)
+        total_bands = all_freqs[:, 1] - all_freqs[:, 0]
+        total_bands = total_bands[..., np.newaxis]
+        bp /= total_bands
+        return bp
```

### Comparing `lm_datahandler-0.1.3/lm_datahandler/functions/sleep_staging.py` & `lm_datahandler-0.1.4/lm_datahandler/functions/sleep_staging.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import numpy as np
 import lightgbm as lgb
 import pandas as pd
 from lm_datahandler.postprocess.label_smooth import pp_label_smooth
 import os
 
 def sleep_staging_with_features(features, model_path, use_acc, use_time, context_mode=1):
-    clf = None
-    feature_for_predict = None
+
     if model_path is not None:
         clf = lgb.Booster(model_file=model_path)
     else:
         model_name = "sleep_staging.txt"
         if use_acc:
             model_name = 'acc_' + model_name
```

### Comparing `lm_datahandler-0.1.3/lm_datahandler/functions/sleep_variable_compute.py` & `lm_datahandler-0.1.4/lm_datahandler/functions/sleep_variable_compute.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.3/lm_datahandler/models/wholenight_sleep_staging.txt` & `lm_datahandler-0.1.4/lm_datahandler/models/wholenight_sleep_staging.txt`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.3/lm_datahandler/plots/biomarker_plot.py` & `lm_datahandler-0.1.4/lm_datahandler/plots/biomarker_plot.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.3/lm_datahandler/plots/sleep_staging_plot.py` & `lm_datahandler-0.1.4/lm_datahandler/plots/sleep_staging_plot.py`

 * *Files 11% similar despite different names*

```diff
@@ -61,14 +61,30 @@
     ax.tick_params(axis='y', labelsize=12)
     ax.tick_params(axis='x', labelsize=12)
     ax.set_ylabel("Avg Diff ACC", fontdict={"fontsize": 16})
     ax.set_xlabel("Time [hrs]", fontdict={"fontsize": 16})
     return fig, ax
 
 
+def plot_sleep_posture(fig, ax, grade, sf=50):
+    # assert grade.shape[0] == 1, "The grade of head bias should be a 1-D ndarray"
+    t = np.arange(grade.shape[0])/sf/3600
+    ax.plot(t, grade, lw=1.5, color='b')
+    ax.set_xlim(0, t.max())
+    ax.set_ylim(-3.5, 3.5)
+    ax.tick_params(axis='y', labelsize=12)
+    ax.tick_params(axis='x', labelsize=12)
+    ax.set_yticks([-np.pi, -np.pi/2, 0, np.pi/2, np.pi])
+    ax.set_yticklabels(['Sleep Face Down', 'Lie on the Left', 'Lie Flat', 'Lie on the Right', 'Sleep Face Down'], )
+    ax.set_ylabel("Sleep Postures", fontdict={"fontsize": 16})
+    ax.set_xlabel("Time [hrs]", fontdict={"fontsize": 16})
+    ax.grid(visible=True, axis='y', linewidth=0.5)
+    return fig, ax
+
+
 def plot_sleep_staging_result(fig, ax, hypno, sleep_variables, win=15):
     assert len(hypno.shape) == 1, "Hypno should be a 1-D array"
 
     t = np.arange(hypno.size) * win / 3600
     deep_sleep = np.ma.masked_not_equal(hypno, 0)
     light_sleep = np.ma.masked_not_equal(hypno, 1)
     rem_sleep = np.ma.masked_not_equal(hypno, 2)
```

### Comparing `lm_datahandler-0.1.3/lm_datahandler/postprocess/label_smooth.py` & `lm_datahandler-0.1.4/lm_datahandler/postprocess/label_smooth.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.3/lm_datahandler/utils/numba_func.py` & `lm_datahandler-0.1.4/lm_datahandler/utils/numba_func.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.3/lm_datahandler.egg-info/SOURCES.txt` & `lm_datahandler-0.1.4/lm_datahandler.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,21 +11,25 @@
 lm_datahandler/data_load/__init__.py
 lm_datahandler/data_load/data_loader.py
 lm_datahandler/data_load/loaders.py
 lm_datahandler/functions/__init__.py
 lm_datahandler/functions/biomarker.py
 lm_datahandler/functions/feature_extract.py
 lm_datahandler/functions/os_detect.py
+lm_datahandler/functions/posture_analyse.py
 lm_datahandler/functions/sleep_staging.py
 lm_datahandler/functions/sleep_variable_compute.py
 lm_datahandler/functions/spindle_detect.py
+lm_datahandler/functions/wear_detect.py
+lm_datahandler/models/wear_detection_1s.txt
 lm_datahandler/models/wholenight_sleep_staging.txt
 lm_datahandler/plots/__init__.py
 lm_datahandler/plots/biomarker_plot.py
 lm_datahandler/plots/sleep_staging_plot.py
+lm_datahandler/plots/stim_plot.py
 lm_datahandler/postprocess/__init__.py
 lm_datahandler/postprocess/label_smooth.py
 lm_datahandler/preprocess/__init__.py
 lm_datahandler/preprocess/filter.py
 lm_datahandler/preprocess/tailor.py
 lm_datahandler/utils/__init__.py
 lm_datahandler/utils/numba_func.py
```

### Comparing `lm_datahandler-0.1.3/setup.py` & `lm_datahandler-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'lm_datahandler',
-    version = '0.1.3',
+    version = '0.1.4',
     keywords='eeg sleep staging analysis',
     description = 'a python analyse tool for LM Data Recorder data',
     license = 'MIT License',
     url = 'https://github.com/zx950618/lm_datahandler',
     author = 'Eric Zheng',
     author_email = '1248471980@qq.com',
     packages = find_packages(),
```

