# Comparing `tmp/denoising-diffusion-pytorch-1.7.4.tar.gz` & `tmp/denoising-diffusion-pytorch-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.7.4.tar", last modified: Mon Jun 19 02:42:19 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.7.5.tar", last modified: Mon Jun 19 04:19:17 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.7.4.tar` & `denoising-diffusion-pytorch-1.7.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:42:19.760907 denoising-diffusion-pytorch-1.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 02:42:19.760907 denoising-diffusion-pytorch-1.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:42:19.760907 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27756 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    35612 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    29598 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    35562 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21169 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:42:19.760907 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 02:42:19.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-19 02:42:19.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 02:42:19.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 02:42:19.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 02:42:19.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 02:42:19.760907 denoising-diffusion-pytorch-1.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:19:17.730773 denoising-diffusion-pytorch-1.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 04:19:17.730773 denoising-diffusion-pytorch-1.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:19:17.730773 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35643 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:19:17.730773 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 04:19:17.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-19 04:19:17.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 04:19:17.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 04:19:17.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 04:19:17.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 04:19:17.730773 denoising-diffusion-pytorch-1.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.7.4/LICENSE` & `denoising-diffusion-pytorch-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.4/PKG-INFO` & `denoising-diffusion-pytorch-1.7.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.7.4
+Version: 1.7.5
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.7.4/README.md` & `denoising-diffusion-pytorch-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from functools import partial
 from collections import namedtuple
 from multiprocessing import cpu_count
 
 import torch
 from torch import nn, einsum
 import torch.nn.functional as F
+from torch.cuda.amp import autocast
 
 from einops import rearrange, reduce, repeat
 from einops.layers.torch import Rearrange
 
 from tqdm.auto import tqdm
 
 # constants
@@ -707,14 +708,15 @@
 
         img = (1 - lam) * xt1 + lam * xt2
         for i in tqdm(reversed(range(0, t)), desc = 'interpolation sample time step', total = t):
             img = self.p_sample(img, torch.full((b,), i, device=device, dtype=torch.long))
 
         return img
 
+    @autocast(enabled = False)
     def q_sample(self, x_start, t, noise=None):
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         if self.offset_noise_strength > 0.:
             offset_noise = torch.randn(x_start.shape[:2], device = self.device)
             noise += self.offset_noise_strength * rearrange(offset_noise, 'b c -> b c 1 1')
```

### Comparing `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import math
 import torch
 from torch import sqrt
 from torch import nn, einsum
 import torch.nn.functional as F
+from torch.cuda.amp import autocast
 from torch.special import expm1
 
 from tqdm import tqdm
 from einops import rearrange, repeat, reduce
 from einops.layers.torch import Rearrange
 
 # helpers
@@ -229,14 +230,15 @@
 
     @torch.no_grad()
     def sample(self, batch_size = 16):
         return self.p_sample_loop((batch_size, self.channels, self.image_size, self.image_size))
 
     # training related functions - noise prediction
 
+    @autocast(enabled = False)
     def q_sample(self, x_start, times, noise = None):
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         log_snr = self.log_snr(times)
 
         log_snr_padded = right_pad_dims_to(x_start, log_snr)
         alpha, sigma = sqrt(log_snr_padded.sigmoid()), sqrt((-log_snr_padded).sigmoid())
```

### Comparing `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -702,14 +702,15 @@
 
         for i in tqdm(reversed(range(0, t)), desc = 'interpolation sample time step', total = t):
             self_cond = x_start if self.self_condition else None
             img, x_start = self.p_sample(img, i, self_cond)
 
         return img
 
+    @autocast(enabled = False)
     def q_sample(self, x_start, t, noise = None):
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         return (
             extract(self.sqrt_alphas_cumprod, t, x_start.shape) * x_start +
             extract(self.sqrt_one_minus_alphas_cumprod, t, x_start.shape) * noise
         )
```

### Comparing `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from collections import namedtuple
 
 import torch
 from accelerate import Accelerator
 from ema_pytorch import EMA
 from torch import nn, einsum
 import torch.nn.functional as F
+from torch.cuda.amp import autocast
 
 from einops import rearrange, reduce
 from einops.layers.torch import Rearrange
 from torch.optim import Adam
 from torch.utils.data import Dataset, DataLoader
 
 from tqdm.auto import tqdm
@@ -635,14 +636,15 @@
 
         for i in tqdm(reversed(range(0, t)), desc = 'interpolation sample time step', total = t):
             self_cond = x_start if self.self_condition else None
             img, x_start = self.p_sample(img, i, self_cond)
 
         return img
 
+    @autocast(enabled = False)
     def q_sample(self, x_start, t, noise=None):
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         return (
             extract(self.sqrt_alphas_cumprod, t, x_start.shape) * x_start +
             extract(self.sqrt_one_minus_alphas_cumprod, t, x_start.shape) * noise
         )
```

### Comparing `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from functools import partial
 from collections import namedtuple
 from multiprocessing import cpu_count
 
 import torch
 from torch import nn, einsum
 import torch.nn.functional as F
+from torch.cuda.amp import autocast
 from torch.utils.data import Dataset, DataLoader
 
 from torch.optim import Adam
 from torchvision import transforms as T, utils
 
 from einops import rearrange, reduce
 from einops.layers.torch import Rearrange
@@ -704,14 +705,15 @@
 
         for i in tqdm(reversed(range(0, t)), desc = 'interpolation sample time step', total = t):
             self_cond = x_start if self.self_condition else None
             img, x_start = self.p_sample(img, i, self_cond)
 
         return img
 
+    @autocast(enabled = False)
     def q_sample(self, x_start, t, noise=None):
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         return (
             extract(self.sqrt_alphas_cumprod, t, x_start.shape) * x_start +
             extract(self.sqrt_one_minus_alphas_cumprod, t, x_start.shape) * noise
         )
```

### Comparing `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from functools import partial, wraps
 
 import torch
 from torch import sqrt
 from torch import nn, einsum
 import torch.nn.functional as F
 from torch.special import expm1
+from torch.cuda.amp import autocast
 
 from tqdm import tqdm
 from einops import rearrange, repeat, reduce, pack, unpack
 from einops.layers.torch import Rearrange
 
 # helpers
 
@@ -649,14 +650,15 @@
 
     @torch.no_grad()
     def sample(self, batch_size = 16):
         return self.p_sample_loop((batch_size, self.channels, self.image_size, self.image_size))
 
     # training related functions - noise prediction
 
+    @autocast(enabled = False)
     def q_sample(self, x_start, times, noise = None):
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         log_snr = self.log_snr(times)
 
         log_snr_padded = right_pad_dims_to(x_start, log_snr)
         alpha, sigma = sqrt(log_snr_padded.sigmoid()), sqrt((-log_snr_padded).sigmoid())
```

### Comparing `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import math
 import torch
 from torch import sqrt
 from torch import nn, einsum
 import torch.nn.functional as F
 from torch.special import expm1
+from torch.cuda.amp import autocast
 
 from tqdm import tqdm
 from einops import rearrange, repeat, reduce
 from einops.layers.torch import Rearrange
 
 # helpers
 
@@ -145,14 +146,15 @@
 
     @torch.no_grad()
     def sample(self, batch_size = 16):
         return self.p_sample_loop((batch_size, self.channels, self.image_size, self.image_size))
 
     # training related functions - noise prediction
 
+    @autocast(enabled = False)
     def q_sample(self, x_start, times, noise = None):
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         log_snr = self.log_snr(times)
 
         log_snr_padded = right_pad_dims_to(x_start, log_snr)
         alpha, sigma = sqrt(log_snr_padded.sigmoid()), sqrt((-log_snr_padded).sigmoid())
```

### Comparing `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.7.4
+Version: 1.7.5
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.4/setup.py` & `denoising-diffusion-pytorch-1.7.5/setup.py`

 * *Files identical despite different names*

