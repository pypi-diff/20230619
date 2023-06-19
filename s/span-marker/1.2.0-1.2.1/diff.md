# Comparing `tmp/span_marker-1.2.0.tar.gz` & `tmp/span_marker-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "span_marker-1.2.0.tar", last modified: Thu Jun 15 19:59:21 2023, max compression
+gzip compressed data, was "span_marker-1.2.1.tar", last modified: Mon Jun 19 14:11:24 2023, max compression
```

## Comparing `span_marker-1.2.0.tar` & `span_marker-1.2.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 19:59:21.172128 span_marker-1.2.0/
--rw-rw-rw-   0        0        0    11558 2023-05-04 23:33:40.000000 span_marker-1.2.0/LICENSE
--rw-rw-rw-   0        0        0    15026 2023-06-15 19:59:21.171128 span_marker-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    14458 2023-06-15 19:51:37.000000 span_marker-1.2.0/README.md
--rw-rw-rw-   0        0        0     2521 2023-06-15 19:58:36.000000 span_marker-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-15 19:59:21.172128 span_marker-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-03-28 09:28:01.000000 span_marker-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:59:21.158129 span_marker-1.2.0/span_marker/
--rw-rw-rw-   0        0        0     1659 2023-06-15 19:56:29.000000 span_marker-1.2.0/span_marker/__init__.py
--rw-rw-rw-   0        0        0     7070 2023-06-15 09:34:01.000000 span_marker-1.2.0/span_marker/configuration.py
--rw-rw-rw-   0        0        0     6630 2023-06-13 22:30:33.000000 span_marker-1.2.0/span_marker/data_collator.py
--rw-rw-rw-   0        0        0     5276 2023-06-15 14:37:15.000000 span_marker-1.2.0/span_marker/evaluation.py
--rw-rw-rw-   0        0        0     5230 2023-05-31 13:34:45.000000 span_marker-1.2.0/span_marker/label_normalizer.py
--rw-rw-rw-   0        0        0     2472 2023-06-13 22:30:43.000000 span_marker-1.2.0/span_marker/model_card.py
--rw-rw-rw-   0        0        0    31490 2023-06-15 10:02:14.000000 span_marker-1.2.0/span_marker/modeling.py
--rw-rw-rw-   0        0        0     2221 2023-06-13 22:30:33.000000 span_marker-1.2.0/span_marker/output.py
--rw-rw-rw-   0        0        0     3914 2023-06-15 15:56:41.000000 span_marker-1.2.0/span_marker/spacy_integration.py
--rw-rw-rw-   0        0        0    11828 2023-06-15 06:57:10.000000 span_marker-1.2.0/span_marker/tokenizer.py
--rw-rw-rw-   0        0        0    21019 2023-06-15 10:02:14.000000 span_marker-1.2.0/span_marker/trainer.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:59:21.167128 span_marker-1.2.0/span_marker.egg-info/
--rw-rw-rw-   0        0        0    15026 2023-06-15 19:59:21.000000 span_marker-1.2.0/span_marker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      606 2023-06-15 19:59:21.000000 span_marker-1.2.0/span_marker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 19:59:21.000000 span_marker-1.2.0/span_marker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      267 2023-06-15 19:59:21.000000 span_marker-1.2.0/span_marker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-15 19:59:21.000000 span_marker-1.2.0/span_marker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-15 19:59:21.170128 span_marker-1.2.0/tests/
--rw-rw-rw-   0        0        0     1645 2023-06-10 13:15:43.000000 span_marker-1.2.0/tests/test_configuration.py
--rw-rw-rw-   0        0        0     1410 2023-06-01 07:33:08.000000 span_marker-1.2.0/tests/test_model_card.py
--rw-rw-rw-   0        0        0     9228 2023-06-15 09:34:01.000000 span_marker-1.2.0/tests/test_modeling.py
--rw-rw-rw-   0        0        0    10372 2023-06-15 09:34:01.000000 span_marker-1.2.0/tests/test_trainer.py
+drwxrwxrwx   0        0        0        0 2023-06-19 14:11:24.682843 span_marker-1.2.1/
+-rw-rw-rw-   0        0        0    11558 2023-05-04 23:33:40.000000 span_marker-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0    15006 2023-06-19 14:11:24.681844 span_marker-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    14438 2023-06-19 14:01:35.000000 span_marker-1.2.1/README.md
+-rw-rw-rw-   0        0        0     2650 2023-06-19 13:46:11.000000 span_marker-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 14:11:24.682843 span_marker-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-06-19 13:47:30.000000 span_marker-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 14:11:24.668761 span_marker-1.2.1/span_marker/
+-rw-rw-rw-   0        0        0     1659 2023-06-19 14:09:48.000000 span_marker-1.2.1/span_marker/__init__.py
+-rw-rw-rw-   0        0        0     7070 2023-06-15 09:34:01.000000 span_marker-1.2.1/span_marker/configuration.py
+-rw-rw-rw-   0        0        0     6630 2023-06-13 22:30:33.000000 span_marker-1.2.1/span_marker/data_collator.py
+-rw-rw-rw-   0        0        0     5276 2023-06-15 14:37:15.000000 span_marker-1.2.1/span_marker/evaluation.py
+-rw-rw-rw-   0        0        0     5230 2023-05-31 13:34:45.000000 span_marker-1.2.1/span_marker/label_normalizer.py
+-rw-rw-rw-   0        0        0     2472 2023-06-13 22:30:43.000000 span_marker-1.2.1/span_marker/model_card.py
+-rw-rw-rw-   0        0        0    31577 2023-06-16 08:01:13.000000 span_marker-1.2.1/span_marker/modeling.py
+-rw-rw-rw-   0        0        0     2221 2023-06-13 22:30:33.000000 span_marker-1.2.1/span_marker/output.py
+-rw-rw-rw-   0        0        0     3914 2023-06-19 13:45:55.000000 span_marker-1.2.1/span_marker/spacy_integration.py
+-rw-rw-rw-   0        0        0    11828 2023-06-19 13:54:52.000000 span_marker-1.2.1/span_marker/tokenizer.py
+-rw-rw-rw-   0        0        0    21019 2023-06-15 10:02:14.000000 span_marker-1.2.1/span_marker/trainer.py
+drwxrwxrwx   0        0        0        0 2023-06-19 14:11:24.678843 span_marker-1.2.1/span_marker.egg-info/
+-rw-rw-rw-   0        0        0    15006 2023-06-19 14:11:24.000000 span_marker-1.2.1/span_marker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-06-19 14:11:24.000000 span_marker-1.2.1/span_marker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 14:11:24.000000 span_marker-1.2.1/span_marker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      267 2023-06-19 14:11:24.000000 span_marker-1.2.1/span_marker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-19 14:11:24.000000 span_marker-1.2.1/span_marker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 14:11:24.681844 span_marker-1.2.1/tests/
+-rw-rw-rw-   0        0        0     1645 2023-06-10 13:15:43.000000 span_marker-1.2.1/tests/test_configuration.py
+-rw-rw-rw-   0        0        0     1410 2023-06-01 07:33:08.000000 span_marker-1.2.1/tests/test_model_card.py
+-rw-rw-rw-   0        0        0     9228 2023-06-15 09:34:01.000000 span_marker-1.2.1/tests/test_modeling.py
+-rw-rw-rw-   0        0        0     1148 2023-06-15 14:47:29.000000 span_marker-1.2.1/tests/test_spacy_integration.py
+-rw-rw-rw-   0        0        0    10372 2023-06-15 09:34:01.000000 span_marker-1.2.1/tests/test_trainer.py
```

### Comparing `span_marker-1.2.0/LICENSE` & `span_marker-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.0/PKG-INFO` & `span_marker-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: span_marker
-Version: 1.2.0
+Version: 1.2.1
 Summary: Named Entity Recognition using Span Markers
 Author: Tom Aarsen
 Maintainer: Tom Aarsen
 Project-URL: Documentation, https://tomaarsen.github.io/SpanMarkerNER
 Project-URL: Repository, https://github.com/tomaarsen/SpanMarkerNER
 Keywords: data-science,natural-language-processing,artificial-intelligence,mlops,nlp,machine-learning,transformers
 Requires-Python: >=3.7
@@ -157,15 +157,14 @@
 ### CoNLL++
 * [`tomaarsen/span-marker-xlm-roberta-large-conllpp-doc-context`](https://huggingface.co/tomaarsen/span-marker-xlm-roberta-large-conllpp-doc-context) was trained in an hour using the `xlm-roberta-large` encoder on the CoNLL++ dataset. Using [document-level context](https://tomaarsen.github.io/SpanMarkerNER/notebooks/document_level_context.html), it reaches a very competitive 0.955 F1. For the best performance, inference should be performed using document-level context ([docs](https://tomaarsen.github.io/SpanMarkerNER/notebooks/document_level_context.html#Inference)).
 
 ## Using pretrained SpanMarker models with spaCy
 All [SpanMarker models on the Hugging Face Hub](https://huggingface.co/models?library=span-marker) can also be easily used in spaCy. It's as simple as including 1 line to add the `span_marker` pipeline. See the Documentation or API Reference for more information.
 ```python
 import spacy
-import span_marker
 
 # Load the spaCy model with the span_marker pipeline component
 nlp = spacy.load("en_core_web_sm")
 nlp.add_pipe("span_marker", config={"model": "tomaarsen/span-marker-roberta-large-ontonotes5"})
 
 # Feed some text through the model to get a spacy Doc
 text = """Cleopatra VII, also known as Cleopatra the Great, was the last active ruler of the \
```

### Comparing `span_marker-1.2.0/README.md` & `span_marker-1.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,14 @@
 ### CoNLL++
 * [`tomaarsen/span-marker-xlm-roberta-large-conllpp-doc-context`](https://huggingface.co/tomaarsen/span-marker-xlm-roberta-large-conllpp-doc-context) was trained in an hour using the `xlm-roberta-large` encoder on the CoNLL++ dataset. Using [document-level context](https://tomaarsen.github.io/SpanMarkerNER/notebooks/document_level_context.html), it reaches a very competitive 0.955 F1. For the best performance, inference should be performed using document-level context ([docs](https://tomaarsen.github.io/SpanMarkerNER/notebooks/document_level_context.html#Inference)).
 
 ## Using pretrained SpanMarker models with spaCy
 All [SpanMarker models on the Hugging Face Hub](https://huggingface.co/models?library=span-marker) can also be easily used in spaCy. It's as simple as including 1 line to add the `span_marker` pipeline. See the Documentation or API Reference for more information.
 ```python
 import spacy
-import span_marker
 
 # Load the spaCy model with the span_marker pipeline component
 nlp = spacy.load("en_core_web_sm")
 nlp.add_pipe("span_marker", config={"model": "tomaarsen/span-marker-roberta-large-ontonotes5"})
 
 # Feed some text through the model to get a spacy Doc
 text = """Cleopatra VII, also known as Cleopatra the Great, was the last active ruler of the \
```

### Comparing `span_marker-1.2.0/pyproject.toml` & `span_marker-1.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -124,7 +124,12 @@
 
 [tool.ruff.per-file-ignores]
 # Ignore imported but unused;
 "__init__.py" = ["F401"]
 
 [tool.black]
 line-length = 120
+
+[tool.poetry.plugins]
+
+[tool.poetry.plugins."spacy_factories"]
+"spacy" = "span_marker.__init__:_spacy_span_marker_factory"
```

### Comparing `span_marker-1.2.0/span_marker/__init__.py` & `span_marker-1.2.1/span_marker/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 
 import logging
 from typing import Optional, Union
 
 import torch
 from transformers import AutoConfig, AutoModel, TrainingArguments
```

### Comparing `span_marker-1.2.0/span_marker/configuration.py` & `span_marker-1.2.1/span_marker/configuration.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.0/span_marker/data_collator.py` & `span_marker-1.2.1/span_marker/data_collator.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.0/span_marker/evaluation.py` & `span_marker-1.2.1/span_marker/evaluation.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.0/span_marker/label_normalizer.py` & `span_marker-1.2.1/span_marker/label_normalizer.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.0/span_marker/model_card.py` & `span_marker-1.2.1/span_marker/model_card.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.0/span_marker/modeling.py` & `span_marker-1.2.1/span_marker/modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     [{'span': 'DB5', 'label': 'product-car', 'score': 0.8675689101219177, 'char_start_index': 52, 'char_end_index': 55},
      {'span': 'Marek', 'label': 'person-other', 'score': 0.9100819230079651, 'char_start_index': 99, 'char_end_index': 104},
      {'span': 'Aston Martin DB7', 'label': 'product-car', 'score': 0.9931442737579346, 'char_start_index': 143, 'char_end_index': 159}]
     """
 
     config_class = SpanMarkerConfig
     base_model_prefix = "encoder"
+    _no_split_modules = []  # To support `load_in_8bit=True`` and `device_map="auto"`
 
     def __init__(self, config: SpanMarkerConfig, encoder: Optional[PreTrainedModel] = None, **kwargs) -> None:
         """Initialize a SpanMarkerModel using configuration.
 
         Do not manually initialize a SpanMarkerModel this way! Use :meth:`~SpanMarkerModel.from_pretrained` instead.
 
         Args:
```

### Comparing `span_marker-1.2.0/span_marker/output.py` & `span_marker-1.2.1/span_marker/output.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.0/span_marker/spacy_integration.py` & `span_marker-1.2.1/span_marker/spacy_integration.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.0/span_marker/tokenizer.py` & `span_marker-1.2.1/span_marker/tokenizer.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.0/span_marker/trainer.py` & `span_marker-1.2.1/span_marker/trainer.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.0/span_marker.egg-info/PKG-INFO` & `span_marker-1.2.1/span_marker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: span-marker
-Version: 1.2.0
+Version: 1.2.1
 Summary: Named Entity Recognition using Span Markers
 Author: Tom Aarsen
 Maintainer: Tom Aarsen
 Project-URL: Documentation, https://tomaarsen.github.io/SpanMarkerNER
 Project-URL: Repository, https://github.com/tomaarsen/SpanMarkerNER
 Keywords: data-science,natural-language-processing,artificial-intelligence,mlops,nlp,machine-learning,transformers
 Requires-Python: >=3.7
@@ -157,15 +157,14 @@
 ### CoNLL++
 * [`tomaarsen/span-marker-xlm-roberta-large-conllpp-doc-context`](https://huggingface.co/tomaarsen/span-marker-xlm-roberta-large-conllpp-doc-context) was trained in an hour using the `xlm-roberta-large` encoder on the CoNLL++ dataset. Using [document-level context](https://tomaarsen.github.io/SpanMarkerNER/notebooks/document_level_context.html), it reaches a very competitive 0.955 F1. For the best performance, inference should be performed using document-level context ([docs](https://tomaarsen.github.io/SpanMarkerNER/notebooks/document_level_context.html#Inference)).
 
 ## Using pretrained SpanMarker models with spaCy
 All [SpanMarker models on the Hugging Face Hub](https://huggingface.co/models?library=span-marker) can also be easily used in spaCy. It's as simple as including 1 line to add the `span_marker` pipeline. See the Documentation or API Reference for more information.
 ```python
 import spacy
-import span_marker
 
 # Load the spaCy model with the span_marker pipeline component
 nlp = spacy.load("en_core_web_sm")
 nlp.add_pipe("span_marker", config={"model": "tomaarsen/span-marker-roberta-large-ontonotes5"})
 
 # Feed some text through the model to get a spacy Doc
 text = """Cleopatra VII, also known as Cleopatra the Great, was the last active ruler of the \
```

### Comparing `span_marker-1.2.0/span_marker.egg-info/SOURCES.txt` & `span_marker-1.2.1/span_marker.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 span_marker.egg-info/SOURCES.txt
 span_marker.egg-info/dependency_links.txt
 span_marker.egg-info/requires.txt
 span_marker.egg-info/top_level.txt
 tests/test_configuration.py
 tests/test_model_card.py
 tests/test_modeling.py
+tests/test_spacy_integration.py
 tests/test_trainer.py
```

### Comparing `span_marker-1.2.0/tests/test_configuration.py` & `span_marker-1.2.1/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.0/tests/test_model_card.py` & `span_marker-1.2.1/tests/test_model_card.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.0/tests/test_modeling.py` & `span_marker-1.2.1/tests/test_modeling.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.0/tests/test_trainer.py` & `span_marker-1.2.1/tests/test_trainer.py`

 * *Files identical despite different names*

