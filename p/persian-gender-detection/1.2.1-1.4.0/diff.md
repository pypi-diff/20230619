# Comparing `tmp/persian-gender-detection-1.2.1.tar.gz` & `tmp/persian-gender-detection-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "persian-gender-detection-1.2.1.tar", last modified: Wed Jun 14 22:39:38 2023, max compression
+gzip compressed data, was "persian-gender-detection-1.4.0.tar", last modified: Mon Jun 19 07:25:44 2023, max compression
```

## Comparing `persian-gender-detection-1.2.1.tar` & `persian-gender-detection-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-14 22:39:38.566149 persian-gender-detection-1.2.1/
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1068 2023-06-07 16:19:28.000000 persian-gender-detection-1.2.1/LICENSE
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     2890 2023-06-14 22:39:38.566149 persian-gender-detection-1.2.1/PKG-INFO
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1571 2023-06-14 22:38:45.000000 persian-gender-detection-1.2.1/README.md
-drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-14 22:39:38.562149 persian-gender-detection-1.2.1/persian_gender_detection/
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       40 2023-06-07 16:13:42.000000 persian-gender-detection-1.2.1/persian_gender_detection/__init__.py
-drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-14 22:39:38.562149 persian-gender-detection-1.2.1/persian_gender_detection/gender/
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)   410371 2023-06-08 06:15:17.000000 persian-gender-detection-1.2.1/persian_gender_detection/gender/iranianNamesDataset.csv
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)   436494 2023-06-12 09:12:51.000000 persian-gender-detection-1.2.1/persian_gender_detection/gender/iranianNamesDataset.py
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1108 2023-06-14 22:31:58.000000 persian-gender-detection-1.2.1/persian_gender_detection/persian_gender_detection.py
-drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-14 22:39:38.562149 persian-gender-detection-1.2.1/persian_gender_detection.egg-info/
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     2890 2023-06-14 22:39:38.000000 persian-gender-detection-1.2.1/persian_gender_detection.egg-info/PKG-INFO
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)      467 2023-06-14 22:39:38.000000 persian-gender-detection-1.2.1/persian_gender_detection.egg-info/SOURCES.txt
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)        1 2023-06-14 22:39:38.000000 persian-gender-detection-1.2.1/persian_gender_detection.egg-info/dependency_links.txt
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       25 2023-06-14 22:39:38.000000 persian-gender-detection-1.2.1/persian_gender_detection.egg-info/top_level.txt
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       38 2023-06-14 22:39:38.566149 persian-gender-detection-1.2.1/setup.cfg
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1732 2023-06-14 22:33:09.000000 persian-gender-detection-1.2.1/setup.py
-drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-14 22:39:38.566149 persian-gender-detection-1.2.1/test/
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1438 2023-06-07 16:03:13.000000 persian-gender-detection-1.2.1/test/test_clean_name.py
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     2119 2023-06-14 22:37:51.000000 persian-gender-detection-1.2.1/test/test_get_gender.py
+drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-19 07:25:44.228789 persian-gender-detection-1.4.0/
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1068 2023-06-07 16:19:28.000000 persian-gender-detection-1.4.0/LICENSE
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     3683 2023-06-19 07:25:44.224789 persian-gender-detection-1.4.0/PKG-INFO
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     2564 2023-06-19 07:22:25.000000 persian-gender-detection-1.4.0/README.md
+drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-19 07:25:44.220789 persian-gender-detection-1.4.0/persian_gender_detection/
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       40 2023-06-07 16:13:42.000000 persian-gender-detection-1.4.0/persian_gender_detection/__init__.py
+drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-19 07:25:44.224789 persian-gender-detection-1.4.0/persian_gender_detection/gender/
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)   410371 2023-06-08 06:15:17.000000 persian-gender-detection-1.4.0/persian_gender_detection/gender/iranianNamesDataset.csv
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)   436494 2023-06-19 06:03:49.000000 persian-gender-detection-1.4.0/persian_gender_detection/gender/iranian_names_dataset.py
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1076 2023-06-19 06:03:49.000000 persian-gender-detection-1.4.0/persian_gender_detection/persian_gender_detection.py
+drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-19 07:25:44.224789 persian-gender-detection-1.4.0/persian_gender_detection.egg-info/
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     3683 2023-06-19 07:25:44.000000 persian-gender-detection-1.4.0/persian_gender_detection.egg-info/PKG-INFO
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)      469 2023-06-19 07:25:44.000000 persian-gender-detection-1.4.0/persian_gender_detection.egg-info/SOURCES.txt
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)        1 2023-06-19 07:25:44.000000 persian-gender-detection-1.4.0/persian_gender_detection.egg-info/dependency_links.txt
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       25 2023-06-19 07:25:44.000000 persian-gender-detection-1.4.0/persian_gender_detection.egg-info/top_level.txt
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       38 2023-06-19 07:25:44.228789 persian-gender-detection-1.4.0/setup.cfg
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1538 2023-06-19 07:25:34.000000 persian-gender-detection-1.4.0/setup.py
+drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-19 07:25:44.224789 persian-gender-detection-1.4.0/test/
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)      919 2023-06-19 06:03:49.000000 persian-gender-detection-1.4.0/test/test_clean_name.py
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     2266 2023-06-19 06:03:49.000000 persian-gender-detection-1.4.0/test/test_get_gender.py
```

### Comparing `persian-gender-detection-1.2.1/LICENSE` & `persian-gender-detection-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `persian-gender-detection-1.2.1/persian_gender_detection/gender/iranianNamesDataset.csv` & `persian-gender-detection-1.4.0/persian_gender_detection/gender/iranianNamesDataset.csv`

 * *Files identical despite different names*

### Comparing `persian-gender-detection-1.2.1/persian_gender_detection/gender/iranianNamesDataset.py` & `persian-gender-detection-1.4.0/persian_gender_detection/gender/iranian_names_dataset.py`

 * *Files identical despite different names*

