# Comparing `tmp/segmentation-mask-overlay-0.4.2.tar.gz` & `tmp/segmentation-mask-overlay-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segmentation-mask-overlay-0.4.2.tar", last modified: Mon Jun 19 13:48:10 2023, max compression
+gzip compressed data, was "segmentation-mask-overlay-0.4.3.tar", last modified: Mon Jun 19 13:54:09 2023, max compression
```

## Comparing `segmentation-mask-overlay-0.4.2.tar` & `segmentation-mask-overlay-0.4.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:48:10.492360 segmentation-mask-overlay-0.4.2/
--rw-r--r--   0 artem      (501) staff       (20)     1072 2023-02-16 13:41:43.000000 segmentation-mask-overlay-0.4.2/LICENSE
--rw-r--r--   0 artem      (501) staff       (20)       45 2023-02-16 14:05:23.000000 segmentation-mask-overlay-0.4.2/MANIFEST.in
--rw-r--r--   0 artem      (501) staff       (20)     2005 2023-06-19 13:48:10.492560 segmentation-mask-overlay-0.4.2/PKG-INFO
--rw-r--r--   0 artem      (501) staff       (20)     1496 2023-06-18 20:39:45.000000 segmentation-mask-overlay-0.4.2/README.md
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:48:10.461547 segmentation-mask-overlay-0.4.2/examples/
--rw-r--r--   0 artem      (501) staff       (20)    39331 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.2/examples/cat.jpg
--rw-r--r--   0 artem      (501) staff       (20)      840 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.2/examples/cat.py
--rw-r--r--   0 artem      (501) staff       (20)   243410 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.2/examples/cat_masked.jpg
--rw-r--r--   0 artem      (501) staff       (20)       81 2023-02-16 13:29:52.000000 segmentation-mask-overlay-0.4.2/pyproject.toml
--rw-r--r--   0 artem      (501) staff       (20)      788 2023-06-19 13:48:10.495633 segmentation-mask-overlay-0.4.2/setup.cfg
--rwx------   0 artem      (501) staff       (20)       69 2023-02-16 13:38:32.000000 segmentation-mask-overlay-0.4.2/setup.py
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:48:10.454466 segmentation-mask-overlay-0.4.2/src/
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:48:10.479559 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay/
--rw-r--r--   0 artem      (501) staff       (20)      187 2023-06-19 13:47:21.000000 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay/__init__.py
--rw-r--r--   0 artem      (501) staff       (20)     5912 2023-06-18 20:39:45.000000 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay/main.py
--rw-r--r--   0 artem      (501) staff       (20)     3322 2023-06-18 20:40:11.000000 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay/utils.py
--rw-r--r--   0 artem      (501) staff       (20)     8679 2023-06-19 13:46:58.000000 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay/video.py
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:48:10.490009 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay.egg-info/
--rw-r--r--   0 artem      (501) staff       (20)     2005 2023-06-19 13:48:10.000000 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay.egg-info/PKG-INFO
--rw-r--r--   0 artem      (501) staff       (20)      564 2023-06-19 13:48:10.000000 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay.egg-info/SOURCES.txt
--rw-r--r--   0 artem      (501) staff       (20)        1 2023-06-19 13:48:10.000000 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay.egg-info/dependency_links.txt
--rw-r--r--   0 artem      (501) staff       (20)       38 2023-06-19 13:48:10.000000 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay.egg-info/requires.txt
--rw-r--r--   0 artem      (501) staff       (20)       26 2023-06-19 13:48:10.000000 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay.egg-info/top_level.txt
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:48:10.491552 segmentation-mask-overlay-0.4.2/tests/
--rw-r--r--   0 artem      (501) staff       (20)     1778 2023-06-18 20:47:46.000000 segmentation-mask-overlay-0.4.2/tests/test_overlay.py
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:54:09.357421 segmentation-mask-overlay-0.4.3/
+-rw-r--r--   0 artem      (501) staff       (20)     1072 2023-02-16 13:41:43.000000 segmentation-mask-overlay-0.4.3/LICENSE
+-rw-r--r--   0 artem      (501) staff       (20)       45 2023-02-16 14:05:23.000000 segmentation-mask-overlay-0.4.3/MANIFEST.in
+-rw-r--r--   0 artem      (501) staff       (20)     2005 2023-06-19 13:54:09.357523 segmentation-mask-overlay-0.4.3/PKG-INFO
+-rw-r--r--   0 artem      (501) staff       (20)     1496 2023-06-18 20:39:45.000000 segmentation-mask-overlay-0.4.3/README.md
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:54:09.316789 segmentation-mask-overlay-0.4.3/examples/
+-rw-r--r--   0 artem      (501) staff       (20)    39331 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.3/examples/cat.jpg
+-rw-r--r--   0 artem      (501) staff       (20)      840 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.3/examples/cat.py
+-rw-r--r--   0 artem      (501) staff       (20)   243410 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.3/examples/cat_masked.jpg
+-rw-r--r--   0 artem      (501) staff       (20)       81 2023-02-16 13:29:52.000000 segmentation-mask-overlay-0.4.3/pyproject.toml
+-rw-r--r--   0 artem      (501) staff       (20)      788 2023-06-19 13:54:09.358407 segmentation-mask-overlay-0.4.3/setup.cfg
+-rwx------   0 artem      (501) staff       (20)       69 2023-02-16 13:38:32.000000 segmentation-mask-overlay-0.4.3/setup.py
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:54:09.294938 segmentation-mask-overlay-0.4.3/src/
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:54:09.325054 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay/
+-rw-r--r--   0 artem      (501) staff       (20)      187 2023-06-19 13:53:39.000000 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay/__init__.py
+-rw-r--r--   0 artem      (501) staff       (20)     5912 2023-06-18 20:39:45.000000 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay/main.py
+-rw-r--r--   0 artem      (501) staff       (20)     3322 2023-06-18 20:40:11.000000 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay/utils.py
+-rw-r--r--   0 artem      (501) staff       (20)     8725 2023-06-19 13:53:04.000000 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay/video.py
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:54:09.328664 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay.egg-info/
+-rw-r--r--   0 artem      (501) staff       (20)     2005 2023-06-19 13:54:09.000000 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay.egg-info/PKG-INFO
+-rw-r--r--   0 artem      (501) staff       (20)      564 2023-06-19 13:54:09.000000 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay.egg-info/SOURCES.txt
+-rw-r--r--   0 artem      (501) staff       (20)        1 2023-06-19 13:54:09.000000 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay.egg-info/dependency_links.txt
+-rw-r--r--   0 artem      (501) staff       (20)       38 2023-06-19 13:54:09.000000 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay.egg-info/requires.txt
+-rw-r--r--   0 artem      (501) staff       (20)       26 2023-06-19 13:54:09.000000 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay.egg-info/top_level.txt
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:54:09.356681 segmentation-mask-overlay-0.4.3/tests/
+-rw-r--r--   0 artem      (501) staff       (20)     1778 2023-06-18 20:47:46.000000 segmentation-mask-overlay-0.4.3/tests/test_overlay.py
```

### Comparing `segmentation-mask-overlay-0.4.2/LICENSE` & `segmentation-mask-overlay-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.2/PKG-INFO` & `segmentation-mask-overlay-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation-mask-overlay
-Version: 0.4.2
+Version: 0.4.3
 Summary: Plotting the segmentation masks has never been so exciting!
 Home-page: https://github.com/lobantseff/segmentation-mask-overlay
 Author: Artem Lobantsev
 Author-email: lobantseff@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `segmentation-mask-overlay-0.4.2/README.md` & `segmentation-mask-overlay-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.2/examples/cat.jpg` & `segmentation-mask-overlay-0.4.3/examples/cat.jpg`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.2/examples/cat.py` & `segmentation-mask-overlay-0.4.3/examples/cat.py`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.2/examples/cat_masked.jpg` & `segmentation-mask-overlay-0.4.3/examples/cat_masked.jpg`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.2/setup.cfg` & `segmentation-mask-overlay-0.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay/main.py` & `segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay/main.py`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay/utils.py` & `segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay/utils.py`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay/video.py` & `segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay/video.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,14 +197,15 @@
             for i in range(len(pts)):
                 points = pts[i]
                 points_im = pts_im[i].copy()
                 points_color = pts_cmaps[i]
                 s = sizes[i] if isinstance(sizes, list) else sizes
 
                 for x, y in points:
+                    x, y = round(x), round(y)
                     pts_im[i] = cv2.circle(points_im, (y, x), s, points_color.tolist(), -1, cv2.LINE_AA)
 
         frame = np.concatenate((im, *pts_im), 1)
         video_frames.append(frame)
 
     if isinstance(output, Path) or output[-4:] == ".mp4":
         height, width, _ = video_frames[-1].shape
```

### Comparing `segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay.egg-info/PKG-INFO` & `segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation-mask-overlay
-Version: 0.4.2
+Version: 0.4.3
 Summary: Plotting the segmentation masks has never been so exciting!
 Home-page: https://github.com/lobantseff/segmentation-mask-overlay
 Author: Artem Lobantsev
 Author-email: lobantseff@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay.egg-info/SOURCES.txt` & `segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.2/tests/test_overlay.py` & `segmentation-mask-overlay-0.4.3/tests/test_overlay.py`

 * *Files identical despite different names*

