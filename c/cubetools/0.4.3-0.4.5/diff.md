# Comparing `tmp/cubetools-0.4.3.tar.gz` & `tmp/cubetools-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubetools-0.4.3.tar", last modified: Mon Jun 19 07:33:33 2023, max compression
+gzip compressed data, was "dist/cubetools-0.4.5.tar", last modified: Mon Jun 19 08:47:58 2023, max compression
```

## Comparing `cubetools-0.4.3.tar` & `cubetools-0.4.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-06-19 07:33:33.000000 cubetools-0.4.3/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2340 2023-06-19 07:33:33.000000 cubetools-0.4.3/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)     1232 2023-06-19 07:26:47.000000 cubetools-0.4.3/README.md
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-06-19 07:33:33.000000 cubetools-0.4.3/cubetools/
--rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.4.3/cubetools/__init__.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3047 2023-06-19 07:32:32.000000 cubetools-0.4.3/cubetools/download_model.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     9987 2023-05-15 01:24:04.000000 cubetools-0.4.3/cubetools/image_tools.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.4.3/cubetools/mindspore_lite_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.4.3/cubetools/onnx_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 07:12:09.000000 cubetools-0.4.3/cubetools/openvino_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.4.3/cubetools/paddle_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2394 2023-05-23 12:05:30.000000 cubetools-0.4.3/cubetools/python_chat_frontend.py
--rw-rw-r--   0 hls       (1000) hls       (1000)    15694 2023-05-25 10:46:59.000000 cubetools-0.4.3/cubetools/python_video_frontend.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2207 2023-06-19 04:55:21.000000 cubetools-0.4.3/cubetools/pytorch_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.4.3/cubetools/video_capture.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3799 2023-05-25 10:06:04.000000 cubetools-0.4.3/cubetools/video_predict.py
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-06-19 07:33:33.000000 cubetools-0.4.3/cubetools.egg-info/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2340 2023-06-19 07:33:33.000000 cubetools-0.4.3/cubetools.egg-info/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)      565 2023-06-19 07:33:33.000000 cubetools-0.4.3/cubetools.egg-info/SOURCES.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-06-19 07:33:33.000000 cubetools-0.4.3/cubetools.egg-info/dependency_links.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       88 2023-06-19 07:33:33.000000 cubetools-0.4.3/cubetools.egg-info/entry_points.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       32 2023-06-19 07:33:33.000000 cubetools-0.4.3/cubetools.egg-info/requires.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       10 2023-06-19 07:33:33.000000 cubetools-0.4.3/cubetools.egg-info/top_level.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-06-19 07:33:33.000000 cubetools-0.4.3/setup.cfg
--rw-rw-r--   0 hls       (1000) hls       (1000)     2291 2023-06-19 07:33:31.000000 cubetools-0.4.3/setup.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-06-19 08:47:58.000000 cubetools-0.4.5/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2340 2023-06-19 08:47:58.000000 cubetools-0.4.5/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1232 2023-06-19 07:55:29.000000 cubetools-0.4.5/README.md
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-06-19 08:47:58.000000 cubetools-0.4.5/cubetools/
+-rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.4.5/cubetools/__init__.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3047 2023-06-19 07:55:29.000000 cubetools-0.4.5/cubetools/download_model.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     9987 2023-05-15 01:24:04.000000 cubetools-0.4.5/cubetools/image_tools.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.4.5/cubetools/mindspore_lite_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.4.5/cubetools/onnx_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 07:12:09.000000 cubetools-0.4.5/cubetools/openvino_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.4.5/cubetools/paddle_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2394 2023-05-23 12:05:30.000000 cubetools-0.4.5/cubetools/python_chat_frontend.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)    15694 2023-05-25 10:46:59.000000 cubetools-0.4.5/cubetools/python_video_frontend.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2016 2023-06-19 08:47:56.000000 cubetools-0.4.5/cubetools/pytorch_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.4.5/cubetools/video_capture.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3799 2023-05-25 10:06:04.000000 cubetools-0.4.5/cubetools/video_predict.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-06-19 08:47:58.000000 cubetools-0.4.5/cubetools.egg-info/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2340 2023-06-19 08:47:58.000000 cubetools-0.4.5/cubetools.egg-info/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)      565 2023-06-19 08:47:58.000000 cubetools-0.4.5/cubetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-06-19 08:47:58.000000 cubetools-0.4.5/cubetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       88 2023-06-19 08:47:58.000000 cubetools-0.4.5/cubetools.egg-info/entry_points.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       32 2023-06-19 08:47:58.000000 cubetools-0.4.5/cubetools.egg-info/requires.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       10 2023-06-19 08:47:58.000000 cubetools-0.4.5/cubetools.egg-info/top_level.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-06-19 08:47:58.000000 cubetools-0.4.5/setup.cfg
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2291 2023-06-19 08:47:56.000000 cubetools-0.4.5/setup.py
```

### Comparing `cubetools-0.4.3/PKG-INFO` & `cubetools-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.4.3
+Version: 0.4.5
 Summary: CubeAI模型开发常用工具集
 Home-page: https://openi.pcl.ac.cn/cubeai/cubetools
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # CubeTools
```

### Comparing `cubetools-0.4.3/README.md` & `cubetools-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.3/cubetools/download_model.py` & `cubetools-0.4.5/cubetools/download_model.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.3/cubetools/image_tools.py` & `cubetools-0.4.5/cubetools/image_tools.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.3/cubetools/mindspore_lite_predict.py` & `cubetools-0.4.5/cubetools/mindspore_lite_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.3/cubetools/onnx_predict.py` & `cubetools-0.4.5/cubetools/onnx_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.3/cubetools/openvino_predict.py` & `cubetools-0.4.5/cubetools/openvino_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.3/cubetools/paddle_predict.py` & `cubetools-0.4.5/cubetools/paddle_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.3/cubetools/python_chat_frontend.py` & `cubetools-0.4.5/cubetools/python_chat_frontend.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.3/cubetools/python_video_frontend.py` & `cubetools-0.4.5/cubetools/python_video_frontend.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.3/cubetools/pytorch_predict.py` & `cubetools-0.4.5/cubetools/pytorch_predict.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding:utf-8 -*-
 import gc
 import torch
-import torch.backends.cudnn as cudnn
 from copy import deepcopy
 
 
 # 通用PyTorch推理框架
 class Model(object):
-    def __init__(self, net, model_path, param_key=None, strict=True):
-        cudnn.benchmark = True
+    def __init__(self, net, model_path, param_key=None, strict=True, cudnn_benchmark=True):
+        if cudnn_benchmark:
+            import torch.backends.cudnn as cudnn
+            cudnn.benchmark = True
         self.device = torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')
         self.cpu_device = torch.device('cpu')
 
         net_params = torch.load(model_path, map_location=self.cpu_device)
         if param_key is not None and param_key in net_params:
                 net_params = net_params[param_key]
 
@@ -28,37 +29,37 @@
         net.load_state_dict(net_params, strict=strict)
 
         self.model = net
         self.model.eval()
         self.model = self.model.to(self.device)
 
     def predict(self, inputs):
-        if isinstance(inputs, tuple):
-            inputs = list(inputs)
+        inputs = to_device(inputs, self.device)
 
         with torch.no_grad():
             if isinstance(inputs, dict):
-                for k, v in inputs.items():
-                    inputs[k] = v.to(self.device)
                 results = self.model(**inputs)
             elif isinstance(inputs, list):
-                for i in range(len(inputs)):
-                    inputs[i] = inputs[i].to(self.device)
                 results = self.model(*inputs)
             else:
-                inputs = inputs.to(self.device)
                 results = self.model(inputs)
 
-        if isinstance(results, tuple):
-            results = list(results)
-        if isinstance(results, torch.Tensor):
-            results = results.to(self.cpu_device)
-        elif isinstance(results, dict):
-            for k, v in results.items():
-                results[k] = v.to(self.cpu_device)
-        elif isinstance(results, list):
-            for i in range(len(results)):
-                results[i] = results[i].to(self.cpu_device)
-
+        results = to_device(results, self.cpu_device)
         gc.collect()
         torch.cuda.empty_cache()
         return results
+
+
+def to_device(data, device):
+    if isinstance(data, tuple):
+        data = list(data)
+
+    if isinstance(data, torch.Tensor):
+        data = data.to(device)
+    elif isinstance(data, dict):
+        for k, v in data.items():
+            data[k] = to_device(v, device)
+    elif isinstance(data, list):
+        for i in range(len(data)):
+            data[i] = to_device(data[i], device)
+
+    return data
```

### Comparing `cubetools-0.4.3/cubetools/video_capture.py` & `cubetools-0.4.5/cubetools/video_capture.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.3/cubetools/video_predict.py` & `cubetools-0.4.5/cubetools/video_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.3/cubetools.egg-info/PKG-INFO` & `cubetools-0.4.5/cubetools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.4.3
+Version: 0.4.5
 Summary: CubeAI模型开发常用工具集
 Home-page: https://openi.pcl.ac.cn/cubeai/cubetools
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # CubeTools
```

### Comparing `cubetools-0.4.3/cubetools.egg-info/SOURCES.txt` & `cubetools-0.4.5/cubetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.3/setup.py` & `cubetools-0.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 with open("README.md", "r", encoding='utf-8') as file:
     long_description = file.read()
 
 
 setup(
     name='cubetools',
-    version='0.4.3',
+    version='0.4.5',
     author='cubeai',
     author_email='cubeai@163.com',
     description='CubeAI模型开发常用工具集',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     packages=find_packages(),
```

