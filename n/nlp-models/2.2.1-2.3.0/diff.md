# Comparing `tmp/nlp-models-2.2.1.tar.gz` & `tmp/nlp-models-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp-models-2.2.1.tar", last modified: Sun Jun 18 19:57:50 2023, max compression
+gzip compressed data, was "nlp-models-2.3.0.tar", last modified: Sun Jun 18 21:03:49 2023, max compression
```

## Comparing `nlp-models-2.2.1.tar` & `nlp-models-2.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:57:50.020737 nlp-models-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-18 19:57:40.000000 nlp-models-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-18 19:57:50.020737 nlp-models-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-18 19:57:40.000000 nlp-models-2.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-18 19:57:40.000000 nlp-models-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-18 19:57:50.024737 nlp-models-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-18 19:57:40.000000 nlp-models-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:57:50.020737 nlp-models-2.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:57:50.020737 nlp-models-2.2.1/src/bert_classifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/bert_classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/bert_classifier/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/bert_classifier/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/bert_classifier/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/bert_classifier/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/bert_classifier/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/bert_classifier/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:57:50.020737 nlp-models-2.2.1/src/multi_task_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/multi_task_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/multi_task_model/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/multi_task_model/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/multi_task_model/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/multi_task_model/mtl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/multi_task_model/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/multi_task_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:57:50.020737 nlp-models-2.2.1/src/nlp_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-18 19:57:50.000000 nlp-models-2.2.1/src/nlp_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-18 19:57:50.000000 nlp-models-2.2.1/src/nlp_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 19:57:50.000000 nlp-models-2.2.1/src/nlp_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-18 19:57:50.000000 nlp-models-2.2.1/src/nlp_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-18 19:57:50.000000 nlp-models-2.2.1/src/nlp_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:03:48.998097 nlp-models-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-18 21:03:39.000000 nlp-models-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-18 21:03:48.998097 nlp-models-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-18 21:03:39.000000 nlp-models-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-18 21:03:39.000000 nlp-models-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-18 21:03:48.998097 nlp-models-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-18 21:03:39.000000 nlp-models-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:03:48.994097 nlp-models-2.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:03:48.994097 nlp-models-2.3.0/src/bert_classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:03:39.000000 nlp-models-2.3.0/src/bert_classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-18 21:03:39.000000 nlp-models-2.3.0/src/bert_classifier/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-18 21:03:39.000000 nlp-models-2.3.0/src/bert_classifier/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-18 21:03:39.000000 nlp-models-2.3.0/src/bert_classifier/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-18 21:03:39.000000 nlp-models-2.3.0/src/bert_classifier/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-18 21:03:39.000000 nlp-models-2.3.0/src/bert_classifier/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-18 21:03:39.000000 nlp-models-2.3.0/src/bert_classifier/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:03:48.998097 nlp-models-2.3.0/src/multi_task_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:03:39.000000 nlp-models-2.3.0/src/multi_task_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-18 21:03:39.000000 nlp-models-2.3.0/src/multi_task_model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-18 21:03:39.000000 nlp-models-2.3.0/src/multi_task_model/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-18 21:03:39.000000 nlp-models-2.3.0/src/multi_task_model/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-18 21:03:39.000000 nlp-models-2.3.0/src/multi_task_model/mtl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-06-18 21:03:39.000000 nlp-models-2.3.0/src/multi_task_model/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-18 21:03:39.000000 nlp-models-2.3.0/src/multi_task_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:03:48.998097 nlp-models-2.3.0/src/nlp_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-18 21:03:48.000000 nlp-models-2.3.0/src/nlp_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-18 21:03:48.000000 nlp-models-2.3.0/src/nlp_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 21:03:48.000000 nlp-models-2.3.0/src/nlp_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-18 21:03:48.000000 nlp-models-2.3.0/src/nlp_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-18 21:03:48.000000 nlp-models-2.3.0/src/nlp_models.egg-info/top_level.txt
```

### Comparing `nlp-models-2.2.1/LICENSE` & `nlp-models-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.1/setup.cfg` & `nlp-models-2.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nlp-models
-version = 2.2.1
+version = 2.3.0
 author = Ming Gao
 author_email = ming_gao@outlook.com
 url = https://github.com/minggnim/nlp-models
 description = Transformers based NLP models
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `nlp-models-2.2.1/src/bert_classifier/bert.py` & `nlp-models-2.3.0/src/bert_classifier/bert.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.1/src/bert_classifier/data.py` & `nlp-models-2.3.0/src/bert_classifier/data.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.1/src/bert_classifier/io.py` & `nlp-models-2.3.0/src/bert_classifier/io.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.1/src/bert_classifier/metrics.py` & `nlp-models-2.3.0/src/bert_classifier/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.1/src/bert_classifier/predict.py` & `nlp-models-2.3.0/src/bert_classifier/predict.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.1/src/bert_classifier/train.py` & `nlp-models-2.3.0/src/bert_classifier/train.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.1/src/multi_task_model/layers.py` & `nlp-models-2.3.0/src/multi_task_model/layers.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.1/src/multi_task_model/metrics.py` & `nlp-models-2.3.0/src/multi_task_model/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.1/src/multi_task_model/mtl.py` & `nlp-models-2.3.0/src/multi_task_model/mtl.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.1/src/multi_task_model/trainer.py` & `nlp-models-2.3.0/src/multi_task_model/trainer.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.1/src/multi_task_model/utils.py` & `nlp-models-2.3.0/src/multi_task_model/utils.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.1/src/nlp_models.egg-info/SOURCES.txt` & `nlp-models-2.3.0/src/nlp_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

