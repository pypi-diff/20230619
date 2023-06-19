# Comparing `tmp/segmentation-mask-overlay-0.4.1.tar.gz` & `tmp/segmentation-mask-overlay-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segmentation-mask-overlay-0.4.1.tar", last modified: Mon Jun 19 09:44:32 2023, max compression
+gzip compressed data, was "segmentation-mask-overlay-0.4.2.tar", last modified: Mon Jun 19 13:48:10 2023, max compression
```

## Comparing `segmentation-mask-overlay-0.4.1.tar` & `segmentation-mask-overlay-0.4.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 09:44:31.979930 segmentation-mask-overlay-0.4.1/
--rw-r--r--   0 artem      (501) staff       (20)     1072 2023-02-16 13:41:43.000000 segmentation-mask-overlay-0.4.1/LICENSE
--rw-r--r--   0 artem      (501) staff       (20)       45 2023-02-16 14:05:23.000000 segmentation-mask-overlay-0.4.1/MANIFEST.in
--rw-r--r--   0 artem      (501) staff       (20)     2005 2023-06-19 09:44:31.980035 segmentation-mask-overlay-0.4.1/PKG-INFO
--rw-r--r--   0 artem      (501) staff       (20)     1496 2023-06-18 20:39:45.000000 segmentation-mask-overlay-0.4.1/README.md
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 09:44:31.963370 segmentation-mask-overlay-0.4.1/examples/
--rw-r--r--   0 artem      (501) staff       (20)    39331 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.1/examples/cat.jpg
--rw-r--r--   0 artem      (501) staff       (20)      840 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.1/examples/cat.py
--rw-r--r--   0 artem      (501) staff       (20)   243410 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.1/examples/cat_masked.jpg
--rw-r--r--   0 artem      (501) staff       (20)       81 2023-02-16 13:29:52.000000 segmentation-mask-overlay-0.4.1/pyproject.toml
--rw-r--r--   0 artem      (501) staff       (20)      788 2023-06-19 09:44:32.004180 segmentation-mask-overlay-0.4.1/setup.cfg
--rwx------   0 artem      (501) staff       (20)       69 2023-02-16 13:38:32.000000 segmentation-mask-overlay-0.4.1/setup.py
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 09:44:31.951076 segmentation-mask-overlay-0.4.1/src/
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 09:44:31.968633 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay/
--rw-r--r--   0 artem      (501) staff       (20)      187 2023-06-19 09:40:47.000000 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay/__init__.py
--rw-r--r--   0 artem      (501) staff       (20)     5912 2023-06-18 20:39:45.000000 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay/main.py
--rw-r--r--   0 artem      (501) staff       (20)     3322 2023-06-18 20:40:11.000000 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay/utils.py
--rw-r--r--   0 artem      (501) staff       (20)     8482 2023-06-19 09:44:28.000000 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay/video.py
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 09:44:31.978598 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay.egg-info/
--rw-r--r--   0 artem      (501) staff       (20)     2005 2023-06-19 09:44:31.000000 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay.egg-info/PKG-INFO
--rw-r--r--   0 artem      (501) staff       (20)      564 2023-06-19 09:44:31.000000 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay.egg-info/SOURCES.txt
--rw-r--r--   0 artem      (501) staff       (20)        1 2023-06-19 09:44:31.000000 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay.egg-info/dependency_links.txt
--rw-r--r--   0 artem      (501) staff       (20)       38 2023-06-19 09:44:31.000000 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay.egg-info/requires.txt
--rw-r--r--   0 artem      (501) staff       (20)       26 2023-06-19 09:44:31.000000 segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay.egg-info/top_level.txt
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 09:44:31.979338 segmentation-mask-overlay-0.4.1/tests/
--rw-r--r--   0 artem      (501) staff       (20)     1778 2023-06-18 20:47:46.000000 segmentation-mask-overlay-0.4.1/tests/test_overlay.py
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:48:10.492360 segmentation-mask-overlay-0.4.2/
+-rw-r--r--   0 artem      (501) staff       (20)     1072 2023-02-16 13:41:43.000000 segmentation-mask-overlay-0.4.2/LICENSE
+-rw-r--r--   0 artem      (501) staff       (20)       45 2023-02-16 14:05:23.000000 segmentation-mask-overlay-0.4.2/MANIFEST.in
+-rw-r--r--   0 artem      (501) staff       (20)     2005 2023-06-19 13:48:10.492560 segmentation-mask-overlay-0.4.2/PKG-INFO
+-rw-r--r--   0 artem      (501) staff       (20)     1496 2023-06-18 20:39:45.000000 segmentation-mask-overlay-0.4.2/README.md
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:48:10.461547 segmentation-mask-overlay-0.4.2/examples/
+-rw-r--r--   0 artem      (501) staff       (20)    39331 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.2/examples/cat.jpg
+-rw-r--r--   0 artem      (501) staff       (20)      840 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.2/examples/cat.py
+-rw-r--r--   0 artem      (501) staff       (20)   243410 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.2/examples/cat_masked.jpg
+-rw-r--r--   0 artem      (501) staff       (20)       81 2023-02-16 13:29:52.000000 segmentation-mask-overlay-0.4.2/pyproject.toml
+-rw-r--r--   0 artem      (501) staff       (20)      788 2023-06-19 13:48:10.495633 segmentation-mask-overlay-0.4.2/setup.cfg
+-rwx------   0 artem      (501) staff       (20)       69 2023-02-16 13:38:32.000000 segmentation-mask-overlay-0.4.2/setup.py
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:48:10.454466 segmentation-mask-overlay-0.4.2/src/
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:48:10.479559 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay/
+-rw-r--r--   0 artem      (501) staff       (20)      187 2023-06-19 13:47:21.000000 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay/__init__.py
+-rw-r--r--   0 artem      (501) staff       (20)     5912 2023-06-18 20:39:45.000000 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay/main.py
+-rw-r--r--   0 artem      (501) staff       (20)     3322 2023-06-18 20:40:11.000000 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay/utils.py
+-rw-r--r--   0 artem      (501) staff       (20)     8679 2023-06-19 13:46:58.000000 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay/video.py
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:48:10.490009 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay.egg-info/
+-rw-r--r--   0 artem      (501) staff       (20)     2005 2023-06-19 13:48:10.000000 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay.egg-info/PKG-INFO
+-rw-r--r--   0 artem      (501) staff       (20)      564 2023-06-19 13:48:10.000000 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay.egg-info/SOURCES.txt
+-rw-r--r--   0 artem      (501) staff       (20)        1 2023-06-19 13:48:10.000000 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay.egg-info/dependency_links.txt
+-rw-r--r--   0 artem      (501) staff       (20)       38 2023-06-19 13:48:10.000000 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay.egg-info/requires.txt
+-rw-r--r--   0 artem      (501) staff       (20)       26 2023-06-19 13:48:10.000000 segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay.egg-info/top_level.txt
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:48:10.491552 segmentation-mask-overlay-0.4.2/tests/
+-rw-r--r--   0 artem      (501) staff       (20)     1778 2023-06-18 20:47:46.000000 segmentation-mask-overlay-0.4.2/tests/test_overlay.py
```

### Comparing `segmentation-mask-overlay-0.4.1/LICENSE` & `segmentation-mask-overlay-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.1/PKG-INFO` & `segmentation-mask-overlay-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation-mask-overlay
-Version: 0.4.1
+Version: 0.4.2
 Summary: Plotting the segmentation masks has never been so exciting!
 Home-page: https://github.com/lobantseff/segmentation-mask-overlay
 Author: Artem Lobantsev
 Author-email: lobantseff@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `segmentation-mask-overlay-0.4.1/README.md` & `segmentation-mask-overlay-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.1/examples/cat.jpg` & `segmentation-mask-overlay-0.4.2/examples/cat.jpg`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.1/examples/cat.py` & `segmentation-mask-overlay-0.4.2/examples/cat.py`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.1/examples/cat_masked.jpg` & `segmentation-mask-overlay-0.4.2/examples/cat_masked.jpg`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.1/setup.cfg` & `segmentation-mask-overlay-0.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay/main.py` & `segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay/main.py`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay/utils.py` & `segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay/utils.py`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay/video.py` & `segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay/video.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             video_frames = video_frames.transpose(0, 3, 1, 2)
         return video_frames
 
 
 def overlay_points_video(
     im_sequence: np.ndarray,
     *pts_sequences: np.ndarray,
-    sizes: list[int] = None,
+    sizes: int | list[int] = 5,
     output: Union[str, Path] = "numpy",
     array_dims: str = "THWC",
     fps: int = 15,
 ):
     """Create videos out of sequences of images and masks.
 
     Parameters
@@ -163,43 +163,46 @@
 
     if array_dims not in ["TCHW", "THWC"]:
         raise AssertionError("array_dims should be THWC | TCHW")
 
     # Check array length consistency between image and masks.
     if len(pts_sequences) > 0:
         assert all(
-            [im_sequence.shape[0] == p.shape[0] for p in pts_sequences]
+            [im_sequence.shape[0] == len(p) for p in pts_sequences]
         ), "Sequence and masks have different size T"
 
     # Set colormaps: 'tab10' if n_classes <=10, 'rainbow' otherwise
     pts_cmaps = []
     num_classes = len(pts_sequences)
     if num_classes <= 10:
         pts_cmaps = plt.cm.tab10(range(10), bytes=True)[:num_classes, :-1][:, ::-1]
     else:
         pts_cmaps = plt.cm.rainbow_r(np.linspace(0, 1, num_classes), bytes=True)[:, :-1][:, ::-1]
 
     # Iterate through: frame, (frame_mask0, frame_mask1, ...)
     video_frames = []
     for im, *pts in zip(im_sequence, *pts_sequences):
 
+        if isinstance(sizes, list):
+            assert len(pts) == len(sizes), "Provide the sizes for all the point arrays"
+
         # Normalize, cast to uint8, convert to RGB
         im = check_convert_image(im, input_dims=array_dims[1:])
 
         pts_im = []
         if len(pts) > 0:
             # Prepare image for each mask
             pts_im = [np.copy(im) for _ in range(len(pts))]
 
             # Inpaint masks into masks_im
             for i in range(len(pts)):
                 points = pts[i]
                 points_im = pts_im[i].copy()
                 points_color = pts_cmaps[i]
-                s = sizes[i]
+                s = sizes[i] if isinstance(sizes, list) else sizes
 
                 for x, y in points:
                     pts_im[i] = cv2.circle(points_im, (y, x), s, points_color.tolist(), -1, cv2.LINE_AA)
 
         frame = np.concatenate((im, *pts_im), 1)
         video_frames.append(frame)
 
@@ -210,15 +213,15 @@
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
 
 
@@ -232,11 +235,11 @@
     # with catchtime("masking video"):
     #     video = overlay_masks_video(run, array_dims="TCHW")
     #     print(video.shape)
     pts1 = np.array([np.arange(0, 512), np.arange(0, 512)[::-1]]).T
     pts1 = np.repeat(pts1[None], 64, 0)
     pts2 = np.array([np.arange(0, 512), np.arange(0, 512)]).T
     pts2 = np.repeat(pts2[None], 64, 0)
-    pts3 = np.random.randint(0, 512, (64, 128, 2))
+    pts3 = [np.random.randint(0, 512, (np.random.randint(0, 256), 2)) for _ in range(64)]
     with catchtime("masking video"):
         video = overlay_points_video(run, pts1, pts2, pts3, array_dims="TCHW", output="video.mp4")
         # print(video.shape)
```

### Comparing `segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay.egg-info/PKG-INFO` & `segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation-mask-overlay
-Version: 0.4.1
+Version: 0.4.2
 Summary: Plotting the segmentation masks has never been so exciting!
 Home-page: https://github.com/lobantseff/segmentation-mask-overlay
 Author: Artem Lobantsev
 Author-email: lobantseff@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `segmentation-mask-overlay-0.4.1/src/segmentation_mask_overlay.egg-info/SOURCES.txt` & `segmentation-mask-overlay-0.4.2/src/segmentation_mask_overlay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.1/tests/test_overlay.py` & `segmentation-mask-overlay-0.4.2/tests/test_overlay.py`

 * *Files identical despite different names*

