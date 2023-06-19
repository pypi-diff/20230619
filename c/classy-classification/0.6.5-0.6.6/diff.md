# Comparing `tmp/classy-classification-0.6.5.tar.gz` & `tmp/classy_classification-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classy-classification-0.6.5.tar", max compression
+gzip compressed data, was "classy_classification-0.6.6.tar", max compression
```

## Comparing `classy-classification-0.6.5.tar` & `classy_classification-0.6.6.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1073 2022-11-01 08:20:25.558101 classy-classification-0.6.5/LICENSE
--rw-r--r--   0        0        0    10736 2023-06-19 12:49:50.792281 classy-classification-0.6.5/README.md
--rw-r--r--   0        0        0     2591 2023-06-19 12:47:07.008098 classy-classification-0.6.5/classy_classification/__init__.py
--rw-r--r--   0        0        0        0 2022-11-01 08:20:25.558372 classy-classification-0.6.5/classy_classification/classifiers/__init__.py
--rw-r--r--   0        0        0    10545 2023-06-18 12:48:16.591005 classy-classification-0.6.5/classy_classification/classifiers/classy_skeleton.py
--rw-r--r--   0        0        0     9186 2023-06-19 12:49:50.792618 classy-classification-0.6.5/classy_classification/classifiers/classy_spacy.py
--rw-r--r--   0        0        0     2274 2023-06-18 12:48:19.711859 classy-classification-0.6.5/classy_classification/classifiers/classy_standalone.py
--rw-r--r--   0        0        0        0 2022-11-01 08:20:25.558915 classy-classification-0.6.5/classy_classification/examples/__init__.py
--rw-r--r--   0        0        0     2324 2023-01-14 09:24:42.022043 classy-classification-0.6.5/classy_classification/examples/data.py
--rw-r--r--   0        0        0      230 2022-12-30 07:21:01.276435 classy-classification-0.6.5/classy_classification/examples/individual_transformer.py
--rw-r--r--   0        0        0      339 2023-03-03 12:03:23.566908 classy-classification-0.6.5/classy_classification/examples/spacy_few_shot_external.py
--rw-r--r--   0        0        0      368 2023-03-03 12:03:22.068037 classy-classification-0.6.5/classy_classification/examples/spacy_internal_embeddings.py
--rw-r--r--   0        0        0      372 2023-03-03 12:03:19.152952 classy-classification-0.6.5/classy_classification/examples/spacy_zero_shot_external.py
--rw-r--r--   0        0        0     2353 2023-06-19 12:51:00.325718 classy-classification-0.6.5/pyproject.toml
--rw-r--r--   0        0        0    12436 1970-01-01 00:00:00.000000 classy-classification-0.6.5/setup.py
--rw-r--r--   0        0        0    12590 1970-01-01 00:00:00.000000 classy-classification-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-19 12:52:23.708245 classy_classification-0.6.6/LICENSE
+-rw-r--r--   0        0        0    10736 2023-06-19 12:52:23.708245 classy_classification-0.6.6/README.md
+-rw-r--r--   0        0        0     2591 2023-06-19 12:52:23.708245 classy_classification-0.6.6/classy_classification/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:52:23.708245 classy_classification-0.6.6/classy_classification/classifiers/__init__.py
+-rw-r--r--   0        0        0    10545 2023-06-19 12:52:23.708245 classy_classification-0.6.6/classy_classification/classifiers/classy_skeleton.py
+-rw-r--r--   0        0        0     9186 2023-06-19 12:52:23.708245 classy_classification-0.6.6/classy_classification/classifiers/classy_spacy.py
+-rw-r--r--   0        0        0     2274 2023-06-19 12:52:23.708245 classy_classification-0.6.6/classy_classification/classifiers/classy_standalone.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:52:23.708245 classy_classification-0.6.6/classy_classification/examples/__init__.py
+-rw-r--r--   0        0        0     2324 2023-06-19 12:52:23.708245 classy_classification-0.6.6/classy_classification/examples/data.py
+-rw-r--r--   0        0        0      230 2023-06-19 12:52:23.708245 classy_classification-0.6.6/classy_classification/examples/individual_transformer.py
+-rw-r--r--   0        0        0      339 2023-06-19 12:52:23.708245 classy_classification-0.6.6/classy_classification/examples/spacy_few_shot_external.py
+-rw-r--r--   0        0        0      368 2023-06-19 12:52:23.708245 classy_classification-0.6.6/classy_classification/examples/spacy_internal_embeddings.py
+-rw-r--r--   0        0        0      372 2023-06-19 12:52:23.708245 classy_classification-0.6.6/classy_classification/examples/spacy_zero_shot_external.py
+-rw-r--r--   0        0        0     2353 2023-06-19 12:52:23.712245 classy_classification-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0    12441 1970-01-01 00:00:00.000000 classy_classification-0.6.6/PKG-INFO
```

### Comparing `classy-classification-0.6.5/LICENSE` & `classy_classification-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `classy-classification-0.6.5/README.md` & `classy_classification-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `classy-classification-0.6.5/classy_classification/__init__.py` & `classy_classification-0.6.6/classy_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `classy-classification-0.6.5/classy_classification/classifiers/classy_skeleton.py` & `classy_classification-0.6.6/classy_classification/classifiers/classy_skeleton.py`

 * *Files identical despite different names*

### Comparing `classy-classification-0.6.5/classy_classification/classifiers/classy_spacy.py` & `classy_classification-0.6.6/classy_classification/classifiers/classy_spacy.py`

 * *Files identical despite different names*

### Comparing `classy-classification-0.6.5/classy_classification/classifiers/classy_standalone.py` & `classy_classification-0.6.6/classy_classification/classifiers/classy_standalone.py`

 * *Files identical despite different names*

### Comparing `classy-classification-0.6.5/classy_classification/examples/data.py` & `classy_classification-0.6.6/classy_classification/examples/data.py`

 * *Files identical despite different names*

### Comparing `classy-classification-0.6.5/pyproject.toml` & `classy_classification-0.6.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "classy-classification"
-version = "0.6.5"
+version = "0.6.6"
 description = "Have you every struggled with needing a Spacy TextCategorizer but didn't have the time to train one from scratch? Classy Classification is the way to go!"
 authors = ["David Berenstein <david.m.berenstein@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/davidberenstein1957/classy-classification"
 repository = "https://github.com/davidberenstein1957/classy-classification"
 documentation = "https://github.com/davidberenstein1957/classy-classification"
```

### Comparing `classy-classification-0.6.5/PKG-INFO` & `classy_classification-0.6.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classy-classification
-Version: 0.6.5
+Version: 0.6.6
 Summary: Have you every struggled with needing a Spacy TextCategorizer but didn't have the time to train one from scratch? Classy Classification is the way to go!
 Home-page: https://github.com/davidberenstein1957/classy-classification
 License: MIT
 Keywords: spacy,rasa,few-shot classification,nlu,sentence-transformers
 Author: David Berenstein
 Author-email: david.m.berenstein@gmail.com
 Requires-Python: >=3.8,<3.12
@@ -13,24 +13,21 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Provides-Extra: onnx
-Requires-Dist: fast-sentence-transformers (>=0.4.1,<0.5.0); extra == "onnx"
-Requires-Dist: optimum[onnxruntime] (>=1.8.6,<2.0.0); extra == "onnx"
+Requires-Dist: fast-sentence-transformers (>=0.4.1,<0.5.0) ; extra == "onnx"
+Requires-Dist: optimum[onnxruntime] (>=1.8.6,<2.0.0) ; extra == "onnx"
 Requires-Dist: pandas (>=1.4,<2.0)
 Requires-Dist: scikit-learn (>=1.0,<2.0)
 Requires-Dist: sentence-transformers (>=2.0,<3.0)
 Requires-Dist: spacy[transformers] (>=3.0,<4.0)
 Requires-Dist: transformers[torch] (>4.20)
 Project-URL: Documentation, https://github.com/davidberenstein1957/classy-classification
 Project-URL: Repository, https://github.com/davidberenstein1957/classy-classification
```

