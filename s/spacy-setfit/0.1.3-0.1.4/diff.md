# Comparing `tmp/spacy-setfit-0.1.3.tar.gz` & `tmp/spacy-setfit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-setfit-0.1.3.tar", max compression
+gzip compressed data, was "spacy-setfit-0.1.4.tar", max compression
```

## Comparing `spacy-setfit-0.1.3.tar` & `spacy-setfit-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-06-18 18:34:17.411751 spacy-setfit-0.1.3/LICENSE
--rw-r--r--   0        0        0     7614 2023-06-19 11:22:30.026441 spacy-setfit-0.1.3/README.md
--rw-r--r--   0        0        0      601 2023-06-19 14:40:04.205002 spacy-setfit-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1586 2023-06-18 20:25:01.039528 spacy-setfit-0.1.3/spacy_setfit/__init__.py
--rw-r--r--   0        0        0     4084 2023-06-19 12:29:15.459829 spacy-setfit-0.1.3/spacy_setfit/models.py
--rw-r--r--   0        0        0     5168 2023-06-19 08:31:56.054341 spacy-setfit-0.1.3/spacy_setfit/schemas.py
--rw-r--r--   0        0        0     8592 1970-01-01 00:00:00.000000 spacy-setfit-0.1.3/setup.py
--rw-r--r--   0        0        0     8116 1970-01-01 00:00:00.000000 spacy-setfit-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-18 18:34:17.411751 spacy-setfit-0.1.4/LICENSE
+-rw-r--r--   0        0        0     7614 2023-06-19 11:22:30.026441 spacy-setfit-0.1.4/README.md
+-rw-r--r--   0        0        0      601 2023-06-19 17:19:56.591881 spacy-setfit-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1560 2023-06-19 17:20:20.188541 spacy-setfit-0.1.4/spacy_setfit/__init__.py
+-rw-r--r--   0        0        0     4084 2023-06-19 12:29:15.459829 spacy-setfit-0.1.4/spacy_setfit/models.py
+-rw-r--r--   0        0        0     5168 2023-06-19 08:31:56.054341 spacy-setfit-0.1.4/spacy_setfit/schemas.py
+-rw-r--r--   0        0        0     8592 1970-01-01 00:00:00.000000 spacy-setfit-0.1.4/setup.py
+-rw-r--r--   0        0        0     8116 1970-01-01 00:00:00.000000 spacy-setfit-0.1.4/PKG-INFO
```

### Comparing `spacy-setfit-0.1.3/LICENSE` & `spacy-setfit-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-setfit-0.1.3/README.md` & `spacy-setfit-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `spacy-setfit-0.1.3/pyproject.toml` & `spacy-setfit-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spacy-setfit"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["davidberenstein1957 <david.m.berenstein@gmail.com>"]
 readme = "README.md"
 packages = [{include = "spacy_setfit"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `spacy-setfit-0.1.3/spacy_setfit/__init__.py` & `spacy-setfit-0.1.4/spacy_setfit/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,24 +2,21 @@
 
 from rich.logging import RichHandler
 from spacy.language import Language
 
 from spacy_setfit.models import SpacySetFit
 from spacy_setfit.schemas import SetFitTrainerArgs
 
-__all__ = [
-    "SpacySetFit",
-    "SetFitTrainerArgs"
-]
+__all__ = ["SpacySetFit", "SetFitTrainerArgs"]
 
 logging.basicConfig(
     level="INFO",
     format="%(message)s",
     datefmt="[%X]",
-    handlers=[RichHandler(rich_tracebacks=True)]
+    handlers=[RichHandler(rich_tracebacks=True)],
 )
 
 
 @Language.factory(
     "text_categorizer",
     default_config={
         "pretrained_model_name_or_path": "all-MiniLM-L6-v2",
@@ -33,26 +30,24 @@
     pretrained_model_name_or_path: str = "all-MiniLM-L6-v2",
     setfit_from_pretrained_args: dict = None,
     setfit_trainer_args: dict = None,
 ):
     if setfit_from_pretrained_args is None:
         setfit_from_pretrained_args = {}
     if setfit_trainer_args is None:
-        setfit_trainer_args = SetFitTrainerArgs()
+        setfit_trainer_args = {}
     else:
         setfit_trainer_args = SetFitTrainerArgs(**setfit_trainer_args)
 
-
     if setfit_trainer_args != {}:
         return SpacySetFit.from_trained(
             nlp=nlp,
             pretrained_model_name_or_path=pretrained_model_name_or_path,
             setfit_from_pretrained_args=setfit_from_pretrained_args,
-            setfit_trainer_args=setfit_trainer_args
+            setfit_trainer_args=setfit_trainer_args,
         )
     else:
         return SpacySetFit.from_pretrained(
             nlp=nlp,
             pretrained_model_name_or_path=pretrained_model_name_or_path,
-            setfit_from_pretrained_args=setfit_from_pretrained_args
+            setfit_from_pretrained_args=setfit_from_pretrained_args,
         )
-
```

### Comparing `spacy-setfit-0.1.3/spacy_setfit/models.py` & `spacy-setfit-0.1.4/spacy_setfit/models.py`

 * *Files identical despite different names*

### Comparing `spacy-setfit-0.1.3/spacy_setfit/schemas.py` & `spacy-setfit-0.1.4/spacy_setfit/schemas.py`

 * *Files identical despite different names*

### Comparing `spacy-setfit-0.1.3/setup.py` & `spacy-setfit-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['rich>=13,<14', 'setfit>=0.7,<0.8', 'spacy>=3,<4']
 
 entry_points = \
 {'spacy_factories': ['spacy = spacy_setfit.__init__:create_setfit_model']}
 
 setup_kwargs = {
     'name': 'spacy-setfit',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': '',
     'long_description': '# spacy-setfit\n\nThis repository contains an easy and intuitive approach to using [SetFit](https://github.com/huggingface/setfit) in combination with [spaCy](https://github.com/explosion/spaCy).\n\n## Installation\n\nBefore using spaCy with SetFit, make sure you have the necessary packages installed. You can install them using pip:\n\n```\npip install spacy spacy-setfit\n```\n\nAdditionally, you will might want to download a spaCy model, for example:\n\n```\npython -m spacy download en_core_web_sm\n```\n\n## Getting Started\n\nTo use spaCy with SetFit use the following code:\n\n```python\nimport spacy\n\n# Create some example data\ntrain_dataset = {\n    "inlier": ["This text is about chairs.",\n               "Couches, benches and televisions.",\n               "I really need to get a new sofa."],\n    "outlier": ["Text about kitchen equipment",\n                "This text is about politics",\n                "Comments about AI and stuff."]\n}\n\n# Load the spaCy language model:\nnlp = spacy.load("en_core_web_sm")\n\n# Add the "text_categorizer" pipeline component to the spaCy model, and configure it with SetFit parameters:\nnlp.add_pipe("text_categorizer", config={\n    "pretrained_model_name_or_path": "paraphrase-MiniLM-L3-v2",\n    "setfit_trainer_args": {\n        "train_dataset": train_dataset\n    }\n})\ndoc = nlp("I really need to get a new sofa.")\ndoc.cats\n# {\'inlier\': 0.902350975129, \'outlier\': 0.097649024871}\n```\n\nThe code above processes the input text with the spaCy model, and the `doc.cats` attribute returns the predicted categories and their associated probabilities.\n\nThat\'s it! You have now successfully integrated spaCy with SetFit for text categorization tasks. You can further customize and train the model using additional data or adjust the SetFit parameters as needed.\n\nFeel free to explore more features and documentation of spaCy and SetFit to enhance your text classification projects.\n\n## setfit_trainer_args\n\nThe `setfit_trainer_args` are a simplified version of [the official args from the SetFit library](https://github.com/huggingface/setfit#training-a-setfit-model).\n\n### Arguments\n\n- `train_dataset` (Union[dict, Dataset]): The training dataset to be used by the SetFitTrainer. It can be either a dictionary or a Dataset object.\n\n- `eval_dataset` (Union[dict, Dataset], optional): The evaluation dataset to be used by the SetFitTrainer. It can be either a dictionary or a Dataset object. Defaults to `None`.\n\n- `num_iterations` (int, optional): The number of iterations to train the model. Defaults to `20`.\n\n- `num_epochs` (int, optional): The number of epochs to train the model. Defaults to `1`.\n\n- `learning_rate` (float, optional): The learning rate for the optimizer. Defaults to `2e-5`.\n\n- `batch_size` (float, optional): The batch size for training. Defaults to `16`.\n\n- `seed` (int, optional): The random seed for reproducibility. Defaults to `42`.\n\n- `column_mapping` (dict, optional): A mapping dictionary that specifies how to map input columns to model inputs. Defaults to `None`.\n\n- `use_amp` (bool, optional): Whether to use Automatic Mixed Precision (AMP) for training. Defaults to `False`.\n\nPlease note that the above documentation provides an overview of the arguments and their purpose. For more detailed information and usage examples, it is recommended to refer to the official SetFit library documentation or any specific implementation details provided by the library.\n\n### Usage\n\nTo use the `setfit_trainer_args`, you can create a dictionary with the desired values for the arguments. Here\'s an example:\n\n```python\nsetfit_trainer_args = {\n    "train_dataset": train_data,\n    "eval_dataset": eval_data,\n    "num_iterations": 20,\n    "num_epochs": 1,\n    "learning_rate": 2e-5,\n    "batch_size": 16,\n    "seed": 42,\n    "column_mapping": column_map,\n    "use_amp": False\n}\n```\n\n## setfit_from_pretrained_args\n\nThe `setfit_from_pretrained_args` are a simplified version of [the official args from the SetFit library](https://github.com/huggingface/setfit#training-a-setfit-model) and [Hugging Face transformers](https://huggingface.co/docs/transformers/main_classes/model#transformers.PreTrainedModel.from_pretrained).\n\n### Arguments\n\n- `pretrained_model_name_or_path` (str or Path): This argument specifies the model to be loaded. It can be either:\n  - The `model_id` (string) of a model hosted on the Hugging Face Model Hub, e.g., `bigscience/bloom`.\n  - A path to a directory containing model weights saved using the `save_pretrained` method of `PreTrainedModel`, e.g., `../path/to/my_model_directory/`.\n\n- `revision` (str, optional): The revision of the model on the Hub. It can be a branch name, a git tag, or any commit id. Defaults to the latest commit on the main branch.\n\n- `force_download` (bool, optional): Whether to force (re-)downloading the model weights and configuration files from the Hub, overriding the existing cache. Defaults to `False`.\n\n- `resume_download` (bool, optional): Whether to delete incompletely received files and attempt to resume the download if such a file exists. Defaults to `False`.\n\n- `proxies` (Dict[str, str], optional): A dictionary of proxy servers to use by protocol or endpoint. It is used for requests made during the downloading process. For example: `proxies = {\'http\': \'foo.bar:3128\', \'http://hostname\': \'foo.bar:4012\'}`\n\n- `token` (str or bool, optional): The token to use as HTTP bearer authorization for remote files. By default, it uses the token cached when running `huggingface-cli login`.\n\n- `cache_dir` (str or Path, optional): The path to the folder where cached files are stored.\n\n- `local_files_only` (bool, optional): If `True`, it avoids downloading the file and returns the path to the local cached file if it exists. Defaults to `False`.\n\n- `model_kwargs` (Dict, optional): Additional keyword arguments to pass to the model during initialization.\n\nPlease note that the above documentation provides an overview of the arguments and their purpose. For more detailed information and usage examples, it is recommended to refer to the official SetFit library documentation or any specific implementation details provided by the library.\n\n### Usage\n\nTo use the `setfit_from_pretrained_args`, you can create a dictionary with the desired values for the arguments. Here\'s an example:\n\n```python\nsetfit_from_pretrained_args = {\n    \'pretrained_model_name_or_path\': \'\',  # str or Path\n    \'revision\': None,  # str, optional\n    \'force_download\': False,  # bool, optional\n    \'resume_download\': False,  # bool, optional\n    \'proxies\': None,  # Dict[str, str], optional\n    \'token\': None,  # str or bool, optional\n    \'cache_dir\': None,  # str or Path, optional\n    \'local_files_only\': False,  # bool, optional\n    \'model_kwargs\': None  # Dict, optional\n}\n```\n\n## Saving and Loading models\n\nYou can use the `pickle` module in Python to save and load instances of the pre-trained pipeline. `pickle` allows you to serialize Python objects, including custom classes, into a binary format that can be saved to a file and loaded back into memory later. Here\'s an example of how to save and load using `pickle`:\n\n```python\nimport pickle\n\nnlp = ...\n\n# Save nlp pipeline\nwith open("my_cool_model.pkl", "wb") as file:\n    pickle.dump(nlp, file)\n\n# Load nlp pipeline\nwith open("my_cool_model.pkl", "rb") as file:\n    nlp = pickle.load(file)\n\ndoc = nlp("I really need to get a new sofa.")\ndoc.cats\n# {\'inlier\': 0.902350975129, \'outlier\': 0.097649024871}\n```\n\n## Logo Reference\n\nQuotation by Adrien Coquet from <a href="https://thenounproject.com/browse/icons/term/quotation/" target="_blank" title="quotation Icons">Noun Project</a>\n',
     'author': 'davidberenstein1957',
     'author_email': 'david.m.berenstein@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `spacy-setfit-0.1.3/PKG-INFO` & `spacy-setfit-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-setfit
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: davidberenstein1957
 Author-email: david.m.berenstein@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

