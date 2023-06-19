# Comparing `tmp/denoising-diffusion-pytorch-1.7.7.tar.gz` & `tmp/denoising-diffusion-pytorch-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.7.7.tar", last modified: Mon Jun 19 14:52:54 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.8.0.tar", last modified: Mon Jun 19 16:26:16 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.7.7.tar` & `denoising-diffusion-pytorch-1.8.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:52:54.665455 denoising-diffusion-pytorch-1.7.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 14:52:54.665455 denoising-diffusion-pytorch-1.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10255 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:52:54.665455 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    35880 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/fid_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:52:54.665455 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 14:52:54.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-19 14:52:54.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 14:52:54.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 14:52:54.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 14:52:54.000000 denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 14:52:54.665455 denoising-diffusion-pytorch-1.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-19 14:52:47.000000 denoising-diffusion-pytorch-1.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:26:16.061913 denoising-diffusion-pytorch-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 16:26:16.061913 denoising-diffusion-pytorch-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:26:16.061913 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36127 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/fid_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:26:16.061913 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 16:26:15.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-19 16:26:16.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:26:15.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 16:26:15.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 16:26:15.000000 denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 16:26:16.065913 denoising-diffusion-pytorch-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-19 16:26:07.000000 denoising-diffusion-pytorch-1.8.0/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.7.7/LICENSE` & `denoising-diffusion-pytorch-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.7/PKG-INFO` & `denoising-diffusion-pytorch-1.8.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.7.7
+Version: 1.8.0
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.7.7/README.md` & `denoising-diffusion-pytorch-1.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -149,18 +149,14 @@
 ```
 
 `Trainer1D` does not evaluate the generated samples in any way since the type of data is not known.
 
 You could consider adding a suitable metric to the training loop yourself after doing an editable install of this package
 `pip install -e .`.
 
-## Todo
-
-- [ ] add flash attention, do full attention at 64x64, linear attention at anything above
-
 ## Citations
 
 ```bibtex
 @inproceedings{NEURIPS2020_4c5bcfec,
     author      = {Ho, Jonathan and Jain, Ajay and Abbeel, Pieter},
     booktitle   = {Advances in Neural Information Processing Systems},
     editor      = {H. Larochelle and M. Ranzato and R. Hadsell and M.F. Balcan and H. Lin},
@@ -318,7 +314,16 @@
 ```bibtex
 @inproceedings{Lin2023CommonDN,
     title   = {Common Diffusion Noise Schedules and Sample Steps are Flawed},
     author  = {Shanchuan Lin and Bingchen Liu and Jiashi Li and Xiao Yang},
     year    = {2023}
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
@@ -45,46 +45,44 @@
 train_lr = 8e-5, train_num_steps = 700000, # total training steps
 gradient_accumulate_every = 2, # gradient accumulation steps ema_decay = 0.995,
 # exponential moving average decay amp = True, # turn on mixed precision )
 trainer.train() # after a lot of training sampled_seq = diffusion.sample
 (batch_size = 4) sampled_seq.shape # (4, 32, 128) ``` `Trainer1D` does not
 evaluate the generated samples in any way since the type of data is not known.
 You could consider adding a suitable metric to the training loop yourself after
-doing an editable install of this package `pip install -e .`. ## Todo - [ ] add
-flash attention, do full attention at 64x64, linear attention at anything above
-## Citations ```bibtex @inproceedings{NEURIPS2020_4c5bcfec, author = {Ho,
-Jonathan and Jain, Ajay and Abbeel, Pieter}, booktitle = {Advances in Neural
-Information Processing Systems}, editor = {H. Larochelle and M. Ranzato and R.
-Hadsell and M.F. Balcan and H. Lin}, pages = {6840--6851}, publisher = {Curran
-Associates, Inc.}, title = {Denoising Diffusion Probabilistic Models}, url =
-{https://proceedings.neurips.cc/paper/2020/file/
-4c5bcfec8584af0d967f1ab10179ca4b-Paper.pdf}, volume = {33}, year = {2020} } ```
-```bibtex @InProceedings{pmlr-v139-nichol21a, title = {Improved Denoising
-Diffusion Probabilistic Models}, author = {Nichol, Alexander Quinn and
-Dhariwal, Prafulla}, booktitle = {Proceedings of the 38th International
-Conference on Machine Learning}, pages = {8162--8171}, year = {2021}, editor =
-{Meila, Marina and Zhang, Tong}, volume = {139}, series = {Proceedings of
-Machine Learning Research}, month = {18--24 Jul}, publisher = {PMLR}, pdf =
-{http://proceedings.mlr.press/v139/nichol21a/nichol21a.pdf}, url = {https://
-proceedings.mlr.press/v139/nichol21a.html}, } ``` ```bibtex @inproceedings
-{kingma2021on, title = {On Density Estimation with Diffusion Models}, author =
-{Diederik P Kingma and Tim Salimans and Ben Poole and Jonathan Ho}, booktitle =
-{Advances in Neural Information Processing Systems}, editor = {A. Beygelzimer
-and Y. Dauphin and P. Liang and J. Wortman Vaughan}, year = {2021}, url =
-{https://openreview.net/forum?id=2LdBqxc1Yv} } ``` ```bibtex @article
-{Karras2022ElucidatingTD, title = {Elucidating the Design Space of Diffusion-
-Based Generative Models}, author = {Tero Karras and Miika Aittala and Timo Aila
-and Samuli Laine}, journal = {ArXiv}, year = {2022}, volume = {abs/2206.00364}
-} ``` ```bibtex @article{Song2021DenoisingDI, title = {Denoising Diffusion
-Implicit Models}, author = {Jiaming Song and Chenlin Meng and Stefano Ermon},
-journal = {ArXiv}, year = {2021}, volume = {abs/2010.02502} } ``` ```bibtex
-@misc{chen2022analog, title = {Analog Bits: Generating Discrete Data using
-Diffusion Models with Self-Conditioning}, author = {Ting Chen and Ruixiang
-Zhang and Geoffrey Hinton}, year = {2022}, eprint = {2208.04202}, archivePrefix
-= {arXiv}, primaryClass = {cs.CV} } ``` ```bibtex @article
+doing an editable install of this package `pip install -e .`. ## Citations
+```bibtex @inproceedings{NEURIPS2020_4c5bcfec, author = {Ho, Jonathan and Jain,
+Ajay and Abbeel, Pieter}, booktitle = {Advances in Neural Information
+Processing Systems}, editor = {H. Larochelle and M. Ranzato and R. Hadsell and
+M.F. Balcan and H. Lin}, pages = {6840--6851}, publisher = {Curran Associates,
+Inc.}, title = {Denoising Diffusion Probabilistic Models}, url = {https://
+proceedings.neurips.cc/paper/2020/file/4c5bcfec8584af0d967f1ab10179ca4b-
+Paper.pdf}, volume = {33}, year = {2020} } ``` ```bibtex @InProceedings{pmlr-
+v139-nichol21a, title = {Improved Denoising Diffusion Probabilistic Models},
+author = {Nichol, Alexander Quinn and Dhariwal, Prafulla}, booktitle =
+{Proceedings of the 38th International Conference on Machine Learning}, pages =
+{8162--8171}, year = {2021}, editor = {Meila, Marina and Zhang, Tong}, volume =
+{139}, series = {Proceedings of Machine Learning Research}, month = {18--24
+Jul}, publisher = {PMLR}, pdf = {http://proceedings.mlr.press/v139/nichol21a/
+nichol21a.pdf}, url = {https://proceedings.mlr.press/v139/nichol21a.html}, }
+``` ```bibtex @inproceedings{kingma2021on, title = {On Density Estimation with
+Diffusion Models}, author = {Diederik P Kingma and Tim Salimans and Ben Poole
+and Jonathan Ho}, booktitle = {Advances in Neural Information Processing
+Systems}, editor = {A. Beygelzimer and Y. Dauphin and P. Liang and J. Wortman
+Vaughan}, year = {2021}, url = {https://openreview.net/forum?id=2LdBqxc1Yv} }
+``` ```bibtex @article{Karras2022ElucidatingTD, title = {Elucidating the Design
+Space of Diffusion-Based Generative Models}, author = {Tero Karras and Miika
+Aittala and Timo Aila and Samuli Laine}, journal = {ArXiv}, year = {2022},
+volume = {abs/2206.00364} } ``` ```bibtex @article{Song2021DenoisingDI, title =
+{Denoising Diffusion Implicit Models}, author = {Jiaming Song and Chenlin Meng
+and Stefano Ermon}, journal = {ArXiv}, year = {2021}, volume = {abs/2010.02502}
+} ``` ```bibtex @misc{chen2022analog, title = {Analog Bits: Generating Discrete
+Data using Diffusion Models with Self-Conditioning}, author = {Ting Chen and
+Ruixiang Zhang and Geoffrey Hinton}, year = {2022}, eprint = {2208.04202},
+archivePrefix = {arXiv}, primaryClass = {cs.CV} } ``` ```bibtex @article
 {Salimans2022ProgressiveDF, title = {Progressive Distillation for Fast Sampling
 of Diffusion Models}, author = {Tim Salimans and Jonathan Ho}, journal =
 {ArXiv}, year = {2022}, volume = {abs/2202.00512} } ``` ```bibtex @article
 {Ho2022ClassifierFreeDG, title = {Classifier-Free Diffusion Guidance}, author =
 {Jonathan Ho}, journal = {ArXiv}, year = {2022}, volume = {abs/2207.12598} }
 ``` ```bibtex @article{Sunkara2022NoMS, title = {No More Strided Convolutions
 or Pooling: A New CNN Building Block for Low-Resolution Images and Small
@@ -107,8 +105,12 @@
 {Efficient Diffusion Training via Min-SNR Weighting Strategy}, author =
 {Tiankai Hang and Shuyang Gu and Chen Li and Jianmin Bao and Dong Chen and Han
 Hu and Xin Geng and Baining Guo}, year = {2023} } ``` ```bibtex @misc
 {Guttenberg2023, author = {Nicholas Guttenberg}, url = {https://
 www.crosslabs.org/blog/diffusion-with-offset-noise} } ``` ```bibtex
 @inproceedings{Lin2023CommonDN, title = {Common Diffusion Noise Schedules and
 Sample Steps are Flawed}, author = {Shanchuan Lin and Bingchen Liu and Jiashi
-Li and Xiao Yang}, year = {2023} } ```
+Li and Xiao Yang}, year = {2023} } ``` ```bibtex @inproceedings
+{dao2022flashattention, title = {Flash{A}ttention: Fast and Memory-Efficient
+Exact Attention with {IO}-Awareness}, author = {Dao, Tri and Fu, Daniel Y. and
+Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher}, booktitle = {Advances
+in Neural Information Processing Systems}, year = {2022} } ```
```

### Comparing `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from PIL import Image
 from tqdm.auto import tqdm
 from ema_pytorch import EMA
 
 from accelerate import Accelerator
 
-import numpy as np
+from denoising_diffusion_pytorch.attend import Attend
 from denoising_diffusion_pytorch.fid_evaluation import FIDEvaluation
 
 from denoising_diffusion_pytorch.version import __version__
 
 # constants
 
 ModelPrediction =  namedtuple('ModelPrediction', ['pred_noise', 'pred_x_start'])
@@ -40,14 +40,19 @@
     return x is not None
 
 def default(val, d):
     if exists(val):
         return val
     return d() if callable(d) else d
 
+def cast_tuple(t, length = 1):
+    if isinstance(t, tuple):
+        return t
+    return ((t,) * length)
+
 def identity(t, *args, **kwargs):
     return t
 
 def cycle(dl):
     while True:
         for data in dl:
             yield data
@@ -74,22 +79,14 @@
     return img * 2 - 1
 
 def unnormalize_to_zero_to_one(t):
     return (t + 1) * 0.5
 
 # small helper modules
 
-class Residual(nn.Module):
-    def __init__(self, fn):
-        super().__init__()
-        self.fn = fn
-
-    def forward(self, x, *args, **kwargs):
-        return self.fn(x, *args, **kwargs) + x
-
 def Upsample(dim, dim_out = None):
     return nn.Sequential(
         nn.Upsample(scale_factor = 2, mode = 'nearest'),
         nn.Conv2d(dim, default(dim_out, dim), 3, padding = 1)
     )
 
 def Downsample(dim, dim_out = None):
@@ -102,24 +99,14 @@
     def __init__(self, dim):
         super().__init__()
         self.g = nn.Parameter(torch.ones(1, dim, 1, 1))
 
     def forward(self, x):
         return F.normalize(x, dim = 1) * self.g * (x.shape[1] ** 0.5)
 
-class PreNorm(nn.Module):
-    def __init__(self, dim, fn):
-        super().__init__()
-        self.fn = fn
-        self.norm = RMSNorm(dim)
-
-    def forward(self, x):
-        x = self.norm(x)
-        return self.fn(x)
-
 # sinusoidal positional embeds
 
 class SinusoidalPosEmb(nn.Module):
     def __init__(self, dim):
         super().__init__()
         self.dim = dim
 
@@ -192,28 +179,38 @@
         h = self.block1(x, scale_shift = scale_shift)
 
         h = self.block2(h)
 
         return h + self.res_conv(x)
 
 class LinearAttention(nn.Module):
-    def __init__(self, dim, heads = 4, dim_head = 32):
+    def __init__(
+        self,
+        dim,
+        heads = 4,
+        dim_head = 32
+    ):
         super().__init__()
         self.scale = dim_head ** -0.5
         self.heads = heads
         hidden_dim = dim_head * heads
+
+        self.norm = RMSNorm(dim)
         self.to_qkv = nn.Conv2d(dim, hidden_dim * 3, 1, bias = False)
 
         self.to_out = nn.Sequential(
             nn.Conv2d(hidden_dim, dim, 1),
             RMSNorm(dim)
         )
 
     def forward(self, x):
         b, c, h, w = x.shape
+
+        x = self.norm(x)
+
         qkv = self.to_qkv(x).chunk(3, dim = 1)
         q, k, v = map(lambda t: rearrange(t, 'b (h c) x y -> b h c (x y)', h = self.heads), qkv)
 
         q = q.softmax(dim = -2)
         k = k.softmax(dim = -1)
 
         q = q * self.scale
@@ -221,53 +218,62 @@
         context = torch.einsum('b h d n, b h e n -> b h d e', k, v)
 
         out = torch.einsum('b h d e, b h d n -> b h e n', context, q)
         out = rearrange(out, 'b h c (x y) -> b (h c) x y', h = self.heads, x = h, y = w)
         return self.to_out(out)
 
 class Attention(nn.Module):
-    def __init__(self, dim, heads = 4, dim_head = 32):
+    def __init__(
+        self,
+        dim,
+        heads = 4,
+        dim_head = 32,
+        flash = False
+    ):
         super().__init__()
-        self.scale = dim_head ** -0.5
         self.heads = heads
         hidden_dim = dim_head * heads
 
+        self.norm = RMSNorm(dim)
+        self.attend = Attend(flash = flash)
+
         self.to_qkv = nn.Conv2d(dim, hidden_dim * 3, 1, bias = False)
         self.to_out = nn.Conv2d(hidden_dim, dim, 1)
 
     def forward(self, x):
         b, c, h, w = x.shape
-        qkv = self.to_qkv(x).chunk(3, dim = 1)
-        q, k, v = map(lambda t: rearrange(t, 'b (h c) x y -> b h c (x y)', h = self.heads), qkv)
 
-        q = q * self.scale
+        x = self.norm(x)
 
-        sim = einsum('b h d i, b h d j -> b h i j', q, k)
-        attn = sim.softmax(dim = -1)
-        out = einsum('b h i j, b h d j -> b h i d', attn, v)
+        qkv = self.to_qkv(x).chunk(3, dim = 1)
+        q, k, v = map(lambda t: rearrange(t, 'b (h c) x y -> b h (x y) c', h = self.heads), qkv)
+
+        out = self.attend(q, k, v)
 
         out = rearrange(out, 'b h (x y) d -> b (h d) x y', x = h, y = w)
         return self.to_out(out)
 
 # model
 
 class Unet(nn.Module):
     def __init__(
         self,
         dim,
         init_dim = None,
         out_dim = None,
-        dim_mults=(1, 2, 4, 8),
+        dim_mults = (1, 2, 4, 8),
         channels = 3,
         self_condition = False,
         resnet_block_groups = 8,
         learned_variance = False,
         learned_sinusoidal_cond = False,
         random_fourier_features = False,
-        learned_sinusoidal_dim = 16
+        learned_sinusoidal_dim = 16,
+        full_attn = (False, False, False, True),
+        flash_attn = False
     ):
         super().__init__()
 
         # determine dimensions
 
         self.channels = channels
         self.self_condition = self_condition
@@ -297,42 +303,53 @@
         self.time_mlp = nn.Sequential(
             sinu_pos_emb,
             nn.Linear(fourier_dim, time_dim),
             nn.GELU(),
             nn.Linear(time_dim, time_dim)
         )
 
+        # attention
+
+        full_attn = cast_tuple(full_attn, length = len(dim_mults))
+        assert len(full_attn) == len(dim_mults)
+
+        FullAttention = partial(Attention, flash = flash_attn)
+
         # layers
 
         self.downs = nn.ModuleList([])
         self.ups = nn.ModuleList([])
         num_resolutions = len(in_out)
 
-        for ind, (dim_in, dim_out) in enumerate(in_out):
+        for ind, ((dim_in, dim_out), layer_full_attn) in enumerate(zip(in_out, full_attn)):
             is_last = ind >= (num_resolutions - 1)
 
+            attn_klass = FullAttention if layer_full_attn else LinearAttention
+
             self.downs.append(nn.ModuleList([
                 block_klass(dim_in, dim_in, time_emb_dim = time_dim),
                 block_klass(dim_in, dim_in, time_emb_dim = time_dim),
-                Residual(PreNorm(dim_in, LinearAttention(dim_in))),
+                attn_klass(dim_in),
                 Downsample(dim_in, dim_out) if not is_last else nn.Conv2d(dim_in, dim_out, 3, padding = 1)
             ]))
 
         mid_dim = dims[-1]
         self.mid_block1 = block_klass(mid_dim, mid_dim, time_emb_dim = time_dim)
-        self.mid_attn = Residual(PreNorm(mid_dim, Attention(mid_dim)))
+        self.mid_attn = FullAttention(mid_dim)
         self.mid_block2 = block_klass(mid_dim, mid_dim, time_emb_dim = time_dim)
 
-        for ind, (dim_in, dim_out) in enumerate(reversed(in_out)):
+        for ind, ((dim_in, dim_out), layer_full_attn) in enumerate(zip(reversed(in_out), reversed(full_attn))):
             is_last = ind == (len(in_out) - 1)
 
+            attn_klass = FullAttention if layer_full_attn else LinearAttention
+
             self.ups.append(nn.ModuleList([
                 block_klass(dim_out + dim_in, dim_out, time_emb_dim = time_dim),
                 block_klass(dim_out + dim_in, dim_out, time_emb_dim = time_dim),
-                Residual(PreNorm(dim_out, LinearAttention(dim_out))),
+                attn_klass(dim_out),
                 Upsample(dim_out, dim_in) if not is_last else  nn.Conv2d(dim_out, dim_in, 3, padding = 1)
             ]))
 
         default_out_dim = channels * (1 if not learned_variance else 2)
         self.out_dim = default(out_dim, default_out_dim)
 
         self.final_res_block = block_klass(dim * 2, dim, time_emb_dim = time_dim)
@@ -351,30 +368,30 @@
         h = []
 
         for block1, block2, attn, downsample in self.downs:
             x = block1(x, t)
             h.append(x)
 
             x = block2(x, t)
-            x = attn(x)
+            x = attn(x) + x
             h.append(x)
 
             x = downsample(x)
 
         x = self.mid_block1(x, t)
-        x = self.mid_attn(x)
+        x = self.mid_attn(x) + x
         x = self.mid_block2(x, t)
 
         for block1, block2, attn, upsample in self.ups:
             x = torch.cat((x, h.pop()), dim = 1)
             x = block1(x, t)
 
             x = torch.cat((x, h.pop()), dim = 1)
             x = block2(x, t)
-            x = attn(x)
+            x = attn(x) + x
 
             x = upsample(x)
 
         x = torch.cat((x, r), dim = 1)
 
         x = self.final_res_block(x, t)
         return self.final_conv(x)
```

### Comparing `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/fid_evaluation.py` & `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/fid_evaluation.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.7.7
+Version: 1.8.0
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.7.7/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.8.0/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 denoising_diffusion_pytorch/__init__.py
+denoising_diffusion_pytorch/attend.py
 denoising_diffusion_pytorch/classifier_free_guidance.py
 denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
 denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
 denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
 denoising_diffusion_pytorch/elucidated_diffusion.py
 denoising_diffusion_pytorch/fid_evaluation.py
 denoising_diffusion_pytorch/guided_diffusion.py
```

### Comparing `denoising-diffusion-pytorch-1.7.7/setup.py` & `denoising-diffusion-pytorch-1.8.0/setup.py`

 * *Files identical despite different names*

