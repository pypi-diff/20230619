# Comparing `tmp/denoising-diffusion-pytorch-1.7.3.tar.gz` & `tmp/denoising-diffusion-pytorch-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.7.3.tar", last modified: Mon Jun 19 02:36:26 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.7.4.tar", last modified: Mon Jun 19 02:42:19 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.7.3.tar` & `denoising-diffusion-pytorch-1.7.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:36:26.373286 denoising-diffusion-pytorch-1.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 02:36:26.373286 denoising-diffusion-pytorch-1.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:36:26.373286 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27780 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    35636 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    29598 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    35586 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21193 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:36:26.373286 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 02:36:26.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-19 02:36:26.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 02:36:26.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 02:36:26.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 02:36:26.000000 denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 02:36:26.373286 denoising-diffusion-pytorch-1.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-19 02:36:17.000000 denoising-diffusion-pytorch-1.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:42:19.760907 denoising-diffusion-pytorch-1.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 02:42:19.760907 denoising-diffusion-pytorch-1.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:42:19.760907 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27756 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35612 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29598 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35562 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21169 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:42:19.760907 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 02:42:19.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-19 02:42:19.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 02:42:19.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 02:42:19.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 02:42:19.000000 denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 02:42:19.760907 denoising-diffusion-pytorch-1.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-19 02:42:10.000000 denoising-diffusion-pytorch-1.7.4/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.7.3/LICENSE` & `denoising-diffusion-pytorch-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.3/PKG-INFO` & `denoising-diffusion-pytorch-1.7.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.7.3
+Version: 1.7.4
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.7.3/README.md` & `denoising-diffusion-pytorch-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,14 @@
         qkv = self.to_qkv(x).chunk(3, dim = 1)
         q, k, v = map(lambda t: rearrange(t, 'b (h c) x y -> b h c (x y)', h = self.heads), qkv)
 
         q = q.softmax(dim = -2)
         k = k.softmax(dim = -1)
 
         q = q * self.scale
-        v = v / (h * w)
 
         context = torch.einsum('b h d n, b h e n -> b h d e', k, v)
 
         out = torch.einsum('b h d e, b h d n -> b h e n', context, q)
         out = rearrange(out, 'b h c (x y) -> b (h c) x y', h = self.heads, x = h, y = w)
         return self.to_out(out)
```

### Comparing `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,14 @@
         qkv = self.to_qkv(x).chunk(3, dim = 1)
         q, k, v = map(lambda t: rearrange(t, 'b (h c) x y -> b h c (x y)', h = self.heads), qkv)
 
         q = q.softmax(dim = -2)
         k = k.softmax(dim = -1)
 
         q = q * self.scale
-        v = v / (h * w)
 
         context = torch.einsum('b h d n, b h e n -> b h d e', k, v)
 
         out = torch.einsum('b h d e, b h d n -> b h e n', context, q)
         out = rearrange(out, 'b h c (x y) -> b (h c) x y', h = self.heads, x = h, y = w)
         return self.to_out(out)
```

### Comparing `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,14 @@
         qkv = self.to_qkv(x).chunk(3, dim = 1)
         q, k, v = map(lambda t: rearrange(t, 'b (h c) x y -> b h c (x y)', h = self.heads), qkv)
 
         q = q.softmax(dim = -2)
         k = k.softmax(dim = -1)
 
         q = q * self.scale
-        v = v / (h * w)
 
         context = torch.einsum('b h d n, b h e n -> b h d e', k, v)
 
         out = torch.einsum('b h d e, b h d n -> b h e n', context, q)
         out = rearrange(out, 'b h c (x y) -> b (h c) x y', h = self.heads, x = h, y = w)
         return self.to_out(out)
```

### Comparing `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,14 @@
         qkv = self.to_qkv(x).chunk(3, dim = 1)
         q, k, v = map(lambda t: rearrange(t, 'b (h c) x y -> b h c (x y)', h = self.heads), qkv)
 
         q = q.softmax(dim = -2)
         k = k.softmax(dim = -1)
 
         q = q * self.scale
-        v = v / (h * w)
 
         context = torch.einsum('b h d n, b h e n -> b h d e', k, v)
 
         out = torch.einsum('b h d e, b h d n -> b h e n', context, q)
         out = rearrange(out, 'b h c (x y) -> b (h c) x y', h = self.heads, x = h, y = w)
 
         return self.to_out(out) + residual
```

### Comparing `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.7.3
+Version: 1.7.4
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.7.3/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.7.4/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.3/setup.py` & `denoising-diffusion-pytorch-1.7.4/setup.py`

 * *Files identical despite different names*

