# Comparing `tmp/classy-classification-0.6.4.tar.gz` & `tmp/classy-classification-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classy-classification-0.6.4.tar", max compression
+gzip compressed data, was "classy-classification-0.6.5.tar", max compression
```

## Comparing `classy-classification-0.6.4.tar` & `classy-classification-0.6.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1073 2022-11-01 08:20:25.558101 classy-classification-0.6.4/LICENSE
--rw-r--r--   0        0        0    10731 2023-06-18 12:45:02.602513 classy-classification-0.6.4/README.md
--rw-r--r--   0        0        0     2583 2022-12-30 07:44:33.081954 classy-classification-0.6.4/classy_classification/__init__.py
--rw-r--r--   0        0        0        0 2022-11-01 08:20:25.558372 classy-classification-0.6.4/classy_classification/classifiers/__init__.py
--rw-r--r--   0        0        0    10545 2023-06-18 12:48:16.591005 classy-classification-0.6.4/classy_classification/classifiers/classy_skeleton.py
--rw-r--r--   0        0        0     9186 2023-06-18 14:01:58.082842 classy-classification-0.6.4/classy_classification/classifiers/classy_spacy.py
--rw-r--r--   0        0        0     2274 2023-06-18 12:48:19.711859 classy-classification-0.6.4/classy_classification/classifiers/classy_standalone.py
--rw-r--r--   0        0        0        0 2022-11-01 08:20:25.558915 classy-classification-0.6.4/classy_classification/examples/__init__.py
--rw-r--r--   0        0        0     2324 2023-01-14 09:24:42.022043 classy-classification-0.6.4/classy_classification/examples/data.py
--rw-r--r--   0        0        0      230 2022-12-30 07:21:01.276435 classy-classification-0.6.4/classy_classification/examples/individual_transformer.py
--rw-r--r--   0        0        0      339 2023-03-03 12:03:23.566908 classy-classification-0.6.4/classy_classification/examples/spacy_few_shot_external.py
--rw-r--r--   0        0        0      368 2023-03-03 12:03:22.068037 classy-classification-0.6.4/classy_classification/examples/spacy_internal_embeddings.py
--rw-r--r--   0        0        0      372 2023-03-03 12:03:19.152952 classy-classification-0.6.4/classy_classification/examples/spacy_zero_shot_external.py
--rw-r--r--   0        0        0     2191 2023-06-18 13:56:56.117112 classy-classification-0.6.4/pyproject.toml
--rw-r--r--   0        0        0    12256 1970-01-01 00:00:00.000000 classy-classification-0.6.4/setup.py
--rw-r--r--   0        0        0    12581 1970-01-01 00:00:00.000000 classy-classification-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-11-01 08:20:25.558101 classy-classification-0.6.5/LICENSE
+-rw-r--r--   0        0        0    10736 2023-06-19 12:49:50.792281 classy-classification-0.6.5/README.md
+-rw-r--r--   0        0        0     2591 2023-06-19 12:47:07.008098 classy-classification-0.6.5/classy_classification/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-01 08:20:25.558372 classy-classification-0.6.5/classy_classification/classifiers/__init__.py
+-rw-r--r--   0        0        0    10545 2023-06-18 12:48:16.591005 classy-classification-0.6.5/classy_classification/classifiers/classy_skeleton.py
+-rw-r--r--   0        0        0     9186 2023-06-19 12:49:50.792618 classy-classification-0.6.5/classy_classification/classifiers/classy_spacy.py
+-rw-r--r--   0        0        0     2274 2023-06-18 12:48:19.711859 classy-classification-0.6.5/classy_classification/classifiers/classy_standalone.py
+-rw-r--r--   0        0        0        0 2022-11-01 08:20:25.558915 classy-classification-0.6.5/classy_classification/examples/__init__.py
+-rw-r--r--   0        0        0     2324 2023-01-14 09:24:42.022043 classy-classification-0.6.5/classy_classification/examples/data.py
+-rw-r--r--   0        0        0      230 2022-12-30 07:21:01.276435 classy-classification-0.6.5/classy_classification/examples/individual_transformer.py
+-rw-r--r--   0        0        0      339 2023-03-03 12:03:23.566908 classy-classification-0.6.5/classy_classification/examples/spacy_few_shot_external.py
+-rw-r--r--   0        0        0      368 2023-03-03 12:03:22.068037 classy-classification-0.6.5/classy_classification/examples/spacy_internal_embeddings.py
+-rw-r--r--   0        0        0      372 2023-03-03 12:03:19.152952 classy-classification-0.6.5/classy_classification/examples/spacy_zero_shot_external.py
+-rw-r--r--   0        0        0     2353 2023-06-19 12:51:00.325718 classy-classification-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0    12436 1970-01-01 00:00:00.000000 classy-classification-0.6.5/setup.py
+-rw-r--r--   0        0        0    12590 1970-01-01 00:00:00.000000 classy-classification-0.6.5/PKG-INFO
```

### Comparing `classy-classification-0.6.4/LICENSE` & `classy-classification-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `classy-classification-0.6.4/README.md` & `classy-classification-0.6.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,20 @@
 
 # Install
 ``` pip install classy-classification```
 
 Or, install with faster inference using ONNX.
 
 ``` pip install classy-classification[onnx]```
+## SetFit support
 
+I got a lot of requests for SetFit support, but I decided to create a [separate package](https://github.com/davidberenstein1957/spacy-setfit) for this. Feel free to check it out. ❤️
 ## ONNX issues
 
+
 ### pickling
 
 ONNX does show some issues when pickling the data.
 ### M1
 
 Some [installation issues](https://github.com/onnx/onnx/issues/3129) might occur, which can be fixed by these commands.
 
@@ -28,17 +31,16 @@
 pip3 install onnx --no-use-pep517
 ```
 
 # Quickstart
 ## SpaCy embeddings
 ```python
 import spacy
-import classy_classification
-# or import standalon
-from classy_classification import ClassyClassifier
+# or import standalone
+# from classy_classification import ClassyClassifier
 
 data = {
     "furniture": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa."],
     "kitchen": ["There also exist things like fridges.",
                 "I hope to be getting a new stove today.",
@@ -59,15 +61,14 @@
 # Output:
 #
 # [{"furniture" : 0.21}, {"kitchen": 0.79}]
 ```
 ### Sentence level classification
 ```python
 import spacy
-import classy_classification
 
 data = {
     "furniture": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa."],
     "kitchen": ["There also exist things like fridges.",
                 "I hope to be getting a new stove today.",
@@ -102,15 +103,14 @@
 )
 ```
 ### Multi-label classification
 Sometimes multiple labels are necessary to fully describe the contents of a text. In that case, we want to make use of the **multi-label** implementation, here the sum of label scores is not limited to 1. Just pass the same training data to multiple keys.
 
 ```python
 import spacy
-import classy_classification
 
 data = {
     "furniture": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa.",
                "We have a new dinner table.",
                "There also exist things like fridges.",
@@ -146,15 +146,14 @@
 ### Outlier detection
 Sometimes it is worth to be able to do outlier detection or binary classification. This can either be approached using
 a binary training dataset, however, I have also implemented support for a `OneClassSVM` for [outlier detection using a single label](https://scikit-learn.org/stable/modules/generated/sklearn.svm.OneClassSVM.html). Not that this method does not return probabilities, but that the data is formatted like label-score value pair to ensure uniformity.
 
 Approach 1:
 ```python
 import spacy
-import classy_classification
 
 data_binary = {
     "inlier": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa."],
     "outlier": ["Text about kitchen equipment",
                 "This text is about politics",
@@ -174,15 +173,14 @@
 # Output:
 #
 # [{'inlier': 0.2926672385488411, 'outlier': 0.707332761451159}]
 ```
 Approach 2:
 ```python
 import spacy
-import classy_classification
 
 data_singular = {
     "furniture": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa.",
                "We have a new dinner table."]
 }
@@ -199,15 +197,14 @@
 # Output:
 #
 # [{'furniture': 0, 'not_furniture': 1}]
 ```
 ## Sentence-transfomer embeddings
 ```python
 import spacy
-import classy_classification
 
 data = {
     "furniture": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa."],
     "kitchen": ["There also exist things like fridges.",
                 "I hope to be getting a new stove today.",
@@ -229,15 +226,14 @@
 # Output:
 #
 # [{"furniture": 0.21}, {"kitchen": 0.79}]
 ```
 ## Hugginface zero-shot classifiers
 ```python
 import spacy
-import classy_classification
 
 data = ["furniture", "kitchen"]
 
 nlp = spacy.blank("en")
 nlp.add_pipe(
     "text_categorizer",
     config={
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `classy-classification-0.6.4/classy_classification/__init__.py` & `classy-classification-0.6.5/classy_classification/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         "verbose": False,
     },
 )
 def make_text_categorizer(
     nlp: Language,
     name: str,
     data: Union[dict, list],
-    device: str,
+    device: str = "cpu",
     config: dict = None,
     model: str = None,
     cat_type: str = "few",
     multi_label: bool = False,
     include_doc: bool = True,
     include_sent: bool = False,
     verbose: bool = False,
```

### Comparing `classy-classification-0.6.4/classy_classification/classifiers/classy_skeleton.py` & `classy-classification-0.6.5/classy_classification/classifiers/classy_skeleton.py`

 * *Files identical despite different names*

### Comparing `classy-classification-0.6.4/classy_classification/classifiers/classy_spacy.py` & `classy-classification-0.6.5/classy_classification/classifiers/classy_spacy.py`

 * *Files identical despite different names*

### Comparing `classy-classification-0.6.4/classy_classification/classifiers/classy_standalone.py` & `classy-classification-0.6.5/classy_classification/classifiers/classy_standalone.py`

 * *Files identical despite different names*

### Comparing `classy-classification-0.6.4/classy_classification/examples/data.py` & `classy-classification-0.6.5/classy_classification/examples/data.py`

 * *Files identical despite different names*

### Comparing `classy-classification-0.6.4/pyproject.toml` & `classy-classification-0.6.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "classy-classification"
-version = "0.6.4"
+version = "0.6.5"
 description = "Have you every struggled with needing a Spacy TextCategorizer but didn't have the time to train one from scratch? Classy Classification is the way to go!"
 authors = ["David Berenstein <david.m.berenstein@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/davidberenstein1957/classy-classification"
 repository = "https://github.com/davidberenstein1957/classy-classification"
 documentation = "https://github.com/davidberenstein1957/classy-classification"
@@ -19,28 +19,35 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development"
 ]
+packages = [{include = "classy_classification"}]
+
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 spacy = {extras = ["transformers"], version = "^3.0"}
 sentence-transformers = "^2.0"
 scikit-learn = "^1.0"
 pandas = "^1.4"
 fast-sentence-transformers = { version = "^0.4.1", optional = true }
-optimum = { version = "^1.8", optional = true,  extras = ["onnxruntime"]}
-transformers = {extras = ["torch"], version = "<4.30"}
+optimum = {extras = ["onnxruntime"], version = "^1.8.6"}
+transformers = {extras = ["torch"], version = ">4.20"}
 
 [tool.poetry.extras]
 onnx = ["fast-sentence-transformers", "optimum"]
 
+[tool.poetry.plugins]
+
+[tool.poetry.plugins."spacy_factories"]
+"spacy" = "classy_classification.__init__:make_text_categorizer"
+
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.1"
 flake8 = "^4.0.1"
 black = "^22.3.0"
 flake8-bugbear = "^22.3.23"
 flake8-docstrings = "^1.6.0"
 isort = "^5.10.1"
```

### Comparing `classy-classification-0.6.4/setup.py` & `classy-classification-0.6.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,32 +10,37 @@
 {'': ['*']}
 
 install_requires = \
 ['pandas>=1.4,<2.0',
  'scikit-learn>=1.0,<2.0',
  'sentence-transformers>=2.0,<3.0',
  'spacy[transformers]>=3.0,<4.0',
- 'transformers[torch]<4.30']
+ 'transformers[torch]>4.20']
 
 extras_require = \
-{'onnx': ['fast-sentence-transformers>=0.4.1,<0.5.0',
-          'optimum[onnxruntime]>=1.8,<2.0']}
+{':extra == "onnx"': ['optimum[onnxruntime]>=1.8.6,<2.0.0'],
+ 'onnx': ['fast-sentence-transformers>=0.4.1,<0.5.0']}
+
+entry_points = \
+{'spacy_factories': ['spacy = '
+                     'classy_classification.__init__:make_text_categorizer']}
 
 setup_kwargs = {
     'name': 'classy-classification',
-    'version': '0.6.4',
+    'version': '0.6.5',
     'description': "Have you every struggled with needing a Spacy TextCategorizer but didn't have the time to train one from scratch? Classy Classification is the way to go!",
-    'long_description': '# Classy Classification\nHave you ever struggled with needing a [Spacy TextCategorizer](https://spacy.io/api/textcategorizer) but didn\'t have the time to train one from scratch? Classy Classification is the way to go! For few-shot classification using [sentence-transformers](https://github.com/UKPLab/sentence-transformers) or [spaCy models](https://spacy.io/usage/models), provide a dictionary with labels and examples, or just provide a list of labels for zero shot-classification with [Hugginface zero-shot classifiers](https://huggingface.co/models?pipeline_tag=zero-shot-classification).\n\n[![Current Release Version](https://img.shields.io/github/release/pandora-intelligence/classy-classification.svg?style=flat-square&logo=github)](https://github.com/pandora-intelligence/classy-classification/releases)\n[![pypi Version](https://img.shields.io/pypi/v/classy-classification.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/classy-classification/)\n[![PyPi downloads](https://static.pepy.tech/personalized-badge/classy-classification?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)](https://pypi.org/project/classy-classification/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)\n\n# Install\n``` pip install classy-classification```\n\nOr, install with faster inference using ONNX.\n\n``` pip install classy-classification[onnx]```\n\n## ONNX issues\n\n### pickling\n\nONNX does show some issues when pickling the data.\n### M1\n\nSome [installation issues](https://github.com/onnx/onnx/issues/3129) might occur, which can be fixed by these commands.\n\n```\nbrew install cmake\nbrew install protobuf\npip3 install onnx --no-use-pep517\n```\n\n# Quickstart\n## SpaCy embeddings\n```python\nimport spacy\nimport classy_classification\n# or import standalon\nfrom classy_classification import ClassyClassifier\n\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens."]\n}\n\nnlp = spacy.load("en_core_web_trf")\nnlp.add_pipe(\n    "text_categorizer",\n    config={\n        "data": data,\n        "model": "spacy"\n    }\n)\n\nprint(nlp("I am looking for kitchen appliances.")._.cats)\n\n# Output:\n#\n# [{"furniture" : 0.21}, {"kitchen": 0.79}]\n```\n### Sentence level classification\n```python\nimport spacy\nimport classy_classification\n\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens."]\n}\n\nnlp.add_pipe(\n    "text_categorizer",\n    config={\n        "data": data,\n        "model": "spacy",\n        "include_sent": True\n    }\n)\n\nprint(nlp("I am looking for kitchen appliances. And I love doing so.").sents[0]._.cats)\n\n# Output:\n#\n# [[{"furniture" : 0.21}, {"kitchen": 0.79}]\n```\n### Define random seed and verbosity\n```python\n\nnlp.add_pipe(\n    "text_categorizer",\n    config={\n        "data": data,\n        "verbose": True,\n        "config": {"seed": 42}\n    }\n)\n```\n### Multi-label classification\nSometimes multiple labels are necessary to fully describe the contents of a text. In that case, we want to make use of the **multi-label** implementation, here the sum of label scores is not limited to 1. Just pass the same training data to multiple keys.\n\n```python\nimport spacy\nimport classy_classification\n\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa.",\n               "We have a new dinner table.",\n               "There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens.",\n                "We have a new dinner table."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens.",\n                "We have a new dinner table.",\n                "There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens.",\n                "We have a new dinner table."]\n}\n\nnlp = spacy.load("en_core_web_md")\nnlp.add_pipe(\n    "text_categorizer",\n    config={\n        "data": data,\n        "model": "spacy",\n        "multi_label": True,\n    }\n)\n\nprint(nlp("I am looking for furniture and kitchen equipment.")._.cats)\n\n# Output:\n#\n# [{"furniture": 0.92}, {"kitchen": 0.91}]\n```\n### Outlier detection\nSometimes it is worth to be able to do outlier detection or binary classification. This can either be approached using\na binary training dataset, however, I have also implemented support for a `OneClassSVM` for [outlier detection using a single label](https://scikit-learn.org/stable/modules/generated/sklearn.svm.OneClassSVM.html). Not that this method does not return probabilities, but that the data is formatted like label-score value pair to ensure uniformity.\n\nApproach 1:\n```python\nimport spacy\nimport classy_classification\n\ndata_binary = {\n    "inlier": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "outlier": ["Text about kitchen equipment",\n                "This text is about politics",\n                "Comments about AI and stuff."]\n}\n\nnlp = spacy.load("en_core_web_md")\nnlp.add_pipe(\n    "text_categorizer",\n    config={\n        "data": data_binary,\n    }\n)\n\nprint(nlp("This text is a random text")._.cats)\n\n# Output:\n#\n# [{\'inlier\': 0.2926672385488411, \'outlier\': 0.707332761451159}]\n```\nApproach 2:\n```python\nimport spacy\nimport classy_classification\n\ndata_singular = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa.",\n               "We have a new dinner table."]\n}\nnlp = spacy.load("en_core_web_md")\nnlp.add_pipe(\n    "text_categorizer",\n    config={\n        "data": data_singular,\n    }\n)\n\nprint(nlp("This text is a random text")._.cats)\n\n# Output:\n#\n# [{\'furniture\': 0, \'not_furniture\': 1}]\n```\n## Sentence-transfomer embeddings\n```python\nimport spacy\nimport classy_classification\n\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens."]\n}\n\nnlp = spacy.blank("en")\nnlp.add_pipe(\n    "text_categorizer",\n    config={\n        "data": data,\n        "model": "sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2",\n        "device": "gpu"\n    }\n)\n\nprint(nlp("I am looking for kitchen appliances.")._.cats)\n\n# Output:\n#\n# [{"furniture": 0.21}, {"kitchen": 0.79}]\n```\n## Hugginface zero-shot classifiers\n```python\nimport spacy\nimport classy_classification\n\ndata = ["furniture", "kitchen"]\n\nnlp = spacy.blank("en")\nnlp.add_pipe(\n    "text_categorizer",\n    config={\n        "data": data,\n        "model": "typeform/distilbert-base-uncased-mnli",\n        "cat_type": "zero",\n        "device": "gpu"\n    }\n)\n\nprint(nlp("I am looking for kitchen appliances.")._.cats)\n\n# Output:\n#\n# [{"furniture": 0.21}, {"kitchen": 0.79}]\n```\n# Credits\n## Inspiration Drawn From\n[Huggingface](https://huggingface.co/) does offer some nice models for few/zero-shot classification, but these are not tailored to multi-lingual approaches. Rasa NLU has [a nice approach](https://rasa.com/blog/rasa-nlu-in-depth-part-1-intent-classification/) for this, but its too embedded in their codebase for easy usage outside of Rasa/chatbots. Additionally, it made sense to integrate [sentence-transformers](https://github.com/UKPLab/sentence-transformers) and [Hugginface zero-shot](https://huggingface.co/models?pipeline_tag=zero-shot-classification), instead of default [word embeddings](https://arxiv.org/abs/1301.3781). Finally, I decided to integrate with Spacy, since training a custom [Spacy TextCategorizer](https://spacy.io/api/textcategorizer) seems like a lot of hassle if you want something quick and dirty.\n\n- [Scikit-learn](https://github.com/scikit-learn/scikit-learn)\n- [Rasa NLU](https://github.com/RasaHQ/rasa)\n- [Sentence Transformers](https://github.com/UKPLab/sentence-transformers)\n- [Spacy](https://github.com/explosion/spaCy)\n\n## Or buy me a coffee\n[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/98kf2552674)\n\n\n# Standalone usage without spaCy\n\n```python\n\nfrom classy_classification import ClassyClassifier\n\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens."]\n}\n\nclassifier = ClassyClassifier(data=data)\nclassifier("I am looking for kitchen appliances.")\nclassifier.pipe(["I am looking for kitchen appliances."])\n\n# overwrite training data\nclassifier.set_training_data(data=data)\nclassifier("I am looking for kitchen appliances.")\n\n# overwrite [embedding model](https://www.sbert.net/docs/pretrained_models.html)\nclassifier.set_embedding_model(model="paraphrase-MiniLM-L3-v2")\nclassifier("I am looking for kitchen appliances.")\n\n# overwrite SVC config\nclassifier.set_classification_model(\n    config={\n        "C": [1, 2, 5, 10, 20, 100],\n        "kernel": ["linear"],\n        "max_cross_validation_folds": 5\n    }\n)\nclassifier("I am looking for kitchen appliances.")\n```\n\n## Save and load models\n```python\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens."]\n}\nclassifier = classyClassifier(data=data)\n\nwith open("./classifier.pkl", "wb") as f:\n    pickle.dump(classifier, f)\n\nf = open("./classifier.pkl", "rb")\nclassifier = pickle.load(f)\nclassifier("I am looking for kitchen appliances.")\n```\n',
+    'long_description': '# Classy Classification\nHave you ever struggled with needing a [Spacy TextCategorizer](https://spacy.io/api/textcategorizer) but didn\'t have the time to train one from scratch? Classy Classification is the way to go! For few-shot classification using [sentence-transformers](https://github.com/UKPLab/sentence-transformers) or [spaCy models](https://spacy.io/usage/models), provide a dictionary with labels and examples, or just provide a list of labels for zero shot-classification with [Hugginface zero-shot classifiers](https://huggingface.co/models?pipeline_tag=zero-shot-classification).\n\n[![Current Release Version](https://img.shields.io/github/release/pandora-intelligence/classy-classification.svg?style=flat-square&logo=github)](https://github.com/pandora-intelligence/classy-classification/releases)\n[![pypi Version](https://img.shields.io/pypi/v/classy-classification.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/classy-classification/)\n[![PyPi downloads](https://static.pepy.tech/personalized-badge/classy-classification?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)](https://pypi.org/project/classy-classification/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)\n\n# Install\n``` pip install classy-classification```\n\nOr, install with faster inference using ONNX.\n\n``` pip install classy-classification[onnx]```\n## SetFit support\n\nI got a lot of requests for SetFit support, but I decided to create a [separate package](https://github.com/davidberenstein1957/spacy-setfit) for this. Feel free to check it out. ❤️\n## ONNX issues\n\n\n### pickling\n\nONNX does show some issues when pickling the data.\n### M1\n\nSome [installation issues](https://github.com/onnx/onnx/issues/3129) might occur, which can be fixed by these commands.\n\n```\nbrew install cmake\nbrew install protobuf\npip3 install onnx --no-use-pep517\n```\n\n# Quickstart\n## SpaCy embeddings\n```python\nimport spacy\n# or import standalone\n# from classy_classification import ClassyClassifier\n\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens."]\n}\n\nnlp = spacy.load("en_core_web_trf")\nnlp.add_pipe(\n    "text_categorizer",\n    config={\n        "data": data,\n        "model": "spacy"\n    }\n)\n\nprint(nlp("I am looking for kitchen appliances.")._.cats)\n\n# Output:\n#\n# [{"furniture" : 0.21}, {"kitchen": 0.79}]\n```\n### Sentence level classification\n```python\nimport spacy\n\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens."]\n}\n\nnlp.add_pipe(\n    "text_categorizer",\n    config={\n        "data": data,\n        "model": "spacy",\n        "include_sent": True\n    }\n)\n\nprint(nlp("I am looking for kitchen appliances. And I love doing so.").sents[0]._.cats)\n\n# Output:\n#\n# [[{"furniture" : 0.21}, {"kitchen": 0.79}]\n```\n### Define random seed and verbosity\n```python\n\nnlp.add_pipe(\n    "text_categorizer",\n    config={\n        "data": data,\n        "verbose": True,\n        "config": {"seed": 42}\n    }\n)\n```\n### Multi-label classification\nSometimes multiple labels are necessary to fully describe the contents of a text. In that case, we want to make use of the **multi-label** implementation, here the sum of label scores is not limited to 1. Just pass the same training data to multiple keys.\n\n```python\nimport spacy\n\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa.",\n               "We have a new dinner table.",\n               "There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens.",\n                "We have a new dinner table."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens.",\n                "We have a new dinner table.",\n                "There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens.",\n                "We have a new dinner table."]\n}\n\nnlp = spacy.load("en_core_web_md")\nnlp.add_pipe(\n    "text_categorizer",\n    config={\n        "data": data,\n        "model": "spacy",\n        "multi_label": True,\n    }\n)\n\nprint(nlp("I am looking for furniture and kitchen equipment.")._.cats)\n\n# Output:\n#\n# [{"furniture": 0.92}, {"kitchen": 0.91}]\n```\n### Outlier detection\nSometimes it is worth to be able to do outlier detection or binary classification. This can either be approached using\na binary training dataset, however, I have also implemented support for a `OneClassSVM` for [outlier detection using a single label](https://scikit-learn.org/stable/modules/generated/sklearn.svm.OneClassSVM.html). Not that this method does not return probabilities, but that the data is formatted like label-score value pair to ensure uniformity.\n\nApproach 1:\n```python\nimport spacy\n\ndata_binary = {\n    "inlier": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "outlier": ["Text about kitchen equipment",\n                "This text is about politics",\n                "Comments about AI and stuff."]\n}\n\nnlp = spacy.load("en_core_web_md")\nnlp.add_pipe(\n    "text_categorizer",\n    config={\n        "data": data_binary,\n    }\n)\n\nprint(nlp("This text is a random text")._.cats)\n\n# Output:\n#\n# [{\'inlier\': 0.2926672385488411, \'outlier\': 0.707332761451159}]\n```\nApproach 2:\n```python\nimport spacy\n\ndata_singular = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa.",\n               "We have a new dinner table."]\n}\nnlp = spacy.load("en_core_web_md")\nnlp.add_pipe(\n    "text_categorizer",\n    config={\n        "data": data_singular,\n    }\n)\n\nprint(nlp("This text is a random text")._.cats)\n\n# Output:\n#\n# [{\'furniture\': 0, \'not_furniture\': 1}]\n```\n## Sentence-transfomer embeddings\n```python\nimport spacy\n\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens."]\n}\n\nnlp = spacy.blank("en")\nnlp.add_pipe(\n    "text_categorizer",\n    config={\n        "data": data,\n        "model": "sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2",\n        "device": "gpu"\n    }\n)\n\nprint(nlp("I am looking for kitchen appliances.")._.cats)\n\n# Output:\n#\n# [{"furniture": 0.21}, {"kitchen": 0.79}]\n```\n## Hugginface zero-shot classifiers\n```python\nimport spacy\n\ndata = ["furniture", "kitchen"]\n\nnlp = spacy.blank("en")\nnlp.add_pipe(\n    "text_categorizer",\n    config={\n        "data": data,\n        "model": "typeform/distilbert-base-uncased-mnli",\n        "cat_type": "zero",\n        "device": "gpu"\n    }\n)\n\nprint(nlp("I am looking for kitchen appliances.")._.cats)\n\n# Output:\n#\n# [{"furniture": 0.21}, {"kitchen": 0.79}]\n```\n# Credits\n## Inspiration Drawn From\n[Huggingface](https://huggingface.co/) does offer some nice models for few/zero-shot classification, but these are not tailored to multi-lingual approaches. Rasa NLU has [a nice approach](https://rasa.com/blog/rasa-nlu-in-depth-part-1-intent-classification/) for this, but its too embedded in their codebase for easy usage outside of Rasa/chatbots. Additionally, it made sense to integrate [sentence-transformers](https://github.com/UKPLab/sentence-transformers) and [Hugginface zero-shot](https://huggingface.co/models?pipeline_tag=zero-shot-classification), instead of default [word embeddings](https://arxiv.org/abs/1301.3781). Finally, I decided to integrate with Spacy, since training a custom [Spacy TextCategorizer](https://spacy.io/api/textcategorizer) seems like a lot of hassle if you want something quick and dirty.\n\n- [Scikit-learn](https://github.com/scikit-learn/scikit-learn)\n- [Rasa NLU](https://github.com/RasaHQ/rasa)\n- [Sentence Transformers](https://github.com/UKPLab/sentence-transformers)\n- [Spacy](https://github.com/explosion/spaCy)\n\n## Or buy me a coffee\n[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/98kf2552674)\n\n\n# Standalone usage without spaCy\n\n```python\n\nfrom classy_classification import ClassyClassifier\n\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens."]\n}\n\nclassifier = ClassyClassifier(data=data)\nclassifier("I am looking for kitchen appliances.")\nclassifier.pipe(["I am looking for kitchen appliances."])\n\n# overwrite training data\nclassifier.set_training_data(data=data)\nclassifier("I am looking for kitchen appliances.")\n\n# overwrite [embedding model](https://www.sbert.net/docs/pretrained_models.html)\nclassifier.set_embedding_model(model="paraphrase-MiniLM-L3-v2")\nclassifier("I am looking for kitchen appliances.")\n\n# overwrite SVC config\nclassifier.set_classification_model(\n    config={\n        "C": [1, 2, 5, 10, 20, 100],\n        "kernel": ["linear"],\n        "max_cross_validation_folds": 5\n    }\n)\nclassifier("I am looking for kitchen appliances.")\n```\n\n## Save and load models\n```python\ndata = {\n    "furniture": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "kitchen": ["There also exist things like fridges.",\n                "I hope to be getting a new stove today.",\n                "Do you also have some ovens."]\n}\nclassifier = classyClassifier(data=data)\n\nwith open("./classifier.pkl", "wb") as f:\n    pickle.dump(classifier, f)\n\nf = open("./classifier.pkl", "rb")\nclassifier = pickle.load(f)\nclassifier("I am looking for kitchen appliances.")\n```\n',
     'author': 'David Berenstein',
     'author_email': 'david.m.berenstein@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/davidberenstein1957/classy-classification',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
+    'entry_points': entry_points,
     'python_requires': '>=3.8,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `classy-classification-0.6.4/PKG-INFO` & `classy-classification-0.6.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classy-classification
-Version: 0.6.4
+Version: 0.6.5
 Summary: Have you every struggled with needing a Spacy TextCategorizer but didn't have the time to train one from scratch? Classy Classification is the way to go!
 Home-page: https://github.com/davidberenstein1957/classy-classification
 License: MIT
 Keywords: spacy,rasa,few-shot classification,nlu,sentence-transformers
 Author: David Berenstein
 Author-email: david.m.berenstein@gmail.com
 Requires-Python: >=3.8,<3.12
@@ -22,20 +22,20 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Provides-Extra: onnx
 Requires-Dist: fast-sentence-transformers (>=0.4.1,<0.5.0); extra == "onnx"
-Requires-Dist: optimum[onnxruntime] (>=1.8,<2.0); extra == "onnx"
+Requires-Dist: optimum[onnxruntime] (>=1.8.6,<2.0.0); extra == "onnx"
 Requires-Dist: pandas (>=1.4,<2.0)
 Requires-Dist: scikit-learn (>=1.0,<2.0)
 Requires-Dist: sentence-transformers (>=2.0,<3.0)
 Requires-Dist: spacy[transformers] (>=3.0,<4.0)
-Requires-Dist: transformers[torch] (<4.30)
+Requires-Dist: transformers[torch] (>4.20)
 Project-URL: Documentation, https://github.com/davidberenstein1957/classy-classification
 Project-URL: Repository, https://github.com/davidberenstein1957/classy-classification
 Description-Content-Type: text/markdown
 
 # Classy Classification
 Have you ever struggled with needing a [Spacy TextCategorizer](https://spacy.io/api/textcategorizer) but didn't have the time to train one from scratch? Classy Classification is the way to go! For few-shot classification using [sentence-transformers](https://github.com/UKPLab/sentence-transformers) or [spaCy models](https://spacy.io/usage/models), provide a dictionary with labels and examples, or just provide a list of labels for zero shot-classification with [Hugginface zero-shot classifiers](https://huggingface.co/models?pipeline_tag=zero-shot-classification).
 
@@ -46,17 +46,20 @@
 
 # Install
 ``` pip install classy-classification```
 
 Or, install with faster inference using ONNX.
 
 ``` pip install classy-classification[onnx]```
+## SetFit support
 
+I got a lot of requests for SetFit support, but I decided to create a [separate package](https://github.com/davidberenstein1957/spacy-setfit) for this. Feel free to check it out. ❤️
 ## ONNX issues
 
+
 ### pickling
 
 ONNX does show some issues when pickling the data.
 ### M1
 
 Some [installation issues](https://github.com/onnx/onnx/issues/3129) might occur, which can be fixed by these commands.
 
@@ -66,17 +69,16 @@
 pip3 install onnx --no-use-pep517
 ```
 
 # Quickstart
 ## SpaCy embeddings
 ```python
 import spacy
-import classy_classification
-# or import standalon
-from classy_classification import ClassyClassifier
+# or import standalone
+# from classy_classification import ClassyClassifier
 
 data = {
     "furniture": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa."],
     "kitchen": ["There also exist things like fridges.",
                 "I hope to be getting a new stove today.",
@@ -97,15 +99,14 @@
 # Output:
 #
 # [{"furniture" : 0.21}, {"kitchen": 0.79}]
 ```
 ### Sentence level classification
 ```python
 import spacy
-import classy_classification
 
 data = {
     "furniture": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa."],
     "kitchen": ["There also exist things like fridges.",
                 "I hope to be getting a new stove today.",
@@ -140,15 +141,14 @@
 )
 ```
 ### Multi-label classification
 Sometimes multiple labels are necessary to fully describe the contents of a text. In that case, we want to make use of the **multi-label** implementation, here the sum of label scores is not limited to 1. Just pass the same training data to multiple keys.
 
 ```python
 import spacy
-import classy_classification
 
 data = {
     "furniture": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa.",
                "We have a new dinner table.",
                "There also exist things like fridges.",
@@ -184,15 +184,14 @@
 ### Outlier detection
 Sometimes it is worth to be able to do outlier detection or binary classification. This can either be approached using
 a binary training dataset, however, I have also implemented support for a `OneClassSVM` for [outlier detection using a single label](https://scikit-learn.org/stable/modules/generated/sklearn.svm.OneClassSVM.html). Not that this method does not return probabilities, but that the data is formatted like label-score value pair to ensure uniformity.
 
 Approach 1:
 ```python
 import spacy
-import classy_classification
 
 data_binary = {
     "inlier": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa."],
     "outlier": ["Text about kitchen equipment",
                 "This text is about politics",
@@ -212,15 +211,14 @@
 # Output:
 #
 # [{'inlier': 0.2926672385488411, 'outlier': 0.707332761451159}]
 ```
 Approach 2:
 ```python
 import spacy
-import classy_classification
 
 data_singular = {
     "furniture": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa.",
                "We have a new dinner table."]
 }
@@ -237,15 +235,14 @@
 # Output:
 #
 # [{'furniture': 0, 'not_furniture': 1}]
 ```
 ## Sentence-transfomer embeddings
 ```python
 import spacy
-import classy_classification
 
 data = {
     "furniture": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa."],
     "kitchen": ["There also exist things like fridges.",
                 "I hope to be getting a new stove today.",
@@ -267,15 +264,14 @@
 # Output:
 #
 # [{"furniture": 0.21}, {"kitchen": 0.79}]
 ```
 ## Hugginface zero-shot classifiers
 ```python
 import spacy
-import classy_classification
 
 data = ["furniture", "kitchen"]
 
 nlp = spacy.blank("en")
 nlp.add_pipe(
     "text_categorizer",
     config={
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

