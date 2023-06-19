# Comparing `tmp/pybefit-0.1.21.tar.gz` & `tmp/pybefit-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybefit-0.1.21.tar", last modified: Tue May  9 14:24:09 2023, max compression
+gzip compressed data, was "pybefit-0.1.22.tar", last modified: Mon Jun 19 15:32:05 2023, max compression
```

## Comparing `pybefit-0.1.21.tar` & `pybefit-0.1.22.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.784801 pybefit-0.1.21/
--rw-r--r--   0 dima      (1000) dima      (1000)     1114 2023-01-22 14:03:59.000000 pybefit-0.1.21/LICENSE.md
--rw-r--r--   0 dima      (1000) dima      (1000)      461 2023-05-09 14:24:09.784801 pybefit-0.1.21/PKG-INFO
--rw-r--r--   0 dima      (1000) dima      (1000)     2996 2023-01-22 14:03:59.000000 pybefit-0.1.21/README.md
--rw-r--r--   0 dima      (1000) dima      (1000)       79 2023-05-09 14:24:09.784801 pybefit-0.1.21/setup.cfg
--rw-r--r--   0 dima      (1000) dima      (1000)     1433 2023-05-09 14:17:55.000000 pybefit-0.1.21/setup.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.781467 pybefit-0.1.21/src/
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.781467 pybefit-0.1.21/src/pybefit/
--rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-04-21 16:18:55.000000 pybefit-0.1.21/src/pybefit/__init__.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.781467 pybefit-0.1.21/src/pybefit/agents/
--rwxr--r--   0 dima      (1000) dima      (1000)       19 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/agents/__init__.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     1414 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/agents/base.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.781467 pybefit-0.1.21/src/pybefit/agents/jax/
--rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/agents/jax/__init__.py
--rw-r--r--   0 dima      (1000) dima      (1000)     6438 2023-01-22 14:03:59.000000 pybefit-0.1.21/src/pybefit/agents/jax/hsmm_ai.py
--rw-r--r--   0 dima      (1000) dima      (1000)      337 2023-01-22 14:03:59.000000 pybefit-0.1.21/src/pybefit/agents/jax/utils.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.784801 pybefit-0.1.21/src/pybefit/agents/torch/
--rw-r--r--   0 dima      (1000) dima      (1000)      130 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/agents/torch/__init__.py
--rwxr--r--   0 dima      (1000) dima      (1000)    13071 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/agents/torch/active_inference.py
--rwxr--r--   0 dima      (1000) dima      (1000)    21780 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/agents/torch/bayesian.py
--rw-r--r--   0 dima      (1000) dima      (1000)    22613 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/agents/torch/dynamic_programming.py
--rw-r--r--   0 dima      (1000) dima      (1000)     1190 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/agents/torch/random.py
--rwxr--r--   0 dima      (1000) dima      (1000)     5247 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/agents/torch/rl.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.784801 pybefit-0.1.21/src/pybefit/inference/
--rwxr--r--   0 dima      (1000) dima      (1000)       92 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/__init__.py
--rwxr--r--   0 dima      (1000) dima      (1000)    10154 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/methods.py
--rw-r--r--   0 dima      (1000) dima      (1000)     1610 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/models.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.784801 pybefit-0.1.21/src/pybefit/inference/numpyro/
--rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/numpyro/__init__.py
--rw-r--r--   0 dima      (1000) dima      (1000)     1500 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/numpyro/likelihoods.py
--rw-r--r--   0 dima      (1000) dima      (1000)     6507 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/numpyro/regression.py
--rw-r--r--   0 dima      (1000) dima      (1000)     5429 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/posteriors.py
--rw-r--r--   0 dima      (1000) dima      (1000)     5904 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/priors.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.784801 pybefit-0.1.21/src/pybefit/inference/pyro/
--rw-r--r--   0 dima      (1000) dima      (1000)       20 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/pyro/__init__.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     4860 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/pyro/flat.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)    10394 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/pyro/hierarchical.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     8701 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/pyro/infer.py
--rw-r--r--   0 dima      (1000) dima      (1000)     1008 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/pyro/likelihoods.py
--rw-r--r--   0 dima      (1000) dima      (1000)     6139 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/pyro/mixed.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     8109 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/pyro/nonparametric.py
--rw-r--r--   0 dima      (1000) dima      (1000)     6575 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/regression.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     2916 2023-01-22 14:03:59.000000 pybefit-0.1.21/src/pybefit/simulate.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.784801 pybefit-0.1.21/src/pybefit/tasks/
--rwxr-xr-x   0 dima      (1000) dima      (1000)       59 2023-01-22 14:03:59.000000 pybefit-0.1.21/src/pybefit/tasks/__init__.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     4136 2023-01-22 14:03:59.000000 pybefit-0.1.21/src/pybefit/tasks/bandits.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     2650 2023-01-22 14:03:59.000000 pybefit-0.1.21/src/pybefit/tasks/rev_learning.py
--rw-r--r--   0 dima      (1000) dima      (1000)     3716 2023-01-22 14:03:59.000000 pybefit-0.1.21/src/pybefit/tasks/sat.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.781467 pybefit-0.1.21/src/pybefit.egg-info/
--rw-r--r--   0 dima      (1000) dima      (1000)      461 2023-05-09 14:24:09.000000 pybefit-0.1.21/src/pybefit.egg-info/PKG-INFO
--rw-r--r--   0 dima      (1000) dima      (1000)     1380 2023-05-09 14:24:09.000000 pybefit-0.1.21/src/pybefit.egg-info/SOURCES.txt
--rw-r--r--   0 dima      (1000) dima      (1000)        1 2023-05-09 14:24:09.000000 pybefit-0.1.21/src/pybefit.egg-info/dependency_links.txt
--rw-r--r--   0 dima      (1000) dima      (1000)      104 2023-05-09 14:24:09.000000 pybefit-0.1.21/src/pybefit.egg-info/requires.txt
--rw-r--r--   0 dima      (1000) dima      (1000)        8 2023-05-09 14:24:09.000000 pybefit-0.1.21/src/pybefit.egg-info/top_level.txt
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.661570 pybefit-0.1.22/
+-rw-r--r--   0 dima      (1000) dima      (1000)     1114 2023-01-22 14:03:59.000000 pybefit-0.1.22/LICENSE.md
+-rw-r--r--   0 dima      (1000) dima      (1000)      461 2023-06-19 15:32:05.661570 pybefit-0.1.22/PKG-INFO
+-rw-r--r--   0 dima      (1000) dima      (1000)     2996 2023-01-22 14:03:59.000000 pybefit-0.1.22/README.md
+-rw-r--r--   0 dima      (1000) dima      (1000)       79 2023-06-19 15:32:05.664903 pybefit-0.1.22/setup.cfg
+-rw-r--r--   0 dima      (1000) dima      (1000)     1433 2023-06-19 15:30:30.000000 pybefit-0.1.22/setup.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.658237 pybefit-0.1.22/src/
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.658237 pybefit-0.1.22/src/pybefit/
+-rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-04-21 16:18:55.000000 pybefit-0.1.22/src/pybefit/__init__.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.661570 pybefit-0.1.22/src/pybefit/agents/
+-rwxr-xr-x   0 dima      (1000) dima      (1000)       40 2023-06-13 14:22:04.000000 pybefit-0.1.22/src/pybefit/agents/__init__.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)     1901 2023-06-19 15:19:44.000000 pybefit-0.1.22/src/pybefit/agents/base.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.661570 pybefit-0.1.22/src/pybefit/agents/jax/
+-rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/agents/jax/__init__.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     6438 2023-01-22 14:03:59.000000 pybefit-0.1.22/src/pybefit/agents/jax/hsmm_ai.py
+-rw-r--r--   0 dima      (1000) dima      (1000)      337 2023-01-22 14:03:59.000000 pybefit-0.1.22/src/pybefit/agents/jax/utils.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.661570 pybefit-0.1.22/src/pybefit/agents/torch/
+-rw-r--r--   0 dima      (1000) dima      (1000)      130 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/agents/torch/__init__.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)    13071 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/agents/torch/active_inference.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)    21780 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/agents/torch/bayesian.py
+-rw-r--r--   0 dima      (1000) dima      (1000)    22613 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/agents/torch/dynamic_programming.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     1190 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/agents/torch/random.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)     5247 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/agents/torch/rl.py
+-rw-r--r--   0 dima      (1000) dima      (1000)      484 2023-06-14 07:55:30.000000 pybefit-0.1.22/src/pybefit/agents/utils.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.661570 pybefit-0.1.22/src/pybefit/inference/
+-rwxr-xr-x   0 dima      (1000) dima      (1000)       92 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/__init__.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)    10166 2023-06-19 11:01:13.000000 pybefit-0.1.22/src/pybefit/inference/methods.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     1610 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/models.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.661570 pybefit-0.1.22/src/pybefit/inference/numpyro/
+-rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/numpyro/__init__.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     4114 2023-06-19 14:30:28.000000 pybefit-0.1.22/src/pybefit/inference/numpyro/likelihoods.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     6507 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/numpyro/regression.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     5489 2023-06-19 10:51:25.000000 pybefit-0.1.22/src/pybefit/inference/posteriors.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     5906 2023-06-19 10:40:53.000000 pybefit-0.1.22/src/pybefit/inference/priors.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.661570 pybefit-0.1.22/src/pybefit/inference/pyro/
+-rw-r--r--   0 dima      (1000) dima      (1000)       20 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/pyro/__init__.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)     4860 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/pyro/flat.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)    10394 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/pyro/hierarchical.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)     8701 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/pyro/infer.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     2580 2023-06-19 14:30:19.000000 pybefit-0.1.22/src/pybefit/inference/pyro/likelihoods.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     6139 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/pyro/mixed.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)     8109 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/pyro/nonparametric.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     6575 2023-04-21 16:18:01.000000 pybefit-0.1.22/src/pybefit/inference/regression.py
+-rwxr--r--   0 dima      (1000) dima      (1000)     2916 2023-01-22 14:03:59.000000 pybefit-0.1.22/src/pybefit/simulate.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.661570 pybefit-0.1.22/src/pybefit/tasks/
+-rwxr--r--   0 dima      (1000) dima      (1000)       78 2023-06-13 14:32:29.000000 pybefit-0.1.22/src/pybefit/tasks/__init__.py
+-rwxr--r--   0 dima      (1000) dima      (1000)     4230 2023-06-13 14:55:44.000000 pybefit-0.1.22/src/pybefit/tasks/bandits.py
+-rw-r--r--   0 dima      (1000) dima      (1000)      798 2023-06-13 16:41:50.000000 pybefit-0.1.22/src/pybefit/tasks/base.py
+-rwxr--r--   0 dima      (1000) dima      (1000)     2594 2023-06-13 15:22:54.000000 pybefit-0.1.22/src/pybefit/tasks/rev_learning.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     3722 2023-06-13 15:04:34.000000 pybefit-0.1.22/src/pybefit/tasks/sat.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-06-19 15:32:05.661570 pybefit-0.1.22/src/pybefit.egg-info/
+-rw-r--r--   0 dima      (1000) dima      (1000)      461 2023-06-19 15:32:05.000000 pybefit-0.1.22/src/pybefit.egg-info/PKG-INFO
+-rw-r--r--   0 dima      (1000) dima      (1000)     1434 2023-06-19 15:32:05.000000 pybefit-0.1.22/src/pybefit.egg-info/SOURCES.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)        1 2023-06-19 15:32:05.000000 pybefit-0.1.22/src/pybefit.egg-info/dependency_links.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)      104 2023-06-19 15:32:05.000000 pybefit-0.1.22/src/pybefit.egg-info/requires.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)        8 2023-06-19 15:32:05.000000 pybefit-0.1.22/src/pybefit.egg-info/top_level.txt
```

### Comparing `pybefit-0.1.21/LICENSE.md` & `pybefit-0.1.22/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.21/README.md` & `pybefit-0.1.22/README.md`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.21/setup.py` & `pybefit-0.1.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     'Topic :: Scientific/Engineering',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.10'
 ]
 
 setup_kwargs = {
     'name': 'pybefit',
-    'version': '0.1.21',
+    'version': '0.1.22',
     'description': 'Probabilistic inference for models of behaviour',
     'long_description': 'PyBefit is a Python library for Bayesian analysis of behavioral data. It is based on Pyro/Numpyro a probabilistic programing language, PyTorch, and Jax machine learning libraries.',
     'author': 'Dimitrije Marković',
     'author_email': 'dimitrije.markovic@tu-dresden.de',
     'url': 'https://github.com/dimarkov/pybefit',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `pybefit-0.1.21/src/pybefit/agents/jax/hsmm_ai.py` & `pybefit-0.1.22/src/pybefit/agents/jax/hsmm_ai.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.21/src/pybefit/agents/torch/active_inference.py` & `pybefit-0.1.22/src/pybefit/agents/torch/active_inference.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.21/src/pybefit/agents/torch/bayesian.py` & `pybefit-0.1.22/src/pybefit/agents/torch/bayesian.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.21/src/pybefit/agents/torch/dynamic_programming.py` & `pybefit-0.1.22/src/pybefit/agents/torch/dynamic_programming.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.21/src/pybefit/agents/torch/random.py` & `pybefit-0.1.22/src/pybefit/agents/torch/random.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.21/src/pybefit/agents/torch/rl.py` & `pybefit-0.1.22/src/pybefit/agents/torch/rl.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.21/src/pybefit/inference/methods.py` & `pybefit-0.1.22/src/pybefit/inference/methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,39 +94,45 @@
     }
 
     pred = pinfer.Predictive(model, guide=guide, **opts['sample_kwargs'])
     samples = pred(data)
 
     return samples, svi, results
 
+default_dict_nuts = dict(
+    seed=0,
+    num_samples=1000,            
+    num_warmup=100,
+    sampler_kwargs={
+        'kernel': {}, 
+        'mcmc': {}
+    }
+)
 
-@dispatch(PyroModel, opts=dict)
+@dispatch(PyroModel, dict, opts=dict)
 def run_nuts(
     model,
+    data,
     *,
-    opts=dict(
-        num_samples=1000,            
-        num_warmup=100,
-        sampler_kwargs={'kernel': {}, 'mcmc': {}}
-    )
+    opts=default_dict_nuts
 ):
     """Perform SVI over free model parameters.
     """
 
     clear_param_store()
 
     kernel = pinfer.NUTS(model, **opts['sampler_kwargs']['kernel'])
     mcmc = pinfer.MCMC(
         kernel, 
         opts['num_samples'], 
         warmup_steps=opts['num_warmup'],
         **opts['sampler_kwargs']['mcmc']
     )
 
-    mcmc.run()
+    mcmc.run(data=data)
     samples = mcmc.get_samples()
 
     return samples, mcmc
 
 
 default_dict_numpyro_svi = dict(
     seed=0,
@@ -177,35 +183,28 @@
         progress_bar=opts['svi_kwargs']['progress_bar'],
         stable_update=opts['svi_kwargs']['stable_update'],
         init_state = opts['svi_kwargs'].pop('init_state', None),
         data=data
     )
 
     rng_key, _rng_key = jr.split(rng_key)
-    pred = ninfer.Predictive(model, guide=guide, params=results.params, **opts['sample_kwargs'])
-    samples = pred(_rng_key, data=data)
+    pred = ninfer.Predictive(guide, params=results.params, **opts['sample_kwargs'])
+    posterior_samples = pred(_rng_key, data=data)
 
-    return samples, svi, results
+    pred = ninfer.Predictive(model, posterior_samples=posterior_samples)
+    samples = pred(_rng_key, data=data)
 
-default_dict_numpyro_nuts = dict(
-    seed=0,
-    num_samples=1000,            
-    num_warmup=100,
-    sampler_kwargs={
-        'kernel': {}, 
-        'mcmc': dict(progress_bar=True)
-    }
-)
+    return samples | posterior_samples, svi, results
 
 @dispatch(NumpyroModel, dict, opts=dict)
 def run_nuts(
     model,
     data,
     *,
-    opts=default_dict_numpyro_nuts
+    opts=default_dict_nuts
 ):
     """Estimate posterior over free model parameters using No-U-Turn sampler.
     """
     rng_key = jr.PRNGKey(opts['seed'])
 
     kernel = ninfer.NUTS(model, **opts['sampler_kwargs']['kernel'])
     mcmc = ninfer.MCMC(
```

### Comparing `pybefit-0.1.21/src/pybefit/inference/models.py` & `pybefit-0.1.22/src/pybefit/inference/models.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.21/src/pybefit/inference/numpyro/regression.py` & `pybefit-0.1.22/src/pybefit/inference/numpyro/regression.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.21/src/pybefit/inference/posteriors.py` & `pybefit-0.1.22/src/pybefit/inference/posteriors.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,18 @@
 from .priors import ModelBase
 
 
 class NormalPosterior(ModelBase):
     """A flat Normal prior over free model parameters.
     """
     
-    def __init__(self, num_params, num_agents, backend=BACKEND):
+    def __init__(self, num_params, num_agents, init_scale=.1, backend=BACKEND):
         super().__init__(num_params=num_params, num_agents=num_agents, backend=backend)
-
+        self.init_scale = init_scale
+        
     def __call__(self, *args, **kwargs):
         na = self.num_agents
         np = self.num_params
         
         # posterior distribution over subject specific model parameters
         with self.plate('agents', na):
             loc = self.param('loc', self.tensor.zeros((na, np)))
```

### Comparing `pybefit-0.1.21/src/pybefit/inference/priors.py` & `pybefit-0.1.22/src/pybefit/inference/priors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 try:
     import numpyro as npyro
     import numpyro.distributions as ndist
     from numpyro import handlers
     from numpyro.infer import reparam as npyro_reparam
     
     BACKEND = 'numpyro'  # default backend
@@ -92,25 +91,25 @@
 
         return z
 
 
 class NormalGamma(ModelBase):
     """NormalGamma over free model parameters.
     """
-    def __init__(self, num_params, num_agents, init_scale=10., backend=BACKEND):
+    def __init__(self, num_params, num_agents, init_scale=1., backend=BACKEND):
         super().__init__(num_params=num_params, num_agents=num_agents, backend=backend)
         self.init_scale = init_scale
 
     def __call__(self, *args, **kwargs):
         na = self.num_agents
         np = self.num_params
 
         # define hyper priors over model parameters
         a = 2 * self.tensor.ones(np)
-        b = self.tensor.ones(np)
+        b = 2 * self.tensor.ones(np)
         tau = self.sample('var_tau', self.dist.Gamma(a, b).to_event(1))
 
         # prior uncertainty is sampled from inverse gamma distribution for each parameter
         sigma = self.deterministic('sigma', self.tensor.sqrt(1/tau)) 
 
         # normal-gamma prior has two hyperparameters which are jointly optimized with 
         # the parameters of the approximate posterior in the case of stochastic variational inference
```

### Comparing `pybefit-0.1.21/src/pybefit/inference/pyro/flat.py` & `pybefit-0.1.22/src/pybefit/inference/pyro/flat.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.21/src/pybefit/inference/pyro/hierarchical.py` & `pybefit-0.1.22/src/pybefit/inference/pyro/hierarchical.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.21/src/pybefit/inference/pyro/infer.py` & `pybefit-0.1.22/src/pybefit/inference/pyro/infer.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.21/src/pybefit/inference/pyro/mixed.py` & `pybefit-0.1.22/src/pybefit/inference/pyro/mixed.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.21/src/pybefit/inference/pyro/nonparametric.py` & `pybefit-0.1.22/src/pybefit/inference/pyro/nonparametric.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.21/src/pybefit/inference/regression.py` & `pybefit-0.1.22/src/pybefit/inference/regression.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.21/src/pybefit/simulate.py` & `pybefit-0.1.22/src/pybefit/simulate.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.21/src/pybefit/tasks/bandits.py` & `pybefit-0.1.22/src/pybefit/tasks/bandits.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,44 +7,41 @@
 Created on Thu Feb  22 14:50:01 2018
 
 @author: Dimitrije Markovic
 """
 import torch
 from torch import zeros, ones
 from torch.distributions import Categorical, Multinomial, Dirichlet
+from .base import Task
 
 __all__ = [
         'MultiArmedBandit'
 ]
 
-class MultiArmedBandit(object):
+class MultiArmedBandit(Task):
     """Implementation of a multi-armed bandit task. Bandit has K arms, each associated 
        with specific probability of delivering different outcomes.
     """
     
-    def __init__(self, priors, transitions, context, offers, arm_types, states=None, nsub=1, blocks=1, trials=100):
+    def __init__(self, priors, transitions, offers, arm_types, states=None, nsub=1, blocks=1, trials=100):
+
+        super().__init__(nsub, blocks, trials)
         
         self.priors = priors  # prior probabilities
-        self.tms = transitions  # dictionary containing tranistion matrices
-        
-        self.blocks = blocks
-        self.trials = trials
-        self.nsub = nsub
+        self.tms = transitions  # dictionary containing transition matrices
         
         if states is not None:
-            self.states = states
-            self.fixed_states = 1
+            self.states = states  # provides a fixed list of states
+            self.fixed_states = True
         else:
-            self.fixed_states = 0
+            self.fixed_states = False
         
-        self.arm_types = arm_types
+        self.arm_types = arm_types  # defines possible arm_types for different offers and responses
     
-        self.context = context        
-        
-        self.offers = offers
+        self.offers = offers  # offers availible to the agent on a specific block and trial
         
         self.initialise()
     
     def initialise(self):
         if not self.fixed_states:
             blocks = self.blocks
             trials = self.trials
@@ -73,28 +70,28 @@
         if trial == 0:
             self.states['points'][block, trial] = 0
             
             if block == 0:
                 probs =  self.priors['probs']
                 self.states['probs'][block, trial] = probs
             else:
-                self.states['probs'][block, trial] = self.states['probs'][block-1, -1]
+                self.states['probs'][block, trial] = self.states['probs'][block - 1, -1]
                 
             self.states['locations'][block, trial] = Categorical(probs=self.priors['locations']).sample((self.nsub,))
         else:
             self.states['points'][block, trial] = self.states['points'][block, trial - 1] + outcomes.long()
             self.states['probs'][block, trial] = self.states['probs'][block, trial - 1]
             loc = self.states['locations'][block, trial - 1]
             self.states['locations'][block, trial] = \
                 Categorical(probs=self.tms['locations'][responses, loc]).sample()
         
         if trial < self.trials:
             return zeros(self.nsub)
         else:
-            success = torch.any(self.states['points'][block, trial, :, 1:] > 2*self.trials//3, -1)
+            success = torch.any(self.states['points'][block, trial, :, 1:] > 2*self.trials // 3, -1)
             return success.long()
         
     def update_environment(self, block, trial, responses):
         """Generate stimuli for the current block and trial and update the state
         """
 
         # offers in the current trial
```

### Comparing `pybefit-0.1.21/src/pybefit/tasks/rev_learning.py` & `pybefit-0.1.22/src/pybefit/tasks/rev_learning.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 This module contains various experimental environments used for testing
 human behavior.
 
-Created on Thu Feb  22 14:50:01 2018
-
 @author: Dimitrije Markovic
 """
 
 import torch
 from torch.distributions import Categorical
+from .base import Task
 
 __all__ = [
         'SocialInfluence',
         'TempRevLearn'
 ]
 
-class SocialInfluence(object):
+class SocialInfluence(Task):
     """Implementation of the social learning task
     """
 
-    def __init__(self, stimuli, nsub=1, blocks=1, trials=120):
-
-        self.trials = trials
-        self.nsub = nsub
+    def __init__(self, stimuli, nsub=1, trials=120):
+        super().__init__(nsub, 1, trials)
 
         # set stimuli
         self.stimuli = stimuli
 
 
     def get_offers(self, block, trial):
         offers = self.stimuli['offers'][block, trial]
@@ -48,22 +45,21 @@
         # position 1 - reward dependent on agents choice
 
         outcomes = torch.stack([reward_if_follow, reward[range(len(responses)), responses]], -1)
 
         return [responses, outcomes]
 
 
-class TempRevLearn(object):
+class TempRevLearn(Task):
     """Implementation of the temporal reversal learning task.
     """
 
-    def __init__(self, stimuli=None, nsub=1, blocks=1, trials=1000):
-        self.trials = trials
-        self.nsub = nsub
-
+    def __init__(self, stimuli=None, nsub=1, trials=1000):
+        super().__init__(nsub, 1, trials)
+        
         # set stimuli
         self.stimuli = stimuli
 
     def likelihood(self, block, trial, responses):
         raise NotImplementedError
 
     def update_states(self, block, trial):
```

### Comparing `pybefit-0.1.21/src/pybefit/tasks/sat.py` & `pybefit-0.1.22/src/pybefit/tasks/sat.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,30 +5,31 @@
 
 @author: markovic
 """
 
 import torch
 from torch.distributions import Categorical, Multinomial
 from torch import ones, zeros
+from .base import Task
 
-class SpaceAdventure(object):
+class SpaceAdventure(Task):
     def __init__(self, conditions,
                  outcome_likelihoods=None,
                  init_states = None,
                  runs = 1,
                  mini_blocks = 1,
                  trials = 2):
         
         
-        self.ns = 6 #number of states
-        self.na = 2 #number of actions
-        self.no = 5 #number of observations
-        self.runs = runs # number of runs
-        self.nmb = mini_blocks #number of mini-blocks for each run
-        
+        super.__init__(runs, mini_blocks, trials)
+
+        self.ns = 6  # number of states
+        self.na = 2  # number of actions
+        self.no = 5  # number of observations
+
         self.list = torch.arange(0, runs, 1, dtype=torch.long)
         
         if outcome_likelihoods is None:
             mnom = Multinomial(probs = ones(self.ns, self.no))
             self.ol = mnom.sample((runs, mini_blocks))
         else:
             self.ol = outcome_likelihoods
@@ -46,19 +47,19 @@
         if init_states is not None:
             self.states[..., 0] = init_states
         else:
             cat = Categorical(probs = torch.ones(runs, mini_blocks, self.ns))
             self.states[..., 0] = cat.sample()
         
     def make_transition_matrix(self):
-        p = self.tp  # transition probability
-        na = self.na # number of actions
-        ns = self.ns # number of states
-        runs = self.runs # number of runs
-        nmb = self.nmb # number of mini-blocks in each run
+        p = self.tp   # transition probability
+        na = self.na  # number of actions
+        ns = self.ns  # number of states
+        runs = self.nsub  # number of agents or parallel runs of the experiment
+        nmb = self.blocks  # number of mini-blocks in each run
         
         self.tm = zeros(runs, nmb, na, ns, ns)
         
         # move left action - no tranistion uncertainty
         self.tm[..., 0, :-1, 1:] = torch.eye(ns - 1).repeat(runs, nmb, 1, 1)
         self.tm[..., 0, -1, 0] = 1
```

### Comparing `pybefit-0.1.21/src/pybefit.egg-info/SOURCES.txt` & `pybefit-0.1.22/src/pybefit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/pybefit.egg-info/PKG-INFO
 src/pybefit.egg-info/SOURCES.txt
 src/pybefit.egg-info/dependency_links.txt
 src/pybefit.egg-info/requires.txt
 src/pybefit.egg-info/top_level.txt
 src/pybefit/agents/__init__.py
 src/pybefit/agents/base.py
+src/pybefit/agents/utils.py
 src/pybefit/agents/jax/__init__.py
 src/pybefit/agents/jax/hsmm_ai.py
 src/pybefit/agents/jax/utils.py
 src/pybefit/agents/torch/__init__.py
 src/pybefit/agents/torch/active_inference.py
 src/pybefit/agents/torch/bayesian.py
 src/pybefit/agents/torch/dynamic_programming.py
@@ -34,9 +35,10 @@
 src/pybefit/inference/pyro/hierarchical.py
 src/pybefit/inference/pyro/infer.py
 src/pybefit/inference/pyro/likelihoods.py
 src/pybefit/inference/pyro/mixed.py
 src/pybefit/inference/pyro/nonparametric.py
 src/pybefit/tasks/__init__.py
 src/pybefit/tasks/bandits.py
+src/pybefit/tasks/base.py
 src/pybefit/tasks/rev_learning.py
 src/pybefit/tasks/sat.py
```

