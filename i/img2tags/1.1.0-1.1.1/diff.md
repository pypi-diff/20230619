# Comparing `tmp/img2tags-1.1.0.tar.gz` & `tmp/img2tags-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "img2tags-1.1.0.tar", max compression
+gzip compressed data, was "img2tags-1.1.1.tar", max compression
```

## Comparing `img2tags-1.1.0.tar` & `img2tags-1.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11342 2023-06-18 12:23:44.766767 img2tags-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1788 2023-06-18 13:00:34.408478 img2tags-1.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-18 12:23:44.766767 img2tags-1.1.0/img2tags/__init__.py
--rw-r--r--   0        0        0     7326 2023-06-18 12:59:53.016518 img2tags-1.1.0/img2tags/cli.py
--rw-r--r--   0        0        0     3085 2023-06-18 12:23:44.766767 img2tags-1.1.0/img2tags/tagger.py
--rw-r--r--   0        0        0     1318 2023-06-18 13:02:07.336388 img2tags-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2792 1970-01-01 00:00:00.000000 img2tags-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-06-18 12:23:44.766767 img2tags-1.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1822 2023-06-19 01:26:08.388203 img2tags-1.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 12:23:44.766767 img2tags-1.1.1/img2tags/__init__.py
+-rw-r--r--   0        0        0     7361 2023-06-19 01:24:55.292352 img2tags-1.1.1/img2tags/cli.py
+-rw-r--r--   0        0        0     3085 2023-06-18 12:23:44.766767 img2tags-1.1.1/img2tags/tagger.py
+-rw-r--r--   0        0        0     1318 2023-06-19 01:25:11.772318 img2tags-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 img2tags-1.1.1/PKG-INFO
```

### Comparing `img2tags-1.1.0/LICENSE.txt` & `img2tags-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `img2tags-1.1.0/README.md` & `img2tags-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/img2tags.svg)](https://pypi.org/project/img2tags/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Downloads](https://pepy.tech/badge/img2tags/week)](https://pepy.tech/project/img2tags)
 
 [![CI](https://github.com/shirayu/img2tags/actions/workflows/ci.yml/badge.svg)](https://github.com/shirayu/img2tags/actions/workflows/ci.yml)
 [![Typos](https://github.com/shirayu/img2tags/actions/workflows/typos.yml/badge.svg)](https://github.com/shirayu/img2tags/actions/workflows/typos.yml)
 
-Tag images by using onnxruntime.
+Tag images by using [ONNX Runtime](https://onnxruntime.ai/).
 The current default model is the converted ``WD 1.4 ConvNext Tagger V2`` on <https://huggingface.co/shirayu/img2tags>.
 It works fine for anime images.
 
 ## Setup
 
 ```bash
 # For CPU
-pip install 'img2tags[cpu]'
+pip install -U 'img2tags[cpu]'
 
 # For GPU
-pip install 'img2tags[gpu]'
+pip install -U 'img2tags[gpu]'
 ```
 
 ## Run
 
 ```bash
 # Generate .txt file
 img2tags -i input_dir
```

### Comparing `img2tags-1.1.0/img2tags/cli.py` & `img2tags-1.1.1/img2tags/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,14 +219,16 @@
         "--model",
         "-m",
         type=str,
         default="shirayu/img2tags/SmilingWolf__wd-v1-4-convnext-tagger-v2",
     )
     parser.add_argument(
         "--batch_size",
+        "--batch",
+        "--bs",
         type=int,
         default=1,
     )
     parser.add_argument(
         "--max_data_loader_n_workers",
         type=int,
         default=2,
```

### Comparing `img2tags-1.1.0/img2tags/tagger.py` & `img2tags-1.1.1/img2tags/tagger.py`

 * *Files identical despite different names*

### Comparing `img2tags-1.1.0/pyproject.toml` & `img2tags-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "img2tags"
-version = "1.1.0"
+version = "1.1.1"
 description = "Tag images"
 authors = ["Yuta Hayashibe <yuta@hayashibe.jp>"]
 readme = "README.md"
 homepage = "https://github.com/shirayu/img2tags"
 repository = "https://github.com/shirayu/img2tags"
 packages = [{include = "img2tags"}]
```

### Comparing `img2tags-1.1.0/PKG-INFO` & `img2tags-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2tags
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tag images
 Home-page: https://github.com/shirayu/img2tags
 Author: Yuta Hayashibe
 Author-email: yuta@hayashibe.jp
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -32,26 +32,26 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/img2tags.svg)](https://pypi.org/project/img2tags/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Downloads](https://pepy.tech/badge/img2tags/week)](https://pepy.tech/project/img2tags)
 
 [![CI](https://github.com/shirayu/img2tags/actions/workflows/ci.yml/badge.svg)](https://github.com/shirayu/img2tags/actions/workflows/ci.yml)
 [![Typos](https://github.com/shirayu/img2tags/actions/workflows/typos.yml/badge.svg)](https://github.com/shirayu/img2tags/actions/workflows/typos.yml)
 
-Tag images by using onnxruntime.
+Tag images by using [ONNX Runtime](https://onnxruntime.ai/).
 The current default model is the converted ``WD 1.4 ConvNext Tagger V2`` on <https://huggingface.co/shirayu/img2tags>.
 It works fine for anime images.
 
 ## Setup
 
 ```bash
 # For CPU
-pip install 'img2tags[cpu]'
+pip install -U 'img2tags[cpu]'
 
 # For GPU
-pip install 'img2tags[gpu]'
+pip install -U 'img2tags[gpu]'
 ```
 
 ## Run
 
 ```bash
 # Generate .txt file
 img2tags -i input_dir
```

