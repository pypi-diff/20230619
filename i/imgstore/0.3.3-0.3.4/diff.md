# Comparing `tmp/imgstore-0.3.3.tar.gz` & `tmp/imgstore-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgstore-0.3.3.tar", last modified: Tue Apr  4 15:49:06 2023, max compression
+gzip compressed data, was "imgstore-0.3.4.tar", last modified: Mon Jun 19 08:59:56 2023, max compression
```

## Comparing `imgstore-0.3.3.tar` & `imgstore-0.3.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:49:06.025455 imgstore-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-04 15:49:02.000000 imgstore-0.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-04 15:49:02.000000 imgstore-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-04 15:49:06.025455 imgstore-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-04-04 15:49:02.000000 imgstore-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:49:06.025455 imgstore-0.3.3/imgstore/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-04 15:49:02.000000 imgstore-0.3.3/imgstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-04 15:49:02.000000 imgstore-0.3.3/imgstore/align.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-04 15:49:02.000000 imgstore-0.3.3/imgstore/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-04 15:49:02.000000 imgstore-0.3.3/imgstore/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-04-04 15:49:02.000000 imgstore-0.3.3/imgstore/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    48120 2023-04-04 15:49:02.000000 imgstore-0.3.3/imgstore/stores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:49:06.025455 imgstore-0.3.3/imgstore/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-04 15:49:02.000000 imgstore-0.3.3/imgstore/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:49:06.025455 imgstore-0.3.3/imgstore/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   861959 2023-04-04 15:49:02.000000 imgstore-0.3.3/imgstore/tests/data/graffiti.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:49:06.025455 imgstore-0.3.3/imgstore/tests/data/store_mp4/
--rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-04-04 15:49:02.000000 imgstore-0.3.3/imgstore/tests/data/store_mp4/000000.mp4
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-04 15:49:02.000000 imgstore-0.3.3/imgstore/tests/data/store_mp4/000000.npz
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-04 15:49:02.000000 imgstore-0.3.3/imgstore/tests/data/store_mp4/000001.mp4
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-04-04 15:49:02.000000 imgstore-0.3.3/imgstore/tests/data/store_mp4/000001.npz
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-04 15:49:02.000000 imgstore-0.3.3/imgstore/tests/data/store_mp4/metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    32368 2023-04-04 15:49:02.000000 imgstore-0.3.3/imgstore/tests/test_imgstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-04 15:49:02.000000 imgstore-0.3.3/imgstore/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-04 15:49:02.000000 imgstore-0.3.3/imgstore/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-04-04 15:49:02.000000 imgstore-0.3.3/imgstore/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:49:06.025455 imgstore-0.3.3/imgstore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-04 15:49:06.000000 imgstore-0.3.3/imgstore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-04 15:49:06.000000 imgstore-0.3.3/imgstore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:49:06.000000 imgstore-0.3.3/imgstore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-04 15:49:06.000000 imgstore-0.3.3/imgstore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-04 15:49:06.000000 imgstore-0.3.3/imgstore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-04 15:49:06.000000 imgstore-0.3.3/imgstore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-04 15:49:06.025455 imgstore-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-04 15:49:02.000000 imgstore-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:59:56.219705 imgstore-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-19 08:59:51.000000 imgstore-0.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-19 08:59:51.000000 imgstore-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-19 08:59:56.219705 imgstore-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-19 08:59:51.000000 imgstore-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:59:56.219705 imgstore-0.3.4/imgstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48533 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/stores.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:59:56.219705 imgstore-0.3.4/imgstore/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:59:56.219705 imgstore-0.3.4/imgstore/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   861959 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/tests/data/graffiti.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:59:56.219705 imgstore-0.3.4/imgstore/tests/data/store_mp4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/tests/data/store_mp4/000000.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/tests/data/store_mp4/000000.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/tests/data/store_mp4/000001.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/tests/data/store_mp4/000001.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/tests/data/store_mp4/metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    32368 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/tests/test_imgstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:59:56.219705 imgstore-0.3.4/imgstore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-19 08:59:56.000000 imgstore-0.3.4/imgstore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-19 08:59:56.000000 imgstore-0.3.4/imgstore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:59:56.000000 imgstore-0.3.4/imgstore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-19 08:59:56.000000 imgstore-0.3.4/imgstore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-19 08:59:56.000000 imgstore-0.3.4/imgstore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 08:59:56.000000 imgstore-0.3.4/imgstore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-19 08:59:56.219705 imgstore-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-19 08:59:51.000000 imgstore-0.3.4/setup.py
```

### Comparing `imgstore-0.3.3/LICENSE.txt` & `imgstore-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.3/PKG-INFO` & `imgstore-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgstore
-Version: 0.3.3
+Version: 0.3.4
 Summary: IMGStore houses your video frames
 Home-page: https://github.com/loopbio/imgstore
 Author: John Stowers, Santi Villalba
 Author-email: john@loopbio.com, santi@loopbio.com
 License: BSD 3 clause
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `imgstore-0.3.3/README.md` & `imgstore-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.3/imgstore/align.py` & `imgstore-0.3.4/imgstore/align.py`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.3/imgstore/apps.py` & `imgstore-0.3.4/imgstore/apps.py`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.3/imgstore/index.py` & `imgstore-0.3.4/imgstore/index.py`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.3/imgstore/stores.py` & `imgstore-0.3.4/imgstore/stores.py`

 * *Files 1% similar despite different names*

```diff
@@ -821,15 +821,15 @@
 
     return ranges
 
 
 class DirectoryImgStore(_ImgStore):
     _supported_modes = 'wr'
 
-    _cv2_fmts = {'tif', 'png', 'jpg', 'ppm', 'pgm', 'bmp'}
+    _cv2_fmts = {'tif', 'png', 'jpg', 'ppm', 'pgm', 'bmp', 'tif+color', 'png+color', 'jpg+color', 'bmp+color'}
     _raw_fmts = {'npy', 'bpk'}
 
     _DEFAULT_CHUNKSIZE = 200
 
     def __init__(self, **kwargs):
 
         self._chunk_cdir = ''
@@ -842,14 +842,23 @@
         kwargs.pop('gpu_id', None)
 
         if kwargs['mode'] == 'w':
             if 'chunksize' not in kwargs:
                 kwargs['chunksize'] = self._DEFAULT_CHUNKSIZE
             kwargs['encoding'] = kwargs.pop('encoding', None)
 
+        kwargs['write_encode_encoding'] = None
+
+        if kwargs['format'].endswith('+color'):
+            kwargs['format'] = kwargs['format'].replace('+color', '')
+
+            if kwargs['encoding']:
+                kwargs['write_encode_encoding'] = kwargs['encoding']
+                kwargs['encoding'] = None  # and so in the store it is no longer encoded
+
         _ImgStore.__init__(self, **kwargs)
 
         self._color = (self._imgshape[-1] == 3) & (len(self._imgshape) == 3)
 
         if (self._mode == 'w') and (self._format == 'pgm') and self._color:
             self._log.warn("store created with color image shape but using grayscale 'pgm' format")
```

### Comparing `imgstore-0.3.3/imgstore/tests/data/graffiti.png` & `imgstore-0.3.4/imgstore/tests/data/graffiti.png`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.3/imgstore/tests/data/store_mp4/000000.mp4` & `imgstore-0.3.4/imgstore/tests/data/store_mp4/000000.mp4`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.3/imgstore/tests/data/store_mp4/000000.npz` & `imgstore-0.3.4/imgstore/tests/data/store_mp4/000000.npz`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.3/imgstore/tests/data/store_mp4/000001.mp4` & `imgstore-0.3.4/imgstore/tests/data/store_mp4/000001.mp4`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.3/imgstore/tests/data/store_mp4/000001.npz` & `imgstore-0.3.4/imgstore/tests/data/store_mp4/000001.npz`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.3/imgstore/tests/test_imgstore.py` & `imgstore-0.3.4/imgstore/tests/test_imgstore.py`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.3/imgstore/tests/test_util.py` & `imgstore-0.3.4/imgstore/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.3/imgstore/ui.py` & `imgstore-0.3.4/imgstore/ui.py`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.3/imgstore/util.py` & `imgstore-0.3.4/imgstore/util.py`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.3/imgstore.egg-info/PKG-INFO` & `imgstore-0.3.4/imgstore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgstore
-Version: 0.3.3
+Version: 0.3.4
 Summary: IMGStore houses your video frames
 Home-page: https://github.com/loopbio/imgstore
 Author: John Stowers, Santi Villalba
 Author-email: john@loopbio.com, santi@loopbio.com
 License: BSD 3 clause
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `imgstore-0.3.3/imgstore.egg-info/SOURCES.txt` & `imgstore-0.3.4/imgstore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.3/setup.py` & `imgstore-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 setup(
     name='imgstore',
     license='BSD 3 clause',
     description='IMGStore houses your video frames',
     long_description=long_description,
     long_description_content_type='text/markdown',
     include_package_data=True,
-    version='0.3.3',
+    version='0.3.4',
     url='https://github.com/loopbio/imgstore',
     author='John Stowers, Santi Villalba',
     author_email='john@loopbio.com, santi@loopbio.com',
     packages=find_packages(),
     classifiers=[
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
```

