# Comparing `tmp/denoising-diffusion-pytorch-1.7.5.tar.gz` & `tmp/denoising-diffusion-pytorch-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.7.5.tar", last modified: Mon Jun 19 04:19:17 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.7.6.tar", last modified: Mon Jun 19 04:48:09 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.7.5.tar` & `denoising-diffusion-pytorch-1.7.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:19:17.730773 denoising-diffusion-pytorch-1.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 04:19:17.730773 denoising-diffusion-pytorch-1.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:19:17.730773 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    35643 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:19:17.730773 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 04:19:17.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-19 04:19:17.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 04:19:17.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 04:19:17.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 04:19:17.000000 denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 04:19:17.730773 denoising-diffusion-pytorch-1.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-19 04:18:58.000000 denoising-diffusion-pytorch-1.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:48:09.920618 denoising-diffusion-pytorch-1.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 04:48:09.920618 denoising-diffusion-pytorch-1.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:48:09.920618 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35717 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:48:09.920618 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 04:48:09.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-19 04:48:09.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 04:48:09.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 04:48:09.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 04:48:09.000000 denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 04:48:09.920618 denoising-diffusion-pytorch-1.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-19 04:48:00.000000 denoising-diffusion-pytorch-1.7.6/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.7.5/LICENSE` & `denoising-diffusion-pytorch-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.5/PKG-INFO` & `denoising-diffusion-pytorch-1.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.7.5
+Version: 1.7.6
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.7.5/README.md` & `denoising-diffusion-pytorch-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -820,31 +820,30 @@
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
         convert_image_to = None,
         calculate_fid = True,
-        inception_block_idx = 2048
+        inception_block_idx = 2048,
+        max_grad_norm = 1.
     ):
         super().__init__()
 
         # accelerator
 
         self.accelerator = Accelerator(
             split_batches = split_batches,
-            mixed_precision = 'fp16' if fp16 else 'no'
+            mixed_precision = mixed_precision_type if amp else 'no'
         )
 
-        self.accelerator.native_amp = amp
-
         # model
 
         self.model = diffusion_model
         self.channels = diffusion_model.channels
 
         # InceptionV3 for fid-score computation
 
@@ -864,14 +863,16 @@
 
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
@@ -977,15 +978,15 @@
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
```

### Comparing `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.7.5
+Version: 1.7.6
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.7.5/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.7.6/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.5/setup.py` & `denoising-diffusion-pytorch-1.7.6/setup.py`

 * *Files identical despite different names*

