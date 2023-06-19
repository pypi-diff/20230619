# Comparing `tmp/smqtk-detection-0.19.0.tar.gz` & `tmp/smqtk_detection-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smqtk-detection-0.19.0.tar", max compression
+gzip compressed data, was "smqtk_detection-0.20.0.tar", max compression
```

## Comparing `smqtk-detection-0.19.0.tar` & `smqtk_detection-0.20.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1481 2022-06-02 17:32:49.701158 smqtk-detection-0.19.0/LICENSE.txt
--rw-r--r--   0        0        0      724 2022-06-02 17:32:49.701158 smqtk-detection-0.19.0/README.md
--rw-r--r--   0        0        0     2950 2022-06-02 17:32:49.701158 smqtk-detection-0.19.0/pyproject.toml
--rw-r--r--   0        0        0      375 2022-06-02 17:32:49.701158 smqtk-detection-0.19.0/smqtk_detection/__init__.py
--rw-r--r--   0        0        0      598 2022-06-02 17:32:49.701158 smqtk-detection-0.19.0/smqtk_detection/_defaults.py
--rw-r--r--   0        0        0     2413 2022-06-02 17:32:49.701158 smqtk-detection-0.19.0/smqtk_detection/detection_element_factory.py
--rw-r--r--   0        0        0      139 2022-06-02 17:32:49.701158 smqtk-detection-0.19.0/smqtk_detection/exceptions.py
--rw-r--r--   0        0        0        0 2022-06-02 17:32:49.701158 smqtk-detection-0.19.0/smqtk_detection/impls/__init__.py
--rw-r--r--   0        0        0        0 2022-06-02 17:32:49.701158 smqtk-detection-0.19.0/smqtk_detection/impls/detect_image_objects/__init__.py
--rw-r--r--   0        0        0    44153 2022-06-02 17:32:49.701158 smqtk-detection-0.19.0/smqtk_detection/impls/detect_image_objects/centernet.py
--rw-r--r--   0        0        0     2045 2022-06-02 17:32:49.701158 smqtk-detection-0.19.0/smqtk_detection/impls/detect_image_objects/random_detector.py
--rw-r--r--   0        0        0    10528 2022-06-02 17:32:49.701158 smqtk-detection-0.19.0/smqtk_detection/impls/detect_image_objects/resnet_frcnn.py
--rw-r--r--   0        0        0        0 2022-06-02 17:32:49.701158 smqtk-detection-0.19.0/smqtk_detection/impls/detection_element/__init__.py
--rw-r--r--   0        0        0     4395 2022-06-02 17:32:49.701158 smqtk-detection-0.19.0/smqtk_detection/impls/detection_element/memory.py
--rw-r--r--   0        0        0        0 2022-06-02 17:32:49.701158 smqtk-detection-0.19.0/smqtk_detection/interfaces/__init__.py
--rw-r--r--   0        0        0     1268 2022-06-02 17:32:49.701158 smqtk-detection-0.19.0/smqtk_detection/interfaces/detect_image_objects.py
--rw-r--r--   0        0        0     6667 2022-06-02 17:32:49.701158 smqtk-detection-0.19.0/smqtk_detection/interfaces/detection_element.py
--rw-r--r--   0        0        0    13957 2022-06-02 17:32:49.701158 smqtk-detection-0.19.0/smqtk_detection/interfaces/object_detector.py
--rw-r--r--   0        0        0        0 2022-06-02 17:32:49.701158 smqtk-detection-0.19.0/smqtk_detection/py.typed
--rw-r--r--   0        0        0        0 2022-06-02 17:32:49.701158 smqtk-detection-0.19.0/smqtk_detection/utils/__init__.py
--rw-r--r--   0        0        0      272 2022-06-02 17:32:49.701158 smqtk-detection-0.19.0/smqtk_detection/utils/bbox.py
--rw-r--r--   0        0        0     2678 2022-06-02 17:33:31.554847 smqtk-detection-0.19.0/setup.py
--rw-r--r--   0        0        0     2171 2022-06-02 17:33:31.555348 smqtk-detection-0.19.0/PKG-INFO
+-rw-r--r--   0        0        0     1481 2023-06-19 04:37:19.832070 smqtk_detection-0.20.0/LICENSE.txt
+-rw-r--r--   0        0        0      510 2023-06-19 04:37:19.832070 smqtk_detection-0.20.0/README.md
+-rw-r--r--   0        0        0     3201 2023-06-19 04:37:19.832070 smqtk_detection-0.20.0/pyproject.toml
+-rw-r--r--   0        0        0      375 2023-06-19 04:37:19.832070 smqtk_detection-0.20.0/smqtk_detection/__init__.py
+-rw-r--r--   0        0        0      598 2023-06-19 04:37:19.832070 smqtk_detection-0.20.0/smqtk_detection/_defaults.py
+-rw-r--r--   0        0        0     2413 2023-06-19 04:37:19.832070 smqtk_detection-0.20.0/smqtk_detection/detection_element_factory.py
+-rw-r--r--   0        0        0      139 2023-06-19 04:37:19.832070 smqtk_detection-0.20.0/smqtk_detection/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-19 04:37:19.832070 smqtk_detection-0.20.0/smqtk_detection/impls/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 04:37:19.832070 smqtk_detection-0.20.0/smqtk_detection/impls/detect_image_objects/__init__.py
+-rw-r--r--   0        0        0    44130 2023-06-19 04:37:19.832070 smqtk_detection-0.20.0/smqtk_detection/impls/detect_image_objects/centernet.py
+-rw-r--r--   0        0        0     2045 2023-06-19 04:37:19.832070 smqtk_detection-0.20.0/smqtk_detection/impls/detect_image_objects/random_detector.py
+-rw-r--r--   0        0        0    10528 2023-06-19 04:37:19.832070 smqtk_detection-0.20.0/smqtk_detection/impls/detect_image_objects/resnet_frcnn.py
+-rw-r--r--   0        0        0        0 2023-06-19 04:37:19.832070 smqtk_detection-0.20.0/smqtk_detection/impls/detection_element/__init__.py
+-rw-r--r--   0        0        0     4395 2023-06-19 04:37:19.832070 smqtk_detection-0.20.0/smqtk_detection/impls/detection_element/memory.py
+-rw-r--r--   0        0        0        0 2023-06-19 04:37:19.832070 smqtk_detection-0.20.0/smqtk_detection/interfaces/__init__.py
+-rw-r--r--   0        0        0     1268 2023-06-19 04:37:19.832070 smqtk_detection-0.20.0/smqtk_detection/interfaces/detect_image_objects.py
+-rw-r--r--   0        0        0     6667 2023-06-19 04:37:19.832070 smqtk_detection-0.20.0/smqtk_detection/interfaces/detection_element.py
+-rw-r--r--   0        0        0    14171 2023-06-19 04:37:19.832070 smqtk_detection-0.20.0/smqtk_detection/interfaces/object_detector.py
+-rw-r--r--   0        0        0        0 2023-06-19 04:37:19.832070 smqtk_detection-0.20.0/smqtk_detection/py.typed
+-rw-r--r--   0        0        0        0 2023-06-19 04:37:19.832070 smqtk_detection-0.20.0/smqtk_detection/utils/__init__.py
+-rw-r--r--   0        0        0      272 2023-06-19 04:37:19.832070 smqtk_detection-0.20.0/smqtk_detection/utils/bbox.py
+-rw-r--r--   0        0        0     2030 1970-01-01 00:00:00.000000 smqtk_detection-0.20.0/PKG-INFO
```

### Comparing `smqtk-detection-0.19.0/LICENSE.txt` & `smqtk_detection-0.20.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smqtk-detection-0.19.0/pyproject.toml` & `smqtk_detection-0.20.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,75 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "smqtk-detection"
-version = "0.19.0"
+version = "0.20.0"
 description = "Algorithms, data structures and utilities around performing detection of inputs"
 license = "BSD-3-Clause"
 authors = ["Kitware, Inc. <smqtk-developers@kitware.com>"]
 readme = "README.md"
 repository = "https://github.com/Kitware/SMQTK-Detection"
 documentation = ""
 classifiers = [
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Unix',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6.2,<3.10"
+python = "^3.8"
 smqtk-core = ">=0.18.0"
 smqtk-classifier = ">=0.19.0"
 smqtk-dataprovider = ">=0.16.0"
-smqtk-image-io = ">=0.16.2"
-torch = {version = "^1.10.0", optional = true}
-torchvision = {version = "^0.11.1", optional = true}
-opencv-python = {version = "~4.5.2.0", optional = true}
-numba = {version = "~0.53.0", optional = true}
+smqtk-image-io = [
+    { version = ">=0.16.2", python = "<3.11" },
+    { version = ">=0.17.0", python=">=3.11"}
+]
+torch = {version = ">=1.10.0,!=2.0.1", optional = true}
+torchvision = {version = ">=0.11.1", optional = true}
+opencv-python = {version = ">=4.5.2.0", optional = true}
+numba = {version = ">=0.56.4", optional = true}
 
 [tool.poetry.extras]
 torch = [ "torch", "torchvision" ]
 centernet = [ "torch", "opencv-python", "numba" ]
 
 [tool.poetry.dev-dependencies]
 #CI
-flake8 = "^3.8.3"
-flake8-mutable = "^1.2.0"
+flake8 = [
+    # Hinge because 6.0 minimum supported python version is 3.8.1
+    { version = ">=5", python = "<3.8.1" },
+    { version = ">=6", python = ">=3.8.1" }
+]
+flake8-mutable = ">=1.2.0"
 mypy = ">=0.790"
 #Docs
-Sphinx = "^3.2.1"
+Sphinx = ">=3.2.1"
 sphinx-rtd-theme = ">=0.5.0"
 sphinx-argparse = ">=0.2.5"
-sphinx-prompt = "^1.3.0"
-livereload = "^2.6.3"
+sphinx-prompt = ">=1.3.0"
+livereload = ">=2.6.3"
 # Testing
-coverage = "^6"
-pytest = "^6"
-pytest-cov = "^3"
-requests = "^2.26.0"
-types-requests = "^2.26.0"
+coverage = ">=6"
+pytest = ">=6"
+pytest-cov = ">=3"
+requests = ">=2.26.0"
+types-requests = ">=2.26.0"
 # Development
-ipython = "^7.16.3"
+ipython = ">=7.16.3"
 
 [tool.poetry.plugins."smqtk_plugins"]
 # Detection Element
 "smqtk_detection.impls.detection_element.memory" = "smqtk_detection.impls.detection_element.memory"
 "smqtk_detection.impls.detect_image_objects.random_detector" = "smqtk_detection.impls.detect_image_objects.random_detector"
 "smqtk_detection.impls.detect_image_objects.resnet_frcnn" = "smqtk_detection.impls.detect_image_objects.resnet_frcnn"
 "smqtk_detection.impls.detect_image_objects.centernet" = "smqtk_detection.impls.detect_image_objects.centernet"
```

### Comparing `smqtk-detection-0.19.0/smqtk_detection/_defaults.py` & `smqtk_detection-0.20.0/smqtk_detection/_defaults.py`

 * *Files identical despite different names*

### Comparing `smqtk-detection-0.19.0/smqtk_detection/detection_element_factory.py` & `smqtk_detection-0.20.0/smqtk_detection/detection_element_factory.py`

 * *Files identical despite different names*

### Comparing `smqtk-detection-0.19.0/smqtk_detection/impls/detect_image_objects/centernet.py` & `smqtk_detection-0.20.0/smqtk_detection/impls/detect_image_objects/centernet.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     def __init__(
         self,
         arch: str,
         model_file: str,
         max_dets: int = 100,
         k: int = 500,
-        scales: List[float] = None,
+        scales: Optional[List[float]] = None,
         flip: bool = False,
         nms: bool = True,
         use_cuda: bool = False,
         batch_size: int = 1,
         num_workers: int = 0,
     ):
         """
@@ -447,15 +447,15 @@
         """
         Initialized CenterNet model using provided .pth file.
         """
         start_epoch = 0
         checkpoint = torch.load(model_path, map_location=lambda storage, loc: storage)
         logger.info(f'loaded {model_path}, epoch {checkpoint["epoch"]}')
         state_dict_ = checkpoint["state_dict"]
-        state_dict = {}  # type: Dict[str, torch.Tensor]
+        state_dict = {}
 
         # convert data_parallal to model
         for k in state_dict_:
             if k.startswith("module") and not k.startswith("module_list"):
                 state_dict[k[7:]] = state_dict_[k]
             else:
                 state_dict[k] = state_dict_[k]
```

### Comparing `smqtk-detection-0.19.0/smqtk_detection/impls/detect_image_objects/random_detector.py` & `smqtk_detection-0.20.0/smqtk_detection/impls/detect_image_objects/random_detector.py`

 * *Files identical despite different names*

### Comparing `smqtk-detection-0.19.0/smqtk_detection/impls/detect_image_objects/resnet_frcnn.py` & `smqtk_detection-0.20.0/smqtk_detection/impls/detect_image_objects/resnet_frcnn.py`

 * *Files identical despite different names*

### Comparing `smqtk-detection-0.19.0/smqtk_detection/impls/detection_element/memory.py` & `smqtk_detection-0.20.0/smqtk_detection/impls/detection_element/memory.py`

 * *Files identical despite different names*

### Comparing `smqtk-detection-0.19.0/smqtk_detection/interfaces/detect_image_objects.py` & `smqtk_detection-0.20.0/smqtk_detection/interfaces/detect_image_objects.py`

 * *Files identical despite different names*

### Comparing `smqtk-detection-0.19.0/smqtk_detection/interfaces/detection_element.py` & `smqtk_detection-0.20.0/smqtk_detection/interfaces/detection_element.py`

 * *Files identical despite different names*

### Comparing `smqtk-detection-0.19.0/smqtk_detection/interfaces/object_detector.py` & `smqtk_detection-0.20.0/smqtk_detection/interfaces/object_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import abc
 import hashlib
 
 import numpy
 
-from typing import Hashable, Set, Iterator, Dict, Tuple, Any, Type, TypeVar
+from typing import Optional, Hashable, Set, Iterator, Dict, Tuple, Any, Type, TypeVar
 
 from smqtk_core import Plugfigurable
 from smqtk_image_io.interfaces.image_reader import ImageReader
 from smqtk_dataprovider import ContentTypeValidator
 from smqtk_core.configuration import (
     make_default_config,
     from_config_dict,
@@ -68,15 +68,15 @@
         return hashlib.sha1(bytes(hashable, "utf8")).hexdigest()
 
     def detect_objects(
             self,
             data_element: DataElement,
             de_factory: DetectionElementFactory = DFLT_DETECTION_FACTORY,
             ce_factory: ClassificationElementFactory = DFLT_CLASSIFIER_FACTORY
-    ) -> Iterator[DetectionElement]:
+    ) -> Optional[Iterator[DetectionElement]]:
         """
         Detect objects in the given data.
 
         UUIDs of detections are based on the hash produced from the combination
         of:
 
         - Detection bounding-box bounding coordinates
@@ -105,26 +105,32 @@
         self.raise_valid_element(data_element)
 
         # We know that the UUID of a DataElement should be a checksum of sorts,
         # so we can generally assume a string-cast is unique preserving.
         de_uuid = str(data_element.uuid())
 
         type_str = 'object detection classification'
-        for bbox, c_map in self._detect_objects(data_element):
+        dets = self._detect_objects(data_element)
+        if dets is None:
+            return None
+        for bbox, c_map in dets:
             # Determine UUID of detection from bbox and classification labels
             det_uuid = self._gen_detection_uuid(de_uuid, bbox, c_map.keys())
 
             ce = ce_factory.new_classification(type_str, det_uuid)
             ce.set_classification(c_map)
 
             de = de_factory.new_detection(det_uuid).set_detection(bbox, ce)
             yield de
 
     @abc.abstractmethod
-    def _detect_objects(self, data: DataElement) -> Iterator[Tuple[AxisAlignedBoundingBox, Dict[Hashable, float]]]:
+    def _detect_objects(
+            self,
+            data: DataElement
+    ) -> Optional[Iterator[Tuple[AxisAlignedBoundingBox, Dict[Hashable, float]]]]:
         """
         Internal method that defines the generation of paired bounding boxes
         and classification maps for detected objects in the given data.
 
         :param smqtk.representation.DataElement data:
             Source data (DataElement) from which to detect objects within.
 
@@ -274,15 +280,18 @@
 
         :return: True if the given element has a valid content type as reported
             by ``valid_content_types``, and False if not.
         :rtype: bool
         """
         return self._image_reader.is_valid_element(data_element)
 
-    def _detect_objects(self, data: DataElement) -> Iterator[Tuple[AxisAlignedBoundingBox, Dict[Hashable, float]]]:
+    def _detect_objects(
+            self,
+            data: DataElement
+    ) -> Optional[Iterator[Tuple[AxisAlignedBoundingBox, Dict[Hashable, float]]]]:
         """
         Internal method that defines the generation of paired bounding boxes
         and classification maps for detected objects in the given data.
 
         This ``ImageMatrixObjectDetector`` implementation ensures that the data
         element is converted to a :class:`numpy.ndarray` before passing the result
         matrix along to the :func:`_detect_objects_matrix` method for the
@@ -298,17 +307,19 @@
             keys are classification labels and values are classification
             probabilities.
         :rtype:
             collections.abc.Iterator[(smqtk.representation.AxisAlignedBoundingBox,
                                       dict[collections.abc.Hashable, float])]
 
         """
-        return self._detect_objects_matrix(
-            self._image_reader.load_as_matrix(data)
-        )
+        mat = self._image_reader.load_as_matrix(data)
+        if mat is None:
+            return None
+
+        return self._detect_objects_matrix(mat)
 
     @abc.abstractmethod
     def _detect_objects_matrix(self, mat: numpy.ndarray) \
             -> Iterator[Tuple[AxisAlignedBoundingBox, Dict[Hashable, float]]]:
         """
         Internal method to be implemented that defines the generation of paired
         bounding boxes and classification maps for detected objects in the given
```

### Comparing `smqtk-detection-0.19.0/PKG-INFO` & `smqtk_detection-0.20.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 Metadata-Version: 2.1
 Name: smqtk-detection
-Version: 0.19.0
+Version: 0.20.0
 Summary: Algorithms, data structures and utilities around performing detection of inputs
 Home-page: https://github.com/Kitware/SMQTK-Detection
 License: BSD-3-Clause
 Author: Kitware, Inc.
 Author-email: smqtk-developers@kitware.com
-Requires-Python: >=3.6.2,<3.10
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: centernet
 Provides-Extra: torch
-Requires-Dist: numba (>=0.53.0,<0.54.0); extra == "centernet"
-Requires-Dist: opencv-python (>=4.5.2.0,<4.6.0.0); extra == "centernet"
+Requires-Dist: numba (>=0.56.4) ; extra == "centernet"
+Requires-Dist: opencv-python (>=4.5.2.0) ; extra == "centernet"
 Requires-Dist: smqtk-classifier (>=0.19.0)
 Requires-Dist: smqtk-core (>=0.18.0)
 Requires-Dist: smqtk-dataprovider (>=0.16.0)
-Requires-Dist: smqtk-image-io (>=0.16.2)
-Requires-Dist: torch (>=1.10.0,<2.0.0); extra == "torch" or extra == "centernet"
-Requires-Dist: torchvision (>=0.11.1,<0.12.0); extra == "torch"
+Requires-Dist: smqtk-image-io (>=0.16.2) ; python_version < "3.11"
+Requires-Dist: smqtk-image-io (>=0.17.0) ; python_version >= "3.11"
+Requires-Dist: torch (>=1.10.0,!=2.0.1) ; extra == "torch" or extra == "centernet"
+Requires-Dist: torchvision (>=0.11.1) ; extra == "torch"
 Project-URL: Repository, https://github.com/Kitware/SMQTK-Detection
 Description-Content-Type: text/markdown
 
+# SMQTK - Detection
+
 ## Intent
+This package provides interfaces and support for black-box object detection.
 
 ## Documentation
+Documentation is [hosted on ReadTheDocs.io here](
+https://smqtk-detection.readthedocs.io/en/stable/).
 
-Documentation for SMQTK is maintained at
-[ReadtheDocs](https://smqtk.readthedocs.org), including
-[build instructions](https://smqtk.readthedocs.io/en/latest/installation.html)
-and [examples](https://smqtk.readthedocs.org/en/latest/examples/overview.html).
-
-Alternatively, you can build the sphinx documentation locally for the most
-up-to-date reference (see also: [Building the Documentation](
-https://smqtk.readthedocs.io/en/latest/installation.html#building-the-documentation)):
+You can build the sphinx documentation locally for the most up-to-date
+reference:
 ```bash
+# Install dependencies
+poetry install
 # Navigate to the documentation root.
 cd docs
-# Install dependencies and build Sphinx docs.
-pip install -r readthedocs-reqs.txt
-make html
+# Build the docs.
+poetry run make html
 # Open in your favorite browser!
 firefox _build/html/index.html
 ```
```

