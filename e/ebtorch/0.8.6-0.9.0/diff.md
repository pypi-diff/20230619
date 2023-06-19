# Comparing `tmp/ebtorch-0.8.6.tar.gz` & `tmp/ebtorch-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebtorch-0.8.6.tar", last modified: Thu Jun 15 14:37:30 2023, max compression
+gzip compressed data, was "ebtorch-0.9.0.tar", last modified: Mon Jun 19 15:54:46 2023, max compression
```

## Comparing `ebtorch-0.8.6.tar` & `ebtorch-0.9.0.tar`

### file list

```diff
@@ -1,55 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:37:30.452027 ebtorch-0.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-15 14:37:15.000000 ebtorch-0.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-15 14:37:30.452027 ebtorch-0.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-15 14:37:15.000000 ebtorch-0.8.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:37:30.440027 ebtorch-0.8.6/ebtorch/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:37:30.444027 ebtorch-0.8.6/ebtorch/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/logging/avgmeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/logging/logcsv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:37:30.448027 ebtorch-0.8.6/ebtorch/nn/
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/conv2drp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/convolutional_flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/coordconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/debuglayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/fieldtransform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:37:30.448027 ebtorch-0.8.6/ebtorch/nn/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/functional/inner_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/kwta.py
--rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/laplacenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/lmu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/mish.py
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/nnsemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/reshapelayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/serf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/serlu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/sinlu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/smelu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:37:30.448027 ebtorch-0.8.6/ebtorch/nn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/utils/adverutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/utils/autoclip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/utils/onlyutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/utils/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/utils/reprutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:37:30.448027 ebtorch-0.8.6/ebtorch/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/optim/adahessian.py
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/optim/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/optim/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/optim/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/optim/lookahead.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/optim/radam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/optim/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:37:30.444027 ebtorch-0.8.6/ebtorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-15 14:37:30.000000 ebtorch-0.8.6/ebtorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-15 14:37:30.000000 ebtorch-0.8.6/ebtorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:37:30.000000 ebtorch-0.8.6/ebtorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:37:30.000000 ebtorch-0.8.6/ebtorch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 14:37:30.000000 ebtorch-0.8.6/ebtorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 14:37:30.452027 ebtorch-0.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-15 14:37:15.000000 ebtorch-0.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:54:46.591891 ebtorch-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-19 15:54:32.000000 ebtorch-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-19 15:54:46.591891 ebtorch-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-19 15:54:32.000000 ebtorch-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:54:46.579891 ebtorch-0.9.0/ebtorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:54:46.583891 ebtorch-0.9.0/ebtorch/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/logging/avgmeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/logging/logcsv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:54:46.587891 ebtorch-0.9.0/ebtorch/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/conv2drp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/convolutional_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/coordconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/debuglayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/fieldtransform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:54:46.587891 ebtorch-0.9.0/ebtorch/nn/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/functional/inner_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/kwta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/laplacenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/mish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/nnsemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/reshapelayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/serf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/serlu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/sinlu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/smelu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:54:46.587891 ebtorch-0.9.0/ebtorch/nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/utils/adverutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/utils/autoclip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/utils/onlyutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/utils/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/utils/reprutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:54:46.587891 ebtorch-0.9.0/ebtorch/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/optim/adahessian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/optim/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/optim/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/optim/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/optim/lookahead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/optim/radam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/optim/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:54:46.583891 ebtorch-0.9.0/ebtorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-19 15:54:46.000000 ebtorch-0.9.0/ebtorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-19 15:54:46.000000 ebtorch-0.9.0/ebtorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:54:46.000000 ebtorch-0.9.0/ebtorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:54:46.000000 ebtorch-0.9.0/ebtorch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 15:54:46.000000 ebtorch-0.9.0/ebtorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 15:54:46.591891 ebtorch-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-06-19 15:54:32.000000 ebtorch-0.9.0/setup.py
```

### Comparing `ebtorch-0.8.6/LICENSE` & `ebtorch-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/PKG-INFO` & `ebtorch-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebtorch
-Version: 0.8.6
+Version: 0.9.0
 Summary: Collection of PyTorch additions, extensions, utilities, uses and abuses
 Home-page: https://github.com/emaballarin/ebtorch
 Author: Emanuele Ballarin
 Author-email: emanuele@ballarin.cc
 License: Apache-2.0
 Keywords: Deep Learning,Machine Learning
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebtorch Version: 0.8.6 Summary: Collection of
+Metadata-Version: 2.1 Name: ebtorch Version: 0.9.0 Summary: Collection of
 PyTorch additions, extensions, utilities, uses and abuses Home-page: https://
 github.com/emaballarin/ebtorch Author: Emanuele Ballarin Author-email:
 emanuele@ballarin.cc License: Apache-2.0 Keywords: Deep Learning,Machine
 Learning Classifier: Development Status :: 3 - Alpha Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Environment ::
 Console Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
```

### Comparing `ebtorch-0.8.6/ebtorch/__init__.py` & `ebtorch-0.9.0/ebtorch/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -38,20 +38,18 @@
 del CoordConv3d
 del Dropout2dRP
 del FCBlock
 del FCBlockLegacy
 del FieldTransform
 del FlatChannelize2DLayer
 del GaussianReparameterizerSampler
+del InnerProduct
 del KWTA1d
 del KWTA2d
-del LMUCell
 del Mish
-del MishPulse
-del MishPulseSymmY
 del MultiSolvePoissonTensor
 del NNEnsemble
 del PoissonNetCifar
 del ProbePrintLayer
 del ReshapeLayer
 del ScaledERF
 del SERLU
@@ -59,16 +57,14 @@
 del SinLU
 del SmeLU
 del SolvePoisson
 del SolvePoissonTensor
 del beta_reco_bce
 del field_transform
 del mishlayer_init
-del mishpulse
-del mishpulse_symmy
 del patch_rp_train_network
 del pixelwise_bce_mean
 del pixelwise_bce_sum
 
 # Deletions (from .optim)
 del AdaHessian
 del Adan
```

### Comparing `ebtorch-0.8.6/ebtorch/logging/__init__.py` & `ebtorch-0.9.0/ebtorch/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/logging/avgmeter.py` & `ebtorch-0.9.0/ebtorch/logging/avgmeter.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/logging/logcsv.py` & `ebtorch-0.9.0/ebtorch/logging/logcsv.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/nn/__init__.py` & `ebtorch-0.9.0/ebtorch/nn/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from .architectures import ArgMaxLayer
 from .architectures import beta_reco_bce
 from .architectures import BinarizeLayer
 from .architectures import CausalConv1d
 from .architectures import FCBlock
 from .architectures import FCBlockLegacy
 from .architectures import GaussianReparameterizerSampler
+from .architectures import InnerProduct
 from .architectures import pixelwise_bce_mean
 from .architectures import pixelwise_bce_sum
 from .architectures import SGRUHCell
 from .conv2drp import BatchNorm2dRP
 from .conv2drp import Conv2dRP
 from .conv2drp import Dropout2dRP
 from .conv2drp import patch_rp_train_network
@@ -39,28 +40,23 @@
 from .coordconv import CoordConv1d
 from .coordconv import CoordConv2d
 from .coordconv import CoordConv3d
 from .debuglayers import ProbePrintLayer
 from .fieldtransform import FieldTransform
 from .functional import field_transform
 from .functional import mish
-from .functional import mishpulse
-from .functional import mishpulse_symmy
 from .kwta import BrokenReLU
 from .kwta import KWTA1d
 from .kwta import KWTA2d
 from .laplacenet import MultiSolvePoissonTensor
 from .laplacenet import PoissonNetCifar
 from .laplacenet import SolvePoisson
 from .laplacenet import SolvePoissonTensor
-from .lmu import LMUCell
 from .mish import Mish
 from .mish import mishlayer_init
-from .mish import MishPulse
-from .mish import MishPulseSymmY
 from .nnsemble import NNEnsemble
 from .reshapelayers import FlatChannelize2DLayer
 from .reshapelayers import ReshapeLayer
 from .serf import ScaledERF
 from .serlu import SERLU
 from .sinlu import SinLU
 from .smelu import SmeLU
@@ -71,15 +67,14 @@
 del conv2drp
 del convolutional_flatten
 del coordconv
 del debuglayers
 del fieldtransform
 del kwta
 del laplacenet
-del lmu
 del mish
 del nnsemble
 del reshapelayers
 del serlu
 del sinlu
 del smelu
 del serf
```

### Comparing `ebtorch-0.8.6/ebtorch/nn/architectures.py` & `ebtorch-0.9.0/ebtorch/nn/architectures.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,15 +279,15 @@
     if device is None:
         device = z_mu.device
         if device != z_log_var.device:
             raise RuntimeError(
                 f"Device mismatch among 'z_mu' ({device}) and 'z_log_var' ({z_log_var.device})!"
             )
     return z_mu.to(device) + torch.randn_like(z_mu).to(device) * torch.exp(
-        z_log_var * 0.5
+        z_log_var * 0.5  # type: ignore
     ).to(device)
 
 
 class GaussianReparameterizerSampler(nn.Module):
     def __init__(self):  # skipcq: PYL-W0235
         super().__init__()
 
@@ -409,7 +409,21 @@
 class BinarizeLayer(nn.Module):
     def __init__(self, threshold: float = 0.5) -> None:
         super().__init__()
         self.threshold: float = threshold
 
     def forward(self, x: Tensor) -> Tensor:
         return (x > self.threshold).float()  # (...): th.Tensor
+
+
+class InnerProduct(nn.Module):
+    """
+    Compute row-wise dot-product of two batches of tensors (vectors).
+    (https://github.com/UnconsciousBias/ublib/blob/master/ublib/torch.py)
+    """
+
+    def __init__(self, dim=1):
+        super(InnerProduct, self).__init__()
+        self.dim = dim
+
+    def forward(self, a, b):
+        return torch.bmm(a.unsqueeze(self.dim), b.unsqueeze(self.dim + 1)).squeeze()
```

### Comparing `ebtorch-0.8.6/ebtorch/nn/conv2drp.py` & `ebtorch-0.9.0/ebtorch/nn/conv2drp.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     return_net: bool = False,
 ) -> Optional[torch.nn.Module]:
     _train_toggle_status: bool = net.training  # Save training value
 
     net.eval()  # Do not track statistics
     with torch.no_grad():  # Do not track gradients
         # Iterate over all layers in the network
-        for layer in tqdm(
+        for layer in tqdm(  # type: ignore
             [
                 _lay
                 for _lay in net.modules()
                 if isinstance(_lay, (BatchNorm2dRP, Conv2dRP, Dropout2dRP))
             ],
             leave=False,
             desc="RP-training network",
@@ -184,15 +184,15 @@
             elif isinstance(layer, Conv2dRP):
                 layer.clear_tracked_inputs()
                 layer.eval()
                 layer.set_tracking(True)
 
             # DATA PASS | All cases
             if isinstance(layer, (BatchNorm2dRP, Conv2dRP, Dropout2dRP)):
-                for batched_datapoint in tqdm(
+                for batched_datapoint in tqdm(  # type: ignore
                     data, leave=True, desc=f"RP-training layer {layer}"
                 ):
                     _ = net(batched_datapoint[0])
 
             # POST | Case 1; Case 2
             if isinstance(layer, (BatchNorm2dRP, Dropout2dRP)):
                 layer.eval()
```

### Comparing `ebtorch-0.8.6/ebtorch/nn/convolutional_flatten.py` & `ebtorch-0.9.0/ebtorch/nn/convolutional_flatten.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/nn/coordconv.py` & `ebtorch-0.9.0/ebtorch/nn/coordconv.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/nn/debuglayers.py` & `ebtorch-0.9.0/ebtorch/nn/debuglayers.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/nn/fieldtransform.py` & `ebtorch-0.9.0/ebtorch/nn/fieldtransform.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/nn/functional/__init__.py` & `ebtorch-0.9.0/ebtorch/nn/functional/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,15 +19,13 @@
 #
 # ==============================================================================
 #
 # SPDX-License-Identifier: Apache-2.0
 # Imports (specific)
 from .inner_functional import field_transform
 from .inner_functional import mish
-from .inner_functional import mishpulse
-from .inner_functional import mishpulse_symmy
 from .inner_functional import serf
 from .inner_functional import serlu
 from .inner_functional import smelu
 
 # Deletions (from .)
 del inner_functional
```

### Comparing `ebtorch-0.8.6/ebtorch/nn/functional/inner_functional.py` & `ebtorch-0.9.0/ebtorch/nn/functional/inner_functional.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,16 +30,14 @@
 # SPDX-License-Identifier: Apache-2.0
 # IMPORTS
 import math
 
 import torch
 import torch.nn.functional as F
 from torch import Tensor
-from torch.overrides import handle_torch_function
-from torch.overrides import has_torch_function_unary
 
 
 # FUNCTIONS
 
 
 def field_transform(
     x_input: Tensor,
@@ -70,60 +68,34 @@
     Applies the mish function element-wise:
     mish(x) = x * tanh(softplus(x)) = x * tanh(ln(1 + exp(x)))
     """
     return F.mish(x_input)
 
 
 @torch.jit.script
-def mishpulse(x_input: Tensor) -> Tensor:
-    """
-    Applies the mishpulse function element-wise:
-    mishpulse(x) = -sign(x) * mish(-abs(x) + 0.6361099463262276) + step(x)
-    """
-    if has_torch_function_unary(x_input):
-        return handle_torch_function(mish, (x_input,), x_input)
-
-    return -torch.sign(x_input) * mish(
-        -torch.abs(x_input) + 0.6361099463262276
-    ) + torch.heaviside(x_input, values=torch.tensor([0.0]))
-
-
-@torch.jit.script
-def mishpulse_symmy(x_input: Tensor) -> Tensor:
-    """
-    Applies the mishpulse function, adapted to be y-symmetric, element-wise:
-    mishpulse_symmy(x) = -sign(x) * (mish(-abs(x) + 1.127332431855187) - 1)
-    """
-    if has_torch_function_unary(x_input):
-        return handle_torch_function(mish, (x_input,), x_input)
-
-    return -torch.sign(x_input) * (mish(-torch.abs(x_input) + 1.127332431855187) - 1.0)
-
-
-@torch.jit.script
 def serlu(x_input: Tensor, lambd: float = 1.07862, alph: float = 2.90427) -> Tensor:
     """
     Applies the SERLU function element-wise,
     defined after [Zhang & Li, 2018]
     """
-    return torch.where(
+    return torch.where(  # type: ignore
         x_input >= 0.0,
         torch.mul(x_input, lambd),
         torch.mul(torch.mul(x_input, torch.exp(x_input)), lambd * alph),
     )
 
 
 @torch.jit.script
 def smelu(x_input: Tensor, beta: float = 2.0) -> Tensor:
     """
     Applies the SmeLU function element-wise,
     defined after [Shamir & Ling, 2022]
     """
     assert beta >= 0
-    return torch.where(
+    return torch.where(  # type: ignore
         torch.abs(x_input) <= beta,
         torch.div(torch.pow(torch.add(x_input, beta), 2), 4.0 * beta),
         F.relu(x_input),
     )
 
 
 @torch.jit.script
```

### Comparing `ebtorch-0.8.6/ebtorch/nn/kwta.py` & `ebtorch-0.9.0/ebtorch/nn/kwta.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/nn/laplacenet.py` & `ebtorch-0.9.0/ebtorch/nn/laplacenet.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         # This slab can't store or leak currents. Ensure the total current flux is 0.
         input_currents = input_currents - input_currents.mean()
 
         # Element (i,j) of this vector is R[i,j]
         center_conductances = torch.exp(self.log_resistances).flatten()
 
         mat_z_off_diagonal = torch.sparse_coo_tensor(
-            (self.edges_center, self.edges_neighbor),
+            (self.edges_center, self.edges_neighbor),  # type: ignore
             center_conductances[self.edges_center]
             + center_conductances[self.edges_neighbor],
             (image_width * image_height, image_width * image_height),
         ).to_dense()
 
         zmat = torch.diag(mat_z_off_diagonal.sum(axis=1)) - mat_z_off_diagonal
```

### Comparing `ebtorch-0.8.6/ebtorch/nn/nnsemble.py` & `ebtorch-0.9.0/ebtorch/nn/nnsemble.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/nn/reshapelayers.py` & `ebtorch-0.9.0/ebtorch/nn/reshapelayers.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/nn/serf.py` & `ebtorch-0.9.0/ebtorch/nn/serf.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/nn/serlu.py` & `ebtorch-0.9.0/ebtorch/nn/serlu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/nn/sinlu.py` & `ebtorch-0.9.0/ebtorch/nn/sinlu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/nn/smelu.py` & `ebtorch-0.9.0/ebtorch/nn/smelu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/nn/utils/__init__.py` & `ebtorch-0.9.0/ebtorch/nn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/nn/utils/adverutils.py` & `ebtorch-0.9.0/ebtorch/nn/utils/adverutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/nn/utils/autoclip.py` & `ebtorch-0.9.0/ebtorch/nn/utils/autoclip.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/nn/utils/onlyutils.py` & `ebtorch-0.9.0/ebtorch/nn/utils/onlyutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/nn/utils/patches.py` & `ebtorch-0.9.0/ebtorch/nn/utils/patches.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/nn/utils/reprutils.py` & `ebtorch-0.9.0/ebtorch/nn/utils/reprutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         name: str
         mod: Module
         for name, mod in model.named_modules():
             if (
                 named_layers is not None and name in named_layers
             ) or named_layers is None:
                 handle: RemovableHandle = mod.register_forward_hook(
-                    partial(
+                    partial(  # type: ignore
                         store_repr_hook,
                         representation_list,
                         starting_indices,
                         device=device,
                         preserve_graph=preserve_graph,
                     )
                 )
```

### Comparing `ebtorch-0.8.6/ebtorch/optim/__init__.py` & `ebtorch-0.9.0/ebtorch/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/optim/adahessian.py` & `ebtorch-0.9.0/ebtorch/optim/adahessian.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                 * 2.0
                 - 1.0
                 for p in params
             ]  # Rademacher distribution {-1.0, 1.0}
             h_zs = torch.autograd.grad(
                 grads,
                 params,
-                grad_outputs=zs,  # Expected type mismatch!
+                grad_outputs=zs,  # type: ignore
                 only_inputs=True,
                 retain_graph=i < self.n_samples - 1,
             )
             for h_z, z, p in zip(h_zs, zs, params):
                 p.hess += (
                     h_z * z / self.n_samples
                 )  # approximate the expected values of z*(H@z)
```

### Comparing `ebtorch-0.8.6/ebtorch/optim/adan.py` & `ebtorch-0.9.0/ebtorch/optim/adan.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/optim/custom.py` & `ebtorch-0.9.0/ebtorch/optim/custom.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/optim/lion.py` & `ebtorch-0.9.0/ebtorch/optim/lion.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/optim/lookahead.py` & `ebtorch-0.9.0/ebtorch/optim/lookahead.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/optim/radam.py` & `ebtorch-0.9.0/ebtorch/optim/radam.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch/optim/sam.py` & `ebtorch-0.9.0/ebtorch/optim/sam.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.6/ebtorch.egg-info/PKG-INFO` & `ebtorch-0.9.0/ebtorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebtorch
-Version: 0.8.6
+Version: 0.9.0
 Summary: Collection of PyTorch additions, extensions, utilities, uses and abuses
 Home-page: https://github.com/emaballarin/ebtorch
 Author: Emanuele Ballarin
 Author-email: emanuele@ballarin.cc
 License: Apache-2.0
 Keywords: Deep Learning,Machine Learning
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebtorch Version: 0.8.6 Summary: Collection of
+Metadata-Version: 2.1 Name: ebtorch Version: 0.9.0 Summary: Collection of
 PyTorch additions, extensions, utilities, uses and abuses Home-page: https://
 github.com/emaballarin/ebtorch Author: Emanuele Ballarin Author-email:
 emanuele@ballarin.cc License: Apache-2.0 Keywords: Deep Learning,Machine
 Learning Classifier: Development Status :: 3 - Alpha Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Environment ::
 Console Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
```

### Comparing `ebtorch-0.8.6/ebtorch.egg-info/SOURCES.txt` & `ebtorch-0.9.0/ebtorch.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 ebtorch/nn/conv2drp.py
 ebtorch/nn/convolutional_flatten.py
 ebtorch/nn/coordconv.py
 ebtorch/nn/debuglayers.py
 ebtorch/nn/fieldtransform.py
 ebtorch/nn/kwta.py
 ebtorch/nn/laplacenet.py
-ebtorch/nn/lmu.py
 ebtorch/nn/mish.py
 ebtorch/nn/nnsemble.py
 ebtorch/nn/reshapelayers.py
 ebtorch/nn/serf.py
 ebtorch/nn/serlu.py
 ebtorch/nn/sinlu.py
 ebtorch/nn/smelu.py
```

### Comparing `ebtorch-0.8.6/setup.py` & `ebtorch-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # ==============================================================================
 #
-# Copyright 2019-* Yana Hasson <yana.hasson.inria@gmail.com>
-# Copyright 2019-* Linxi (Jim) Fan <jimfanspire@gmail.com>
-#
-# ==============================================================================
-#
 # Copyright 2020-* Emanuele Ballarin <emanuele@ballarin.cc>
 # All Rights Reserved. Unless otherwise explicitly stated.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -34,51 +29,55 @@
 
 
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read().strip()
 
 
-def check_dependencies():
-    missing_dependencies = []
-    for package_name in DEPENDENCY_PACKAGE_NAMES:
+def check_dependencies(dependencies: list[str]):
+    missing_dependencies: list[str] = []
+    package_name: str
+    for package_name in dependencies:
         try:
             __import__(package_name)
         except ImportError:
             missing_dependencies.append(package_name)
 
     if missing_dependencies:
         warnings.warn(f"Missing dependencies: {missing_dependencies}")
 
 
-DEPENDENCY_PACKAGE_NAMES = [
+DEPENDENCY_PACKAGE_NAMES: list[str] = [
     "advertorch",
-    "nengolib",
     "numpy",
     "requests",
     "torch",
     "torchattacks",
     "tqdm",
 ]
 
-check_dependencies()
+check_dependencies(DEPENDENCY_PACKAGE_NAMES)
+
+PACKAGENAME: str = "ebtorch"
 
 
 setup(
-    name="ebtorch",
-    version="0.8.6",
+    name=PACKAGENAME,
+    version="0.9.0",
     author="Emanuele Ballarin",
     author_email="emanuele@ballarin.cc",
     url="https://github.com/emaballarin/ebtorch",
     description="Collection of PyTorch additions, extensions, utilities, uses and abuses",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     keywords=["Deep Learning", "Machine Learning"],
     license="Apache-2.0",
-    packages=[package for package in find_packages() if package.startswith("ebtorch")],
+    packages=[
+        package for package in find_packages() if package.startswith(PACKAGENAME)
+    ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Environment :: Console",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
     ],
```

