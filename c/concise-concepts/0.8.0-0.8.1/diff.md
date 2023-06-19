# Comparing `tmp/concise-concepts-0.8.0.tar.gz` & `tmp/concise-concepts-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "concise-concepts-0.8.0.tar", max compression
+gzip compressed data, was "concise-concepts-0.8.1.tar", max compression
```

## Comparing `concise-concepts-0.8.0.tar` & `concise-concepts-0.8.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1077 2022-11-10 17:12:54.786691 concise-concepts-0.8.0/LICENSE
--rw-r--r--   0        0        0     7853 2023-01-12 23:06:09.963712 concise-concepts-0.8.0/README.md
--rw-r--r--   0        0        0     1715 2023-01-12 19:01:33.030058 concise-concepts-0.8.0/concise_concepts/__init__.py
--rw-r--r--   0        0        0    25647 2023-01-13 06:47:31.392336 concise-concepts-0.8.0/concise_concepts/conceptualizer/Conceptualizer.py
--rw-r--r--   0        0        0       97 2022-11-10 17:12:54.787446 concise-concepts-0.8.0/concise_concepts/conceptualizer/__init__.py
--rw-r--r--   0        0        0        0 2022-11-10 17:12:54.787537 concise-concepts-0.8.0/concise_concepts/examples/__init__.py
--rw-r--r--   0        0        0      759 2023-01-12 21:06:28.921251 concise-concepts-0.8.0/concise_concepts/examples/data.py
--rw-r--r--   0        0        0      862 2022-11-10 17:12:54.787806 concise-concepts-0.8.0/concise_concepts/examples/example_gensim_custom_model.py
--rw-r--r--   0        0        0      405 2022-11-10 17:12:54.787927 concise-concepts-0.8.0/concise_concepts/examples/example_gensim_custom_path.py
--rw-r--r--   0        0        0      316 2022-11-10 17:12:54.787997 concise-concepts-0.8.0/concise_concepts/examples/example_gensim_default.py
--rw-r--r--   0        0        0      268 2022-11-10 17:12:54.788060 concise-concepts-0.8.0/concise_concepts/examples/example_spacy.py
--rw-r--r--   0        0        0     1642 2023-01-13 06:48:34.174281 concise-concepts-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     9043 1970-01-01 00:00:00.000000 concise-concepts-0.8.0/setup.py
--rw-r--r--   0        0        0     9371 1970-01-01 00:00:00.000000 concise-concepts-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2022-11-10 17:12:54.786691 concise-concepts-0.8.1/LICENSE
+-rw-r--r--   0        0        0     8005 2023-06-19 12:56:52.268959 concise-concepts-0.8.1/README.md
+-rw-r--r--   0        0        0     1715 2023-01-12 19:01:33.030058 concise-concepts-0.8.1/concise_concepts/__init__.py
+-rw-r--r--   0        0        0    25645 2023-06-19 12:56:52.269790 concise-concepts-0.8.1/concise_concepts/conceptualizer/Conceptualizer.py
+-rw-r--r--   0        0        0       97 2022-11-10 17:12:54.787446 concise-concepts-0.8.1/concise_concepts/conceptualizer/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-10 17:12:54.787537 concise-concepts-0.8.1/concise_concepts/examples/__init__.py
+-rw-r--r--   0        0        0      759 2023-01-12 21:06:28.921251 concise-concepts-0.8.1/concise_concepts/examples/data.py
+-rw-r--r--   0        0        0      862 2022-11-10 17:12:54.787806 concise-concepts-0.8.1/concise_concepts/examples/example_gensim_custom_model.py
+-rw-r--r--   0        0        0      405 2022-11-10 17:12:54.787927 concise-concepts-0.8.1/concise_concepts/examples/example_gensim_custom_path.py
+-rw-r--r--   0        0        0      316 2022-11-10 17:12:54.787997 concise-concepts-0.8.1/concise_concepts/examples/example_gensim_default.py
+-rw-r--r--   0        0        0      268 2022-11-10 17:12:54.788060 concise-concepts-0.8.1/concise_concepts/examples/example_spacy.py
+-rw-r--r--   0        0        0     1810 2023-06-19 12:56:15.322867 concise-concepts-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     9337 1970-01-01 00:00:00.000000 concise-concepts-0.8.1/setup.py
+-rw-r--r--   0        0        0     9523 1970-01-01 00:00:00.000000 concise-concepts-0.8.1/PKG-INFO
```

### Comparing `concise-concepts-0.8.0/LICENSE` & `concise-concepts-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `concise-concepts-0.8.0/README.md` & `concise-concepts-0.8.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -40,35 +40,36 @@
 from spacy import displacy
 
 import concise_concepts
 
 data = {
     "fruit": ["apple", "pear", "orange"],
     "vegetable": ["broccoli", "spinach", "tomato"],
-    "meat": ["beef", "pork", "fish", "lamb"],
+    "meat": ['beef', 'pork', 'turkey', 'duck']
 }
 
 text = """
     Heat the oil in a large pan and add the Onion, celery and carrots.
     Then, cook over a medium–low heat for 10 minutes, or until softened.
     Add the courgette, garlic, red peppers and oregano and cook for 2–3 minutes.
     Later, add some oranges and chickens. """
 
-nlp = spacy.load("en_core_web_lg", disable=["ner"])
+nlp = spacy.load("en_core_web_md", disable=["ner"])
 
 nlp.add_pipe(
     "concise_concepts",
     config={
         "data": data,
         "ent_score": True,  # Entity Scoring section
         "verbose": True,
         "exclude_pos": ["VERB", "AUX"],
         "exclude_dep": ["DOBJ", "PCOMP"],
         "include_compound_words": False,
         "json_path": "./fruitful_patterns.json",
+        "topn": (100,500,300)
     },
 )
 doc = nlp(text)
 
 options = {
     "colors": {"fruit": "darkorange", "vegetable": "limegreen", "meat": "salmon"},
     "ents": ["fruit", "vegetable", "meat"],
@@ -185,15 +186,15 @@
 # output
 #
 # [('Sony', 'ORG', 0.5207586), ('Japan', 'GPE', 0.7371268)]
 ```
 
 ## Custom Embedding Models
 
-- `model_path`: Use `sense2vec.Sense2Vec`, `gensim.Word2vec` `gensim.FastText`, or `gensim.KeyedVectors` model from the [pre-trained gensim](https://radimrehurek.com/gensim/downloader.html) library or a custom model path.
+- `model_path`: Use custom `sense2vec.Sense2Vec`, `gensim.Word2vec` `gensim.FastText`, or `gensim.KeyedVectors`, or a pretrained model from [gensim](https://radimrehurek.com/gensim/downloader.html) library or a custom model path. For using a `sense2vec.Sense2Vec` take a look [here](https://github.com/explosion/sense2vec#pretrained-vectors).
 - `model`: within [standalone usage](#standalone), it is possible to pass these models directly.
 
 ```python
 data = {
     "fruit": ["apple", "pear", "orange"],
     "vegetable": ["broccoli", "spinach", "tomato"],
     "meat": ["beef", "pork", "fish", "lamb"]
```

### Comparing `concise-concepts-0.8.0/concise_concepts/__init__.py` & `concise-concepts-0.8.1/concise_concepts/__init__.py`

 * *Files identical despite different names*

### Comparing `concise-concepts-0.8.0/concise_concepts/conceptualizer/Conceptualizer.py` & `concise-concepts-0.8.1/concise_concepts/conceptualizer/Conceptualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         :param nlp: The spaCy model to use.
         :type nlp: Language
         :param name: The name of the entity.
         :type name: str
         :param data: A dictionary of the words you want to match. The keys are the classes you want to match,
             and the values are the words you want to expand over.
         :type data: dict
-        :param topn(): The number of words to be returned for each class.
+        :param topn: The number of words to be returned for each class.
         :type topn: list
         :param model_path: The path to the model you want to use. If you don't have a model, you can use the spaCy one.
         :param word_delimiter: The delimiter used to separate words in model the dictionary, defaults to _ (optional)
         :param ent_score: If True, the extension "ent_score" will be added to the Span object. This will be the score of
             the entity, defaults to False (optional)
         :param exclude_pos: A list of POS tags to exclude from the rule based match
         :param exclude_dep: list of dependencies to exclude from the rule based match
```

### Comparing `concise-concepts-0.8.0/concise_concepts/examples/data.py` & `concise-concepts-0.8.1/concise_concepts/examples/data.py`

 * *Files identical despite different names*

### Comparing `concise-concepts-0.8.0/concise_concepts/examples/example_gensim_custom_model.py` & `concise-concepts-0.8.1/concise_concepts/examples/example_gensim_custom_model.py`

 * *Files identical despite different names*

### Comparing `concise-concepts-0.8.0/pyproject.toml` & `concise-concepts-0.8.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "concise-concepts"
-version = "0.8.0"
+version = "0.8.1"
 description = "This repository contains an easy and intuitive approach to few-shot NER using most similar expansion over spaCy embeddings. Now with entity confidence scores!"
 authors = ["David Berenstein <david.m.berenstein@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pandora-intelligence/concise-concepts"
 repository = "https://github.com/pandora-intelligence/concise-concepts"
 documentation = "https://github.com/pandora-intelligence/concise-concepts"
@@ -17,23 +17,29 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development"
 ]
+packages = [{include = "concise_concepts"}]
+
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 spacy = "^3"
 scipy = "^1.7"
 gensim = "^4"
 spaczz = "^0.5.4"
 sense2vec = "^2.0.1"
 
+[tool.poetry.plugins]
+
+[tool.poetry.plugins."spacy_factories"]
+"spacy" = "concise_concepts.__init__:make_concise_concepts"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22"
 flake8 = "^5"
 pytest = "^7.1"
 pre-commit = "^2.20"
 pep8-naming = "^0.13"
```

### Comparing `concise-concepts-0.8.0/setup.py` & `concise-concepts-0.8.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,25 +12,29 @@
 install_requires = \
 ['gensim>=4,<5',
  'scipy>=1.7,<2.0',
  'sense2vec>=2.0.1,<3.0.0',
  'spacy>=3,<4',
  'spaczz>=0.5.4,<0.6.0']
 
+entry_points = \
+{'spacy_factories': ['spacy = concise_concepts.__init__:make_concise_concepts']}
+
 setup_kwargs = {
     'name': 'concise-concepts',
-    'version': '0.8.0',
+    'version': '0.8.1',
     'description': 'This repository contains an easy and intuitive approach to few-shot NER using most similar expansion over spaCy embeddings. Now with entity confidence scores!',
-    'long_description': '# Concise Concepts\nWhen wanting to apply NER to concise concepts, it is really easy to come up with examples, but pretty difficult to train an entire pipeline. Concise Concepts uses few-shot NER based on word embedding similarity to get you going\nwith easy! Now with entity scoring!\n\n\n[![Python package](https://github.com/Pandora-Intelligence/concise-concepts/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/Pandora-Intelligence/concise-concepts/actions/workflows/python-package.yml)\n[![Current Release Version](https://img.shields.io/github/release/pandora-intelligence/concise-concepts.svg?style=flat-square&logo=github)](https://github.com/pandora-intelligence/concise-concepts/releases)\n[![pypi Version](https://img.shields.io/pypi/v/concise-concepts.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/concise-concepts/)\n[![PyPi downloads](https://static.pepy.tech/personalized-badge/concise-concepts?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)](https://pypi.org/project/concise-concepts/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)\n\n\n## Usage\nThis library defines matching patterns based on the most similar words found in each group, which are used to fill a [spaCy EntityRuler](https://spacy.io/api/entityruler). To better understand the rule definition, I recommend playing around with the [spaCy Rule-based Matcher Explorer](https://demos.explosion.ai/matcher).\n\n### Tutorials\n- [TechVizTheDataScienceGuy](https://www.youtube.com/c/TechVizTheDataScienceGuy) created a [nice tutorial](https://prakhar-mishra.medium.com/few-shot-named-entity-recognition-in-natural-language-processing-92d31f0d1143) on how to use it.\n\n- [I](https://www.linkedin.com/in/david-berenstein-1bab11105/) created a [tutorial](https://www.rubrix.ml/blog/concise-concepts-rubrix/) in collaboration with Rubrix.\n\nThe section [Matching Pattern Rules](#matching-pattern-rules) expands on the construction, analysis and customization of these matching patterns.\n\n\n# Install\n\n```\npip install concise-concepts\n```\n\n# Quickstart\n\nTake a look at the [configuration section](#configuration) for more info.\n\n## Spacy Pipeline Component\n\nNote that, [custom embedding models](#custom-embedding-models) are passed via `model_path`.\n\n```python\nimport spacy\nfrom spacy import displacy\n\nimport concise_concepts\n\ndata = {\n    "fruit": ["apple", "pear", "orange"],\n    "vegetable": ["broccoli", "spinach", "tomato"],\n    "meat": ["beef", "pork", "fish", "lamb"],\n}\n\ntext = """\n    Heat the oil in a large pan and add the Onion, celery and carrots.\n    Then, cook over a medium–low heat for 10 minutes, or until softened.\n    Add the courgette, garlic, red peppers and oregano and cook for 2–3 minutes.\n    Later, add some oranges and chickens. """\n\nnlp = spacy.load("en_core_web_lg", disable=["ner"])\n\nnlp.add_pipe(\n    "concise_concepts",\n    config={\n        "data": data,\n        "ent_score": True,  # Entity Scoring section\n        "verbose": True,\n        "exclude_pos": ["VERB", "AUX"],\n        "exclude_dep": ["DOBJ", "PCOMP"],\n        "include_compound_words": False,\n        "json_path": "./fruitful_patterns.json",\n    },\n)\ndoc = nlp(text)\n\noptions = {\n    "colors": {"fruit": "darkorange", "vegetable": "limegreen", "meat": "salmon"},\n    "ents": ["fruit", "vegetable", "meat"],\n}\n\nents = doc.ents\nfor ent in ents:\n    new_label = f"{ent.label_} ({ent._.ent_score:.0%})"\n    options["colors"][new_label] = options["colors"].get(ent.label_.lower(), None)\n    options["ents"].append(new_label)\n    ent.label_ = new_label\ndoc.ents = ents\n\ndisplacy.render(doc, style="ent", options=options)\n```\n![](https://raw.githubusercontent.com/Pandora-Intelligence/concise-concepts/master/img/example.png)\n\n## Standalone\n\nThis might be useful when iterating over few_shot training data when not wanting to reload larger models continuously.\nNote that, [custom embedding models](#custom-embedding-models) are passed via `model`.\n\n```python\nimport gensim\nimport spacy\n\nfrom concise_concepts import Conceptualizer\n\nmodel = gensim.downloader.load("fasttext-wiki-news-subwords-300")\nnlp = spacy.load("en_core_web_sm")\ndata = {\n    "disease": ["cancer", "diabetes", "heart disease", "influenza", "pneumonia"],\n    "symptom": ["headache", "fever", "cough", "nausea", "vomiting", "diarrhea"],\n}\nconceptualizer = Conceptualizer(nlp, data, model)\nconceptualizer.nlp("I have a headache and a fever.").ents\n\ndata = {\n    "disease": ["cancer", "diabetes"],\n    "symptom": ["headache", "fever"],\n}\nconceptualizer = Conceptualizer(nlp, data, model)\nconceptualizer.nlp("I have a headache and a fever.").ents\n```\n\n# Configuration\n## Matching Pattern Rules\nA general introduction about the usage of matching patterns in the [usage section](#usage).\n### Customizing Matching Pattern Rules\nEven though the baseline parameters provide a decent result, the construction of these matching rules can be customized via the config passed to the spaCy pipeline.\n\n - `exclude_pos`: A list of POS tags to be excluded from the rule-based match.\n - `exclude_dep`: A list of dependencies to be excluded from the rule-based match.\n - `include_compound_words`:  If True, it will include compound words in the entity. For example, if the entity is "New York", it will also include "New York City" as an entity.\n - `case_sensitive`: Whether to match the case of the words in the text.\n\n\n### Analyze Matching Pattern Rules\nTo motivate actually looking at the data and support interpretability, the matching patterns that have been generated are stored as `./main_patterns.json`. This behavior can be changed by using the `json_path` variable via the config passed to the spaCy pipeline.\n\n\n## Fuzzy matching using `spaczz`\n\n - `fuzzy`: A boolean value that determines whether to use fuzzy matching\n\n```python\ndata = {\n    "fruit": ["apple", "pear", "orange"],\n    "vegetable": ["broccoli", "spinach", "tomato"],\n    "meat": ["beef", "pork", "fish", "lamb"]\n}\n\nnlp.add_pipe("concise_concepts", config={"data": data, "fuzzy": True})\n```\n\n## Most Similar Word Expansion\n\n- `topn`: Use a specific number of words to expand over.\n\n```python\ndata = {\n    "fruit": ["apple", "pear", "orange"],\n    "vegetable": ["broccoli", "spinach", "tomato"],\n    "meat": ["beef", "pork", "fish", "lamb"]\n}\n\ntopn = [50, 50, 150]\n\nassert len(topn) == len\n\nnlp.add_pipe("concise_concepts", config={"data": data, "topn": topn})\n```\n\n## Entity Scoring\n\n- `ent_score`: Use embedding based word similarity to score entities against their groups\n\n```python\nimport spacy\nimport concise_concepts\n\ndata = {\n    "ORG": ["Google", "Apple", "Amazon"],\n    "GPE": ["Netherlands", "France", "China"],\n}\n\ntext = """Sony was founded in Japan."""\n\nnlp = spacy.load("en_core_web_lg")\nnlp.add_pipe("concise_concepts", config={"data": data, "ent_score": True, "case_sensitive": True})\ndoc = nlp(text)\n\nprint([(ent.text, ent.label_, ent._.ent_score) for ent in doc.ents])\n# output\n#\n# [(\'Sony\', \'ORG\', 0.5207586), (\'Japan\', \'GPE\', 0.7371268)]\n```\n\n## Custom Embedding Models\n\n- `model_path`: Use `sense2vec.Sense2Vec`, `gensim.Word2vec` `gensim.FastText`, or `gensim.KeyedVectors` model from the [pre-trained gensim](https://radimrehurek.com/gensim/downloader.html) library or a custom model path.\n- `model`: within [standalone usage](#standalone), it is possible to pass these models directly.\n\n```python\ndata = {\n    "fruit": ["apple", "pear", "orange"],\n    "vegetable": ["broccoli", "spinach", "tomato"],\n    "meat": ["beef", "pork", "fish", "lamb"]\n}\n\n# model from https://radimrehurek.com/gensim/downloader.html or path to local file\nmodel_path = "glove-wiki-gigaword-300"\n\nnlp.add_pipe("concise_concepts", config={"data": data, "model_path": model_path})\n````\n',
+    'long_description': '# Concise Concepts\nWhen wanting to apply NER to concise concepts, it is really easy to come up with examples, but pretty difficult to train an entire pipeline. Concise Concepts uses few-shot NER based on word embedding similarity to get you going\nwith easy! Now with entity scoring!\n\n\n[![Python package](https://github.com/Pandora-Intelligence/concise-concepts/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/Pandora-Intelligence/concise-concepts/actions/workflows/python-package.yml)\n[![Current Release Version](https://img.shields.io/github/release/pandora-intelligence/concise-concepts.svg?style=flat-square&logo=github)](https://github.com/pandora-intelligence/concise-concepts/releases)\n[![pypi Version](https://img.shields.io/pypi/v/concise-concepts.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/concise-concepts/)\n[![PyPi downloads](https://static.pepy.tech/personalized-badge/concise-concepts?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)](https://pypi.org/project/concise-concepts/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)\n\n\n## Usage\nThis library defines matching patterns based on the most similar words found in each group, which are used to fill a [spaCy EntityRuler](https://spacy.io/api/entityruler). To better understand the rule definition, I recommend playing around with the [spaCy Rule-based Matcher Explorer](https://demos.explosion.ai/matcher).\n\n### Tutorials\n- [TechVizTheDataScienceGuy](https://www.youtube.com/c/TechVizTheDataScienceGuy) created a [nice tutorial](https://prakhar-mishra.medium.com/few-shot-named-entity-recognition-in-natural-language-processing-92d31f0d1143) on how to use it.\n\n- [I](https://www.linkedin.com/in/david-berenstein-1bab11105/) created a [tutorial](https://www.rubrix.ml/blog/concise-concepts-rubrix/) in collaboration with Rubrix.\n\nThe section [Matching Pattern Rules](#matching-pattern-rules) expands on the construction, analysis and customization of these matching patterns.\n\n\n# Install\n\n```\npip install concise-concepts\n```\n\n# Quickstart\n\nTake a look at the [configuration section](#configuration) for more info.\n\n## Spacy Pipeline Component\n\nNote that, [custom embedding models](#custom-embedding-models) are passed via `model_path`.\n\n```python\nimport spacy\nfrom spacy import displacy\n\nimport concise_concepts\n\ndata = {\n    "fruit": ["apple", "pear", "orange"],\n    "vegetable": ["broccoli", "spinach", "tomato"],\n    "meat": [\'beef\', \'pork\', \'turkey\', \'duck\']\n}\n\ntext = """\n    Heat the oil in a large pan and add the Onion, celery and carrots.\n    Then, cook over a medium–low heat for 10 minutes, or until softened.\n    Add the courgette, garlic, red peppers and oregano and cook for 2–3 minutes.\n    Later, add some oranges and chickens. """\n\nnlp = spacy.load("en_core_web_md", disable=["ner"])\n\nnlp.add_pipe(\n    "concise_concepts",\n    config={\n        "data": data,\n        "ent_score": True,  # Entity Scoring section\n        "verbose": True,\n        "exclude_pos": ["VERB", "AUX"],\n        "exclude_dep": ["DOBJ", "PCOMP"],\n        "include_compound_words": False,\n        "json_path": "./fruitful_patterns.json",\n        "topn": (100,500,300)\n    },\n)\ndoc = nlp(text)\n\noptions = {\n    "colors": {"fruit": "darkorange", "vegetable": "limegreen", "meat": "salmon"},\n    "ents": ["fruit", "vegetable", "meat"],\n}\n\nents = doc.ents\nfor ent in ents:\n    new_label = f"{ent.label_} ({ent._.ent_score:.0%})"\n    options["colors"][new_label] = options["colors"].get(ent.label_.lower(), None)\n    options["ents"].append(new_label)\n    ent.label_ = new_label\ndoc.ents = ents\n\ndisplacy.render(doc, style="ent", options=options)\n```\n![](https://raw.githubusercontent.com/Pandora-Intelligence/concise-concepts/master/img/example.png)\n\n## Standalone\n\nThis might be useful when iterating over few_shot training data when not wanting to reload larger models continuously.\nNote that, [custom embedding models](#custom-embedding-models) are passed via `model`.\n\n```python\nimport gensim\nimport spacy\n\nfrom concise_concepts import Conceptualizer\n\nmodel = gensim.downloader.load("fasttext-wiki-news-subwords-300")\nnlp = spacy.load("en_core_web_sm")\ndata = {\n    "disease": ["cancer", "diabetes", "heart disease", "influenza", "pneumonia"],\n    "symptom": ["headache", "fever", "cough", "nausea", "vomiting", "diarrhea"],\n}\nconceptualizer = Conceptualizer(nlp, data, model)\nconceptualizer.nlp("I have a headache and a fever.").ents\n\ndata = {\n    "disease": ["cancer", "diabetes"],\n    "symptom": ["headache", "fever"],\n}\nconceptualizer = Conceptualizer(nlp, data, model)\nconceptualizer.nlp("I have a headache and a fever.").ents\n```\n\n# Configuration\n## Matching Pattern Rules\nA general introduction about the usage of matching patterns in the [usage section](#usage).\n### Customizing Matching Pattern Rules\nEven though the baseline parameters provide a decent result, the construction of these matching rules can be customized via the config passed to the spaCy pipeline.\n\n - `exclude_pos`: A list of POS tags to be excluded from the rule-based match.\n - `exclude_dep`: A list of dependencies to be excluded from the rule-based match.\n - `include_compound_words`:  If True, it will include compound words in the entity. For example, if the entity is "New York", it will also include "New York City" as an entity.\n - `case_sensitive`: Whether to match the case of the words in the text.\n\n\n### Analyze Matching Pattern Rules\nTo motivate actually looking at the data and support interpretability, the matching patterns that have been generated are stored as `./main_patterns.json`. This behavior can be changed by using the `json_path` variable via the config passed to the spaCy pipeline.\n\n\n## Fuzzy matching using `spaczz`\n\n - `fuzzy`: A boolean value that determines whether to use fuzzy matching\n\n```python\ndata = {\n    "fruit": ["apple", "pear", "orange"],\n    "vegetable": ["broccoli", "spinach", "tomato"],\n    "meat": ["beef", "pork", "fish", "lamb"]\n}\n\nnlp.add_pipe("concise_concepts", config={"data": data, "fuzzy": True})\n```\n\n## Most Similar Word Expansion\n\n- `topn`: Use a specific number of words to expand over.\n\n```python\ndata = {\n    "fruit": ["apple", "pear", "orange"],\n    "vegetable": ["broccoli", "spinach", "tomato"],\n    "meat": ["beef", "pork", "fish", "lamb"]\n}\n\ntopn = [50, 50, 150]\n\nassert len(topn) == len\n\nnlp.add_pipe("concise_concepts", config={"data": data, "topn": topn})\n```\n\n## Entity Scoring\n\n- `ent_score`: Use embedding based word similarity to score entities against their groups\n\n```python\nimport spacy\nimport concise_concepts\n\ndata = {\n    "ORG": ["Google", "Apple", "Amazon"],\n    "GPE": ["Netherlands", "France", "China"],\n}\n\ntext = """Sony was founded in Japan."""\n\nnlp = spacy.load("en_core_web_lg")\nnlp.add_pipe("concise_concepts", config={"data": data, "ent_score": True, "case_sensitive": True})\ndoc = nlp(text)\n\nprint([(ent.text, ent.label_, ent._.ent_score) for ent in doc.ents])\n# output\n#\n# [(\'Sony\', \'ORG\', 0.5207586), (\'Japan\', \'GPE\', 0.7371268)]\n```\n\n## Custom Embedding Models\n\n- `model_path`: Use custom `sense2vec.Sense2Vec`, `gensim.Word2vec` `gensim.FastText`, or `gensim.KeyedVectors`, or a pretrained model from [gensim](https://radimrehurek.com/gensim/downloader.html) library or a custom model path. For using a `sense2vec.Sense2Vec` take a look [here](https://github.com/explosion/sense2vec#pretrained-vectors).\n- `model`: within [standalone usage](#standalone), it is possible to pass these models directly.\n\n```python\ndata = {\n    "fruit": ["apple", "pear", "orange"],\n    "vegetable": ["broccoli", "spinach", "tomato"],\n    "meat": ["beef", "pork", "fish", "lamb"]\n}\n\n# model from https://radimrehurek.com/gensim/downloader.html or path to local file\nmodel_path = "glove-wiki-gigaword-300"\n\nnlp.add_pipe("concise_concepts", config={"data": data, "model_path": model_path})\n````\n',
     'author': 'David Berenstein',
     'author_email': 'david.m.berenstein@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pandora-intelligence/concise-concepts',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'entry_points': entry_points,
     'python_requires': '>=3.8,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `concise-concepts-0.8.0/PKG-INFO` & `concise-concepts-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: concise-concepts
-Version: 0.8.0
+Version: 0.8.1
 Summary: This repository contains an easy and intuitive approach to few-shot NER using most similar expansion over spaCy embeddings. Now with entity confidence scores!
 Home-page: https://github.com/pandora-intelligence/concise-concepts
 License: MIT
 Keywords: spacy,NER,few-shot classification,nlu
 Author: David Berenstein
 Author-email: david.m.berenstein@gmail.com
 Requires-Python: >=3.8,<3.12
@@ -73,35 +73,36 @@
 from spacy import displacy
 
 import concise_concepts
 
 data = {
     "fruit": ["apple", "pear", "orange"],
     "vegetable": ["broccoli", "spinach", "tomato"],
-    "meat": ["beef", "pork", "fish", "lamb"],
+    "meat": ['beef', 'pork', 'turkey', 'duck']
 }
 
 text = """
     Heat the oil in a large pan and add the Onion, celery and carrots.
     Then, cook over a medium–low heat for 10 minutes, or until softened.
     Add the courgette, garlic, red peppers and oregano and cook for 2–3 minutes.
     Later, add some oranges and chickens. """
 
-nlp = spacy.load("en_core_web_lg", disable=["ner"])
+nlp = spacy.load("en_core_web_md", disable=["ner"])
 
 nlp.add_pipe(
     "concise_concepts",
     config={
         "data": data,
         "ent_score": True,  # Entity Scoring section
         "verbose": True,
         "exclude_pos": ["VERB", "AUX"],
         "exclude_dep": ["DOBJ", "PCOMP"],
         "include_compound_words": False,
         "json_path": "./fruitful_patterns.json",
+        "topn": (100,500,300)
     },
 )
 doc = nlp(text)
 
 options = {
     "colors": {"fruit": "darkorange", "vegetable": "limegreen", "meat": "salmon"},
     "ents": ["fruit", "vegetable", "meat"],
@@ -218,15 +219,15 @@
 # output
 #
 # [('Sony', 'ORG', 0.5207586), ('Japan', 'GPE', 0.7371268)]
 ```
 
 ## Custom Embedding Models
 
-- `model_path`: Use `sense2vec.Sense2Vec`, `gensim.Word2vec` `gensim.FastText`, or `gensim.KeyedVectors` model from the [pre-trained gensim](https://radimrehurek.com/gensim/downloader.html) library or a custom model path.
+- `model_path`: Use custom `sense2vec.Sense2Vec`, `gensim.Word2vec` `gensim.FastText`, or `gensim.KeyedVectors`, or a pretrained model from [gensim](https://radimrehurek.com/gensim/downloader.html) library or a custom model path. For using a `sense2vec.Sense2Vec` take a look [here](https://github.com/explosion/sense2vec#pretrained-vectors).
 - `model`: within [standalone usage](#standalone), it is possible to pass these models directly.
 
 ```python
 data = {
     "fruit": ["apple", "pear", "orange"],
     "vegetable": ["broccoli", "spinach", "tomato"],
     "meat": ["beef", "pork", "fish", "lamb"]
```

