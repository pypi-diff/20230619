# Comparing `tmp/drillvision-0.0.4.tar.gz` & `tmp/drillvision-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drillvision-0.0.4.tar", last modified: Thu Jun 15 05:41:08 2023, max compression
+gzip compressed data, was "drillvision-0.0.5.tar", last modified: Mon Jun 19 21:36:56 2023, max compression
```

## Comparing `drillvision-0.0.4.tar` & `drillvision-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,22 @@
-drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-06-15 05:41:08.700652 drillvision-0.0.4/
--rw-r--r--   0 amin       (501) staff       (20)      305 2023-05-21 20:38:44.000000 drillvision-0.0.4/MANIFEST.in
--rw-r--r--   0 amin       (501) staff       (20)     8511 2023-06-15 05:41:08.700195 drillvision-0.0.4/PKG-INFO
--rw-r--r--   0 amin       (501) staff       (20)     8080 2023-06-13 00:15:55.000000 drillvision-0.0.4/README.md
-drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-06-15 05:41:08.696889 drillvision-0.0.4/drillvision.egg-info/
--rw-r--r--   0 amin       (501) staff       (20)     8511 2023-06-15 05:41:08.000000 drillvision-0.0.4/drillvision.egg-info/PKG-INFO
--rw-r--r--   0 amin       (501) staff       (20)      747 2023-06-15 05:41:08.000000 drillvision-0.0.4/drillvision.egg-info/SOURCES.txt
--rw-r--r--   0 amin       (501) staff       (20)        1 2023-06-15 05:41:08.000000 drillvision-0.0.4/drillvision.egg-info/dependency_links.txt
--rw-r--r--   0 amin       (501) staff       (20)      248 2023-06-15 05:41:08.000000 drillvision-0.0.4/drillvision.egg-info/requires.txt
--rw-r--r--   0 amin       (501) staff       (20)       21 2023-06-15 05:41:08.000000 drillvision-0.0.4/drillvision.egg-info/top_level.txt
-drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-06-15 05:41:08.693288 drillvision-0.0.4/neural_network_model/
--rw-r--r--   0 amin       (501) staff       (20)        5 2023-06-15 05:40:18.000000 drillvision-0.0.4/neural_network_model/VERSION
--rw-r--r--   0 amin       (501) staff       (20)        0 2023-05-16 02:02:49.000000 drillvision-0.0.4/neural_network_model/__init__.py
--rw-r--r--   0 amin       (501) staff       (20)    25121 2023-06-15 04:38:31.000000 drillvision-0.0.4/neural_network_model/bit_vision.py
--rw-r--r--   0 amin       (501) staff       (20)     5926 2023-06-11 16:44:26.000000 drillvision-0.0.4/neural_network_model/model.py
--rw-r--r--   0 amin       (501) staff       (20)    14882 2023-06-15 04:53:05.000000 drillvision-0.0.4/neural_network_model/process_data.py
--rw-r--r--   0 amin       (501) staff       (20)     2843 2023-05-20 18:27:45.000000 drillvision-0.0.4/neural_network_model/s3.py
--rw-r--r--   0 amin       (501) staff       (20)     1913 2023-05-21 20:09:15.000000 drillvision-0.0.4/pyproject.toml
--rw-r--r--   0 amin       (501) staff       (20)      108 2023-06-12 16:36:38.000000 drillvision-0.0.4/requirements-test.txt
--rw-r--r--   0 amin       (501) staff       (20)      248 2023-05-31 01:33:26.000000 drillvision-0.0.4/requirements.txt
--rw-r--r--   0 amin       (501) staff       (20)       38 2023-06-15 05:41:08.700798 drillvision-0.0.4/setup.cfg
--rw-r--r--   0 amin       (501) staff       (20)     2134 2023-06-15 05:14:07.000000 drillvision-0.0.4/setup.py
-drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-06-15 05:41:08.698942 drillvision-0.0.4/tests/
--rw-r--r--   0 amin       (501) staff       (20)      399 2023-06-15 04:02:43.000000 drillvision-0.0.4/tests/test_bitvision.py
--rw-r--r--   0 amin       (501) staff       (20)     5873 2023-06-15 04:05:57.000000 drillvision-0.0.4/tests/test_preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:36:56.092094 drillvision-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-19 21:35:29.000000 drillvision-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-06-19 21:36:56.092094 drillvision-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-19 21:35:29.000000 drillvision-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:36:56.088094 drillvision-0.0.5/drillvision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-06-19 21:36:55.000000 drillvision-0.0.5/drillvision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-19 21:36:56.000000 drillvision-0.0.5/drillvision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 21:36:56.000000 drillvision-0.0.5/drillvision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-19 21:36:56.000000 drillvision-0.0.5/drillvision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-19 21:36:56.000000 drillvision-0.0.5/drillvision.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:36:56.088094 drillvision-0.0.5/neural_network_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-19 21:35:29.000000 drillvision-0.0.5/neural_network_model/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:35:29.000000 drillvision-0.0.5/neural_network_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25121 2023-06-19 21:35:29.000000 drillvision-0.0.5/neural_network_model/bit_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-19 21:35:29.000000 drillvision-0.0.5/neural_network_model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14883 2023-06-19 21:35:29.000000 drillvision-0.0.5/neural_network_model/process_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-19 21:35:29.000000 drillvision-0.0.5/neural_network_model/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-19 21:35:29.000000 drillvision-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-19 21:35:29.000000 drillvision-0.0.5/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-19 21:35:29.000000 drillvision-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 21:36:56.092094 drillvision-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-19 21:35:29.000000 drillvision-0.0.5/setup.py
```

### Comparing `drillvision-0.0.4/PKG-INFO` & `drillvision-0.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: drillvision
-Version: 0.0.4
-Summary: # Drill Bit Classifier
+Version: 0.0.5
+Summary: DrillBitVision
 Home-page: https://github.com/Atashnezhad/DrillBitVision
 Author: Amin Atashnezhad
 Author-email: atashnezhad2@gmail.com
 License: BSD-3
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6.0
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 
 # Drill Bit Classifier
-[![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-360/)
-[![PyPI version](https://badge.fury.io/py/drillvision.svg)](https://badge.fury.io/py/drillvision)
-[![Github All Releases](https://img.shields.io/github/downloads/Atashnezhad/DrillBitVision/total.svg)]()
-[![CircleCI](https://circleci.com/gh/Atashnezhad/DrillBitVision.svg?style=svg)](https://github.com/Atashnezhad/DrillBitVision)
-
 
+[![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-360/)
+[![Downloads](https://static.pepy.tech/personalized-badge/drillvision?period=total&units=international_system&left_color=grey&right_color=red&left_text=Downloads)](https://pepy.tech/project/drillvision)
+![GitHub CI](https://github.com/Atashnezhad/DrillBitVision/actions/workflows/main.yml/badge.svg)
 
 The Drill Bit Classifier is an app that uses a Convolutional Neural Network (CNN) to 
 classify images of drill bits. The app can be used by machinists and engineers to 
 quickly and accurately identify the type of drill bit required for a particular job.
 
 ## Description:
 ### Preprocessing Module
@@ -73,22 +72,14 @@
 ```mermaid
 flowchart LR
 A[Categories\nproperty] --> B[Data Details\nproperty]
 B --> C[Assemble Model] --> D[Compile Model] --> E[Rescale Images\nTrain and Val] 
 --> F[Fit Model] --> G[Save Model]
 ```
 
-
-[//]: # (# CNN Model Prediction on Test Data)
-
-[//]: # (![alt text]&#40;figures/prediction_pdc_bit.png "Logo Title Text 1"&#41;)
-
-[//]: # (![alt text]&#40;figures/prediction_rollercone_bit.png "Logo Title Text 1"&#41;)
-
-
 ## Grad Cam Heatmap - Rollercone Bit
 ![alt text](figures/grad_cam_rc_1.png "Logo Title Text 1")
 
 ## Grad Cam Heatmap - PDC Bit
 ![alt text](figures/grad_cam_pdc_1.png "Logo Title Text 1")
 
 
@@ -145,7 +136,9 @@
         model_path=Path(__file__).parent / "deep_model" / model_name,
         fig_to_save_address=Path(__file__).parent / "figures",
         img_to_be_applied_path=Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit" / list_of_images[0],
         output_gradcam_fig_name="gradcam.png"
     )
 
 
+
+
```

### Comparing `drillvision-0.0.4/README.md` & `drillvision-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # Drill Bit Classifier
-[![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-360/)
-[![PyPI version](https://badge.fury.io/py/drillvision.svg)](https://badge.fury.io/py/drillvision)
-[![Github All Releases](https://img.shields.io/github/downloads/Atashnezhad/DrillBitVision/total.svg)]()
-[![CircleCI](https://circleci.com/gh/Atashnezhad/DrillBitVision.svg?style=svg)](https://github.com/Atashnezhad/DrillBitVision)
-
 
+[![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-360/)
+[![Downloads](https://static.pepy.tech/personalized-badge/drillvision?period=total&units=international_system&left_color=grey&right_color=red&left_text=Downloads)](https://pepy.tech/project/drillvision)
+![GitHub CI](https://github.com/Atashnezhad/DrillBitVision/actions/workflows/main.yml/badge.svg)
 
 The Drill Bit Classifier is an app that uses a Convolutional Neural Network (CNN) to 
 classify images of drill bits. The app can be used by machinists and engineers to 
 quickly and accurately identify the type of drill bit required for a particular job.
 
 ## Description:
 ### Preprocessing Module
@@ -59,22 +57,14 @@
 ```mermaid
 flowchart LR
 A[Categories\nproperty] --> B[Data Details\nproperty]
 B --> C[Assemble Model] --> D[Compile Model] --> E[Rescale Images\nTrain and Val] 
 --> F[Fit Model] --> G[Save Model]
 ```
 
-
-[//]: # (# CNN Model Prediction on Test Data)
-
-[//]: # (![alt text]&#40;figures/prediction_pdc_bit.png "Logo Title Text 1"&#41;)
-
-[//]: # (![alt text]&#40;figures/prediction_rollercone_bit.png "Logo Title Text 1"&#41;)
-
-
 ## Grad Cam Heatmap - Rollercone Bit
 ![alt text](figures/grad_cam_rc_1.png "Logo Title Text 1")
 
 ## Grad Cam Heatmap - PDC Bit
 ![alt text](figures/grad_cam_pdc_1.png "Logo Title Text 1")
```

### Comparing `drillvision-0.0.4/drillvision.egg-info/PKG-INFO` & `drillvision-0.0.5/drillvision.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: drillvision
-Version: 0.0.4
-Summary: # Drill Bit Classifier
+Version: 0.0.5
+Summary: DrillBitVision
 Home-page: https://github.com/Atashnezhad/DrillBitVision
 Author: Amin Atashnezhad
 Author-email: atashnezhad2@gmail.com
 License: BSD-3
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6.0
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 
 # Drill Bit Classifier
-[![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-360/)
-[![PyPI version](https://badge.fury.io/py/drillvision.svg)](https://badge.fury.io/py/drillvision)
-[![Github All Releases](https://img.shields.io/github/downloads/Atashnezhad/DrillBitVision/total.svg)]()
-[![CircleCI](https://circleci.com/gh/Atashnezhad/DrillBitVision.svg?style=svg)](https://github.com/Atashnezhad/DrillBitVision)
-
 
+[![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-360/)
+[![Downloads](https://static.pepy.tech/personalized-badge/drillvision?period=total&units=international_system&left_color=grey&right_color=red&left_text=Downloads)](https://pepy.tech/project/drillvision)
+![GitHub CI](https://github.com/Atashnezhad/DrillBitVision/actions/workflows/main.yml/badge.svg)
 
 The Drill Bit Classifier is an app that uses a Convolutional Neural Network (CNN) to 
 classify images of drill bits. The app can be used by machinists and engineers to 
 quickly and accurately identify the type of drill bit required for a particular job.
 
 ## Description:
 ### Preprocessing Module
@@ -73,22 +72,14 @@
 ```mermaid
 flowchart LR
 A[Categories\nproperty] --> B[Data Details\nproperty]
 B --> C[Assemble Model] --> D[Compile Model] --> E[Rescale Images\nTrain and Val] 
 --> F[Fit Model] --> G[Save Model]
 ```
 
-
-[//]: # (# CNN Model Prediction on Test Data)
-
-[//]: # (![alt text]&#40;figures/prediction_pdc_bit.png "Logo Title Text 1"&#41;)
-
-[//]: # (![alt text]&#40;figures/prediction_rollercone_bit.png "Logo Title Text 1"&#41;)
-
-
 ## Grad Cam Heatmap - Rollercone Bit
 ![alt text](figures/grad_cam_rc_1.png "Logo Title Text 1")
 
 ## Grad Cam Heatmap - PDC Bit
 ![alt text](figures/grad_cam_pdc_1.png "Logo Title Text 1")
 
 
@@ -145,7 +136,9 @@
         model_path=Path(__file__).parent / "deep_model" / model_name,
         fig_to_save_address=Path(__file__).parent / "figures",
         img_to_be_applied_path=Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit" / list_of_images[0],
         output_gradcam_fig_name="gradcam.png"
     )
 
 
+
+
```

### Comparing `drillvision-0.0.4/drillvision.egg-info/SOURCES.txt` & `drillvision-0.0.5/drillvision.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,10 +18,8 @@
 drillvision.egg-info/requires.txt
 drillvision.egg-info/top_level.txt
 neural_network_model/VERSION
 neural_network_model/__init__.py
 neural_network_model/bit_vision.py
 neural_network_model/model.py
 neural_network_model/process_data.py
-neural_network_model/s3.py
-tests/test_bitvision.py
-tests/test_preprocessing.py
+neural_network_model/s3.py
```

### Comparing `drillvision-0.0.4/neural_network_model/bit_vision.py` & `drillvision-0.0.5/neural_network_model/bit_vision.py`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.4/neural_network_model/model.py` & `drillvision-0.0.5/neural_network_model/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     ZOOM_RANGE: float = 0.5
     HORIZONTAL_FLIP: bool = True
     FILL_MODE: str = "nearest"
 
     BATCH_SIZE: int = 1
 
     # Address to save augmented images
-    AUGMENTED_IMAGES_DIR_ADDRESS: str = (
+    AUGMENTED_IMAGES_DIR_ADDRESS: Path = (
         Path(__file__).parent / ".." / "dataset_augmented"
     )
     AUGMENTED_IMAGES_SAVE_PREFIX: str = "augmented_image"
     AUGMENTED_IMAGES_SAVE_FORMAT: str = "jpeg"
 
     NUMBER_OF_IMAGES_TOBE_GENERATED: int = 200
```

### Comparing `drillvision-0.0.4/neural_network_model/process_data.py` & `drillvision-0.0.5/neural_network_model/process_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
             )
 
         return image_dicts
 
     def augment_data(
         self,
         number_of_images_tobe_gen: int = SETTING.AUGMENTATION_SETTING.NUMBER_OF_IMAGES_TOBE_GENERATED,
-        augment_data_address: str = SETTING.AUGMENTATION_SETTING.AUGMENTED_IMAGES_DIR_ADDRESS,
+        augment_data_address: Path = SETTING.AUGMENTATION_SETTING.AUGMENTED_IMAGES_DIR_ADDRESS,
     ):
         """
         This function augments the images and save them into the dataset_augmented folder.
         :param number_of_images_tobe_gen: number of images to be generated
         :param augment_data_address: address to save the augmented images
         :return: None
         """
```

### Comparing `drillvision-0.0.4/neural_network_model/s3.py` & `drillvision-0.0.5/neural_network_model/s3.py`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.4/pyproject.toml` & `drillvision-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.4/setup.py` & `drillvision-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 # Package meta-data.
 NAME = "drillvision"
-DESCRIPTION = long_description
+DESCRIPTION = "DrillBitVision"
 URL = "https://github.com/Atashnezhad/DrillBitVision"
 EMAIL = "atashnezhad2@gmail.com"
 AUTHOR = "Amin Atashnezhad"
-REQUIRES_PYTHON = ">=3.6.0"
+REQUIRES_PYTHON = ">=3.9.0"
 
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
 # Except, perhaps the License and Trove Classifiers!
 # If you do change the License, remember to change the
 # Trove Classifier for that!
```

