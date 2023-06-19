# Comparing `tmp/sd_meh-0.7.0.tar.gz` & `tmp/sd_meh-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_meh-0.7.0.tar", max compression
+gzip compressed data, was "sd_meh-0.8.0.tar", max compression
```

## Comparing `sd_meh-0.7.0.tar` & `sd_meh-0.8.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1062 2023-06-13 19:20:47.976472 sd_meh-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     1002 2023-06-13 19:20:47.976472 sd_meh-0.7.0/README.md
--rw-r--r--   0        0        0      390 2023-06-13 19:20:47.980473 sd_meh-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-13 19:20:47.980473 sd_meh-0.7.0/sd_meh/__init__.py
--rw-r--r--   0        0        0    13082 2023-06-13 19:20:47.980473 sd_meh-0.7.0/sd_meh/merge.py
--rw-r--r--   0        0        0     6626 2023-06-13 19:20:47.980473 sd_meh-0.7.0/sd_meh/merge_methods.py
--rw-r--r--   0        0        0     1521 2023-06-13 19:20:47.980473 sd_meh-0.7.0/sd_meh/model.py
--rw-r--r--   0        0        0    10306 2023-06-13 19:20:47.980473 sd_meh-0.7.0/sd_meh/presets.py
--rw-r--r--   0        0        0    83404 2023-06-13 19:20:47.980473 sd_meh-0.7.0/sd_meh/rebasin.py
--rw-r--r--   0        0        0     1526 1970-01-01 00:00:00.000000 sd_meh-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-19 15:13:33.966544 sd_meh-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     1911 2023-06-19 15:13:33.966544 sd_meh-0.8.0/README.md
+-rw-r--r--   0        0        0      390 2023-06-19 15:13:33.966544 sd_meh-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-19 15:13:33.966544 sd_meh-0.8.0/sd_meh/__init__.py
+-rw-r--r--   0        0        0    13427 2023-06-19 15:13:33.966544 sd_meh-0.8.0/sd_meh/merge.py
+-rw-r--r--   0        0        0     6626 2023-06-19 15:13:33.966544 sd_meh-0.8.0/sd_meh/merge_methods.py
+-rw-r--r--   0        0        0     1606 2023-06-19 15:13:33.966544 sd_meh-0.8.0/sd_meh/model.py
+-rw-r--r--   0        0        0    10306 2023-06-19 15:13:33.966544 sd_meh-0.8.0/sd_meh/presets.py
+-rw-r--r--   0        0        0    83496 2023-06-19 15:13:33.966544 sd_meh-0.8.0/sd_meh/rebasin.py
+-rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 sd_meh-0.8.0/PKG-INFO
```

### Comparing `sd_meh-0.7.0/LICENSE.txt` & `sd_meh-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sd_meh-0.7.0/sd_meh/merge.py` & `sd_meh-0.8.0/sd_meh/merge.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import gc
+import logging
 import os
 import re
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Dict, Optional, Tuple
 
@@ -16,14 +17,15 @@
     apply_permutation,
     sdunet_permutation_spec,
     step_weights_and_bases,
     update_model_a,
     weight_matching,
 )
 
+logging.getLogger("sd_meh").addHandler(logging.NullHandler())
 MAX_TOKENS = 77
 NUM_INPUT_BLOCKS = 12
 NUM_MID_BLOCK = 1
 NUM_OUTPUT_BLOCKS = 12
 NUM_TOTAL_BLOCKS = NUM_INPUT_BLOCKS + NUM_MID_BLOCK + NUM_OUTPUT_BLOCKS
 
 KEY_POSITION_IDS = ".".join(
@@ -95,15 +97,15 @@
         if k not in merged_model:
             merged_model[k] = original_model[k]
     return merged_model
 
 
 def log_vram(txt=""):
     alloc = torch.cuda.memory_allocated(0)
-    print(f"{txt}: {alloc*1e-9:5.3f}")
+    logging.debug(f"{txt} VRAM: {alloc*1e-9:5.3f}GB")
 
 
 def load_thetas(
     models: Dict[str, os.PathLike | str],
     prune: bool,
     device: str,
     precision: int,
@@ -138,14 +140,15 @@
     device: str = "cpu",
     work_device: Optional[str] = None,
     prune: bool = False,
     threads: int = 1,
 ) -> Dict:
     thetas = load_thetas(models, prune, device, precision)
 
+    logging.info(f"start merging with {merge_mode} method")
     if re_basin:
         merged = rebasin_merge(
             thetas,
             weights,
             bases,
             merge_mode,
             precision=precision,
@@ -179,14 +182,15 @@
     thetas: Dict,
     models: Dict,
     device: str,
     prune: bool,
     precision: int,
 ) -> Dict:
     if prune:
+        logging.info("Un-pruning merged model")
         del thetas
         gc.collect()
         log_vram("remove thetas")
         original_a = load_sd_model(models["model_a"], device)
         for key in tqdm(original_a.keys(), desc="un-prune model a"):
             if KEY_POSITION_IDS in key:
                 continue
@@ -271,19 +275,24 @@
     threads: int = 1,
 ):
     # WARNING: not sure how this does when 3 models are involved...
 
     model_a = thetas["model_a"].clone()
     perm_spec = sdunet_permutation_spec()
 
-    print("permuting")
+    logging.info("Init rebasin iterations")
     for it in range(iterations):
-        # print(it)
+        logging.info(f"Rebasin iteration {it}")
         log_vram(f"{it} iteration start")
-        new_weights, new_bases = step_weights_and_bases(weights, bases, it, iterations)
+        new_weights, new_bases = step_weights_and_bases(
+            weights,
+            bases,
+            it,
+            iterations,
+        )
         log_vram("weights & bases, before simple merge")
 
         # normal block merge we already know and love
         thetas["model_a"] = simple_merge(
             thetas,
             new_weights,
             new_bases,
@@ -350,19 +359,19 @@
     key: str,
     thetas: Dict,
     weights: Dict,
     bases: Dict,
     merge_mode: str,
     precision: int = 16,
     weights_clip: bool = False,
-    storage_device: str = "cpu",
+    device: str = "cpu",
     work_device: Optional[str] = None,
 ) -> Optional[Tuple[str, Dict]]:
     if work_device is None:
-        work_device = storage_device
+        work_device = device
 
     if KEY_POSITION_IDS in key:
         return
 
     for theta in thetas.values():
         if key not in theta.keys():
             return
@@ -396,15 +405,15 @@
 
         try:
             merge_method = getattr(merge_methods, merge_mode)
         except AttributeError as e:
             raise ValueError(f"{merge_mode} not implemented, aborting merge!") from e
 
         merge_args = get_merge_method_args(current_bases, thetas, key, work_device)
-        merged_key = merge_method(**merge_args).to(storage_device)
+        merged_key = merge_method(**merge_args).to(device)
 
         if weights_clip:
             t0 = thetas["model_a"][key]
             t1 = thetas["model_b"][key]
             threshold = torch.maximum(torch.abs(t0), torch.abs(t1))
             merged_key = torch.minimum(torch.maximum(merged_key, -threshold), threshold)
 
@@ -412,17 +421,18 @@
             merged_key = merged_key.half()
 
         return merged_key
 
 
 def clip_weights(thetas, merged):
     for k, t0 in thetas["model_a"].items():
-        t1 = thetas["model_b"][k]
-        th = torch.maximum(torch.abs(t0), torch.abs(t1))
-        merged.update({k: torch.minimum(torch.maximum(merged[k], -th), th)})
+        if k in thetas["model_b"].keys():
+            t1 = thetas["model_b"][k]
+            th = torch.maximum(torch.abs(t0), torch.abs(t1))
+            merged.update({k: torch.minimum(torch.maximum(merged[k], -th), th)})
     return merged
 
 
 @contextmanager
 def merge_key_context(*args, **kwargs):
     result = merge_key(*args, **kwargs)
     try:
@@ -447,15 +457,15 @@
     if "model_c" in thetas:
         merge_method_args["c"] = thetas["model_c"][key].to(work_device)
 
     return merge_method_args
 
 
 def save_model(model, output_file, file_format) -> None:
-    print(f"saving {output_file}")
+    logging.info(f"Saving {output_file}")
     if file_format == "safetensors":
         safetensors.torch.save_file(
             model if type(model) == dict else model.to_dict(),
             f"{output_file}.safetensors",
             metadata={"format": "pt"},
         )
     else:
```

### Comparing `sd_meh-0.7.0/sd_meh/merge_methods.py` & `sd_meh-0.8.0/sd_meh/merge_methods.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.7.0/sd_meh/model.py` & `sd_meh-0.8.0/sd_meh/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,25 @@
+import logging
 import os
 from dataclasses import dataclass
 
 import safetensors
 import torch
 from tensordict import TensorDict
 
+logging.getLogger("sd_meh").addHandler(logging.NullHandler())
+
 
 @dataclass
 class SDModel:
     model_path: os.PathLike
     device: str
 
     def load_model(self):
-        print(f"loading: {self.model_path}")
+        logging.info(f"Loading: {self.model_path}")
         if self.model_path.suffix == ".safetensors":
             ckpt = safetensors.torch.load_file(
                 self.model_path,
                 device=self.device,
             )
         else:
             ckpt = torch.load(self.model_path, map_location=self.device)
```

### Comparing `sd_meh-0.7.0/sd_meh/presets.py` & `sd_meh-0.8.0/sd_meh/presets.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.7.0/sd_meh/rebasin.py` & `sd_meh-0.8.0/sd_meh/rebasin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # https://github.com/ogkalu2/Merge-Stable-Diffusion-models-without-distortion
-
-
+import logging
 from collections import defaultdict
 from random import shuffle
 from typing import Dict, NamedTuple, Tuple
 
 import torch
 from scipy.optimize import linear_sum_assignment
 
+logging.getLogger("sd_meh").addHandler(logging.NullHandler())
 SPECIAL_KEYS = [
     "first_stage_model.decoder.norm_out.weight",
     "first_stage_model.decoder.norm_out.bias",
     "first_stage_model.encoder.norm_out.weight",
     "first_stage_model.encoder.norm_out.bias",
     "model.diffusion_model.out.0.weight",
     "model.diffusion_model.out.0.bias",
@@ -2252,15 +2252,15 @@
     if usefp16:
         oldL = oldL.half()
         newL = newL.half()
 
     if newL - oldL != 0:
         linear_sum += abs((newL - oldL).item())
         number += 1
-        print(f" > {p}: {newL - oldL}")
+        logging.info(f" permutation {p}: {newL - oldL}")
 
     progress = progress or newL > oldL + 1e-12
 
     perm[p] = torch.Tensor(ci).to(device)
 
     return linear_sum, number, perm, progress
```

