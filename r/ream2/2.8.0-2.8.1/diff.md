# Comparing `tmp/ream2-2.8.0.tar.gz` & `tmp/ream2-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ream2-2.8.0.tar", max compression
+gzip compressed data, was "ream2-2.8.1.tar", max compression
```

## Comparing `ream2-2.8.0.tar` & `ream2-2.8.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1064 2023-06-13 06:02:33.452605 ream2-2.8.0/LICENSE
--rw-r--r--   0        0        0     5267 2023-06-13 06:02:33.452605 ream2-2.8.0/README.md
--rw-r--r--   0        0        0      763 2023-06-13 06:02:33.452605 ream2-2.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-13 06:02:33.452605 ream2-2.8.0/ream/__init__.py
--rw-r--r--   0        0        0    14886 2023-06-13 06:02:33.452605 ream2-2.8.0/ream/actor_graph.py
--rw-r--r--   0        0        0     2197 2023-06-13 06:02:33.452605 ream2-2.8.0/ream/actor_state.py
--rw-r--r--   0        0        0     2040 2023-06-13 06:02:33.452605 ream2-2.8.0/ream/actor_version.py
--rw-r--r--   0        0        0        0 2023-06-13 06:02:33.452605 ream2-2.8.0/ream/actors/__init__.py
--rw-r--r--   0        0        0     4115 2023-06-13 06:02:33.452605 ream2-2.8.0/ream/actors/base.py
--rw-r--r--   0        0        0     1155 2023-06-13 06:02:33.452605 ream2-2.8.0/ream/actors/dsid.py
--rw-r--r--   0        0        0     1332 2023-06-13 06:02:33.452605 ream2-2.8.0/ream/actors/enum.py
--rw-r--r--   0        0        0      363 2023-06-13 06:02:33.452605 ream2-2.8.0/ream/actors/interface.py
--rw-r--r--   0        0        0    37569 2023-06-13 06:02:33.456605 ream2-2.8.0/ream/cache_helper.py
--rw-r--r--   0        0        0     3393 2023-06-13 06:02:33.456605 ream2-2.8.0/ream/cli_helper.py
--rw-r--r--   0        0        0    34210 2023-06-13 06:02:33.456605 ream2-2.8.0/ream/data_model_helper.py
--rw-r--r--   0        0        0    14434 2023-06-13 06:02:33.456605 ream2-2.8.0/ream/dataset_helper.py
--rw-r--r--   0        0        0     9838 2023-06-13 06:02:33.456605 ream2-2.8.0/ream/fs.py
--rw-r--r--   0        0        0     6636 2023-06-13 06:02:33.456605 ream2-2.8.0/ream/helper.py
--rw-r--r--   0        0        0     5684 2023-06-13 06:02:33.456605 ream2-2.8.0/ream/params_helper.py
--rw-r--r--   0        0        0     1090 2023-06-13 06:02:33.456605 ream2-2.8.0/ream/prelude.py
--rw-r--r--   0        0        0     2248 2023-06-13 06:02:33.456605 ream2-2.8.0/ream/workspace.py
--rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 ream2-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-19 18:04:44.079771 ream2-2.8.1/LICENSE
+-rw-r--r--   0        0        0     5267 2023-06-19 18:04:44.079771 ream2-2.8.1/README.md
+-rw-r--r--   0        0        0      763 2023-06-19 18:04:44.079771 ream2-2.8.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-19 18:04:44.079771 ream2-2.8.1/ream/__init__.py
+-rw-r--r--   0        0        0    14886 2023-06-19 18:04:44.079771 ream2-2.8.1/ream/actor_graph.py
+-rw-r--r--   0        0        0     2197 2023-06-19 18:04:44.079771 ream2-2.8.1/ream/actor_state.py
+-rw-r--r--   0        0        0     2040 2023-06-19 18:04:44.079771 ream2-2.8.1/ream/actor_version.py
+-rw-r--r--   0        0        0        0 2023-06-19 18:04:44.079771 ream2-2.8.1/ream/actors/__init__.py
+-rw-r--r--   0        0        0     4115 2023-06-19 18:04:44.079771 ream2-2.8.1/ream/actors/base.py
+-rw-r--r--   0        0        0     1155 2023-06-19 18:04:44.079771 ream2-2.8.1/ream/actors/dsid.py
+-rw-r--r--   0        0        0     1332 2023-06-19 18:04:44.079771 ream2-2.8.1/ream/actors/enum.py
+-rw-r--r--   0        0        0      363 2023-06-19 18:04:44.079771 ream2-2.8.1/ream/actors/interface.py
+-rw-r--r--   0        0        0    37569 2023-06-19 18:04:44.079771 ream2-2.8.1/ream/cache_helper.py
+-rw-r--r--   0        0        0     3393 2023-06-19 18:04:44.079771 ream2-2.8.1/ream/cli_helper.py
+-rw-r--r--   0        0        0    34210 2023-06-19 18:04:44.079771 ream2-2.8.1/ream/data_model_helper.py
+-rw-r--r--   0        0        0    14434 2023-06-19 18:04:44.079771 ream2-2.8.1/ream/dataset_helper.py
+-rw-r--r--   0        0        0     9838 2023-06-19 18:04:44.079771 ream2-2.8.1/ream/fs.py
+-rw-r--r--   0        0        0     6636 2023-06-19 18:04:44.079771 ream2-2.8.1/ream/helper.py
+-rw-r--r--   0        0        0     5684 2023-06-19 18:04:44.079771 ream2-2.8.1/ream/params_helper.py
+-rw-r--r--   0        0        0     1119 2023-06-19 18:04:44.079771 ream2-2.8.1/ream/prelude.py
+-rw-r--r--   0        0        0     2248 2023-06-19 18:04:44.079771 ream2-2.8.1/ream/workspace.py
+-rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 ream2-2.8.1/PKG-INFO
```

### Comparing `ream2-2.8.0/LICENSE` & `ream2-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ream2-2.8.0/README.md` & `ream2-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `ream2-2.8.0/pyproject.toml` & `ream2-2.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ream2"
-version = "2.8.0"
+version = "2.8.1"
 description = "An actor architecture for research software"
 authors = ["Binh Vu <binh@toan2.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/binh-vu/ream"
 repository = "https://github.com/binh-vu/ream"
 packages = [
```

### Comparing `ream2-2.8.0/ream/actor_graph.py` & `ream2-2.8.1/ream/actor_graph.py`

 * *Files identical despite different names*

### Comparing `ream2-2.8.0/ream/actor_state.py` & `ream2-2.8.1/ream/actor_state.py`

 * *Files identical despite different names*

### Comparing `ream2-2.8.0/ream/actor_version.py` & `ream2-2.8.1/ream/actor_version.py`

 * *Files identical despite different names*

### Comparing `ream2-2.8.0/ream/actors/base.py` & `ream2-2.8.1/ream/actors/base.py`

 * *Files identical despite different names*

### Comparing `ream2-2.8.0/ream/actors/dsid.py` & `ream2-2.8.1/ream/actors/dsid.py`

 * *Files identical despite different names*

### Comparing `ream2-2.8.0/ream/actors/enum.py` & `ream2-2.8.1/ream/actors/enum.py`

 * *Files identical despite different names*

### Comparing `ream2-2.8.0/ream/cache_helper.py` & `ream2-2.8.1/ream/cache_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.8.0/ream/cli_helper.py` & `ream2-2.8.1/ream/cli_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.8.0/ream/data_model_helper.py` & `ream2-2.8.1/ream/data_model_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.8.0/ream/dataset_helper.py` & `ream2-2.8.1/ream/dataset_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.8.0/ream/fs.py` & `ream2-2.8.1/ream/fs.py`

 * *Files identical despite different names*

### Comparing `ream2-2.8.0/ream/helper.py` & `ream2-2.8.1/ream/helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.8.0/ream/params_helper.py` & `ream2-2.8.1/ream/params_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.8.0/ream/prelude.py` & `ream2-2.8.1/ream/prelude.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,24 @@
+from ream.actor_graph import ActorEdge, ActorGraph, ActorNode
 from ream.actor_state import ActorState
 from ream.actor_version import ActorVersion
-from ream.fs import FS, FSPath
-from ream.params_helper import (
-    EnumParams,
-    NoParams,
-    param_as_dict,
-)
-from ream.workspace import ReamWorkspace
-from ream.actors.interface import Actor
 from ream.actors.base import BaseActor
-from ream.actor_graph import ActorGraph, ActorNode, ActorEdge
-from ream.dataset_helper import DatasetQuery, DatasetDict
-from ream.cache_helper import Cache, CacheArgsHelper, Cacheable
-from ream.helper import configure_loguru
+from ream.actors.interface import Actor
+from ream.cache_helper import Cache, Cacheable, CacheArgsHelper
 from ream.data_model_helper import (
     NumpyDataModel,
     NumpyDataModelContainer,
     NumpyDataModelHelper,
+    SingleNumpyArray,
 )
+from ream.dataset_helper import DatasetDict, DatasetQuery
+from ream.fs import FS, FSPath
+from ream.helper import configure_loguru
+from ream.params_helper import EnumParams, NoParams, param_as_dict
+from ream.workspace import ReamWorkspace
 
 __all__ = [
     "Actor",
     "BaseActor",
     "ActorState",
     "ActorVersion",
     "FS",
@@ -38,8 +35,9 @@
     "configure_loguru",
     "Cache",
     "CacheArgsHelper",
     "Cacheable",
     "NumpyDataModel",
     "NumpyDataModelContainer",
     "NumpyDataModelHelper",
+    "SingleNumpyArray",
 ]
```

### Comparing `ream2-2.8.0/ream/workspace.py` & `ream2-2.8.1/ream/workspace.py`

 * *Files identical despite different names*

### Comparing `ream2-2.8.0/PKG-INFO` & `ream2-2.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ream2
-Version: 2.8.0
+Version: 2.8.1
 Summary: An actor architecture for research software
 Home-page: https://github.com/binh-vu/ream
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

