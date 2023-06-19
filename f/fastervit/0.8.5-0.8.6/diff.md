# Comparing `tmp/fastervit-0.8.5.tar.gz` & `tmp/fastervit-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ali/Desktop/Gitlab_repos/FasterViT_pip_test/dist/.tmp-6yjzyjaz/fastervit-0.8.5.tar", last modified: Mon Jun 19 06:48:48 2023, max compression
+gzip compressed data, was "/home/ali/Desktop/Gitlab_repos/FasterViT_pip_test/dist/.tmp-gymc9d88/fastervit-0.8.6.tar", last modified: Mon Jun 19 06:52:25 2023, max compression
```

## Comparing `fastervit-0.8.5.tar` & `fastervit-0.8.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-19 06:48:48.000000 fastervit-0.8.5/
--rw-rw-r--   0 ali       (1000) ali       (1000)     4146 2023-06-17 23:20:57.000000 fastervit-0.8.5/LICENSE
--rw-rw-r--   0 ali       (1000) ali       (1000)       45 2023-06-19 01:32:21.000000 fastervit-0.8.5/MANIFEST.in
--rw-rw-r--   0 ali       (1000) ali       (1000)     9396 2023-06-19 06:48:48.000000 fastervit-0.8.5/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)     8445 2023-06-19 06:48:02.000000 fastervit-0.8.5/README.md
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-19 06:48:48.000000 fastervit-0.8.5/fastervit/
--rw-rw-r--   0 ali       (1000) ali       (1000)       41 2023-06-19 01:24:49.000000 fastervit-0.8.5/fastervit/__init__.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-19 06:48:48.000000 fastervit-0.8.5/fastervit/assets/
--rw-rw-r--   0 ali       (1000) ali       (1000)   100537 2023-06-17 23:20:57.000000 fastervit-0.8.5/fastervit/assets/hierarchial_attn.png
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-19 06:48:48.000000 fastervit-0.8.5/fastervit/models/
--rw-rw-r--   0 ali       (1000) ali       (1000)       96 2023-06-19 01:23:28.000000 fastervit-0.8.5/fastervit/models/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    46961 2023-06-19 06:34:23.000000 fastervit-0.8.5/fastervit/models/faster_vit.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    48699 2023-06-19 06:34:44.000000 fastervit-0.8.5/fastervit/models/faster_vit_any_res.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     7840 2023-06-19 01:34:49.000000 fastervit-0.8.5/fastervit/models/registry.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-19 06:48:48.000000 fastervit-0.8.5/fastervit/scheduler/
--rw-rw-r--   0 ali       (1000) ali       (1000)      291 2023-06-17 23:20:57.000000 fastervit-0.8.5/fastervit/scheduler/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     4161 2023-06-17 23:20:57.000000 fastervit-0.8.5/fastervit/scheduler/cosine_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     2098 2023-06-17 23:20:57.000000 fastervit-0.8.5/fastervit/scheduler/multistep_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3457 2023-06-17 23:20:57.000000 fastervit-0.8.5/fastervit/scheduler/plateau_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     4003 2023-06-17 23:20:57.000000 fastervit-0.8.5/fastervit/scheduler/poly_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     5095 2023-06-17 23:20:57.000000 fastervit-0.8.5/fastervit/scheduler/scheduler.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3907 2023-06-17 23:20:57.000000 fastervit-0.8.5/fastervit/scheduler/scheduler_factory.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1902 2023-06-17 23:20:57.000000 fastervit-0.8.5/fastervit/scheduler/step_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3936 2023-06-17 23:20:57.000000 fastervit-0.8.5/fastervit/scheduler/tanh_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      734 2023-06-17 23:20:57.000000 fastervit-0.8.5/fastervit/tensorboard.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    49797 2023-06-17 23:23:20.000000 fastervit-0.8.5/fastervit/train.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    16145 2023-06-17 23:20:57.000000 fastervit-0.8.5/fastervit/validate.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-19 06:48:48.000000 fastervit-0.8.5/fastervit.egg-info/
--rw-rw-r--   0 ali       (1000) ali       (1000)     9396 2023-06-19 06:48:48.000000 fastervit-0.8.5/fastervit.egg-info/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)      768 2023-06-19 06:48:48.000000 fastervit-0.8.5/fastervit.egg-info/SOURCES.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-06-19 06:48:48.000000 fastervit-0.8.5/fastervit.egg-info/dependency_links.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       32 2023-06-19 06:48:48.000000 fastervit-0.8.5/fastervit.egg-info/requires.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       10 2023-06-19 06:48:48.000000 fastervit-0.8.5/fastervit.egg-info/top_level.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)      126 2023-06-19 06:48:48.000000 fastervit-0.8.5/setup.cfg
--rw-rw-r--   0 ali       (1000) ali       (1000)     1549 2023-06-19 06:47:58.000000 fastervit-0.8.5/setup.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-19 06:52:25.000000 fastervit-0.8.6/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4146 2023-06-17 23:20:57.000000 fastervit-0.8.6/LICENSE
+-rw-rw-r--   0 ali       (1000) ali       (1000)       45 2023-06-19 01:32:21.000000 fastervit-0.8.6/MANIFEST.in
+-rw-rw-r--   0 ali       (1000) ali       (1000)     9405 2023-06-19 06:52:25.000000 fastervit-0.8.6/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)     8454 2023-06-19 06:50:27.000000 fastervit-0.8.6/README.md
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-19 06:52:25.000000 fastervit-0.8.6/fastervit/
+-rw-rw-r--   0 ali       (1000) ali       (1000)       41 2023-06-19 01:24:49.000000 fastervit-0.8.6/fastervit/__init__.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-19 06:52:25.000000 fastervit-0.8.6/fastervit/assets/
+-rw-rw-r--   0 ali       (1000) ali       (1000)   100537 2023-06-17 23:20:57.000000 fastervit-0.8.6/fastervit/assets/hierarchial_attn.png
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-19 06:52:25.000000 fastervit-0.8.6/fastervit/models/
+-rw-rw-r--   0 ali       (1000) ali       (1000)       96 2023-06-19 01:23:28.000000 fastervit-0.8.6/fastervit/models/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    46961 2023-06-19 06:34:23.000000 fastervit-0.8.6/fastervit/models/faster_vit.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    48699 2023-06-19 06:34:44.000000 fastervit-0.8.6/fastervit/models/faster_vit_any_res.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     7840 2023-06-19 01:34:49.000000 fastervit-0.8.6/fastervit/models/registry.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-19 06:52:25.000000 fastervit-0.8.6/fastervit/scheduler/
+-rw-rw-r--   0 ali       (1000) ali       (1000)      291 2023-06-17 23:20:57.000000 fastervit-0.8.6/fastervit/scheduler/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4161 2023-06-17 23:20:57.000000 fastervit-0.8.6/fastervit/scheduler/cosine_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     2098 2023-06-17 23:20:57.000000 fastervit-0.8.6/fastervit/scheduler/multistep_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3457 2023-06-17 23:20:57.000000 fastervit-0.8.6/fastervit/scheduler/plateau_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4003 2023-06-17 23:20:57.000000 fastervit-0.8.6/fastervit/scheduler/poly_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     5095 2023-06-17 23:20:57.000000 fastervit-0.8.6/fastervit/scheduler/scheduler.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3907 2023-06-17 23:20:57.000000 fastervit-0.8.6/fastervit/scheduler/scheduler_factory.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1902 2023-06-17 23:20:57.000000 fastervit-0.8.6/fastervit/scheduler/step_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3936 2023-06-17 23:20:57.000000 fastervit-0.8.6/fastervit/scheduler/tanh_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      734 2023-06-17 23:20:57.000000 fastervit-0.8.6/fastervit/tensorboard.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    49797 2023-06-17 23:23:20.000000 fastervit-0.8.6/fastervit/train.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    16145 2023-06-17 23:20:57.000000 fastervit-0.8.6/fastervit/validate.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-19 06:52:25.000000 fastervit-0.8.6/fastervit.egg-info/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     9405 2023-06-19 06:52:25.000000 fastervit-0.8.6/fastervit.egg-info/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)      768 2023-06-19 06:52:25.000000 fastervit-0.8.6/fastervit.egg-info/SOURCES.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-06-19 06:52:25.000000 fastervit-0.8.6/fastervit.egg-info/dependency_links.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       32 2023-06-19 06:52:25.000000 fastervit-0.8.6/fastervit.egg-info/requires.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       10 2023-06-19 06:52:25.000000 fastervit-0.8.6/fastervit.egg-info/top_level.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)      126 2023-06-19 06:52:25.000000 fastervit-0.8.6/setup.cfg
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1549 2023-06-19 06:52:08.000000 fastervit-0.8.6/setup.py
```

### Comparing `fastervit-0.8.5/LICENSE` & `fastervit-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.5/PKG-INFO` & `fastervit-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastervit
-Version: 0.8.5
+Version: 0.8.6
 Summary: FasterViT: Fast Vision Transformers with Hierarchical Attention
 Home-page: https://github.com/NVlabs/FasterViT
 Author: Ali Hatamizadeh
 Author-email: ahatamiz123@gmail.com
 License: NVIDIA Source Code License-NC
 Keywords: pytorch pretrained models efficientnet mobilenetv3 mnasnet resnet vision transformer vit
 Classifier: Programming Language :: Python :: 3.7
@@ -42,19 +42,19 @@
 
 <p align="center">
 <img src="https://github.com/NVlabs/FasterViT/assets/26806394/253d1a2e-b5f5-4a9b-a362-6cdd16bfccc1" width=62% height=62% 
 class="center">
 </p>
 
 
-We introduce a new self-attention mechanism, denoted as Hierarchical
+<!-- We introduce a new self-attention mechanism, denoted as Hierarchical
 Attention (HAT), that captures both short and long-range information by learning
 cross-window carrier tokens.
 
-![teaser](./fastervit/assets/hierarchial_attn.png)
+![teaser](./fastervit/assets/hierarchial_attn.png) -->
 
 
 ## 💥 News 💥
 
 - **[06.18.2023]** 🔥 We have released the FasterViT [pip package](https://pypi.org/project/fastervit/0.8.3/) !
 - **[06.17.2023]** 🔥 [Any-resolution FasterViT](https://github.com/NVlabs/FasterViT/blob/main/models/faster_vit_any_res.py)  model is now available ! the model can be used for variety of applications such as detection and segmentation or high-resolution fine-tuning with arbitrary input image resolutions. 
 - **[06.09.2023]** 🔥🔥 We have released source code and ImageNet-1K FasterViT-models !
```

### Comparing `fastervit-0.8.5/README.md` & `fastervit-0.8.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 
 <p align="center">
 <img src="https://github.com/NVlabs/FasterViT/assets/26806394/253d1a2e-b5f5-4a9b-a362-6cdd16bfccc1" width=62% height=62% 
 class="center">
 </p>
 
 
-We introduce a new self-attention mechanism, denoted as Hierarchical
+<!-- We introduce a new self-attention mechanism, denoted as Hierarchical
 Attention (HAT), that captures both short and long-range information by learning
 cross-window carrier tokens.
 
-![teaser](./fastervit/assets/hierarchial_attn.png)
+![teaser](./fastervit/assets/hierarchial_attn.png) -->
 
 
 ## 💥 News 💥
 
 - **[06.18.2023]** 🔥 We have released the FasterViT [pip package](https://pypi.org/project/fastervit/0.8.3/) !
 - **[06.17.2023]** 🔥 [Any-resolution FasterViT](https://github.com/NVlabs/FasterViT/blob/main/models/faster_vit_any_res.py)  model is now available ! the model can be used for variety of applications such as detection and segmentation or high-resolution fine-tuning with arbitrary input image resolutions. 
 - **[06.09.2023]** 🔥🔥 We have released source code and ImageNet-1K FasterViT-models !
```

#### html2text {}

```diff
@@ -8,18 +8,15 @@
 Kautz](https://jankautz.com/), [Pavlo Molchanov](https://www.pmolchanov.com/).
 For business inquiries, please visit our website and submit the form: [NVIDIA
 Research Licensing](https://www.nvidia.com/en-us/research/inquiries/) --
 - FasterViT achieves a new SOTA Pareto-front in terms of accuracy vs. image
 throughput (no extra training data !)
  [https://github.com/NVlabs/FasterViT/assets/26806394/253d1a2e-b5f5-4a9b-a362-
                                  6cdd16bfccc1]
-We introduce a new self-attention mechanism, denoted as Hierarchical Attention
-(HAT), that captures both short and long-range information by learning cross-
-window carrier tokens. ![teaser](./fastervit/assets/hierarchial_attn.png) ##
-ð¥ News ð¥ - **[06.18.2023]** ð¥ We have released the FasterViT [pip
+ ## ð¥ News ð¥ - **[06.18.2023]** ð¥ We have released the FasterViT [pip
 package](https://pypi.org/project/fastervit/0.8.3/) ! - **[06.17.2023]** ð¥
 [Any-resolution FasterViT](https://github.com/NVlabs/FasterViT/blob/main/
 models/faster_vit_any_res.py) model is now available ! the model can be used
 for variety of applications such as detection and segmentation or high-
 resolution fine-tuning with arbitrary input image resolutions. - **
 [06.09.2023]** ð¥ð¥ We have released source code and ImageNet-1K FasterViT-
 models ! ## Quick Start The FasterViT can be conveniently installed by: ```bash
```

### Comparing `fastervit-0.8.5/fastervit/assets/hierarchial_attn.png` & `fastervit-0.8.6/fastervit/assets/hierarchial_attn.png`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.5/fastervit/models/faster_vit.py` & `fastervit-0.8.6/fastervit/models/faster_vit.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.5/fastervit/models/faster_vit_any_res.py` & `fastervit-0.8.6/fastervit/models/faster_vit_any_res.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.5/fastervit/models/registry.py` & `fastervit-0.8.6/fastervit/models/registry.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.5/fastervit/scheduler/cosine_lr.py` & `fastervit-0.8.6/fastervit/scheduler/cosine_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.5/fastervit/scheduler/multistep_lr.py` & `fastervit-0.8.6/fastervit/scheduler/multistep_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.5/fastervit/scheduler/plateau_lr.py` & `fastervit-0.8.6/fastervit/scheduler/plateau_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.5/fastervit/scheduler/poly_lr.py` & `fastervit-0.8.6/fastervit/scheduler/poly_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.5/fastervit/scheduler/scheduler.py` & `fastervit-0.8.6/fastervit/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.5/fastervit/scheduler/scheduler_factory.py` & `fastervit-0.8.6/fastervit/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.5/fastervit/scheduler/step_lr.py` & `fastervit-0.8.6/fastervit/scheduler/step_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.5/fastervit/scheduler/tanh_lr.py` & `fastervit-0.8.6/fastervit/scheduler/tanh_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.5/fastervit/tensorboard.py` & `fastervit-0.8.6/fastervit/tensorboard.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.5/fastervit/train.py` & `fastervit-0.8.6/fastervit/train.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.5/fastervit/validate.py` & `fastervit-0.8.6/fastervit/validate.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.5/fastervit.egg-info/PKG-INFO` & `fastervit-0.8.6/fastervit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastervit
-Version: 0.8.5
+Version: 0.8.6
 Summary: FasterViT: Fast Vision Transformers with Hierarchical Attention
 Home-page: https://github.com/NVlabs/FasterViT
 Author: Ali Hatamizadeh
 Author-email: ahatamiz123@gmail.com
 License: NVIDIA Source Code License-NC
 Keywords: pytorch pretrained models efficientnet mobilenetv3 mnasnet resnet vision transformer vit
 Classifier: Programming Language :: Python :: 3.7
@@ -42,19 +42,19 @@
 
 <p align="center">
 <img src="https://github.com/NVlabs/FasterViT/assets/26806394/253d1a2e-b5f5-4a9b-a362-6cdd16bfccc1" width=62% height=62% 
 class="center">
 </p>
 
 
-We introduce a new self-attention mechanism, denoted as Hierarchical
+<!-- We introduce a new self-attention mechanism, denoted as Hierarchical
 Attention (HAT), that captures both short and long-range information by learning
 cross-window carrier tokens.
 
-![teaser](./fastervit/assets/hierarchial_attn.png)
+![teaser](./fastervit/assets/hierarchial_attn.png) -->
 
 
 ## 💥 News 💥
 
 - **[06.18.2023]** 🔥 We have released the FasterViT [pip package](https://pypi.org/project/fastervit/0.8.3/) !
 - **[06.17.2023]** 🔥 [Any-resolution FasterViT](https://github.com/NVlabs/FasterViT/blob/main/models/faster_vit_any_res.py)  model is now available ! the model can be used for variety of applications such as detection and segmentation or high-resolution fine-tuning with arbitrary input image resolutions. 
 - **[06.09.2023]** 🔥🔥 We have released source code and ImageNet-1K FasterViT-models !
```

### Comparing `fastervit-0.8.5/fastervit.egg-info/SOURCES.txt` & `fastervit-0.8.6/fastervit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.5/setup.py` & `fastervit-0.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='fastervit',
-    version='0.8.5',
+    version='0.8.6',
     description='FasterViT: Fast Vision Transformers with Hierarchical Attention',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/NVlabs/FasterViT',
     author='Ali Hatamizadeh',
     author_email='ahatamiz123@gmail.com',
     classifiers=[
```

