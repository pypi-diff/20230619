# Comparing `tmp/fau_tools-1.4.5.2.tar.gz` & `tmp/fau_tools-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fau_tools-1.4.5.2.tar", max compression
+gzip compressed data, was "fau_tools-1.5.0.tar", max compression
```

## Comparing `fau_tools-1.4.5.2.tar` & `fau_tools-1.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      179 2022-09-17 06:01:57.485247 fau_tools-1.4.5.2/Fau_tools/__init__.py
--rw-r--r--   0        0        0       30 2022-11-07 07:34:00.261010 fau_tools-1.4.5.2/Fau_tools/data_structure/__init__.py
--rw-r--r--   0        0        0     3432 2023-06-14 07:04:20.652148 fau_tools-1.4.5.2/Fau_tools/data_structure/data_structure.py
--rw-r--r--   0        0        0      914 2023-04-20 02:46:11.824752 fau_tools-1.4.5.2/Fau_tools/data_structure/data_structure.pyi
--rw-r--r--   0        0        0       27 2022-09-17 05:48:40.673809 fau_tools-1.4.5.2/Fau_tools/torch_tools/__init__.py
--rw-r--r--   0        0        0    10116 2023-06-14 07:06:31.832738 fau_tools-1.4.5.2/Fau_tools/torch_tools/torch_tools.py
--rw-r--r--   0        0        0     1440 2023-04-20 02:46:11.825456 fau_tools-1.4.5.2/Fau_tools/torch_tools/torch_tools.pyi
--rw-r--r--   0        0        0       23 2022-09-17 05:58:01.298778 fau_tools-1.4.5.2/Fau_tools/utility/__init__.py
--rw-r--r--   0        0        0    10983 2023-06-14 07:11:29.039437 fau_tools-1.4.5.2/Fau_tools/utility/utility.py
--rw-r--r--   0        0        0     1008 2023-06-05 09:23:30.478542 fau_tools-1.4.5.2/Fau_tools/utility/utility.pyi
--rw-r--r--   0        0        0     2680 2023-04-20 02:37:45.625671 fau_tools-1.4.5.2/README.md
--rw-r--r--   0        0        0     1150 2023-06-14 07:13:01.011155 fau_tools-1.4.5.2/pyproject.toml
--rw-r--r--   0        0        0     3431 1970-01-01 00:00:00.000000 fau_tools-1.4.5.2/PKG-INFO
+-rw-r--r--   0        0        0     2680 2023-06-19 09:30:37.454323 fau_tools-1.5.0/README.md
+-rw-r--r--   0        0        0      179 2023-06-19 09:26:38.024769 fau_tools-1.5.0/fau_tools/__init__.py
+-rw-r--r--   0        0        0       30 2022-11-07 07:34:00.261010 fau_tools-1.5.0/fau_tools/data_structure/__init__.py
+-rw-r--r--   0        0        0     3432 2023-06-19 09:26:42.735406 fau_tools-1.5.0/fau_tools/data_structure/data_structure.py
+-rw-r--r--   0        0        0      914 2023-04-20 02:46:11.824752 fau_tools-1.5.0/fau_tools/data_structure/data_structure.pyi
+-rw-r--r--   0        0        0       27 2022-09-17 05:48:40.673809 fau_tools-1.5.0/fau_tools/torch_tools/__init__.py
+-rw-r--r--   0        0        0    10116 2023-06-19 09:30:03.487112 fau_tools-1.5.0/fau_tools/torch_tools/torch_tools.py
+-rw-r--r--   0        0        0     1440 2023-06-19 09:26:46.569110 fau_tools-1.5.0/fau_tools/torch_tools/torch_tools.pyi
+-rw-r--r--   0        0        0       23 2022-09-17 05:58:01.298778 fau_tools-1.5.0/fau_tools/utility/__init__.py
+-rw-r--r--   0        0        0    10983 2023-06-14 07:11:29.039437 fau_tools-1.5.0/fau_tools/utility/utility.py
+-rw-r--r--   0        0        0     1008 2023-06-05 09:23:30.478542 fau_tools-1.5.0/fau_tools/utility/utility.pyi
+-rw-r--r--   0        0        0     1148 2023-06-19 09:35:01.615607 fau_tools-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3429 1970-01-01 00:00:00.000000 fau_tools-1.5.0/PKG-INFO
```

### Comparing `fau_tools-1.4.5.2/Fau_tools/data_structure/data_structure.py` & `fau_tools-1.5.0/fau_tools/data_structure/data_structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import time
 
-from Fau_tools.utility import cprint
+from fau_tools.utility import cprint
 
 
 class ModelManager:
   """Manage the trained models."""
 
   def __init__(self):
     self.loss, self.accuracy = None, None
```

### Comparing `fau_tools-1.4.5.2/Fau_tools/data_structure/data_structure.pyi` & `fau_tools-1.5.0/fau_tools/data_structure/data_structure.pyi`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.5.2/Fau_tools/torch_tools/torch_tools.py` & `fau_tools-1.5.0/fau_tools/torch_tools/torch_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
 import torch
 import matplotlib.pyplot as plt
 from matplotlib import ticker
 
-from Fau_tools import utility
-from Fau_tools.data_structure import ModelManager, TimeManager, TrainRecorder
-from Fau_tools.utility import cprint
+from fau_tools import utility
+from fau_tools.data_structure import ModelManager, TimeManager, TrainRecorder
+from fau_tools.utility import cprint
 
 
 
 # ------------------------------------------------------------
 # --------------- Function --- training
 # ------------------------------------------------------------
```

### Comparing `fau_tools-1.4.5.2/Fau_tools/torch_tools/torch_tools.pyi` & `fau_tools-1.5.0/fau_tools/torch_tools/torch_tools.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 from torch import nn
 import torch.utils.data as tdata
 
-from Fau_tools.data_structure import TimeManager
+from fau_tools.data_structure import TimeManager
 
 
 # ------------------------------------------------------------
 # --------------- Function --- training
 # ------------------------------------------------------------
 
 def __show_progress(now: int, total: int, loss: float=None, accuracy: float=None, time_manager: TimeManager=None) -> None: ...
```

### Comparing `fau_tools-1.4.5.2/Fau_tools/utility/utility.py` & `fau_tools-1.5.0/fau_tools/utility/utility.py`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.5.2/Fau_tools/utility/utility.pyi` & `fau_tools-1.5.0/fau_tools/utility/utility.pyi`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.5.2/README.md` & `fau_tools-1.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,41 +2,41 @@
 
 This is an individual module, which is mainly for **pytorch CNN** training.
 
 Moreover, it also supports some awesome features: saving model, saving training process, plotting figures and so on...
 
 ## Install
 
-`pip install Fau-tools`
+`pip install fau-tools`
 
 ## Usage
 
 ### import
 
 The following code is recommended.
 
 ```python
-import Fau_tools
-from Fau_tools import torch_tools
+import fau_tools
+from fau_tools import torch_tools
 ```
 
 ### quick start
 
 The tutor will use a simple example to help you get started quickly!
 
 **The following example uses Fau-tools to train a model in MNIST hand-written digits dataset.**
 
 ```python
 import torch
 import torch.utils.data as tdata
 import torchvision
 from torch import nn
 
-import Fau_tools
-from Fau_tools import torch_tools
+import fau_tools
+from fau_tools import torch_tools
 
 # A simple CNN network
 class CNN(nn.Module):
   def __init__(self):
     super().__init__()
     self.conv = nn.Sequential(
       nn.Conv2d(1, 16, 3, 1, 1),  # -> (16, 28, 28)
```

### Comparing `fau_tools-1.4.5.2/pyproject.toml` & `fau_tools-1.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -21,23 +21,23 @@
 # reportMissingTypeStubs  = false
 reportUnusedExpression  = false
 
 # useLibraryCodeForTypes = false
 
 
 [tool.poetry]
-name = "Fau-tools"
-version = "1.4.5.2"
+name = "fau-tools"
+version = "1.5.0"
 description = "A python module. The main function is for pytorch training."
 authors = ["Fau <Fau818@qq.com>"]
 license = "MIT"
 readme = "README.md"
-packages = [{include = "Fau_tools"}]
-homepage   = "https://github.com/Fau818/Fau_tools"
-repository = "https://github.com/Fau818/Fau_tools"
+packages = [{include = "fau_tools"}]
+homepage   = "https://github.com/Fau818/fau-tools"
+repository = "https://github.com/Fau818/fau-tools"
 
 [tool.poetry.dependencies]
 python = ">=3.6"
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `fau_tools-1.4.5.2/PKG-INFO` & `fau_tools-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 Metadata-Version: 2.1
 Name: fau-tools
-Version: 1.4.5.2
+Version: 1.5.0
 Summary: A python module. The main function is for pytorch training.
-Home-page: https://github.com/Fau818/Fau_tools
+Home-page: https://github.com/Fau818/fau-tools
 License: MIT
 Author: Fau
 Author-email: Fau818@qq.com
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Project-URL: Repository, https://github.com/Fau818/Fau_tools
+Project-URL: Repository, https://github.com/Fau818/fau-tools
 Description-Content-Type: text/markdown
 
 ## Introduction
 
 This is an individual module, which is mainly for **pytorch CNN** training.
 
 Moreover, it also supports some awesome features: saving model, saving training process, plotting figures and so on...
 
 ## Install
 
-`pip install Fau-tools`
+`pip install fau-tools`
 
 ## Usage
 
 ### import
 
 The following code is recommended.
 
 ```python
-import Fau_tools
-from Fau_tools import torch_tools
+import fau_tools
+from fau_tools import torch_tools
 ```
 
 ### quick start
 
 The tutor will use a simple example to help you get started quickly!
 
 **The following example uses Fau-tools to train a model in MNIST hand-written digits dataset.**
 
 ```python
 import torch
 import torch.utils.data as tdata
 import torchvision
 from torch import nn
 
-import Fau_tools
-from Fau_tools import torch_tools
+import fau_tools
+from fau_tools import torch_tools
 
 # A simple CNN network
 class CNN(nn.Module):
   def __init__(self):
     super().__init__()
     self.conv = nn.Sequential(
       nn.Conv2d(1, 16, 3, 1, 1),  # -> (16, 28, 28)
```

