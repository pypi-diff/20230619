# Comparing `tmp/dreamai_ray-0.0.1.tar.gz` & `tmp/dreamai_ray-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai_ray-0.0.1.tar", last modified: Fri Jun  9 13:08:23 2023, max compression
+gzip compressed data, was "dreamai_ray-0.0.2.tar", last modified: Mon Jun 19 06:03:07 2023, max compression
```

## Comparing `dreamai_ray-0.0.1.tar` & `dreamai_ray-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,36 @@
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-06-09 13:08:23.605931 dreamai_ray-0.0.1/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_ray-0.0.1/LICENSE
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_ray-0.0.1/MANIFEST.in
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      854 2023-06-09 13:08:23.605931 dreamai_ray-0.0.1/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      123 2023-06-07 14:33:01.000000 dreamai_ray-0.0.1/README.md
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-06-09 13:08:23.605931 dreamai_ray-0.0.1/dreamai_ray/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-06-09 12:42:50.000000 dreamai_ray-0.0.1/dreamai_ray/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    13590 2023-06-09 12:42:50.000000 dreamai_ray-0.0.1/dreamai_ray/_modidx.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      932 2023-06-07 18:33:34.000000 dreamai_ray-0.0.1/dreamai_ray/imports.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2167 2023-06-09 12:42:50.000000 dreamai_ray-0.0.1/dreamai_ray/mapper.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-06-09 13:08:23.605931 dreamai_ray-0.0.1/dreamai_ray/pdf/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        0 2023-06-09 12:42:50.000000 dreamai_ray-0.0.1/dreamai_ray/pdf/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11737 2023-06-09 12:42:50.000000 dreamai_ray-0.0.1/dreamai_ray/pdf/app.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     4830 2023-06-09 12:42:50.000000 dreamai_ray-0.0.1/dreamai_ray/pdf/core.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     4154 2023-06-09 12:42:50.000000 dreamai_ray-0.0.1/dreamai_ray/pdf/df.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     6659 2023-06-09 12:42:50.000000 dreamai_ray-0.0.1/dreamai_ray/pdf/extract.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     1074 2023-06-09 12:42:50.000000 dreamai_ray-0.0.1/dreamai_ray/pdf/mappers.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2363 2023-06-09 12:42:50.000000 dreamai_ray-0.0.1/dreamai_ray/pdf/ner.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     1822 2023-06-07 16:18:46.000000 dreamai_ray-0.0.1/dreamai_ray/redis_kv_store.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     6206 2023-06-09 12:42:50.000000 dreamai_ray-0.0.1/dreamai_ray/utils.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-06-09 13:08:23.605931 dreamai_ray-0.0.1/dreamai_ray.egg-info/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      854 2023-06-09 13:08:23.000000 dreamai_ray-0.0.1/dreamai_ray.egg-info/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      614 2023-06-09 13:08:23.000000 dreamai_ray-0.0.1/dreamai_ray.egg-info/SOURCES.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-06-09 13:08:23.000000 dreamai_ray-0.0.1/dreamai_ray.egg-info/dependency_links.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       44 2023-06-09 13:08:23.000000 dreamai_ray-0.0.1/dreamai_ray.egg-info/entry_points.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-06-07 14:32:47.000000 dreamai_ray-0.0.1/dreamai_ray.egg-info/not-zip-safe
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      121 2023-06-09 13:08:23.000000 dreamai_ray-0.0.1/dreamai_ray.egg-info/requires.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       12 2023-06-09 13:08:23.000000 dreamai_ray-0.0.1/dreamai_ray.egg-info/top_level.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      799 2023-06-09 02:42:37.000000 dreamai_ray-0.0.1/settings.ini
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-06-09 13:08:23.605931 dreamai_ray-0.0.1/setup.cfg
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_ray-0.0.1/setup.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-06-19 06:03:07.813552 dreamai_ray-0.0.2/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_ray-0.0.2/LICENSE
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_ray-0.0.2/MANIFEST.in
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      854 2023-06-19 06:03:07.813552 dreamai_ray-0.0.2/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      123 2023-06-07 14:33:01.000000 dreamai_ray-0.0.2/README.md
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-06-19 06:03:07.809553 dreamai_ray-0.0.2/dreamai_ray/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-06-19 06:02:56.000000 dreamai_ray-0.0.2/dreamai_ray/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    20871 2023-06-19 06:02:56.000000 dreamai_ray-0.0.2/dreamai_ray/_modidx.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      893 2023-06-18 03:46:21.000000 dreamai_ray-0.0.2/dreamai_ray/imports.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-06-19 06:03:07.809553 dreamai_ray-0.0.2/dreamai_ray/index/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        0 2023-06-19 06:02:56.000000 dreamai_ray-0.0.2/dreamai_ray/index/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     4425 2023-06-19 06:02:56.000000 dreamai_ray-0.0.2/dreamai_ray/index/core.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     1667 2023-06-19 06:02:56.000000 dreamai_ray-0.0.2/dreamai_ray/index/df.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     1829 2023-06-19 06:02:56.000000 dreamai_ray-0.0.2/dreamai_ray/index/utils.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     4602 2023-06-19 06:02:56.000000 dreamai_ray-0.0.2/dreamai_ray/mapper.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-06-19 06:03:07.809553 dreamai_ray-0.0.2/dreamai_ray/pdf/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        0 2023-06-19 06:02:56.000000 dreamai_ray-0.0.2/dreamai_ray/pdf/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    11738 2023-06-19 06:02:56.000000 dreamai_ray-0.0.2/dreamai_ray/pdf/app.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     3384 2023-06-19 06:02:56.000000 dreamai_ray-0.0.2/dreamai_ray/pdf/df.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     6660 2023-06-19 06:02:56.000000 dreamai_ray-0.0.2/dreamai_ray/pdf/extract.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     1076 2023-06-19 06:02:56.000000 dreamai_ray-0.0.2/dreamai_ray/pdf/mappers.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2564 2023-06-19 06:02:56.000000 dreamai_ray-0.0.2/dreamai_ray/pdf/ner.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     5416 2023-06-19 06:02:56.000000 dreamai_ray-0.0.2/dreamai_ray/pdf/utils.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     1822 2023-06-07 16:18:46.000000 dreamai_ray-0.0.2/dreamai_ray/redis_kv_store.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     6206 2023-06-19 06:02:56.000000 dreamai_ray-0.0.2/dreamai_ray/utils.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-06-19 06:03:07.809553 dreamai_ray-0.0.2/dreamai_ray.egg-info/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      854 2023-06-19 06:03:07.000000 dreamai_ray-0.0.2/dreamai_ray.egg-info/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      722 2023-06-19 06:03:07.000000 dreamai_ray-0.0.2/dreamai_ray.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-06-19 06:03:07.000000 dreamai_ray-0.0.2/dreamai_ray.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       44 2023-06-19 06:03:07.000000 dreamai_ray-0.0.2/dreamai_ray.egg-info/entry_points.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-06-07 14:32:47.000000 dreamai_ray-0.0.2/dreamai_ray.egg-info/not-zip-safe
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      128 2023-06-19 06:03:07.000000 dreamai_ray-0.0.2/dreamai_ray.egg-info/requires.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       12 2023-06-19 06:03:07.000000 dreamai_ray-0.0.2/dreamai_ray.egg-info/top_level.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      804 2023-06-19 06:02:45.000000 dreamai_ray-0.0.2/settings.ini
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-06-19 06:03:07.813552 dreamai_ray-0.0.2/setup.cfg
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_ray-0.0.2/setup.py
```

### Comparing `dreamai_ray-0.0.1/LICENSE` & `dreamai_ray-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dreamai_ray-0.0.1/PKG-INFO` & `dreamai_ray-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai_ray
-Version: 0.0.1
+Version: 0.0.2
 Summary: DreamAI platform leveraging RAY.
 Home-page: https://github.com/HamzaFarhan/dreamai_ray
 Author: Hamza Farhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_ray-0.0.1/dreamai_ray/imports.py` & `dreamai_ray-0.0.2/dreamai_ray/imports.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from dreamai.imports import *
 from dreamai.core import *
 
+import faiss
 import requests
 import subprocess
 from torch import nn
-
-# import pandas as pd
 from pypdf import PdfReader
 from ast import literal_eval
 from setfit import SetFitModel
 from fastai.torch_core import default_device
 from sentence_transformers import SentenceTransformer
 from transformers import (
     AutoTokenizer,
@@ -17,16 +16,14 @@
     AutoModelForSequenceClassification,
     AutoModelForTokenClassification,
     pipeline,
 )
 
 import ray
 from ray import serve
-
-# import modin.pandas as pd
 from ray import data as rd
 from ray.air import Checkpoint
 from ray.train.predictor import Predictor
 from ray.train.batch_predictor import BatchPredictor
 from ray.data.preprocessors import Chain, BatchMapper
 from ray.serve.air_integrations import PredictorDeployment
 from ray.air.util.data_batch_conversion import BatchFormat
```

### Comparing `dreamai_ray-0.0.1/dreamai_ray/pdf/app.py` & `dreamai_ray-0.0.2/dreamai_ray/pdf/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # %% auto 0
 __all__ = ['SegsPredictor', 'NERPredictor', 'EmsPredictor', 'pdf_pipeline', 'ner_pipeline', 'pdf_pipeline_params',
            'ner_pipeline_params']
 
 # %% ../../nbs/pdf/05_app.ipynb 2
 from ..imports import *
 from ..utils import *
-from .core import *
+from .utils import *
 from .extract import *
 from .ner import *
 from .df import *
 from .. import redis_kv_store
 
 
 # %% ../../nbs/pdf/05_app.ipynb 4
```

### Comparing `dreamai_ray-0.0.1/dreamai_ray/pdf/core.py` & `dreamai_ray-0.0.2/dreamai_ray/pdf/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,37 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/pdf/00_core.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/pdf/00_utils.ipynb.
 
 # %% auto 0
-__all__ = ['cid_to_char', 'process_text', 'process_line', 'extract_text', 'extract_text_list', 'extract_text_dict']
+__all__ = ['create_paths_df', 'create_pdf_df', 'extract_df_text', 'cid_to_char', 'process_text', 'process_line', 'extract_text',
+           'extract_text_list', 'extract_text_dict']
 
-# %% ../../nbs/pdf/00_core.ipynb 2
+# %% ../../nbs/pdf/00_utils.ipynb 2
 from ..imports import *
 
 
-# %% ../../nbs/pdf/00_core.ipynb 4
+# %% ../../nbs/pdf/00_utils.ipynb 4
+def create_paths_df(data_path, suffix=".pdf"):
+    files = [str(x) for x in resolve_data_path(data_path) if Path(x).suffix == suffix]
+    df = pd.DataFrame({"path": files})
+    return df
+
+
+def create_pdf_df(data_path, segs_folder, ems_folder):
+    df = create_paths_df(data_path, suffix=".pdf")
+    df["segs_folder"] = str(segs_folder)
+    df["ems_folder"] = str(ems_folder)
+    return df
+
+
+
+def extract_df_text(df, col="path", n_lines=3):
+    df["text"] = extract_text_list(df[col], n_lines=n_lines)
+    return df
+
+
 def cid_to_char(cidx: str):
     try:
         return chr(int(re.findall(r"\(cid\:(\d+)\)", cidx)[0]) + 29)
     except:
         return cidx
```

### Comparing `dreamai_ray-0.0.1/dreamai_ray/pdf/df.py` & `dreamai_ray-0.0.2/dreamai_ray/pdf/df.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,20 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/pdf/02_df.ipynb.
 
 # %% auto 0
-__all__ = ['create_pdf_df', 'create_ner_df', 'extract_df_text', 'write_df_ner', 'df_segs', 'write_df_segs', 'write_df_ems']
+__all__ = ['write_df_ner', 'df_segs', 'write_df_segs', 'write_df_ems']
 
 # %% ../../nbs/pdf/02_df.ipynb 2
 from ..imports import *
 from ..utils import *
-from .core import *
+from .utils import *
 from .extract import *
 from .ner import *
 
-
 # %% ../../nbs/pdf/02_df.ipynb 4
-def create_pdf_df(data_path, segs_folder, ems_folder):
-    files = [str(x) for x in resolve_data_path(data_path) if Path(x).suffix == ".pdf"]
-    df = pd.DataFrame({"path": files})
-    df["segs_folder"] = str(segs_folder)
-    df["ems_folder"] = str(ems_folder)
-    return df
-
-
-def create_ner_df(data_path, segs_folder):
-    data_path = Path(data_path)
-    if data_path.is_file():
-        files = [str(data_path)]
-    else:
-        files = get_files(data_path, extensions=[".pdf"], make_str=True)
-    df = pd.DataFrame({"path": files})
-    df["segs_folder"] = str(segs_folder)
-    return df
-
-
-def extract_df_text(df, col="path", n_lines=3):
-    df["text"] = extract_text_list(df[col], n_lines=n_lines)
-    return df
-
-
 def write_df_ner(df, tner, jner, work_ner_dict={"company": "", "date": ""}):
     segs_path = json_file(df["path"], df["segs_folder"])
     if os.path.exists(segs_path):
         with open(segs_path, "r") as f:
             segs = json.load(f)
         if not is_list(segs["Work Experience"][0]):
             segs = {k: [v] for k, v in segs.items()}
```

### Comparing `dreamai_ray-0.0.1/dreamai_ray/pdf/extract.py` & `dreamai_ray-0.0.2/dreamai_ray/pdf/extract.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # %% auto 0
 __all__ = ['add_other_class', 'print_segments', 'text_to_segments', 'text_to_ems', 'load_segs_model', 'load_ems_model',
            'write_segments', 'write_embeddings']
 
 # %% ../../nbs/pdf/01_extract.ipynb 2
 from ..imports import *
-from .core import *
+from .utils import *
 
 # %% ../../nbs/pdf/01_extract.ipynb 4
 def add_other_class(classes, other_class="Other"):
     # Add 'Other' class if not present
     if other_class not in classes:
         classes.append(other_class)
     return classes
@@ -90,24 +90,24 @@
     data_path,
     output_path="pdf_segments",
     n_lines=3,
     classes=["Work Experience", "Education", "Certifications", "Other"],
     other_class="Other",
 ):
     """
-    Extracts text from PDFs and writes segments to JSON files.
+    Extracts text from PDFs and writes segments to json files.
 
     Parameters
     ----------
     segs_model : SetFitModel
         SetFit model for segment classification.
     data_path : Union[str, Path, List[Union[str, Path]]]
         Path to PDFs. Can be a single file, a directory, or a list of files/directories.
     output_path : Union[str, Path]
-        Folder to write JSON files. Defaults to 'pdf_segments'.
+        Folder to write json files. Defaults to 'pdf_segments'.
     n_lines : int
         Number of lines to group together when extracting text from PDFs.
     classes : List[str]
         List of segment classes. Defaults to ["Work Experience", "Education", "Certifications", "Other"].
     other_class : str
         Name of the 'Other' class. Defaults to "Other".
     Returns
@@ -142,26 +142,26 @@
     data_path,
     output_path="pdf_ems",
     n_lines=3,
     classes=["Work Experience", "Education", "Certifications", "Other"],
     other_class="Other",
 ):
     """
-    Extracts text from PDFs and writes embeddings to JSON files.
+    Extracts text from PDFs and writes embeddings to json files.
 
     Parameters
     ----------
     segs_model : SetFitModel
         SetFit model for segment classification.
     ems_model : SentenceTransformer
         SentenceTransformer model for embedding generation.
     data_path : Union[str, Path, List[Union[str, Path]]]
         Path to PDFs. Can be a single file, a directory, or a list of files/directories.
     output_path : Union[str, Path]
-        Folder to write JSON files. Defaults to 'pdf_ems'.
+        Folder to write json files. Defaults to 'pdf_ems'.
     n_lines : int
         Number of lines to group together when extracting text from PDFs.
     classes : List[str]
         List of segment classes. Defaults to ["Work Experience", "Education", "Certifications", "Other"].
     other_class : str
         Name of the 'Other' class. Defaults to "Other".
     Returns
```

### Comparing `dreamai_ray-0.0.1/dreamai_ray/pdf/mappers.py` & `dreamai_ray-0.0.2/dreamai_ray/pdf/mappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # %% ../../nbs/pdf/04_mappers.ipynb 2
 from ..imports import *
 from ..utils import *
 from ..mapper import *
 from .extract import *
 from .df import *
 
+
 # %% ../../nbs/pdf/04_mappers.ipynb 4
 class SegsMapper(Mapper):
     """
     A custom mapper for PDF segmentation. It uses the `df_segs` function to extract the segments from the PDF.
     """
 
     def __init__(
@@ -26,7 +27,8 @@
             other_class="Other",
         ),
         **kwargs,
     ):
         segs_model = load_segs_model(segs_model, device=default_device())
         udf_kwargs["segs_model"] = segs_model
         super().__init__(**locals_to_params(locals()))
+
```

### Comparing `dreamai_ray-0.0.1/dreamai_ray/pdf/ner.py` & `dreamai_ray-0.0.2/dreamai_ray/pdf/ner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/pdf/03_ner.ipynb.
 
 # %% auto 0
-__all__ = ['load_ner_model', 'load_job_model', 'proc_ner', 'job_ner', 'edu_ner', 'work_ner', 'is_valid_jner', 'is_valid_tner']
+__all__ = ['create_ner_df', 'load_ner_model', 'load_job_model', 'proc_ner', 'job_ner', 'edu_ner', 'work_ner', 'is_valid_jner',
+           'is_valid_tner']
 
 # %% ../../nbs/pdf/03_ner.ipynb 2
 from ..imports import *
+from .utils import *
+
 
 # %% ../../nbs/pdf/03_ner.ipynb 4
+def create_ner_df(data_path, segs_folder):
+    df = create_paths_df(data_path, suffix=".pdf")
+    df["segs_folder"] = str(segs_folder)
+    return df
+
+
 def load_ner_model(model_name="tner/deberta-v3-large-ontonotes5", device="cpu"):
     tokenizer = AutoTokenizer.from_pretrained(model_name)
     model = AutoModelForTokenClassification.from_pretrained(model_name)
     return pipeline(
         "ner",
         model=model,
         tokenizer=tokenizer,
```

### Comparing `dreamai_ray-0.0.1/dreamai_ray/redis_kv_store.py` & `dreamai_ray-0.0.2/dreamai_ray/redis_kv_store.py`

 * *Files identical despite different names*

### Comparing `dreamai_ray-0.0.1/dreamai_ray/utils.py` & `dreamai_ray-0.0.2/dreamai_ray/utils.py`

 * *Files identical despite different names*

### Comparing `dreamai_ray-0.0.1/dreamai_ray.egg-info/PKG-INFO` & `dreamai_ray-0.0.2/dreamai_ray.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai-ray
-Version: 0.0.1
+Version: 0.0.2
 Summary: DreamAI platform leveraging RAY.
 Home-page: https://github.com/HamzaFarhan/dreamai_ray
 Author: Hamza Farhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_ray-0.0.1/settings.ini` & `dreamai_ray-0.0.2/settings.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dreamai_ray
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.8
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = dreamai_ray
 nbs_path = nbs
 recursive = True
@@ -22,9 +22,8 @@
 author_email = thehamza96@gmail.com
 copyright = 2023 onwards, %(author)s
 description = DreamAI platform leveraging RAY.
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = HamzaFarhan
-pip_requirements = "ray[air]" dreamai fastai fastapi modin pandas pypdf redis requests sentence_transformers setfit torch transformers
-
+pip_requirements = "ray[air]" dreamai fastai pypdf redis requests sentence_transformers setfit setuptools torch transformers wasabi faiss-cpu
```

### Comparing `dreamai_ray-0.0.1/setup.py` & `dreamai_ray-0.0.2/setup.py`

 * *Files identical despite different names*

