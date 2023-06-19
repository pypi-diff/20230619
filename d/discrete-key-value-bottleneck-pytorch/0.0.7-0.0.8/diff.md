# Comparing `tmp/discrete-key-value-bottleneck-pytorch-0.0.7.tar.gz` & `tmp/discrete-key-value-bottleneck-pytorch-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discrete-key-value-bottleneck-pytorch-0.0.7.tar", last modified: Tue Jan 17 00:31:32 2023, max compression
+gzip compressed data, was "discrete-key-value-bottleneck-pytorch-0.0.8.tar", last modified: Mon Jun 19 19:56:44 2023, max compression
```

## Comparing `discrete-key-value-bottleneck-pytorch-0.0.7.tar` & `discrete-key-value-bottleneck-pytorch-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 00:31:32.256649 discrete-key-value-bottleneck-pytorch-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-17 00:31:22.000000 discrete-key-value-bottleneck-pytorch-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-01-17 00:31:32.256649 discrete-key-value-bottleneck-pytorch-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-01-17 00:31:22.000000 discrete-key-value-bottleneck-pytorch-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 00:31:32.252649 discrete-key-value-bottleneck-pytorch-0.0.7/discrete_key_value_bottleneck_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-17 00:31:22.000000 discrete-key-value-bottleneck-pytorch-0.0.7/discrete_key_value_bottleneck_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-01-17 00:31:22.000000 discrete-key-value-bottleneck-pytorch-0.0.7/discrete_key_value_bottleneck_pytorch/discrete_key_value_bottleneck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 00:31:32.252649 discrete-key-value-bottleneck-pytorch-0.0.7/discrete_key_value_bottleneck_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-01-17 00:31:32.000000 discrete-key-value-bottleneck-pytorch-0.0.7/discrete_key_value_bottleneck_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-01-17 00:31:32.000000 discrete-key-value-bottleneck-pytorch-0.0.7/discrete_key_value_bottleneck_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 00:31:32.000000 discrete-key-value-bottleneck-pytorch-0.0.7/discrete_key_value_bottleneck_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-17 00:31:32.000000 discrete-key-value-bottleneck-pytorch-0.0.7/discrete_key_value_bottleneck_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 00:31:32.000000 discrete-key-value-bottleneck-pytorch-0.0.7/discrete_key_value_bottleneck_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 00:31:32.256649 discrete-key-value-bottleneck-pytorch-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-01-17 00:31:22.000000 discrete-key-value-bottleneck-pytorch-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:56:44.595391 discrete-key-value-bottleneck-pytorch-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 19:56:28.000000 discrete-key-value-bottleneck-pytorch-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-19 19:56:44.595391 discrete-key-value-bottleneck-pytorch-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-19 19:56:28.000000 discrete-key-value-bottleneck-pytorch-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:56:44.595391 discrete-key-value-bottleneck-pytorch-0.0.8/discrete_key_value_bottleneck_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-19 19:56:28.000000 discrete-key-value-bottleneck-pytorch-0.0.8/discrete_key_value_bottleneck_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-19 19:56:28.000000 discrete-key-value-bottleneck-pytorch-0.0.8/discrete_key_value_bottleneck_pytorch/discrete_key_value_bottleneck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:56:44.595391 discrete-key-value-bottleneck-pytorch-0.0.8/discrete_key_value_bottleneck_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-19 19:56:44.000000 discrete-key-value-bottleneck-pytorch-0.0.8/discrete_key_value_bottleneck_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-19 19:56:44.000000 discrete-key-value-bottleneck-pytorch-0.0.8/discrete_key_value_bottleneck_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:56:44.000000 discrete-key-value-bottleneck-pytorch-0.0.8/discrete_key_value_bottleneck_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-19 19:56:44.000000 discrete-key-value-bottleneck-pytorch-0.0.8/discrete_key_value_bottleneck_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 19:56:44.000000 discrete-key-value-bottleneck-pytorch-0.0.8/discrete_key_value_bottleneck_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 19:56:44.595391 discrete-key-value-bottleneck-pytorch-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-19 19:56:28.000000 discrete-key-value-bottleneck-pytorch-0.0.8/setup.py
```

### Comparing `discrete-key-value-bottleneck-pytorch-0.0.7/LICENSE` & `discrete-key-value-bottleneck-pytorch-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `discrete-key-value-bottleneck-pytorch-0.0.7/PKG-INFO` & `discrete-key-value-bottleneck-pytorch-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discrete-key-value-bottleneck-pytorch
-Version: 0.0.7
+Version: 0.0.8
 Summary: Discrete Key / Value Bottleneck - Pytorch
 Home-page: https://github.com/lucidrains/discrete-key-value-bottleneck-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,quantization,memory,transfer learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `discrete-key-value-bottleneck-pytorch-0.0.7/README.md` & `discrete-key-value-bottleneck-pytorch-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `discrete-key-value-bottleneck-pytorch-0.0.7/discrete_key_value_bottleneck_pytorch.egg-info/PKG-INFO` & `discrete-key-value-bottleneck-pytorch-0.0.8/discrete_key_value_bottleneck_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discrete-key-value-bottleneck-pytorch
-Version: 0.0.7
+Version: 0.0.8
 Summary: Discrete Key / Value Bottleneck - Pytorch
 Home-page: https://github.com/lucidrains/discrete-key-value-bottleneck-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,quantization,memory,transfer learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `discrete-key-value-bottleneck-pytorch-0.0.7/setup.py` & `discrete-key-value-bottleneck-pytorch-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'discrete-key-value-bottleneck-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.7',
+  version = '0.0.8',
   license='MIT',
   description = 'Discrete Key / Value Bottleneck - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/discrete-key-value-bottleneck-pytorch',
   keywords = [
```

