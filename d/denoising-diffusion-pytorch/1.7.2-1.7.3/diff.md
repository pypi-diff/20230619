# Comparing `tmp/denoising-diffusion-pytorch-1.7.2.tar.gz` & `tmp/denoising-diffusion-pytorch-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.7.2.tar", last modified: Mon Jun 19 02:19:05 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.7.3.tar", last modified: Mon Jun 19 02:36:26 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.7.2.tar` & `denoising-diffusion-pytorch-1.7.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:19:05.472139 denoising-diffusion-pytorch-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 02:18:53.000000 denoising-diffusion-pytorch-1.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 02:19:05.472139 denoising-diffusion-pytorch-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-06-19 02:18:53.000000 denoising-diffusion-pytorch-1.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:19:05.468140 denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-19 02:18:53.000000 denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27780 2023-06-19 02:18:53.000000 denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-06-19 02:18:53.000000 denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    35636 2023-06-19 02:18:53.000000 denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    29598 2023-06-19 02:18:53.000000 denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-19 02:18:53.000000 denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    35586 2023-06-19 02:18:53.000000 denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-19 02:18:53.000000 denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21193 2023-06-19 02:18:53.000000 denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-06-19 02:18:53.000000 denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 02:18:53.000000 denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-19 02:18:53.000000 denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:19:05.468140 denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 02:19:05.000000 denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-19 02:19:05.000000 denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 02:19:05.000000 denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 02:19:05.000000 denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 02:19:05.000000 denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 02:19:05.472139 denoising-diffusion-pytorch-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-19 02:18:53.000000 denoising-diffusion-pytorch-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:36:26.373286 denoising-diffusion-pytorch-1.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 02:36:26.373286 denoising-diffusion-pytorch-1.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:36:26.373286 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27780 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35636 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29598 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35586 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21193 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:36:26.373286 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 02:36:26.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-19 02:36:26.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 02:36:26.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 02:36:26.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 02:36:26.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 02:36:26.373286 denoising-diffusion-pytorch-1.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.7.2/LICENSE` & `denoising-diffusion-pytorch-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.2/PKG-INFO` & `denoising-diffusion-pytorch-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.7.2
+Version: 1.7.3
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.7.2/README.md` & `denoising-diffusion-pytorch-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         return fouriered
 
 # building block modules
 
 class Block(nn.Module):
     def __init__(self, dim, dim_out, groups = 8):
         super().__init__()
-        self.proj = nn.Conv2d(dim, dim_out, 3, padding = 1)
+        self.proj = nn.Conv1d(dim, dim_out, 3, padding = 1)
         self.norm = nn.GroupNorm(groups, dim_out)
         self.act = nn.SiLU()
 
     def forward(self, x, scale_shift = None):
         x = self.proj(x)
         x = self.norm(x)
```

### Comparing `denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.7.2
+Version: 1.7.3
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.7.2/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.2/setup.py` & `denoising-diffusion-pytorch-1.7.3/setup.py`

 * *Files identical despite different names*

