# Comparing `tmp/make-a-video-pytorch-0.2.0.tar.gz` & `tmp/make-a-video-pytorch-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "make-a-video-pytorch-0.2.0.tar", last modified: Wed Mar 22 20:29:16 2023, max compression
+gzip compressed data, was "make-a-video-pytorch-0.2.1.tar", last modified: Mon Jun 19 17:49:25 2023, max compression
```

## Comparing `make-a-video-pytorch-0.2.0.tar` & `make-a-video-pytorch-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 20:29:16.310652 make-a-video-pytorch-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-22 20:29:02.000000 make-a-video-pytorch-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-22 20:29:16.310652 make-a-video-pytorch-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-03-22 20:29:02.000000 make-a-video-pytorch-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 20:29:16.310652 make-a-video-pytorch-0.2.0/make_a_video_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-22 20:29:02.000000 make-a-video-pytorch-0.2.0/make_a_video_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19716 2023-03-22 20:29:02.000000 make-a-video-pytorch-0.2.0/make_a_video_pytorch/make_a_video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 20:29:16.310652 make-a-video-pytorch-0.2.0/make_a_video_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-22 20:29:16.000000 make-a-video-pytorch-0.2.0/make_a_video_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-22 20:29:16.000000 make-a-video-pytorch-0.2.0/make_a_video_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 20:29:16.000000 make-a-video-pytorch-0.2.0/make_a_video_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-22 20:29:16.000000 make-a-video-pytorch-0.2.0/make_a_video_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-22 20:29:16.000000 make-a-video-pytorch-0.2.0/make_a_video_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 20:29:16.310652 make-a-video-pytorch-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-03-22 20:29:02.000000 make-a-video-pytorch-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:49:25.231940 make-a-video-pytorch-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 17:49:14.000000 make-a-video-pytorch-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-19 17:49:25.231940 make-a-video-pytorch-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-06-19 17:49:14.000000 make-a-video-pytorch-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:49:25.231940 make-a-video-pytorch-0.2.1/make_a_video_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-19 17:49:14.000000 make-a-video-pytorch-0.2.1/make_a_video_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19962 2023-06-19 17:49:14.000000 make-a-video-pytorch-0.2.1/make_a_video_pytorch/make_a_video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:49:25.231940 make-a-video-pytorch-0.2.1/make_a_video_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-19 17:49:25.000000 make-a-video-pytorch-0.2.1/make_a_video_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-19 17:49:25.000000 make-a-video-pytorch-0.2.1/make_a_video_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 17:49:25.000000 make-a-video-pytorch-0.2.1/make_a_video_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-19 17:49:25.000000 make-a-video-pytorch-0.2.1/make_a_video_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-19 17:49:25.000000 make-a-video-pytorch-0.2.1/make_a_video_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 17:49:25.231940 make-a-video-pytorch-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-19 17:49:14.000000 make-a-video-pytorch-0.2.1/setup.py
```

### Comparing `make-a-video-pytorch-0.2.0/LICENSE` & `make-a-video-pytorch-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `make-a-video-pytorch-0.2.0/PKG-INFO` & `make-a-video-pytorch-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: make-a-video-pytorch
-Version: 0.2.0
+Version: 0.2.1
 Summary: Make-A-Video - Pytorch
 Home-page: https://github.com/lucidrains/make-a-video-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanism,text-to-video,axial convolutions
 Classifier: Development Status :: 4 - Beta
```

### Comparing `make-a-video-pytorch-0.2.0/README.md` & `make-a-video-pytorch-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -133,14 +133,15 @@
 ```
 
 ## Todo
 
 - [x] give attention the best positional embeddings research has to offer
 - [x] soup up the attention
 
+- [ ] add flash attention
 - [ ] make sure dalle2-pytorch can accept `SpaceTimeUnet` for training
 
 ## Citations
 
 ```bibtex
 @misc{Singer2022,
     author  = {Uriel Singer},
@@ -174,16 +175,15 @@
     author  = {Hao Zhang and Y. Hao and Chong-Wah Ngo},
     journal = {Proceedings of the 29th ACM International Conference on Multimedia},
     year    = {2021}
 }
 ```
 
 ```bibtex
-@inproceedings{anonymous2022normformer,
+@inproceedings{shleifer2022normformer,
     title   = {NormFormer: Improved Transformer Pretraining with Extra Normalization},
-    author  = {Anonymous},
+    author  = {Sam Shleifer and Myle Ott},
     booktitle = {Submitted to The Tenth International Conference on Learning Representations },
     year    = {2022},
     url     = {https://openreview.net/forum?id=GMYWzWztDx5},
-    note    = {under review}
 }
 ```
```

#### html2text {}

```diff
@@ -43,26 +43,25 @@
 False, True), condition_on_timestep = False ).cuda() # train on images images =
 torch.randn(1, 3, 128, 128).cuda() images_out = unet(images) assert
 images.shape == images_out.shape # then train on videos video = torch.randn(1,
 3, 16, 128, 128).cuda() video_out = unet(video) assert video_out.shape ==
 video.shape # or even treat your videos as images video_as_images_out = unet
 (video, enable_time = False) ``` ## Todo - [x] give attention the best
 positional embeddings research has to offer - [x] soup up the attention - [ ]
-make sure dalle2-pytorch can accept `SpaceTimeUnet` for training ## Citations
-```bibtex @misc{Singer2022, author = {Uriel Singer}, url = {https://
-makeavideo.studio/Make-A-Video.pdf} } ``` ```bibtex @inproceedings
-{rogozhnikov2022einops, title = {Einops: Clear and Reliable Tensor
-Manipulations with Einstein-like Notation}, author = {Alex Rogozhnikov},
+add flash attention - [ ] make sure dalle2-pytorch can accept `SpaceTimeUnet`
+for training ## Citations ```bibtex @misc{Singer2022, author = {Uriel Singer},
+url = {https://makeavideo.studio/Make-A-Video.pdf} } ``` ```bibtex
+@inproceedings{rogozhnikov2022einops, title = {Einops: Clear and Reliable
+Tensor Manipulations with Einstein-like Notation}, author = {Alex Rogozhnikov},
 booktitle = {International Conference on Learning Representations}, year =
 {2022}, url = {https://openreview.net/forum?id=oapKSVM2bcj} } ``` ```bibtex
 @article{Dong2021AttentionIN, title = {Attention is Not All You Need: Pure
 Attention Loses Rank Doubly Exponentially with Depth}, author = {Yihe Dong and
 Jean-Baptiste Cordonnier and Andreas Loukas}, journal = {ArXiv}, year = {2021},
 volume = {abs/2103.03404} } ``` ```bibtex @article{Zhang2021TokenST, title =
 {Token Shift Transformer for Video Classification}, author = {Hao Zhang and Y.
 Hao and Chong-Wah Ngo}, journal = {Proceedings of the 29th ACM International
 Conference on Multimedia}, year = {2021} } ``` ```bibtex @inproceedings
-{anonymous2022normformer, title = {NormFormer: Improved Transformer Pretraining
-with Extra Normalization}, author = {Anonymous}, booktitle = {Submitted to The
-Tenth International Conference on Learning Representations }, year = {2022},
-url = {https://openreview.net/forum?id=GMYWzWztDx5}, note = {under review} }
-```
+{shleifer2022normformer, title = {NormFormer: Improved Transformer Pretraining
+with Extra Normalization}, author = {Sam Shleifer and Myle Ott}, booktitle =
+{Submitted to The Tenth International Conference on Learning Representations },
+year = {2022}, url = {https://openreview.net/forum?id=GMYWzWztDx5}, } ```
```

### Comparing `make-a-video-pytorch-0.2.0/make_a_video_pytorch/make_a_video.py` & `make-a-video-pytorch-0.2.1/make_a_video_pytorch/make_a_video.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,20 +80,32 @@
 
         self.proj_out = nn.Sequential(
             ChanLayerNorm(inner_dim),
             nn.Conv3d(inner_dim, dim, 1, bias = False)
         )
 
     def forward(self, x, enable_time = True):
+
+        is_video = x.ndim == 5
+        enable_time &= is_video
+
+        if not is_video:
+            x = rearrange(x, 'b c h w -> b c 1 h w')
+
         x = self.proj_in(x)
 
         if enable_time:
             x = shift_token(x)
 
-        return self.proj_out(x)
+        out = self.proj_out(x)
+
+        if not is_video:
+            out = rearrange(out, 'b c 1 h w -> b c h w')
+
+        return out
 
 # best relative positional encoding
 
 class ContinuousPositionBias(nn.Module):
     """ from https://arxiv.org/abs/2111.09883 """
 
     def __init__(
```

### Comparing `make-a-video-pytorch-0.2.0/make_a_video_pytorch.egg-info/PKG-INFO` & `make-a-video-pytorch-0.2.1/make_a_video_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: make-a-video-pytorch
-Version: 0.2.0
+Version: 0.2.1
 Summary: Make-A-Video - Pytorch
 Home-page: https://github.com/lucidrains/make-a-video-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanism,text-to-video,axial convolutions
 Classifier: Development Status :: 4 - Beta
```

### Comparing `make-a-video-pytorch-0.2.0/setup.py` & `make-a-video-pytorch-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'make-a-video-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.2.0',
+  version = '0.2.1',
   license='MIT',
   description = 'Make-A-Video - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/make-a-video-pytorch',
   keywords = [
```

