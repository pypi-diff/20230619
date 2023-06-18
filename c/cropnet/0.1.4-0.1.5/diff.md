# Comparing `tmp/cropnet-0.1.4.tar.gz` & `tmp/cropnet-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cropnet-0.1.4.tar", last modified: Sun Jun 18 21:41:47 2023, max compression
+gzip compressed data, was "cropnet-0.1.5.tar", last modified: Sun Jun 18 22:22:14 2023, max compression
```

## Comparing `cropnet-0.1.4.tar` & `cropnet-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 21:41:47.900168 cropnet-0.1.4/
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     4756 2023-06-18 21:41:47.900168 cropnet-0.1.4/PKG-INFO
--rw-r--r--   0 fudong    (1000) fudong    (1000)     4071 2023-06-18 21:41:32.000000 cropnet-0.1.4/README.md
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 21:41:47.900168 cropnet-0.1.4/cropnet/
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 21:41:47.900168 cropnet-0.1.4/cropnet/dataset/
--rw-rw-r--   0 fudong    (1000) fudong    (1000)       55 2023-06-17 22:41:39.000000 cropnet-0.1.4/cropnet/dataset/__init__.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     6251 2023-06-18 21:33:51.000000 cropnet-0.1.4/cropnet/dataset/hrrr_computed_dataset.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     1956 2023-06-17 22:36:51.000000 cropnet-0.1.4/cropnet/dataset/sentinel2_imagery.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     2433 2023-06-18 21:33:51.000000 cropnet-0.1.4/cropnet/dataset/usda_crop_dataset.py
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 21:41:47.900168 cropnet-0.1.4/cropnet.egg-info/
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     4756 2023-06-18 21:41:47.000000 cropnet-0.1.4/cropnet.egg-info/PKG-INFO
--rw-rw-r--   0 fudong    (1000) fudong    (1000)      315 2023-06-18 21:41:47.000000 cropnet-0.1.4/cropnet.egg-info/SOURCES.txt
--rw-rw-r--   0 fudong    (1000) fudong    (1000)        1 2023-06-18 21:41:47.000000 cropnet-0.1.4/cropnet.egg-info/dependency_links.txt
--rw-rw-r--   0 fudong    (1000) fudong    (1000)       64 2023-06-18 21:41:47.000000 cropnet-0.1.4/cropnet.egg-info/requires.txt
--rw-rw-r--   0 fudong    (1000) fudong    (1000)        8 2023-06-18 21:41:47.000000 cropnet-0.1.4/cropnet.egg-info/top_level.txt
--rw-rw-r--   0 fudong    (1000) fudong    (1000)       38 2023-06-18 21:41:47.900168 cropnet-0.1.4/setup.cfg
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     1191 2023-06-18 21:33:58.000000 cropnet-0.1.4/setup.py
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 22:22:14.205689 cropnet-0.1.5/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     4756 2023-06-18 22:22:14.205689 cropnet-0.1.5/PKG-INFO
+-rw-r--r--   0 fudong    (1000) fudong    (1000)     4071 2023-06-18 21:41:32.000000 cropnet-0.1.5/README.md
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 22:22:14.201689 cropnet-0.1.5/cropnet/
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 22:22:14.205689 cropnet-0.1.5/cropnet/dataset/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)       55 2023-06-18 22:22:05.000000 cropnet-0.1.5/cropnet/dataset/__init__.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     6251 2023-06-18 21:33:51.000000 cropnet-0.1.5/cropnet/dataset/hrrr_computed_dataset.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     1956 2023-06-17 22:36:51.000000 cropnet-0.1.5/cropnet/dataset/sentinel2_imagery.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     2433 2023-06-18 21:33:51.000000 cropnet-0.1.5/cropnet/dataset/usda_crop_dataset.py
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 22:22:14.205689 cropnet-0.1.5/cropnet.egg-info/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     4756 2023-06-18 22:22:14.000000 cropnet-0.1.5/cropnet.egg-info/PKG-INFO
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)      315 2023-06-18 22:22:14.000000 cropnet-0.1.5/cropnet.egg-info/SOURCES.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)        1 2023-06-18 22:22:14.000000 cropnet-0.1.5/cropnet.egg-info/dependency_links.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)       72 2023-06-18 22:22:14.000000 cropnet-0.1.5/cropnet.egg-info/requires.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)        8 2023-06-18 22:22:14.000000 cropnet-0.1.5/cropnet.egg-info/top_level.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)       38 2023-06-18 22:22:14.205689 cropnet-0.1.5/setup.cfg
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     1210 2023-06-18 22:21:35.000000 cropnet-0.1.5/setup.py
```

### Comparing `cropnet-0.1.4/PKG-INFO` & `cropnet-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cropnet
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package for the CropNet dataset
 Author: Anonymous AI4Science
 Author-email: anonymous.ai4science@gmail.com
 License: Free for non-commercial use
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
```

### Comparing `cropnet-0.1.4/README.md` & `cropnet-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.4/cropnet/dataset/hrrr_computed_dataset.py` & `cropnet-0.1.5/cropnet/dataset/hrrr_computed_dataset.py`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.4/cropnet/dataset/sentinel2_imagery.py` & `cropnet-0.1.5/cropnet/dataset/sentinel2_imagery.py`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.4/cropnet/dataset/usda_crop_dataset.py` & `cropnet-0.1.5/cropnet/dataset/usda_crop_dataset.py`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.4/cropnet.egg-info/PKG-INFO` & `cropnet-0.1.5/cropnet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cropnet
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package for the CropNet dataset
 Author: Anonymous AI4Science
 Author-email: anonymous.ai4science@gmail.com
 License: Free for non-commercial use
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
```

### Comparing `cropnet-0.1.4/setup.py` & `cropnet-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # read the contents of the README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cropnet',
-    version='0.1.4',
+    version='0.1.5',
     description='A Python package for the CropNet dataset',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Anonymous AI4Science',
     author_email='anonymous.ai4science@gmail.com',
     license='Free for non-commercial use',
     packages=['cropnet.dataset'],
@@ -20,14 +20,15 @@
         'numpy',
         'torchvision',
         'numpy',
         'pandas',
         'h5py',
         'Pillow',
         'einops',
+        'sklearn',
     ],
 
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
         'License :: Free for non-commercial use',
         'Operating System :: MacOS',
```

