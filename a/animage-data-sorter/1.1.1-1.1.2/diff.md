# Comparing `tmp/animage-data_sorter-1.1.1.tar.gz` & `tmp/animage-data_sorter-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\animage-data_sorter-1.1.1.tar", last modified: Wed Jun  7 06:43:29 2023, max compression
+gzip compressed data, was "dist\animage-data_sorter-1.1.2.tar", last modified: Mon Jun 19 08:42:44 2023, max compression
```

## Comparing `animage-data_sorter-1.1.1.tar` & `animage-data_sorter-1.1.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 06:43:29.000000 animage-data_sorter-1.1.1/
--rw-rw-rw-   0        0        0     1363 2023-06-07 06:43:29.000000 animage-data_sorter-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      976 2023-05-11 05:19:09.000000 animage-data_sorter-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 06:43:29.000000 animage-data_sorter-1.1.1/animage_data_sorter.egg-info/
--rw-rw-rw-   0        0        0     1363 2023-06-07 06:43:29.000000 animage-data_sorter-1.1.1/animage_data_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1347 2023-06-07 06:43:29.000000 animage-data_sorter-1.1.1/animage_data_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 06:43:29.000000 animage-data_sorter-1.1.1/animage_data_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-07 06:43:29.000000 animage-data_sorter-1.1.1/animage_data_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 06:43:29.000000 animage-data_sorter-1.1.1/data_sorter/
--rw-rw-rw-   0        0        0      630 2023-05-31 06:58:45.000000 animage-data_sorter-1.1.1/data_sorter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:43:29.000000 animage-data_sorter-1.1.1/data_sorter/old/
--rw-rw-rw-   0        0        0    23325 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.1/data_sorter/old/AnImageASLUtility.py
--rw-rw-rw-   0        0        0     7768 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.1/data_sorter/old/AnImageDCMUtility.py
--rw-rw-rw-   0        0        0    26840 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.1/data_sorter/old/AnImageDataSorter.py
--rw-rw-rw-   0        0        0     9852 2023-02-08 06:54:39.000000 animage-data_sorter-1.1.1/data_sorter/old/AnImageDataSorterGEeASL7.py
--rw-rw-rw-   0        0        0     9373 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.1/data_sorter/old/AnImageDataSorterGEpCASL13.py
--rw-rw-rw-   0        0        0     4348 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.1/data_sorter/old/AnImageDataSorterMISC.py
--rw-rw-rw-   0        0        0     5901 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.1/data_sorter/old/AnImageDataSorterPhilips13.py
--rw-rw-rw-   0        0        0    13115 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.1/data_sorter/old/AnImageDataSorterSiemens4.py
--rw-rw-rw-   0        0        0    12711 2022-11-17 03:53:33.000000 animage-data_sorter-1.1.1/data_sorter/old/AnImageDataSorterSiemens5.py
--rw-rw-rw-   0        0        0    12032 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.1/data_sorter/old/AnImageDataSorterSiemensPASL.py
--rw-rw-rw-   0        0        0    21838 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.1/data_sorter/old/AnImageDataSorterSiemens_UCLA.py
--rw-rw-rw-   0        0        0    11395 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.1/data_sorter/old/AnImageDataSorterUtility.py
--rw-rw-rw-   0        0        0        0 2023-05-31 06:57:47.000000 animage-data_sorter-1.1.1/data_sorter/old/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:43:29.000000 animage-data_sorter-1.1.1/data_sorter/restructure/
--rw-rw-rw-   0        0        0     5204 2023-05-16 02:45:03.000000 animage-data_sorter-1.1.1/data_sorter/restructure/__init__.py
--rw-rw-rw-   0        0        0    36867 2023-06-07 06:32:18.000000 animage-data_sorter-1.1.1/data_sorter/restructure/_dicom.py
--rw-rw-rw-   0        0        0     9885 2023-05-16 02:58:30.000000 animage-data_sorter-1.1.1/data_sorter/restructure/_dicom_util.py
--rw-rw-rw-   0        0        0     3833 2023-05-16 01:45:10.000000 animage-data_sorter-1.1.1/data_sorter/restructure/_type.py
--rw-rw-rw-   0        0        0     4279 2023-05-29 05:21:20.000000 animage-data_sorter-1.1.1/data_sorter/restructure/data_sorter_base.py
--rw-rw-rw-   0        0        0     7621 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.1/data_sorter/restructure/dcm2nifti.py
--rw-rw-rw-   0        0        0     3515 2023-05-17 05:44:59.000000 animage-data_sorter-1.1.1/data_sorter/restructure/errors.py
--rw-rw-rw-   0        0        0     5737 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.1/data_sorter/restructure/ge_3d_pcasl.py
--rw-rw-rw-   0        0        0     8516 2023-05-29 05:23:17.000000 animage-data_sorter-1.1.1/data_sorter/restructure/ge_easl.py
--rw-rw-rw-   0        0        0    10501 2023-06-02 03:26:56.000000 animage-data_sorter-1.1.1/data_sorter/restructure/noASL_MRI.py
--rw-rw-rw-   0        0        0     4431 2023-05-30 02:25:25.000000 animage-data_sorter-1.1.1/data_sorter/restructure/philips_3d_pcasl.py
--rw-rw-rw-   0        0        0     6769 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.1/data_sorter/restructure/siemens_3d_pasl.py
--rw-rw-rw-   0        0        0     7951 2023-05-31 02:53:56.000000 animage-data_sorter-1.1.1/data_sorter/restructure/siemens_3d_pcasl.py
--rw-rw-rw-   0        0        0     8366 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.1/data_sorter/restructure/siemens_3d_pcasl_old.py
--rw-rw-rw-   0        0        0     4421 2023-05-16 01:48:06.000000 animage-data_sorter-1.1.1/data_sorter/restructure/uih_3d_pasl.py
--rw-rw-rw-   0        0        0       42 2023-06-07 06:43:29.000000 animage-data_sorter-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      602 2023-06-07 06:43:16.000000 animage-data_sorter-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/
+-rw-rw-rw-   0        0        0     1363 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      976 2023-05-11 05:19:09.000000 animage-data_sorter-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/animage_data_sorter.egg-info/
+-rw-rw-rw-   0        0        0     1363 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/animage_data_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1347 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/animage_data_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/animage_data_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/animage_data_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/data_sorter/
+-rw-rw-rw-   0        0        0      630 2023-05-31 06:58:45.000000 animage-data_sorter-1.1.2/data_sorter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/data_sorter/old/
+-rw-rw-rw-   0        0        0    23325 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageASLUtility.py
+-rw-rw-rw-   0        0        0     7768 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDCMUtility.py
+-rw-rw-rw-   0        0        0    26840 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorter.py
+-rw-rw-rw-   0        0        0     9852 2023-02-08 06:54:39.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterGEeASL7.py
+-rw-rw-rw-   0        0        0     9373 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterGEpCASL13.py
+-rw-rw-rw-   0        0        0     4348 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterMISC.py
+-rw-rw-rw-   0        0        0     5901 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterPhilips13.py
+-rw-rw-rw-   0        0        0    13115 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterSiemens4.py
+-rw-rw-rw-   0        0        0    12711 2022-11-17 03:53:33.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterSiemens5.py
+-rw-rw-rw-   0        0        0    12032 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterSiemensPASL.py
+-rw-rw-rw-   0        0        0    21838 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterSiemens_UCLA.py
+-rw-rw-rw-   0        0        0    11395 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterUtility.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 06:57:47.000000 animage-data_sorter-1.1.2/data_sorter/old/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/data_sorter/restructure/
+-rw-rw-rw-   0        0        0     5204 2023-05-16 02:45:03.000000 animage-data_sorter-1.1.2/data_sorter/restructure/__init__.py
+-rw-rw-rw-   0        0        0    36867 2023-06-07 06:32:18.000000 animage-data_sorter-1.1.2/data_sorter/restructure/_dicom.py
+-rw-rw-rw-   0        0        0     9885 2023-05-16 02:58:30.000000 animage-data_sorter-1.1.2/data_sorter/restructure/_dicom_util.py
+-rw-rw-rw-   0        0        0     3833 2023-05-16 01:45:10.000000 animage-data_sorter-1.1.2/data_sorter/restructure/_type.py
+-rw-rw-rw-   0        0        0     4279 2023-05-29 05:21:20.000000 animage-data_sorter-1.1.2/data_sorter/restructure/data_sorter_base.py
+-rw-rw-rw-   0        0        0     7621 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.2/data_sorter/restructure/dcm2nifti.py
+-rw-rw-rw-   0        0        0     3515 2023-05-17 05:44:59.000000 animage-data_sorter-1.1.2/data_sorter/restructure/errors.py
+-rw-rw-rw-   0        0        0     5737 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.2/data_sorter/restructure/ge_3d_pcasl.py
+-rw-rw-rw-   0        0        0     8516 2023-05-29 05:23:17.000000 animage-data_sorter-1.1.2/data_sorter/restructure/ge_easl.py
+-rw-rw-rw-   0        0        0    10444 2023-06-19 06:06:18.000000 animage-data_sorter-1.1.2/data_sorter/restructure/noASL_MRI.py
+-rw-rw-rw-   0        0        0     4431 2023-06-07 08:39:25.000000 animage-data_sorter-1.1.2/data_sorter/restructure/philips_3d_pcasl.py
+-rw-rw-rw-   0        0        0     6769 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.2/data_sorter/restructure/siemens_3d_pasl.py
+-rw-rw-rw-   0        0        0     7951 2023-05-31 02:53:56.000000 animage-data_sorter-1.1.2/data_sorter/restructure/siemens_3d_pcasl.py
+-rw-rw-rw-   0        0        0     8366 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.2/data_sorter/restructure/siemens_3d_pcasl_old.py
+-rw-rw-rw-   0        0        0     4421 2023-05-16 01:48:06.000000 animage-data_sorter-1.1.2/data_sorter/restructure/uih_3d_pasl.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 08:42:44.000000 animage-data_sorter-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      602 2023-06-19 08:40:59.000000 animage-data_sorter-1.1.2/setup.py
```

### Comparing `animage-data_sorter-1.1.1/PKG-INFO` & `animage-data_sorter-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animage-data_sorter
-Version: 1.1.1
+Version: 1.1.2
 Summary: dicom sort
 Home-page: https://gitee.com/AnImage-Beijing/data_sorter
 Author: zhaomy
 Author-email: zhaomy@an-image.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `animage-data_sorter-1.1.1/README.md` & `animage-data_sorter-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/animage_data_sorter.egg-info/PKG-INFO` & `animage-data_sorter-1.1.2/animage_data_sorter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animage-data-sorter
-Version: 1.1.1
+Version: 1.1.2
 Summary: dicom sort
 Home-page: https://gitee.com/AnImage-Beijing/data_sorter
 Author: zhaomy
 Author-email: zhaomy@an-image.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `animage-data_sorter-1.1.1/animage_data_sorter.egg-info/SOURCES.txt` & `animage-data_sorter-1.1.2/animage_data_sorter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/__init__.py` & `animage-data_sorter-1.1.2/data_sorter/__init__.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/old/AnImageASLUtility.py` & `animage-data_sorter-1.1.2/data_sorter/old/AnImageASLUtility.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/old/AnImageDCMUtility.py` & `animage-data_sorter-1.1.2/data_sorter/old/AnImageDCMUtility.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/old/AnImageDataSorter.py` & `animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorter.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/old/AnImageDataSorterGEeASL7.py` & `animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterGEeASL7.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/old/AnImageDataSorterGEpCASL13.py` & `animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterGEpCASL13.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/old/AnImageDataSorterMISC.py` & `animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterMISC.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/old/AnImageDataSorterPhilips13.py` & `animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterPhilips13.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/old/AnImageDataSorterSiemens4.py` & `animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterSiemens4.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/old/AnImageDataSorterSiemens5.py` & `animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterSiemens5.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/old/AnImageDataSorterSiemensPASL.py` & `animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterSiemensPASL.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/old/AnImageDataSorterSiemens_UCLA.py` & `animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterSiemens_UCLA.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/old/AnImageDataSorterUtility.py` & `animage-data_sorter-1.1.2/data_sorter/old/AnImageDataSorterUtility.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/restructure/__init__.py` & `animage-data_sorter-1.1.2/data_sorter/restructure/__init__.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/restructure/_dicom.py` & `animage-data_sorter-1.1.2/data_sorter/restructure/_dicom.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/restructure/_dicom_util.py` & `animage-data_sorter-1.1.2/data_sorter/restructure/_dicom_util.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/restructure/_type.py` & `animage-data_sorter-1.1.2/data_sorter/restructure/_type.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/restructure/data_sorter_base.py` & `animage-data_sorter-1.1.2/data_sorter/restructure/data_sorter_base.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/restructure/dcm2nifti.py` & `animage-data_sorter-1.1.2/data_sorter/restructure/dcm2nifti.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/restructure/errors.py` & `animage-data_sorter-1.1.2/data_sorter/restructure/errors.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/restructure/ge_3d_pcasl.py` & `animage-data_sorter-1.1.2/data_sorter/restructure/ge_3d_pcasl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/restructure/ge_easl.py` & `animage-data_sorter-1.1.2/data_sorter/restructure/ge_easl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/restructure/noASL_MRI.py` & `animage-data_sorter-1.1.2/data_sorter/restructure/noASL_MRI.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,24 +114,22 @@
         self.series_list = self.DWI_list + self.ADC_list
 
     def validate_series(self):
         if len(self.DWI_list) < 1:
             raise MissingSequenceError('DWI')
         elif len(self.DWI_list) > 1:
             logger.warning(f'发现{len(self.DWI_list)}组DWI数据')
-        else:
-            self.DWI = self.DWI_list[0]
+        self.DWI = self.DWI_list[0]
 
         if len(self.ADC_list) < 1:
             logger.warning(f'未发现ADC序列')
             self.ADC: SeriesModel = None
             # raise MissingSequenceError('ADC')
-        elif len(self.ADC_list) > 1:
-            logger.warning(f'发现{len(self.DWI_list)}组ADC数据')
         else:
+            logger.warning(f'发现{len(self.DWI_list)}组ADC数据')
             self.ADC = self.ADC_list[0]
 
         if self.ADC is not None and self.DWI.SliceNumber != self.ADC.SliceNumber:
             raise SpaceIsDifferentError('DWI', 'ADC')
         if self.ADC is not None and (self.DWI.Repetition != 2 or self.ADC.Repetition != 1):
             raise SliceLessError(self.ADC.SliceNumber)
```

### Comparing `animage-data_sorter-1.1.1/data_sorter/restructure/philips_3d_pcasl.py` & `animage-data_sorter-1.1.2/data_sorter/restructure/philips_3d_pcasl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/restructure/siemens_3d_pasl.py` & `animage-data_sorter-1.1.2/data_sorter/restructure/siemens_3d_pasl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/restructure/siemens_3d_pcasl.py` & `animage-data_sorter-1.1.2/data_sorter/restructure/siemens_3d_pcasl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/restructure/siemens_3d_pcasl_old.py` & `animage-data_sorter-1.1.2/data_sorter/restructure/siemens_3d_pcasl_old.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/data_sorter/restructure/uih_3d_pasl.py` & `animage-data_sorter-1.1.2/data_sorter/restructure/uih_3d_pasl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.1/setup.py` & `animage-data_sorter-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="animage-data_sorter",
-  version="1.1.1",
+  version="1.1.2",
   author="zhaomy",
   author_email="zhaomy@an-image.cn",
   description="dicom sort",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://gitee.com/AnImage-Beijing/data_sorter",
   packages=setuptools.find_packages(),
```

