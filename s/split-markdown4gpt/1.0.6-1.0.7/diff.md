# Comparing `tmp/split_markdown4gpt-1.0.6.tar.gz` & `tmp/split_markdown4gpt-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "split_markdown4gpt-1.0.6.tar", last modified: Sun Jun 18 02:07:46 2023, max compression
+gzip compressed data, was "split_markdown4gpt-1.0.7.tar", last modified: Mon Jun 19 17:31:42 2023, max compression
```

## Comparing `split_markdown4gpt-1.0.6.tar` & `split_markdown4gpt-1.0.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:07:46.134235 split_markdown4gpt-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:07:46.130234 split_markdown4gpt-1.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:07:46.130234 split_markdown4gpt-1.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/API.md
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-06-18 02:07:46.134235 split_markdown4gpt-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/pydoc-markdown.yml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-18 02:07:46.134235 split_markdown4gpt-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:07:46.130234 split_markdown4gpt-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:07:46.130234 split_markdown4gpt-1.0.6/src/split_markdown4gpt/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/src/split_markdown4gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/src/split_markdown4gpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/src/split_markdown4gpt/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:07:46.134235 split_markdown4gpt-1.0.6/src/split_markdown4gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-06-18 02:07:46.000000 split_markdown4gpt-1.0.6/src/split_markdown4gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-18 02:07:46.000000 split_markdown4gpt-1.0.6/src/split_markdown4gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:07:46.000000 split_markdown4gpt-1.0.6/src/split_markdown4gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-18 02:07:46.000000 split_markdown4gpt-1.0.6/src/split_markdown4gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:07:45.000000 split_markdown4gpt-1.0.6/src/split_markdown4gpt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-18 02:07:46.000000 split_markdown4gpt-1.0.6/src/split_markdown4gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 02:07:46.000000 split_markdown4gpt-1.0.6/src/split_markdown4gpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:07:46.134235 split_markdown4gpt-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/tests/test.md
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/tests/test_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:31:42.810658 split_markdown4gpt-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:31:42.806658 split_markdown4gpt-1.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:31:42.810658 split_markdown4gpt-1.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/API.md
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-19 17:31:42.810658 split_markdown4gpt-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/pydoc-markdown.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-19 17:31:42.814658 split_markdown4gpt-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:31:42.806658 split_markdown4gpt-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:31:42.810658 split_markdown4gpt-1.0.7/src/split_markdown4gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/src/split_markdown4gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/src/split_markdown4gpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14635 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/src/split_markdown4gpt/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:31:42.810658 split_markdown4gpt-1.0.7/src/split_markdown4gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-19 17:31:42.000000 split_markdown4gpt-1.0.7/src/split_markdown4gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-19 17:31:42.000000 split_markdown4gpt-1.0.7/src/split_markdown4gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 17:31:42.000000 split_markdown4gpt-1.0.7/src/split_markdown4gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-19 17:31:42.000000 split_markdown4gpt-1.0.7/src/split_markdown4gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 17:31:42.000000 split_markdown4gpt-1.0.7/src/split_markdown4gpt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-19 17:31:42.000000 split_markdown4gpt-1.0.7/src/split_markdown4gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 17:31:42.000000 split_markdown4gpt-1.0.7/src/split_markdown4gpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:31:42.810658 split_markdown4gpt-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/tests/test.md
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/tests/test_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/tox.ini
```

### Comparing `split_markdown4gpt-1.0.6/.DS_Store` & `split_markdown4gpt-1.0.7/.DS_Store`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.6/.coveragerc` & `split_markdown4gpt-1.0.7/.coveragerc`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.6/.github/workflows/ci.yml` & `split_markdown4gpt-1.0.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.6/.gitignore` & `split_markdown4gpt-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.6/.pre-commit-config.yaml` & `split_markdown4gpt-1.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.6/API.md` & `split_markdown4gpt-1.0.7/API.md`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.6/LICENSE.txt` & `split_markdown4gpt-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.6/PKG-INFO` & `split_markdown4gpt-1.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: split_markdown4gpt
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python tool for splitting large Markdown files into smaller sections based on a specified token limit. This is particularly useful for processing large Markdown files with GPT models, as it allows the models to handle the data in manageable chunks.
 Home-page: https://github.com/twardoch/split-markdown4gpt
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: Apache-2.0
 Project-URL: Documentation, https://twardoch.github.io/split-markdown4gpt/
 Project-URL: Source, https://github.com/twardoch/split-markdown4gpt
@@ -25,15 +25,15 @@
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # split_markdown4gpt
 
 `split_markdown4gpt` is a Python tool designed to split large Markdown files into smaller sections based on a specified token limit. This is particularly useful for processing large Markdown files with GPT models, as it allows the models to handle the data in manageable chunks.
 
-_**Version 1.0.6** (2023-06-18)_
+_**Version 1.0.7** (2023-06-19)_
 
 ## Installation
 
 You can install `split_markdown4gpt` via pip:
 
 ```bash
 pip install split_markdown4gpt
@@ -116,20 +116,26 @@
 - `syntok` for splitting the text into sentences.
 - `regex` and `PyYAML` for various utility functions.
 
 ### Use Cases
 
 `split_markdown4gpt` is particularly useful in scenarios where you need to process large Markdown files with GPT models. For instance:
 
-- **Text Generation**: If you're using a GPT model to generate text based on a large Markdown file, you can use `split_markdown4gpt` to split the file into manageable sections. This allows the GPT model to process the file in chunks, preventing memory overflow errors.
+- **Text Generation**: If you're using a GPT model to generate text based on a large Markdown file, you can use `split_markdown4gpt` to split the file into manageable sections. This allows the GPT model to process the file in chunks, preventing token overflow errors.
 
 - **Data Preprocessing**: In machine learning projects, you often need to preprocess your data before feeding it into your model. If your data is in the form of large Markdown files, `split_markdown4gpt` can help you split these files into smaller sections based on the token limit of your model.
 
 - **Document Analysis**: If you're analyzing large Markdown documents (e.g., extracting keywords, summarizing content), you can use `split_markdown4gpt` to break down the documents into smaller sections. This makes the analysis more manageable and efficient.
 
+## Changelog
+
+- v1.0.7: Switched the model for each section from namedtuple to dict
+- v1.0.6: Fixes
+- v1.0.0: Initial release
+
 ## Contributing
 
 Contributions to `split_markdown4gpt` are welcome! Please open an issue or submit a pull request on the [GitHub repository](https://github.com/twardoch/split-markdown4gpt).
 
 ## License
 
 - Copyright (c) 2023 [Adam Twardoch](./AUTHORS.md)
```

### Comparing `split_markdown4gpt-1.0.6/README.md` & `split_markdown4gpt-1.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # split_markdown4gpt
 
 `split_markdown4gpt` is a Python tool designed to split large Markdown files into smaller sections based on a specified token limit. This is particularly useful for processing large Markdown files with GPT models, as it allows the models to handle the data in manageable chunks.
 
-_**Version 1.0.6** (2023-06-18)_
+_**Version 1.0.7** (2023-06-19)_
 
 ## Installation
 
 You can install `split_markdown4gpt` via pip:
 
 ```bash
 pip install split_markdown4gpt
@@ -89,20 +89,26 @@
 - `syntok` for splitting the text into sentences.
 - `regex` and `PyYAML` for various utility functions.
 
 ### Use Cases
 
 `split_markdown4gpt` is particularly useful in scenarios where you need to process large Markdown files with GPT models. For instance:
 
-- **Text Generation**: If you're using a GPT model to generate text based on a large Markdown file, you can use `split_markdown4gpt` to split the file into manageable sections. This allows the GPT model to process the file in chunks, preventing memory overflow errors.
+- **Text Generation**: If you're using a GPT model to generate text based on a large Markdown file, you can use `split_markdown4gpt` to split the file into manageable sections. This allows the GPT model to process the file in chunks, preventing token overflow errors.
 
 - **Data Preprocessing**: In machine learning projects, you often need to preprocess your data before feeding it into your model. If your data is in the form of large Markdown files, `split_markdown4gpt` can help you split these files into smaller sections based on the token limit of your model.
 
 - **Document Analysis**: If you're analyzing large Markdown documents (e.g., extracting keywords, summarizing content), you can use `split_markdown4gpt` to break down the documents into smaller sections. This makes the analysis more manageable and efficient.
 
+## Changelog
+
+- v1.0.7: Switched the model for each section from namedtuple to dict
+- v1.0.6: Fixes
+- v1.0.0: Initial release
+
 ## Contributing
 
 Contributions to `split_markdown4gpt` are welcome! Please open an issue or submit a pull request on the [GitHub repository](https://github.com/twardoch/split-markdown4gpt).
 
 ## License
 
 - Copyright (c) 2023 [Adam Twardoch](./AUTHORS.md)
```

### Comparing `split_markdown4gpt-1.0.6/setup.cfg` & `split_markdown4gpt-1.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.6/setup.py` & `split_markdown4gpt-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.6/src/split_markdown4gpt/__init__.py` & `split_markdown4gpt-1.0.7/src/split_markdown4gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.6/src/split_markdown4gpt/__main__.py` & `split_markdown4gpt-1.0.7/src/split_markdown4gpt/__main__.py`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.6/src/split_markdown4gpt/splitter.py` & `split_markdown4gpt-1.0.7/src/split_markdown4gpt/splitter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-from collections import defaultdict, namedtuple
+from collections import defaultdict
 from functools import lru_cache
 from io import TextIOWrapper
 from pathlib import Path
 from typing import Any, Dict, Generator, List, Tuple, Union
 
 try:
     import regex as re
@@ -12,34 +12,50 @@
 
 import frontmatter
 import tiktoken
 from mistletoe import Document, block_token, markdown_renderer, span_token
 from syntok.segmenter import analyze as syntok_analyze
 from yaml.parser import ParserError
 
+
+def meta_data(md: str) -> tuple:
+    try:
+        if hasattr(frontmatter, "Frontmatter"):
+            # frontmatter package is installed
+            metadata = frontmatter.Frontmatter.read(md)
+            meta = metadata["attributes"]
+            data = metadata["body"]
+        else:
+            # python-frontmatter package is installed
+            metadata = frontmatter.loads(md)
+            meta, data = metadata.metadata, metadata.content
+    except Exception:
+        meta, data = None
+
+    return meta or {}, data or md
+
+
 OPENAI_MODELS = {
     "gpt-4": 8192,
     "gpt-4-32k": 32768,
     "gpt-4-32k-0613": 32768,
     "gpt-4-0613": 8192,
     "gpt-3.5-turbo": 4096,
     "gpt-3.5-turbo-0613": 4096,
     "gpt-3.5-turbo-16k": 16384,
     "gpt-3.5-turbo-16k-0613": 16384,
 }
 
 RE_NEWLINES = re.compile("\n{3,}")
 
-Section = namedtuple("Section", ("md", "size"))
-
 
 class MarkdownLLMSplitter:
     """
     A class to split Markdown files into sections according to GPT token size limits. Currently supports OpenAI models only, since it uses the `tiktoken` library for tokenization.
-    
+
     Attributes:
         gptoker: GPT tokenizer instance used to calculate token sizes.
         gptok_limit: The maximum number of GPT tokens allowed per section.
         md_meta: Metadata found in the source Markdown file.
         md_str: The source Markdown string.
         md_doc: The parsed source Markdown document as a mistletoe Document instance.
         md_dict: A dictionary representing the structure of the Markdown document.
@@ -77,27 +93,24 @@
     def load_md_file(self, md_file: TextIOWrapper) -> None:
         """
         Load a Markdown file from a file-like object.
 
         Args:
             md_file: The file-like object containing the source Markdown content.
         """
-        file_content = md_file.read()
-        parsed = frontmatter.loads(file_content)
-        self.md_meta = parsed.metadata
-        self.md_str = parsed.content
+        self.load_md_str(md_file.read())
 
     def load_md_str(self, md_str: str) -> None:
         """
         Load a Markdown file from a string.
 
         Args:
             md_str: The source Markdown content as a string.
         """
-        self.md_str = md_str
+        self.md_meta, self.md_str = meta_data(md_str)
 
     def load_md(self, md: Union[str, Path, TextIOWrapper]) -> None:
         """
         Load a Markdown file from a string, file path, or file-like object.
 
         Args:
             md: The source Markdown content, can be a string, file path or file-like object.
@@ -131,15 +144,15 @@
         self.md_doc = Document(self.md_str)
         current_level = 0
         current_dict = self.md_dict
         dict_stack = [current_dict]
 
         for child in self.md_doc.children:
             if isinstance(child, block_token.Heading):
-                new_dict = {"size": 0, "children": defaultdict(list)}
+                new_dict = {"gptok_size": 0, "children": defaultdict(list)}
                 if child.level > current_level:
                     current_dict[child.level].append(new_dict)
                     current_dict = new_dict["children"]
                     dict_stack.append(current_dict)
                 else:
                     dict_stack = dict_stack[: child.level]
                     current_dict = dict_stack[-1]
@@ -147,15 +160,18 @@
                     current_dict = new_dict["children"]
                 current_level = child.level
             if isinstance(child, block_token.BlockToken):
                 new_doc = Document([])
                 new_doc.children.append(child)
                 with markdown_renderer.MarkdownRenderer() as renderer:
                     fragment = renderer.render(new_doc)
-                fragment_dict = {"md": fragment, "size": self.gpttok_size(fragment)}
+                fragment_dict = {
+                    "md": fragment,
+                    "gptok_size": self.gpttok_size(fragment),
+                }
                 current_dict[current_level].append(fragment_dict)
 
     def calculate_sizes(self, md_dict: Dict) -> int:
         """
         Recursively calculates the total size of GPT tokens in the provided Markdown dictionary.
 
         Args:
@@ -166,25 +182,25 @@
         """
         total_size = 0
         for key, value in md_dict.items():
             if isinstance(value, list):
                 for item in value:
                     if isinstance(item, dict):
                         if "children" in item:
-                            item["size"] = self.calculate_sizes(item["children"])
-                        if "size" in item:
-                            total_size += item["size"]
+                            item["gptok_size"] = self.calculate_sizes(item["children"])
+                        if "gptok_size" in item:
+                            total_size += item["gptok_size"]
         return total_size
 
     def process_item(
         self,
         item: Dict,
         current_section: List[str],
         current_size: int,
-        md_sections: List[Section],
+        md_sections: List[Dict[str, Union[str, int]]],
     ) -> Tuple[List[str], int]:
         """
         Processes an item in the Markdown dictionary and adds it to the appropriate section.
 
         Args:
             item: The Markdown item to process.
             current_section: The current section being built as a list of strings.
@@ -202,49 +218,51 @@
                     )
         if "md" in item:
             current_section, current_size = self.process_md(
                 item, current_section, current_size, md_sections
             )
         return current_section, current_size
 
-    def prep_section(self, section_text: str, size: int = None) -> Section:
+    def prep_section(
+        self, section_text: str, size: int = None
+    ) -> Dict[str, Union[str, int]]:
         """
         Prepares a section by removing excessive newlines and calculating the section size if not provided.
 
         Args:
             section_text: The Markdown content of the section.
             size: The size of the section in GPT tokens, defaults to None (automatically calculated).
 
         Returns:
             A Section named tuple containing the prepared Markdown content and its size in tokens.
         """
         if not size:
             size = self.gpttok_size(section_text)
-        return Section(RE_NEWLINES.sub("\n\n", section_text), size)
+        return {"md": RE_NEWLINES.sub("\n\n", section_text), "gptok_size": size}
 
     def process_md(
         self,
         item: Dict,
         current_section: List[str],
         current_size: int,
-        md_sections: List[Section],
+        md_sections: List[Dict[str, Union[str, int]]],
     ) -> Tuple[List[str], int]:
         """
         Processes a Markdown item and adds it to the appropriate section.
 
         Args:
             item: The Markdown item to process.
             current_section: The current section being built as a list of strings.
             current_size: The current size of the section in GPT tokens.
             md_sections: The list of sections (named tuples) being built.
 
         Returns:
             A tuple containing the updated current_section and the current_size.
         """
-        if item["size"] > self.gptok_limit:
+        if item["gptok_size"] > self.gptok_limit:
             for syntok_paragraph in syntok_analyze(item["md"]):
                 for syntok_sentence in syntok_paragraph:
                     sentence = (
                         "".join(
                             token.spacing + token.value for token in syntok_sentence
                         ).lstrip()
                         + " "
@@ -252,30 +270,32 @@
                     sentence_size = self.gpttok_size(sentence)
                     if current_size + sentence_size <= self.gptok_limit:
                         current_section.append(sentence)
                         current_size += sentence_size
                     else:
                         md_sections.append(
                             self.prep_section("".join(current_section), current_size)
-)
+                        )
                         current_section = [sentence]
                         current_size = sentence_size
                 current_section.append("\n\n")
-        elif current_size + item["size"] <= self.gptok_limit:
+        elif current_size + item["gptok_size"] <= self.gptok_limit:
             current_section.append(item["md"] + "\n")
-            current_size += item["size"]
+            current_size += item["gptok_size"]
         else:
             md_sections.append(
                 self.prep_section("".join(current_section), current_size)
             )
             current_section = [item["md"] + "\n"]
-            current_size = item["size"]
+            current_size = item["gptok_size"]
         return current_section, current_size
 
-    def get_sections_from_md_dict_by_limit(self, md_dict: Dict) -> List[Section]:
+    def get_sections_from_md_dict_by_limit(
+        self, md_dict: Dict
+    ) -> List[Dict[str, Union[str, int]]]:
         """
         Builds the sections from the provided Markdown dictionary by fitting the content within token limits.
 
         Args:
             md_dict: The Markdown dictionary to build sections from.
 
         Returns:
@@ -316,15 +336,16 @@
         return list(self.gen_section_dicts())
 
     def gen_section_dicts(self) -> Generator[Dict[str, Union[str, int]], None, None]:
         """
         Generator that yields section dictionaries containing the Markdown content and its size.
         """
         return (
-            {"md": section.md, "size": section.size} for section in self.md_sections
+            {"md": section["md"], "gptok_size": section["gptok_size"]}
+            for section in self.md_sections
         )
 
     def list_section_texts(self) -> List[str]:
         """
         Returns a list of section texts containing the Markdown content.
 
         Returns:
@@ -332,15 +353,15 @@
         """
         return list(self.gen_section_texts())
 
     def gen_section_texts(self) -> Generator[str, None, None]:
         """
         Generator that yields the Markdown content of each section.
         """
-        return (section.md for section in self.md_sections)
+        return (section["md"] for section in self.md_sections)
 
     def split(self, md: Union[str, Path, TextIOWrapper]) -> List[str]:
         """
         Splits the loaded Markdown document into sections according to the GPT token size limits.
 
         Args:
             md: The source Markdown content, can be a string, file path or file-like object.
```

### Comparing `split_markdown4gpt-1.0.6/src/split_markdown4gpt.egg-info/PKG-INFO` & `split_markdown4gpt-1.0.7/src/split_markdown4gpt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: split-markdown4gpt
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python tool for splitting large Markdown files into smaller sections based on a specified token limit. This is particularly useful for processing large Markdown files with GPT models, as it allows the models to handle the data in manageable chunks.
 Home-page: https://github.com/twardoch/split-markdown4gpt
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: Apache-2.0
 Project-URL: Documentation, https://twardoch.github.io/split-markdown4gpt/
 Project-URL: Source, https://github.com/twardoch/split-markdown4gpt
@@ -25,15 +25,15 @@
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # split_markdown4gpt
 
 `split_markdown4gpt` is a Python tool designed to split large Markdown files into smaller sections based on a specified token limit. This is particularly useful for processing large Markdown files with GPT models, as it allows the models to handle the data in manageable chunks.
 
-_**Version 1.0.6** (2023-06-18)_
+_**Version 1.0.7** (2023-06-19)_
 
 ## Installation
 
 You can install `split_markdown4gpt` via pip:
 
 ```bash
 pip install split_markdown4gpt
@@ -116,20 +116,26 @@
 - `syntok` for splitting the text into sentences.
 - `regex` and `PyYAML` for various utility functions.
 
 ### Use Cases
 
 `split_markdown4gpt` is particularly useful in scenarios where you need to process large Markdown files with GPT models. For instance:
 
-- **Text Generation**: If you're using a GPT model to generate text based on a large Markdown file, you can use `split_markdown4gpt` to split the file into manageable sections. This allows the GPT model to process the file in chunks, preventing memory overflow errors.
+- **Text Generation**: If you're using a GPT model to generate text based on a large Markdown file, you can use `split_markdown4gpt` to split the file into manageable sections. This allows the GPT model to process the file in chunks, preventing token overflow errors.
 
 - **Data Preprocessing**: In machine learning projects, you often need to preprocess your data before feeding it into your model. If your data is in the form of large Markdown files, `split_markdown4gpt` can help you split these files into smaller sections based on the token limit of your model.
 
 - **Document Analysis**: If you're analyzing large Markdown documents (e.g., extracting keywords, summarizing content), you can use `split_markdown4gpt` to break down the documents into smaller sections. This makes the analysis more manageable and efficient.
 
+## Changelog
+
+- v1.0.7: Switched the model for each section from namedtuple to dict
+- v1.0.6: Fixes
+- v1.0.0: Initial release
+
 ## Contributing
 
 Contributions to `split_markdown4gpt` are welcome! Please open an issue or submit a pull request on the [GitHub repository](https://github.com/twardoch/split-markdown4gpt).
 
 ## License
 
 - Copyright (c) 2023 [Adam Twardoch](./AUTHORS.md)
```

### Comparing `split_markdown4gpt-1.0.6/src/split_markdown4gpt.egg-info/SOURCES.txt` & `split_markdown4gpt-1.0.7/src/split_markdown4gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.6/tests/test.md` & `split_markdown4gpt-1.0.7/tests/test.md`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.6/tox.ini` & `split_markdown4gpt-1.0.7/tox.ini`

 * *Files identical despite different names*

