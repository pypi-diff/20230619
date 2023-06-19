# Comparing `tmp/pbaa-1.0.1.tar.gz` & `tmp/pbaa-1.0.2.tar.gz`

## Comparing `pbaa-1.0.1.tar` & `pbaa-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 pbaa-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pbaa-1.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0  5701095 2020-02-02 00:00:00.000000 pbaa-1.0.1/assets/demo9.jpg
--rw-r--r--   0        0        0   720440 2020-02-02 00:00:00.000000 pbaa-1.0.1/assets/demo9.json
--rw-r--r--   0        0        0  1287943 2020-02-02 00:00:00.000000 pbaa-1.0.1/assets/demo9_det.jpg
--rw-r--r--   0        0        0  1239235 2020-02-02 00:00:00.000000 pbaa-1.0.1/assets/demo9_seg.jpg
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pbaa-1.0.1/src/pbaa/__about__.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 pbaa-1.0.1/src/pbaa/__init__.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 pbaa-1.0.1/src/pbaa/__main__.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 pbaa-1.0.1/src/pbaa/cli/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pbaa-1.0.1/src/pbaa/core/__init__.py
--rw-r--r--   0        0        0     6782 2020-02-02 00:00:00.000000 pbaa-1.0.1/src/pbaa/core/check.py
--rw-r--r--   0        0        0     5046 2020-02-02 00:00:00.000000 pbaa-1.0.1/src/pbaa/core/grounded_sam.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 pbaa-1.0.1/src/pbaa/core/prerequisite.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 pbaa-1.0.1/src/pbaa/core/utils.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 pbaa-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pbaa-1.0.1/tests/test_dependencies.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 pbaa-1.0.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 pbaa-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 pbaa-1.0.1/README.md
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 pbaa-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 pbaa-1.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0      434 2020-02-02 00:00:00.000000 pbaa-1.0.2/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0     1077 2020-02-02 00:00:00.000000 pbaa-1.0.2/.github/workflows/test.yml
+-rwxr-xr-x   0        0        0  5701095 2020-02-02 00:00:00.000000 pbaa-1.0.2/assets/demo9.jpg
+-rwxr-xr-x   0        0        0   720440 2020-02-02 00:00:00.000000 pbaa-1.0.2/assets/demo9.json
+-rwxr-xr-x   0        0        0  1287943 2020-02-02 00:00:00.000000 pbaa-1.0.2/assets/demo9_det.jpg
+-rwxr-xr-x   0        0        0  1239235 2020-02-02 00:00:00.000000 pbaa-1.0.2/assets/demo9_seg.jpg
+-rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 pbaa-1.0.2/src/pbaa/__about__.py
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 pbaa-1.0.2/src/pbaa/__init__.py
+-rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 pbaa-1.0.2/src/pbaa/__main__.py
+-rwxr-xr-x   0        0        0     1111 2020-02-02 00:00:00.000000 pbaa-1.0.2/src/pbaa/cli/__init__.py
+-rwxr-xr-x   0        0        0      248 2020-02-02 00:00:00.000000 pbaa-1.0.2/src/pbaa/core/__init__.py
+-rwxr-xr-x   0        0        0     6782 2020-02-02 00:00:00.000000 pbaa-1.0.2/src/pbaa/core/check.py
+-rwxr-xr-x   0        0        0     5059 2020-02-02 00:00:00.000000 pbaa-1.0.2/src/pbaa/core/grounded_sam.py
+-rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 pbaa-1.0.2/src/pbaa/core/prerequisite.py
+-rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 pbaa-1.0.2/src/pbaa/core/utils.py
+-rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 pbaa-1.0.2/tests/__init__.py
+-rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 pbaa-1.0.2/tests/test_dependencies.py
+-rwxr-xr-x   0        0        0     3092 2020-02-02 00:00:00.000000 pbaa-1.0.2/.gitignore
+-rwxr-xr-x   0        0        0    10280 2020-02-02 00:00:00.000000 pbaa-1.0.2/LICENSE.txt
+-rwxr-xr-x   0        0        0     3361 2020-02-02 00:00:00.000000 pbaa-1.0.2/README.md
+-rwxr-xr-x   0        0        0     3252 2020-02-02 00:00:00.000000 pbaa-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 pbaa-1.0.2/PKG-INFO
```

### Comparing `pbaa-1.0.1/.github/workflows/test.yml` & `pbaa-1.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.1/assets/demo9.jpg` & `pbaa-1.0.2/assets/demo9.jpg`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.1/assets/demo9.json` & `pbaa-1.0.2/assets/demo9.json`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.1/assets/demo9_det.jpg` & `pbaa-1.0.2/assets/demo9_det.jpg`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.1/assets/demo9_seg.jpg` & `pbaa-1.0.2/assets/demo9_seg.jpg`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.1/src/pbaa/cli/__init__.py` & `pbaa-1.0.2/src/pbaa/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.1/src/pbaa/core/check.py` & `pbaa-1.0.2/src/pbaa/core/check.py`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.1/src/pbaa/core/grounded_sam.py` & `pbaa-1.0.2/src/pbaa/core/grounded_sam.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     for box in xyxy:
         masks, scores, logits = sam_predictor.predict(box=box, multimask_output=True)
         index = np.argmax(scores)
         result_masks.append(masks[index])
     return np.array(result_masks)
 
 
-def inference(_src, _prompt, box_threshold, nms_threshold, output_dir):
+def inference(_src, _prompt, box_threshold=0.25, nms_threshold=0.8, output_dir="."):
     src = Path(_src)
     dst = Path(output_dir)
     _prompt = {i.lower(): v for i, v in _prompt}
 
     # Building GroundingDINO inference model
     grounding_dino_model = Model(
         model_config_path=grounding_dino_config_path, model_checkpoint_path=GROUNDING_DINO_CHECKPOINT_PATH
```

### Comparing `pbaa-1.0.1/.gitignore` & `pbaa-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.1/LICENSE.txt` & `pbaa-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.1/README.md` & `pbaa-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.1/pyproject.toml` & `pbaa-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.1/PKG-INFO` & `pbaa-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbaa
-Version: 1.0.1
+Version: 1.0.2
 Summary: Prompt based automatic annotation
 Project-URL: Documentation, https://github.com/dh031200/pbaa#readme
 Project-URL: Issues, https://github.com/dh031200/pbaa/issues
 Project-URL: Source, https://github.com/dh031200/pbaa
 Author-email: dh031200 <imbird0312@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

