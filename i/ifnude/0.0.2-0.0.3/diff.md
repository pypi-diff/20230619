# Comparing `tmp/ifnude-0.0.2.tar.gz` & `tmp/ifnude-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifnude-0.0.2.tar", last modified: Sun Jun 18 21:57:02 2023, max compression
+gzip compressed data, was "ifnude-0.0.3.tar", last modified: Sun Jun 18 22:34:44 2023, max compression
```

## Comparing `ifnude-0.0.2.tar` & `ifnude-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2023-06-18 21:57:02.845304 ifnude-0.0.2/
--rw-r--r--   0 d3v       (1000) d3v       (1000)     1067 2023-06-18 21:56:34.000000 ifnude-0.0.2/LICENSE.md
--rw-r--r--   0 d3v       (1000) d3v       (1000)     1561 2023-06-18 21:57:02.845304 ifnude-0.0.2/PKG-INFO
--rw-r--r--   0 d3v       (1000) d3v       (1000)      899 2023-06-18 21:56:34.000000 ifnude-0.0.2/README.md
-drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2023-06-18 21:57:02.845304 ifnude-0.0.2/ifnude/
--rw-r--r--   0 d3v       (1000) d3v       (1000)       29 2023-06-18 21:56:34.000000 ifnude-0.0.2/ifnude/__init__.py
--rw-r--r--   0 d3v       (1000) d3v       (1000)     3319 2023-06-18 21:56:34.000000 ifnude-0.0.2/ifnude/detector.py
--rw-r--r--   0 d3v       (1000) d3v       (1000)     1607 2023-06-18 21:56:34.000000 ifnude-0.0.2/ifnude/detector_utils.py
--rw-r--r--   0 d3v       (1000) d3v       (1000)     5240 2023-06-18 21:56:34.000000 ifnude-0.0.2/ifnude/image_utils.py
-drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2023-06-18 21:57:02.845304 ifnude-0.0.2/ifnude.egg-info/
--rw-r--r--   0 d3v       (1000) d3v       (1000)     1561 2023-06-18 21:57:02.000000 ifnude-0.0.2/ifnude.egg-info/PKG-INFO
--rw-r--r--   0 d3v       (1000) d3v       (1000)      263 2023-06-18 21:57:02.000000 ifnude-0.0.2/ifnude.egg-info/SOURCES.txt
--rw-r--r--   0 d3v       (1000) d3v       (1000)        1 2023-06-18 21:57:02.000000 ifnude-0.0.2/ifnude.egg-info/dependency_links.txt
--rw-r--r--   0 d3v       (1000) d3v       (1000)       70 2023-06-18 21:57:02.000000 ifnude-0.0.2/ifnude.egg-info/requires.txt
--rw-r--r--   0 d3v       (1000) d3v       (1000)        7 2023-06-18 21:57:02.000000 ifnude-0.0.2/ifnude.egg-info/top_level.txt
--rw-r--r--   0 d3v       (1000) d3v       (1000)       38 2023-06-18 21:57:02.845304 ifnude-0.0.2/setup.cfg
--rw-r--r--   0 d3v       (1000) d3v       (1000)     2633 2023-06-18 21:56:34.000000 ifnude-0.0.2/setup.py
+drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2023-06-18 22:34:44.186013 ifnude-0.0.3/
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     1067 2023-06-18 21:56:34.000000 ifnude-0.0.3/LICENSE.md
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     1561 2023-06-18 22:34:44.186013 ifnude-0.0.3/PKG-INFO
+-rw-r--r--   0 d3v       (1000) d3v       (1000)      899 2023-06-18 21:56:34.000000 ifnude-0.0.3/README.md
+drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2023-06-18 22:34:44.186013 ifnude-0.0.3/ifnude/
+-rw-r--r--   0 d3v       (1000) d3v       (1000)       29 2023-06-18 21:56:34.000000 ifnude-0.0.3/ifnude/__init__.py
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     3336 2023-06-18 22:34:15.000000 ifnude-0.0.3/ifnude/detector.py
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     1607 2023-06-18 21:56:34.000000 ifnude-0.0.3/ifnude/detector_utils.py
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     5240 2023-06-18 21:56:34.000000 ifnude-0.0.3/ifnude/image_utils.py
+drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2023-06-18 22:34:44.186013 ifnude-0.0.3/ifnude.egg-info/
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     1561 2023-06-18 22:34:44.000000 ifnude-0.0.3/ifnude.egg-info/PKG-INFO
+-rw-r--r--   0 d3v       (1000) d3v       (1000)      263 2023-06-18 22:34:44.000000 ifnude-0.0.3/ifnude.egg-info/SOURCES.txt
+-rw-r--r--   0 d3v       (1000) d3v       (1000)        1 2023-06-18 22:34:44.000000 ifnude-0.0.3/ifnude.egg-info/dependency_links.txt
+-rw-r--r--   0 d3v       (1000) d3v       (1000)       70 2023-06-18 22:34:44.000000 ifnude-0.0.3/ifnude.egg-info/requires.txt
+-rw-r--r--   0 d3v       (1000) d3v       (1000)        7 2023-06-18 22:34:44.000000 ifnude-0.0.3/ifnude.egg-info/top_level.txt
+-rw-r--r--   0 d3v       (1000) d3v       (1000)       38 2023-06-18 22:34:44.186013 ifnude-0.0.3/setup.cfg
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     2633 2023-06-18 22:31:50.000000 ifnude-0.0.3/setup.py
```

### Comparing `ifnude-0.0.2/LICENSE.md` & `ifnude-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ifnude-0.0.2/PKG-INFO` & `ifnude-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifnude
-Version: 0.0.2
+Version: 0.0.3
 Summary: An AI powered nudity detection library
 Home-page: https://github.com/s0md3v/ifnude
 Author: Somdev Sangwan
 Author-email: s0md3v@gmail.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `ifnude-0.0.2/README.md` & `ifnude-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ifnude-0.0.2/ifnude/detector.py` & `ifnude-0.0.3/ifnude/detector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import cv2
 import numpy as np
 import onnxruntime
+from pathlib import Path
 from tqdm import tqdm
-import urllib
+import urllib.request
 
 from .detector_utils import preprocess_image
 
 
 def dummy(*args, **kwargs):
     pass
 
@@ -17,16 +18,16 @@
     with tqdm(total=total, desc='Downloading', unit='B', unit_scale=True, unit_divisor=1024) as progress:
         urllib.request.urlretrieve(url, path, reporthook=lambda count, block_size, total_size: progress.update(block_size))
 
 model_url = "https://huggingface.co/s0md3v/nudity-checker/resolve/main/detector.onnx"
 classes_url = "https://huggingface.co/s0md3v/nudity-checker/resolve/main/classes"
 
 
-home = os.path.expanduser("~")
-model_folder = os.path.join(home, f".models/")
+home = Path.home()
+model_folder = os.path.join(home, f".ifnude/")
 if not os.path.exists(model_folder):
     os.makedirs(model_folder)
 
 model_name = os.path.basename(model_url)
 model_path = os.path.join(model_folder, model_name)
 classes_path = os.path.join(model_folder, "classes")
 
@@ -39,15 +40,15 @@
     download(classes_url, classes_path)
 
 classes = [c.strip() for c in open(classes_path).readlines() if c.strip()]
 
 def detect(img, mode="default", min_prob=None):
     # we are loading the model on every detect() because it crashes otherwise for some reason xD
     detection_model = onnxruntime.InferenceSession(model_path, providers=["CPUExecutionProvider"])
-    
+
     if mode == "fast":
         image, scale = preprocess_image(img, min_side=480, max_side=800)
         if not min_prob:
             min_prob = 0.5
     else:
         image, scale = preprocess_image(img)
         if not min_prob:
```

### Comparing `ifnude-0.0.2/ifnude/detector_utils.py` & `ifnude-0.0.3/ifnude/detector_utils.py`

 * *Files identical despite different names*

### Comparing `ifnude-0.0.2/ifnude/image_utils.py` & `ifnude-0.0.3/ifnude/image_utils.py`

 * *Files identical despite different names*

### Comparing `ifnude-0.0.2/ifnude.egg-info/PKG-INFO` & `ifnude-0.0.3/ifnude.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifnude
-Version: 0.0.2
+Version: 0.0.3
 Summary: An AI powered nudity detection library
 Home-page: https://github.com/s0md3v/ifnude
 Author: Somdev Sangwan
 Author-email: s0md3v@gmail.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `ifnude-0.0.2/setup.py` & `ifnude-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Package meta-data.
 NAME = 'ifnude'
 DESCRIPTION = 'An AI powered nudity detection library'
 URL = 'https://github.com/s0md3v/ifnude'
 EMAIL = 's0md3v@gmail.com'
 AUTHOR = 'Somdev Sangwan'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'pillow',
     'opencv-python-headless>=4.5.1.48',
     'tqdm',
     'scikit-image',
```

