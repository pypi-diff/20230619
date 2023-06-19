# Comparing `tmp/pbaa-1.0.2.tar.gz` & `tmp/pbaa-1.0.3.tar.gz`

## Comparing `pbaa-1.0.2.tar` & `pbaa-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rwxr-xr-x   0        0        0      434 2020-02-02 00:00:00.000000 pbaa-1.0.2/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0     1077 2020-02-02 00:00:00.000000 pbaa-1.0.2/.github/workflows/test.yml
--rwxr-xr-x   0        0        0  5701095 2020-02-02 00:00:00.000000 pbaa-1.0.2/assets/demo9.jpg
--rwxr-xr-x   0        0        0   720440 2020-02-02 00:00:00.000000 pbaa-1.0.2/assets/demo9.json
--rwxr-xr-x   0        0        0  1287943 2020-02-02 00:00:00.000000 pbaa-1.0.2/assets/demo9_det.jpg
--rwxr-xr-x   0        0        0  1239235 2020-02-02 00:00:00.000000 pbaa-1.0.2/assets/demo9_seg.jpg
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 pbaa-1.0.2/src/pbaa/__about__.py
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 pbaa-1.0.2/src/pbaa/__init__.py
--rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 pbaa-1.0.2/src/pbaa/__main__.py
--rwxr-xr-x   0        0        0     1111 2020-02-02 00:00:00.000000 pbaa-1.0.2/src/pbaa/cli/__init__.py
--rwxr-xr-x   0        0        0      248 2020-02-02 00:00:00.000000 pbaa-1.0.2/src/pbaa/core/__init__.py
--rwxr-xr-x   0        0        0     6782 2020-02-02 00:00:00.000000 pbaa-1.0.2/src/pbaa/core/check.py
--rwxr-xr-x   0        0        0     5059 2020-02-02 00:00:00.000000 pbaa-1.0.2/src/pbaa/core/grounded_sam.py
--rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 pbaa-1.0.2/src/pbaa/core/prerequisite.py
--rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 pbaa-1.0.2/src/pbaa/core/utils.py
--rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 pbaa-1.0.2/tests/__init__.py
--rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 pbaa-1.0.2/tests/test_dependencies.py
--rwxr-xr-x   0        0        0     3092 2020-02-02 00:00:00.000000 pbaa-1.0.2/.gitignore
--rwxr-xr-x   0        0        0    10280 2020-02-02 00:00:00.000000 pbaa-1.0.2/LICENSE.txt
--rwxr-xr-x   0        0        0     3361 2020-02-02 00:00:00.000000 pbaa-1.0.2/README.md
--rwxr-xr-x   0        0        0     3252 2020-02-02 00:00:00.000000 pbaa-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 pbaa-1.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0      434 2020-02-02 00:00:00.000000 pbaa-1.0.3/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0     1077 2020-02-02 00:00:00.000000 pbaa-1.0.3/.github/workflows/test.yml
+-rwxr-xr-x   0        0        0  5701095 2020-02-02 00:00:00.000000 pbaa-1.0.3/assets/demo9.jpg
+-rwxr-xr-x   0        0        0   720440 2020-02-02 00:00:00.000000 pbaa-1.0.3/assets/demo9.json
+-rwxr-xr-x   0        0        0  1287943 2020-02-02 00:00:00.000000 pbaa-1.0.3/assets/demo9_det.jpg
+-rwxr-xr-x   0        0        0  1239235 2020-02-02 00:00:00.000000 pbaa-1.0.3/assets/demo9_seg.jpg
+-rwxr-xr-x   0        0        0      170 2020-02-02 00:00:00.000000 pbaa-1.0.3/docker/Dockerfile
+-rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 pbaa-1.0.3/src/pbaa/__about__.py
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 pbaa-1.0.3/src/pbaa/__init__.py
+-rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 pbaa-1.0.3/src/pbaa/__main__.py
+-rwxr-xr-x   0        0        0     1160 2020-02-02 00:00:00.000000 pbaa-1.0.3/src/pbaa/cli/__init__.py
+-rwxr-xr-x   0        0        0      248 2020-02-02 00:00:00.000000 pbaa-1.0.3/src/pbaa/core/__init__.py
+-rwxr-xr-x   0        0        0     6782 2020-02-02 00:00:00.000000 pbaa-1.0.3/src/pbaa/core/check.py
+-rwxr-xr-x   0        0        0     5053 2020-02-02 00:00:00.000000 pbaa-1.0.3/src/pbaa/core/grounded_sam.py
+-rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 pbaa-1.0.3/src/pbaa/core/prerequisite.py
+-rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 pbaa-1.0.3/src/pbaa/core/utils.py
+-rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 pbaa-1.0.3/tests/__init__.py
+-rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 pbaa-1.0.3/tests/test_dependencies.py
+-rwxr-xr-x   0        0        0     3092 2020-02-02 00:00:00.000000 pbaa-1.0.3/.gitignore
+-rwxr-xr-x   0        0        0    10280 2020-02-02 00:00:00.000000 pbaa-1.0.3/LICENSE.txt
+-rwxr-xr-x   0        0        0     3812 2020-02-02 00:00:00.000000 pbaa-1.0.3/README.md
+-rwxr-xr-x   0        0        0     3252 2020-02-02 00:00:00.000000 pbaa-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 pbaa-1.0.3/PKG-INFO
```

### Comparing `pbaa-1.0.2/.github/workflows/test.yml` & `pbaa-1.0.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.2/assets/demo9.jpg` & `pbaa-1.0.3/assets/demo9.jpg`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.2/assets/demo9.json` & `pbaa-1.0.3/assets/demo9.json`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.2/assets/demo9_det.jpg` & `pbaa-1.0.3/assets/demo9_det.jpg`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.2/assets/demo9_seg.jpg` & `pbaa-1.0.3/assets/demo9_seg.jpg`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.2/src/pbaa/cli/__init__.py` & `pbaa-1.0.3/src/pbaa/cli/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,8 +19,9 @@
     help="Space-separated a pair of prompt and target classe. (Multi)",
 )
 @click.option("--box_threshold", "-b", type=float, default=0.25, help="Threshold for Object Detection (default: 0.25)")
 @click.option("--nms_threshold", "-n", type=float, default=0.8, help="Threshold for NMS (default: 0.8)")
 @click.option("--output_dir", "-o", type=str, default=".", help="Path to result data (default: '.')")
 def pbaa(src, prompt, box_threshold, nms_threshold, output_dir):
     model_init()
-    inference(src, prompt, box_threshold, nms_threshold, output_dir)
+    _prompt = {i.lower(): v for i, v in prompt}
+    inference(src, _prompt, box_threshold, nms_threshold, output_dir)
```

### Comparing `pbaa-1.0.2/src/pbaa/core/check.py` & `pbaa-1.0.3/src/pbaa/core/check.py`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.2/src/pbaa/core/grounded_sam.py` & `pbaa-1.0.3/src/pbaa/core/grounded_sam.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         result_masks.append(masks[index])
     return np.array(result_masks)
 
 
 def inference(_src, _prompt, box_threshold=0.25, nms_threshold=0.8, output_dir="."):
     src = Path(_src)
     dst = Path(output_dir)
-    _prompt = {i.lower(): v for i, v in _prompt}
+    dst.mkdir(parents=True, exist_ok=True)
 
     # Building GroundingDINO inference model
     grounding_dino_model = Model(
         model_config_path=grounding_dino_config_path, model_checkpoint_path=GROUNDING_DINO_CHECKPOINT_PATH
     )
 
     # Building SAM Model and SAM Predictor
```

### Comparing `pbaa-1.0.2/.gitignore` & `pbaa-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.2/LICENSE.txt` & `pbaa-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.2/README.md` & `pbaa-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,17 +10,30 @@
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [Usage](#Usage)
 - [Demo](#Demo)
 - [License](#license)
+- [Acknowledgements](#acknowledgements)
 
 ## Installation
 
+### Docker (Recommend)
+
+```console
+git clone https://github.com/dh031200/pbaa.git
+docker build docker -t pbaa:latest
+docker run --gpus all -it --ipc=host -v `pwd`:/workspace pbaa:latest
+```
+
+### Without docker
+
+The code requires `python>=3.8`, `CUDA==11.7`.
+
 ```console
 pip install pbaa
 ```
 
 ## Usage
 
 ### Options
@@ -50,40 +63,45 @@
 
 ### Python
 
 ```python
 from pbaa import model_init, inference
 
 model_init()
+# inference(<Source path>, <prompt:class>, box_threshold=0.25, nms_threshold=0.8, output_dir=".")
 inference("path/to/source_image.jpg", {"black dog": "dog", "white cat": "cat"})
 ```
 
 ## Demo
 
 ```console
-## Source : assets/demo9.jpg
-## prompts : {"plant" : "plant", "picture" : "picture", "dog": "dog", "lamp" : "lamp", "carpet" : "carpet", "sofa" : "sofa"}
+# Source : assets/demo9.jpg
+# prompts : {"plant" : "plant", "picture" : "picture", "dog": "dog", "lamp" : "lamp", "carpet" : "carpet", "sofa" : "sofa"}
 
 pbaa -s assets/demo9.jpg -p plant plant -p picture picture -p dog dog -p lamp lamp -p carpet carpet -p sofa sofa
 ```
 
-| Origin                                                                          | Detection                                                                              | Segmentation                                                                           |
-|---------------------------------------------------------------------------------|----------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------|
-| ![Before](https://github.com/dh031200/pbaa/blob/main/assets/demo9.jpg?raw=true) | ![detection](https://github.com/dh031200/pbaa/blob/main/assets/demo9_det.jpg?raw=true) | ![detection](https://github.com/dh031200/pbaa/blob/main/assets/demo9_seg.jpg?raw=true) |
+|                                     Origin                                      |                                       Detection                                        |                                       Segmentation                                        |
+|:-------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
+| ![Before](https://github.com/dh031200/pbaa/blob/main/assets/demo9.jpg?raw=true) | ![detection](https://github.com/dh031200/pbaa/blob/main/assets/demo9_det.jpg?raw=true) | ![segmentation](https://github.com/dh031200/pbaa/blob/main/assets/demo9_seg.jpg?raw=true) |
+
 ### Result data
-[demo9.json](assets/demo9.json)<br>
+
+[demo9.json](https://github.com/dh031200/pbaa/blob/main/assets/demo9.json)<br>
+
 ```console
 json structure
 
 index
   ├ cls : class name
   ├ conf : confidence score
   ├ box : bounding box coordinates
   └ poly : polygon coordinates
 ```
+
 ## License
 
 `pbaa` is distributed under the terms of the [Apache-2.0](https://spdx.org/licenses/Apache-2.0.html) license.
 
 ## Acknowledgements
 
 Grounded-Segment-Anything : [https://github.com/IDEA-Research/Grounded-Segment-Anything](https://github.com/IDEA-Research/Grounded-Segment-Anything)<br>
```

### Comparing `pbaa-1.0.2/pyproject.toml` & `pbaa-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.2/PKG-INFO` & `pbaa-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbaa
-Version: 1.0.2
+Version: 1.0.3
 Summary: Prompt based automatic annotation
 Project-URL: Documentation, https://github.com/dh031200/pbaa#readme
 Project-URL: Issues, https://github.com/dh031200/pbaa/issues
 Project-URL: Source, https://github.com/dh031200/pbaa
 Author-email: dh031200 <imbird0312@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
@@ -35,17 +35,30 @@
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [Usage](#Usage)
 - [Demo](#Demo)
 - [License](#license)
+- [Acknowledgements](#acknowledgements)
 
 ## Installation
 
+### Docker (Recommend)
+
+```console
+git clone https://github.com/dh031200/pbaa.git
+docker build docker -t pbaa:latest
+docker run --gpus all -it --ipc=host -v `pwd`:/workspace pbaa:latest
+```
+
+### Without docker
+
+The code requires `python>=3.8`, `CUDA==11.7`.
+
 ```console
 pip install pbaa
 ```
 
 ## Usage
 
 ### Options
@@ -75,40 +88,45 @@
 
 ### Python
 
 ```python
 from pbaa import model_init, inference
 
 model_init()
+# inference(<Source path>, <prompt:class>, box_threshold=0.25, nms_threshold=0.8, output_dir=".")
 inference("path/to/source_image.jpg", {"black dog": "dog", "white cat": "cat"})
 ```
 
 ## Demo
 
 ```console
-## Source : assets/demo9.jpg
-## prompts : {"plant" : "plant", "picture" : "picture", "dog": "dog", "lamp" : "lamp", "carpet" : "carpet", "sofa" : "sofa"}
+# Source : assets/demo9.jpg
+# prompts : {"plant" : "plant", "picture" : "picture", "dog": "dog", "lamp" : "lamp", "carpet" : "carpet", "sofa" : "sofa"}
 
 pbaa -s assets/demo9.jpg -p plant plant -p picture picture -p dog dog -p lamp lamp -p carpet carpet -p sofa sofa
 ```
 
-| Origin                                                                          | Detection                                                                              | Segmentation                                                                           |
-|---------------------------------------------------------------------------------|----------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------|
-| ![Before](https://github.com/dh031200/pbaa/blob/main/assets/demo9.jpg?raw=true) | ![detection](https://github.com/dh031200/pbaa/blob/main/assets/demo9_det.jpg?raw=true) | ![detection](https://github.com/dh031200/pbaa/blob/main/assets/demo9_seg.jpg?raw=true) |
+|                                     Origin                                      |                                       Detection                                        |                                       Segmentation                                        |
+|:-------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
+| ![Before](https://github.com/dh031200/pbaa/blob/main/assets/demo9.jpg?raw=true) | ![detection](https://github.com/dh031200/pbaa/blob/main/assets/demo9_det.jpg?raw=true) | ![segmentation](https://github.com/dh031200/pbaa/blob/main/assets/demo9_seg.jpg?raw=true) |
+
 ### Result data
-[demo9.json](assets/demo9.json)<br>
+
+[demo9.json](https://github.com/dh031200/pbaa/blob/main/assets/demo9.json)<br>
+
 ```console
 json structure
 
 index
   ├ cls : class name
   ├ conf : confidence score
   ├ box : bounding box coordinates
   └ poly : polygon coordinates
 ```
+
 ## License
 
 `pbaa` is distributed under the terms of the [Apache-2.0](https://spdx.org/licenses/Apache-2.0.html) license.
 
 ## Acknowledgements
 
 Grounded-Segment-Anything : [https://github.com/IDEA-Research/Grounded-Segment-Anything](https://github.com/IDEA-Research/Grounded-Segment-Anything)<br>
```

