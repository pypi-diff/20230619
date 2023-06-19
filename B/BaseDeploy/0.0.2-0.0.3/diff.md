# Comparing `tmp/BaseDeploy-0.0.2.tar.gz` & `tmp/BaseDeploy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaseDeploy-0.0.2.tar", last modified: Tue Jun 13 08:04:20 2023, max compression
+gzip compressed data, was "dist/BaseDeploy-0.0.3.tar", last modified: Mon Jun 19 06:01:24 2023, max compression
```

## Comparing `BaseDeploy-0.0.2.tar` & `BaseDeploy-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/BaseDeploy/
--rw-rw-r--   0 user      (1001) user      (1001)    21811 2023-06-13 07:43:46.000000 BaseDeploy-0.0.2/BaseDeploy/BaseDeploy.py
--rw-rw-r--   0 user      (1001) user      (1001)      206 2023-06-13 08:04:12.000000 BaseDeploy-0.0.2/BaseDeploy/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     1298 2023-06-13 07:57:10.000000 BaseDeploy-0.0.2/BaseDeploy/version.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/BaseDeploy.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      299 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/BaseDeploy.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      346 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/BaseDeploy.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/BaseDeploy.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       57 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/BaseDeploy.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1001) user      (1001)       60 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/BaseDeploy.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)       11 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/BaseDeploy.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-07 11:34:56.000000 BaseDeploy-0.0.2/BaseDeploy.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDeploy-0.0.2/MANIFEST.in
--rw-rw-r--   0 user      (1001) user      (1001)      299 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)       59 2023-06-08 08:27:27.000000 BaseDeploy-0.0.2/install_requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     4238 2023-06-13 07:53:50.000000 BaseDeploy-0.0.2/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/BaseDeploy/
+-rw-rw-r--   0 user      (1001) user      (1001)    23218 2023-06-19 05:59:49.000000 BaseDeploy-0.0.3/BaseDeploy/BaseDeploy.py
+-rw-rw-r--   0 user      (1001) user      (1001)      206 2023-06-13 08:04:12.000000 BaseDeploy-0.0.3/BaseDeploy/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1298 2023-06-19 06:01:09.000000 BaseDeploy-0.0.3/BaseDeploy/version.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/BaseDeploy.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      299 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/BaseDeploy.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      346 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/BaseDeploy.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/BaseDeploy.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       57 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/BaseDeploy.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       60 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/BaseDeploy.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       11 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/BaseDeploy.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-07 11:34:56.000000 BaseDeploy-0.0.3/BaseDeploy.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDeploy-0.0.3/MANIFEST.in
+-rw-rw-r--   0 user      (1001) user      (1001)      299 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)       59 2023-06-08 08:27:27.000000 BaseDeploy-0.0.3/install_requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-06-19 06:01:24.000000 BaseDeploy-0.0.3/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     4238 2023-06-19 06:01:03.000000 BaseDeploy-0.0.3/setup.py
```

### Comparing `BaseDeploy-0.0.2/BaseDeploy/BaseDeploy.py` & `BaseDeploy-0.0.3/BaseDeploy/BaseDeploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import BaseDT
 from BaseDT.data import ModelData, ImageData
 import numpy as np
 from typing import Union, List
 import os
 import cv2
 import matplotlib.pyplot as plt
+from BaseDT.utils import mmpose_preprocess, mmpose_postprocess
 
 def get_host_ip():
     try:
         import socket
     except ImportError:
         print("The library 'socket' does not exist. Please use 'pip3 install socket' to install library.")
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
@@ -187,14 +188,32 @@
                             show_cls([dt], [result])
                             print(result)
                         else:
                             print("The accuracy is lower than the preset value, "
                                   "if you want to draw a picture, "
                                   "please set score={:.2f}, or lower.".format(result['置信度']))
                     #pred_onx = self.model.run(output_names, {input_name: dt.to_tensor()})
+                elif self.codebase == 'MMPose':
+                    h, w = self.model.get_inputs()[0].shape[2:]
+                    model_input_size = (w, h)
+                    img_shape = dt.raw_value.shape[:2]
+                    img = dt.raw_value
+                    bbox = np.array([0, 0, img_shape[1], img_shape[0]])
+                    resized_img, center, scale = mmpose_preprocess(img, model_input_size)
+                    input_tensor = [resized_img.transpose(2, 0, 1)]
+                    outputs = self.model.run(output_names, {input_name: input_tensor})
+                    keypoints, scores = mmpose_postprocess(outputs, model_input_size, center, scale)
+                    result = {'关键点':keypoints, '得分':scores}
+                    if show_path:
+                        result['路径'] = dt.data_source
+                    results.append(result)
+                    if show:
+                        from BaseDT.plot import show_pose
+                        show_pose([dt], [result])
+                        print(result)
                 else:
                     input_shape = self.model.get_inputs()[0].shape
                     print('The onnx model is not exported by the XEdu tool.'\
 						' BaseDeploy calls BaseDT to adapt the input to {}.'\
 						' \'mean\': [123.675, 116.28, 103.53], \'std\': [58.395, 57.12, 57.375], \'normalize\': True'.format(input_shape))
                     if input_shape[0] == 'unk__606':
                         score = 0
@@ -426,33 +445,39 @@
                 if show == False:
                     if results[i]['置信度'] < score:
                         print("The accuracy is lower than the preset value, "
                           "if you want to draw a picture, "
                           "please set score={:.2f}, or lower.".format(results[i]['置信度']))
                         dt.init_plt()
                     else:
-                        from BaseDT.plot import show_cls
-                        show_cls(dt, results[i])
-                imgs.append(dt.get_image())
+                        from BaseDT.plot import draw_single_cls
+                        draw_single_cls(dt, results[i])
+                #imgs.append(dt.get_image())
             elif self.codebase == 'MMDet':
                 if show == False:
-                    from BaseDT.plot import show_det
-                    show_det(dt, results[i])      
-                imgs.append(dt.get_image())
+                    from BaseDT.plot import draw_single_det
+                    draw_single_det(dt, results[i])      
+                
+                #imgs.append(dt.get_image())
             elif self.codebase == 'TFJS':
                 if show == False:
                     if results[i]['置信度'] < score:
                         print("The accuracy is lower than the preset value, "
                           "if you want to draw a picture, "
                           "please set score={:.2f}, or lower.".format(results[i]['置信度']))
                         dt.init_plt()
                     else:
-                        from BaseDT.plot import show_cls
-                        show_cls(dt, results[i])
-                imgs.append(dt.get_image())
+                        from BaseDT.plot import draw_single_cls
+                        draw_single_cls(dt, results[i])
+                #imgs.append(dt.get_image())
+            elif self.codebase == 'MMPose':
+                if show == False:
+                    from BaseDT.plot import draw_single_pose
+                    draw_single_pose(dt, results[i])
+            imgs.append(dt.get_image())
         return results, imgs
     
     def diy_inference(self, input_data):
         assert isinstance(input_data, np.ndarray)
         input_name = self.model.get_inputs()[0].name
         output_names = [o.name for o in self.model.get_outputs()]
         pred_onx = self.model.run(output_names, {input_name: input_data})
```

### Comparing `BaseDeploy-0.0.2/BaseDeploy/version.py` & `BaseDeploy-0.0.3/BaseDeploy/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-__version__='0.0.2'
+__version__='0.0.3'
 __path__=os.path.abspath(os.getcwd())
 
 def parse_version_info(version_str):
     version_info = []
     for x in version_str.split('.'):
         if x.isdigit():
             version_info.append(int(x))
```

### Comparing `BaseDeploy-0.0.2/setup.py` & `BaseDeploy-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 yield item
 
     packages = list(gen_packages_items())
     return packages
 
 setup(
     name='BaseDeploy',
-    version='0.0.2',
+    version='0.0.3',
     # version='0.0.1rc1',
     description='BaseDeploy is a simple deployment tool made by XEdu.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
```

