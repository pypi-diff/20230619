# Comparing `tmp/segmentation-mask-overlay-0.4.0.tar.gz` & `tmp/segmentation-mask-overlay-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segmentation-mask-overlay-0.4.0.tar", last modified: Sun Jun 18 20:44:45 2023, max compression
+gzip compressed data, was "segmentation-mask-overlay-0.4.1.tar", last modified: Mon Jun 19 09:44:32 2023, max compression
```

## Comparing `segmentation-mask-overlay-0.4.0.tar` & `segmentation-mask-overlay-0.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-18 20:44:45.687200 segmentation-mask-overlay-0.4.0/
--rw-r--r--   0 artem      (501) staff       (20)     1072 2023-02-16 13:41:43.000000 segmentation-mask-overlay-0.4.0/LICENSE
--rw-r--r--   0 artem      (501) staff       (20)       45 2023-02-16 14:05:23.000000 segmentation-mask-overlay-0.4.0/MANIFEST.in
--rw-r--r--   0 artem      (501) staff       (20)     2005 2023-06-18 20:44:45.687317 segmentation-mask-overlay-0.4.0/PKG-INFO
--rw-r--r--   0 artem      (501) staff       (20)     1496 2023-06-18 20:39:45.000000 segmentation-mask-overlay-0.4.0/README.md
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-18 20:44:45.674756 segmentation-mask-overlay-0.4.0/examples/
--rw-r--r--   0 artem      (501) staff       (20)    39331 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.0/examples/cat.jpg
--rw-r--r--   0 artem      (501) staff       (20)      840 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.0/examples/cat.py
--rw-r--r--   0 artem      (501) staff       (20)   243410 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.0/examples/cat_masked.jpg
--rw-r--r--   0 artem      (501) staff       (20)       81 2023-02-16 13:29:52.000000 segmentation-mask-overlay-0.4.0/pyproject.toml
--rw-r--r--   0 artem      (501) staff       (20)      788 2023-06-18 20:44:45.688393 segmentation-mask-overlay-0.4.0/setup.cfg
--rwx------   0 artem      (501) staff       (20)       69 2023-02-16 13:38:32.000000 segmentation-mask-overlay-0.4.0/setup.py
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-18 20:44:45.641708 segmentation-mask-overlay-0.4.0/src/
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-18 20:44:45.678713 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay/
--rw-r--r--   0 artem      (501) staff       (20)      187 2023-06-18 20:39:50.000000 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay/__init__.py
--rw-r--r--   0 artem      (501) staff       (20)     5912 2023-06-18 20:39:45.000000 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay/main.py
--rw-r--r--   0 artem      (501) staff       (20)     3322 2023-06-18 20:40:11.000000 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay/utils.py
--rw-r--r--   0 artem      (501) staff       (20)     8442 2023-06-18 20:39:45.000000 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay/video.py
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-18 20:44:45.685934 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay.egg-info/
--rw-r--r--   0 artem      (501) staff       (20)     2005 2023-06-18 20:44:45.000000 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay.egg-info/PKG-INFO
--rw-r--r--   0 artem      (501) staff       (20)      564 2023-06-18 20:44:45.000000 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay.egg-info/SOURCES.txt
--rw-r--r--   0 artem      (501) staff       (20)        1 2023-06-18 20:44:45.000000 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay.egg-info/dependency_links.txt
--rw-r--r--   0 artem      (501) staff       (20)       38 2023-06-18 20:44:45.000000 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay.egg-info/requires.txt
--rw-r--r--   0 artem      (501) staff       (20)       26 2023-06-18 20:44:45.000000 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay.egg-info/top_level.txt
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-18 20:44:45.686694 segmentation-mask-overlay-0.4.0/tests/
--rw-r--r--   0 artem      (501) staff       (20)     1778 2023-06-18 20:39:45.000000 segmentation-mask-overlay-0.4.0/tests/test_overlay.py
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 09:44:31.979930 segmentation-mask-overlay-0.4.1/
+-rw-r--r--   0 artem      (501) staff       (20)     1072 2023-02-16 13:41:43.000000 segmentation-mask-overlay-0.4.1/LICENSE
+-rw-r--r--   0 artem      (501) staff       (20)       45 2023-02-16 14:05:23.000000 segmentation-mask-overlay-0.4.1/MANIFEST.in
+-rw-r--r--   0 artem      (501) staff       (20)     2005 2023-06-19 09:44:31.980035 segmentation-mask-overlay-0.4.1/PKG-INFO
+-rw-r--r--   0 artem      (501) staff       (20)     1496 2023-06-18 20:39:45.000000 segmentation-mask-overlay-0.4.1/README.md
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 09:44:31.963370 segmentation-mask-overlay-0.4.1/examples/
+-rw-r--r--   0 artem      (501) staff       (20)    39331 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.1/examples/cat.jpg
+-rw-r--r--   0 artem      (501) staff       (20)      840 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.1/examples/cat.py
+-rw-r--r--   0 artem      (501) staff       (20)   243410 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.1/examples/cat_masked.jpg
+-rw-r--r--   0 artem      (501) staff       (20)       81 2023-02-16 13:29:52.000000 segmentation-mask-overlay-0.4.1/pyproject.toml
+-rw-r--r--   0 artem      (501) staff       (20)      788 2023-06-19 09:44:32.004180 segmentation-mask-overlay-0.4.1/setup.cfg
+-rwx------   0 artem      (501) staff       (20)       69 2023-02-16 13:38:32.000000 segmentation-mask-overlay-0.4.1/setup.py
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 09:44:31.951076 segmentation-mask-overlay-0.4.1/src/
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 09:44:31.968633 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay/
+-rw-r--r--   0 artem      (501) staff       (20)      187 2023-06-19 09:40:47.000000 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay/__init__.py
+-rw-r--r--   0 artem      (501) staff       (20)     5912 2023-06-18 20:39:45.000000 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay/main.py
+-rw-r--r--   0 artem      (501) staff       (20)     3322 2023-06-18 20:40:11.000000 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay/utils.py
+-rw-r--r--   0 artem      (501) staff       (20)     8482 2023-06-19 09:44:28.000000 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay/video.py
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 09:44:31.978598 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay.egg-info/
+-rw-r--r--   0 artem      (501) staff       (20)     2005 2023-06-19 09:44:31.000000 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay.egg-info/PKG-INFO
+-rw-r--r--   0 artem      (501) staff       (20)      564 2023-06-19 09:44:31.000000 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay.egg-info/SOURCES.txt
+-rw-r--r--   0 artem      (501) staff       (20)        1 2023-06-19 09:44:31.000000 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay.egg-info/dependency_links.txt
+-rw-r--r--   0 artem      (501) staff       (20)       38 2023-06-19 09:44:31.000000 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay.egg-info/requires.txt
+-rw-r--r--   0 artem      (501) staff       (20)       26 2023-06-19 09:44:31.000000 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay.egg-info/top_level.txt
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 09:44:31.979338 segmentation-mask-overlay-0.4.1/tests/
+-rw-r--r--   0 artem      (501) staff       (20)     1778 2023-06-18 20:47:46.000000 segmentation-mask-overlay-0.4.1/tests/test_overlay.py
```

### Comparing `segmentation-mask-overlay-0.4.0/LICENSE` & `segmentation-mask-overlay-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.0/PKG-INFO` & `segmentation-mask-overlay-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation-mask-overlay
-Version: 0.4.0
+Version: 0.4.1
 Summary: Plotting the segmentation masks has never been so exciting!
 Home-page: https://github.com/lobantseff/segmentation-mask-overlay
 Author: Artem Lobantsev
 Author-email: lobantseff@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `segmentation-mask-overlay-0.4.0/README.md` & `segmentation-mask-overlay-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.0/examples/cat.jpg` & `segmentation-mask-overlay-0.4.1/examples/cat.jpg`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.0/examples/cat.py` & `segmentation-mask-overlay-0.4.1/examples/cat.py`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.0/examples/cat_masked.jpg` & `segmentation-mask-overlay-0.4.1/examples/cat_masked.jpg`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.0/setup.cfg` & `segmentation-mask-overlay-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay/main.py` & `segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay/main.py`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay/utils.py` & `segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay/utils.py`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay/video.py` & `segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay/video.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from pathlib import Path
 from typing import Union
 
 from segmentation_mask_overlay.utils import catchtime
 from segmentation_mask_overlay.utils import check_convert_image
 
 
-Pathlike = Union[str, Path]
+Pathlike = Union[str, bytes, Path]
+
 
 def overlay_masks_video(
     im_sequence: np.ndarray,
     *mask_sequences: np.ndarray,
     output: Union[str, Path] = "numpy",
     array_dims: str = "THWC",
     fps: int = 15,
@@ -68,15 +69,14 @@
     # Iterate through: frame, (frame_mask0, frame_mask1, ...)
     video_frames = []
     for im, *masks in zip(im_sequence, *mask_sequences):
 
         # Normalize, cast to uint8, convert to RGB
         im = check_convert_image(im, input_dims=array_dims[1:])
 
-        # 
         masks_im = []
         if len(masks) > 0:
             # Prepare image for each mask
             masks_im = [np.copy(im) for _ in range(len(masks))]
             # Segmentation canvas to fuse-in the colored masks (uint16)
             segmentation_overlay_list = [np.zeros_like(im, dtype=np.uint16) for _ in range(len(masks))]
             # Segmentation masks (bool)
@@ -119,25 +119,26 @@
             fourcc=cv2.VideoWriter_fourcc(*"mp4v"),
             fps=fps,
             frameSize=(width, height),
         )
         for frame in video_frames:
             out.write(frame)
         out.release()
-    
+
     elif output == "numpy":
         video_frames = np.array(video_frames)
         if array_dims == "TCHW":
             video_frames = video_frames.transpose(0, 3, 1, 2)
         return video_frames
 
 
 def overlay_points_video(
     im_sequence: np.ndarray,
     *pts_sequences: np.ndarray,
+    sizes: list[int] = None,
     output: Union[str, Path] = "numpy",
     array_dims: str = "THWC",
     fps: int = 15,
 ):
     """Create videos out of sequences of images and masks.
 
     Parameters
@@ -180,28 +181,28 @@
     # Iterate through: frame, (frame_mask0, frame_mask1, ...)
     video_frames = []
     for im, *pts in zip(im_sequence, *pts_sequences):
 
         # Normalize, cast to uint8, convert to RGB
         im = check_convert_image(im, input_dims=array_dims[1:])
 
-        # 
         pts_im = []
         if len(pts) > 0:
             # Prepare image for each mask
             pts_im = [np.copy(im) for _ in range(len(pts))]
 
             # Inpaint masks into masks_im
             for i in range(len(pts)):
                 points = pts[i]
                 points_im = pts_im[i].copy()
                 points_color = pts_cmaps[i]
+                s = sizes[i]
 
                 for x, y in points:
-                    pts_im[i] = cv2.circle(points_im, (x, y), 1, points_color.tolist(), -1, cv2.LINE_AA)
+                    pts_im[i] = cv2.circle(points_im, (y, x), s, points_color.tolist(), -1, cv2.LINE_AA)
 
         frame = np.concatenate((im, *pts_im), 1)
         video_frames.append(frame)
 
     if isinstance(output, Path) or output[-4:] == ".mp4":
         height, width, _ = video_frames[-1].shape
         out = cv2.VideoWriter(
```

### Comparing `segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay.egg-info/PKG-INFO` & `segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation-mask-overlay
-Version: 0.4.0
+Version: 0.4.1
 Summary: Plotting the segmentation masks has never been so exciting!
 Home-page: https://github.com/lobantseff/segmentation-mask-overlay
 Author: Artem Lobantsev
 Author-email: lobantseff@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay.egg-info/SOURCES.txt` & `segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.0/tests/test_overlay.py` & `segmentation-mask-overlay-0.4.1/tests/test_overlay.py`

 * *Files identical despite different names*

