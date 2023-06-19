# Comparing `tmp/split_markdown4gpt-1.0.7.tar.gz` & `tmp/split_markdown4gpt-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "split_markdown4gpt-1.0.7.tar", last modified: Mon Jun 19 17:31:42 2023, max compression
+gzip compressed data, was "split_markdown4gpt-1.0.8.tar", last modified: Mon Jun 19 18:11:59 2023, max compression
```

## Comparing `split_markdown4gpt-1.0.7.tar` & `split_markdown4gpt-1.0.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:31:42.810658 split_markdown4gpt-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:31:42.806658 split_markdown4gpt-1.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:31:42.810658 split_markdown4gpt-1.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/API.md
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-19 17:31:42.810658 split_markdown4gpt-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/pydoc-markdown.yml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-19 17:31:42.814658 split_markdown4gpt-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:31:42.806658 split_markdown4gpt-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:31:42.810658 split_markdown4gpt-1.0.7/src/split_markdown4gpt/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/src/split_markdown4gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/src/split_markdown4gpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14635 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/src/split_markdown4gpt/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:31:42.810658 split_markdown4gpt-1.0.7/src/split_markdown4gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-19 17:31:42.000000 split_markdown4gpt-1.0.7/src/split_markdown4gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-19 17:31:42.000000 split_markdown4gpt-1.0.7/src/split_markdown4gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 17:31:42.000000 split_markdown4gpt-1.0.7/src/split_markdown4gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-19 17:31:42.000000 split_markdown4gpt-1.0.7/src/split_markdown4gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 17:31:42.000000 split_markdown4gpt-1.0.7/src/split_markdown4gpt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-19 17:31:42.000000 split_markdown4gpt-1.0.7/src/split_markdown4gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 17:31:42.000000 split_markdown4gpt-1.0.7/src/split_markdown4gpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:31:42.810658 split_markdown4gpt-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/tests/test.md
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/tests/test_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-19 17:31:27.000000 split_markdown4gpt-1.0.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:11:59.701735 split_markdown4gpt-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-19 18:11:47.000000 split_markdown4gpt-1.0.8/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-19 18:11:47.000000 split_markdown4gpt-1.0.8/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:11:59.697735 split_markdown4gpt-1.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:11:59.701735 split_markdown4gpt-1.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-19 18:11:47.000000 split_markdown4gpt-1.0.8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-19 18:11:47.000000 split_markdown4gpt-1.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-19 18:11:47.000000 split_markdown4gpt-1.0.8/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-19 18:11:47.000000 split_markdown4gpt-1.0.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-06-19 18:11:47.000000 split_markdown4gpt-1.0.8/API.md
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-19 18:11:47.000000 split_markdown4gpt-1.0.8/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 18:11:47.000000 split_markdown4gpt-1.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-19 18:11:59.701735 split_markdown4gpt-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-06-19 18:11:47.000000 split_markdown4gpt-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-19 18:11:47.000000 split_markdown4gpt-1.0.8/pydoc-markdown.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-19 18:11:47.000000 split_markdown4gpt-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-19 18:11:59.705735 split_markdown4gpt-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-19 18:11:47.000000 split_markdown4gpt-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:11:59.697735 split_markdown4gpt-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:11:59.701735 split_markdown4gpt-1.0.8/src/split_markdown4gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-19 18:11:47.000000 split_markdown4gpt-1.0.8/src/split_markdown4gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-19 18:11:47.000000 split_markdown4gpt-1.0.8/src/split_markdown4gpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14635 2023-06-19 18:11:47.000000 split_markdown4gpt-1.0.8/src/split_markdown4gpt/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:11:59.701735 split_markdown4gpt-1.0.8/src/split_markdown4gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-19 18:11:59.000000 split_markdown4gpt-1.0.8/src/split_markdown4gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-19 18:11:59.000000 split_markdown4gpt-1.0.8/src/split_markdown4gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 18:11:59.000000 split_markdown4gpt-1.0.8/src/split_markdown4gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-19 18:11:59.000000 split_markdown4gpt-1.0.8/src/split_markdown4gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 18:11:59.000000 split_markdown4gpt-1.0.8/src/split_markdown4gpt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-19 18:11:59.000000 split_markdown4gpt-1.0.8/src/split_markdown4gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 18:11:59.000000 split_markdown4gpt-1.0.8/src/split_markdown4gpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:11:59.701735 split_markdown4gpt-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-19 18:11:47.000000 split_markdown4gpt-1.0.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-19 18:11:47.000000 split_markdown4gpt-1.0.8/tests/test.md
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-19 18:11:47.000000 split_markdown4gpt-1.0.8/tests/test_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-19 18:11:47.000000 split_markdown4gpt-1.0.8/tox.ini
```

### Comparing `split_markdown4gpt-1.0.7/.DS_Store` & `split_markdown4gpt-1.0.8/.DS_Store`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.7/.coveragerc` & `split_markdown4gpt-1.0.8/.coveragerc`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.7/.github/workflows/ci.yml` & `split_markdown4gpt-1.0.8/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -37,28 +37,30 @@
         run: pytest
 
   update-docs:
     needs: test
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
+        with:
+          ref: ${{ github.head_ref }}
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
           python-version: '3.10'
       - name: Install pydoc-markdown
         run: pip install pydoc-markdown
       - name: Generate API documentation
         run: pydoc-markdown > API.md
       - name: Commit and push if it's changed
         uses: EndBug/add-and-commit@v9
         with:
           message: 'Update API documentation'
           add: 'API.md'
-      
+
   build-and-publish:
     needs: test
     runs-on: ubuntu-latest
     if: startsWith(github.ref, 'refs/tags/')
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python
@@ -72,9 +74,7 @@
       - name: Build distribution
         run: python -m build
       - name: Publish to PyPi
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
-
-
```

### Comparing `split_markdown4gpt-1.0.7/.gitignore` & `split_markdown4gpt-1.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.7/.pre-commit-config.yaml` & `split_markdown4gpt-1.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.7/API.md` & `split_markdown4gpt-1.0.8/API.md`

 * *Files 4% similar despite different names*

```diff
@@ -126,16 +126,18 @@
     The total number of GPT tokens in the Markdown dictionary.
 
 <a id="split_markdown4gpt.splitter.MarkdownLLMSplitter.process_item"></a>
 
 #### process\_item
 
 ```python
-def process_item(item: Dict, current_section: List[str], current_size: int,
-                 md_sections: List[Section]) -> Tuple[List[str], int]
+def process_item(
+        item: Dict, current_section: List[str], current_size: int,
+        md_sections: List[Dict[str, Union[str,
+                                          int]]]) -> Tuple[List[str], int]
 ```
 
 Processes an item in the Markdown dictionary and adds it to the appropriate section.
 
 Args:
     item: The Markdown item to process.
     current_section: The current section being built as a list of strings.
@@ -146,15 +148,16 @@
     A tuple containing the updated current_section and the current_size.
 
 <a id="split_markdown4gpt.splitter.MarkdownLLMSplitter.prep_section"></a>
 
 #### prep\_section
 
 ```python
-def prep_section(section_text: str, size: int = None) -> Section
+def prep_section(section_text: str,
+                 size: int = None) -> Dict[str, Union[str, int]]
 ```
 
 Prepares a section by removing excessive newlines and calculating the section size if not provided.
 
 Args:
     section_text: The Markdown content of the section.
     size: The size of the section in GPT tokens, defaults to None (automatically calculated).
@@ -163,16 +166,18 @@
     A Section named tuple containing the prepared Markdown content and its size in tokens.
 
 <a id="split_markdown4gpt.splitter.MarkdownLLMSplitter.process_md"></a>
 
 #### process\_md
 
 ```python
-def process_md(item: Dict, current_section: List[str], current_size: int,
-               md_sections: List[Section]) -> Tuple[List[str], int]
+def process_md(
+        item: Dict, current_section: List[str], current_size: int,
+        md_sections: List[Dict[str, Union[str,
+                                          int]]]) -> Tuple[List[str], int]
 ```
 
 Processes a Markdown item and adds it to the appropriate section.
 
 Args:
     item: The Markdown item to process.
     current_section: The current section being built as a list of strings.
@@ -183,15 +188,16 @@
     A tuple containing the updated current_section and the current_size.
 
 <a id="split_markdown4gpt.splitter.MarkdownLLMSplitter.get_sections_from_md_dict_by_limit"></a>
 
 #### get\_sections\_from\_md\_dict\_by\_limit
 
 ```python
-def get_sections_from_md_dict_by_limit(md_dict: Dict) -> List[Section]
+def get_sections_from_md_dict_by_limit(
+        md_dict: Dict) -> List[Dict[str, Union[str, int]]]
 ```
 
 Builds the sections from the provided Markdown dictionary by fitting the content within token limits.
 
 Args:
     md_dict: The Markdown dictionary to build sections from.
```

### Comparing `split_markdown4gpt-1.0.7/LICENSE.txt` & `split_markdown4gpt-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.7/PKG-INFO` & `split_markdown4gpt-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: split_markdown4gpt
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python tool for splitting large Markdown files into smaller sections based on a specified token limit. This is particularly useful for processing large Markdown files with GPT models, as it allows the models to handle the data in manageable chunks.
 Home-page: https://github.com/twardoch/split-markdown4gpt
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: Apache-2.0
 Project-URL: Documentation, https://twardoch.github.io/split-markdown4gpt/
 Project-URL: Source, https://github.com/twardoch/split-markdown4gpt
```

### Comparing `split_markdown4gpt-1.0.7/README.md` & `split_markdown4gpt-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.7/setup.cfg` & `split_markdown4gpt-1.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.7/setup.py` & `split_markdown4gpt-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.7/src/split_markdown4gpt/__init__.py` & `split_markdown4gpt-1.0.8/src/split_markdown4gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.7/src/split_markdown4gpt/__main__.py` & `split_markdown4gpt-1.0.8/src/split_markdown4gpt/__main__.py`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.7/src/split_markdown4gpt/splitter.py` & `split_markdown4gpt-1.0.8/src/split_markdown4gpt/splitter.py`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.7/src/split_markdown4gpt.egg-info/PKG-INFO` & `split_markdown4gpt-1.0.8/src/split_markdown4gpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: split-markdown4gpt
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python tool for splitting large Markdown files into smaller sections based on a specified token limit. This is particularly useful for processing large Markdown files with GPT models, as it allows the models to handle the data in manageable chunks.
 Home-page: https://github.com/twardoch/split-markdown4gpt
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: Apache-2.0
 Project-URL: Documentation, https://twardoch.github.io/split-markdown4gpt/
 Project-URL: Source, https://github.com/twardoch/split-markdown4gpt
```

### Comparing `split_markdown4gpt-1.0.7/src/split_markdown4gpt.egg-info/SOURCES.txt` & `split_markdown4gpt-1.0.8/src/split_markdown4gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.7/tests/test.md` & `split_markdown4gpt-1.0.8/tests/test.md`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.7/tox.ini` & `split_markdown4gpt-1.0.8/tox.ini`

 * *Files identical despite different names*

