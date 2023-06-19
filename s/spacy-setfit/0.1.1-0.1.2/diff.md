# Comparing `tmp/spacy-setfit-0.1.1.tar.gz` & `tmp/spacy_setfit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-setfit-0.1.1.tar", max compression
+gzip compressed data, was "spacy_setfit-0.1.2.tar", max compression
```

## Comparing `spacy-setfit-0.1.1.tar` & `spacy_setfit-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-06-18 18:34:17.411751 spacy-setfit-0.1.1/LICENSE
--rw-r--r--   0        0        0     7634 2023-06-19 08:31:56.053644 spacy-setfit-0.1.1/README.md
--rw-r--r--   0        0        0      492 2023-06-19 08:32:05.623581 spacy-setfit-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1586 2023-06-18 20:25:01.039528 spacy-setfit-0.1.1/spacy_setfit/__init__.py
--rw-r--r--   0        0        0     3841 2023-06-18 20:30:02.689552 spacy-setfit-0.1.1/spacy_setfit/models.py
--rw-r--r--   0        0        0     5168 2023-06-19 08:31:56.054341 spacy-setfit-0.1.1/spacy_setfit/schemas.py
--rw-r--r--   0        0        0     8506 1970-01-01 00:00:00.000000 spacy-setfit-0.1.1/setup.py
--rw-r--r--   0        0        0     8156 1970-01-01 00:00:00.000000 spacy-setfit-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-19 12:34:50.878479 spacy_setfit-0.1.2/LICENSE
+-rw-r--r--   0        0        0     7614 2023-06-19 12:34:50.878479 spacy_setfit-0.1.2/README.md
+-rw-r--r--   0        0        0      611 2023-06-19 12:34:50.882479 spacy_setfit-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1586 2023-06-19 12:34:50.882479 spacy_setfit-0.1.2/spacy_setfit/__init__.py
+-rw-r--r--   0        0        0     4084 2023-06-19 12:34:50.882479 spacy_setfit-0.1.2/spacy_setfit/models.py
+-rw-r--r--   0        0        0     5168 2023-06-19 12:34:50.882479 spacy_setfit-0.1.2/spacy_setfit/schemas.py
+-rw-r--r--   0        0        0     8187 1970-01-01 00:00:00.000000 spacy_setfit-0.1.2/PKG-INFO
```

### Comparing `spacy-setfit-0.1.1/LICENSE` & `spacy_setfit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-setfit-0.1.1/README.md` & `spacy_setfit-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 ## Getting Started
 
 To use spaCy with SetFit use the following code:
 
 ```python
 import spacy
-import spacy_setfit
 
 # Create some example data
 train_dataset = {
     "inlier": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa."],
     "outlier": ["Text about kitchen equipment",
```

### Comparing `spacy-setfit-0.1.1/spacy_setfit/__init__.py` & `spacy_setfit-0.1.2/spacy_setfit/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-setfit-0.1.1/spacy_setfit/models.py` & `spacy_setfit-0.1.2/spacy_setfit/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import logging
 import types
 
 from setfit import SetFitModel, SetFitTrainer
 from spacy import util
 from spacy.language import Language
 from spacy.tokens import Doc
 
 from spacy_setfit.schemas import SetFitTrainerArgs
 
+__LOGGER__ = logging.getLogger(__name__)
+
 
 class SpacySetFit:
-    def __init__(self, nlp: Language, model: SetFitModel, labels = None):
+    def __init__(self, nlp: Language, model: SetFitModel, labels=None):
         self.nlp = nlp
         self.model = model
         self.multi_label = self._check_multi_label(model)
         self.labels = labels
         if self.labels:
             self.id2label = {i: label for i, label in enumerate(self.labels)}
         else:
@@ -23,49 +26,66 @@
     def _check_multi_label(model: SetFitModel):
         if model.multi_target_strategy:
             return True
         else:
             return False
 
     @staticmethod
-    def _from_pretrained(pretrained_model_name_or_path: str, setfit_from_pretrained_args: dict = None):
+    def _from_pretrained(
+        pretrained_model_name_or_path: str, setfit_from_pretrained_args: dict = None
+    ):
         if setfit_from_pretrained_args is None:
             setfit_from_pretrained_args = {}
         model = SetFitModel.from_pretrained(
             pretrained_model_name_or_path, **setfit_from_pretrained_args
         )
         return model
 
     @classmethod
-    def from_pretrained(cls, nlp: Language, pretrained_model_name_or_path: str, setfit_from_pretrained_args: dict = None):
-        model = cls._from_pretrained(pretrained_model_name_or_path, setfit_from_pretrained_args)
+    def from_pretrained(
+        cls,
+        nlp: Language,
+        pretrained_model_name_or_path: str,
+        setfit_from_pretrained_args: dict = None,
+    ):
+        model = cls._from_pretrained(
+            pretrained_model_name_or_path, setfit_from_pretrained_args
+        )
         return cls(nlp, model)
 
     @classmethod
-    def from_trained(cls, nlp: Language, pretrained_model_name_or_path: str, setfit_trainer_args: SetFitTrainerArgs, setfit_from_pretrained_args: dict = None):
-
-        setfit_from_pretrained_args["multi_target_strategy"] = setfit_from_pretrained_args.get("multi_target_strategy")
+    def from_trained(
+        cls,
+        nlp: Language,
+        pretrained_model_name_or_path: str,
+        setfit_trainer_args: SetFitTrainerArgs,
+        setfit_from_pretrained_args: dict = None,
+    ):
+        setfit_from_pretrained_args[
+            "multi_target_strategy"
+        ] = setfit_from_pretrained_args.get("multi_target_strategy")
         if setfit_trainer_args.multi_label:
             setfit_from_pretrained_args["multi_target_strategy"] = "one-vs-rest"
 
-        model = cls._from_pretrained(pretrained_model_name_or_path, setfit_from_pretrained_args)
-        trainer = SetFitTrainer(
-            model=model,
-            **setfit_trainer_args.dict()
+        model = cls._from_pretrained(
+            pretrained_model_name_or_path, setfit_from_pretrained_args
         )
+        trainer = SetFitTrainer(model=model, **setfit_trainer_args.dict())
         trainer.train()
         if setfit_trainer_args.eval_dataset:
             evaluation = trainer.evaluate()
-            print(evaluation)
+            __LOGGER__.info(f"evaluation: {evaluation}")
 
         return cls(nlp, model, labels=setfit_trainer_args.labels)
 
     def _assign_labels(self, doc, prediction: list):
         if self.id2label:
-            doc.cats = {self.id2label[idx]: float(score) for idx, score in enumerate(prediction)}
+            doc.cats = {
+                self.id2label[idx]: float(score) for idx, score in enumerate(prediction)
+            }
         else:
             doc.cats = {idx: float(score) for idx, score in enumerate(prediction)}
         return doc
 
     def __call__(self, doc: Doc):
         """
         It takes a doc, gets the embeddings from the doc, reshapes the embeddings, gets the prediction from the embeddings,
```

### Comparing `spacy-setfit-0.1.1/spacy_setfit/schemas.py` & `spacy_setfit-0.1.2/spacy_setfit/schemas.py`

 * *Files identical despite different names*

### Comparing `spacy-setfit-0.1.1/setup.py` & `spacy_setfit-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,189 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: spacy-setfit
+Version: 0.1.2
+Summary: 
+Author: davidberenstein1957
+Author-email: david.m.berenstein@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: rich (>=13.4.2,<14.0.0)
+Requires-Dist: setfit (>=0.7.0,<0.8.0)
+Requires-Dist: spacy (>=3.5.3,<4.0.0)
+Description-Content-Type: text/markdown
+
+# spacy-setfit
+
+This repository contains an easy and intuitive approach to using [SetFit](https://github.com/huggingface/setfit) in combination with [spaCy](https://github.com/explosion/spaCy).
+
+## Installation
+
+Before using spaCy with SetFit, make sure you have the necessary packages installed. You can install them using pip:
+
+```
+pip install spacy spacy-setfit
+```
+
+Additionally, you will might want to download a spaCy model, for example:
+
+```
+python -m spacy download en_core_web_sm
+```
+
+## Getting Started
+
+To use spaCy with SetFit use the following code:
+
+```python
+import spacy
+
+# Create some example data
+train_dataset = {
+    "inlier": ["This text is about chairs.",
+               "Couches, benches and televisions.",
+               "I really need to get a new sofa."],
+    "outlier": ["Text about kitchen equipment",
+                "This text is about politics",
+                "Comments about AI and stuff."]
+}
+
+# Load the spaCy language model:
+nlp = spacy.load("en_core_web_sm")
+
+# Add the "text_categorizer" pipeline component to the spaCy model, and configure it with SetFit parameters:
+nlp.add_pipe("text_categorizer", config={
+    "pretrained_model_name_or_path": "paraphrase-MiniLM-L3-v2",
+    "setfit_trainer_args": {
+        "train_dataset": train_dataset
+    }
+})
+doc = nlp("I really need to get a new sofa.")
+doc.cats
+# {'inlier': 0.902350975129, 'outlier': 0.097649024871}
+```
+
+The code above processes the input text with the spaCy model, and the `doc.cats` attribute returns the predicted categories and their associated probabilities.
+
+That's it! You have now successfully integrated spaCy with SetFit for text categorization tasks. You can further customize and train the model using additional data or adjust the SetFit parameters as needed.
+
+Feel free to explore more features and documentation of spaCy and SetFit to enhance your text classification projects.
+
+## setfit_trainer_args
+
+The `setfit_trainer_args` are a simplified version of [the official args from the SetFit library](https://github.com/huggingface/setfit#training-a-setfit-model).
+
+### Arguments
+
+- `train_dataset` (Union[dict, Dataset]): The training dataset to be used by the SetFitTrainer. It can be either a dictionary or a Dataset object.
+
+- `eval_dataset` (Union[dict, Dataset], optional): The evaluation dataset to be used by the SetFitTrainer. It can be either a dictionary or a Dataset object. Defaults to `None`.
+
+- `num_iterations` (int, optional): The number of iterations to train the model. Defaults to `20`.
+
+- `num_epochs` (int, optional): The number of epochs to train the model. Defaults to `1`.
+
+- `learning_rate` (float, optional): The learning rate for the optimizer. Defaults to `2e-5`.
+
+- `batch_size` (float, optional): The batch size for training. Defaults to `16`.
+
+- `seed` (int, optional): The random seed for reproducibility. Defaults to `42`.
+
+- `column_mapping` (dict, optional): A mapping dictionary that specifies how to map input columns to model inputs. Defaults to `None`.
+
+- `use_amp` (bool, optional): Whether to use Automatic Mixed Precision (AMP) for training. Defaults to `False`.
+
+Please note that the above documentation provides an overview of the arguments and their purpose. For more detailed information and usage examples, it is recommended to refer to the official SetFit library documentation or any specific implementation details provided by the library.
+
+### Usage
+
+To use the `setfit_trainer_args`, you can create a dictionary with the desired values for the arguments. Here's an example:
+
+```python
+setfit_trainer_args = {
+    "train_dataset": train_data,
+    "eval_dataset": eval_data,
+    "num_iterations": 20,
+    "num_epochs": 1,
+    "learning_rate": 2e-5,
+    "batch_size": 16,
+    "seed": 42,
+    "column_mapping": column_map,
+    "use_amp": False
+}
+```
+
+## setfit_from_pretrained_args
+
+The `setfit_from_pretrained_args` are a simplified version of [the official args from the SetFit library](https://github.com/huggingface/setfit#training-a-setfit-model) and [Hugging Face transformers](https://huggingface.co/docs/transformers/main_classes/model#transformers.PreTrainedModel.from_pretrained).
+
+### Arguments
+
+- `pretrained_model_name_or_path` (str or Path): This argument specifies the model to be loaded. It can be either:
+  - The `model_id` (string) of a model hosted on the Hugging Face Model Hub, e.g., `bigscience/bloom`.
+  - A path to a directory containing model weights saved using the `save_pretrained` method of `PreTrainedModel`, e.g., `../path/to/my_model_directory/`.
+
+- `revision` (str, optional): The revision of the model on the Hub. It can be a branch name, a git tag, or any commit id. Defaults to the latest commit on the main branch.
+
+- `force_download` (bool, optional): Whether to force (re-)downloading the model weights and configuration files from the Hub, overriding the existing cache. Defaults to `False`.
+
+- `resume_download` (bool, optional): Whether to delete incompletely received files and attempt to resume the download if such a file exists. Defaults to `False`.
+
+- `proxies` (Dict[str, str], optional): A dictionary of proxy servers to use by protocol or endpoint. It is used for requests made during the downloading process. For example: `proxies = {'http': 'foo.bar:3128', 'http://hostname': 'foo.bar:4012'}`
+
+- `token` (str or bool, optional): The token to use as HTTP bearer authorization for remote files. By default, it uses the token cached when running `huggingface-cli login`.
+
+- `cache_dir` (str or Path, optional): The path to the folder where cached files are stored.
 
-packages = \
-['spacy_setfit']
+- `local_files_only` (bool, optional): If `True`, it avoids downloading the file and returns the path to the local cached file if it exists. Defaults to `False`.
 
-package_data = \
-{'': ['*']}
+- `model_kwargs` (Dict, optional): Additional keyword arguments to pass to the model during initialization.
 
-install_requires = \
-['rich>=13.4.2,<14.0.0', 'setfit>=0.7.0,<0.8.0', 'spacy>=3.5.3,<4.0.0']
-
-setup_kwargs = {
-    'name': 'spacy-setfit',
-    'version': '0.1.1',
-    'description': '',
-    'long_description': '# spacy-setfit\n\nThis repository contains an easy and intuitive approach to using [SetFit](https://github.com/huggingface/setfit) in combination with [spaCy](https://github.com/explosion/spaCy).\n\n## Installation\n\nBefore using spaCy with SetFit, make sure you have the necessary packages installed. You can install them using pip:\n\n```\npip install spacy spacy-setfit\n```\n\nAdditionally, you will might want to download a spaCy model, for example:\n\n```\npython -m spacy download en_core_web_sm\n```\n\n## Getting Started\n\nTo use spaCy with SetFit use the following code:\n\n```python\nimport spacy\nimport spacy_setfit\n\n# Create some example data\ntrain_dataset = {\n    "inlier": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "outlier": ["Text about kitchen equipment",\n                "This text is about politics",\n                "Comments about AI and stuff."]\n}\n\n# Load the spaCy language model:\nnlp = spacy.load("en_core_web_sm")\n\n# Add the "text_categorizer" pipeline component to the spaCy model, and configure it with SetFit parameters:\nnlp.add_pipe("text_categorizer", config={\n    "pretrained_model_name_or_path": "paraphrase-MiniLM-L3-v2",\n    "setfit_trainer_args": {\n        "train_dataset": train_dataset\n    }\n})\ndoc = nlp("I really need to get a new sofa.")\ndoc.cats\n# {\'inlier\': 0.902350975129, \'outlier\': 0.097649024871}\n```\n\nThe code above processes the input text with the spaCy model, and the `doc.cats` attribute returns the predicted categories and their associated probabilities.\n\nThat\'s it! You have now successfully integrated spaCy with SetFit for text categorization tasks. You can further customize and train the model using additional data or adjust the SetFit parameters as needed.\n\nFeel free to explore more features and documentation of spaCy and SetFit to enhance your text classification projects.\n\n## setfit_trainer_args\n\nThe `setfit_trainer_args` are a simplified version of [the official args from the SetFit library](https://github.com/huggingface/setfit#training-a-setfit-model).\n\n### Arguments\n\n- `train_dataset` (Union[dict, Dataset]): The training dataset to be used by the SetFitTrainer. It can be either a dictionary or a Dataset object.\n\n- `eval_dataset` (Union[dict, Dataset], optional): The evaluation dataset to be used by the SetFitTrainer. It can be either a dictionary or a Dataset object. Defaults to `None`.\n\n- `num_iterations` (int, optional): The number of iterations to train the model. Defaults to `20`.\n\n- `num_epochs` (int, optional): The number of epochs to train the model. Defaults to `1`.\n\n- `learning_rate` (float, optional): The learning rate for the optimizer. Defaults to `2e-5`.\n\n- `batch_size` (float, optional): The batch size for training. Defaults to `16`.\n\n- `seed` (int, optional): The random seed for reproducibility. Defaults to `42`.\n\n- `column_mapping` (dict, optional): A mapping dictionary that specifies how to map input columns to model inputs. Defaults to `None`.\n\n- `use_amp` (bool, optional): Whether to use Automatic Mixed Precision (AMP) for training. Defaults to `False`.\n\nPlease note that the above documentation provides an overview of the arguments and their purpose. For more detailed information and usage examples, it is recommended to refer to the official SetFit library documentation or any specific implementation details provided by the library.\n\n### Usage\n\nTo use the `setfit_trainer_args`, you can create a dictionary with the desired values for the arguments. Here\'s an example:\n\n```python\nsetfit_trainer_args = {\n    "train_dataset": train_data,\n    "eval_dataset": eval_data,\n    "num_iterations": 20,\n    "num_epochs": 1,\n    "learning_rate": 2e-5,\n    "batch_size": 16,\n    "seed": 42,\n    "column_mapping": column_map,\n    "use_amp": False\n}\n```\n\n## setfit_from_pretrained_args\n\nThe `setfit_from_pretrained_args` are a simplified version of [the official args from the SetFit library](https://github.com/huggingface/setfit#training-a-setfit-model) and [Hugging Face transformers](https://huggingface.co/docs/transformers/main_classes/model#transformers.PreTrainedModel.from_pretrained).\n\n### Arguments\n\n- `pretrained_model_name_or_path` (str or Path): This argument specifies the model to be loaded. It can be either:\n  - The `model_id` (string) of a model hosted on the Hugging Face Model Hub, e.g., `bigscience/bloom`.\n  - A path to a directory containing model weights saved using the `save_pretrained` method of `PreTrainedModel`, e.g., `../path/to/my_model_directory/`.\n\n- `revision` (str, optional): The revision of the model on the Hub. It can be a branch name, a git tag, or any commit id. Defaults to the latest commit on the main branch.\n\n- `force_download` (bool, optional): Whether to force (re-)downloading the model weights and configuration files from the Hub, overriding the existing cache. Defaults to `False`.\n\n- `resume_download` (bool, optional): Whether to delete incompletely received files and attempt to resume the download if such a file exists. Defaults to `False`.\n\n- `proxies` (Dict[str, str], optional): A dictionary of proxy servers to use by protocol or endpoint. It is used for requests made during the downloading process. For example: `proxies = {\'http\': \'foo.bar:3128\', \'http://hostname\': \'foo.bar:4012\'}`\n\n- `token` (str or bool, optional): The token to use as HTTP bearer authorization for remote files. By default, it uses the token cached when running `huggingface-cli login`.\n\n- `cache_dir` (str or Path, optional): The path to the folder where cached files are stored.\n\n- `local_files_only` (bool, optional): If `True`, it avoids downloading the file and returns the path to the local cached file if it exists. Defaults to `False`.\n\n- `model_kwargs` (Dict, optional): Additional keyword arguments to pass to the model during initialization.\n\nPlease note that the above documentation provides an overview of the arguments and their purpose. For more detailed information and usage examples, it is recommended to refer to the official SetFit library documentation or any specific implementation details provided by the library.\n\n### Usage\n\nTo use the `setfit_from_pretrained_args`, you can create a dictionary with the desired values for the arguments. Here\'s an example:\n\n```python\nsetfit_from_pretrained_args = {\n    \'pretrained_model_name_or_path\': \'\',  # str or Path\n    \'revision\': None,  # str, optional\n    \'force_download\': False,  # bool, optional\n    \'resume_download\': False,  # bool, optional\n    \'proxies\': None,  # Dict[str, str], optional\n    \'token\': None,  # str or bool, optional\n    \'cache_dir\': None,  # str or Path, optional\n    \'local_files_only\': False,  # bool, optional\n    \'model_kwargs\': None  # Dict, optional\n}\n```\n\n## Saving and Loading models\n\nYou can use the `pickle` module in Python to save and load instances of the pre-trained pipeline. `pickle` allows you to serialize Python objects, including custom classes, into a binary format that can be saved to a file and loaded back into memory later. Here\'s an example of how to save and load using `pickle`:\n\n```python\nimport pickle\n\nnlp = ...\n\n# Save nlp pipeline\nwith open("my_cool_model.pkl", "wb") as file:\n    pickle.dump(nlp, file)\n\n# Load nlp pipeline\nwith open("my_cool_model.pkl", "rb") as file:\n    nlp = pickle.load(file)\n\ndoc = nlp("I really need to get a new sofa.")\ndoc.cats\n# {\'inlier\': 0.902350975129, \'outlier\': 0.097649024871}\n```\n\n## Logo Reference\n\nQuotation by Adrien Coquet from <a href="https://thenounproject.com/browse/icons/term/quotation/" target="_blank" title="quotation Icons">Noun Project</a>\n',
-    'author': 'davidberenstein1957',
-    'author_email': 'david.m.berenstein@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+Please note that the above documentation provides an overview of the arguments and their purpose. For more detailed information and usage examples, it is recommended to refer to the official SetFit library documentation or any specific implementation details provided by the library.
+
+### Usage
+
+To use the `setfit_from_pretrained_args`, you can create a dictionary with the desired values for the arguments. Here's an example:
+
+```python
+setfit_from_pretrained_args = {
+    'pretrained_model_name_or_path': '',  # str or Path
+    'revision': None,  # str, optional
+    'force_download': False,  # bool, optional
+    'resume_download': False,  # bool, optional
+    'proxies': None,  # Dict[str, str], optional
+    'token': None,  # str or bool, optional
+    'cache_dir': None,  # str or Path, optional
+    'local_files_only': False,  # bool, optional
+    'model_kwargs': None  # Dict, optional
 }
+```
+
+## Saving and Loading models
+
+You can use the `pickle` module in Python to save and load instances of the pre-trained pipeline. `pickle` allows you to serialize Python objects, including custom classes, into a binary format that can be saved to a file and loaded back into memory later. Here's an example of how to save and load using `pickle`:
+
+```python
+import pickle
+
+nlp = ...
+
+# Save nlp pipeline
+with open("my_cool_model.pkl", "wb") as file:
+    pickle.dump(nlp, file)
+
+# Load nlp pipeline
+with open("my_cool_model.pkl", "rb") as file:
+    nlp = pickle.load(file)
+
+doc = nlp("I really need to get a new sofa.")
+doc.cats
+# {'inlier': 0.902350975129, 'outlier': 0.097649024871}
+```
+
+## Logo Reference
 
+Quotation by Adrien Coquet from <a href="https://thenounproject.com/browse/icons/term/quotation/" target="_blank" title="quotation Icons">Noun Project</a>
 
-setup(**setup_kwargs)
```

