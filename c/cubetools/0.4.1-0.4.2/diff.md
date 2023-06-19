# Comparing `tmp/cubetools-0.4.1.tar.gz` & `tmp/cubetools-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubetools-0.4.1.tar", last modified: Thu May 25 10:36:23 2023, max compression
+gzip compressed data, was "dist/cubetools-0.4.2.tar", last modified: Mon Jun 19 07:26:59 2023, max compression
```

## Comparing `cubetools-0.4.1.tar` & `cubetools-0.4.2.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-25 10:36:23.000000 cubetools-0.4.1/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2251 2023-05-25 10:36:23.000000 cubetools-0.4.1/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)     1151 2023-05-25 10:06:04.000000 cubetools-0.4.1/README.md
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-25 10:36:23.000000 cubetools-0.4.1/cubetools/
--rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.4.1/cubetools/__init__.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     9987 2023-05-15 01:24:04.000000 cubetools-0.4.1/cubetools/image_tools.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.4.1/cubetools/mindspore_lite_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.4.1/cubetools/onnx_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 07:12:09.000000 cubetools-0.4.1/cubetools/openvino_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.4.1/cubetools/paddle_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2394 2023-05-23 12:05:30.000000 cubetools-0.4.1/cubetools/python_chat_frontend.py
--rw-rw-r--   0 hls       (1000) hls       (1000)    15694 2023-05-25 10:36:21.000000 cubetools-0.4.1/cubetools/python_video_frontend.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.4.1/cubetools/video_capture.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3799 2023-05-25 10:06:04.000000 cubetools-0.4.1/cubetools/video_predict.py
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-25 10:36:23.000000 cubetools-0.4.1/cubetools.egg-info/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2251 2023-05-25 10:36:23.000000 cubetools-0.4.1/cubetools.egg-info/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)      508 2023-05-25 10:36:23.000000 cubetools-0.4.1/cubetools.egg-info/SOURCES.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-25 10:36:23.000000 cubetools-0.4.1/cubetools.egg-info/dependency_links.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        5 2023-05-25 10:36:23.000000 cubetools-0.4.1/cubetools.egg-info/entry_points.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       27 2023-05-25 10:36:23.000000 cubetools-0.4.1/cubetools.egg-info/requires.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       10 2023-05-25 10:36:23.000000 cubetools-0.4.1/cubetools.egg-info/top_level.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-25 10:36:23.000000 cubetools-0.4.1/setup.cfg
--rw-rw-r--   0 hls       (1000) hls       (1000)     2192 2023-05-25 10:36:20.000000 cubetools-0.4.1/setup.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-06-19 07:26:59.000000 cubetools-0.4.2/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2340 2023-06-19 07:26:59.000000 cubetools-0.4.2/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1232 2023-06-19 07:26:47.000000 cubetools-0.4.2/README.md
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-06-19 07:26:59.000000 cubetools-0.4.2/cubetools/
+-rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.4.2/cubetools/__init__.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3052 2023-06-19 06:38:49.000000 cubetools-0.4.2/cubetools/download_model.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     9987 2023-05-15 01:24:04.000000 cubetools-0.4.2/cubetools/image_tools.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.4.2/cubetools/mindspore_lite_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.4.2/cubetools/onnx_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 07:12:09.000000 cubetools-0.4.2/cubetools/openvino_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.4.2/cubetools/paddle_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2394 2023-05-23 12:05:30.000000 cubetools-0.4.2/cubetools/python_chat_frontend.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)    15694 2023-05-25 10:46:59.000000 cubetools-0.4.2/cubetools/python_video_frontend.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2207 2023-06-19 04:55:21.000000 cubetools-0.4.2/cubetools/pytorch_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.4.2/cubetools/video_capture.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3799 2023-05-25 10:06:04.000000 cubetools-0.4.2/cubetools/video_predict.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-06-19 07:26:59.000000 cubetools-0.4.2/cubetools.egg-info/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2340 2023-06-19 07:26:58.000000 cubetools-0.4.2/cubetools.egg-info/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)      565 2023-06-19 07:26:59.000000 cubetools-0.4.2/cubetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-06-19 07:26:58.000000 cubetools-0.4.2/cubetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       73 2023-06-19 07:26:58.000000 cubetools-0.4.2/cubetools.egg-info/entry_points.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       32 2023-06-19 07:26:58.000000 cubetools-0.4.2/cubetools.egg-info/requires.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       10 2023-06-19 07:26:58.000000 cubetools-0.4.2/cubetools.egg-info/top_level.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-06-19 07:26:59.000000 cubetools-0.4.2/setup.cfg
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2276 2023-06-19 07:26:47.000000 cubetools-0.4.2/setup.py
```

### Comparing `cubetools-0.4.1/PKG-INFO` & `cubetools-0.4.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.4.1
+Version: 0.4.2
 Summary: CubeAI模型开发常用工具集
 Home-page: https://openi.pcl.ac.cn/cubeai/cubetools
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # CubeTools
         
         [CubeAI智立方](https://openi.pcl.ac.cn/OpenI/cubeai) 模型和应用开发常用工具集。
         
         目前主要包括：
         
-        - 图像前处理、后处理常用函数封装。
-        - 支持多路视频流媒体在线AI流式服务的通用SDK组件。
-        - 基于Gradio的视频流媒体类Python前端SDK组件。
-        - 基于Gradio的聊天对话类Python前端SDK组件。
-        - 基于 [OpenVino Runtime](https://pypi.org/project/openvino/) 封装的通用OpenVino模型推理器。
-        - 基于 [ONNX Runtime](https://pypi.org/project/onnxruntime-gpu/) 封装的通用ONNX模型推理器。
-        - 基于 [Paddle Inference](https://www.paddlepaddle.org.cn/paddle/paddleinference) 推理引擎封装的通用PaddlePaddle模型推理器。
-        - 基于 [MindSpore Lite](https://www.mindspore.cn/lite) 推理引擎封装的通用MindSporeLite推理器。
-        
+        - 图像前处理、后处理等常用函数封装。
+        - 通用视频流媒体在线流式AI推理服务组件。
+        - 通用OpenVino模型推理框架（基于 [OpenVino Runtime](https://pypi.org/project/openvino/) 封装）。
+        - 通用ONNX模型推理框架（基于 [ONNX Runtime](https://pypi.org/project/onnxruntime-gpu/) 封装）。
+        - 通用PaddlePaddle模型推理框架（基于 [Paddle Inference](https://www.paddlepaddle.org.cn/paddle/paddleinference) 推理引擎封装）。
+        - 通用MindSporeLite推理框架（基于 [MindSpore Lite](https://www.mindspore.cn/lite) 推理引擎封装）。
+        - 通用Pytorch模型推理框架。
+        - 基于Gradio的视频流媒体类Python前端服务组件。
+        - 基于Gradio的聊天对话类Python前端服务组件。
+        - 模型文件下载。
         
         ## 开源主页
         
         - https://openi.pcl.ac.cn/cubeai/cubetools
         
         ## 依赖包主页
```

### Comparing `cubetools-0.4.1/cubetools/image_tools.py` & `cubetools-0.4.2/cubetools/image_tools.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.1/cubetools/mindspore_lite_predict.py` & `cubetools-0.4.2/cubetools/mindspore_lite_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.1/cubetools/onnx_predict.py` & `cubetools-0.4.2/cubetools/onnx_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.1/cubetools/openvino_predict.py` & `cubetools-0.4.2/cubetools/openvino_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.1/cubetools/paddle_predict.py` & `cubetools-0.4.2/cubetools/paddle_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.1/cubetools/python_chat_frontend.py` & `cubetools-0.4.2/cubetools/python_chat_frontend.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.1/cubetools/python_video_frontend.py` & `cubetools-0.4.2/cubetools/python_video_frontend.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.1/cubetools/video_capture.py` & `cubetools-0.4.2/cubetools/video_capture.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.1/cubetools/video_predict.py` & `cubetools-0.4.2/cubetools/video_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.1/cubetools.egg-info/PKG-INFO` & `cubetools-0.4.2/cubetools.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.4.1
+Version: 0.4.2
 Summary: CubeAI模型开发常用工具集
 Home-page: https://openi.pcl.ac.cn/cubeai/cubetools
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # CubeTools
         
         [CubeAI智立方](https://openi.pcl.ac.cn/OpenI/cubeai) 模型和应用开发常用工具集。
         
         目前主要包括：
         
-        - 图像前处理、后处理常用函数封装。
-        - 支持多路视频流媒体在线AI流式服务的通用SDK组件。
-        - 基于Gradio的视频流媒体类Python前端SDK组件。
-        - 基于Gradio的聊天对话类Python前端SDK组件。
-        - 基于 [OpenVino Runtime](https://pypi.org/project/openvino/) 封装的通用OpenVino模型推理器。
-        - 基于 [ONNX Runtime](https://pypi.org/project/onnxruntime-gpu/) 封装的通用ONNX模型推理器。
-        - 基于 [Paddle Inference](https://www.paddlepaddle.org.cn/paddle/paddleinference) 推理引擎封装的通用PaddlePaddle模型推理器。
-        - 基于 [MindSpore Lite](https://www.mindspore.cn/lite) 推理引擎封装的通用MindSporeLite推理器。
-        
+        - 图像前处理、后处理等常用函数封装。
+        - 通用视频流媒体在线流式AI推理服务组件。
+        - 通用OpenVino模型推理框架（基于 [OpenVino Runtime](https://pypi.org/project/openvino/) 封装）。
+        - 通用ONNX模型推理框架（基于 [ONNX Runtime](https://pypi.org/project/onnxruntime-gpu/) 封装）。
+        - 通用PaddlePaddle模型推理框架（基于 [Paddle Inference](https://www.paddlepaddle.org.cn/paddle/paddleinference) 推理引擎封装）。
+        - 通用MindSporeLite推理框架（基于 [MindSpore Lite](https://www.mindspore.cn/lite) 推理引擎封装）。
+        - 通用Pytorch模型推理框架。
+        - 基于Gradio的视频流媒体类Python前端服务组件。
+        - 基于Gradio的聊天对话类Python前端服务组件。
+        - 模型文件下载。
         
         ## 开源主页
         
         - https://openi.pcl.ac.cn/cubeai/cubetools
         
         ## 依赖包主页
```

### Comparing `cubetools-0.4.1/setup.py` & `cubetools-0.4.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,38 +21,41 @@
 
 with open("README.md", "r", encoding='utf-8') as file:
     long_description = file.read()
 
 
 setup(
     name='cubetools',
-    version='0.4.1',
+    version='0.4.2',
     author='cubeai',
     author_email='cubeai@163.com',
     description='CubeAI模型开发常用工具集',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pillow',
-        'opencv-python'
+        'opencv-python',
+        'tqdm'
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'License :: OSI Approved :: Apache Software License',
     ],
     entry_points="""
+    [console_scripts]
+    download_model = cubetools.download_model
     """,
     keywords='AI application tools',
     python_requires='>=3.5',
     url='https://openi.pcl.ac.cn/cubeai/cubetools',
 )
```

