# Comparing `tmp/make-a-video-pytorch-0.2.1.tar.gz` & `tmp/make-a-video-pytorch-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "make-a-video-pytorch-0.2.1.tar", last modified: Mon Jun 19 17:49:25 2023, max compression
+gzip compressed data, was "make-a-video-pytorch-0.3.0.tar", last modified: Mon Jun 19 18:19:38 2023, max compression
```

## Comparing `make-a-video-pytorch-0.2.1.tar` & `make-a-video-pytorch-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:49:25.231940 make-a-video-pytorch-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 17:49:14.000000 make-a-video-pytorch-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-19 17:49:25.231940 make-a-video-pytorch-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-06-19 17:49:14.000000 make-a-video-pytorch-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:49:25.231940 make-a-video-pytorch-0.2.1/make_a_video_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-19 17:49:14.000000 make-a-video-pytorch-0.2.1/make_a_video_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19962 2023-06-19 17:49:14.000000 make-a-video-pytorch-0.2.1/make_a_video_pytorch/make_a_video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:49:25.231940 make-a-video-pytorch-0.2.1/make_a_video_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-19 17:49:25.000000 make-a-video-pytorch-0.2.1/make_a_video_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-19 17:49:25.000000 make-a-video-pytorch-0.2.1/make_a_video_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 17:49:25.000000 make-a-video-pytorch-0.2.1/make_a_video_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-19 17:49:25.000000 make-a-video-pytorch-0.2.1/make_a_video_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-19 17:49:25.000000 make-a-video-pytorch-0.2.1/make_a_video_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 17:49:25.231940 make-a-video-pytorch-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-19 17:49:14.000000 make-a-video-pytorch-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:19:38.512952 make-a-video-pytorch-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 18:19:28.000000 make-a-video-pytorch-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-19 18:19:38.512952 make-a-video-pytorch-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-19 18:19:28.000000 make-a-video-pytorch-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:19:38.512952 make-a-video-pytorch-0.3.0/make_a_video_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-19 18:19:28.000000 make-a-video-pytorch-0.3.0/make_a_video_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-06-19 18:19:28.000000 make-a-video-pytorch-0.3.0/make_a_video_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20350 2023-06-19 18:19:28.000000 make-a-video-pytorch-0.3.0/make_a_video_pytorch/make_a_video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:19:38.512952 make-a-video-pytorch-0.3.0/make_a_video_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-19 18:19:38.000000 make-a-video-pytorch-0.3.0/make_a_video_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-19 18:19:38.000000 make-a-video-pytorch-0.3.0/make_a_video_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 18:19:38.000000 make-a-video-pytorch-0.3.0/make_a_video_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-19 18:19:38.000000 make-a-video-pytorch-0.3.0/make_a_video_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-19 18:19:38.000000 make-a-video-pytorch-0.3.0/make_a_video_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 18:19:38.512952 make-a-video-pytorch-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-19 18:19:28.000000 make-a-video-pytorch-0.3.0/setup.py
```

### Comparing `make-a-video-pytorch-0.2.1/LICENSE` & `make-a-video-pytorch-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `make-a-video-pytorch-0.2.1/PKG-INFO` & `make-a-video-pytorch-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: make-a-video-pytorch
-Version: 0.2.1
+Version: 0.3.0
 Summary: Make-A-Video - Pytorch
 Home-page: https://github.com/lucidrains/make-a-video-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanism,text-to-video,axial convolutions
 Classifier: Development Status :: 4 - Beta
```

### Comparing `make-a-video-pytorch-0.2.1/README.md` & `make-a-video-pytorch-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -104,17 +104,20 @@
 import torch
 from make_a_video_pytorch import SpaceTimeUnet
 
 unet = SpaceTimeUnet(
     dim = 64,
     channels = 3,
     dim_mult = (1, 2, 4, 8),
+    resnet_block_depths = (1, 1, 1, 2),
     temporal_compression = (False, False, False, True),
     self_attns = (False, False, False, True),
-    condition_on_timestep = False
+    condition_on_timestep = False,
+    attn_pos_bias = False,
+    flash_attn = True
 ).cuda()
 
 # train on images
 
 images = torch.randn(1, 3, 128, 128).cuda()
 images_out  = unet(images)
 
@@ -132,16 +135,16 @@
 video_as_images_out = unet(video, enable_time = False)
 ```
 
 ## Todo
 
 - [x] give attention the best positional embeddings research has to offer
 - [x] soup up the attention
+- [x] add flash attention
 
-- [ ] add flash attention
 - [ ] make sure dalle2-pytorch can accept `SpaceTimeUnet` for training
 
 ## Citations
 
 ```bibtex
 @misc{Singer2022,
     author  = {Uriel Singer},
@@ -183,7 +186,16 @@
     title   = {NormFormer: Improved Transformer Pretraining with Extra Normalization},
     author  = {Sam Shleifer and Myle Ott},
     booktitle = {Submitted to The Tenth International Conference on Learning Representations },
     year    = {2022},
     url     = {https://openreview.net/forum?id=GMYWzWztDx5},
 }
 ```
+
+```bibtex
+@inproceedings{dao2022flashattention,
+    title   = {Flash{A}ttention: Fast and Memory-Efficient Exact Attention with {IO}-Awareness},
+    author  = {Dao, Tri and Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
+    booktitle = {Advances in Neural Information Processing Systems},
+    year    = {2022}
+}
+```
```

#### html2text {}

```diff
@@ -35,22 +35,23 @@
 heads = 8 ) video = torch.randn(1, 256, 8, 16, 16) # (batch, features, frames,
 height, width) # below it will not train across time conv_out = conv(video,
 enable_time = False) # (1, 256, 8, 16, 16) attn_out = attn(video, enable_time =
 False) # (1, 256, 8, 16, 16) ``` Full `SpaceTimeUnet` that is agnostic to
 images or video training, and where even if video is passed in, time can be
 ignored ```python import torch from make_a_video_pytorch import SpaceTimeUnet
 unet = SpaceTimeUnet( dim = 64, channels = 3, dim_mult = (1, 2, 4, 8),
-temporal_compression = (False, False, False, True), self_attns = (False, False,
-False, True), condition_on_timestep = False ).cuda() # train on images images =
-torch.randn(1, 3, 128, 128).cuda() images_out = unet(images) assert
+resnet_block_depths = (1, 1, 1, 2), temporal_compression = (False, False,
+False, True), self_attns = (False, False, False, True), condition_on_timestep =
+False, attn_pos_bias = False, flash_attn = True ).cuda() # train on images
+images = torch.randn(1, 3, 128, 128).cuda() images_out = unet(images) assert
 images.shape == images_out.shape # then train on videos video = torch.randn(1,
 3, 16, 128, 128).cuda() video_out = unet(video) assert video_out.shape ==
 video.shape # or even treat your videos as images video_as_images_out = unet
 (video, enable_time = False) ``` ## Todo - [x] give attention the best
-positional embeddings research has to offer - [x] soup up the attention - [ ]
+positional embeddings research has to offer - [x] soup up the attention - [x]
 add flash attention - [ ] make sure dalle2-pytorch can accept `SpaceTimeUnet`
 for training ## Citations ```bibtex @misc{Singer2022, author = {Uriel Singer},
 url = {https://makeavideo.studio/Make-A-Video.pdf} } ``` ```bibtex
 @inproceedings{rogozhnikov2022einops, title = {Einops: Clear and Reliable
 Tensor Manipulations with Einstein-like Notation}, author = {Alex Rogozhnikov},
 booktitle = {International Conference on Learning Representations}, year =
 {2022}, url = {https://openreview.net/forum?id=oapKSVM2bcj} } ``` ```bibtex
@@ -61,7 +62,12 @@
 {Token Shift Transformer for Video Classification}, author = {Hao Zhang and Y.
 Hao and Chong-Wah Ngo}, journal = {Proceedings of the 29th ACM International
 Conference on Multimedia}, year = {2021} } ``` ```bibtex @inproceedings
 {shleifer2022normformer, title = {NormFormer: Improved Transformer Pretraining
 with Extra Normalization}, author = {Sam Shleifer and Myle Ott}, booktitle =
 {Submitted to The Tenth International Conference on Learning Representations },
 year = {2022}, url = {https://openreview.net/forum?id=GMYWzWztDx5}, } ```
+```bibtex @inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast
+and Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri
+and Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
+booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
+} ```
```

### Comparing `make-a-video-pytorch-0.2.1/make_a_video_pytorch/make_a_video.py` & `make-a-video-pytorch-0.3.0/make_a_video_pytorch/make_a_video.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import torch
 import torch.nn.functional as F
 from torch import nn, einsum
 
 from einops import rearrange, repeat, pack, unpack
 from einops.layers.torch import Rearrange
 
+from make_a_video_pytorch.attend import Attend
+
 # helper functions
 
 def exists(val):
     return val is not None
 
 def default(val, d):
     return val if exists(val) else d
@@ -41,24 +43,25 @@
         emb = math.log(self.theta) / (half_dim - 1)
         emb = torch.exp(torch.arange(half_dim, device = device, dtype = dtype) * -emb)
         emb = rearrange(x, 'i -> i 1') * rearrange(emb, 'j -> 1 j')
         return torch.cat((emb.sin(), emb.cos()), dim = -1).type(dtype)
 
 # layernorm 3d
 
-class ChanLayerNorm(nn.Module):
-    def __init__(self, dim):
+class RMSNorm(nn.Module):
+    def __init__(self, chan, dim = 1):
         super().__init__()
-        self.g = nn.Parameter(torch.ones(dim, 1, 1, 1))
+        self.dim = dim
+        self.gamma = nn.Parameter(torch.ones(chan))
 
     def forward(self, x):
-        eps = 1e-5 if x.dtype == torch.float32 else 1e-3
-        var = torch.var(x, dim = 1, unbiased = False, keepdim = True)
-        mean = torch.mean(x, dim = 1, keepdim = True)
-        return (x - mean) * var.clamp(min = eps).rsqrt() * self.g
+        dim = self.dim
+        right_ones = (dim + 1) if dim < 0 else (x.ndim - 1 - dim)
+        gamma = self.gamma.reshape(-1, *((1,) * right_ones))
+        return F.normalize(x, dim = dim) * (x.shape[dim] ** 0.5) * gamma
 
 # feedforward
 
 def shift_token(t):
     t, t_shift = t.chunk(2, dim = 1)
     t_shift = F.pad(t_shift, (0, 0, 0, 0, 1, -1), value = 0.)
     return torch.cat((t, t_shift), dim = 1)
@@ -75,15 +78,15 @@
         inner_dim = int(dim * mult * 2 / 3)
         self.proj_in = nn.Sequential(
             nn.Conv3d(dim, inner_dim * 2, 1, bias = False),
             GEGLU()
         )
 
         self.proj_out = nn.Sequential(
-            ChanLayerNorm(inner_dim),
+            RMSNorm(inner_dim),
             nn.Conv3d(inner_dim, dim, 1, bias = False)
         )
 
     def forward(self, x, enable_time = True):
 
         is_video = x.ndim == 5
         enable_time &= is_video
@@ -176,51 +179,44 @@
 # helper classes
 
 class Attention(nn.Module):
     def __init__(
         self,
         dim,
         dim_head = 64,
-        heads = 8
+        heads = 8,
+        flash = False
     ):
         super().__init__()
         self.heads = heads
         self.scale = dim_head ** -0.5
         inner_dim = dim_head * heads
 
-        self.norm = nn.LayerNorm(dim)
+        self.attend = Attend(flash = flash)
+
+        self.norm = RMSNorm(dim, dim = -1)
 
         self.to_q = nn.Linear(dim, inner_dim, bias = False)
         self.to_kv = nn.Linear(dim, inner_dim * 2, bias = False)
         self.to_out = nn.Linear(inner_dim, dim, bias = False)
 
         nn.init.zeros_(self.to_out.weight.data) # identity with skip connection
 
     def forward(
         self,
         x,
         rel_pos_bias = None
     ):
-
         x = self.norm(x)
 
         q, k, v = self.to_q(x), *self.to_kv(x).chunk(2, dim = -1)
 
         q, k, v = map(lambda t: rearrange(t, 'b n (h d) -> b h n d', h = self.heads), (q, k, v))
 
-        q = q * self.scale
-
-        sim = einsum('b h i d, b h j d -> b h i j', q, k)
-
-        if exists(rel_pos_bias):
-            sim = sim + rel_pos_bias
-
-        attn = sim.softmax(dim = -1)
-
-        out = einsum('b h i j, b h j d -> b h i d', attn, v)
+        out = self.attend(q, k, v, bias = rel_pos_bias)
 
         out = rearrange(out, 'b h n d -> b n (h d)')
         return self.to_out(out)
 
 # main contribution - pseudo 3d conv
 
 class PseudoConv3d(nn.Module):
@@ -279,22 +275,26 @@
     def __init__(
         self,
         dim,
         *,
         dim_head = 64,
         heads = 8,
         add_feed_forward = True,
-        ff_mult = 4
+        ff_mult = 4,
+        pos_bias = True,
+        flash = False
     ):
         super().__init__()
-        self.spatial_attn = Attention(dim = dim, dim_head = dim_head, heads = heads)
-        self.spatial_rel_pos_bias = ContinuousPositionBias(dim = dim // 2, heads = heads, num_dims = 2)
+        assert not (flash and pos_bias), 'learned positional attention bias is not compatible with flash attention'
+
+        self.spatial_attn = Attention(dim = dim, dim_head = dim_head, heads = heads, flash = flash)
+        self.spatial_rel_pos_bias = ContinuousPositionBias(dim = dim // 2, heads = heads, num_dims = 2) if pos_bias else None
 
-        self.temporal_attn = Attention(dim = dim, dim_head = dim_head, heads = heads)
-        self.temporal_rel_pos_bias = ContinuousPositionBias(dim = dim // 2, heads = heads, num_dims = 1)
+        self.temporal_attn = Attention(dim = dim, dim_head = dim_head, heads = heads, flash = flash)
+        self.temporal_rel_pos_bias = ContinuousPositionBias(dim = dim // 2, heads = heads, num_dims = 1) if pos_bias else None
 
         self.has_feed_forward = add_feed_forward
         if not add_feed_forward:
             return
 
         self.ff = FeedForward(dim = dim, mult = ff_mult)
 
@@ -308,28 +308,28 @@
         enable_time &= is_video
 
         if is_video:
             x = rearrange(x, 'b c f h w -> (b f) (h w) c')
         else:
             x = rearrange(x, 'b c h w -> b (h w) c')
 
-        space_rel_pos_bias = self.spatial_rel_pos_bias(h, w)
+        space_rel_pos_bias = self.spatial_rel_pos_bias(h, w) if exists(self.spatial_rel_pos_bias) else None
 
         x = self.spatial_attn(x, rel_pos_bias = space_rel_pos_bias) + x
 
         if is_video:
             x = rearrange(x, '(b f) (h w) c -> b c f h w', b = b, h = h, w = w)
         else:
             x = rearrange(x, 'b (h w) c -> b c h w', h = h, w = w)
 
         if enable_time:
 
             x = rearrange(x, 'b c f h w -> (b h w) f c')
 
-            time_rel_pos_bias = self.temporal_rel_pos_bias(x.shape[1])
+            time_rel_pos_bias = self.temporal_rel_pos_bias(x.shape[1]) if exists(self.temporal_rel_pos_bias) else None
 
             x = self.temporal_attn(x, rel_pos_bias = time_rel_pos_bias) + x
 
             x = rearrange(x, '(b h w) f c -> b c f h w', w = w, h = h)
 
         if self.has_feed_forward:
             x = self.ff(x, enable_time = enable_time) + x
@@ -539,15 +539,17 @@
         channels = 3,
         dim_mult = (1, 2, 4, 8),
         self_attns = (False, False, False, True),
         temporal_compression = (False, True, True, True),
         resnet_block_depths = (2, 2, 2, 2),
         attn_dim_head = 64,
         attn_heads = 8,
-        condition_on_timestep = True
+        condition_on_timestep = True,
+        attn_pos_bias = True,
+        flash_attn = False
     ):
         super().__init__()
         assert len(dim_mult) == len(self_attns) == len(temporal_compression) == len(resnet_block_depths)
         num_layers = len(dim_mult)
 
         dims = [dim, *map(lambda mult: mult * dim, dim_mult)]
         dim_in_out = zip(dims[:-1], dims[1:])
@@ -572,21 +574,23 @@
         # layers
 
         self.downs = mlist([])
         self.ups = mlist([])
 
         attn_kwargs = dict(
             dim_head = attn_dim_head,
-            heads = attn_heads
+            heads = attn_heads,
+            pos_bias = attn_pos_bias,
+            flash= flash_attn
         )
 
         mid_dim = dims[-1]
 
         self.mid_block1 = ResnetBlock(mid_dim, mid_dim, timestep_cond_dim = timestep_cond_dim)
-        self.mid_attn = SpatioTemporalAttention(dim = mid_dim)
+        self.mid_attn = SpatioTemporalAttention(dim = mid_dim, **attn_kwargs)
         self.mid_block2 = ResnetBlock(mid_dim, mid_dim, timestep_cond_dim = timestep_cond_dim)
 
         for _, self_attend, (dim_in, dim_out), compress_time, resnet_block_depth in zip(range(num_layers), self_attns, dim_in_out, temporal_compression, resnet_block_depths):
             assert resnet_block_depth >= 1
 
             self.downs.append(mlist([
                 ResnetBlock(dim_in, dim_out, timestep_cond_dim = timestep_cond_dim),
```

### Comparing `make-a-video-pytorch-0.2.1/make_a_video_pytorch.egg-info/PKG-INFO` & `make-a-video-pytorch-0.3.0/make_a_video_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: make-a-video-pytorch
-Version: 0.2.1
+Version: 0.3.0
 Summary: Make-A-Video - Pytorch
 Home-page: https://github.com/lucidrains/make-a-video-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanism,text-to-video,axial convolutions
 Classifier: Development Status :: 4 - Beta
```

### Comparing `make-a-video-pytorch-0.2.1/setup.py` & `make-a-video-pytorch-0.3.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'make-a-video-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.2.1',
+  version = '0.3.0',
   license='MIT',
   description = 'Make-A-Video - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/make-a-video-pytorch',
   keywords = [
```

