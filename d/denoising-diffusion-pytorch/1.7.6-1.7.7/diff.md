# Comparing `tmp/denoising-diffusion-pytorch-1.7.6.tar.gz` & `tmp/denoising-diffusion-pytorch-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.7.6.tar", last modified: Mon Jun 19 04:48:09 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.7.7.tar", last modified: Mon Jun 19 14:52:54 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.7.6.tar` & `denoising-diffusion-pytorch-1.7.7.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:48:09.920618 denoising-diffusion-pytorch-1.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 04:48:09.920618 denoising-diffusion-pytorch-1.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:48:09.920618 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    35717 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:48:09.920618 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 04:48:09.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-19 04:48:09.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 04:48:09.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 04:48:09.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 04:48:09.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 04:48:09.920618 denoising-diffusion-pytorch-1.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:52:54.665455 denoising-diffusion-pytorch-1.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 14:52:54.665455 denoising-diffusion-pytorch-1.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10255 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:52:54.665455 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35880 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/fid_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:52:54.665455 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 14:52:54.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-19 14:52:54.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 14:52:54.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 14:52:54.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 14:52:54.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 14:52:54.665455 denoising-diffusion-pytorch-1.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.7.6/LICENSE` & `denoising-diffusion-pytorch-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.6/PKG-INFO` & `denoising-diffusion-pytorch-1.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.7.6
+Version: 1.7.7
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.7.6/README.md` & `denoising-diffusion-pytorch-1.7.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,15 @@
 ```
 
 ## Miscellaneous
 
 ### 1D Sequence
 
 By popular request, a 1D Unet + Gaussian Diffusion implementation.
+
 ```python
 import torch
 from denoising_diffusion_pytorch import Unet1D, GaussianDiffusion1D, Trainer1D
 
 model = Unet1D(
     dim = 64,
     dim_mults = (1, 2, 4, 8),
@@ -142,15 +143,17 @@
 
 # after a lot of training
 
 sampled_seq = diffusion.sample(batch_size = 4)
 sampled_seq.shape # (4, 32, 128)
 
 ```
-`Trainer1D` does not evaluate the generated samples in any way since the type of data is not known. 
+
+`Trainer1D` does not evaluate the generated samples in any way since the type of data is not known.
+
 You could consider adding a suitable metric to the training loop yourself after doing an editable install of this package
 `pip install -e .`.
 
 ## Todo
 
 - [ ] add flash attention, do full attention at 64x64, linear attention at anything above
```

### Comparing `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,36 +4,31 @@
 from random import random
 from functools import partial
 from collections import namedtuple
 from multiprocessing import cpu_count
 
 import torch
 from torch import nn, einsum
-from torch.cuda.amp import autocast
 import torch.nn.functional as F
+from torch.cuda.amp import autocast
 from torch.utils.data import Dataset, DataLoader
 
 from torch.optim import Adam
-
 from torchvision import transforms as T, utils
 
-from einops import rearrange, reduce, repeat
+from einops import rearrange, reduce
 from einops.layers.torch import Rearrange
 
 from PIL import Image
 from tqdm.auto import tqdm
 from ema_pytorch import EMA
 
 from accelerate import Accelerator
 
-import numpy as np
-from pytorch_fid.inception import InceptionV3
-from pytorch_fid.fid_score import calculate_frechet_distance
-
-from denoising_diffusion_pytorch.version import __version__
+# from denoising_diffusion_pytorch.version import __version__
 
 # constants
 
 ModelPrediction =  namedtuple('ModelPrediction', ['pred_noise', 'pred_x_start'])
 
 # helpers functions
 
@@ -101,15 +96,15 @@
 
 class RMSNorm(nn.Module):
     def __init__(self, dim):
         super().__init__()
         self.g = nn.Parameter(torch.ones(1, dim, 1, 1))
 
     def forward(self, x):
-        return F.normalize(x, dim = 1) * self.g * (x.shape[1] ** 0.5)
+        return F.normalize(x, dim = 1) * self.g * (x.shape[-1] ** 0.5)
 
 class PreNorm(nn.Module):
     def __init__(self, dim, fn):
         super().__init__()
         self.fn = fn
         self.norm = RMSNorm(dim)
 
@@ -418,38 +413,38 @@
     t = torch.linspace(0, timesteps, steps, dtype = torch.float64) / timesteps
     v_start = torch.tensor(start / tau).sigmoid()
     v_end = torch.tensor(end / tau).sigmoid()
     alphas_cumprod = (-((t * (end - start) + start) / tau).sigmoid() + v_end) / (v_end - v_start)
     alphas_cumprod = alphas_cumprod / alphas_cumprod[0]
     betas = 1 - (alphas_cumprod[1:] / alphas_cumprod[:-1])
     return torch.clip(betas, 0, 0.999)
+    
 
+    
 class GaussianDiffusion(nn.Module):
     def __init__(
         self,
         model,
         *,
         image_size,
         timesteps = 1000,
         sampling_timesteps = None,
-        objective = 'pred_v',
+        objective = 'pred_noise',
         beta_schedule = 'sigmoid',
         schedule_fn_kwargs = dict(),
         ddim_sampling_eta = 0.,
         auto_normalize = True,
-        offset_noise_strength = 0.,  # https://www.crosslabs.org/blog/diffusion-with-offset-noise
-        min_snr_loss_weight = False, # https://arxiv.org/abs/2303.09556
+        min_snr_loss_weight = False,
         min_snr_gamma = 5
     ):
         super().__init__()
         assert not (type(self) == GaussianDiffusion and model.channels != model.out_dim)
         assert not model.random_or_learned_sinusoidal_cond
 
         self.model = model
-
         self.channels = self.model.channels
         self.self_condition = self.model.self_condition
 
         self.image_size = image_size
 
         self.objective = objective
 
@@ -507,45 +502,36 @@
 
         # below: log calculation clipped because the posterior variance is 0 at the beginning of the diffusion chain
 
         register_buffer('posterior_log_variance_clipped', torch.log(posterior_variance.clamp(min =1e-20)))
         register_buffer('posterior_mean_coef1', betas * torch.sqrt(alphas_cumprod_prev) / (1. - alphas_cumprod))
         register_buffer('posterior_mean_coef2', (1. - alphas_cumprod_prev) * torch.sqrt(alphas) / (1. - alphas_cumprod))
 
-        # offset noise strength - in blogpost, they claimed 0.1 was ideal
-
-        self.offset_noise_strength = offset_noise_strength
-
-        # derive loss weight
-        # snr - signal noise ratio
+        # loss weight
 
         snr = alphas_cumprod / (1 - alphas_cumprod)
 
-        # https://arxiv.org/abs/2303.09556
-
         maybe_clipped_snr = snr.clone()
         if min_snr_loss_weight:
             maybe_clipped_snr.clamp_(max = min_snr_gamma)
 
         if objective == 'pred_noise':
-            register_buffer('loss_weight', maybe_clipped_snr / snr)
+            loss_weight = maybe_clipped_snr / snr
         elif objective == 'pred_x0':
-            register_buffer('loss_weight', maybe_clipped_snr)
+            loss_weight = maybe_clipped_snr
         elif objective == 'pred_v':
-            register_buffer('loss_weight', maybe_clipped_snr / (snr + 1))
+            loss_weight = maybe_clipped_snr / (snr + 1)
+
+        register_buffer('loss_weight', loss_weight)
 
         # auto-normalization of data [0, 1] -> [-1, 1] - can turn off by setting it to be False
 
         self.normalize = normalize_to_neg_one_to_one if auto_normalize else identity
         self.unnormalize = unnormalize_to_zero_to_one if auto_normalize else identity
 
-    @property
-    def device(self):
-        return self.betas.device
-
     def predict_start_from_noise(self, x_t, t, noise):
         return (
             extract(self.sqrt_recip_alphas_cumprod, t, x_t.shape) * x_t -
             extract(self.sqrt_recipm1_alphas_cumprod, t, x_t.shape) * noise
         )
 
     def predict_noise_from_start(self, x_t, t, x0):
@@ -571,26 +557,23 @@
             extract(self.posterior_mean_coef1, t, x_t.shape) * x_start +
             extract(self.posterior_mean_coef2, t, x_t.shape) * x_t
         )
         posterior_variance = extract(self.posterior_variance, t, x_t.shape)
         posterior_log_variance_clipped = extract(self.posterior_log_variance_clipped, t, x_t.shape)
         return posterior_mean, posterior_variance, posterior_log_variance_clipped
 
-    def model_predictions(self, x, t, x_self_cond = None, clip_x_start = False, rederive_pred_noise = False):
+    def model_predictions(self, x, t, x_self_cond = None, clip_x_start = False):
         model_output = self.model(x, t, x_self_cond)
         maybe_clip = partial(torch.clamp, min = -1., max = 1.) if clip_x_start else identity
 
         if self.objective == 'pred_noise':
             pred_noise = model_output
             x_start = self.predict_start_from_noise(x, t, pred_noise)
             x_start = maybe_clip(x_start)
 
-            if clip_x_start and rederive_pred_noise:
-                pred_noise = self.predict_noise_from_start(x, t, x_start)
-
         elif self.objective == 'pred_x0':
             x_start = model_output
             x_start = maybe_clip(x_start)
             pred_noise = self.predict_noise_from_start(x, t, x_start)
 
         elif self.objective == 'pred_v':
             v = model_output
@@ -605,90 +588,110 @@
         x_start = preds.pred_x_start
 
         if clip_denoised:
             x_start.clamp_(-1., 1.)
 
         model_mean, posterior_variance, posterior_log_variance = self.q_posterior(x_start = x_start, x_t = x, t = t)
         return model_mean, posterior_variance, posterior_log_variance, x_start
+     
+    def condition_mean(self, cond_fn, mean,variance, x, t, guidance_kwargs=None):
+        """
+        Compute the mean for the previous step, given a function cond_fn that
+        computes the gradient of a conditional log probability with respect to
+        x. In particular, cond_fn computes grad(log(p(y|x))), and we want to
+        condition on y.
+        This uses the conditioning strategy from Sohl-Dickstein et al. (2015).
+        """
+        gradient = cond_fn(x, t, **guidance_kwargs)
+        new_mean = (
+            mean.float() + variance * gradient.float()
+        )
+        print("gradient: ",(variance * gradient.float()).mean())
+        return new_mean
 
+        
     @torch.no_grad()
-    def p_sample(self, x, t: int, x_self_cond = None):
-        b, *_, device = *x.shape, self.device
-        batched_times = torch.full((b,), t, device = device, dtype = torch.long)
-        model_mean, _, model_log_variance, x_start = self.p_mean_variance(x = x, t = batched_times, x_self_cond = x_self_cond, clip_denoised = True)
+    def p_sample(self, x, t: int, x_self_cond = None, cond_fn=None, guidance_kwargs=None):
+        b, *_, device = *x.shape, x.device
+        batched_times = torch.full((b,), t, device = x.device, dtype = torch.long)
+        model_mean, variance, model_log_variance, x_start = self.p_mean_variance(
+            x = x, t = batched_times, x_self_cond = x_self_cond, clip_denoised = True
+        )
+        if exists(cond_fn) and exists(guidance_kwargs):
+            model_mean = self.condition_mean(cond_fn, model_mean, variance, x, batched_times, guidance_kwargs)
+        
         noise = torch.randn_like(x) if t > 0 else 0. # no noise if t == 0
         pred_img = model_mean + (0.5 * model_log_variance).exp() * noise
         return pred_img, x_start
 
     @torch.no_grad()
-    def p_sample_loop(self, shape, return_all_timesteps = False):
-        batch, device = shape[0], self.device
+    def p_sample_loop(self, shape, return_all_timesteps = False, cond_fn=None, guidance_kwargs=None):
+        batch, device = shape[0], self.betas.device
 
         img = torch.randn(shape, device = device)
         imgs = [img]
 
         x_start = None
 
         for t in tqdm(reversed(range(0, self.num_timesteps)), desc = 'sampling loop time step', total = self.num_timesteps):
             self_cond = x_start if self.self_condition else None
-            img, x_start = self.p_sample(img, t, self_cond)
+            img, x_start = self.p_sample(img, t, self_cond, cond_fn, guidance_kwargs)
             imgs.append(img)
 
         ret = img if not return_all_timesteps else torch.stack(imgs, dim = 1)
 
         ret = self.unnormalize(ret)
         return ret
 
     @torch.no_grad()
-    def ddim_sample(self, shape, return_all_timesteps = False):
-        batch, device, total_timesteps, sampling_timesteps, eta, objective = shape[0], self.device, self.num_timesteps, self.sampling_timesteps, self.ddim_sampling_eta, self.objective
+    def ddim_sample(self, shape, return_all_timesteps = False, cond_fn=None, guidance_kwargs=None):
+        batch, device, total_timesteps, sampling_timesteps, eta, objective = shape[0], self.betas.device, self.num_timesteps, self.sampling_timesteps, self.ddim_sampling_eta, self.objective
 
         times = torch.linspace(-1, total_timesteps - 1, steps = sampling_timesteps + 1)   # [-1, 0, 1, 2, ..., T-1] when sampling_timesteps == total_timesteps
         times = list(reversed(times.int().tolist()))
         time_pairs = list(zip(times[:-1], times[1:])) # [(T-1, T-2), (T-2, T-3), ..., (1, 0), (0, -1)]
 
         img = torch.randn(shape, device = device)
         imgs = [img]
 
         x_start = None
 
         for time, time_next in tqdm(time_pairs, desc = 'sampling loop time step'):
             time_cond = torch.full((batch,), time, device = device, dtype = torch.long)
             self_cond = x_start if self.self_condition else None
-            pred_noise, x_start, *_ = self.model_predictions(img, time_cond, self_cond, clip_x_start = True, rederive_pred_noise = True)
+            pred_noise, x_start, *_ = self.model_predictions(img, time_cond, self_cond, clip_x_start = True)
+
+            imgs.append(img)
 
             if time_next < 0:
                 img = x_start
-                imgs.append(img)
                 continue
 
             alpha = self.alphas_cumprod[time]
             alpha_next = self.alphas_cumprod[time_next]
 
             sigma = eta * ((1 - alpha / alpha_next) * (1 - alpha_next) / (1 - alpha)).sqrt()
             c = (1 - alpha_next - sigma ** 2).sqrt()
 
             noise = torch.randn_like(img)
 
             img = x_start * alpha_next.sqrt() + \
                   c * pred_noise + \
                   sigma * noise
 
-            imgs.append(img)
-
         ret = img if not return_all_timesteps else torch.stack(imgs, dim = 1)
 
         ret = self.unnormalize(ret)
         return ret
 
     @torch.no_grad()
-    def sample(self, batch_size = 16, return_all_timesteps = False):
+    def sample(self, batch_size = 16, return_all_timesteps = False, cond_fn=None, guidance_kwargs=None):
         image_size, channels = self.image_size, self.channels
         sample_fn = self.p_sample_loop if not self.is_ddim_sampling else self.ddim_sample
-        return sample_fn((batch_size, channels, image_size, image_size), return_all_timesteps = return_all_timesteps)
+        return sample_fn((batch_size, channels, image_size, image_size), return_all_timesteps = return_all_timesteps, cond_fn=cond_fn, guidance_kwargs=guidance_kwargs)
 
     @torch.no_grad()
     def interpolate(self, x1, x2, t = None, lam = 0.5):
         b, *_, device = *x1.shape, x1.device
         t = default(t, self.num_timesteps - 1)
 
         assert x1.shape == x2.shape
@@ -703,35 +706,26 @@
         for i in tqdm(reversed(range(0, t)), desc = 'interpolation sample time step', total = t):
             self_cond = x_start if self.self_condition else None
             img, x_start = self.p_sample(img, i, self_cond)
 
         return img
 
     @autocast(enabled = False)
-    def q_sample(self, x_start, t, noise = None):
+    def q_sample(self, x_start, t, noise=None):
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         return (
             extract(self.sqrt_alphas_cumprod, t, x_start.shape) * x_start +
             extract(self.sqrt_one_minus_alphas_cumprod, t, x_start.shape) * noise
         )
 
-    def p_losses(self, x_start, t, noise = None, offset_noise_strength = None):
+    def p_losses(self, x_start, t, noise = None):
         b, c, h, w = x_start.shape
-
         noise = default(noise, lambda: torch.randn_like(x_start))
 
-        # offset noise - https://www.crosslabs.org/blog/diffusion-with-offset-noise
-
-        offset_noise_strength = default(offset_noise_strength, self.offset_noise_strength)
-
-        if offset_noise_strength > 0.:
-            offset_noise = torch.randn(x_start.shape[:2], device = self.device)
-            noise += offset_noise_strength * rearrange(offset_noise, 'b c -> b c 1 1')
-
         # noise sample
 
         x = self.q_sample(x_start = x_start, t = t, noise = noise)
 
         # if doing self-conditioning, 50% of the time, predict x_start from current set of times
         # and condition with unet with that
         # this technique will slow down training by 25%, but seems to lower FID significantly
@@ -820,59 +814,39 @@
         ema_update_every = 10,
         ema_decay = 0.995,
         adam_betas = (0.9, 0.99),
         save_and_sample_every = 1000,
         num_samples = 25,
         results_folder = './results',
         amp = False,
-        mixed_precision_type = 'fp16',
+        fp16 = False,
         split_batches = True,
-        convert_image_to = None,
-        calculate_fid = True,
-        inception_block_idx = 2048,
-        max_grad_norm = 1.
+        convert_image_to = None
     ):
         super().__init__()
 
-        # accelerator
-
         self.accelerator = Accelerator(
             split_batches = split_batches,
-            mixed_precision = mixed_precision_type if amp else 'no'
+            mixed_precision = 'fp16' if fp16 else 'no'
         )
 
-        # model
+        self.accelerator.native_amp = amp
 
         self.model = diffusion_model
-        self.channels = diffusion_model.channels
-
-        # InceptionV3 for fid-score computation
-
-        self.inception_v3 = None
-
-        if calculate_fid:
-            assert inception_block_idx in InceptionV3.BLOCK_INDEX_BY_DIM
-            block_idx = InceptionV3.BLOCK_INDEX_BY_DIM[inception_block_idx]
-            self.inception_v3 = InceptionV3([block_idx])
-            self.inception_v3.to(self.device)
-
-        # sampling and training hyperparameters
 
         assert has_int_squareroot(num_samples), 'number of samples must have an integer square root'
         self.num_samples = num_samples
         self.save_and_sample_every = save_and_sample_every
 
         self.batch_size = train_batch_size
         self.gradient_accumulate_every = gradient_accumulate_every
 
         self.train_num_steps = train_num_steps
         self.image_size = diffusion_model.image_size
 
-        self.max_grad_norm = max_grad_norm
-
         # dataset and dataloader
 
         self.ds = Dataset(folder, self.image_size, augment_horizontal_flip = augment_horizontal_flip, convert_image_to = convert_image_to)
         dl = DataLoader(self.ds, batch_size = train_batch_size, shuffle = True, pin_memory = True, num_workers = cpu_count())
 
         dl = self.accelerator.prepare(dl)
         self.dl = cycle(dl)
@@ -881,31 +855,26 @@
 
         self.opt = Adam(diffusion_model.parameters(), lr = train_lr, betas = adam_betas)
 
         # for logging results in a folder periodically
 
         if self.accelerator.is_main_process:
             self.ema = EMA(diffusion_model, beta = ema_decay, update_every = ema_update_every)
-            self.ema.to(self.device)
 
         self.results_folder = Path(results_folder)
         self.results_folder.mkdir(exist_ok = True)
 
         # step counter state
 
         self.step = 0
 
         # prepare model, dataloader, optimizer with accelerator
 
         self.model, self.opt = self.accelerator.prepare(self.model, self.opt)
 
-    @property
-    def device(self):
-        return self.accelerator.device
-
     def save(self, milestone):
         if not self.accelerator.is_local_main_process:
             return
 
         data = {
             'step': self.step,
             'model': self.accelerator.get_state_dict(self.model),
@@ -924,48 +893,22 @@
         data = torch.load(str(self.results_folder / f'model-{milestone}.pt'), map_location=device)
 
         model = self.accelerator.unwrap_model(self.model)
         model.load_state_dict(data['model'])
 
         self.step = data['step']
         self.opt.load_state_dict(data['opt'])
-        if self.accelerator.is_main_process:
-            self.ema.load_state_dict(data["ema"])
+        self.ema.load_state_dict(data['ema'])
 
         if 'version' in data:
             print(f"loading from version {data['version']}")
 
         if exists(self.accelerator.scaler) and exists(data['scaler']):
             self.accelerator.scaler.load_state_dict(data['scaler'])
 
-    @torch.no_grad()
-    def calculate_activation_statistics(self, samples):
-        assert exists(self.inception_v3)
-
-        features = self.inception_v3(samples)[0]
-        features = rearrange(features, '... 1 1 -> ...').cpu().numpy()
-
-        mu = np.mean(features, axis = 0)
-        sigma = np.cov(features, rowvar = False)
-        return mu, sigma
-
-    def fid_score(self, real_samples, fake_samples):
-
-        if self.channels == 1:
-            real_samples, fake_samples = map(lambda t: repeat(t, 'b 1 ... -> b c ...', c = 3), (real_samples, fake_samples))
-
-        min_batch = min(real_samples.shape[0], fake_samples.shape[0])
-        real_samples, fake_samples = map(lambda t: t[:min_batch], (real_samples, fake_samples))
-
-        m1, s1 = self.calculate_activation_statistics(real_samples)
-        m2, s2 = self.calculate_activation_statistics(fake_samples)
-
-        fid_value = calculate_frechet_distance(m1, s1, m2, s2)
-        return fid_value
-
     def train(self):
         accelerator = self.accelerator
         device = accelerator.device
 
         with tqdm(initial = self.step, total = self.train_num_steps, disable = not accelerator.is_main_process) as pbar:
 
             while self.step < self.train_num_steps:
@@ -978,43 +921,97 @@
                     with self.accelerator.autocast():
                         loss = self.model(data)
                         loss = loss / self.gradient_accumulate_every
                         total_loss += loss.item()
 
                     self.accelerator.backward(loss)
 
-                accelerator.clip_grad_norm_(self.model.parameters(), self.max_grad_norm)
+                accelerator.clip_grad_norm_(self.model.parameters(), 1.0)
                 pbar.set_description(f'loss: {total_loss:.4f}')
 
                 accelerator.wait_for_everyone()
 
                 self.opt.step()
                 self.opt.zero_grad()
 
                 accelerator.wait_for_everyone()
 
                 self.step += 1
                 if accelerator.is_main_process:
+                    self.ema.to(device)
                     self.ema.update()
 
                     if self.step != 0 and self.step % self.save_and_sample_every == 0:
                         self.ema.ema_model.eval()
 
                         with torch.no_grad():
                             milestone = self.step // self.save_and_sample_every
                             batches = num_to_groups(self.num_samples, self.batch_size)
                             all_images_list = list(map(lambda n: self.ema.ema_model.sample(batch_size=n), batches))
 
                         all_images = torch.cat(all_images_list, dim = 0)
-
                         utils.save_image(all_images, str(self.results_folder / f'sample-{milestone}.png'), nrow = int(math.sqrt(self.num_samples)))
                         self.save(milestone)
 
-                        # whether to calculate fid
-
-                        if exists(self.inception_v3):
-                            fid_score = self.fid_score(real_samples = data, fake_samples = all_images)
-                            accelerator.print(f'fid_score: {fid_score}')
-
                 pbar.update(1)
 
         accelerator.print('training complete')
+
+if __name__ == '__main__':
+    class Classifier(nn.Module):
+        def __init__(self, image_size, num_classes, t_dim=1) -> None:
+            super().__init__()
+            self.linear_t = nn.Linear(t_dim, num_classes)
+            self.linear_img = nn.Linear(image_size * image_size * 3, num_classes)
+        def forward(self, x, t):
+            """
+            Args:
+                x (_type_): [B, 3, N, N]
+                t (_type_): [B,]
+
+            Returns:
+                    logits [B, num_classes]
+            """
+            B = x.shape[0]
+            t = t.view(B, 1)
+            logits = self.linear_t(t.float()) + self.linear_img(x.view(x.shape[0], -1))
+            return logits
+        
+    def classifier_cond_fn(x, t, classifier, y, classifier_scale=1):
+        """
+        return the graident of the classifier outputing y wrt x.
+        formally expressed as d_log(classifier(x, t)) / dx
+        """
+        assert y is not None
+        with torch.enable_grad():
+            x_in = x.detach().requires_grad_(True)
+            logits = classifier(x_in, t)
+            log_probs = F.log_softmax(logits, dim=-1)
+            selected = log_probs[range(len(logits)), y.view(-1)]
+            grad = torch.autograd.grad(selected.sum(), x_in)[0] * classifier_scale
+            return grad
+        
+    
+    
+    model = Unet(
+        dim = 64,
+        dim_mults = (1, 2, 4, 8)
+    )
+    image_size = 128
+    diffusion = GaussianDiffusion(
+        model,
+        image_size = image_size,
+        timesteps = 1000   # number of steps
+    )
+
+    classifier = Classifier(image_size=image_size, num_classes=1000, t_dim=1)
+    batch_size = 4
+    sampled_images = diffusion.sample(
+        batch_size = batch_size,
+        cond_fn=classifier_cond_fn, 
+        guidance_kwargs={
+            "classifier":classifier,
+            "y":torch.fill(torch.zeros(batch_size), 1).long(),
+            "classifier_scale":1,
+        }
+    )
+    sampled_images.shape # (4, 3, 128, 128)
```

### Comparing `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,31 +4,35 @@
 from random import random
 from functools import partial
 from collections import namedtuple
 from multiprocessing import cpu_count
 
 import torch
 from torch import nn, einsum
-import torch.nn.functional as F
 from torch.cuda.amp import autocast
+import torch.nn.functional as F
 from torch.utils.data import Dataset, DataLoader
 
 from torch.optim import Adam
+
 from torchvision import transforms as T, utils
 
-from einops import rearrange, reduce
+from einops import rearrange, reduce, repeat
 from einops.layers.torch import Rearrange
 
 from PIL import Image
 from tqdm.auto import tqdm
 from ema_pytorch import EMA
 
 from accelerate import Accelerator
 
-# from denoising_diffusion_pytorch.version import __version__
+import numpy as np
+from denoising_diffusion_pytorch.fid_evaluation import FIDEvaluation
+
+from denoising_diffusion_pytorch.version import __version__
 
 # constants
 
 ModelPrediction =  namedtuple('ModelPrediction', ['pred_noise', 'pred_x_start'])
 
 # helpers functions
 
@@ -96,15 +100,15 @@
 
 class RMSNorm(nn.Module):
     def __init__(self, dim):
         super().__init__()
         self.g = nn.Parameter(torch.ones(1, dim, 1, 1))
 
     def forward(self, x):
-        return F.normalize(x, dim = 1) * self.g * (x.shape[-1] ** 0.5)
+        return F.normalize(x, dim = 1) * self.g * (x.shape[1] ** 0.5)
 
 class PreNorm(nn.Module):
     def __init__(self, dim, fn):
         super().__init__()
         self.fn = fn
         self.norm = RMSNorm(dim)
 
@@ -413,38 +417,38 @@
     t = torch.linspace(0, timesteps, steps, dtype = torch.float64) / timesteps
     v_start = torch.tensor(start / tau).sigmoid()
     v_end = torch.tensor(end / tau).sigmoid()
     alphas_cumprod = (-((t * (end - start) + start) / tau).sigmoid() + v_end) / (v_end - v_start)
     alphas_cumprod = alphas_cumprod / alphas_cumprod[0]
     betas = 1 - (alphas_cumprod[1:] / alphas_cumprod[:-1])
     return torch.clip(betas, 0, 0.999)
-    
 
-    
 class GaussianDiffusion(nn.Module):
     def __init__(
         self,
         model,
         *,
         image_size,
         timesteps = 1000,
         sampling_timesteps = None,
-        objective = 'pred_noise',
+        objective = 'pred_v',
         beta_schedule = 'sigmoid',
         schedule_fn_kwargs = dict(),
         ddim_sampling_eta = 0.,
         auto_normalize = True,
-        min_snr_loss_weight = False,
+        offset_noise_strength = 0.,  # https://www.crosslabs.org/blog/diffusion-with-offset-noise
+        min_snr_loss_weight = False, # https://arxiv.org/abs/2303.09556
         min_snr_gamma = 5
     ):
         super().__init__()
         assert not (type(self) == GaussianDiffusion and model.channels != model.out_dim)
         assert not model.random_or_learned_sinusoidal_cond
 
         self.model = model
+
         self.channels = self.model.channels
         self.self_condition = self.model.self_condition
 
         self.image_size = image_size
 
         self.objective = objective
 
@@ -502,36 +506,45 @@
 
         # below: log calculation clipped because the posterior variance is 0 at the beginning of the diffusion chain
 
         register_buffer('posterior_log_variance_clipped', torch.log(posterior_variance.clamp(min =1e-20)))
         register_buffer('posterior_mean_coef1', betas * torch.sqrt(alphas_cumprod_prev) / (1. - alphas_cumprod))
         register_buffer('posterior_mean_coef2', (1. - alphas_cumprod_prev) * torch.sqrt(alphas) / (1. - alphas_cumprod))
 
-        # loss weight
+        # offset noise strength - in blogpost, they claimed 0.1 was ideal
+
+        self.offset_noise_strength = offset_noise_strength
+
+        # derive loss weight
+        # snr - signal noise ratio
 
         snr = alphas_cumprod / (1 - alphas_cumprod)
 
+        # https://arxiv.org/abs/2303.09556
+
         maybe_clipped_snr = snr.clone()
         if min_snr_loss_weight:
             maybe_clipped_snr.clamp_(max = min_snr_gamma)
 
         if objective == 'pred_noise':
-            loss_weight = maybe_clipped_snr / snr
+            register_buffer('loss_weight', maybe_clipped_snr / snr)
         elif objective == 'pred_x0':
-            loss_weight = maybe_clipped_snr
+            register_buffer('loss_weight', maybe_clipped_snr)
         elif objective == 'pred_v':
-            loss_weight = maybe_clipped_snr / (snr + 1)
-
-        register_buffer('loss_weight', loss_weight)
+            register_buffer('loss_weight', maybe_clipped_snr / (snr + 1))
 
         # auto-normalization of data [0, 1] -> [-1, 1] - can turn off by setting it to be False
 
         self.normalize = normalize_to_neg_one_to_one if auto_normalize else identity
         self.unnormalize = unnormalize_to_zero_to_one if auto_normalize else identity
 
+    @property
+    def device(self):
+        return self.betas.device
+
     def predict_start_from_noise(self, x_t, t, noise):
         return (
             extract(self.sqrt_recip_alphas_cumprod, t, x_t.shape) * x_t -
             extract(self.sqrt_recipm1_alphas_cumprod, t, x_t.shape) * noise
         )
 
     def predict_noise_from_start(self, x_t, t, x0):
@@ -557,23 +570,26 @@
             extract(self.posterior_mean_coef1, t, x_t.shape) * x_start +
             extract(self.posterior_mean_coef2, t, x_t.shape) * x_t
         )
         posterior_variance = extract(self.posterior_variance, t, x_t.shape)
         posterior_log_variance_clipped = extract(self.posterior_log_variance_clipped, t, x_t.shape)
         return posterior_mean, posterior_variance, posterior_log_variance_clipped
 
-    def model_predictions(self, x, t, x_self_cond = None, clip_x_start = False):
+    def model_predictions(self, x, t, x_self_cond = None, clip_x_start = False, rederive_pred_noise = False):
         model_output = self.model(x, t, x_self_cond)
         maybe_clip = partial(torch.clamp, min = -1., max = 1.) if clip_x_start else identity
 
         if self.objective == 'pred_noise':
             pred_noise = model_output
             x_start = self.predict_start_from_noise(x, t, pred_noise)
             x_start = maybe_clip(x_start)
 
+            if clip_x_start and rederive_pred_noise:
+                pred_noise = self.predict_noise_from_start(x, t, x_start)
+
         elif self.objective == 'pred_x0':
             x_start = model_output
             x_start = maybe_clip(x_start)
             pred_noise = self.predict_noise_from_start(x, t, x_start)
 
         elif self.objective == 'pred_v':
             v = model_output
@@ -588,112 +604,92 @@
         x_start = preds.pred_x_start
 
         if clip_denoised:
             x_start.clamp_(-1., 1.)
 
         model_mean, posterior_variance, posterior_log_variance = self.q_posterior(x_start = x_start, x_t = x, t = t)
         return model_mean, posterior_variance, posterior_log_variance, x_start
-     
-    def condition_mean(self, cond_fn, mean,variance, x, t, guidance_kwargs=None):
-        """
-        Compute the mean for the previous step, given a function cond_fn that
-        computes the gradient of a conditional log probability with respect to
-        x. In particular, cond_fn computes grad(log(p(y|x))), and we want to
-        condition on y.
-        This uses the conditioning strategy from Sohl-Dickstein et al. (2015).
-        """
-        gradient = cond_fn(x, t, **guidance_kwargs)
-        new_mean = (
-            mean.float() + variance * gradient.float()
-        )
-        print("gradient: ",(variance * gradient.float()).mean())
-        return new_mean
 
-        
-    @torch.no_grad()
-    def p_sample(self, x, t: int, x_self_cond = None, cond_fn=None, guidance_kwargs=None):
-        b, *_, device = *x.shape, x.device
-        batched_times = torch.full((b,), t, device = x.device, dtype = torch.long)
-        model_mean, variance, model_log_variance, x_start = self.p_mean_variance(
-            x = x, t = batched_times, x_self_cond = x_self_cond, clip_denoised = True
-        )
-        if exists(cond_fn) and exists(guidance_kwargs):
-            model_mean = self.condition_mean(cond_fn, model_mean, variance, x, batched_times, guidance_kwargs)
-        
+    @torch.inference_mode()
+    def p_sample(self, x, t: int, x_self_cond = None):
+        b, *_, device = *x.shape, self.device
+        batched_times = torch.full((b,), t, device = device, dtype = torch.long)
+        model_mean, _, model_log_variance, x_start = self.p_mean_variance(x = x, t = batched_times, x_self_cond = x_self_cond, clip_denoised = True)
         noise = torch.randn_like(x) if t > 0 else 0. # no noise if t == 0
         pred_img = model_mean + (0.5 * model_log_variance).exp() * noise
         return pred_img, x_start
 
-    @torch.no_grad()
-    def p_sample_loop(self, shape, return_all_timesteps = False, cond_fn=None, guidance_kwargs=None):
-        batch, device = shape[0], self.betas.device
+    @torch.inference_mode()
+    def p_sample_loop(self, shape, return_all_timesteps = False):
+        batch, device = shape[0], self.device
 
         img = torch.randn(shape, device = device)
         imgs = [img]
 
         x_start = None
 
         for t in tqdm(reversed(range(0, self.num_timesteps)), desc = 'sampling loop time step', total = self.num_timesteps):
             self_cond = x_start if self.self_condition else None
-            img, x_start = self.p_sample(img, t, self_cond, cond_fn, guidance_kwargs)
+            img, x_start = self.p_sample(img, t, self_cond)
             imgs.append(img)
 
         ret = img if not return_all_timesteps else torch.stack(imgs, dim = 1)
 
         ret = self.unnormalize(ret)
         return ret
 
-    @torch.no_grad()
-    def ddim_sample(self, shape, return_all_timesteps = False, cond_fn=None, guidance_kwargs=None):
-        batch, device, total_timesteps, sampling_timesteps, eta, objective = shape[0], self.betas.device, self.num_timesteps, self.sampling_timesteps, self.ddim_sampling_eta, self.objective
+    @torch.inference_mode()
+    def ddim_sample(self, shape, return_all_timesteps = False):
+        batch, device, total_timesteps, sampling_timesteps, eta, objective = shape[0], self.device, self.num_timesteps, self.sampling_timesteps, self.ddim_sampling_eta, self.objective
 
         times = torch.linspace(-1, total_timesteps - 1, steps = sampling_timesteps + 1)   # [-1, 0, 1, 2, ..., T-1] when sampling_timesteps == total_timesteps
         times = list(reversed(times.int().tolist()))
         time_pairs = list(zip(times[:-1], times[1:])) # [(T-1, T-2), (T-2, T-3), ..., (1, 0), (0, -1)]
 
         img = torch.randn(shape, device = device)
         imgs = [img]
 
         x_start = None
 
         for time, time_next in tqdm(time_pairs, desc = 'sampling loop time step'):
             time_cond = torch.full((batch,), time, device = device, dtype = torch.long)
             self_cond = x_start if self.self_condition else None
-            pred_noise, x_start, *_ = self.model_predictions(img, time_cond, self_cond, clip_x_start = True)
-
-            imgs.append(img)
+            pred_noise, x_start, *_ = self.model_predictions(img, time_cond, self_cond, clip_x_start = True, rederive_pred_noise = True)
 
             if time_next < 0:
                 img = x_start
+                imgs.append(img)
                 continue
 
             alpha = self.alphas_cumprod[time]
             alpha_next = self.alphas_cumprod[time_next]
 
             sigma = eta * ((1 - alpha / alpha_next) * (1 - alpha_next) / (1 - alpha)).sqrt()
             c = (1 - alpha_next - sigma ** 2).sqrt()
 
             noise = torch.randn_like(img)
 
             img = x_start * alpha_next.sqrt() + \
                   c * pred_noise + \
                   sigma * noise
 
+            imgs.append(img)
+
         ret = img if not return_all_timesteps else torch.stack(imgs, dim = 1)
 
         ret = self.unnormalize(ret)
         return ret
 
-    @torch.no_grad()
-    def sample(self, batch_size = 16, return_all_timesteps = False, cond_fn=None, guidance_kwargs=None):
+    @torch.inference_mode()
+    def sample(self, batch_size = 16, return_all_timesteps = False):
         image_size, channels = self.image_size, self.channels
         sample_fn = self.p_sample_loop if not self.is_ddim_sampling else self.ddim_sample
-        return sample_fn((batch_size, channels, image_size, image_size), return_all_timesteps = return_all_timesteps, cond_fn=cond_fn, guidance_kwargs=guidance_kwargs)
+        return sample_fn((batch_size, channels, image_size, image_size), return_all_timesteps = return_all_timesteps)
 
-    @torch.no_grad()
+    @torch.inference_mode()
     def interpolate(self, x1, x2, t = None, lam = 0.5):
         b, *_, device = *x1.shape, x1.device
         t = default(t, self.num_timesteps - 1)
 
         assert x1.shape == x2.shape
 
         t_batched = torch.full((b,), t, device = device)
@@ -706,37 +702,46 @@
         for i in tqdm(reversed(range(0, t)), desc = 'interpolation sample time step', total = t):
             self_cond = x_start if self.self_condition else None
             img, x_start = self.p_sample(img, i, self_cond)
 
         return img
 
     @autocast(enabled = False)
-    def q_sample(self, x_start, t, noise=None):
+    def q_sample(self, x_start, t, noise = None):
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         return (
             extract(self.sqrt_alphas_cumprod, t, x_start.shape) * x_start +
             extract(self.sqrt_one_minus_alphas_cumprod, t, x_start.shape) * noise
         )
 
-    def p_losses(self, x_start, t, noise = None):
+    def p_losses(self, x_start, t, noise = None, offset_noise_strength = None):
         b, c, h, w = x_start.shape
+
         noise = default(noise, lambda: torch.randn_like(x_start))
 
+        # offset noise - https://www.crosslabs.org/blog/diffusion-with-offset-noise
+
+        offset_noise_strength = default(offset_noise_strength, self.offset_noise_strength)
+
+        if offset_noise_strength > 0.:
+            offset_noise = torch.randn(x_start.shape[:2], device = self.device)
+            noise += offset_noise_strength * rearrange(offset_noise, 'b c -> b c 1 1')
+
         # noise sample
 
         x = self.q_sample(x_start = x_start, t = t, noise = noise)
 
         # if doing self-conditioning, 50% of the time, predict x_start from current set of times
         # and condition with unet with that
         # this technique will slow down training by 25%, but seems to lower FID significantly
 
         x_self_cond = None
         if self.self_condition and random() < 0.5:
-            with torch.no_grad():
+            with torch.inference_mode():
                 x_self_cond = self.model_predictions(x, t).pred_x_start
                 x_self_cond.detach_()
 
         # predict and take gradient step
 
         model_out = self.model(x, t, x_self_cond)
 
@@ -814,39 +819,55 @@
         ema_update_every = 10,
         ema_decay = 0.995,
         adam_betas = (0.9, 0.99),
         save_and_sample_every = 1000,
         num_samples = 25,
         results_folder = './results',
         amp = False,
-        fp16 = False,
+        mixed_precision_type = 'fp16',
         split_batches = True,
-        convert_image_to = None
+        convert_image_to = None,
+        calculate_fid = True,
+        inception_block_idx = 2048,
+        max_grad_norm = 1.,
+        num_fid_samples = 50000,
+        save_best_and_latest_only = False
     ):
         super().__init__()
 
+        # accelerator
+
         self.accelerator = Accelerator(
             split_batches = split_batches,
-            mixed_precision = 'fp16' if fp16 else 'no'
+            mixed_precision = mixed_precision_type if amp else 'no'
         )
 
-        self.accelerator.native_amp = amp
+        # model
 
         self.model = diffusion_model
+        self.channels = diffusion_model.channels
+
+        # sampling and training hyperparameters
 
         assert has_int_squareroot(num_samples), 'number of samples must have an integer square root'
         self.num_samples = num_samples
         self.save_and_sample_every = save_and_sample_every
+        if save_best_and_latest_only:
+            assert calculate_fid, "`calculate_fid` must be True to provide a means for model evaluation for `save_best_and_latest_only`."
+            self.best_fid = 1e10 # infinite
+        self.save_best_and_latest_only = save_best_and_latest_only
 
         self.batch_size = train_batch_size
         self.gradient_accumulate_every = gradient_accumulate_every
 
         self.train_num_steps = train_num_steps
         self.image_size = diffusion_model.image_size
 
+        self.max_grad_norm = max_grad_norm
+
         # dataset and dataloader
 
         self.ds = Dataset(folder, self.image_size, augment_horizontal_flip = augment_horizontal_flip, convert_image_to = convert_image_to)
         dl = DataLoader(self.ds, batch_size = train_batch_size, shuffle = True, pin_memory = True, num_workers = cpu_count())
 
         dl = self.accelerator.prepare(dl)
         self.dl = cycle(dl)
@@ -855,26 +876,52 @@
 
         self.opt = Adam(diffusion_model.parameters(), lr = train_lr, betas = adam_betas)
 
         # for logging results in a folder periodically
 
         if self.accelerator.is_main_process:
             self.ema = EMA(diffusion_model, beta = ema_decay, update_every = ema_update_every)
+            self.ema.to(self.device)
 
         self.results_folder = Path(results_folder)
         self.results_folder.mkdir(exist_ok = True)
 
         # step counter state
 
         self.step = 0
 
         # prepare model, dataloader, optimizer with accelerator
 
         self.model, self.opt = self.accelerator.prepare(self.model, self.opt)
 
+        # FID-score computation
+
+        if calculate_fid:
+            self.calculate_fid = True
+            if not self.model.is_ddim_sampling:
+                self.accelerator.print(
+                    "WARNING: Robust FID computation requires a lot of generated samples and can therefore be very time consuming."\
+                    "Consider using DDIM sampling to save time."
+                )
+            self.fid_scorer = FIDEvaluation(
+                batch_size=self.batch_size,
+                dl=self.dl,
+                sampler=self.ema.ema_model,
+                channels=self.channels,
+                accelerator=self.accelerator,
+                stats_dir=results_folder,
+                device=self.device,
+                num_fid_samples=num_fid_samples,
+                inception_block_idx=inception_block_idx
+            )
+
+    @property
+    def device(self):
+        return self.accelerator.device
+
     def save(self, milestone):
         if not self.accelerator.is_local_main_process:
             return
 
         data = {
             'step': self.step,
             'model': self.accelerator.get_state_dict(self.model),
@@ -893,15 +940,16 @@
         data = torch.load(str(self.results_folder / f'model-{milestone}.pt'), map_location=device)
 
         model = self.accelerator.unwrap_model(self.model)
         model.load_state_dict(data['model'])
 
         self.step = data['step']
         self.opt.load_state_dict(data['opt'])
-        self.ema.load_state_dict(data['ema'])
+        if self.accelerator.is_main_process:
+            self.ema.load_state_dict(data["ema"])
 
         if 'version' in data:
             print(f"loading from version {data['version']}")
 
         if exists(self.accelerator.scaler) and exists(data['scaler']):
             self.accelerator.scaler.load_state_dict(data['scaler'])
 
@@ -921,97 +969,49 @@
                     with self.accelerator.autocast():
                         loss = self.model(data)
                         loss = loss / self.gradient_accumulate_every
                         total_loss += loss.item()
 
                     self.accelerator.backward(loss)
 
-                accelerator.clip_grad_norm_(self.model.parameters(), 1.0)
+                accelerator.clip_grad_norm_(self.model.parameters(), self.max_grad_norm)
                 pbar.set_description(f'loss: {total_loss:.4f}')
 
                 accelerator.wait_for_everyone()
 
                 self.opt.step()
                 self.opt.zero_grad()
 
                 accelerator.wait_for_everyone()
 
                 self.step += 1
                 if accelerator.is_main_process:
-                    self.ema.to(device)
                     self.ema.update()
 
                     if self.step != 0 and self.step % self.save_and_sample_every == 0:
                         self.ema.ema_model.eval()
 
-                        with torch.no_grad():
+                        with torch.inference_mode():
                             milestone = self.step // self.save_and_sample_every
                             batches = num_to_groups(self.num_samples, self.batch_size)
                             all_images_list = list(map(lambda n: self.ema.ema_model.sample(batch_size=n), batches))
 
                         all_images = torch.cat(all_images_list, dim = 0)
+
                         utils.save_image(all_images, str(self.results_folder / f'sample-{milestone}.png'), nrow = int(math.sqrt(self.num_samples)))
-                        self.save(milestone)
 
-                pbar.update(1)
+                        # whether to calculate fid
 
-        accelerator.print('training complete')
+                        if self.calculate_fid:
+                            fid_score = self.fid_scorer.fid_score()
+                            accelerator.print(f'fid_score: {fid_score}')
+                        if self.save_best_and_latest_only:
+                            if self.best_fid > fid_score:
+                                self.best_fid = fid_score
+                                self.save("best")
+                            self.save("latest")
+                        else:
+                            self.save(milestone)
 
-if __name__ == '__main__':
-    class Classifier(nn.Module):
-        def __init__(self, image_size, num_classes, t_dim=1) -> None:
-            super().__init__()
-            self.linear_t = nn.Linear(t_dim, num_classes)
-            self.linear_img = nn.Linear(image_size * image_size * 3, num_classes)
-        def forward(self, x, t):
-            """
-            Args:
-                x (_type_): [B, 3, N, N]
-                t (_type_): [B,]
-
-            Returns:
-                    logits [B, num_classes]
-            """
-            B = x.shape[0]
-            t = t.view(B, 1)
-            logits = self.linear_t(t.float()) + self.linear_img(x.view(x.shape[0], -1))
-            return logits
-        
-    def classifier_cond_fn(x, t, classifier, y, classifier_scale=1):
-        """
-        return the graident of the classifier outputing y wrt x.
-        formally expressed as d_log(classifier(x, t)) / dx
-        """
-        assert y is not None
-        with torch.enable_grad():
-            x_in = x.detach().requires_grad_(True)
-            logits = classifier(x_in, t)
-            log_probs = F.log_softmax(logits, dim=-1)
-            selected = log_probs[range(len(logits)), y.view(-1)]
-            grad = torch.autograd.grad(selected.sum(), x_in)[0] * classifier_scale
-            return grad
-        
-    
-    
-    model = Unet(
-        dim = 64,
-        dim_mults = (1, 2, 4, 8)
-    )
-    image_size = 128
-    diffusion = GaussianDiffusion(
-        model,
-        image_size = image_size,
-        timesteps = 1000   # number of steps
-    )
+                pbar.update(1)
 
-    classifier = Classifier(image_size=image_size, num_classes=1000, t_dim=1)
-    batch_size = 4
-    sampled_images = diffusion.sample(
-        batch_size = batch_size,
-        cond_fn=classifier_cond_fn, 
-        guidance_kwargs={
-            "classifier":classifier,
-            "y":torch.fill(torch.zeros(batch_size), 1).long(),
-            "classifier_scale":1,
-        }
-    )
-    sampled_images.shape # (4, 3, 128, 128)
+        accelerator.print('training complete')
```

### Comparing `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.7.6
+Version: 1.7.7
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 denoising_diffusion_pytorch/__init__.py
 denoising_diffusion_pytorch/classifier_free_guidance.py
 denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
 denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
 denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
 denoising_diffusion_pytorch/elucidated_diffusion.py
+denoising_diffusion_pytorch/fid_evaluation.py
 denoising_diffusion_pytorch/guided_diffusion.py
 denoising_diffusion_pytorch/learned_gaussian_diffusion.py
 denoising_diffusion_pytorch/simple_diffusion.py
 denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
 denoising_diffusion_pytorch/version.py
 denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
 denoising_diffusion_pytorch.egg-info/PKG-INFO
```

### Comparing `denoising-diffusion-pytorch-1.7.6/setup.py` & `denoising-diffusion-pytorch-1.7.7/setup.py`

 * *Files identical despite different names*

