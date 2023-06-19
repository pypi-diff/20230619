# Comparing `tmp/pytdml-1.0.0.tar.gz` & `tmp/pytdml-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pytdml-1.0.0.tar", last modified: Wed May  4 08:54:30 2022, max compression
+gzip compressed data, was "pytdml-1.1.1.tar", last modified: Tue Mar 28 08:09:03 2023, max compression
```

## Comparing `pytdml-1.0.0.tar` & `pytdml-1.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2022-05-04 08:54:30.000000 pytdml-1.0.0/
--rw-rw-rw-   0        0        0     1120 2022-05-04 07:02:44.000000 pytdml-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     7429 2022-05-04 08:54:30.000000 pytdml-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6573 2022-05-04 08:48:44.000000 pytdml-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2022-05-04 08:54:30.000000 pytdml-1.0.0/examples/
--rw-rw-rw-   0        0        0        0 2022-04-21 07:23:25.000000 pytdml-1.0.0/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 08:54:30.000000 pytdml-1.0.0/pytdml/
--rw-rw-rw-   0        0        0     1590 2022-05-04 08:54:14.000000 pytdml-1.0.0/pytdml/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 08:54:30.000000 pytdml-1.0.0/pytdml/io/
--rw-rw-rw-   0        0        0     1627 2022-05-04 07:07:22.000000 pytdml-1.0.0/pytdml/io/__init__.py
--rw-rw-rw-   0        0        0     2183 2022-05-04 07:07:25.000000 pytdml-1.0.0/pytdml/io/tdml_readers.py
--rw-rw-rw-   0        0        0     1879 2022-05-04 07:07:33.000000 pytdml-1.0.0/pytdml/io/tdml_writers.py
-drwxrwxrwx   0        0        0        0 2022-05-04 08:54:30.000000 pytdml-1.0.0/pytdml/ml/
--rw-rw-rw-   0        0        0     1854 2022-05-04 08:28:17.000000 pytdml-1.0.0/pytdml/ml/__init__.py
--rw-rw-rw-   0        0        0     2640 2022-05-04 07:07:09.000000 pytdml-1.0.0/pytdml/ml/ml_operators.py
--rw-rw-rw-   0        0        0     6151 2022-05-04 07:06:44.000000 pytdml-1.0.0/pytdml/ml/tdml_tensorflow.py
--rw-rw-rw-   0        0        0     5396 2022-05-04 07:07:16.000000 pytdml-1.0.0/pytdml/ml/tdml_torch.py
--rw-rw-rw-   0        0        0     4988 2022-05-04 08:13:09.000000 pytdml-1.0.0/pytdml/tdml_image_crop.py
-drwxrwxrwx   0        0        0        0 2022-05-04 08:54:30.000000 pytdml-1.0.0/pytdml/type/
--rw-rw-rw-   0        0        0     1837 2022-05-04 07:06:08.000000 pytdml-1.0.0/pytdml/type/__init__.py
--rw-rw-rw-   0        0        0    14394 2022-05-04 07:06:28.000000 pytdml-1.0.0/pytdml/type/basic_types.py
--rw-rw-rw-   0        0        0    14770 2022-05-04 07:06:22.000000 pytdml-1.0.0/pytdml/type/extended_types.py
--rw-rw-rw-   0        0        0     4537 2022-05-04 07:05:55.000000 pytdml-1.0.0/pytdml/utils.py
--rw-rw-rw-   0        0        0    14079 2022-05-04 07:48:39.000000 pytdml-1.0.0/pytdml/yaml_to_tdml.py
-drwxrwxrwx   0        0        0        0 2022-05-04 08:54:30.000000 pytdml-1.0.0/pytdml.egg-info/
--rw-rw-rw-   0        0        0     7429 2022-05-04 08:54:30.000000 pytdml-1.0.0/pytdml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      554 2022-05-04 08:54:30.000000 pytdml-1.0.0/pytdml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-04 08:54:30.000000 pytdml-1.0.0/pytdml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2022-05-04 08:54:30.000000 pytdml-1.0.0/pytdml.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2022-05-04 08:54:30.000000 pytdml-1.0.0/pytdml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-04 08:54:30.000000 pytdml-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     3147 2022-05-04 07:05:21.000000 pytdml-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-04 08:54:30.000000 pytdml-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2021-12-21 13:48:43.000000 pytdml-1.0.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-28 08:09:03.503695 pytdml-1.1.1/
+-rw-rw-rw-   0        0        0     1141 2023-03-24 06:36:34.000000 pytdml-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     7407 2023-03-28 08:09:03.503695 pytdml-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6805 2023-03-24 06:36:34.000000 pytdml-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-03-28 08:09:03.471837 pytdml-1.1.1/examples/
+-rw-rw-rw-   0        0        0        0 2023-03-24 06:36:34.000000 pytdml-1.1.1/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-28 08:09:03.474823 pytdml-1.1.1/pytdml/
+-rw-rw-rw-   0        0        0     1608 2023-03-28 08:08:49.000000 pytdml-1.1.1/pytdml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-28 08:09:03.497725 pytdml-1.1.1/pytdml/io/
+-rw-rw-rw-   0        0        0     1629 2023-03-27 11:13:28.000000 pytdml-1.1.1/pytdml/io/__init__.py
+-rw-rw-rw-   0        0        0     2250 2023-03-28 08:04:38.000000 pytdml-1.1.1/pytdml/io/tdml_readers.py
+-rw-rw-rw-   0        0        0     1959 2023-03-28 08:04:30.000000 pytdml-1.1.1/pytdml/io/tdml_writers.py
+drwxrwxrwx   0        0        0        0 2023-03-28 08:09:03.499712 pytdml-1.1.1/pytdml/ml/
+-rw-rw-rw-   0        0        0     1854 2023-03-24 06:36:35.000000 pytdml-1.1.1/pytdml/ml/__init__.py
+-rw-rw-rw-   0        0        0     2640 2023-03-24 06:36:35.000000 pytdml-1.1.1/pytdml/ml/ml_operators.py
+-rw-rw-rw-   0        0        0     6151 2023-03-24 06:36:35.000000 pytdml-1.1.1/pytdml/ml/tdml_tensorflow.py
+-rw-rw-rw-   0        0        0     5396 2023-03-24 06:36:35.000000 pytdml-1.1.1/pytdml/ml/tdml_torch.py
+-rw-rw-rw-   0        0        0     4988 2023-03-24 06:36:35.000000 pytdml-1.1.1/pytdml/tdml_image_crop.py
+drwxrwxrwx   0        0        0        0 2023-03-28 08:09:03.501701 pytdml-1.1.1/pytdml/type/
+-rw-rw-rw-   0        0        0     1828 2023-03-28 07:45:12.000000 pytdml-1.1.1/pytdml/type/__init__.py
+-rw-rw-rw-   0        0        0    22698 2023-03-28 07:44:06.000000 pytdml-1.1.1/pytdml/type/basic_types.py
+-rw-rw-rw-   0        0        0    16253 2023-03-28 07:44:06.000000 pytdml-1.1.1/pytdml/type/extended_types.py
+-rw-rw-rw-   0        0        0     4537 2023-03-24 06:36:35.000000 pytdml-1.1.1/pytdml/utils.py
+-rw-rw-rw-   0        0        0    15294 2023-03-28 07:52:13.000000 pytdml-1.1.1/pytdml/yaml_to_tdml.py
+drwxrwxrwx   0        0        0        0 2023-03-28 08:09:03.495770 pytdml-1.1.1/pytdml.egg-info/
+-rw-rw-rw-   0        0        0     7407 2023-03-28 08:09:03.000000 pytdml-1.1.1/pytdml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-03-28 08:09:03.000000 pytdml-1.1.1/pytdml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-28 08:09:03.000000 pytdml-1.1.1/pytdml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-03-28 08:09:03.000000 pytdml-1.1.1/pytdml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-03-28 08:09:03.000000 pytdml-1.1.1/pytdml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-28 08:09:03.503695 pytdml-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     3136 2023-03-27 09:56:30.000000 pytdml-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-28 08:09:03.502701 pytdml-1.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-24 06:36:35.000000 pytdml-1.1.1/tests/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytdml-1.0.0/PKG-INFO` & `pytdml-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pytdml
-Version: 1.0.0
+Version: 1.1.1
 Summary: Parsing and encoding training datasets based on OGC Training Data Markup Language for AI (TrainingDML-AI) standard
 Home-page: https://github.com/TrainingDML/pytdml
 Author: Boyi Shangguan
 Author-email: sgby@whu.edu.cn
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -51,15 +50,15 @@
 
 The training dataset can be encoded to TrainingDML-AI JSON format by YAML configuration file with command line.
 
 ```bash
 pytdml/yaml_to_tdml.py --config=<YAML configuration file path> --output=<Output TrainingDML-AI JSON file path>
 ```
 
-YAML configuration file schema is described in [encoding YAML configuration file schema](https://github.com/TrainingDML/pytdml/blob/main/encoding_config_schema.yaml).
+YAML configuration file schema is described in [encoding YAML configuration file schema](https://github.com/TrainingDML/pytdml/blob/main/encoding_config_schema.yml).
 
 #### Using the API from python
 
 The training dataset can also be encoded to TrainingDML-AI JSON format with Python API.
 
 ```python
 from pytdml.io import write_to_json
@@ -242,8 +241,7 @@
 
 The images of training dataset in TrainingDML-AI JSON format can be cropped with command line for preprocessing.
 
 ```bash
 pytdml/tdml_image_crop.py  --input=<Input original TrainingDML-AU file path> --output_json=<Output result TrainingDML-AI JSON file path>
                           --output_images=<Output dir of result cropped images> --size=<Crop size of images>
 ```
-
```

### Comparing `pytdml-1.0.0/README.md` & `pytdml-1.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,233 +1,233 @@
-# pytdml
-
-[pytdml](https://github.com/TrainingDML/pytdml) is a pure python parser and encoder for training datasets based on OGC
-Training Data Markup Language for AI standard.
-
----
-
-## Installation
-
-The package can be installed via pip.
-
-### Requirements
-
-* Python 3 and above
-
-### Dependencies
-
-Dependencies are listed in [requirements.txt](https://github.com/TrainingDML/pytdml/blob/main/requirements.txt). Dependencies are automatically installed during
-pytdml's installation.
-
-### Installing the Package
-
-```bash
-pip install pytdml
-```
-
----
-
-## Usage
-
-### Encoding
-
-#### From the command line
-
-The training dataset can be encoded to TrainingDML-AI JSON format by YAML configuration file with command line.
-
-```bash
-pytdml/yaml_to_tdml.py --config=<YAML configuration file path> --output=<Output TrainingDML-AI JSON file path>
-```
-
-YAML configuration file schema is described in [encoding YAML configuration file schema](https://github.com/TrainingDML/pytdml/blob/main/encoding_config_schema.yaml).
-
-#### Using the API from python
-
-The training dataset can also be encoded to TrainingDML-AI JSON format with Python API.
-
-```python
-from pytdml.io import write_to_json
-from pytdml.type import EOTrainingDataset, EOTrainingData, EOTask, EODataSource, SceneLabel
-
-# generate EO training dataset
-dataset = EOTrainingDataset(
-    id='...',
-    name='...',
-    description='...',
-    data=[
-        EOTrainingData(
-            id='...',
-            labels=[
-                SceneLabel(
-                    label_class='...',
-                    data_url='...',
-                    date_time='...'),
-                ...
-            ]),
-        ...
-    ],
-    version="...",
-    amount_of_training_data=...,
-    created_time="...",
-    updated_time="...",
-    providers=["..."],
-    keywords=["...", "..."],
-    tasks=[EOTask(task_type="...",
-                  description="...")],
-    data_sources=[EODataSource(
-        id="...",
-        data_type="...",
-        resolution="..."
-    )],
-    classes=["...", "...", "..."],
-    number_of_classes=...,
-    bands=["...", "...", "..."],
-    image_size="..."
-)
-# write to json
-write_to_json(dataset, "dataset.json")
-```
-
-### Parsing
-
-The training dataset described with TrainingDML-AI JSON file can be parsed with python API and transformed to
-PyTorch/TensorFlow dataset.
-
-#### Read TrainingDataset object from JSON file
-
-```python
-import pytdml
-
-training_dataset = pytdml.io.read_from_json("dataset.json")  # read from TDML json file
-print("Load training dataset: " + training_dataset.name)
-print("Number of training samples: " + str(training_dataset.amount_of_training_data))
-print("Number of classes: " + str(training_dataset.number_of_classes))
-```
-
-#### Transform to PyTorch dataset
-
-* Scene classification dataset
-
-```python
-import pytdml
-from torchvision import transforms
-
-# Load the training dataset
-training_dataset = pytdml.io.read_from_json("dataset.json")  # read from TDML json file
-
-# Transform the training dataset
-class_map = pytdml.ml.creat_class_map(training_dataset)  # create class map
-train_dataset = pytdml.ml.TorchEOImageSceneTD(  # create Torch train dataset
-    training_dataset.data,
-    class_map,
-    transform=transforms.Compose(  # transform for the training set
-        [transforms.RandomResizedCrop(size=156, scale=(0.8, 1.0)),  # random resize
-         transforms.RandomRotation(degrees=15),  # random rotate
-         transforms.RandomHorizontalFlip(),  # random flip
-         transforms.CenterCrop(size=124),  # center crop
-         transforms.ToTensor(),  # transform to tensor
-         transforms.Normalize([0.485, 0.456, 0.406], [0.229, 0.224, 0.225])  # normalize
-         ]
-    ))
-```
-
-* Object detection dataset
-
-```python
-import pytdml
-
-# Load the training dataset
-training_dataset = pytdml.io.read_from_json("dataset.json")  # read from TDML json file
-
-# Transform the training dataset
-class_map = pytdml.ml.creat_class_map(training_dataset)  # create class map
-train_dataset = pytdml.ml.TorchEOImageObjectTD(  # create Torch train dataset
-    training_dataset.data,
-    class_map,
-    transform=pytdml.ml.BaseTransform([128, 128])
-)
-```
-
-* Semantic segmentation dataset
-
-```python
-import pytdml
-from torchvision import transforms
-
-# Load the training dataset
-training_dataset = pytdml.io.read_from_json("dataset.json")  # read from TDML json file
-
-# Transform the training dataset
-class_map = pytdml.ml.creat_class_map(training_dataset)  # create class map
-train_dataset = pytdml.ml.TorchEOImageSegmentationTD(  # create Torch train dataset
-    training_dataset.data,
-    class_map,
-    transform=transforms.Compose([
-        transforms.ToTensor(),
-        transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225])
-    ])
-)
-```
-
-#### Transform to TensorFlow dataset
-
-* Scene classification dataset
-
-```python
-import pytdml
-
-# Load the training dataset
-training_dataset = pytdml.io.read_from_json("dataset.json")  # read from TDML json file
-
-# Transform the training dataset
-class_map = pytdml.ml.creat_class_map(training_dataset)  # create class map
-train_dataset = pytdml.ml.TensorflowEOImageSceneTD(  # create TensorFlow train dataset
-    training_dataset.data,
-    class_map
-)
-tf_train_dataset = train_dataset.create_dataset()
-```
-
-* Object detection dataset
-
-```python
-import pytdml
-
-# Load the training dataset
-training_dataset = pytdml.io.read_from_json("dataset.json")  # read from TDML json file
-
-# Transform the training dataset
-class_map = pytdml.ml.creat_class_map(training_dataset)  # create class map
-train_dataset = pytdml.ml.TensorflowEOImageObjectTD(  # create TensorFlow train dataset
-    training_dataset.data,
-    class_map
-)
-tf_train_dataset = train_dataset.create_dataset()
-```
-
-* Semantic segmentation dataset
-
-```python
-import pytdml
-
-# Load the training dataset
-training_dataset = pytdml.io.read_from_json("dataset.json")  # read from TDML json file
-
-# Transform the training dataset
-class_map = pytdml.ml.creat_class_map(training_dataset)  # create class map
-train_dataset = pytdml.ml.TensorflowEOImageSegmentationTD(  # create TensorFlow train dataset
-    training_dataset.data,
-    class_map
-)
-tf_train_dataset = train_dataset.create_dataset()
-```
-
-### Image Cropping
-
-The images of training dataset in TrainingDML-AI JSON format can be cropped with command line for preprocessing.
-
-```bash
-pytdml/tdml_image_crop.py  --input=<Input original TrainingDML-AU file path> --output_json=<Output result TrainingDML-AI JSON file path>
-                          --output_images=<Output dir of result cropped images> --size=<Crop size of images>
-```
-
-
+# pytdml
+
+[pytdml](https://github.com/TrainingDML/pytdml) is a pure python parser and encoder for training datasets based on OGC
+Training Data Markup Language for AI standard.
+
+---
+
+## Installation
+
+The package can be installed via pip.
+
+### Requirements
+
+* Python 3 and above
+
+### Dependencies
+
+Dependencies are listed in [requirements.txt](https://github.com/TrainingDML/pytdml/blob/main/requirements.txt). Dependencies are automatically installed during
+pytdml's installation.
+
+### Installing the Package
+
+```bash
+pip install pytdml
+```
+
+---
+
+## Usage
+
+### Encoding
+
+#### From the command line
+
+The training dataset can be encoded to TrainingDML-AI JSON format by YAML configuration file with command line.
+
+```bash
+pytdml/yaml_to_tdml.py --config=<YAML configuration file path> --output=<Output TrainingDML-AI JSON file path>
+```
+
+YAML configuration file schema is described in [encoding YAML configuration file schema](https://github.com/TrainingDML/pytdml/blob/main/encoding_config_schema.yml).
+
+#### Using the API from python
+
+The training dataset can also be encoded to TrainingDML-AI JSON format with Python API.
+
+```python
+from pytdml.io import write_to_json
+from pytdml.type import EOTrainingDataset, EOTrainingData, EOTask, EODataSource, SceneLabel
+
+# generate EO training dataset
+dataset = EOTrainingDataset(
+    id='...',
+    name='...',
+    description='...',
+    data=[
+        EOTrainingData(
+            id='...',
+            labels=[
+                SceneLabel(
+                    label_class='...',
+                    data_url='...',
+                    date_time='...'),
+                ...
+            ]),
+        ...
+    ],
+    version="...",
+    amount_of_training_data=...,
+    created_time="...",
+    updated_time="...",
+    providers=["..."],
+    keywords=["...", "..."],
+    tasks=[EOTask(task_type="...",
+                  description="...")],
+    data_sources=[EODataSource(
+        id="...",
+        data_type="...",
+        resolution="..."
+    )],
+    classes=["...", "...", "..."],
+    number_of_classes=...,
+    bands=["...", "...", "..."],
+    image_size="..."
+)
+# write to json
+write_to_json(dataset, "dataset.json")
+```
+
+### Parsing
+
+The training dataset described with TrainingDML-AI JSON file can be parsed with python API and transformed to
+PyTorch/TensorFlow dataset.
+
+#### Read TrainingDataset object from JSON file
+
+```python
+import pytdml
+
+training_dataset = pytdml.io.read_from_json("dataset.json")  # read from TDML json file
+print("Load training dataset: " + training_dataset.name)
+print("Number of training samples: " + str(training_dataset.amount_of_training_data))
+print("Number of classes: " + str(training_dataset.number_of_classes))
+```
+
+#### Transform to PyTorch dataset
+
+* Scene classification dataset
+
+```python
+import pytdml
+from torchvision import transforms
+
+# Load the training dataset
+training_dataset = pytdml.io.read_from_json("dataset.json")  # read from TDML json file
+
+# Transform the training dataset
+class_map = pytdml.ml.creat_class_map(training_dataset)  # create class map
+train_dataset = pytdml.ml.TorchEOImageSceneTD(  # create Torch train dataset
+    training_dataset.data,
+    class_map,
+    transform=transforms.Compose(  # transform for the training set
+        [transforms.RandomResizedCrop(size=156, scale=(0.8, 1.0)),  # random resize
+         transforms.RandomRotation(degrees=15),  # random rotate
+         transforms.RandomHorizontalFlip(),  # random flip
+         transforms.CenterCrop(size=124),  # center crop
+         transforms.ToTensor(),  # transform to tensor
+         transforms.Normalize([0.485, 0.456, 0.406], [0.229, 0.224, 0.225])  # normalize
+         ]
+    ))
+```
+
+* Object detection dataset
+
+```python
+import pytdml
+
+# Load the training dataset
+training_dataset = pytdml.io.read_from_json("dataset.json")  # read from TDML json file
+
+# Transform the training dataset
+class_map = pytdml.ml.creat_class_map(training_dataset)  # create class map
+train_dataset = pytdml.ml.TorchEOImageObjectTD(  # create Torch train dataset
+    training_dataset.data,
+    class_map,
+    transform=pytdml.ml.BaseTransform([128, 128])
+)
+```
+
+* Semantic segmentation dataset
+
+```python
+import pytdml
+from torchvision import transforms
+
+# Load the training dataset
+training_dataset = pytdml.io.read_from_json("dataset.json")  # read from TDML json file
+
+# Transform the training dataset
+class_map = pytdml.ml.creat_class_map(training_dataset)  # create class map
+train_dataset = pytdml.ml.TorchEOImageSegmentationTD(  # create Torch train dataset
+    training_dataset.data,
+    class_map,
+    transform=transforms.Compose([
+        transforms.ToTensor(),
+        transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225])
+    ])
+)
+```
+
+#### Transform to TensorFlow dataset
+
+* Scene classification dataset
+
+```python
+import pytdml
+
+# Load the training dataset
+training_dataset = pytdml.io.read_from_json("dataset.json")  # read from TDML json file
+
+# Transform the training dataset
+class_map = pytdml.ml.creat_class_map(training_dataset)  # create class map
+train_dataset = pytdml.ml.TensorflowEOImageSceneTD(  # create TensorFlow train dataset
+    training_dataset.data,
+    class_map
+)
+tf_train_dataset = train_dataset.create_dataset()
+```
+
+* Object detection dataset
+
+```python
+import pytdml
+
+# Load the training dataset
+training_dataset = pytdml.io.read_from_json("dataset.json")  # read from TDML json file
+
+# Transform the training dataset
+class_map = pytdml.ml.creat_class_map(training_dataset)  # create class map
+train_dataset = pytdml.ml.TensorflowEOImageObjectTD(  # create TensorFlow train dataset
+    training_dataset.data,
+    class_map
+)
+tf_train_dataset = train_dataset.create_dataset()
+```
+
+* Semantic segmentation dataset
+
+```python
+import pytdml
+
+# Load the training dataset
+training_dataset = pytdml.io.read_from_json("dataset.json")  # read from TDML json file
+
+# Transform the training dataset
+class_map = pytdml.ml.creat_class_map(training_dataset)  # create class map
+train_dataset = pytdml.ml.TensorflowEOImageSegmentationTD(  # create TensorFlow train dataset
+    training_dataset.data,
+    class_map
+)
+tf_train_dataset = train_dataset.create_dataset()
+```
+
+### Image Cropping
+
+The images of training dataset in TrainingDML-AI JSON format can be cropped with command line for preprocessing.
+
+```bash
+pytdml/tdml_image_crop.py  --input=<Input original TrainingDML-AU file path> --output_json=<Output result TrainingDML-AI JSON file path>
+                          --output_images=<Output dir of result cropped images> --size=<Crop size of images>
+```
+
+
```

### Comparing `pytdml-1.0.0/pytdml/__init__.py` & `pytdml-1.1.1/pytdml/io/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,32 @@
-# ------------------------------------------------------------------------------
-#
-# Project: pytdml
-# Authors: Boyi Shangguan, Kaixuan Wang
-# Created: 2022-05-04
-# Email: sgby@whu.edu.cn
-#
-# ------------------------------------------------------------------------------
-#
-# Copyright (c) 2022 OGC Training Data Markup Language for AI Standard Working Group
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-#
-# ------------------------------------------------------------------------------
-import pytdml.type
-import pytdml.io
-import pytdml.ml
-
-name = 'pytdml'
-__version__ = '1.0.0'
+# ------------------------------------------------------------------------------
+#
+# Project: pytdml
+# Authors: Boyi Shangguan, Kaixuan Wang
+# Created: 2022-05-04
+# Email: sgby@whu.edu.cn
+#
+# ------------------------------------------------------------------------------
+#
+# Copyright (c) 2022 OGC Training Data Markup Language for AI Standard Working Group
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+#
+# ------------------------------------------------------------------------------
+from pytdml.io.tdml_readers import read_from_json
+from pytdml.io.tdml_writers import write_to_json
```

### Comparing `pytdml-1.0.0/pytdml/io/__init__.py` & `pytdml-1.1.1/pytdml/type/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,9 +24,11 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # ------------------------------------------------------------------------------
-from pytdml.io.tdml_readers import read_from_json
-from pytdml.io.tdml_writers import write_to_json
+from pytdml.type.basic_types import TrainingDataset, TrainingData, DataQuality, Task, Label, Labeling, Labeler, \
+    LabelingProcedure, Changeset, Scope, ScopeDescription
+from pytdml.type.extended_types import EOTrainingDataset, EOTrainingData, SceneLabel, ObjectLabel, PixelLabel, \
+    EOTask
```

### Comparing `pytdml-1.0.0/pytdml/io/tdml_writers.py` & `pytdml-1.1.1/pytdml/io/tdml_writers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# ------------------------------------------------------------------------------
-#
-# Project: pytdml
-# Authors: Boyi Shangguan, Kaixuan Wang
-# Created: 2022-05-04
-# Email: sgby@whu.edu.cn
-#
-# ------------------------------------------------------------------------------
-#
-# Copyright (c) 2022 OGC Training Data Markup Language for AI Standard Working Group
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-#
-# ------------------------------------------------------------------------------
-import json
-from typing import Union
-from pytdml.type.basic_types import TrainingDataset
-from pytdml.utils import remove_empty
-
-
-def write_to_json(td: TrainingDataset, file_path: str, indent: Union[None, int, str] = 4):
-    """
-    Writes a TrainingDataset to a JSON file.
-    """
-    with open(file_path, "w") as f:
-        json.dump(remove_empty(td.to_dict()), f, indent=indent)
+# ------------------------------------------------------------------------------
+#
+# Project: pytdml
+# Authors: Boyi Shangguan, Kaixuan Wang
+# Created: 2022-05-04
+# Email: sgby@whu.edu.cn
+#
+# ------------------------------------------------------------------------------
+#
+# Copyright (c) 2022 OGC Training Data Markup Language for AI Standard Working Group
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+#
+# ------------------------------------------------------------------------------
+import json
+from typing import Union
+from pytdml.type.basic_types import TrainingDataset
+from pytdml.utils import remove_empty
+
+
+def write_to_json(td: TrainingDataset, file_path: str, indent: Union[None, int, str] = 4):
+    """
+    Writes a TrainingDataset to a JSON file.
+    """
+    with open(file_path, "w", encoding='utf-8') as f:
+        json.dump(remove_empty(td.to_dict()), f, indent=indent, ensure_ascii=False)
```

### Comparing `pytdml-1.0.0/pytdml/ml/__init__.py` & `pytdml-1.1.1/pytdml/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.0.0/pytdml/ml/ml_operators.py` & `pytdml-1.1.1/pytdml/ml/ml_operators.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.0.0/pytdml/ml/tdml_tensorflow.py` & `pytdml-1.1.1/pytdml/ml/tdml_tensorflow.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.0.0/pytdml/ml/tdml_torch.py` & `pytdml-1.1.1/pytdml/ml/tdml_torch.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.0.0/pytdml/tdml_image_crop.py` & `pytdml-1.1.1/pytdml/tdml_image_crop.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,16 +44,16 @@
     td_dict = td.to_dict()
     td_list = td_dict['data']
     new_td_list = []
     index = 0
     for d in td_list:
         label_type = d['labels'][0]['type']
         if label_type == 'PixelLabel':
-            image_url = d['dataUrl']
-            label_url = d['labels'][0]['imageUrl']
+            image_url = d['dataURL']
+            label_url = d['labels'][0]['imageURL']
             image_dir = os.path.join(save_crop_dir, "images")
             label_dir = os.path.join(save_crop_dir, "labels")
             if not os.path.isdir(image_dir):
                 os.makedirs(image_dir)
             if not os.path.isdir(label_dir):
                 os.makedirs(label_dir)
             crop_image_list = image_crop(image_url, image_dir, sub_size)
```

### Comparing `pytdml-1.0.0/pytdml/type/__init__.py` & `pytdml-1.1.1/pytdml/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,11 +24,12 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # ------------------------------------------------------------------------------
-from pytdml.type.basic_types import TrainingDataset, TrainingData, TrainingDataQuality, Task, Label, Labeling, Labeler, \
-    LabelingProcedure
-from pytdml.type.extended_types import EOTrainingDataset, EOTrainingData, SceneLabel, ObjectLabel, PixelLabel, \
-    EODataSource, EOTask, EOTrainingDataQuality
+import pytdml.type
+import pytdml.io
+
+name = 'pytdml'
+__version__ = '1.1.1'
```

### Comparing `pytdml-1.0.0/pytdml/type/basic_types.py` & `pytdml-1.1.1/pytdml/type/extended_types.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,353 +27,314 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # ------------------------------------------------------------------------------
 from dataclasses import dataclass, field
 from typing import List, Union
 
-
-@dataclass
-class KeyValuePair:
-    """
-    Key/Value pair type
-    """
-    key: str
-    value: Union[str, int, float, bool, None]
-
-    def to_dict(self):
-        return {self.key: self.value}
-
-    @staticmethod
-    def from_dict(json_dict: dict):
-        if len(json_dict.keys()) == 1:
-            for key in json_dict.keys():
-                return KeyValuePair(key, json_dict[key])
-        else:
-            raise ValueError("The given json_dict is not a valid KeyValuePair")
+import geojson
+from geojson import Feature
+from pytdml.type.basic_types import Label, TrainingData, TrainingDataset, DataQuality, Task, \
+    MetricsInLiterature, \
+    KeyValuePair, Labeling, Changeset
 
 
 @dataclass
-class MetricsInLiterature:
+class SceneLabel(Label):
     """
-    Metrics in literature type
+    Extended label type for scene level training data
     """
-    doi: str
-    algorithm: str = field(default=None)
-    metrics: List[KeyValuePair] = field(default_factory=list)
+    label_class: str = field(default=None)
 
     def to_dict(self):
         return {
-            "doi": self.doi,
-            "algorithm": self.algorithm,
-            "metrics": [m.to_dict() for m in self.metrics]
+            "type": "SceneLabel",
+            "isNegative": self.is_negative,
+            "confidence": self.confidence,
+            'class': self.label_class
         }
 
     @staticmethod
     def from_dict(json_dict: dict):
-        if json_dict.__contains__("doi"):
-            metrics_in_literature = MetricsInLiterature(json_dict["doi"])
-            if json_dict.__contains__("algorithm"):
-                metrics_in_literature.algorithm = json_dict["algorithm"]
-            if json_dict.__contains__("metrics"):
-                metrics_in_literature.metrics = [KeyValuePair.from_dict(m) for m in json_dict["metrics"]]
-            return metrics_in_literature
+        if json_dict.__contains__("class") and json_dict["type"] == "SceneLabel":
+            label = SceneLabel(label_class=json_dict["class"])
+            if json_dict.__contains__("isNegative"):
+                label.is_negative = json_dict["isNegative"]
+            if json_dict.__contains__("confidence"):
+                label.confidence = json_dict["confidence"]
+            return label
         else:
-            raise ValueError("The given json_dict is not a valid MetricsInLiterature")
+            raise ValueError("The given json_dict is not a valid SceneLabel")
 
 
 @dataclass
-class Task:
+class ObjectLabel(Label):
     """
-    Basic task type
+    Extended label type for object level training data
     """
-    description: str = field(default=None)
+    object: Feature = field(default=None)
+    label_class: str = field(default=None)
+    bbox_type: str = field(default=None)
+    is_difficultly_detectable: bool = field(default=None)
+    date_time: str = field(default=None)
 
     def to_dict(self):
         return {
-            "type": "Task",
-            "description": self.description
+            "type": "ObjectLabel",
+            "isNegative": self.is_negative,
+            "confidence": self.confidence,
+            'object': self.object,
+            'bboxType': self.bbox_type,
+            'class': self.label_class,
+            'isDiffDetectable': self.is_difficultly_detectable,
+            'dateTime': self.date_time
         }
 
     @staticmethod
     def from_dict(json_dict: dict):
-        if json_dict["type"] == "Task":
-            task = Task()
-            if json_dict.__contains__("type"):
-                task.description = json_dict["description"]
-            return task
+        if json_dict.__contains__("object") and json_dict["type"] == "ObjectLabel":
+            label = ObjectLabel(object=geojson.loads(json_dict["object"].__str__().replace("'", "\"")))
+            if json_dict.__contains__("isNegative"):
+                label.is_negative = json_dict["isNegative"]
+            if json_dict.__contains__("confidence"):
+                label.confidence = json_dict["confidence"]
+            if json_dict.__contains__("bboxType"):
+                label.bbox_type = json_dict["bboxType"]
+            if json_dict.__contains__("class"):
+                label.label_class = json_dict["class"]
+            if json_dict.__contains__("isDiffDetectable"):
+                label.is_difficultly_detectable = json_dict["isDiffDetectable"]
+            if json_dict.__contains__("dateTime"):
+                label.date_time = json_dict["dateTime"]
+            return label
         else:
-            raise ValueError("The given json_dict is not a valid Task")
+            raise ValueError("The given json_dict is not a valid ObjectLabel")
 
 
 @dataclass
-class Labeler:
+class PixelLabel(Label):
     """
-    Labeler type
+    Extended label type for pixel level training data
     """
-    id: str
-    name: str = field(default=None)
+    image_url: Union[str, List[str]] = field(default=None)
+    image_format: Union[str, List[str]] = field(default=None)
 
     def to_dict(self):
         return {
-            "type": "Labeler",
-            "id": self.id,
-            "name": self.name
+            "type": "PixelLabel",
+            "isNegative": self.is_negative,
+            "confidence": self.confidence,
+            "imageURL": self.image_url,
+            "imageFormat": self.image_format
         }
 
     @staticmethod
     def from_dict(json_dict: dict):
-        if json_dict.__contains__("id") and json_dict["type"] == "Labeler":
-            labeler = Labeler(json_dict["id"])
-            if json_dict.__contains__("name"):
-                labeler.name = json_dict["name"]
-            return labeler
+        if json_dict.__contains__("imageURL") and json_dict.__contains__("imageFormat") \
+                and json_dict["type"] == "PixelLabel":
+            label = PixelLabel(image_url=json_dict["imageURL"], image_format=json_dict["imageFormat"])
+            if json_dict.__contains__("isNegative"):
+                label.is_negative = json_dict["isNegative"]
+            if json_dict.__contains__("confidence"):
+                label.confidence = json_dict["confidence"]
+            return label
         else:
-            raise ValueError("The given json_dict is not a valid Labeler")
-
-
-@dataclass
-class LabelingProcedure:
-    """
-    Labeling procedure type
-    """
-    id: str
-    method: str = field(default=None)
-    tool: str = field(default=None)
+            raise ValueError("The given json_dict is not a valid PixelLabel")
 
-    def to_dict(self):
-        return {
-            "type": "LabelingProcedure",
-            "id": self.id,
-            "method": self.method,
-            "tool": self.tool
-        }
 
-    @staticmethod
-    def from_dict(json_dict: dict):
-        if json_dict.__contains__("id") and json_dict["type"] == "LabelingProcedure":
-            labeling_procedure = LabelingProcedure(json_dict["id"])
-            if json_dict.__contains__("method"):
-                labeling_procedure.method = json_dict["method"]
-            if json_dict.__contains__("tool"):
-                labeling_procedure.tool = json_dict["tool"]
-            return labeling_procedure
-        else:
-            raise ValueError("The given json_dict is not a valid LabelingProcedure")
+# @dataclass
+# class EODataSource:
+#     """
+#     EO data source type
+#     """
+#     id: str
+#     data_type: str = field(default=None)
+#     citation: str = field(default=None)
+#     platform: str = field(default=None)
+#     sensor: str = field(default=None)
+#     resolution: str = field(default=None)
+#     format: str = field(default=None)
+#
+#     def to_dict(self):
+#         return {
+#             'id': self.id,
+#             'dataType': self.data_type,
+#             'citation': self.citation,
+#             'platform': self.platform,
+#             'sensor': self.sensor,
+#             'resolution': self.resolution,
+#             'format': self.format
+#         }
+#
+#     @staticmethod
+#     def from_dict(json_dict: dict):
+#         if json_dict.__contains__("id"):
+#             data_source = EODataSource(json_dict["id"])
+#             if json_dict.__contains__("dataType"):
+#                 data_source.data_type = json_dict["dataType"]
+#             if json_dict.__contains__("citation"):
+#                 data_source.citation = json_dict["citation"]
+#             if json_dict.__contains__("platform"):
+#                 data_source.platform = json_dict["platform"]
+#             if json_dict.__contains__("sensor"):
+#                 data_source.sensor = json_dict["sensor"]
+#             if json_dict.__contains__("resolution"):
+#                 data_source.resolution = json_dict["resolution"]
+#             if json_dict.__contains__("format"):
+#                     data_source.resolution = json_dict["format"]
+#             return data_source
+#         else:
+#             raise ValueError("The given json_dict is not a valid EODataSource")
 
 
 @dataclass
-class Labeling:
+class EOTask(Task):
     """
-    Labeling type
+    Extended task type for EO training data
     """
-    id: str
-    labelers: List[Labeler] = field(default_factory=list)
-    procedure: LabelingProcedure = field(default=LabelingProcedure(""))
+    task_type: str = field(default=None)
 
     def to_dict(self):
         return {
-            "type": "Labeling",
+            "type": "EOTask",
             "id": self.id,
-            "labelers": [labeler.to_dict() for labeler in self.labelers],
-            "procedure": self.procedure.to_dict()
-        }
-
-    @staticmethod
-    def from_dict(json_dict: dict):
-        if json_dict.__contains__("id") and json_dict["type"] == "Labeling":
-            labeling = Labeling(json_dict["id"])
-            if json_dict.__contains__("labelers"):
-                labeling.labelers = [Labeler.from_dict(labeler) for labeler in json_dict["labelers"]]
-            if json_dict.__contains__("procedure"):
-                labeling.procedure = LabelingProcedure.from_dict(json_dict["procedure"])
-            return labeling
-        else:
-            raise ValueError("The given json_dict is not a valid Labeling")
-
-
-@dataclass
-class TrainingDataQuality:
-    """
-    Basic training data quality type
-    """
-
-    def to_dict(self):
-        return {
-            "type": "TrainingDataQuality"
-        }
-
-    @staticmethod
-    def from_dict(json_dict: dict):
-        if json_dict["type"] == "TrainingDataQuality":
-            return TrainingDataQuality()
-        else:
-            raise ValueError("The given json_dict is not a valid TrainingDataQuality")
-
-
-@dataclass
-class Label:
-    """
-    Basic label type
-    """
-    is_negative: bool = field(default=None)
-
-    def to_dict(self):
-        return {
-            "type": "Label",
-            "isNegative": self.is_negative
+            "datasetId": self.dataset_id,
+            "description": self.description,
+            "taskType": self.task_type
         }
 
     @staticmethod
     def from_dict(json_dict: dict):
-        if json_dict["type"] == "Label":
-            label = Label()
-            if json_dict.__contains__("isNegative"):
-                label.is_negative = json_dict["isNegative"]
-            return label
+        if json_dict.__contains__("id") and json_dict.__contains__("type") and json_dict["type"] == "EOTask":
+            task = EOTask(json_dict["id"])
+            if json_dict.__contains__("datasetId"):
+                task.dataset_id = json_dict["datasetId"]
+            if json_dict.__contains__("description"):
+                task.description = json_dict["description"]
+            if json_dict.__contains__("taskType"):
+                task.task_type = json_dict["taskType"]
+            return task
         else:
-            raise ValueError("The given json_dict is not a valid Label")
+            raise ValueError("The given json_dict is not a valid EOTask")
 
 
 @dataclass
-class TrainingData:
+class EOTrainingData(TrainingData):
     """
-    Basic training data type
+    Extended training data type for EO training data
     """
-    id: str
-    training_type: str = field(default=None)
-    number_of_Labels: int = field(default=None)
-    labels: List[Label] = field(default_factory=list)
-
-    def get_labels(self) -> List[Label]:
-        """
-        Returns the labels of the training data
-        """
-        return self.labels
+    extent: List[float] = field(default_factory=list)
+    date_time: Union[str, List[str]] = field(default=None)
+    data_url: Union[str, List[str]] = field(default=None)
 
     def to_dict(self):
         return {
-            "type": "TrainingData",
+            "type": "EOTrainingData",
             "id": self.id,
             "trainingType": self.training_type,
-            "numberOfLabels": self.number_of_Labels,
+            "numberOfLabels": self.number_of_labels,
+            "dataSources": self.data_sources,
+            'extent': self.extent,
+            'dateTime': self.date_time,
+            'dataURL': self.data_url,
+            "quality": self.quality.to_dict() if self.quality is not None else None,
+            "labeling": [ll.to_dict() for ll in self.labeling],
             "labels": [label.to_dict() for label in self.labels]
         }
 
     @staticmethod
     def from_dict(json_dict: dict):
-        if json_dict.__contains__("id") and json_dict["type"] == "TrainingData":
-            training_data = TrainingData(json_dict["id"])
+        if json_dict.__contains__("id") and json_dict["type"] == "EOTrainingData":
+            training_data = EOTrainingData(json_dict["id"])
             if json_dict.__contains__("trainingType"):
                 training_data.training_type = json_dict["trainingType"]
             if json_dict.__contains__("numberOfLabels"):
-                training_data.number_of_Labels = json_dict["numberOfLabels"]
+                training_data.number_of_labels = json_dict["numberOfLabels"]
+            if json_dict.__contains__("dataSources"):
+                training_data.data_sources = json_dict["dataSources"]
+            if json_dict.__contains__("quality"):
+                training_data.quality = DataQuality.from_dict(json_dict["quality"])
+            if json_dict.__contains__("labeling"):
+                training_data.labeling = [Labeling.from_dict(ll) for ll in json_dict["labeling"]]
             if json_dict.__contains__("labels"):
-                training_data.labels = [Label.from_dict(label) for label in json_dict["labels"]]
+                # Different type of labels
+                if json_dict["labels"][0]["type"] == "SceneLabel":
+                    training_data.labels = [SceneLabel.from_dict(label) for label in json_dict["labels"]]
+                elif json_dict["labels"][0]["type"] == "ObjectLabel":
+                    training_data.labels = [ObjectLabel.from_dict(label) for label in json_dict["labels"]]
+                elif json_dict["labels"][0]["type"] == "PixelLabel":
+                    training_data.labels = [PixelLabel.from_dict(label) for label in json_dict["labels"]]
+            if json_dict.__contains__("extent"):
+                training_data.extent = json_dict["extent"]
+            if json_dict.__contains__("dateTime"):
+                training_data.date_time = json_dict["dateTime"]
+            if json_dict.__contains__("dataURL"):
+                training_data.data_url = json_dict["dataURL"]
             return training_data
         else:
-            raise ValueError("The given json_dict is not a valid TrainingData")
+            raise ValueError("The given json_dict is not a valid EOTrainingData")
 
 
 @dataclass
-class TrainingDataset:
+class EOTrainingDataset(TrainingDataset):
     """
-    Basic training dataset type
+    Extended training dataset type for EO training dataset
     """
-    id: str
-    name: str
-    description: str
-    version: str = field(default=None)
-    amount_of_training_data: int = field(default=None)
-    created_time: str = field(default=None)
-    updated_time: str = field(default=None)
-    license: str = field(default=None)
-    providers: List[str] = field(default=None)
-    keywords: List[str] = field(default=None)
-    metrics_in_literature: List[MetricsInLiterature] = field(default_factory=list)
-    statistics_info: List[KeyValuePair] = field(default_factory=list)
-    number_of_classes: int = field(default=None)
-    classification_schema: str = field(default=None)
-    classes: Union[List[KeyValuePair], List[str]] = field(default=None)
-    tasks: List[Task] = field(default_factory=list)
-    labelings: List[Labeling] = field(default_factory=list)
-    quality: TrainingDataQuality = field(default=TrainingDataQuality())
-    data: List[TrainingData] = field(default_factory=list)
-
-    def get_training_data(self) -> List[TrainingData]:
-        """
-        Return the training data of the training dataset
-        """
-        return self.data
-
-    def get_training_data_by_id(self, _id: str) -> TrainingData:
-        """
-        Get training data of the training dataset by id
-        """
-        for data in self.data:
-            if data.id == _id:
-                return data
-
-    def get_labelings(self) -> List[Labeling]:
-        """
-        Return the labelings of the training dataset
-        """
-        return self.labelings
-
-    def get_tasks(self) -> List[Task]:
-        """
-        Return the tasks of the training dataset
-        """
-        return self.tasks
-
-    def get_quality(self) -> TrainingDataQuality:
-        """
-        Return the quality of the training dataset
-        """
-        return self.quality
+    extent: List[float] = field(default_factory=list)
+    bands: List[str] = field(default_factory=list)
+    image_size: str = field(default=None)
 
     def to_dict(self):
         return {
-            "type": "TrainingDataset",
+            "type": "EOTrainingDataset",
             "id": self.id,
             "name": self.name,
             "description": self.description,
+            "license": self.license,
+            "doi": self.doi,
+            "scope": self.scope.to_dict() if self.scope is not None else None,
             "version": self.version,
             "amountOfTrainingData": self.amount_of_training_data,
             "createdTime": self.created_time,
             "updatedTime": self.updated_time,
-            "license": self.license,
             "providers": self.providers,
             "keywords": self.keywords,
             "metricsInLIT": [m.to_dict() for m in self.metrics_in_literature],
             "statisticsInfo": [s.to_dict() for s in self.statistics_info],
             "numberOfClasses": self.number_of_classes,
             "classificationSchema": self.classification_schema,
             "classes": self.classes,
             "tasks": [t.to_dict() for t in self.tasks],
-            "labelings": [labeling.to_dict() for labeling in self.labelings],
-            "quality": self.quality.to_dict(),
+            'extent': self.extent,
+            'bands': self.bands,
+            'imageSize': self.image_size,
+            "labeling": [labeling.to_dict() for labeling in self.labeling],
+            "quality": self.quality.to_dict() if self.quality is not None else None,
+            "changesets": [changeset.to_dict() for changeset in self.changesets],
             "data": [d.to_dict() for d in self.data]
         }
 
     @staticmethod
     def from_dict(json_dict: dict):
         if json_dict.__contains__("id") and json_dict.__contains__("name") \
-                and json_dict.__contains__("description") and json_dict["type"] == "TrainingDataset":
-            td = TrainingDataset(json_dict["id"], json_dict["name"], json_dict["description"])
+                and json_dict.__contains__("description") and json_dict.__contains__("license") \
+                and json_dict["type"] == "EOTrainingDataset":
+            td = EOTrainingDataset(json_dict["id"], json_dict["name"], json_dict["description"], json_dict["license"])
+            if json_dict.__contains__("doi"):
+                td.doi = json_dict["doi"]
+            if json_dict.__contains__("scope"):
+                td.scope = Scope.from_dict(json_dict["scope"])
             if json_dict.__contains__("version"):
                 td.version = json_dict["version"]
             if json_dict.__contains__("amountOfTrainingData"):
                 td.amount_of_training_data = json_dict["amountOfTrainingData"]
             if json_dict.__contains__("createdTime"):
                 td.created_time = json_dict["createdTime"]
             if json_dict.__contains__("updatedTime"):
                 td.updated_time = json_dict["updatedTime"]
-            if json_dict.__contains__("license"):
-                td.license = json_dict["license"]
             if json_dict.__contains__("providers"):
                 td.providers = json_dict["providers"]
             if json_dict.__contains__("keywords"):
                 td.keywords = json_dict["keywords"]
             if json_dict.__contains__("metricsInLIT"):
                 td.metrics_in_literature = [MetricsInLiterature.from_dict(m) for m in
                                             json_dict["metricsInLIT"]]
@@ -382,17 +343,25 @@
             if json_dict.__contains__("numberOfClasses"):
                 td.number_of_classes = json_dict["numberOfClasses"]
             if json_dict.__contains__("classificationSchema"):
                 td.classification_schema = json_dict["classificationSchema"]
             if json_dict.__contains__("classes"):
                 td.classes = json_dict["classes"]
             if json_dict.__contains__("tasks"):
-                td.tasks = [Task.from_dict(t) for t in json_dict["tasks"]]
-            if json_dict.__contains__("labelings"):
-                td.labelings = [Labeling.from_dict(labeling) for labeling in json_dict["labelings"]]
+                td.tasks = [EOTask.from_dict(t) for t in json_dict["tasks"]]
+            if json_dict.__contains__("labeling"):
+                td.labeling = [Labeling.from_dict(labeling) for labeling in json_dict["labeling"]]
             if json_dict.__contains__("quality"):
-                td.quality = TrainingDataQuality.from_dict(json_dict["quality"])
+                td.quality = DataQuality.from_dict(json_dict["quality"])
+            if json_dict.__contains__("changesets"):
+                td.changesets = [Changeset.from_dict(changeset) for changeset in json_dict["changesets"]]
             if json_dict.__contains__("data"):
-                td.data = [TrainingData.from_dict(data) for data in json_dict["data"]]
+                td.data = [EOTrainingData.from_dict(data) for data in json_dict["data"]]
+            if json_dict.__contains__("extent"):
+                td.extent = json_dict["extent"]
+            if json_dict.__contains__("bands"):
+                td.bands = json_dict["bands"]
+            if json_dict.__contains__("imageSize"):
+                td.image_size = json_dict["imageSize"]
             return td
         else:
-            raise ValueError("The given json_dict is not a valid TrainingDataset")
+            raise ValueError("The given json_dict is not a valid EOTrainingDataset")
```

### Comparing `pytdml-1.0.0/pytdml/type/extended_types.py` & `pytdml-1.1.1/pytdml/type/basic_types.py`

 * *Files 26% similar despite different names*

```diff
@@ -27,302 +27,546 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # ------------------------------------------------------------------------------
 from dataclasses import dataclass, field
 from typing import List, Union
 
-import geojson
-from geojson import Point, LineString, Polygon
-from pytdml.type.basic_types import Label, TrainingData, TrainingDataset, TrainingDataQuality, Task, \
-    MetricsInLiterature, \
-    KeyValuePair, Labeling
+
+@dataclass
+class KeyValuePair:
+    """
+    Key/Value pair type
+    """
+    key: str
+    value: Union[str, int, float, bool, None]
+
+    def to_dict(self):
+        return {self.key: self.value}
+
+    @staticmethod
+    def from_dict(json_dict: dict):
+        if len(json_dict.keys()) == 1:
+            for key in json_dict.keys():
+                return KeyValuePair(key, json_dict[key])
+        else:
+            raise ValueError("The given json_dict is not a valid KeyValuePair")
 
 
 @dataclass
-class SceneLabel(Label):
+class MetricsInLiterature:
     """
-    Extended label type for scene level training data
+    Metrics in literature type
     """
-    label_class: str = field(default=None)
+    doi: str
+    algorithm: str = field(default=None)
+    metrics: List[KeyValuePair] = field(default_factory=list[KeyValuePair])
 
     def to_dict(self):
         return {
-            "type": "SceneLabel",
-            "isNegative": self.is_negative,
-            'class': self.label_class
+            "doi": self.doi,
+            "algorithm": self.algorithm,
+            "metrics": [m.to_dict() for m in self.metrics]
         }
 
     @staticmethod
     def from_dict(json_dict: dict):
-        if json_dict.__contains__("class") and json_dict["type"] == "SceneLabel":
-            label = SceneLabel(label_class=json_dict["class"])
-            if json_dict.__contains__("isNegative"):
-                label.is_negative = json_dict["isNegative"]
-            return label
+        if json_dict.__contains__("doi"):
+            metrics_in_literature = MetricsInLiterature(json_dict["doi"])
+            if json_dict.__contains__("algorithm"):
+                metrics_in_literature.algorithm = json_dict["algorithm"]
+            if json_dict.__contains__("metrics"):
+                metrics_in_literature.metrics = [KeyValuePair.from_dict(m) for m in json_dict["metrics"]]
+            return metrics_in_literature
         else:
-            raise ValueError("The given json_dict is not a valid SceneLabel")
+            raise ValueError("The given json_dict is not a valid MetricsInLiterature")
 
 
 @dataclass
-class ObjectLabel(Label):
+class Task:
     """
-    Extended label type for object level training data
+    Basic task type
     """
-    object: Union[Point, LineString, Polygon] = field(default=None)
-    label_class: str = field(default=None)
-    geometry_type: str = field(default=None)
-    is_difficultly_detectable: bool = field(default=None)
+    id: str
+    dataset_id: str = field(default=None)
+    description: str = field(default=None)
 
     def to_dict(self):
         return {
-            "type": "ObjectLabel",
-            "isNegative": self.is_negative,
-            'object': self.object,
-            'geometryType': self.geometry_type,
-            'class': self.label_class,
-            'isDiffDetectable': self.is_difficultly_detectable
+            "type": "Task",
+            "id": self.id,
+            "datasetId": self.dataset_id,
+            "description": self.description
         }
 
     @staticmethod
     def from_dict(json_dict: dict):
-        if json_dict.__contains__("object") and json_dict["type"] == "ObjectLabel":
-            label = ObjectLabel(object=geojson.loads(json_dict["object"].__str__().replace("'", "\"")))
-            if json_dict.__contains__("isNegative"):
-                label.is_negative = json_dict["isNegative"]
-            if json_dict.__contains__("geometryType"):
-                label.geometry_type = json_dict["geometryType"]
-            if json_dict.__contains__("class"):
-                label.label_class = json_dict["class"]
-            if json_dict.__contains__("isDiffDetectable"):
-                label.is_difficultly_detectable = json_dict["isDiffDetectable"]
-            return label
+        if json_dict.__contains__("id") and json_dict["type"] == "Task":
+            task = Task(json_dict["id"])
+            if json_dict.__contains__("datasetId"):
+                task.dataset_id = json_dict["datasetId"]
+            if json_dict.__contains__("description"):
+                task.description = json_dict["description"]
+            return task
         else:
-            raise ValueError("The given json_dict is not a valid ObjectLabel")
+            raise ValueError("The given json_dict is not a valid Task")
 
 
 @dataclass
-class PixelLabel(Label):
+class Labeler:
     """
-    Extended label type for pixel level training data
+    Labeler type
     """
-    image_url: Union[str, List[str]] = field(default=None)
+    id: str
+    name: str = field(default=None)
 
     def to_dict(self):
         return {
-            "type": "PixelLabel",
-            "isNegative": self.is_negative,
-            'imageUrl': self.image_url
+            "type": "Labeler",
+            "id": self.id,
+            "name": self.name
         }
 
     @staticmethod
     def from_dict(json_dict: dict):
-        if json_dict.__contains__("imageUrl") and json_dict["type"] == "PixelLabel":
-            label = PixelLabel(image_url=json_dict["imageUrl"])
-            if json_dict.__contains__("isNegative"):
-                label.is_negative = json_dict["isNegative"]
-            return label
+        if json_dict.__contains__("id") and json_dict["type"] == "Labeler":
+            labeler = Labeler(json_dict["id"])
+            if json_dict.__contains__("name"):
+                labeler.name = json_dict["name"]
+            return labeler
         else:
-            raise ValueError("The given json_dict is not a valid PixelLabel")
+            raise ValueError("The given json_dict is not a valid Labeler")
 
 
 @dataclass
-class EODataSource:
+class LabelingProcedure:
     """
-    EO data source type
+    Labeling procedure type
     """
     id: str
-    data_type: str = field(default=None)
-    citation: str = field(default=None)
-    platform: str = field(default=None)
-    sensor: str = field(default=None)
-    resolution: str = field(default=None)
+    methods: list[str] = field(default_factory=list)
+    tools: list[str] = field(default_factory=list)
 
     def to_dict(self):
         return {
-            'id': self.id,
-            'dataType': self.data_type,
-            'citation': self.citation,
-            'platform': self.platform,
-            'sensor': self.sensor,
-            'resolution': self.resolution
+            "type": "LabelingProcedure",
+            "id": self.id,
+            "methods": self.methods,
+            "tools": self.tools
         }
 
     @staticmethod
     def from_dict(json_dict: dict):
-        if json_dict.__contains__("id"):
-            data_source = EODataSource(json_dict["id"])
-            if json_dict.__contains__("dataType"):
-                data_source.data_type = json_dict["dataType"]
-            if json_dict.__contains__("citation"):
-                data_source.citation = json_dict["citation"]
-            if json_dict.__contains__("platform"):
-                data_source.platform = json_dict["platform"]
-            if json_dict.__contains__("sensor"):
-                data_source.sensor = json_dict["sensor"]
-            if json_dict.__contains__("resolution"):
-                data_source.resolution = json_dict["resolution"]
-            return data_source
+        if json_dict.__contains__("id") and json_dict["type"] == "LabelingProcedure":
+            labeling_procedure = LabelingProcedure(json_dict["id"])
+            if json_dict.__contains__("methods"):
+                labeling_procedure.method = json_dict["methods"]
+            if json_dict.__contains__("tools"):
+                labeling_procedure.tool = json_dict["tools"]
+            return labeling_procedure
         else:
-            raise ValueError("The given json_dict is not a valid EODataSource")
+            raise ValueError("The given json_dict is not a valid LabelingProcedure")
 
 
 @dataclass
-class EOTask(Task):
+class Labeling:
     """
-    Extended task type for EO training data
+    Labeling type
     """
-    task_type: str = field(default=None)
+    id: str
+    scope: object
+    labelers: List[Labeler] = field(default_factory=list)
+    procedure: LabelingProcedure = field(default=None)
 
     def to_dict(self):
         return {
-            "type": "EOTask",
-            "description": self.description,
-            "taskType": self.task_type
+            "type": "Labeling",
+            "id": self.id,
+            "scope": self.scope,
+            "labelers": [labeler.to_dict() for labeler in self.labelers],
+            "procedure": self.procedure.to_dict() if self.procedure is not None else None,
         }
 
     @staticmethod
     def from_dict(json_dict: dict):
-        if json_dict.__contains__("type") and json_dict["type"] == "EOTask":
-            task = EOTask()
-            if json_dict.__contains__("description"):
-                task.description = json_dict["description"]
-            if json_dict.__contains__("taskType"):
-                task.task_type = json_dict["taskType"]
-            return task
+        if json_dict.__contains__("id") and json_dict.__contains__("scope") and json_dict["type"] == "Labeling":
+            labeling = Labeling(json_dict["id"], json_dict["scope"])
+            if json_dict.__contains__("labelers"):
+                labeling.labelers = [Labeler.from_dict(labeler) for labeler in json_dict["labelers"]]
+            if json_dict.__contains__("procedure"):
+                labeling.procedure = LabelingProcedure.from_dict(json_dict["procedure"])
+            return labeling
         else:
-            raise ValueError("Invalid EOTask dict")
+            raise ValueError("The given json_dict is not a valid Labeling")
+
+
+@dataclass
+class ScopeDescription:
+    """
+    From ISO 19115-1 MD_ScopeDescription
+    """
+    attributes: list[str] = field(default_factory=list)
+    features: list[str] = field(default_factory=list)
+    featureInstances: list[str] = field(default_factory=list)
+    attributeInstances: list[str] = field(default_factory=list)
+    dataset: str = field(default=None)
+    other: str = field(default=None)
+
+    def to_dict(self):
+        return {
+            "attributes": self.attributes,
+            "features": self.features,
+            "featureInstances": self.featureInstances,
+            "attributeInstances": self.attributeInstances,
+            "dataset": self.dataset,
+            "other": self.other
+        }
+
+    @staticmethod
+    def from_dict(json_dict: dict):
+        sd = ScopeDescription()
+        if json_dict.__contains__("attributes"):
+            sd.attributes = json_dict["attributes"]
+        if json_dict.__contains__("features"):
+            sd.features = json_dict["features"]
+        if json_dict.__contains__("featureInstances"):
+            sd.featureInstances = json_dict["featureInstances"]
+        if json_dict.__contains__("attributeInstances"):
+            sd.attributeInstances = json_dict["attributeInstances"]
+        if json_dict.__contains__("dataset"):
+            sd.dataset = json_dict["dataset"]
+        if json_dict.__contains__("other"):
+            sd.other = json_dict["other"]
+        return sd
 
 
 @dataclass
-class EOTrainingDataQuality(TrainingDataQuality):
+class Scope:
     """
-    Extended quality type for EO training data
+    From ISO 19115-1 MD_Scope
     """
+    level: str
+    levelDescription: List[ScopeDescription] = field(default_factory=list[ScopeDescription])
 
     def to_dict(self):
         return {
-            "type": "EOTrainingDataQuality",
+            "level": self.level,
+            "levelDescription": [ld.to_dict for ld in self.levelDescription]
         }
 
     @staticmethod
     def from_dict(json_dict: dict):
-        if json_dict["type"] == "EOTrainingDataQuality":
-            tdq = EOTrainingDataQuality()
-            return tdq
+        if json_dict.__contains__("level"):
+            scope = Scope(json_dict["level"])
+            if json_dict.__contains__("levelDescription"):
+                scope.levelDescription = [ScopeDescription.from_dict(ld) for ld in json_dict["levelDescription"]]
+            return scope
         else:
-            raise ValueError("Invalid EOTrainingDataQuality dict")
+            raise ValueError("The given json_dict is not a valid Scope")
 
 
 @dataclass
-class EOTrainingData(TrainingData):
+class QualityElement:
     """
-    Extended training data type for EO training data
+    From ISO 19157-1 QualityElement
     """
-    extent: List[float] = field(default=None)
-    date_time: Union[str, List[str]] = field(default=None)
-    data_url: Union[str, List[str]] = field(default=None)
+    type: str = field(default=None)
+    measure: str = field(default=None)
+    evaluation_method: str = field(default=None)
+    result: str = field(default=None)
 
     def to_dict(self):
         return {
-            "type": "EOTrainingData",
+            "type": self.type,
+            "measure": self.measure,
+            "evaluationMethod": self.evaluation_method,
+            "result": self.result
+        }
+
+    @staticmethod
+    def from_dict(json_dict: dict):
+        quality_element = QualityElement()
+        if json_dict.__contains__("type"):
+            quality_element.type = json_dict["type"]
+        if json_dict.__contains__("measure"):
+            quality_element.measure = json_dict["measure"]
+        if json_dict.__contains__("evaluationMethod"):
+            quality_element.evaluation_method = json_dict["evaluationMethod"]
+        if json_dict.__contains__("result"):
+            quality_element.result = json_dict["resule"]
+        return quality_element
+
+
+@dataclass
+class DataQuality:
+    """
+    From ISO 19157-1 DataQuality
+    """
+    scope: Scope
+    report: List[QualityElement] = field(default_factory=list[QualityElement])
+
+    def to_dict(self):
+        return {
+            "scope": self.scope.to_dict() if self.scope is not None else None,
+            "report": [r.to_dict() for r in self.report],
+        }
+
+    @staticmethod
+    def from_dict(json_dict: dict):
+        if json_dict.__contains__("scope"):
+            data_quality = DataQuality(scope=Scope.from_dict(json_dict["scope"]))
+            if json_dict.__contains__("report"):
+                data_quality.report = [QualityElement.from_dict(element) for element in json_dict["report"]]
+            return data_quality
+        else:
+            raise ValueError("The given json_dict is not a valid DataQuality")
+
+
+@dataclass
+class Label:
+    """
+    Basic label type
+    """
+    is_negative: bool = field(default=None)
+    confidence: float = field(default=None)
+
+    def to_dict(self):
+        return {
+            "type": "Label",
+            "isNegative": self.is_negative,
+            "confidence": self.confidence
+        }
+
+    @staticmethod
+    def from_dict(json_dict: dict):
+        if json_dict["type"] == "Label":
+            label = Label()
+            if json_dict.__contains__("isNegative"):
+                label.is_negative = json_dict["isNegative"]
+            if json_dict.__contains__("confidence"):
+                label.confidence = json_dict["confidence"]
+            return label
+        else:
+            raise ValueError("The given json_dict is not a valid Label")
+
+
+@dataclass
+class TrainingData:
+    """
+    Basic training data type
+    """
+    id: str
+    dataset_id: str = field(default=None)
+    training_type: str = field(default=None)
+    number_of_labels: int = field(default=None)
+    data_sources: List[str] = field(default_factory=list)
+    quality: DataQuality = field(default=None)
+    labeling: List[Labeling] = field(default_factory=list[Labeling])
+    labels: List[Label] = field(default_factory=list[Label])
+
+    def get_labels(self) -> List[Label]:
+        """
+        Returns the labels of the training data
+        """
+        return self.labels
+
+    def to_dict(self):
+        return {
+            "type": "TrainingData",
             "id": self.id,
             "trainingType": self.training_type,
-            "numberOfLabels": self.number_of_Labels,
-            "labels": [label.to_dict() for label in self.labels],
-            'extent': self.extent,
-            'dateTime': self.date_time,
-            'dataUrl': self.data_url
+            "numberOfLabels": self.number_of_labels,
+            "dataSources": self.data_sources,
+            "quality": self.quality.to_dict() if self.quality is not None else None,
+            "labeling": [ll.to_dict() for ll in self.labeling],
+            "labels": [label.to_dict() for label in self.labels]
         }
 
     @staticmethod
     def from_dict(json_dict: dict):
-        if json_dict.__contains__("id") and json_dict["type"] == "EOTrainingData":
-            training_data = EOTrainingData(json_dict["id"])
+        if json_dict.__contains__("id") and json_dict["type"] == "TrainingData":
+            training_data = TrainingData(json_dict["id"])
             if json_dict.__contains__("trainingType"):
                 training_data.training_type = json_dict["trainingType"]
             if json_dict.__contains__("numberOfLabels"):
-                training_data.number_of_Labels = json_dict["numberOfLabels"]
+                training_data.number_of_labels = json_dict["numberOfLabels"]
+            if json_dict.__contains__("dataSources"):
+                training_data.data_sources = json_dict["dataSources"]
+            if json_dict.__contains__("quality"):
+                training_data.quality = DataQuality.from_dict(json_dict["quality"])
+            if json_dict.__contains__("labeling"):
+                training_data.labeling = [Labeling.from_dict(ll) for ll in json_dict["labeling"]]
             if json_dict.__contains__("labels"):
-                # Different type of labels
-                if json_dict["labels"][0]["type"] == "SceneLabel":
-                    training_data.labels = [SceneLabel.from_dict(label) for label in json_dict["labels"]]
-                elif json_dict["labels"][0]["type"] == "ObjectLabel":
-                    training_data.labels = [ObjectLabel.from_dict(label) for label in json_dict["labels"]]
-                elif json_dict["labels"][0]["type"] == "PixelLabel":
-                    training_data.labels = [PixelLabel.from_dict(label) for label in json_dict["labels"]]
-            if json_dict.__contains__("extent"):
-                training_data.extent = json_dict["extent"]
-            if json_dict.__contains__("dateTime"):
-                training_data.date_time = json_dict["dateTime"]
-            if json_dict.__contains__("dataUrl"):
-                training_data.data_url = json_dict["dataUrl"]
+                training_data.labels = [Label.from_dict(label) for label in json_dict["labels"]]
             return training_data
         else:
-            raise ValueError("The given json_dict is not a valid EOTrainingData")
+            raise ValueError("The given json_dict is not a valid TrainingData")
 
 
 @dataclass
-class EOTrainingDataset(TrainingDataset):
+class Changeset:
     """
-    Extended training dataset type for EO training dataset
+    Training Data Changeset
     """
-    quality: TrainingDataQuality = field(default=EOTrainingDataQuality())
-    extent: List[float] = field(default=None)
-    data_sources: List[EODataSource] = field(default=None)
-    bands: List[str] = field(default=None)
-    image_size: str = field(default=None)
+    id: str
+    change_count: int
+    dataset_id: str = field(default=None)
+    version: str = field(default=None)
+    created_time: str = field(default=None)
+    add: List[TrainingData] = field(default_factory=list[TrainingData])
+    modify: List[TrainingData] = field(default_factory=list[TrainingData])
+    delete: List[TrainingData] = field(default_factory=list[TrainingData])
 
     def to_dict(self):
         return {
-            "type": "EOTrainingDataset",
+            "type": "TDChangeset",
+            "id": self.id,
+            "changeCount": self.change_count,
+            "datasetId": self.dataset_id,
+            "version": self.version,
+            "createdTime": self.created_time,
+            "add": [td.to_dict() for td in self.add],
+            "modify": [td.to_dict() for td in self.modify],
+            "delete": [td.to_dict() for td in self.delete],
+        }
+
+    @staticmethod
+    def from_dict(json_dict: dict):
+        if json_dict.__contains__("id") and json_dict.__contains__("changeCount") \
+                and json_dict["type"] == "TDChangeset":
+            changeset = Changeset(json_dict["id"], json_dict["changeCount"])
+            if json_dict.__contains__("datasetId"):
+                changeset.dataset_id = json_dict["datasetId"]
+            if json_dict.__contains__("version"):
+                changeset.version = json_dict["version"]
+            if json_dict.__contains__("createdTime"):
+                changeset.created_time = json_dict["createdTime"]
+            if json_dict.__contains__("add"):
+                changeset.add = [TrainingData.from_dict(td) for td in json_dict["add"]]
+            if json_dict.__contains__("modify"):
+                changeset.add = [TrainingData.from_dict(td) for td in json_dict["modify"]]
+            if json_dict.__contains__("delete"):
+                changeset.add = [TrainingData.from_dict(td) for td in json_dict["delete"]]
+            return changeset
+        else:
+            raise ValueError("The given json_dict is not a valid Changeset")
+
+
+@dataclass
+class TrainingDataset:
+    """
+    Basic training dataset type
+    """
+    id: str
+    name: str
+    description: str
+    license: str
+    doi: str = field(default=None)
+    scope: Scope = field(default=None)
+    version: str = field(default=None)
+    amount_of_training_data: int = field(default=None)
+    created_time: str = field(default=None)
+    updated_time: str = field(default=None)
+    providers: List[str] = field(default_factory=list)
+    keywords: List[str] = field(default_factory=list)
+    metrics_in_literature: List[MetricsInLiterature] = field(default_factory=list[MetricsInLiterature])
+    statistics_info: List[KeyValuePair] = field(default_factory=list[KeyValuePair])
+    dataSources: List[str] = field(default_factory=list)
+    number_of_classes: int = field(default=None)
+    classification_schema: str = field(default=None)
+    classes: Union[List[KeyValuePair], List[str]] = field(default=None)
+    tasks: List[Task] = field(default_factory=list[Task])
+    labeling: List[Labeling] = field(default_factory=list[Labeling])
+    quality: DataQuality = field(default=None)
+    changesets: List[Changeset] = field(default_factory=list[Changeset])
+    data: List[TrainingData] = field(default_factory=list[TrainingData])
+
+    def get_training_data(self) -> List[TrainingData]:
+        """
+        Return the training data of the training dataset
+        """
+        return self.data
+
+    def get_training_data_by_id(self, _id: str) -> TrainingData:
+        """
+        Get training data of the training dataset by id
+        """
+        for data in self.data:
+            if data.id == _id:
+                return data
+
+    def get_labelings(self) -> List[Labeling]:
+        """
+        Return the labeling of the training dataset
+        """
+        return self.labeling
+
+    def get_tasks(self) -> List[Task]:
+        """
+        Return the tasks of the training dataset
+        """
+        return self.tasks
+
+    def get_quality(self) -> DataQuality:
+        """
+        Return the quality of the training dataset
+        """
+        return self.quality
+
+    def get_changesets(self) -> List[Changeset]:
+        """
+        Return the changesets of the training dataset
+        """
+        return self.changesets
+
+    def to_dict(self):
+        return {
+            "type": "TrainingDataset",
             "id": self.id,
             "name": self.name,
             "description": self.description,
+            "license": self.license,
+            "doi": self.doi,
+            "scope": self.scope.to_dict() if self.scope is not None else None,
             "version": self.version,
             "amountOfTrainingData": self.amount_of_training_data,
             "createdTime": self.created_time,
             "updatedTime": self.updated_time,
-            "license": self.license,
             "providers": self.providers,
             "keywords": self.keywords,
             "metricsInLIT": [m.to_dict() for m in self.metrics_in_literature],
             "statisticsInfo": [s.to_dict() for s in self.statistics_info],
             "numberOfClasses": self.number_of_classes,
             "classificationSchema": self.classification_schema,
             "classes": self.classes,
-            'extent': self.extent,
-            'dataSources': [ds.to_dict() for ds in self.data_sources],
-            'bands': self.bands,
-            'imageSize': self.image_size,
             "tasks": [t.to_dict() for t in self.tasks],
-            "labelings": [labeling.to_dict() for labeling in self.labelings],
-            "quality": self.quality.to_dict(),
+            "labeling": [ll.to_dict() for ll in self.labeling],
+            "quality": self.quality.to_dict() if self.quality is not None else None,
+            "changesets": [changeset.to_dict() for changeset in self.changesets],
             "data": [d.to_dict() for d in self.data]
         }
 
     @staticmethod
     def from_dict(json_dict: dict):
         if json_dict.__contains__("id") and json_dict.__contains__("name") \
-                and json_dict.__contains__("description") and json_dict["type"] == "EOTrainingDataset":
-            td = EOTrainingDataset(json_dict["id"], json_dict["name"], json_dict["description"])
-            if json_dict.__contains__("name"):
-                td.name = json_dict["name"]
-            if json_dict.__contains__("description"):
-                td.description = json_dict["description"]
+                and json_dict.__contains__("description") and json_dict.__contains__("license") \
+                and json_dict["type"] == "TrainingDataset":
+            td = TrainingDataset(json_dict["id"], json_dict["name"], json_dict["description"], json_dict["license"])
+            if json_dict.__contains__("doi"):
+                td.doi = json_dict["doi"]
+            if json_dict.__contains__("scope"):
+                td.scope = Scope.from_dict(json_dict["scope"])
             if json_dict.__contains__("version"):
                 td.version = json_dict["version"]
             if json_dict.__contains__("amountOfTrainingData"):
                 td.amount_of_training_data = json_dict["amountOfTrainingData"]
             if json_dict.__contains__("createdTime"):
                 td.created_time = json_dict["createdTime"]
             if json_dict.__contains__("updatedTime"):
                 td.updated_time = json_dict["updatedTime"]
-            if json_dict.__contains__("license"):
-                td.license = json_dict["license"]
             if json_dict.__contains__("providers"):
                 td.providers = json_dict["providers"]
             if json_dict.__contains__("keywords"):
                 td.keywords = json_dict["keywords"]
             if json_dict.__contains__("metricsInLIT"):
                 td.metrics_in_literature = [MetricsInLiterature.from_dict(m) for m in
                                             json_dict["metricsInLIT"]]
@@ -330,26 +574,20 @@
                 td.statistics_info = [KeyValuePair.from_dict(s) for s in json_dict["statisticsInfo"]]
             if json_dict.__contains__("numberOfClasses"):
                 td.number_of_classes = json_dict["numberOfClasses"]
             if json_dict.__contains__("classificationSchema"):
                 td.classification_schema = json_dict["classificationSchema"]
             if json_dict.__contains__("classes"):
                 td.classes = json_dict["classes"]
-            if json_dict.__contains__("extent"):
-                td.extent = json_dict["extent"]
-            if json_dict.__contains__("dataSources"):
-                td.data_sources = [EODataSource.from_dict(ds) for ds in json_dict["dataSources"]]
-            if json_dict.__contains__("bands"):
-                td.bands = json_dict["bands"]
-            if json_dict.__contains__("imageSize"):
-                td.image_size = json_dict["imageSize"]
             if json_dict.__contains__("tasks"):
-                td.tasks = [EOTask.from_dict(t) for t in json_dict["tasks"]]
-            if json_dict.__contains__("labelings"):
-                td.labelings = [Labeling.from_dict(labeling) for labeling in json_dict["labelings"]]
+                td.tasks = [Task.from_dict(t) for t in json_dict["tasks"]]
+            if json_dict.__contains__("labeling"):
+                td.labeling = [Labeling.from_dict(labeling) for labeling in json_dict["labeling"]]
             if json_dict.__contains__("quality"):
-                td.quality = EOTrainingDataQuality.from_dict(json_dict["quality"])
+                td.quality = DataQuality.from_dict(json_dict["quality"])
+            if json_dict.__contains__("changesets"):
+                td.changesets = [Changeset.from_dict(changeset) for changeset in json_dict["changesets"]]
             if json_dict.__contains__("data"):
-                td.data = [EOTrainingData.from_dict(data) for data in json_dict["data"]]
+                td.data = [TrainingData.from_dict(data) for data in json_dict["data"]]
             return td
         else:
-            raise ValueError("Invalid EOTrainingDataset dict")
+            raise ValueError("The given json_dict is not a valid TrainingDataset")
```

### Comparing `pytdml-1.0.0/pytdml/utils.py` & `pytdml-1.1.1/pytdml/utils.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.0.0/pytdml/yaml_to_tdml.py` & `pytdml-1.1.1/pytdml/yaml_to_tdml.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,80 +25,69 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # ------------------------------------------------------------------------------
 import argparse
+import json
 import os
 import sys
 
 import yaml
 import pandas as pd
-from geojson import Polygon
+from geojson import Polygon, Feature
 
 from pytdml.io import write_to_json
-from pytdml.type import EOTask, EODataSource, EOTrainingDataset, EOTrainingData, SceneLabel, PixelLabel, ObjectLabel
+from pytdml.type import EOTask, EOTrainingDataset, EOTrainingData, SceneLabel, PixelLabel, ObjectLabel, Scope
 
 
 def yaml_to_eo_tdml(yaml_path):
     """
     Transform yaml to tdml
     """
-    try:
-        yaml_file = open(yaml_path, "r", encoding='utf-8')
-        yaml_dict = yaml.load(yaml_file, Loader=yaml.FullLoader)
-        dataset_type = yaml_dict['dataset_type']
-        tasks_list = yaml_dict['tasks']
-        data_sources_list = yaml_dict['data_sources']
-        td_list = load_data(yaml_dict['data'])
-
-        tasks = []
-        for task in tasks_list:
-            eo_task = EOTask(
-                task_type=task.__contains__('task_type') and task['task_type'] or "",
-                description=task.__contains__('description') and task['description'] or ""
-            )
-            tasks.append(eo_task)
-
-        data_sources = []
-        for data_source in data_sources_list:
-            eo_data_source = EODataSource(
-                id=data_source.__contains__('id') and data_source['id'] or "",
-                data_type=data_source.__contains__('data_type') and data_source['data_type'] or "",
-                platform=data_source.__contains__('platform') and data_source['platform'] or "",
-                sensor=data_source.__contains__('sensor') and data_source['sensor'] or "",
-                citation=data_source.__contains__('citation') and data_source['citation'] or "",
-                resolution=data_source.__contains__('resolution') and data_source['resolution'] or "",
-            )
-            data_sources.append(eo_data_source)
+    yaml_file = open(yaml_path, "r", encoding='utf-8')
+    yaml_dict = yaml.load(yaml_file, Loader=yaml.FullLoader)
+    dataset_type = yaml_dict['dataset_type']
+    tasks_list = yaml_dict['tasks']
+    td_list = load_data(yaml_dict['data'])
+
+    tasks = []
+    for task in tasks_list:
+        eo_task = EOTask(
+            id=task.__contains__('id') and task['id'] or "",
+            dataset_id=task.__contains__('dataset_id') and task['dataset_id'] or "",
+            task_type=task.__contains__('task_type') and task['task_type'] or "",
+            description=task.__contains__('description') and task['description'] or ""
+        )
+        tasks.append(eo_task)
 
-        if dataset_type == 'EOTrainingDataset':
-            eo_training_dataset = EOTrainingDataset(
-                id=yaml_dict['id'],
-                name=yaml_dict['name'],
-                description=yaml_dict['description'],
-                tasks=tasks,
-                data=td_list,
-                version=yaml_dict['version'],
-                amount_of_training_data=len(td_list),
-                created_time=yaml_dict['created_time'],
-                updated_time=yaml_dict['updated_time'],
-                providers=yaml_dict["providers"],
-                keywords=yaml_dict["keywords"],
-                data_sources=data_sources,
-                classes=yaml_dict['classes'],
-                number_of_classes=len(yaml_dict['classes']),
-                bands=yaml_dict['bands'],
-                image_size=yaml_dict['image_size']
-            )
-            return eo_training_dataset
-    except KeyError:
-        print("Invalid EOTrainingDataset yaml")
-        return None
+    if dataset_type == 'EOTrainingDataset':
+        eo_training_dataset = EOTrainingDataset(
+            id=yaml_dict['id'],
+            name=yaml_dict['name'],
+            description=yaml_dict['description'],
+            license=yaml_dict['license'],
+            doi=yaml_dict['doi'],
+            scope=Scope.from_dict(yaml_dict['scope']),
+            version=yaml_dict['version'],
+            amount_of_training_data=len(td_list),
+            created_time=yaml_dict['created_time'],
+            updated_time=yaml_dict['updated_time'],
+            providers=yaml_dict["providers"],
+            keywords=yaml_dict["keywords"],
+            classification_schema=yaml_dict['classification_schema'],
+            classes=yaml_dict['classes'],
+            tasks=tasks,
+            extent=yaml_dict['extent'],
+            bands=yaml_dict['bands'],
+            image_size=yaml_dict['image_size'],
+            data=td_list,
+        )
+        return eo_training_dataset
 
 
 def load_data(data_dict):
     """
     Load training dataset
     """
     task_type = data_dict['task_type']
@@ -157,14 +146,16 @@
             sub_dirs = dirs
             break
     try:
         for sub_dir in sub_dirs:
             image_path = os.path.join(root_path, sub_dir)
             for root, dirs, files in os.walk(image_path):
                 for file in files:
+                    root = str(root)
+                    file = str(file)
                     data_url = os.path.join(root, file)
                     if file_format == os.path.splitext(data_url)[-1]:
                         td = EOTrainingData(
                             id=file.split(".")[0],
                             labels=[SceneLabel(label_class=sub_dir)],
                             data_url=data_url,
                         )
@@ -181,15 +172,15 @@
     td_list = []
     image_dir, label_dir = get_image_label_url(image_set, label_set)
     index = 0
     for image_url, label_url in zip(image_dir, label_dir):
         td = EOTrainingData(
             id=str(index),
             labels=[PixelLabel(image_url=label_url)],
-            data_url=image_url
+            data_url=str(image_url)
         )
         index = index + 1
         td_list.append(td)
     return td_list
 
 
 def load_data_change_detection(image_before_set, image_after_set, label_set, data_time):
@@ -241,30 +232,55 @@
 
 def load_data_object_detection(image_set, label_set):
     """
     Load training dataset for object detection
     """
     td_list = []
     label_format = label_set['format']
-    label_column = label_set['column']
-    image_dir, label_dir = get_image_label_url(image_set, label_set)
+    image_format = image_set['format']
 
-    index = 0
     if label_format == '.txt':  # txt format
+        image_dir, label_dir = get_image_label_url(image_set, label_set)
         separate = label_set['separate']
+        label_column = label_set['column']
+        index = 0
         for image_url, label_url in zip(image_dir, label_dir):
             labels = read_txt_label(label_url, label_column, separate)
             td = EOTrainingData(
                 id=str(index),
                 labels=labels,
                 data_url=image_url,
             )
-            td.number_of_Labels = len(td.labels)
+            td.number_of_labels = len(td.labels)
             index = index + 1
             td_list.append(td)
+    elif label_format == 'stac' and image_format == 'stac':  # stac format
+        images_stac_path = image_set['root_path'] + "\\collection.json"
+        labels_stac_path = label_set['root_path'] + "\\collection.json"
+        images_stac_json = json.load(open(images_stac_path, 'r'))
+        labels_stac_json = json.load(open(labels_stac_path, 'r'))
+        num = len(images_stac_json['links'])
+        for i in range(num):
+            image_stac_path = os.path.join(image_set['root_path'], images_stac_json['links'][i]['href'])
+            label_stac_path = os.path.join(label_set['root_path'], labels_stac_json['links'][i]['href'])
+            image_stac_json = json.load(open(image_stac_path, 'r'))
+            label_stac_json = json.load(open(label_stac_path, 'r'))
+            label_json_path = os.path.join(os.path.dirname(label_stac_path),
+                                           label_stac_json['assets']['labels']['href'])
+            labels = read_geojson_label(label_json_path)
+            td = EOTrainingData(
+                id=image_stac_json['id'],
+                extent=image_stac_json['bbox'],
+                date_time=image_stac_json['properties']['datetime'],
+                data_url=os.path.join(os.path.dirname(image_stac_path),
+                                      list(image_stac_json['assets'].values())[0]['href']),
+                labels=labels,
+            )
+            td.number_of_labels = len(td.labels)
+            td_list.append(td)
         return td_list
 
 
 def read_txt_label(csv_path, column_name, separate):
     """
     Read the label file in text format in object detection
     """
@@ -276,23 +292,36 @@
             polygon = Polygon(
                 [(float(row['x1']), float(row['y1'])),
                  (float(row['x2']), float(row['y2'])),
                  (float(row['x3']), float(row['y3'])),
                  (float(row['x4']), float(row['y4']))]
             )
             label = ObjectLabel(
-                object=polygon,
-                geometry_type='Horizontal BBox',
+                object=Feature(geometry=polygon),
+                bbox_type='Horizontal BBox',
                 label_class=row['class'],
                 is_difficultly_detectable=row['isDiffDetectable']
             )
             labels.append(label)
     return labels
 
 
+def read_geojson_label(geojson_path):
+    """
+    Read the label file in geojson format in object detection
+    """
+    fc = json.load(open(geojson_path))
+    labels = []
+    for f in fc['features']:
+        labels.append(ObjectLabel(
+            object=f
+        ))
+    return labels
+
+
 def traverse_folder(file_path, file_format):
     """
     Traverse target folder
     """
     try:
         file_dir = []
         for root, dirs, files in os.walk(file_path):
```

### Comparing `pytdml-1.0.0/pytdml.egg-info/PKG-INFO` & `pytdml-1.1.1/pytdml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pytdml
-Version: 1.0.0
+Version: 1.1.1
 Summary: Parsing and encoding training datasets based on OGC Training Data Markup Language for AI (TrainingDML-AI) standard
 Home-page: https://github.com/TrainingDML/pytdml
 Author: Boyi Shangguan
 Author-email: sgby@whu.edu.cn
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -51,15 +50,15 @@
 
 The training dataset can be encoded to TrainingDML-AI JSON format by YAML configuration file with command line.
 
 ```bash
 pytdml/yaml_to_tdml.py --config=<YAML configuration file path> --output=<Output TrainingDML-AI JSON file path>
 ```
 
-YAML configuration file schema is described in [encoding YAML configuration file schema](https://github.com/TrainingDML/pytdml/blob/main/encoding_config_schema.yaml).
+YAML configuration file schema is described in [encoding YAML configuration file schema](https://github.com/TrainingDML/pytdml/blob/main/encoding_config_schema.yml).
 
 #### Using the API from python
 
 The training dataset can also be encoded to TrainingDML-AI JSON format with Python API.
 
 ```python
 from pytdml.io import write_to_json
@@ -242,8 +241,7 @@
 
 The images of training dataset in TrainingDML-AI JSON format can be cropped with command line for preprocessing.
 
 ```bash
 pytdml/tdml_image_crop.py  --input=<Input original TrainingDML-AU file path> --output_json=<Output result TrainingDML-AI JSON file path>
                           --output_images=<Output dir of result cropped images> --size=<Crop size of images>
 ```
-
```

### Comparing `pytdml-1.0.0/pytdml.egg-info/SOURCES.txt` & `pytdml-1.1.1/pytdml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytdml-1.0.0/setup.py` & `pytdml-1.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     long_description_content_type="text/markdown",
     author='Boyi Shangguan',
     author_email='sgby@whu.edu.cn',
     url='https://github.com/TrainingDML/pytdml',
     license='MIT',
     packages=find_packages(),
     include_package_data=True,
-    install_requires=read('requirements.txt').splitlines(),
+    install_requires=["dataclasses", "geojson"],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Scientific/Engineering :: GIS',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
```

