# Comparing `tmp/upload_manager-1.0.0.tar.gz` & `tmp/upload_manager-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upload_manager-1.0.0.tar", last modified: Tue Nov  8 08:57:03 2022, max compression
+gzip compressed data, was "upload_manager-1.1.0.tar", last modified: Mon Jun 19 08:31:08 2023, max compression
```

## Comparing `upload_manager-1.0.0.tar` & `upload_manager-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2022-11-08 08:57:03.538402 upload_manager-1.0.0/
--rw-r--r--   0 dharmesh   (502) staff       (20)     1144 2021-02-10 09:04:07.000000 upload_manager-1.0.0/LICENSE.md
--rw-r--r--   0 dharmesh   (502) staff       (20)      114 2021-03-02 13:09:30.000000 upload_manager-1.0.0/MANIFEST.in
--rw-r--r--   0 dharmesh   (502) staff       (20)     2703 2022-11-08 08:57:03.538144 upload_manager-1.0.0/PKG-INFO
--rw-r--r--   0 dharmesh   (502) staff       (20)     2132 2021-03-02 13:17:30.000000 upload_manager-1.0.0/README.md
-drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2022-11-08 08:57:03.527039 upload_manager-1.0.0/images/
--rw-r--r--   0 dharmesh   (502) staff       (20)   200603 2021-03-02 12:37:59.000000 upload_manager-1.0.0/images/dashboard.png
--rw-rw-r--   0 dharmesh   (502) staff       (20)       67 2021-02-10 13:25:58.000000 upload_manager-1.0.0/requirements.txt
--rw-r--r--   0 dharmesh   (502) staff       (20)       38 2022-11-08 08:57:03.538481 upload_manager-1.0.0/setup.cfg
--rw-r--r--   0 dharmesh   (502) staff       (20)      981 2022-11-08 08:46:55.000000 upload_manager-1.0.0/setup.py
-drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2022-11-08 08:57:03.530177 upload_manager-1.0.0/tests/
--rw-r--r--   0 dharmesh   (502) staff       (20)        0 2021-02-10 06:21:51.000000 upload_manager-1.0.0/tests/__init__.py
--rw-r--r--   0 dharmesh   (502) staff       (20)      621 2021-02-10 13:58:22.000000 upload_manager-1.0.0/tests/test_s3.py
-drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2022-11-08 08:57:03.535602 upload_manager-1.0.0/upload_manager/
--rw-rw-r--   0 dharmesh   (502) staff       (20)        0 2020-08-07 09:11:53.000000 upload_manager-1.0.0/upload_manager/__init__.py
--rw-r--r--   0 dharmesh   (502) staff       (20)     1196 2022-11-04 06:16:29.000000 upload_manager-1.0.0/upload_manager/admin.py
--rw-rw-r--   0 dharmesh   (502) staff       (20)      138 2021-03-02 12:35:59.000000 upload_manager-1.0.0/upload_manager/apps.py
--rw-rw-r--   0 dharmesh   (502) staff       (20)      626 2020-08-07 09:11:53.000000 upload_manager-1.0.0/upload_manager/file_operator.py
-drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2022-11-08 08:57:03.537814 upload_manager-1.0.0/upload_manager/migrations/
--rw-rw-r--   0 dharmesh   (502) staff       (20)     1477 2020-08-07 09:11:53.000000 upload_manager-1.0.0/upload_manager/migrations/0001_initial.py
--rw-rw-r--   0 dharmesh   (502) staff       (20)        0 2020-08-07 09:11:53.000000 upload_manager-1.0.0/upload_manager/migrations/__init__.py
--rw-rw-r--   0 dharmesh   (502) staff       (20)     1527 2020-08-07 09:11:53.000000 upload_manager-1.0.0/upload_manager/models.py
--rw-rw-r--   0 dharmesh   (502) staff       (20)     4503 2021-02-01 17:23:37.000000 upload_manager-1.0.0/upload_manager/s3.py
--rw-rw-r--   0 dharmesh   (502) staff       (20)     6052 2021-03-01 11:28:31.000000 upload_manager-1.0.0/upload_manager/service.py
--rw-rw-r--   0 dharmesh   (502) staff       (20)      445 2020-08-07 09:11:53.000000 upload_manager-1.0.0/upload_manager/utils.py
-drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2022-11-08 08:57:03.537115 upload_manager-1.0.0/upload_manager.egg-info/
--rw-r--r--   0 dharmesh   (502) staff       (20)     2703 2022-11-08 08:57:03.000000 upload_manager-1.0.0/upload_manager.egg-info/PKG-INFO
--rw-r--r--   0 dharmesh   (502) staff       (20)      585 2022-11-08 08:57:03.000000 upload_manager-1.0.0/upload_manager.egg-info/SOURCES.txt
--rw-r--r--   0 dharmesh   (502) staff       (20)        1 2022-11-08 08:57:03.000000 upload_manager-1.0.0/upload_manager.egg-info/dependency_links.txt
--rw-r--r--   0 dharmesh   (502) staff       (20)       67 2022-11-08 08:57:03.000000 upload_manager-1.0.0/upload_manager.egg-info/requires.txt
--rw-r--r--   0 dharmesh   (502) staff       (20)       21 2022-11-08 08:57:03.000000 upload_manager-1.0.0/upload_manager.egg-info/top_level.txt
+drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2023-06-19 08:31:08.866213 upload_manager-1.1.0/
+-rw-r--r--   0 dharmesh   (502) staff       (20)     1144 2021-02-10 09:04:07.000000 upload_manager-1.1.0/LICENSE.md
+-rw-r--r--   0 dharmesh   (502) staff       (20)      114 2021-03-02 13:09:30.000000 upload_manager-1.1.0/MANIFEST.in
+-rw-r--r--   0 dharmesh   (502) staff       (20)     2703 2023-06-19 08:31:08.865967 upload_manager-1.1.0/PKG-INFO
+-rw-r--r--   0 dharmesh   (502) staff       (20)     2132 2021-03-02 13:17:30.000000 upload_manager-1.1.0/README.md
+drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2023-06-19 08:31:08.856236 upload_manager-1.1.0/images/
+-rw-r--r--   0 dharmesh   (502) staff       (20)   200603 2021-03-02 12:37:59.000000 upload_manager-1.1.0/images/dashboard.png
+-rw-rw-r--   0 dharmesh   (502) staff       (20)       67 2021-02-10 13:25:58.000000 upload_manager-1.1.0/requirements.txt
+-rw-r--r--   0 dharmesh   (502) staff       (20)       38 2023-06-19 08:31:08.866282 upload_manager-1.1.0/setup.cfg
+-rw-r--r--   0 dharmesh   (502) staff       (20)      981 2023-06-19 08:30:35.000000 upload_manager-1.1.0/setup.py
+drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2023-06-19 08:31:08.858377 upload_manager-1.1.0/tests/
+-rw-r--r--   0 dharmesh   (502) staff       (20)        0 2021-02-10 06:21:51.000000 upload_manager-1.1.0/tests/__init__.py
+-rw-r--r--   0 dharmesh   (502) staff       (20)      621 2021-02-10 13:58:22.000000 upload_manager-1.1.0/tests/test_s3.py
+drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2023-06-19 08:31:08.863682 upload_manager-1.1.0/upload_manager/
+-rw-rw-r--   0 dharmesh   (502) staff       (20)        0 2020-08-07 09:11:53.000000 upload_manager-1.1.0/upload_manager/__init__.py
+-rw-r--r--   0 dharmesh   (502) staff       (20)     1196 2022-11-04 06:16:29.000000 upload_manager-1.1.0/upload_manager/admin.py
+-rw-rw-r--   0 dharmesh   (502) staff       (20)      138 2021-03-02 12:35:59.000000 upload_manager-1.1.0/upload_manager/apps.py
+-rw-rw-r--   0 dharmesh   (502) staff       (20)      626 2020-08-07 09:11:53.000000 upload_manager-1.1.0/upload_manager/file_operator.py
+drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2023-06-19 08:31:08.865697 upload_manager-1.1.0/upload_manager/migrations/
+-rw-rw-r--   0 dharmesh   (502) staff       (20)     1477 2020-08-07 09:11:53.000000 upload_manager-1.1.0/upload_manager/migrations/0001_initial.py
+-rw-rw-r--   0 dharmesh   (502) staff       (20)        0 2020-08-07 09:11:53.000000 upload_manager-1.1.0/upload_manager/migrations/__init__.py
+-rw-rw-r--   0 dharmesh   (502) staff       (20)     1527 2020-08-07 09:11:53.000000 upload_manager-1.1.0/upload_manager/models.py
+-rw-rw-r--   0 dharmesh   (502) staff       (20)     4503 2021-02-01 17:23:37.000000 upload_manager-1.1.0/upload_manager/s3.py
+-rw-rw-r--   0 dharmesh   (502) staff       (20)     6052 2021-03-01 11:28:31.000000 upload_manager-1.1.0/upload_manager/service.py
+-rw-r--r--   0 dharmesh   (502) staff       (20)      169 2023-06-19 07:21:57.000000 upload_manager-1.1.0/upload_manager/urls.py
+-rw-rw-r--   0 dharmesh   (502) staff       (20)      445 2020-08-07 09:11:53.000000 upload_manager-1.1.0/upload_manager/utils.py
+-rw-r--r--   0 dharmesh   (502) staff       (20)     1747 2023-06-19 07:21:57.000000 upload_manager-1.1.0/upload_manager/views.py
+drwxr-xr-x   0 dharmesh   (502) staff       (20)        0 2023-06-19 08:31:08.865092 upload_manager-1.1.0/upload_manager.egg-info/
+-rw-r--r--   0 dharmesh   (502) staff       (20)     2703 2023-06-19 08:31:08.000000 upload_manager-1.1.0/upload_manager.egg-info/PKG-INFO
+-rw-r--r--   0 dharmesh   (502) staff       (20)      632 2023-06-19 08:31:08.000000 upload_manager-1.1.0/upload_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 dharmesh   (502) staff       (20)        1 2023-06-19 08:31:08.000000 upload_manager-1.1.0/upload_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 dharmesh   (502) staff       (20)       67 2023-06-19 08:31:08.000000 upload_manager-1.1.0/upload_manager.egg-info/requires.txt
+-rw-r--r--   0 dharmesh   (502) staff       (20)       21 2023-06-19 08:31:08.000000 upload_manager-1.1.0/upload_manager.egg-info/top_level.txt
```

### Comparing `upload_manager-1.0.0/LICENSE.md` & `upload_manager-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `upload_manager-1.0.0/PKG-INFO` & `upload_manager-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upload_manager
-Version: 1.0.0
+Version: 1.1.0
 Summary: Upload manager
 Home-page: https://github.com/Bigbasket/bbuploadmanager
 Author: bb-tech
 Author-email: asodiyadharmesh@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `upload_manager-1.0.0/README.md` & `upload_manager-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `upload_manager-1.0.0/images/dashboard.png` & `upload_manager-1.1.0/images/dashboard.png`

 * *Files identical despite different names*

### Comparing `upload_manager-1.0.0/setup.py` & `upload_manager-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 with open('requirements.txt') as infile:
     requirements = infile.read().splitlines()
 
 setuptools.setup(
     name="upload_manager",
-    version="1.0.0",
+    version="1.1.0",
     author="bb-tech",
     author_email="asodiyadharmesh@gmail.com",
     description="Upload manager",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/Bigbasket/bbuploadmanager",
     include_package_data=True,
```

### Comparing `upload_manager-1.0.0/tests/test_s3.py` & `upload_manager-1.1.0/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `upload_manager-1.0.0/upload_manager/admin.py` & `upload_manager-1.1.0/upload_manager/admin.py`

 * *Files identical despite different names*

### Comparing `upload_manager-1.0.0/upload_manager/file_operator.py` & `upload_manager-1.1.0/upload_manager/file_operator.py`

 * *Files identical despite different names*

### Comparing `upload_manager-1.0.0/upload_manager/migrations/0001_initial.py` & `upload_manager-1.1.0/upload_manager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `upload_manager-1.0.0/upload_manager/models.py` & `upload_manager-1.1.0/upload_manager/models.py`

 * *Files identical despite different names*

### Comparing `upload_manager-1.0.0/upload_manager/s3.py` & `upload_manager-1.1.0/upload_manager/s3.py`

 * *Files identical despite different names*

### Comparing `upload_manager-1.0.0/upload_manager/service.py` & `upload_manager-1.1.0/upload_manager/service.py`

 * *Files identical despite different names*

### Comparing `upload_manager-1.0.0/upload_manager.egg-info/PKG-INFO` & `upload_manager-1.1.0/upload_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upload-manager
-Version: 1.0.0
+Version: 1.1.0
 Summary: Upload manager
 Home-page: https://github.com/Bigbasket/bbuploadmanager
 Author: bb-tech
 Author-email: asodiyadharmesh@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `upload_manager-1.0.0/upload_manager.egg-info/SOURCES.txt` & `upload_manager-1.1.0/upload_manager.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 upload_manager/__init__.py
 upload_manager/admin.py
 upload_manager/apps.py
 upload_manager/file_operator.py
 upload_manager/models.py
 upload_manager/s3.py
 upload_manager/service.py
+upload_manager/urls.py
 upload_manager/utils.py
+upload_manager/views.py
 upload_manager.egg-info/PKG-INFO
 upload_manager.egg-info/SOURCES.txt
 upload_manager.egg-info/dependency_links.txt
 upload_manager.egg-info/requires.txt
 upload_manager.egg-info/top_level.txt
 upload_manager/migrations/0001_initial.py
 upload_manager/migrations/__init__.py
```

