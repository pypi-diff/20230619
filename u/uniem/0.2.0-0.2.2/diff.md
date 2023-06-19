# Comparing `tmp/uniem-0.2.0.tar.gz` & `tmp/uniem-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniem-0.2.0.tar", max compression
+gzip compressed data, was "uniem-0.2.2.tar", max compression
```

## Comparing `uniem-0.2.0.tar` & `uniem-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-05-09 07:54:15.399692 uniem-0.2.0/LICENSE
--rw-r--r--   0        0        0     6101 2023-06-15 11:16:21.191745 uniem-0.2.0/README.md
--rw-r--r--   0        0        0      607 2023-06-15 11:18:52.184649 uniem-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      104 2023-06-15 11:25:08.185076 uniem-0.2.0/uniem/__init__.py
--rw-r--r--   0        0        0     6884 2023-06-15 05:12:54.271051 uniem-0.2.0/uniem/criteria.py
--rw-r--r--   0        0        0    10028 2023-06-15 11:23:52.141569 uniem-0.2.0/uniem/data.py
--rw-r--r--   0        0        0      628 2023-06-15 08:39:00.949540 uniem-0.2.0/uniem/data_structures.py
--rw-r--r--   0        0        0     8004 2023-06-15 10:13:33.939494 uniem-0.2.0/uniem/finetuner.py
--rw-r--r--   0        0        0    13637 2023-06-15 11:44:36.163028 uniem-0.2.0/uniem/model.py
--rw-r--r--   0        0        0     5860 2023-06-15 09:39:32.604643 uniem-0.2.0/uniem/trainer.py
--rw-r--r--   0        0        0      659 2023-06-07 06:09:24.419876 uniem-0.2.0/uniem/types.py
--rw-r--r--   0        0        0      915 2023-06-15 08:02:39.812246 uniem-0.2.0/uniem/utils.py
--rw-r--r--   0        0        0       22 2023-05-22 10:36:54.260085 uniem-0.2.0/uniem/version.py
--rw-r--r--   0        0        0     6997 1970-01-01 00:00:00.000000 uniem-0.2.0/setup.py
--rw-r--r--   0        0        0     6723 1970-01-01 00:00:00.000000 uniem-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-19 08:27:50.354983 uniem-0.2.2/LICENSE
+-rw-r--r--   0        0        0     5252 2023-06-19 08:27:50.354983 uniem-0.2.2/README.md
+-rw-r--r--   0        0        0      793 2023-06-19 08:27:50.366984 uniem-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-06-19 08:27:50.470985 uniem-0.2.2/uniem/__init__.py
+-rw-r--r--   0        0        0     7166 2023-06-19 08:27:50.470985 uniem-0.2.2/uniem/criteria.py
+-rw-r--r--   0        0        0    10988 2023-06-19 08:27:50.470985 uniem-0.2.2/uniem/data.py
+-rw-r--r--   0        0        0     1089 2023-06-19 08:27:50.470985 uniem-0.2.2/uniem/data_structures.py
+-rw-r--r--   0        0        0    13985 2023-06-19 08:27:50.470985 uniem-0.2.2/uniem/finetuner.py
+-rw-r--r--   0        0        0    13796 2023-06-19 08:27:50.470985 uniem-0.2.2/uniem/model.py
+-rw-r--r--   0        0        0     6025 2023-06-19 08:27:50.470985 uniem-0.2.2/uniem/trainer.py
+-rw-r--r--   0        0        0      658 2023-06-19 08:27:50.470985 uniem-0.2.2/uniem/types.py
+-rw-r--r--   0        0        0     1663 2023-06-19 08:27:50.470985 uniem-0.2.2/uniem/utils.py
+-rw-r--r--   0        0        0       22 2023-06-19 08:27:50.470985 uniem-0.2.2/uniem/version.py
+-rw-r--r--   0        0        0     5887 1970-01-01 00:00:00.000000 uniem-0.2.2/PKG-INFO
```

### Comparing `uniem-0.2.0/LICENSE` & `uniem-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uniem-0.2.0/pyproject.toml` & `uniem-0.2.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 [tool.poetry]
 name = "uniem"
-version = "0.2.0"
+version = "0.2.2"
 description = "unified embedding model"
 authors = ["wangyuxin <wangyuxin@mokahr.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-torch = "^2.0.0"
 transformers = "^4.28.0"
 accelerate = "^0.19.0"
 tqdm = "^4.65.0"
 typer = {extras = ["all"], version = "^0.9.0"}
 datasets = "^2.12.0"
 
-
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 blue = "^0.9.1"
 ruff = "^0.0.265"
 isort = "^5.12.0"
+pyright = "^1.1.314"
+
+[tool.poetry.group.mteb.dependencies]
 mteb = "^1.0.2"
+openai = "^0.27.8"
+sentence-transformers = "^2.2.2"
 
 [tool.ruff]
 line-length = 128
+select = [
+    'E',
+    'F',
+    'I',
+    'N'
+]
+src = ['uniem', 'mteb-zh/mteb_zh', 'tests']
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `uniem-0.2.0/uniem/criteria.py` & `uniem-0.2.2/uniem/criteria.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 
 class PairInBatchNegCoSentLoss(ContrastLoss):
     def forward(
         self,
         text_embeddings: torch.Tensor,
         text_pos_embeddings: torch.Tensor,
     ) -> torch.Tensor:
-        sim_matrix = torch.cosine_similarity(text_embeddings.unsqueeze(1), text_pos_embeddings.unsqueeze(0), dim=-1)
+        sim_matrix = torch.cosine_similarity(
+            text_embeddings.unsqueeze(1),
+            text_pos_embeddings.unsqueeze(0),
+            dim=-1,
+        )
         sim_matrix = sim_matrix / self.temperature
         sim_matrix_diag = sim_matrix.diag()
         sim_matrix_diff = sim_matrix - sim_matrix_diag.unsqueeze(1)
         loss = torch.logsumexp(sim_matrix_diff, dim=1).mean()
         return loss
 
 
@@ -33,15 +37,19 @@
     def forward(
         self,
         text_embeddings: torch.Tensor,
         text_pos_embeddings: torch.Tensor,
         text_neg_embeddings: torch.Tensor,
     ) -> torch.Tensor:
         sim_pos_vector = torch.cosine_similarity(text_embeddings, text_pos_embeddings, dim=-1)
-        sim_neg_matrix = torch.cosine_similarity(text_embeddings.unsqueeze(1), text_neg_embeddings.unsqueeze(0), dim=-1)
+        sim_neg_matrix = torch.cosine_similarity(
+            text_embeddings.unsqueeze(1),
+            text_neg_embeddings.unsqueeze(0),
+            dim=-1,
+        )
         sim_matrix = torch.cat([sim_pos_vector.unsqueeze(1), sim_neg_matrix], dim=1)
         sim_matrix = sim_matrix / self.temperature
         sim_matrix_diff = sim_matrix - sim_matrix[:, 0].unsqueeze(1)
         loss = torch.logsumexp(sim_matrix_diff, dim=1).mean()
         if self._pair_contrast_softmax_loss:
             loss += self._pair_contrast_softmax_loss(text_pos_embeddings, text_embeddings)
         return loss
@@ -54,15 +62,19 @@
         self._cross_entropy_loss = torch.nn.CrossEntropyLoss()
 
     def forward(
         self,
         text_embeddings: torch.Tensor,
         text_pos_embeddings: torch.Tensor,
     ) -> torch.Tensor:
-        sim_matrix = torch.cosine_similarity(text_embeddings.unsqueeze(1), text_pos_embeddings.unsqueeze(0), dim=-1)
+        sim_matrix = torch.cosine_similarity(
+            text_embeddings.unsqueeze(1),
+            text_pos_embeddings.unsqueeze(0),
+            dim=-1,
+        )
         sim_matrix = sim_matrix / self.temperature
         labels = torch.arange(sim_matrix.size(0), device=text_embeddings.device, dtype=torch.long)
         loss = self._cross_entropy_loss(sim_matrix, labels)
         return loss
 
 
 class TripletInBatchNegSoftmaxContrastLoss(ContrastLoss):
@@ -77,15 +89,19 @@
     def forward(
         self,
         text_embeddings: torch.Tensor,
         text_pos_embeddings: torch.Tensor,
         text_neg_embeddings: torch.Tensor,
     ) -> torch.Tensor:
         sim_pos_vector = torch.cosine_similarity(text_embeddings, text_pos_embeddings, dim=-1)
-        sim_neg_matrix = torch.cosine_similarity(text_embeddings.unsqueeze(1), text_neg_embeddings.unsqueeze(0), dim=-1)
+        sim_neg_matrix = torch.cosine_similarity(
+            text_embeddings.unsqueeze(1),
+            text_neg_embeddings.unsqueeze(0),
+            dim=-1,
+        )
         sim_matrix = torch.cat([sim_pos_vector.unsqueeze(1), sim_neg_matrix], dim=1)
         sim_matrix = sim_matrix / self.temperature
         labels = torch.zeros(sim_matrix.size(0), dtype=torch.long, device=sim_matrix.device)
         loss = torch.nn.CrossEntropyLoss()(sim_matrix, labels)
         if self._pair_contrast_softmax_loss:
             loss += self._pair_contrast_softmax_loss(text_pos_embeddings, text_embeddings)
         return loss
@@ -98,15 +114,19 @@
 
     def forward(
         self,
         text_embeddings: torch.Tensor,
         text_pos_embeddings: torch.Tensor,
     ) -> torch.Tensor:
         batch_size = text_embeddings.size(0)
-        sim_matrix = torch.cosine_similarity(text_embeddings.unsqueeze(1), text_pos_embeddings.unsqueeze(0), dim=-1)
+        sim_matrix = torch.cosine_similarity(
+            text_embeddings.unsqueeze(1),
+            text_pos_embeddings.unsqueeze(0),
+            dim=-1,
+        )
         sim_matrix = sim_matrix / self.temperature
         sim_matrix_diag = sim_matrix.diag()
 
         sim_diff_matrix = sim_matrix_diag.unsqueeze(1) - sim_matrix
         diag_mask = torch.eye(sim_matrix.size(0), dtype=torch.bool, device=sim_matrix.device)
         sim_diff_matrix = sim_diff_matrix.masked_fill(diag_mask, 1e9)
 
@@ -127,15 +147,19 @@
         self,
         text_embeddings: torch.Tensor,
         text_pos_embeddings: torch.Tensor,
         text_neg_embeddings: torch.Tensor,
     ) -> torch.Tensor:
         sim_pos_vector = torch.cosine_similarity(text_embeddings, text_pos_embeddings, dim=-1)
         sim_pos_vector = sim_pos_vector / self.temperature
-        sim_neg_matrix = torch.cosine_similarity(text_embeddings.unsqueeze(1), text_neg_embeddings.unsqueeze(0), dim=-1)
+        sim_neg_matrix = torch.cosine_similarity(
+            text_embeddings.unsqueeze(1),
+            text_neg_embeddings.unsqueeze(0),
+            dim=-1,
+        )
         sim_neg_matrix = sim_neg_matrix / self.temperature
         sim_diff_matrix = sim_pos_vector.unsqueeze(1) - sim_neg_matrix
         loss = -torch.log(torch.sigmoid(sim_diff_matrix)).mean()
         if self._pair_contrast_sigmoid_loss:
             loss += self._pair_contrast_sigmoid_loss(text_pos_embeddings, text_embeddings)
         return loss
```

### Comparing `uniem-0.2.0/uniem/data.py` & `uniem-0.2.2/uniem/data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 import json
 from collections import defaultdict
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Any, cast, Sequence
+from typing import Any, Sequence, cast
 
 import torch
+from datasets import Dataset as HfDataset
 from torch.utils.data import Dataset, RandomSampler
 
-from datasets import Dataset as HfDataset
-from uniem.data_structures import RecordType, PairRecord, ScoredPairRecord, TripletRecord, record_type_cls_map
+from uniem.data_structures import (
+    PairRecord,
+    RecordType,
+    ScoredPairRecord,
+    TripletRecord,
+    get_record_type,
+    record_type_cls_map,
+)
 from uniem.types import Tokenizer
 
 
 class PairCollator:
     def __init__(self, tokenizer: Tokenizer, max_length: int | None = None) -> None:
         self.tokenizer = tokenizer
         self.max_length = max_length or tokenizer.model_max_length
@@ -120,27 +127,56 @@
             'text_ids': text_ids,
             'text_pair_ids': text_pair_ids,
             'labels': labels,
         }
 
 
 class FinetuneDataset(Dataset):
-    def __init__(self, dataset: HfDataset | Sequence[dict], record_type: RecordType | str) -> None:
+    def __init__(
+        self,
+        dataset: HfDataset | Sequence[dict],
+        record_type: RecordType | str | None = None,
+    ) -> None:
         self.dataset = dataset
-        self.record_type = RecordType(record_type)
+        if record_type:
+            self.record_type = RecordType(record_type)
+        else:
+            self.record_type = get_record_type(dataset[0])
         self.record_cls = record_type_cls_map[self.record_type]
 
     def __getitem__(self, index: int):
         record = self.dataset[index]
         return self.record_cls(**record)
 
     def __len__(self):
         return len(self.dataset)
 
 
+class PrefixFinetuneDataset(FinetuneDataset):
+    def __init__(
+        self,
+        dataset: HfDataset | Sequence[dict],
+        prefix: str,
+        record_type: RecordType | str | None = None,
+    ) -> None:
+        super().__init__(dataset=dataset, record_type=record_type)
+        self.prefix = prefix
+
+    def __getitem__(self, index: int):
+        record = self.dataset[index]
+        match self.record_type:
+            case RecordType.PAIR:
+                record['text'] = self.prefix + record['text']
+            case RecordType.TRIPLET:
+                record['text'] = self.prefix + record['text']
+            case RecordType.SCORED_PAIR:
+                record['sentence1'] = self.prefix + record['sentence1']
+        return self.record_cls(**record)
+
+
 class MediDataset(Dataset):
     def __init__(
         self,
         medi_data_file: str | Path,
         batch_size: int = 32,
         pair_or_triplet: str = 'triplet',
         with_prompt: bool = True,
```

### Comparing `uniem-0.2.0/uniem/model.py` & `uniem-0.2.2/uniem/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 from pathlib import Path
 from typing import ClassVar, Literal, Type, TypeVar, cast
 
-import tqdm
-import torch
 import numpy as np
-from transformers import AutoTokenizer, AutoConfig, AutoModel, PreTrainedModel
+import torch
+import tqdm
+from transformers import AutoConfig, AutoModel, AutoTokenizer, PreTrainedModel  # type: ignore
 
 from uniem.criteria import (
     CoSentLoss,
     PairInBatchNegCoSentLoss,
     PairInBatchNegSigmoidContrastLoss,
     PairInBatchNegSoftmaxContrastLoss,
     TripletInBatchNegCoSentLoss,
@@ -46,15 +46,15 @@
     mask = mask.float()
     return torch.sum(hidden_state * mask.unsqueeze(-1), dim=1) / torch.sum(mask, dim=-1, keepdim=True)
 
 
 def load_hf_pretrained_model(model_name_or_path: str) -> PreTrainedModel:
     config = AutoConfig.from_pretrained(model_name_or_path)
     if config.model_type == 't5':
-        from transformers import T5EncoderModel
+        from transformers import T5EncoderModel  # type: ignore
 
         pretrained_model = T5EncoderModel.from_pretrained(model_name_or_path)
     else:
         pretrained_model = AutoModel.from_pretrained(model_name_or_path)
     return pretrained_model  # type: ignore
 
 
@@ -172,14 +172,16 @@
         else:
             raise ValueError('Can not find uniem pooling strategy in config, Model is not trained by UniEmbedder.')
         embedder_cls = StrategyEmbedderClsMap[PoolingStrategy(strategy_string)]
         return embedder_cls(encoder)
 
 
 class EmbedderForTrain(torch.nn.Module):
+    embedder: Embedder
+
     def __init__(self, embedder: Embedder):
         super().__init__()
         self.embedder = embedder
 
 
 class EmbedderForPairInBatchNegTrain(EmbedderForTrain):
     def __init__(
@@ -228,15 +230,18 @@
                 self.criterion = TripletInBatchNegSigmoidContrastLoss(temperature, add_swap_loss)
             case InBatchNegLossType.softmax:
                 self.criterion = TripletInBatchNegSoftmaxContrastLoss(temperature, add_swap_loss)
             case InBatchNegLossType.cosent:
                 self.criterion = TripletInBatchNegCoSentLoss(temperature, add_swap_loss)
 
     def forward(
-        self, text_ids: torch.Tensor, text_pos_ids: torch.Tensor, text_neg_ids: torch.Tensor
+        self,
+        text_ids: torch.Tensor,
+        text_pos_ids: torch.Tensor,
+        text_neg_ids: torch.Tensor,
     ) -> dict[str, torch.Tensor]:
         text_embeddings = self.embedder(text_ids)
         text_pos_embeddings = self.embedder(text_pos_ids)
         text_neg_embeddings = self.embedder(text_neg_ids)
         loss = self.criterion(text_embeddings, text_pos_embeddings, text_neg_embeddings)
         return {'loss': loss}
 
@@ -250,15 +255,20 @@
     ):
         pretrained_model = load_hf_pretrained_model(model_name_or_path)
         embedder = StrategyEmbedderClsMap[PoolingStrategy(embedding_strategy)](pretrained_model)
         super().__init__(embedder)
         temperature = temperature or 0.05
         self.criterion = CoSentLoss(temperature)
 
-    def forward(self, text_ids: torch.Tensor, text_pair_ids: torch.Tensor, labels: torch.Tensor) -> dict[str, torch.Tensor]:
+    def forward(
+        self,
+        text_ids: torch.Tensor,
+        text_pair_ids: torch.Tensor,
+        labels: torch.Tensor,
+    ) -> dict[str, torch.Tensor]:
         text_embeddings = self.embedder(text_ids)
         text_pos_embeddings = self.embedder(text_pair_ids)
         predict_labels = torch.cosine_similarity(text_embeddings, text_pos_embeddings, dim=-1)
         loss = self.criterion(predict_labels, labels)
         return {'loss': loss, 'predict_labels': predict_labels}
 
 
@@ -283,15 +293,20 @@
         self.max_length = (
             max_length or self.embedder.encoder.config.max_length or self.embedder.encoder.config.max_position_embeddings
         )
 
     def __call__(self, sentences: list[str], batch_size: int = 32):
         return self.encode(sentences, batch_size)
 
-    def encode(self, sentences: list[str], batch_size: int = 32, progress_bar: Literal['auto'] | bool = 'auto'):
+    def encode(
+        self,
+        sentences: list[str],
+        batch_size: int = 32,
+        progress_bar: Literal['auto'] | bool = 'auto',
+    ):
         embeddings: list[np.ndarray] = []
         if progress_bar == 'auto':
             progress_bar = len(sentences) > self.PROGRESS_BAR_THRESHOLD
 
         for batch in tqdm.tqdm(
             generate_batch(sentences, batch_size),
             disable=not progress_bar,
```

### Comparing `uniem-0.2.0/uniem/trainer.py` & `uniem-0.2.2/uniem/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from typing import Any
 
 import torch
-from tqdm.auto import tqdm
 from accelerate import Accelerator
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import LRScheduler
 from torch.utils.data import DataLoader
+from tqdm.auto import tqdm
 
 
 class Trainer:
     def __init__(
         self,
         *,
         model: torch.nn.Module,
@@ -56,23 +56,30 @@
                     if self.lr_scheduler is not None:
                         self.lr_scheduler.step()
                     self.train_loss_tracker.update(loss)
 
                 self.progress_bar.update()
                 self.current_step += 1
                 if batch_index % self.log_interval == 0:
-                    self.log_metrics({'loss': self.train_loss_tracker.loss}, step=self.current_step)
+                    self.log_metrics(
+                        {'loss': self.train_loss_tracker.loss},
+                        step=self.current_step,
+                    )
 
             train_metrics = self.add_prefix({'loss': self.train_loss_tracker.loss}, 'train')
             self.accelerator.log(train_metrics, step=current_epoch)
             self.train_loss_tracker.on_epoch_end()
             self.progress_bar.on_epoch_end()
 
             if self.validation_dataloader:
-                validation_loss = evaluate(self.model, self.validation_dataloader, self.validation_loss_tracker)
+                validation_loss = evaluate(
+                    self.model,
+                    self.validation_dataloader,
+                    self.validation_loss_tracker,
+                )
                 validation_metrics = self.add_prefix({'loss': validation_loss}, 'validation')
                 self.accelerator.log(validation_metrics, step=current_epoch)
 
             if self.save_on_epoch_end:
                 self.accelerator.save_state()
 
             if self.epoch_end_callbacks:
@@ -86,15 +93,19 @@
         self.progress_bar.show_metrics(metrics)
 
     @staticmethod
     def add_prefix(values: dict[str, Any], prefix: str):
         return {f'{prefix}/{k}': v for k, v in values.items()}
 
 
-def evaluate(model: torch.nn.Module, dataloader: DataLoader, loss_tracker: LossTracker | None = None):
+def evaluate(
+    model: torch.nn.Module,
+    dataloader: DataLoader,
+    loss_tracker: LossTracker | None = None,
+):
     model = model.eval()
     loss_tracker = loss_tracker or LossTracker()
     for batch in dataloader:
         with torch.inference_mode():
             batch_output = model(**batch)
             loss_tracker.update(batch_output['loss'])
     loss = loss_tracker.loss
```

### Comparing `uniem-0.2.0/uniem/types.py` & `uniem-0.2.2/uniem/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from dataclasses import dataclass
 from enum import Enum
 from typing import Callable, TypeAlias
 
+from datasets import DatasetDict
 from transformers.tokenization_utils import PreTrainedTokenizer
 from transformers.tokenization_utils_fast import PreTrainedTokenizerFast
 
-from datasets import DatasetDict
-
 Tokenizer: TypeAlias = PreTrainedTokenizer | PreTrainedTokenizerFast
 
 
 class MixedPrecisionType(str, Enum):
     fp16 = 'fp16'
     bf16 = 'bf16'
     no = 'no'
```

