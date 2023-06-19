# Comparing `tmp/tfts-0.0.6.tar.gz` & `tmp/tfts-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfts-0.0.6.tar", max compression
+gzip compressed data, was "tfts-0.0.7.tar", max compression
```

## Comparing `tfts-0.0.6.tar` & `tfts-0.0.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rwxr-xr-x   0        0        0     1093 2023-06-13 04:09:54.906426 tfts-0.0.6/LICENSE
--rw-r--r--   0        0        0    10195 2023-06-13 04:09:54.906426 tfts-0.0.6/README.md
--rw-r--r--   0        0        0     2346 2023-06-13 04:10:24.048173 tfts-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      462 2023-06-13 04:10:24.052173 tfts-0.0.6/tfts/__init__.py
--rw-r--r--   0        0        0       20 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/datasets/__init__.py
--rw-r--r--   0        0        0     3822 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/datasets/get_data.py
--rw-r--r--   0        0        0       20 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/features/__init__.py
--rw-r--r--   0        0        0      109 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/features/ar_feature.py
--rw-r--r--   0        0        0       49 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/features/time_feature.py
--rw-r--r--   0        0        0       42 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/features/two_order_feature.py
--rw-r--r--   0        0        0       18 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/layers/__init__.py
--rw-r--r--   0        0        0     9975 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/layers/attention_layer.py
--rw-r--r--   0        0        0     5329 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/layers/autoformer_layer.py
--rw-r--r--   0        0        0     3245 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/layers/cnn_layer.py
--rw-r--r--   0        0        0     1716 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/layers/deepar_layer.py
--rw-r--r--   0        0        0     4003 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/layers/dense_layer.py
--rw-r--r--   0        0        0     8593 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/layers/embed_layer.py
--rw-r--r--   0        0        0     1387 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/layers/mask_layer.py
--rw-r--r--   0        0        0     6420 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/layers/nbeats_layer.py
--rw-r--r--   0        0        0     4081 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/layers/unet_layer.py
--rw-r--r--   0        0        0       18 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/__init__.py
--rw-r--r--   0        0        0     2064 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/auto_config.py
--rw-r--r--   0        0        0     4263 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/auto_model.py
--rw-r--r--   0        0        0     7507 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/autoformer.py
--rw-r--r--   0        0        0     5721 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/bert.py
--rw-r--r--   0        0        0     1560 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/deepar.py
--rw-r--r--   0        0        0    10177 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/informer.py
--rw-r--r--   0        0        0     2784 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/nbeats.py
--rw-r--r--   0        0        0      123 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/patchtst.py
--rw-r--r--   0        0        0     7428 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/rnn.py
--rw-r--r--   0        0        0    13873 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/seq2seq.py
--rw-r--r--   0        0        0     5513 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/tcn.py
--rw-r--r--   0        0        0      111 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/tide.py
--rw-r--r--   0        0        0    18805 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/transformer.py
--rw-r--r--   0        0        0     4905 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/unet.py
--rw-r--r--   0        0        0    12701 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/wavenet.py
--rw-r--r--   0        0        0    13386 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/trainer.py
--rw-r--r--   0        0        0      429 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/tuner.py
--rw-r--r--   0        0        0    11461 1970-01-01 00:00:00.000000 tfts-0.0.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1093 2023-06-19 06:15:21.487797 tfts-0.0.7/LICENSE
+-rw-r--r--   0        0        0    10206 2023-06-19 06:15:21.487797 tfts-0.0.7/README.md
+-rw-r--r--   0        0        0     2346 2023-06-19 06:15:54.823986 tfts-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      462 2023-06-19 06:15:54.827986 tfts-0.0.7/tfts/__init__.py
+-rw-r--r--   0        0        0       20 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/datasets/__init__.py
+-rw-r--r--   0        0        0     3822 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/datasets/get_data.py
+-rw-r--r--   0        0        0       20 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/features/__init__.py
+-rw-r--r--   0        0        0      109 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/features/ar_feature.py
+-rw-r--r--   0        0        0       49 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/features/time_feature.py
+-rw-r--r--   0        0        0       42 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/features/two_order_feature.py
+-rw-r--r--   0        0        0       18 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/layers/__init__.py
+-rw-r--r--   0        0        0     9988 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/layers/attention_layer.py
+-rw-r--r--   0        0        0     5329 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/layers/autoformer_layer.py
+-rw-r--r--   0        0        0     3245 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/layers/cnn_layer.py
+-rw-r--r--   0        0        0     1716 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/layers/deepar_layer.py
+-rw-r--r--   0        0        0     4003 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/layers/dense_layer.py
+-rw-r--r--   0        0        0     8593 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/layers/embed_layer.py
+-rw-r--r--   0        0        0     1408 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/layers/mask_layer.py
+-rw-r--r--   0        0        0     6420 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/layers/nbeats_layer.py
+-rw-r--r--   0        0        0     4081 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/layers/unet_layer.py
+-rw-r--r--   0        0        0       18 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/models/__init__.py
+-rw-r--r--   0        0        0     2064 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/models/auto_config.py
+-rw-r--r--   0        0        0     4263 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/models/auto_model.py
+-rw-r--r--   0        0        0     7507 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/models/autoformer.py
+-rw-r--r--   0        0        0     5721 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/models/bert.py
+-rw-r--r--   0        0        0     1560 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/models/deepar.py
+-rw-r--r--   0        0        0    10357 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/models/informer.py
+-rw-r--r--   0        0        0     2784 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/models/nbeats.py
+-rw-r--r--   0        0        0      123 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/models/patchtst.py
+-rw-r--r--   0        0        0     7429 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/models/rnn.py
+-rw-r--r--   0        0        0    14814 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/models/seq2seq.py
+-rw-r--r--   0        0        0     5513 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/models/tcn.py
+-rw-r--r--   0        0        0      111 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/models/tide.py
+-rw-r--r--   0        0        0    18138 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/models/transformer.py
+-rw-r--r--   0        0        0     4905 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/models/unet.py
+-rw-r--r--   0        0        0    12708 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/models/wavenet.py
+-rw-r--r--   0        0        0    13386 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/trainer.py
+-rw-r--r--   0        0        0      429 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/tuner.py
+-rw-r--r--   0        0        0    11472 1970-01-01 00:00:00.000000 tfts-0.0.7/PKG-INFO
```

### Comparing `tfts-0.0.6/LICENSE` & `tfts-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tfts-0.0.6/README.md` & `tfts-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,15 @@
 - rnn
 - tcn
 - bert
 - nbeats
 - seq2seq
 - wavenet
 - transformer
+- informer
 
 </details>
 
 You could build the custom model based on tfts, especially
 - add custom-defined embeddings for categorical variables
 - add custom-defined head layers for classification or anomaly task
```

### Comparing `tfts-0.0.6/pyproject.toml` & `tfts-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 [tool.nbqa.mutate]
 isort = 1
 black = 1
 
 [tool.poetry]
 name = "tfts"
 readme = "README.md"  # Markdown files are supported
-version = "0.0.6"  # is being replaced automatically
+version = "0.0.7"  # is being replaced automatically
 
 authors = ["Longxing Tan"]
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
```

### Comparing `tfts-0.0.6/tfts/datasets/get_data.py` & `tfts-0.0.7/tfts/datasets/get_data.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.6/tfts/layers/attention_layer.py` & `tfts-0.0.7/tfts/layers/attention_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         tf.Tensor
             tensor with shape batch * seq_q * (units * num_heads)
         """
         q = self.dense_q(q)  # project the query/key/value to num_heads * units
         k = self.dense_k(k)
         v = self.dense_v(v)
 
-        q_ = tf.concat(tf.split(q, self.num_heads, axis=2), axis=0)  # multi-heads transfer to
+        q_ = tf.concat(tf.split(q, self.num_heads, axis=2), axis=0)  # multi-heads transfer to multi-sample
         k_ = tf.concat(tf.split(k, self.num_heads, axis=2), axis=0)
         v_ = tf.concat(tf.split(v, self.num_heads, axis=2), axis=0)
 
         score = tf.linalg.matmul(q_, k_, transpose_b=True)  # => (batch * heads) * seq_q * seq_k
         score /= tf.cast(tf.shape(q_)[-1], tf.float32) ** 0.5
 
         if mask is not None:
```

### Comparing `tfts-0.0.6/tfts/layers/autoformer_layer.py` & `tfts-0.0.7/tfts/layers/autoformer_layer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.6/tfts/layers/cnn_layer.py` & `tfts-0.0.7/tfts/layers/cnn_layer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.6/tfts/layers/deepar_layer.py` & `tfts-0.0.7/tfts/layers/deepar_layer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.6/tfts/layers/dense_layer.py` & `tfts-0.0.7/tfts/layers/dense_layer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.6/tfts/layers/embed_layer.py` & `tfts-0.0.7/tfts/layers/embed_layer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.6/tfts/layers/mask_layer.py` & `tfts-0.0.7/tfts/layers/mask_layer.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,43 +2,40 @@
 # @author: Longxing Tan, tanlongxing888@163.com
 """Layer for :py:class:`~tfts.models.transformer`"""
 
 import tensorflow as tf
 from tensorflow.keras import activations, constraints, initializers, regularizers
 
 
-class MaskLayer(tf.keras.layers.Layer):
-    def __init__(self):
-        super().__init__()
+class CausalMask:
+    """Casual Mask is used for transformer decoder, used in first self-attention for decoder feature"""
 
-
-class TriangularCausalMask:
     def __init__(self, B, L):
-        mask_shape = [B, 1, L, L]
-
+        mask_shape = [B, L, L]  # for multi-heads split [B, 1, L, L]
         mask_a = tf.linalg.band_part(tf.ones(mask_shape), 0, -1)  # Upper triangular matrix of 0s and 1s
         mask_b = tf.linalg.band_part(tf.ones(mask_shape), 0, 0)  # Diagonal matrix of 0s and 1s
         mask = tf.cast(mask_a - mask_b, dtype=tf.float32)
 
         self._mask = mask
         tf.stop_gradient(self._mask)
 
     @property
     def mask(self):
         return self._mask
 
 
 class ProbMask:
+    """ProbMask for informer"""
+
     def __init__(self, B, H, L, index, scores):
         # B: batch_size, H: num_heads, L: seq_length
         mask = tf.ones([L, scores.shape[-1]], tf.float32)
 
         mask = 1 - tf.linalg.band_part(mask, -1, 0)
         mask_expanded = tf.broadcast_to(mask, [B, H, L, scores.shape[-1]])
         # mask specific q based on reduced Q
-        print(mask_expanded.shape, index.shape)
         mask_Q = tf.gather_nd(mask_expanded, index)
         self._mask = tf.cast(tf.reshape(mask_Q, scores.shape), tf.bool)
 
     @property
     def mask(self):
         return self._mask
```

### Comparing `tfts-0.0.6/tfts/layers/nbeats_layer.py` & `tfts-0.0.7/tfts/layers/nbeats_layer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.6/tfts/layers/unet_layer.py` & `tfts-0.0.7/tfts/layers/unet_layer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.6/tfts/models/auto_config.py` & `tfts-0.0.7/tfts/models/auto_config.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.6/tfts/models/auto_model.py` & `tfts-0.0.7/tfts/models/auto_model.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.6/tfts/models/autoformer.py` & `tfts-0.0.7/tfts/models/autoformer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.6/tfts/models/bert.py` & `tfts-0.0.7/tfts/models/bert.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.6/tfts/models/deepar.py` & `tfts-0.0.7/tfts/models/deepar.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.6/tfts/models/informer.py` & `tfts-0.0.7/tfts/models/informer.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Dropout,
     LayerNormalization,
     MaxPool1D,
 )
 
 from tfts.layers.attention_layer import FullAttention, ProbAttention
 from tfts.layers.embed_layer import DataEmbedding, TokenEmbedding
+from tfts.layers.mask_layer import CausalMask
 
 params = {
     "n_encoder_layers": 1,
     "n_decoder_layers": 1,
     "attention_hidden_sizes": 32 * 1,
     "num_heads": 1,
     "attention_dropout": 0.0,
@@ -44,16 +45,16 @@
         custom_model_params: Optional[Dict[str, Any]] = None,
         custom_model_head: Optional[Callable] = None,
     ):
         if custom_model_params:
             params.update(custom_model_params)
         self.params = params
         self.predict_sequence_length = predict_sequence_length
-        self.encoder_embedding = TokenEmbedding(params["attention_hidden_sizes"])
-        self.decoder_embedding = TokenEmbedding(params["attention_hidden_sizes"])
+        self.encoder_embedding = DataEmbedding(params["attention_hidden_sizes"])
+        self.decoder_embedding = DataEmbedding(params["attention_hidden_sizes"])
         if not params["prob_attention"]:
             attn_layer = FullAttention(
                 params["attention_hidden_sizes"], params["num_heads"], params["attention_dropout"]
             )
         else:
             attn_layer = ProbAttention(
                 params["attention_hidden_sizes"], params["num_heads"], params["attention_dropout"]
@@ -114,16 +115,19 @@
             decoder_feature = tf.cast(
                 tf.reshape(tf.range(self.predict_sequence_length), (-1, self.predict_sequence_length, 1)), tf.float32
             )
 
         encoder_feature = self.encoder_embedding(encoder_feature)  # batch * seq * embedding_size
         memory = self.encoder(encoder_feature, mask=None)
 
+        B, L, _ = tf.shape(decoder_feature)
+        casual_mask = CausalMask(B * self.params["num_heads"], L).mask
         decoder_feature = self.decoder_embedding(decoder_feature)
-        outputs = self.decoder(decoder_feature, memory=memory)
+
+        outputs = self.decoder(decoder_feature, memory=memory, x_mask=casual_mask)
         outputs = self.projection(outputs)
 
         if self.params["skip_connect_circle"]:
             x_mean = x[:, -self.predict_sequence_length :, 0:1]
             outputs = outputs + x_mean
         if self.params["skip_connect_mean"]:
             x_mean = tf.tile(tf.reduce_mean(x[..., 0:1], axis=1, keepdims=True), [1, self.predict_sequence_length, 1])
```

### Comparing `tfts-0.0.6/tfts/models/nbeats.py` & `tfts-0.0.7/tfts/models/nbeats.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.6/tfts/models/rnn.py` & `tfts-0.0.7/tfts/models/rnn.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
         self.params = params
         self.predict_sequence_length = predict_sequence_length
         self.rnn = GRU(units=params["rnn_size"], activation="tanh", return_state=True, return_sequences=True, dropout=0)
         self.dense1 = Dense(predict_sequence_length)
         self.dense2 = Dense(1)
 
     def __call__(self, inputs, teacher=None):
-        """_summary_
+        """RNN model2
 
         Parameters
         ----------
         inputs : _type_
             _description_
         teacher : _type_, optional
             _description_, by default None
```

### Comparing `tfts-0.0.6/tfts/models/seq2seq.py` & `tfts-0.0.7/tfts/models/seq2seq.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,22 +51,22 @@
             use_attention=params["use_attention"],
             attention_sizes=params["attention_sizes"],
             attention_heads=params["attention_heads"],
             attention_dropout=params["attention_dropout"],
         )
 
     def __call__(self, inputs, teacher=None):
-        """A RNN seq2seq structure for time series
+        """An RNN seq2seq structure for time series
 
         :param inputs: _description_
         :type inputs: _type_
         :param teacher: teacher forcing decoding, defaults to None
         :type teacher: _type_, optional
         :return: _description_
-        :rtype: _type_
+        :type: _type_
         """
         if isinstance(inputs, (list, tuple)):
             x, encoder_feature, decoder_feature = inputs
             encoder_feature = tf.concat([x, encoder_feature], axis=-1)
         elif isinstance(inputs, dict):
             x = inputs["x"]
             encoder_feature = inputs["encoder_feature"]
@@ -101,44 +101,50 @@
             decoder_outputs = decoder_outputs + x_mean
         return decoder_outputs
 
 
 class Encoder(tf.keras.layers.Layer):
     def __init__(self, rnn_type, rnn_size, rnn_dropout=0, dense_size=32, **kwargs):
         super(Encoder, self).__init__(**kwargs)
+        self.rnn_type = rnn_type
         if rnn_type.lower() == "gru":
             self.rnn = GRU(
                 units=rnn_size, activation="tanh", return_state=True, return_sequences=True, dropout=rnn_dropout
             )
-        elif self.rnn_type.lower() == "lstm":
+        elif rnn_type.lower() == "lstm":
             self.rnn = LSTM(
-                units=self.rnn_size,
+                units=rnn_size,
                 activation="tanh",
                 return_state=True,
                 return_sequences=True,
-                dropout=self.rnn_dropout,
+                dropout=rnn_dropout,
             )
         self.dense = Dense(units=dense_size, activation="tanh")
 
     def call(self, inputs):
-        """_summary_
+        """Seq2seq encoder
 
         Parameters
         ----------
-        inputs : _type_
+        inputs : tf.Tensor
             _description_
 
         Returns
         -------
-        _type_
-            _description_
+        tf.Tensor
+            batch_size * input_seq_length * rnn_size, state: batch_size * rnn_size
         """
-        # outputs: batch_size * input_seq_length * rnn_size, state: batch_size * rnn_size
-        outputs, state = self.rnn(inputs)
-        state = self.dense(state)
+        if self.rnn_type.lower() == "gru":
+            outputs, state = self.rnn(inputs)
+            state = self.dense(state)
+        elif self.rnn_type.lower() == "lstm":
+            outputs, state1, state2 = self.rnn(inputs)
+            state = (state1, state2)
+        else:
+            raise ValueError("No supported rnn type of {}".format(self.rnn_type))
         # encoder_hidden_state = tuple(self.dense(hidden_state) for _ in range(params['num_stacked_layers']))
         # outputs = self.dense(outputs)  # => batch_size * input_seq_length * dense_size
         return outputs, state
 
 
 class Decoder1(tf.keras.layers.Layer):
     def __init__(
@@ -160,34 +166,35 @@
         self.attention_heads = attention_heads
         self.attention_dropout = attention_dropout
 
     def build(self, input_shape):
         if self.rnn_type.lower() == "gru":
             self.rnn_cell = GRUCell(self.rnn_size)
         elif self.rnn_type.lower() == "lstm":
-            self.rnn = LSTMCell(units=self.rnn_size)
+            self.rnn_cell = LSTMCell(units=self.rnn_size)
         self.dense = Dense(units=1, activation=None)
         if self.use_attention:
             self.attention = FullAttention(
                 hidden_size=self.attention_sizes,
                 num_heads=self.attention_heads,
                 attention_dropout=self.attention_dropout,
             )
+        super().build(input_shape)
 
     def call(
         self,
         decoder_features,
         decoder_init_input,
         init_state,
         teacher=None,
         scheduler_sampling=0,
         training=None,
         **kwargs
     ):
-        """_summary_
+        """Seq2seq decoder1: step by step
 
         :param decoder_features: _description_
         :type decoder_features: _type_
         :param decoder_init_input: _description_
         :type decoder_init_input: _type_
         :param init_state: _description_
         :type init_state: _type_
@@ -217,18 +224,29 @@
             else:
                 this_input = prev_output
 
             if decoder_features is not None:
                 this_input = tf.concat([this_input, decoder_features[:, i]], axis=-1)
 
             if self.use_attention:
-                att = self.attention(
-                    tf.expand_dims(prev_state, 1), k=kwargs["encoder_output"], v=kwargs["encoder_output"]
-                )
-                att = tf.squeeze(att, 1)
+                if self.rnn_type.lower() == "gru":
+                    # q: (batch, 1, feature), att_output: (batch, 1, feature)
+                    att = self.attention(
+                        tf.expand_dims(prev_state, 1), k=kwargs["encoder_output"], v=kwargs["encoder_output"]
+                    )
+                    att = tf.squeeze(att, 1)  # (batch, feature)
+                elif self.rnn_type.lower() == "lstm":
+                    # q: (batch, 1, feature * 2), att_output: (batch, 1, feature)
+                    att = self.attention(
+                        tf.expand_dims(tf.concat(prev_state, 1), 1),
+                        k=kwargs["encoder_output"],
+                        v=kwargs["encoder_output"],
+                    )
+                    att = tf.squeeze(att, 1)  # (batch, feature)
+
                 this_input = tf.concat([this_input, att], axis=-1)
 
             this_output, this_state = self.rnn_cell(this_input, prev_state)
             prev_state = this_state
             prev_output = self.dense(this_output)
             decoder_outputs.append(prev_output)
 
@@ -264,14 +282,15 @@
         self.dense = Dense(units=1)
         if self.use_attention:
             self.attention = FullAttention(
                 hidden_size=self.attention_sizes,
                 num_heads=self.attention_heads,
                 attention_dropout=self.attention_dropout,
             )
+        super().build(input_shape)
 
     def forward(
         self,
         decoder_feature,
         decoder_init_value,
         init_state,
         teacher=None,
@@ -323,26 +342,24 @@
         decoder_init_input,
         init_state,
         teacher=None,
         scheduler_sampling=0,
         training=None,
         **kwargs
     ):
-        """_summary_
+        """Decoder model2
 
         Parameters
         ----------
         decoder_feature : _type_
             _description_
         init_state : _type_
             _description_
         decoder_init_input : _type_
             _description_
-        encoder_output : _type_
-            _description_
         teacher : _type_, optional
             _description_, by default None
 
         Returns
         -------
         _type_
             _description_
@@ -380,15 +397,15 @@
         decoder_init_input,
         init_state,
         teacher=None,
         scheduler_sampling=0,
         training=None,
         **kwargs
     ):
-        """_summary_
+        """Decoder3: just simple
 
         Parameters
         ----------
         decoder_features : _type_
             _description_
         decoder_init_input : _type_
             _description_
```

### Comparing `tfts-0.0.6/tfts/models/tcn.py` & `tfts-0.0.7/tfts/models/tcn.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.6/tfts/models/transformer.py` & `tfts-0.0.7/tfts/models/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import numpy as np
 import tensorflow as tf
 from tensorflow.keras.layers import Dense, Dropout, LayerNormalization, TimeDistributed
 
 from tfts.layers.attention_layer import FullAttention, SelfAttention
 from tfts.layers.dense_layer import FeedForwardNetwork
 from tfts.layers.embed_layer import DataEmbedding, TokenEmbedding
+from tfts.layers.mask_layer import CausalMask
 
 params = {
     "n_encoder_layers": 1,
     "n_decoder_layers": 1,
     "use_token_embedding": False,
     "attention_hidden_sizes": 32 * 1,
     "num_heads": 1,
@@ -46,37 +47,28 @@
         :param dynamic_decoding: _description_, defaults to True
         :type dynamic_decoding: bool, optional
         """
         if custom_model_params:
             params.update(custom_model_params)
         self.params = params
         self.predict_sequence_length = predict_sequence_length
-        self.encoder_embedding = TokenEmbedding(params["attention_hidden_sizes"])
+        self.encoder_embedding = DataEmbedding(params["attention_hidden_sizes"])
 
         self.encoder = Encoder(
             params["n_encoder_layers"],
             params["attention_hidden_sizes"],
             params["num_heads"],
             params["attention_dropout"],
             params["ffn_hidden_sizes"],
             params["ffn_filter_sizes"],
             params["ffn_dropout"],
         )
-        # self.decoder = Decoder(
-        #     predict_sequence_length,
-        #     params['n_decoder_layers'],
-        #     params['attention_hidden_sizes'],
-        #     params['num_heads'],
-        #     params['attention_dropout'],
-        #     params['ffn_hidden_sizes'],
-        #     params['ffn_filter_sizes'],
-        #     params['ffn_dropout'])
+
         self.decoder = Decoder2(
-            predict_sequence_length,
-            embed_layer=TokenEmbedding(params["attention_hidden_sizes"]),
+            embed_layer=DataEmbedding(params["attention_hidden_sizes"]),
             att_layers=[
                 DecoderLayer2(
                     params["n_decoder_layers"],
                     params["attention_hidden_sizes"],
                     params["num_heads"],
                     params["attention_dropout"],
                     params["ffn_hidden_sizes"],
@@ -86,27 +78,27 @@
                 for _ in range(params["n_decoder_layers"])
             ],
             # norm_layer = LayerNormalization()
         )
         self.project = Dense(1, activation=None)
 
     def __call__(self, inputs, teacher=None):
-        """_summary_
+        """Time series transformer
 
         Parameters
         ----------
-        inputs : _type_
-            _description_
-        teacher : _type_, optional
+        inputs : tf.Tensor
+            3D tensor for batch * seq_len * features
+        teacher : tf.Tensor, optional
             _description_, by default None
 
         Returns
         -------
-        _type_
-            _description_
+        tf.Tensor
+            3D tensor for output, batch * output_seq * 1
         """
         if isinstance(inputs, (list, tuple)):
             x, encoder_feature, decoder_feature = inputs
             encoder_feature = tf.concat([x, encoder_feature], axis=-1)
         elif isinstance(inputs, dict):
             x = inputs["x"]
             encoder_feature = inputs["encoder_feature"]
@@ -122,15 +114,18 @@
                 tf.float32,
             )
 
         encoder_feature = self.encoder_embedding(encoder_feature)  # batch * seq * embedding_size
         memory = self.encoder(encoder_feature, src_mask=None)
 
         # decoder_outputs = self.decoder(decoder_features, init_input=x[:, -1:], encoder_memory=memory, teacher=teacher)
-        decoder_outputs = self.decoder(decoder_feature, memory)
+
+        B, L, _ = tf.shape(decoder_feature)
+        casual_mask = CausalMask(B * self.params["num_heads"], L).mask
+        decoder_outputs = self.decoder(decoder_feature, memory, x_mask=casual_mask)
         decoder_outputs = self.project(decoder_outputs)
 
         if self.params["skip_connect_circle"]:
             x_mean = x[:, -self.predict_sequence_length :, 0:1]
             decoder_outputs = decoder_outputs + x_mean
         if self.params["skip_connect_mean"]:
             x_mean = tf.tile(tf.reduce_mean(x[..., 0:1], axis=1, keepdims=True), [1, self.predict_sequence_length, 1])
@@ -165,15 +160,15 @@
             feed_forward_layer = FeedForwardNetwork(self.ffn_hidden_sizes, self.ffn_filter_sizes, self.ffn_dropout)
             ln_layer1 = LayerNormalization(epsilon=1e-6, dtype="float32")
             ln_layer2 = LayerNormalization(epsilon=1e-6, dtype="float32")
             self.layers.append([attention_layer, ln_layer1, feed_forward_layer, ln_layer2])
         super(Encoder, self).build(input_shape)
 
     def call(self, encoder_inputs, src_mask=None):
-        """_summary_
+        """Transformer encoder
 
         Parameters
         ----------
         encoder_inputs : _type_
             _description_
         src_mask : _type_, optional
             _description_, by default None
@@ -326,15 +321,15 @@
             ln_layer3 = LayerNormalization(epsilon=self.eps, dtype="float32")
             self.layers.append(
                 [self_attention_layer, enc_dec_attention_layer, feed_forward_layer, ln_layer1, ln_layer2, ln_layer3]
             )
         super(DecoderLayer, self).build(input_shape)
 
     def call(self, decoder_inputs, encoder_memory, tgt_mask=None, cross_mask=None):
-        """_summary_
+        """Decoder layer
 
         Parameters
         ----------
         decoder_inputs : _type_
             _description_
         encoder_memory : _type_
             _description_
@@ -372,69 +367,55 @@
             "ffn_dropout": self.ffn_dropout,
         }
         base_config = super(DecoderLayer, self).get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
 
 class Decoder2(tf.keras.layers.Layer):
-    def __init__(self, predict_sequence_length, embed_layer, att_layers, norm_layer=None) -> None:
+    def __init__(self, embed_layer, att_layers, norm_layer=None) -> None:
         super().__init__()
-        self.predict_sequence_length = predict_sequence_length
         self.att_layers = att_layers
         self.norm = norm_layer
         self.decoder_embedding = embed_layer
         self.drop = Dropout(0.2)
         # self.dense1 = TimeDistributed(Dense(256))
         # self.drop1 = TimeDistributed(Dropout(0.2))
         self.dense2 = TimeDistributed(Dense(32))
         self.drop2 = TimeDistributed(Dropout(0.1))
         self.proj = TimeDistributed(Dense(1))
 
-    def decode(self, x, cross, x_mask, cross_mask):
-        x = self.decoder_embedding(x)
-        for layer in self.att_layers:
-            x = layer(x, cross, x_mask, cross_mask)
-        if self.norm is not None:
-            x = self.norm(x)
-        return x
-
-    def call(self, x, cross, x_mask=None, cross_mask=None, training=True):
-        """_summary_
+    def call(self, x, memory, x_mask=None, memory_mask=None):
+        """Transformer decoder2
 
         Parameters
         ----------
         x : _type_
             _description_
-        cross : _type_
+        memory : _type_
             _description_
         x_mask : _type_, optional
             _description_, by default None
-        cross_mask : _type_, optional
+        memory_mask : _type_, optional
             _description_, by default None
-        training : bool, optional
-            _description_, by default True
 
         Returns
         -------
-        _type_
+        tf.Tensor
             _description_
         """
-        x = self.decode(x, cross, x_mask, cross_mask)
+        x = self.decoder_embedding(x)
+        for layer in self.att_layers:
+            x = layer(x, memory, x_mask, memory_mask)
+        if self.norm is not None:
+            x = self.norm(x)
+
         x = self.drop(x)
         x = self.dense2(x)
         x = self.drop2(x)
         x = self.proj(x)
-
-        # if training:
-        #     x = self.decode(x, cross, x_mask, cross_mask)
-        # else:
-        # for _ in range(self.predict_sequence_length):
-        #     x1 = self.decode(x, cross, x_mask, cross_mask)
-        #     print(x1.shape, x.shape)
-        #     x = tf.concat([x, x1], axis=0)
         return x
 
 
 class DecoderLayer2(tf.keras.layers.Layer):
     def __init__(
         self,
         n_decoder_layers,
@@ -466,45 +447,45 @@
             ln_layer2 = LayerNormalization(epsilon=self.eps, dtype="float32")
             ln_layer3 = LayerNormalization(epsilon=self.eps, dtype="float32")
             self.layers.append(
                 [self_attention_layer, enc_dec_attention_layer, feed_forward_layer, ln_layer1, ln_layer2, ln_layer3]
             )
         super(DecoderLayer2, self).build(input_shape)
 
-    def call(self, decoder_inputs, encoder_memory, tgt_mask=None, cross_mask=None):
-        """_summary_
+    def call(self, decoder_inputs, encoder_memory, decoder_mask=None, memory_mask=None):
+        """Decoder layer2
 
         Parameters
         ----------
         decoder_inputs : _type_
             _description_
         encoder_memory : _type_
             _description_
         tgt_mask : _type_, optional
             _description_, by default None
-        cross_mask : _type_, optional
+        memory_mask : _type_, optional
             _description_, by default None
 
         Returns
         -------
         _type_
             _description_
         """
         x = decoder_inputs
 
         for _, layer in enumerate(self.layers):
             self_attention_layer, enc_dec_attention_layer, ffn_layer, ln_layer1, ln_layer2, ln_layer3 = layer
-            dec1 = x
-            # dec = self_attention_layer(dec, mask=tgt_mask)
-            # dec1 = ln_layer1(x + dec)
-            dec1 = enc_dec_attention_layer(dec1, encoder_memory, encoder_memory, mask=cross_mask)
+            dec = x
+            dec = self_attention_layer(dec, mask=decoder_mask)
+            dec1 = ln_layer1(x + dec)
+            dec1 = enc_dec_attention_layer(dec1, encoder_memory, encoder_memory, mask=memory_mask)
             dec2 = ln_layer2(x + dec1)
             dec2 = ffn_layer(dec2)
-            # x = ln_layer3(dec1 + dec2)
-            x = dec1 + dec2
+            x = ln_layer3(dec1 + dec2)  # note that don't repeat ln
+            # x = dec1 + dec2
         return x
 
     def get_config(self):
         config = {
             "n_decoder_layers": self.n_decoder_layers,
             "attention_hidden_sizes": self.attention_hidden_sizes,
             "num_heads": self.num_heads,
```

### Comparing `tfts-0.0.6/tfts/models/unet.py` & `tfts-0.0.7/tfts/models/unet.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.6/tfts/models/wavenet.py` & `tfts-0.0.7/tfts/models/wavenet.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         decoder_init_input,
         encoder_outputs,
         teacher=None,
         scheduler_sampling=0,
         training=None,
         **kwargs
     ):
-        """_summary_
+        """wavenet decoder1
 
         Parameters
         ----------
         decoder_features : _type_
             _description_
         decoder_init_input : _type_
             _description_
```

### Comparing `tfts-0.0.6/tfts/trainer.py` & `tfts-0.0.7/tfts/trainer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.6/PKG-INFO` & `tfts-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfts
-Version: 0.0.6
+Version: 0.0.7
 Summary: Deep learning time series with TensorFlow
 Home-page: https://time-series-prediction.readthedocs.io
 Author: Longxing Tan
 Requires-Python: >=3.7.1,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -225,14 +225,15 @@
 - rnn
 - tcn
 - bert
 - nbeats
 - seq2seq
 - wavenet
 - transformer
+- informer
 
 </details>
 
 You could build the custom model based on tfts, especially
 - add custom-defined embeddings for categorical variables
 - add custom-defined head layers for classification or anomaly task
```

