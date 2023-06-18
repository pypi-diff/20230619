# Comparing `tmp/torch_adapters-0.0.5.tar.gz` & `tmp/torch_adapters-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_adapters-0.0.5.tar", max compression
+gzip compressed data, was "torch_adapters-0.0.6.tar", max compression
```

## Comparing `torch_adapters-0.0.5.tar` & `torch_adapters-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1062 2023-05-29 03:00:27.152099 torch_adapters-0.0.5/LICENSE
--rw-r--r--   0        0        0      365 2023-06-03 17:10:11.157420 torch_adapters-0.0.5/README.md
--rw-r--r--   0        0        0      576 2023-06-03 17:10:11.125420 torch_adapters-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 03:01:19.456108 torch_adapters-0.0.5/src/torch_adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 03:03:05.272210 torch_adapters-0.0.5/src/torch_adapters/adapters/__init__.py
--rw-r--r--   0        0        0     1112 2023-06-03 16:58:19.487497 torch_adapters-0.0.5/src/torch_adapters/adapters/adapter.py
--rw-r--r--   0        0        0     1731 2023-06-03 16:44:50.108688 torch_adapters-0.0.5/src/torch_adapters/adapters/lora.py
--rw-r--r--   0        0        0      193 2023-05-30 14:23:42.706006 torch_adapters-0.0.5/src/torch_adapters/adapters/mixin.py
--rw-r--r--   0        0        0     3161 2023-06-01 19:54:15.021807 torch_adapters-0.0.5/src/torch_adapters/adapters/prompt_tuning.py
--rw-r--r--   0        0        0     4038 2023-06-03 17:04:27.528683 torch_adapters-0.0.5/src/torch_adapters/utils.py
--rw-r--r--   0        0        0     1150 1970-01-01 00:00:00.000000 torch_adapters-0.0.5/setup.py
--rw-r--r--   0        0        0     1111 1970-01-01 00:00:00.000000 torch_adapters-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-29 03:00:27.152099 torch_adapters-0.0.6/LICENSE
+-rw-r--r--   0        0        0      428 2023-06-18 22:29:51.003591 torch_adapters-0.0.6/README.md
+-rw-r--r--   0        0        0      576 2023-06-18 22:29:51.023591 torch_adapters-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 03:01:19.456108 torch_adapters-0.0.6/src/torch_adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 03:03:05.272210 torch_adapters-0.0.6/src/torch_adapters/adapters/__init__.py
+-rw-r--r--   0        0        0     1204 2023-06-10 02:56:28.071451 torch_adapters-0.0.6/src/torch_adapters/adapters/adapter.py
+-rw-r--r--   0        0        0     1946 2023-06-18 22:34:23.207267 torch_adapters-0.0.6/src/torch_adapters/adapters/lora.py
+-rw-r--r--   0        0        0      196 2023-06-10 02:56:28.027452 torch_adapters-0.0.6/src/torch_adapters/adapters/mixin.py
+-rw-r--r--   0        0        0     2725 2023-06-11 23:42:58.493986 torch_adapters-0.0.6/src/torch_adapters/adapters/prefix_tuning.py
+-rw-r--r--   0        0        0     3408 2023-06-10 02:56:28.115450 torch_adapters-0.0.6/src/torch_adapters/adapters/prompt_tuning.py
+-rw-r--r--   0        0        0     5083 2023-06-18 22:30:55.755535 torch_adapters-0.0.6/src/torch_adapters/utils.py
+-rw-r--r--   0        0        0     1219 1970-01-01 00:00:00.000000 torch_adapters-0.0.6/setup.py
+-rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 torch_adapters-0.0.6/PKG-INFO
```

### Comparing `torch_adapters-0.0.5/LICENSE` & `torch_adapters-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_adapters-0.0.5/pyproject.toml` & `torch_adapters-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "torch-adapters"
-version = "0.0.5"
+version = "0.0.6"
 description = "Small Library of Torch Adaptation modules"
 authors = ["ma2za <mazzapaolo2019@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "torch_adapters", from = "src" }]
 
 repository = "https://github.com/ma2za/torch-adapters"
```

### Comparing `torch_adapters-0.0.5/src/torch_adapters/adapters/adapter.py` & `torch_adapters-0.0.6/src/torch_adapters/adapters/adapter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 from collections import OrderedDict
 
-import torch.nn.init
-from torch import nn, Tensor
-from torch.nn import GELU
+from torch import Tensor
+from torch.nn import GELU, init, Linear, Module, Sequential
 
 from torch_adapters.adapters.mixin import AdapterMixin
 
+__all__ = ["Adapter"]
 
-class Adapter(AdapterMixin, nn.Module):
+
+class Adapter(AdapterMixin, Module):
     """
 
     Parameter-Efficient Transfer Learning for NLP
     by Neil Houlsby, Andrei Giurgiu, Stanislaw Jastrzebski, Bruna Morrone,
     Quentin de Laroussilhe, Andrea Gesmundo, Mona Attariyan, Sylvain Gelly
 
     """
 
-    def __init__(self,
-                 src: nn.Linear,
-                 adapter_size: int):
+    def __init__(self, src: Linear, adapter_size: int):
         super().__init__()
         self.src = src
-        self.adapter = nn.Sequential(OrderedDict([
-            ("A", nn.Linear(src.out_features, adapter_size, bias=True)),
-            ("act", GELU()),
-            ("B", nn.Linear(adapter_size, src.out_features, bias=True))
-        ]))
+        self.adapter = Sequential(
+            OrderedDict(
+                [
+                    ("A", Linear(src.out_features, adapter_size, bias=True)),
+                    ("act", GELU()),
+                    ("B", Linear(adapter_size, src.out_features, bias=True)),
+                ]
+            )
+        )
+
+        self.reset_parameters()
 
     def reset_parameters(self):
         # TODO check if gaussian init is the standard
         for param in self.adapter.parameters():
-            torch.nn.init.zeros_(param)
+            init.zeros_(param)
 
     def forward(self, input: Tensor) -> Tensor:
         output = self.src(input)
         return self.adapter(output) + output
```

### Comparing `torch_adapters-0.0.5/src/torch_adapters/adapters/lora.py` & `torch_adapters-0.0.6/src/torch_adapters/adapters/lora.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,60 @@
 from collections import OrderedDict
 
 from torch import nn, Tensor
 
 from torch_adapters.adapters.mixin import AdapterMixin
 
+__all__ = ["LoRA"]
+
 
 class LoRA(nn.Linear, AdapterMixin):
     """
 
     Layers to train at finetuning: adapter, layer-norm, classifier.
 
     LoRA: Low-Rank Adaptation of Large Language Models
     by Edward J. Hu, Yelong Shen, Phillip Wallis, Zeyuan Allen-Zhu,
     Yuanzhi Li, Shean Wang, Lu Wang, Weizhu Chen
     https://arxiv.org/abs/2106.09685
 
     """
 
-    def __init__(self,
-                 src: nn.Linear,
-                 alpha: int = 8,
-                 r: int = 8):
+    def __init__(
+            self, src: nn.Linear, alpha: int = 8, r: int = 8, dropout: float = 0.0
+    ):
         super().__init__(src.in_features, src.out_features)
 
         self.copy_attributes_from_source(src)
 
-        self.lora_weight = nn.Sequential(OrderedDict([
-            ("A", nn.Linear(self.in_features, r, bias=False)),
-            ("B", nn.Linear(r, self.out_features, bias=False))
-        ]))
+        # TODO check dropout location
+        self.lora_weight = nn.Sequential(
+            OrderedDict(
+                [
+                    ("A", nn.Linear(self.in_features, r, bias=False)),
+                    ("dropout", nn.Dropout(p=dropout)),
+                    ("B", nn.Linear(r, self.out_features, bias=False)),
+                ]
+            )
+        )
 
         self.alpha = alpha
         self.r = r
 
         nn.init.zeros_(self.lora_weight.B.weight)
         nn.init.normal_(self.lora_weight.A.weight)
 
     def merge(self) -> nn.Linear:
         # TODO add copy of other attributes
         # TODO check if matrix transpose is required
         merged_layer = nn.Linear(self.in_features, self.out_features)
         merged_weight = self.weight.data + (self.alpha / self.r) * (
-                self.lora_weight.B.weight.data @ self.lora_weight.A.weight.data)
+                self.lora_weight.B.weight.data @ self.lora_weight.A.weight.data
+        )
         merged_layer.weight.data = merged_weight.detach().clone().to(self.weight.device)
         merged_layer.bias.data = self.bias.data.detach().clone().to(self.bias.device)
         return merged_layer
 
     def forward(self, input_ids: Tensor) -> Tensor:
-        return super().forward(input_ids) + self.lora_weight(input_ids) * (self.alpha / self.r)
+        return super().forward(input_ids) + self.lora_weight(input_ids) * (
+                self.alpha / self.r
+        )
```

### Comparing `torch_adapters-0.0.5/src/torch_adapters/adapters/prompt_tuning.py` & `torch_adapters-0.0.6/src/torch_adapters/adapters/prompt_tuning.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,80 +1,103 @@
 import torch
 from torch import nn, Tensor
 from torch.nn import Parameter
 
 from torch_adapters.adapters.mixin import AdapterMixin
 
+__all__ = [
+    "prompt_attention_mask",
+    "PromptTokenTypeEmbedding",
+    "PromptAbsolutePositionalEmbedding",
+    "PromptTuningEmbedding",
+]
+
 
 def prompt_attention_mask(attention_mask: Tensor, prompt_length: int) -> Tensor:
     """
 
     :param attention_mask:
     :param prompt_length:
     :return:
     """
-    prompt_mask = torch.ones((attention_mask.shape[0], prompt_length),
-                             dtype=attention_mask.dtype,
-                             device=attention_mask.device)
+    prompt_mask = torch.ones(
+        (attention_mask.shape[0], prompt_length),
+        dtype=attention_mask.dtype,
+        device=attention_mask.device,
+    )
     return torch.cat([prompt_mask, attention_mask], dim=-1)
 
 
 class PromptTokenTypeEmbedding(nn.Embedding, AdapterMixin):
     def __init__(self, src: nn.Embedding, prompt_length: int):
-        super().__init__(num_embeddings=src.num_embeddings,
-                         embedding_dim=src.embedding_dim)
+        super().__init__(
+            num_embeddings=src.num_embeddings, embedding_dim=src.embedding_dim
+        )
 
         self.copy_attributes_from_source(src)
         self.prompt_length = prompt_length
 
     def forward(self, input: Tensor) -> Tensor:
         prompt = input[:, 0].unsqueeze(1).expand(-1, self.prompt_length)
         extended_input = torch.cat([prompt, input], dim=1)
         return super().forward(extended_input)
 
 
 class PromptAbsolutePositionalEmbedding(nn.Embedding, AdapterMixin):
     def __init__(self, src: nn.Embedding, prompt_length: int):
-        super().__init__(num_embeddings=src.num_embeddings,
-                         embedding_dim=src.embedding_dim)
+        super().__init__(
+            num_embeddings=src.num_embeddings, embedding_dim=src.embedding_dim
+        )
 
         self.copy_attributes_from_source(src)
         self.prompt_length = prompt_length
 
     def forward(self, input: Tensor) -> Tensor:
-        prompt_ids = torch.arange(1, 1 + self.prompt_length, dtype=torch.long, device=input.device)
+        prompt_ids = torch.arange(
+            1, 1 + self.prompt_length, dtype=torch.long, device=input.device
+        )
         prompt_ids = prompt_ids.unsqueeze(0).expand(input.shape[0], -1)
         mask = input.ne(self.padding_idx).int()
         incremental_indices = (input - self.padding_idx + prompt_ids.max()) * mask
-        extended_input = torch.cat([prompt_ids, incremental_indices], dim=1) + self.padding_idx
+        extended_input = (
+            torch.cat([prompt_ids, incremental_indices], dim=1) + self.padding_idx
+        )
         return super().forward(extended_input)
 
 
 class PromptTuningEmbedding(nn.Embedding, AdapterMixin):
     """
 
     The Power of Scale for Parameter-Efficient Prompt Tuning
     by Brian Lester, Rami Al-Rfou and Noah Constant
     https://arxiv.org/abs/2104.08691
 
     """
 
-    def __init__(self,
-                 src: nn.Embedding,
-                 prompt_length: int):
-        super().__init__(num_embeddings=src.num_embeddings,
-                         embedding_dim=src.embedding_dim)
+    def __init__(self, src: nn.Embedding, prompt_length: int):
+        super().__init__(
+            num_embeddings=src.num_embeddings, embedding_dim=src.embedding_dim
+        )
 
         self.copy_attributes_from_source(src)
         self.prompt_length = prompt_length
 
         self.prompt_embedding = nn.Embedding(self.prompt_length, self.embedding_dim)
 
         # TODO add random init, best 5000 sampling and text init and move to reset_parameters method
-        self.prompt_embedding.weight = Parameter(self.weight[torch.randint(0, self.weight.shape[0], (
-            self.prompt_embedding.num_embeddings,))].detach().clone())
+        self.prompt_embedding.weight = Parameter(
+            self.weight[
+                torch.randint(
+                    0, self.weight.shape[0], (self.prompt_embedding.num_embeddings,)
+                )
+            ]
+            .detach()
+            .clone()
+        )
 
     def forward(self, input: Tensor) -> Tensor:
-        prompt_ids = torch.arange(self.prompt_length, dtype=torch.long, device=input.device)
+        prompt_ids = torch.arange(
+            self.prompt_length, dtype=torch.long, device=input.device
+        )
         prompt_ids = prompt_ids.unsqueeze(0).expand(input.shape[0], -1)
         prompt = self.prompt_embedding(prompt_ids)
         return torch.cat([prompt, self.weight[input]], dim=1)
```

### Comparing `torch_adapters-0.0.5/src/torch_adapters/utils.py` & `torch_adapters-0.0.6/src/torch_adapters/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,24 +2,58 @@
 from typing import List, Dict
 
 import torch
 from torch import nn
 
 from .adapters.adapter import Adapter
 from .adapters.lora import LoRA
-from .adapters.prompt_tuning import PromptTuningEmbedding, PromptTokenTypeEmbedding, \
-    PromptAbsolutePositionalEmbedding
+from .adapters.prefix_tuning import PrefixTuning
+from .adapters.prompt_tuning import (
+    PromptTuningEmbedding,
+    PromptTokenTypeEmbedding,
+    PromptAbsolutePositionalEmbedding,
+)
 
 
 # TODO group in a utility class
 
 # TODO consider if unify in one add method with configuration
 
 
-def add_adapter(model: nn.Module, layers_names: List[str], config: Dict) -> torch.nn.Module:
+def add_prefix_tuning(
+        model: nn.Module, layers_names: List[str], config: Dict
+) -> torch.nn.Module:
+    for name, module in model.named_modules():
+        if any([i in name for i in layers_names]):
+            module_name, attr_name = name.rsplit(".", 1)
+            module: nn.Module = attrgetter(module_name)(model)
+            if attr_name not in layers_names:
+                continue
+            attr: nn.Module = attrgetter(name)(model)
+            module.__setattr__(
+                attr_name,
+                PrefixTuning(
+                    attr,
+                    prefix_size=config.get("prefix_size", 64),
+                    hidden_size=config.get("prefix_size", 768),
+                ),
+            )
+    return model
+
+
+def drop_prefix_tuning_reparametrization(model: nn.Module):
+    for name, module in model.named_modules():
+        if isinstance(module, PrefixTuning):
+            module.drop()
+    return model
+
+
+def add_adapter(
+        model: nn.Module, layers_names: List[str], config: Dict
+) -> torch.nn.Module:
     """
 
     :param model:
     :param layers_names:
     :param config:
     :return:
     """
@@ -29,19 +63,23 @@
             module: nn.Module = attrgetter(module_name)(model)
             attr: nn.Module = attrgetter(name)(model)
 
             # TODO specialize exception
             if not isinstance(attr, nn.Linear):
                 raise Exception
 
-            module.__setattr__(attr_name, Adapter(attr, adapter_size=config.get("adapter_size", 64)))
+            module.__setattr__(
+                attr_name, Adapter(attr, adapter_size=config.get("adapter_size", 64))
+            )
     return model
 
 
-def add_lora(model: nn.Module, layers_names: List[str], config: Dict) -> torch.nn.Module:
+def add_lora(
+        model: nn.Module, layers_names: List[str], config: Dict
+) -> torch.nn.Module:
     """
 
     Replace in-place the linear layers named in layers_names with a LoRA layer
     having the same weight and bias parameters.
 
     :param model:
     :param layers_names:
@@ -56,23 +94,25 @@
             module: nn.Module = attrgetter(module_name)(model)
             attr: nn.Linear = attrgetter(name)(model)
 
             # TODO specialize exception
             if not isinstance(attr, nn.Linear):
                 raise Exception
 
-            module.__setattr__(attr_name, LoRA(
-                attr,
-                alpha=config.get("alpha", 8),
-                r=config.get("r", 8)
-            ))
+            module.__setattr__(
+                attr_name,
+                LoRA(attr,
+                     alpha=config.get("alpha", 8),
+                     r=config.get("r", 8),
+                     dropout=config.get("dropout", 0.0)),
+            )
     return model
 
 
-def merge_lora(model, layers_names):
+def merge_lora(model):
     for name, module in model.named_modules():
         if isinstance(module, LoRA):
             module_name, attr_name = name.rsplit(".", 1)
             parent_module: nn.Module = attrgetter(module_name)(model)
             parent_module.__setattr__(attr_name, module.merge())
     return model
 
@@ -84,23 +124,26 @@
             if attr_name not in embeddings.keys():
                 continue
             module: nn.Module = attrgetter(module_name)(model)
             attr: nn.Embedding = attrgetter(name)(model)
             embedding_type = embeddings.get(attr_name)
             extended_embedding = None
             if embedding_type == "word":
-                extended_embedding = PromptTuningEmbedding(src=attr,
-                                                           prompt_length=config.get("prompt_length", 30))
+                extended_embedding = PromptTuningEmbedding(
+                    src=attr, prompt_length=config.get("prompt_length", 30)
+                )
             elif embedding_type == "token_type":
-                extended_embedding = PromptTokenTypeEmbedding(src=attr,
-                                                              prompt_length=config.get("prompt_length", 30))
+                extended_embedding = PromptTokenTypeEmbedding(
+                    src=attr, prompt_length=config.get("prompt_length", 30)
+                )
             elif embedding_type == "position":
                 # TODO check relative embeddings
-                extended_embedding = PromptAbsolutePositionalEmbedding(src=attr,
-                                                                       prompt_length=config.get("prompt_length", 30))
+                extended_embedding = PromptAbsolutePositionalEmbedding(
+                    src=attr, prompt_length=config.get("prompt_length", 30)
+                )
             if extended_embedding is None:
                 # TODO replace with custom exception
                 raise Exception
             module.__setattr__(attr_name, extended_embedding)
     return model
```

### Comparing `torch_adapters-0.0.5/setup.py` & `torch_adapters-0.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['torch>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'torch-adapters',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': 'Small Library of Torch Adaptation modules',
-    'long_description': '# Torch Adapters\n\n> <em>"During a gold rush, sell shovels."</em>\n\n# Introduction\n\nSmall Library of Torch Adaptation modules\n\n### Supported Methods\n\n- [X] LoRA\n- [X] Prompt Tuning\n- [X] Bottleneck Adapter\n\n# Installation\n\nYou can install torch-adapters using:\n\n    $ pip install torch-adapters\n\n# Usage\n\n    $ add_lora(model, ["key", "value"], {"alpha": 8, "r": 8})\n',
+    'long_description': '# Torch Adapters\n\n# Introduction\n\nSmall Library of Torch Adaptation modules\n\n### Supported Methods\n\n- [X] LoRA\n- [X] Prompt Tuning\n- [X] Bottleneck Adapter\n- [X] Prefix Tuning\n- [ ] P-Tuning\n\n# Installation\n\nYou can install torch-adapters using:\n\n    $ pip install torch-adapters\n\n# Usage\n\n```python\nfrom torch_adapters.utils import add_lora\n\n# Add lora to the model\nadd_lora(model, ["key", "value"], {"alpha": 8, "r": 8})\n```\n\n',
     'author': 'ma2za',
     'author_email': 'mazzapaolo2019@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ma2za/torch-adapters',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `torch_adapters-0.0.5/PKG-INFO` & `torch_adapters-0.0.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-adapters
-Version: 0.0.5
+Version: 0.0.6
 Summary: Small Library of Torch Adaptation modules
 Home-page: https://github.com/ma2za/torch-adapters
 License: MIT
 Keywords: lora,adapters,llm,transformers,bert
 Author: ma2za
 Author-email: mazzapaolo2019@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -16,29 +16,35 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://github.com/ma2za/torch-adapters
 Description-Content-Type: text/markdown
 
 # Torch Adapters
 
-> <em>"During a gold rush, sell shovels."</em>
-
 # Introduction
 
 Small Library of Torch Adaptation modules
 
 ### Supported Methods
 
 - [X] LoRA
 - [X] Prompt Tuning
 - [X] Bottleneck Adapter
+- [X] Prefix Tuning
+- [ ] P-Tuning
 
 # Installation
 
 You can install torch-adapters using:
 
     $ pip install torch-adapters
 
 # Usage
 
-    $ add_lora(model, ["key", "value"], {"alpha": 8, "r": 8})
+```python
+from torch_adapters.utils import add_lora
+
+# Add lora to the model
+add_lora(model, ["key", "value"], {"alpha": 8, "r": 8})
+```
+
```

