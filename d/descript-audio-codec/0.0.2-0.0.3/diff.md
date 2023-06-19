# Comparing `tmp/descript-audio-codec-0.0.2.tar.gz` & `tmp/descript-audio-codec-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "descript-audio-codec-0.0.2.tar", last modified: Wed Jun 14 20:32:17 2023, max compression
+gzip compressed data, was "descript-audio-codec-0.0.3.tar", last modified: Mon Jun 19 19:31:56 2023, max compression
```

## Comparing `descript-audio-codec-0.0.2.tar` & `descript-audio-codec-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-14 20:32:17.217899 descript-audio-codec-0.0.2/
--rw-r--r--   0 ishaan    (1016) research  (1001)     1074 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.2/LICENSE
--rw-r--r--   0 ishaan    (1016) research  (1001)     5933 2023-06-14 20:32:17.217899 descript-audio-codec-0.0.2/PKG-INFO
--rw-r--r--   0 ishaan    (1016) research  (1001)     5176 2023-06-14 20:20:06.000000 descript-audio-codec-0.0.2/README.md
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-14 20:32:17.217899 descript-audio-codec-0.0.2/dac/
--rw-r--r--   0 ishaan    (1016) research  (1001)      198 2023-06-14 20:20:06.000000 descript-audio-codec-0.0.2/dac/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)      690 2023-06-14 20:20:06.000000 descript-audio-codec-0.0.2/dac/__main__.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-14 20:32:17.217899 descript-audio-codec-0.0.2/dac/compare/
--rw-r--r--   0 ishaan    (1016) research  (1001)        0 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.2/dac/compare/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     1592 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.2/dac/compare/encodec.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-14 20:32:17.217899 descript-audio-codec-0.0.2/dac/model/
--rw-r--r--   0 ishaan    (1016) research  (1001)       91 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.2/dac/model/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     4190 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.2/dac/model/base.py
--rw-r--r--   0 ishaan    (1016) research  (1001)    10483 2023-06-14 20:20:06.000000 descript-audio-codec-0.0.2/dac/model/dac.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     7056 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.2/dac/model/discriminator.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-14 20:32:17.217899 descript-audio-codec-0.0.2/dac/nn/
--rw-r--r--   0 ishaan    (1016) research  (1001)       63 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.2/dac/nn/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)      809 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.2/dac/nn/layers.py
--rw-r--r--   0 ishaan    (1016) research  (1001)    12042 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.2/dac/nn/loss.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     9067 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.2/dac/nn/quantize.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-14 20:32:17.217899 descript-audio-codec-0.0.2/dac/utils/
--rw-r--r--   0 ishaan    (1016) research  (1001)     1421 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.2/dac/utils/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     4795 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.2/dac/utils/decode.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     5234 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.2/dac/utils/encode.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-14 20:32:17.217899 descript-audio-codec-0.0.2/descript_audio_codec.egg-info/
--rw-r--r--   0 ishaan    (1016) research  (1001)     5933 2023-06-14 20:32:17.000000 descript-audio-codec-0.0.2/descript_audio_codec.egg-info/PKG-INFO
--rw-r--r--   0 ishaan    (1016) research  (1001)      596 2023-06-14 20:32:17.000000 descript-audio-codec-0.0.2/descript_audio_codec.egg-info/SOURCES.txt
--rw-r--r--   0 ishaan    (1016) research  (1001)        1 2023-06-14 20:32:17.000000 descript-audio-codec-0.0.2/descript_audio_codec.egg-info/dependency_links.txt
--rw-r--r--   0 ishaan    (1016) research  (1001)      194 2023-06-14 20:32:17.000000 descript-audio-codec-0.0.2/descript_audio_codec.egg-info/requires.txt
--rw-r--r--   0 ishaan    (1016) research  (1001)       10 2023-06-14 20:32:17.000000 descript-audio-codec-0.0.2/descript_audio_codec.egg-info/top_level.txt
--rw-r--r--   0 ishaan    (1016) research  (1001)       38 2023-06-14 20:32:17.217899 descript-audio-codec-0.0.2/setup.cfg
--rw-r--r--   0 ishaan    (1016) research  (1001)     1548 2023-06-14 20:29:10.000000 descript-audio-codec-0.0.2/setup.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-14 20:32:17.217899 descript-audio-codec-0.0.2/tests/
--rw-r--r--   0 ishaan    (1016) research  (1001)        0 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.2/tests/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     1284 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.2/tests/test_cli.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     2752 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.2/tests/test_train.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-19 19:31:56.568479 descript-audio-codec-0.0.3/
+-rw-r--r--   0 ishaan    (1016) research  (1001)     1074 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/LICENSE
+-rw-r--r--   0 ishaan    (1016) research  (1001)     5933 2023-06-19 19:31:56.568479 descript-audio-codec-0.0.3/PKG-INFO
+-rw-r--r--   0 ishaan    (1016) research  (1001)     5176 2023-06-14 20:20:06.000000 descript-audio-codec-0.0.3/README.md
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-19 19:31:56.564479 descript-audio-codec-0.0.3/dac/
+-rw-r--r--   0 ishaan    (1016) research  (1001)      198 2023-06-19 19:31:34.000000 descript-audio-codec-0.0.3/dac/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)      690 2023-06-14 20:20:06.000000 descript-audio-codec-0.0.3/dac/__main__.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-19 19:31:56.564479 descript-audio-codec-0.0.3/dac/compare/
+-rw-r--r--   0 ishaan    (1016) research  (1001)        0 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/dac/compare/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     1592 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/dac/compare/encodec.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-19 19:31:56.564479 descript-audio-codec-0.0.3/dac/model/
+-rw-r--r--   0 ishaan    (1016) research  (1001)       91 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/dac/model/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     4190 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/dac/model/base.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)    10483 2023-06-14 20:20:06.000000 descript-audio-codec-0.0.3/dac/model/dac.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     7056 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/dac/model/discriminator.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-19 19:31:56.568479 descript-audio-codec-0.0.3/dac/nn/
+-rw-r--r--   0 ishaan    (1016) research  (1001)       63 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/dac/nn/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)      809 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/dac/nn/layers.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)    12042 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/dac/nn/loss.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     9151 2023-06-19 19:31:34.000000 descript-audio-codec-0.0.3/dac/nn/quantize.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-19 19:31:56.568479 descript-audio-codec-0.0.3/dac/utils/
+-rw-r--r--   0 ishaan    (1016) research  (1001)     1421 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/dac/utils/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     4826 2023-06-19 19:31:34.000000 descript-audio-codec-0.0.3/dac/utils/decode.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     5252 2023-06-19 19:31:34.000000 descript-audio-codec-0.0.3/dac/utils/encode.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-19 19:31:56.568479 descript-audio-codec-0.0.3/descript_audio_codec.egg-info/
+-rw-r--r--   0 ishaan    (1016) research  (1001)     5933 2023-06-19 19:31:56.000000 descript-audio-codec-0.0.3/descript_audio_codec.egg-info/PKG-INFO
+-rw-r--r--   0 ishaan    (1016) research  (1001)      596 2023-06-19 19:31:56.000000 descript-audio-codec-0.0.3/descript_audio_codec.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaan    (1016) research  (1001)        1 2023-06-19 19:31:56.000000 descript-audio-codec-0.0.3/descript_audio_codec.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaan    (1016) research  (1001)      194 2023-06-19 19:31:56.000000 descript-audio-codec-0.0.3/descript_audio_codec.egg-info/requires.txt
+-rw-r--r--   0 ishaan    (1016) research  (1001)       10 2023-06-19 19:31:56.000000 descript-audio-codec-0.0.3/descript_audio_codec.egg-info/top_level.txt
+-rw-r--r--   0 ishaan    (1016) research  (1001)       38 2023-06-19 19:31:56.568479 descript-audio-codec-0.0.3/setup.cfg
+-rw-r--r--   0 ishaan    (1016) research  (1001)     1548 2023-06-19 19:31:34.000000 descript-audio-codec-0.0.3/setup.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-19 19:31:56.568479 descript-audio-codec-0.0.3/tests/
+-rw-r--r--   0 ishaan    (1016) research  (1001)        0 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/tests/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     1913 2023-06-19 19:31:34.000000 descript-audio-codec-0.0.3/tests/test_cli.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     2752 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/tests/test_train.py
```

### Comparing `descript-audio-codec-0.0.2/LICENSE` & `descript-audio-codec-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.2/PKG-INFO` & `descript-audio-codec-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: descript-audio-codec
-Version: 0.0.2
+Version: 0.0.3
 Summary: A high-quality general neural audio codec.
 Home-page: https://github.com/descriptinc/descript-audio-codec
 Author: Prem Seetharaman, Rithesh Kumar
 Author-email: prem@descript.com
 License: MIT
 Keywords: audio,compression,machine learning
 Classifier: Intended Audience :: Developers
```

### Comparing `descript-audio-codec-0.0.2/README.md` & `descript-audio-codec-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.2/dac/__main__.py` & `descript-audio-codec-0.0.3/dac/__main__.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.2/dac/compare/encodec.py` & `descript-audio-codec-0.0.3/dac/compare/encodec.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.2/dac/model/base.py` & `descript-audio-codec-0.0.3/dac/model/base.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.2/dac/model/dac.py` & `descript-audio-codec-0.0.3/dac/model/dac.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.2/dac/model/discriminator.py` & `descript-audio-codec-0.0.3/dac/model/discriminator.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.2/dac/nn/layers.py` & `descript-audio-codec-0.0.3/dac/nn/layers.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.2/dac/nn/loss.py` & `descript-audio-codec-0.0.3/dac/nn/loss.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.2/dac/nn/quantize.py` & `descript-audio-codec-0.0.3/dac/nn/quantize.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,14 +167,17 @@
             n_quantizers = torch.ones((z.shape[0],)) * self.n_codebooks + 1
             dropout = torch.randint(1, self.n_codebooks + 1, (z.shape[0],))
             n_dropout = int(z.shape[0] * self.quantizer_dropout)
             n_quantizers[:n_dropout] = dropout[:n_dropout]
             n_quantizers = n_quantizers.to(z.device)
 
         for i, quantizer in enumerate(self.quantizers):
+            if self.training is False and i >= n_quantizers:
+                break
+
             z_q_i, commitment_loss_i, codebook_loss_i, indices_i, z_e_i = quantizer(
                 residual
             )
 
             # Create mask to apply quantizer dropout
             mask = (
                 torch.full((z.shape[0],), fill_value=i, device=z.device) < n_quantizers
```

### Comparing `descript-audio-codec-0.0.2/dac/utils/__init__.py` & `descript-audio-codec-0.0.3/dac/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.2/dac/utils/decode.py` & `descript-audio-codec-0.0.3/dac/utils/decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,17 @@
 
     Returns
     -------
     AudioSignal
     """
     if isinstance(generator, torch.nn.DataParallel):
         generator = generator.module
-    audio_signal = AudioSignal(artifacts["codes"], generator.sample_rate)
+    audio_signal = AudioSignal(
+        artifacts["codes"].astype(np.int64), generator.sample_rate
+    )
     metadata = artifacts["metadata"]
 
     # Decode chunks
     output = []
     for i in range(audio_signal.batch_size):
         signal_from_batch = AudioSignal(
             audio_signal.audio_data[i, ...], audio_signal.sample_rate, device=device
```

### Comparing `descript-audio-codec-0.0.2/dac/utils/encode.py` & `descript-audio-codec-0.0.3/dac/utils/encode.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             signal_from_batch.audio_data, signal_from_batch.sample_rate, **kwargs
         )["codes"].cpu()
         codebook_indices.append(codes)
 
     codebook_indices = torch.cat(codebook_indices, dim=0)
 
     return {
-        "codes": codebook_indices.numpy(),
+        "codes": codebook_indices.numpy().astype(np.uint16),
         "metadata": {
             "original_db": input_db,
             "overlap_hop_duration": overlap_hop_duration,
             "original_length": original_length,
             "is_overlap": do_overlap_and_add,
             "batch_size": nb,
             "channels": nac,
```

### Comparing `descript-audio-codec-0.0.2/descript_audio_codec.egg-info/PKG-INFO` & `descript-audio-codec-0.0.3/descript_audio_codec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: descript-audio-codec
-Version: 0.0.2
+Version: 0.0.3
 Summary: A high-quality general neural audio codec.
 Home-page: https://github.com/descriptinc/descript-audio-codec
 Author: Prem Seetharaman, Rithesh Kumar
 Author-email: prem@descript.com
 License: MIT
 Keywords: audio,compression,machine learning
 Classifier: Intended Audience :: Developers
```

### Comparing `descript-audio-codec-0.0.2/descript_audio_codec.egg-info/SOURCES.txt` & `descript-audio-codec-0.0.3/descript_audio_codec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.2/setup.py` & `descript-audio-codec-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="descript-audio-codec",
-    version="0.0.2",
+    version="0.0.3",
     classifiers=[
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.7",
         "Topic :: Artistic Software",
         "Topic :: Multimedia",
         "Topic :: Multimedia :: Sound/Audio",
```

### Comparing `descript-audio-codec-0.0.2/tests/test_train.py` & `descript-audio-codec-0.0.3/tests/test_train.py`

 * *Files identical despite different names*

