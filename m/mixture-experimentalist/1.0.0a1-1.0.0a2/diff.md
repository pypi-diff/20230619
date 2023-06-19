# Comparing `tmp/mixture_experimentalist-1.0.0a1.tar.gz` & `tmp/mixture_experimentalist-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixture_experimentalist-1.0.0a1.tar", last modified: Sat Jun 17 09:52:50 2023, max compression
+gzip compressed data, was "mixture_experimentalist-1.0.0a2.tar", last modified: Mon Jun 19 13:20:58 2023, max compression
```

## Comparing `mixture_experimentalist-1.0.0a1.tar` & `mixture_experimentalist-1.0.0a2.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-17 09:52:50.890619 mixture_experimentalist-1.0.0a1/
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-17 09:52:50.875527 mixture_experimentalist-1.0.0a1/.github/
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-17 09:52:50.880127 mixture_experimentalist-1.0.0a1/.github/workflows/
--rw-r--r--   0 marinadubova   (503) staff       (20)     1077 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a1/.github/workflows/python-publish.yml
--rw-r--r--   0 marinadubova   (503) staff       (20)      938 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a1/.gitignore
--rw-r--r--   0 marinadubova   (503) staff       (20)      674 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a1/.pre-commit-config.yaml
--rw-r--r--   0 marinadubova   (503) staff       (20)     1070 2023-05-24 16:18:58.000000 mixture_experimentalist-1.0.0a1/LICENSE
--rw-r--r--   0 marinadubova   (503) staff       (20)     2657 2023-06-17 09:52:50.890026 mixture_experimentalist-1.0.0a1/PKG-INFO
--rw-r--r--   0 marinadubova   (503) staff       (20)     1963 2023-06-16 19:37:48.000000 mixture_experimentalist-1.0.0a1/README.md
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-17 09:52:50.883323 mixture_experimentalist-1.0.0a1/docs/
--rw-r--r--   0 marinadubova   (503) staff       (20)      568 2023-06-16 19:46:14.000000 mixture_experimentalist-1.0.0a1/docs/additional-example.ipynb
--rw-r--r--   0 marinadubova   (503) staff       (20)   206990 2023-06-16 19:46:09.000000 mixture_experimentalist-1.0.0a1/docs/basic-usage.ipynb
--rw-r--r--   0 marinadubova   (503) staff       (20)      650 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a1/docs/index.md
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-17 09:52:50.883911 mixture_experimentalist-1.0.0a1/docs/javascripts/
--rw-r--r--   0 marinadubova   (503) staff       (20)      313 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a1/docs/javascripts/mathjax.js
--rw-r--r--   0 marinadubova   (503) staff       (20)      420 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a1/docs/quickstart.md
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-17 09:52:50.884452 mixture_experimentalist-1.0.0a1/mkdocs/
--rw-r--r--   0 marinadubova   (503) staff       (20)      729 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a1/mkdocs/base.yml
--rw-r--r--   0 marinadubova   (503) staff       (20)      435 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a1/mkdocs.yml
--rw-r--r--   0 marinadubova   (503) staff       (20)      973 2023-06-17 09:29:15.000000 mixture_experimentalist-1.0.0a1/pyproject.toml
--rw-r--r--   0 marinadubova   (503) staff       (20)       38 2023-06-17 09:52:50.890791 mixture_experimentalist-1.0.0a1/setup.cfg
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-17 09:52:50.877091 mixture_experimentalist-1.0.0a1/src/
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-17 09:52:50.876610 mixture_experimentalist-1.0.0a1/src/autora/
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-17 09:52:50.876752 mixture_experimentalist-1.0.0a1/src/autora/experimentalist/
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-17 09:52:50.876895 mixture_experimentalist-1.0.0a1/src/autora/experimentalist/sampler/
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-17 09:52:50.885000 mixture_experimentalist-1.0.0a1/src/autora/experimentalist/sampler/mixture_experimentalist/
--rw-r--r--   0 marinadubova   (503) staff       (20)     4274 2023-06-16 19:27:59.000000 mixture_experimentalist-1.0.0a1/src/autora/experimentalist/sampler/mixture_experimentalist/__init__.py
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-17 09:52:50.887752 mixture_experimentalist-1.0.0a1/src/mixture_experimentalist.egg-info/
--rw-r--r--   0 marinadubova   (503) staff       (20)     2657 2023-06-17 09:52:50.000000 mixture_experimentalist-1.0.0a1/src/mixture_experimentalist.egg-info/PKG-INFO
--rw-r--r--   0 marinadubova   (503) staff       (20)      642 2023-06-17 09:52:50.000000 mixture_experimentalist-1.0.0a1/src/mixture_experimentalist.egg-info/SOURCES.txt
--rw-r--r--   0 marinadubova   (503) staff       (20)        1 2023-06-17 09:52:50.000000 mixture_experimentalist-1.0.0a1/src/mixture_experimentalist.egg-info/dependency_links.txt
--rw-r--r--   0 marinadubova   (503) staff       (20)       49 2023-06-17 09:52:50.000000 mixture_experimentalist-1.0.0a1/src/mixture_experimentalist.egg-info/requires.txt
--rw-r--r--   0 marinadubova   (503) staff       (20)        7 2023-06-17 09:52:50.000000 mixture_experimentalist-1.0.0a1/src/mixture_experimentalist.egg-info/top_level.txt
-drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-17 09:52:50.889256 mixture_experimentalist-1.0.0a1/tests/
--rw-r--r--   0 marinadubova   (503) staff       (20)      841 2023-06-17 08:53:52.000000 mixture_experimentalist-1.0.0a1/tests/README.md
--rw-r--r--   0 marinadubova   (503) staff       (20)        0 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a1/tests/__init__.py
--rw-r--r--   0 marinadubova   (503) staff       (20)     1676 2023-06-17 08:46:35.000000 mixture_experimentalist-1.0.0a1/tests/test_mixture_experimentalist.py
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.361372 mixture_experimentalist-1.0.0a2/
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.343318 mixture_experimentalist-1.0.0a2/.github/
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.348810 mixture_experimentalist-1.0.0a2/.github/workflows/
+-rw-r--r--   0 marinadubova   (503) staff       (20)     1077 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a2/.github/workflows/python-publish.yml
+-rw-r--r--   0 marinadubova   (503) staff       (20)      938 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a2/.gitignore
+-rw-r--r--   0 marinadubova   (503) staff       (20)      674 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a2/.pre-commit-config.yaml
+-rw-r--r--   0 marinadubova   (503) staff       (20)     1070 2023-05-24 16:18:58.000000 mixture_experimentalist-1.0.0a2/LICENSE
+-rw-r--r--   0 marinadubova   (503) staff       (20)     2655 2023-06-19 13:20:58.360831 mixture_experimentalist-1.0.0a2/PKG-INFO
+-rw-r--r--   0 marinadubova   (503) staff       (20)     1961 2023-06-19 13:09:17.000000 mixture_experimentalist-1.0.0a2/README.md
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.353459 mixture_experimentalist-1.0.0a2/docs/
+-rw-r--r--   0 marinadubova   (503) staff       (20)   206968 2023-06-19 13:14:02.000000 mixture_experimentalist-1.0.0a2/docs/basic-usage.ipynb
+-rw-r--r--   0 marinadubova   (503) staff       (20)      491 2023-06-19 13:11:31.000000 mixture_experimentalist-1.0.0a2/docs/index.md
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.354181 mixture_experimentalist-1.0.0a2/docs/javascripts/
+-rw-r--r--   0 marinadubova   (503) staff       (20)      313 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a2/docs/javascripts/mathjax.js
+-rw-r--r--   0 marinadubova   (503) staff       (20)      420 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a2/docs/quickstart.md
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.355036 mixture_experimentalist-1.0.0a2/mkdocs/
+-rw-r--r--   0 marinadubova   (503) staff       (20)      729 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a2/mkdocs/base.yml
+-rw-r--r--   0 marinadubova   (503) staff       (20)      384 2023-06-19 13:09:17.000000 mixture_experimentalist-1.0.0a2/mkdocs.yml
+-rw-r--r--   0 marinadubova   (503) staff       (20)      973 2023-06-19 13:19:36.000000 mixture_experimentalist-1.0.0a2/pyproject.toml
+-rw-r--r--   0 marinadubova   (503) staff       (20)       38 2023-06-19 13:20:58.361515 mixture_experimentalist-1.0.0a2/setup.cfg
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.344870 mixture_experimentalist-1.0.0a2/src/
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.344394 mixture_experimentalist-1.0.0a2/src/autora/
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.344534 mixture_experimentalist-1.0.0a2/src/autora/experimentalist/
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.344699 mixture_experimentalist-1.0.0a2/src/autora/experimentalist/sampler/
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.355755 mixture_experimentalist-1.0.0a2/src/autora/experimentalist/sampler/mixture_experimentalist/
+-rw-r--r--   0 marinadubova   (503) staff       (20)     4273 2023-06-19 13:09:17.000000 mixture_experimentalist-1.0.0a2/src/autora/experimentalist/sampler/mixture_experimentalist/__init__.py
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.358089 mixture_experimentalist-1.0.0a2/src/mixture_experimentalist.egg-info/
+-rw-r--r--   0 marinadubova   (503) staff       (20)     2655 2023-06-19 13:20:58.000000 mixture_experimentalist-1.0.0a2/src/mixture_experimentalist.egg-info/PKG-INFO
+-rw-r--r--   0 marinadubova   (503) staff       (20)      612 2023-06-19 13:20:58.000000 mixture_experimentalist-1.0.0a2/src/mixture_experimentalist.egg-info/SOURCES.txt
+-rw-r--r--   0 marinadubova   (503) staff       (20)        1 2023-06-19 13:20:58.000000 mixture_experimentalist-1.0.0a2/src/mixture_experimentalist.egg-info/dependency_links.txt
+-rw-r--r--   0 marinadubova   (503) staff       (20)       49 2023-06-19 13:20:58.000000 mixture_experimentalist-1.0.0a2/src/mixture_experimentalist.egg-info/requires.txt
+-rw-r--r--   0 marinadubova   (503) staff       (20)        7 2023-06-19 13:20:58.000000 mixture_experimentalist-1.0.0a2/src/mixture_experimentalist.egg-info/top_level.txt
+drwxr-xr-x   0 marinadubova   (503) staff       (20)        0 2023-06-19 13:20:58.359852 mixture_experimentalist-1.0.0a2/tests/
+-rw-r--r--   0 marinadubova   (503) staff       (20)      841 2023-06-17 08:53:52.000000 mixture_experimentalist-1.0.0a2/tests/README.md
+-rw-r--r--   0 marinadubova   (503) staff       (20)        0 2023-05-24 16:20:27.000000 mixture_experimentalist-1.0.0a2/tests/__init__.py
+-rw-r--r--   0 marinadubova   (503) staff       (20)     1669 2023-06-19 13:09:17.000000 mixture_experimentalist-1.0.0a2/tests/test_mixture_experimentalist.py
```

### Comparing `mixture_experimentalist-1.0.0a1/.github/workflows/python-publish.yml` & `mixture_experimentalist-1.0.0a2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a1/.gitignore` & `mixture_experimentalist-1.0.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a1/.pre-commit-config.yaml` & `mixture_experimentalist-1.0.0a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a1/LICENSE` & `mixture_experimentalist-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a1/PKG-INFO` & `mixture_experimentalist-1.0.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture_experimentalist
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: The goal of this project is to examine the performance of a mixture experimentalist–a hybrid of different experimental sampling strategies–in terms of its ability to recover a ground-truth model from synthetic data.
 Author-email: Marina Dubova <marina.dubova.97@gmail.com>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/blinodelka/mixture_experimental_strategies
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
@@ -29,15 +29,15 @@
 ```bash
 pip install -U autora["mixture_experimentalist"]
 ```
 
 Check your installation by running:
 
 ```bash
-python -c "from autora.experimentalist.sampler.mixture_experimentalist import mixture_sampler"
+python -c "from autora.experimentalist.sampler.mixture_experimentalist import mixture_sample"
 ```
 
 ## Usage
 
 The Mixture Experimentalist can be used to select experimental conditions based on a mixture of different strategies. Here's a basic example:
 
 ```python
@@ -46,15 +46,15 @@
 # Define your condition pool, temperature, samplers, and parameters
 condition_pool = ...
 temperature = ...
 samplers = ...
 params = ...
 
 # Use the mixture_sampler to select conditions
-selected_conditions = mixture_sampler(
+selected_conditions = mixture_sample(
     condition_pool=condition_pool,
     temperature=temperature,
     samplers=samplers,
     params=params,
     num_samples=10
 )
 ```
```

### Comparing `mixture_experimentalist-1.0.0a1/README.md` & `mixture_experimentalist-1.0.0a2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ```bash
 pip install -U autora["mixture_experimentalist"]
 ```
 
 Check your installation by running:
 
 ```bash
-python -c "from autora.experimentalist.sampler.mixture_experimentalist import mixture_sampler"
+python -c "from autora.experimentalist.sampler.mixture_experimentalist import mixture_sample"
 ```
 
 ## Usage
 
 The Mixture Experimentalist can be used to select experimental conditions based on a mixture of different strategies. Here's a basic example:
 
 ```python
@@ -32,15 +32,15 @@
 # Define your condition pool, temperature, samplers, and parameters
 condition_pool = ...
 temperature = ...
 samplers = ...
 params = ...
 
 # Use the mixture_sampler to select conditions
-selected_conditions = mixture_sampler(
+selected_conditions = mixture_sample(
     condition_pool=condition_pool,
     temperature=temperature,
     samplers=samplers,
     params=params,
     num_samples=10
 )
 ```
```

### Comparing `mixture_experimentalist-1.0.0a1/docs/basic-usage.ipynb` & `mixture_experimentalist-1.0.0a2/docs/basic-usage.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998592509920635%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Basic Usage\\n'), (2, 'The goal of this notebook is "*

 * *            'to demonstrate the usage of the `mixture_sample` function, which combines different '*

 * *            'sampling strategies to select experimental conditions. The `mixture_sample` function '*

 * *            'takes a pool of experimental conditions, a temperature parameter, a list of samplers '*

 * *            'with their weights, a dictionary of parameters for the samplers, and an optional '*

 * *            "numbe […]*

```diff
@@ -1,16 +1,16 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Mixture Sampler Basic Usage\n",
+                "# Basic Usage\n",
                 "\n",
-                "The goal of this notebook is to demonstrate the usage of the `mixture_sampler` function, which combines different sampling strategies to select experimental conditions. The `mixture_sampler` function takes a pool of experimental conditions, a temperature parameter, a list of samplers with their weights, a dictionary of parameters for the samplers, and an optional number of samples to return.\n",
+                "The goal of this notebook is to demonstrate the usage of the `mixture_sample` function, which combines different sampling strategies to select experimental conditions. The `mixture_sample` function takes a pool of experimental conditions, a temperature parameter, a list of samplers with their weights, a dictionary of parameters for the samplers, and an optional number of samples to return.\n",
                 "\n",
                 "We begin with importing the necessary packages."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
@@ -27,15 +27,15 @@
                         "\u001b[0;31mModuleNotFoundError\u001b[0m                       Traceback (most recent call last)",
                         "Cell \u001b[0;32mIn[2], line 1\u001b[0m\n\u001b[0;32m----> 1\u001b[0m \u001b[38;5;28;01mfrom\u001b[39;00m \u001b[38;5;21;01mautora\u001b[39;00m\u001b[38;5;21;01m.\u001b[39;00m\u001b[38;5;21;01mexperimentalist\u001b[39;00m\u001b[38;5;21;01m.\u001b[39;00m\u001b[38;5;21;01msampler\u001b[39;00m\u001b[38;5;21;01m.\u001b[39;00m\u001b[38;5;21;01mmixture_experimentalist\u001b[39;00m \u001b[38;5;28;01mimport\u001b[39;00m mixture_sampler\n",
                         "\u001b[0;31mModuleNotFoundError\u001b[0m: No module named 'autora.experimentalist.sampler.mixture_experimentalist'"
                     ]
                 }
             ],
             "source": [
-                "from autora.experimentalist.sampler.mixture_experimentalist import mixture_sampler"
+                "from autora.experimentalist.sampler.mixture_experimentalist import mixture_sample"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 132,
             "metadata": {},
             "outputs": [],
@@ -132,15 +132,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": 140,
             "metadata": {},
             "outputs": [],
             "source": [
-                "selected_conditions = mixture_sampler(\n",
+                "selected_conditions = mixture_sample(\n",
                 "    condition_pool=new_X,\n",
                 "    temperature=0.01,\n",
                 "    samplers=[[novelty_score_sample, \"novelty\", [0.8, 0.2]]],\n",
                 "    params=params,\n",
                 "    num_samples=10\n",
                 ")"
             ]
@@ -217,15 +217,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": 144,
             "metadata": {},
             "outputs": [],
             "source": [
-                "selected_conditions = mixture_sampler(\n",
+                "selected_conditions = mixture_sample(\n",
                 "    condition_pool=new_X,\n",
                 "    temperature=2,\n",
                 "    samplers=[[novelty_score_sample, \"novelty\", [0.8, 0.2]]],\n",
                 "    params=params,\n",
                 "    num_samples=10\n",
                 ")"
             ]
@@ -347,15 +347,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": 149,
             "metadata": {},
             "outputs": [],
             "source": [
-                "selected_conditions = mixture_sampler(\n",
+                "selected_conditions = mixture_sample(\n",
                 "    condition_pool=new_X,\n",
                 "    temperature=0.01,\n",
                 "    samplers=[[novelty_score_sample, \"novelty\", [0.7, 0.1]], [falsification_score_sampler, \"falsification\", [0.5, 0]]],\n",
                 "    params=params,\n",
                 "    num_samples=10\n",
                 ")"
             ]
```

### Comparing `mixture_experimentalist-1.0.0a1/mkdocs/base.yml` & `mixture_experimentalist-1.0.0a2/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a1/pyproject.toml` & `mixture_experimentalist-1.0.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 # UPDATE THIS BEFORE PUBLISHING
 name = "mixture_experimentalist"
 description = "The goal of this project is to examine the performance of a mixture experimentalist–a hybrid of different experimental sampling strategies–in terms of its ability to recover a ground-truth model from synthetic data."
 authors = [{ name = "Marina Dubova", email = "marina.dubova.97@gmail.com" }]
-version = "1.0.0a1"
+version = "1.0.0a2"
 
 readme = "README.md"
 license = { text = "MIT license" }
 requires-python = ">=3.8,<4"
 
 # ADD NEW DEPENDENCIES HERE
 dependencies = [
```

### Comparing `mixture_experimentalist-1.0.0a1/src/autora/experimentalist/sampler/mixture_experimentalist/__init__.py` & `mixture_experimentalist-1.0.0a2/src/autora/experimentalist/sampler/mixture_experimentalist/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         p = np.exp(p / temperature)  
         final_p = p / np.sum(p) # Normalizing the final distribution
         return final_p
 
 
 
     
-def mixture_sampler(condition_pool: np.ndarray, temperature: float, samplers: list, params: dict, num_samples: Optional[int] = None) -> np.ndarray:
+def mixture_sample(condition_pool: np.ndarray, temperature: float, samplers: list, params: dict, num_samples: Optional[int] = None) -> np.ndarray:
     """
 
     Args:
         condition_pool: pool of experimental conditions to evaluate
         temperature: how random is selection of conditions (cannot be 0; (0:1) - the choices are more deterministic than the choices made wrt
         samplers: tuple containing sampler functions, their names, and weights 
         for sampler functions that return both positive and negative scores, user can provide a list with two weights: the first one will be applied to positive scores, the second one -- to the negative
```

### Comparing `mixture_experimentalist-1.0.0a1/src/mixture_experimentalist.egg-info/PKG-INFO` & `mixture_experimentalist-1.0.0a2/src/mixture_experimentalist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-experimentalist
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: The goal of this project is to examine the performance of a mixture experimentalist–a hybrid of different experimental sampling strategies–in terms of its ability to recover a ground-truth model from synthetic data.
 Author-email: Marina Dubova <marina.dubova.97@gmail.com>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/blinodelka/mixture_experimental_strategies
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
@@ -29,15 +29,15 @@
 ```bash
 pip install -U autora["mixture_experimentalist"]
 ```
 
 Check your installation by running:
 
 ```bash
-python -c "from autora.experimentalist.sampler.mixture_experimentalist import mixture_sampler"
+python -c "from autora.experimentalist.sampler.mixture_experimentalist import mixture_sample"
 ```
 
 ## Usage
 
 The Mixture Experimentalist can be used to select experimental conditions based on a mixture of different strategies. Here's a basic example:
 
 ```python
@@ -46,15 +46,15 @@
 # Define your condition pool, temperature, samplers, and parameters
 condition_pool = ...
 temperature = ...
 samplers = ...
 params = ...
 
 # Use the mixture_sampler to select conditions
-selected_conditions = mixture_sampler(
+selected_conditions = mixture_sample(
     condition_pool=condition_pool,
     temperature=temperature,
     samplers=samplers,
     params=params,
     num_samples=10
 )
 ```
```

### Comparing `mixture_experimentalist-1.0.0a1/src/mixture_experimentalist.egg-info/SOURCES.txt` & `mixture_experimentalist-1.0.0a2/src/mixture_experimentalist.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
 mkdocs.yml
 pyproject.toml
 .github/workflows/python-publish.yml
-docs/additional-example.ipynb
 docs/basic-usage.ipynb
 docs/index.md
 docs/quickstart.md
 docs/javascripts/mathjax.js
 mkdocs/base.yml
 src/autora/experimentalist/sampler/mixture_experimentalist/__init__.py
 src/mixture_experimentalist.egg-info/PKG-INFO
```

### Comparing `mixture_experimentalist-1.0.0a1/tests/README.md` & `mixture_experimentalist-1.0.0a2/tests/README.md`

 * *Files identical despite different names*

### Comparing `mixture_experimentalist-1.0.0a1/tests/test_mixture_experimentalist.py` & `mixture_experimentalist-1.0.0a2/tests/test_mixture_experimentalist.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from autora.experimentalist.sampler.mixture_experimentalist import mixture_sampler
+from autora.experimentalist.sampler.mixture_experimentalist import mixture_sample
 import numpy as np
 import pytest
 
 def mock_sampler(condition_pool, **kwargs):
     return condition_pool, np.random.rand(len(condition_pool))
 
-def test_mixture_sampler():
+def test_mixture_sample():
     condition_pool = np.array([1, 2, 3, 4, 5])
     temperature = 0.5
     samplers = [[mock_sampler, "mock", 1]]
     params = {"mock": {}}
 
     # Test that the function runs without errors
-    conditions = mixture_sampler(condition_pool, temperature, samplers, params)
+    conditions = mixture_sample(condition_pool, temperature, samplers, params)
     assert conditions is not None
 
     # Test that the function returns the correct number of samples
-    conditions = mixture_sampler(condition_pool, temperature, samplers, params, num_samples=2)
+    conditions = mixture_sample(condition_pool, temperature, samplers, params, num_samples=2)
     assert len(conditions) == 2
 
     # Test that the function returns unique samples when replace=False
-    conditions = mixture_sampler(condition_pool, temperature, samplers, params, num_samples=len(condition_pool))
+    conditions = mixture_sample(condition_pool, temperature, samplers, params, num_samples=len(condition_pool))
     assert len(conditions) == len(set(conditions))
 
     # Test that the function raises an error when temperature is 0
     with pytest.raises(AssertionError):
-        conditions = mixture_sampler(condition_pool, 0, samplers, params)
+        conditions = mixture_sample(condition_pool, 0, samplers, params)
 
     # Test that the function raises an error when num_samples is greater than the size of the condition pool
     with pytest.raises(ValueError):
-        conditions = mixture_sampler(condition_pool, temperature, samplers, params, num_samples=len(condition_pool) + 1)
+        conditions = mixture_sample(condition_pool, temperature, samplers, params, num_samples=len(condition_pool) + 1)
 
     # Test that the function raises an error when a sampler is not provided in the samplers list
     with pytest.raises(KeyError):
-        conditions = mixture_sampler(condition_pool, temperature, [[mock_sampler, "nonexistent", 1]], params)
+        conditions = mixture_sample(condition_pool, temperature, [[mock_sampler, "nonexistent", 1]], params)
```

