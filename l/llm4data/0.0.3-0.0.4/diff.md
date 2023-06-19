# Comparing `tmp/llm4data-0.0.3.tar.gz` & `tmp/llm4data-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm4data-0.0.3.tar", max compression
+gzip compressed data, was "llm4data-0.0.4.tar", max compression
```

## Comparing `llm4data-0.0.3.tar` & `llm4data-0.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    30757 2023-05-26 17:27:00.950549 llm4data-0.0.3/LICENSE
--rw-r--r--   0        0        0     9149 2023-06-05 20:17:16.274426 llm4data-0.0.3/README.md
--rw-r--r--   0        0        0      289 2023-06-19 04:29:36.913046 llm4data-0.0.3/llm4data/__init__.py
--rw-r--r--   0        0        0     3172 2023-06-15 20:16:00.899057 llm4data-0.0.3/llm4data/configs.py
--rw-r--r--   0        0        0      243 2023-05-31 23:34:02.046957 llm4data-0.0.3/llm4data/embeddings/__init__.py
--rw-r--r--   0        0        0     3186 2023-06-15 20:16:00.899273 llm4data-0.0.3/llm4data/embeddings/base.py
--rw-r--r--   0        0        0      566 2023-06-15 20:16:00.899473 llm4data-0.0.3/llm4data/embeddings/docs.py
--rw-r--r--   0        0        0      834 2023-06-15 20:16:00.899679 llm4data-0.0.3/llm4data/embeddings/indicators.py
--rw-r--r--   0        0        0      841 2023-06-15 20:16:00.899898 llm4data-0.0.3/llm4data/embeddings/microdata.py
--rw-r--r--   0        0        0      170 2023-06-15 20:16:00.900058 llm4data-0.0.3/llm4data/index/__init__.py
--rw-r--r--   0        0        0     2680 2023-06-15 20:16:00.900299 llm4data-0.0.3/llm4data/index/qdrant.py
--rw-r--r--   0        0        0     5838 2023-06-19 04:14:57.702274 llm4data-0.0.3/llm4data/llm/indicators/wdi_sql.py
--rw-r--r--   0        0        0        0 2023-05-26 16:41:36.283163 llm4data-0.0.3/llm4data/llm/microdata/.gitkeep
--rw-r--r--   0        0        0     1780 2023-06-15 20:16:00.900797 llm4data-0.0.3/llm4data/prompts/base.py
--rw-r--r--   0        0        0     2945 2023-06-18 23:29:06.835846 llm4data-0.0.3/llm4data/prompts/context.py
--rw-r--r--   0        0        0     1663 2023-05-27 17:39:37.424246 llm4data-0.0.3/llm4data/prompts/indicators/templates.py
--rw-r--r--   0        0        0     5065 2023-06-19 04:14:57.702708 llm4data-0.0.3/llm4data/prompts/indicators/wdi.py
--rw-r--r--   0        0        0        0 2023-05-26 16:40:23.801226 llm4data-0.0.3/llm4data/prompts/microdata/.gitkeep
--rw-r--r--   0        0        0      352 2023-05-26 19:58:54.433048 llm4data-0.0.3/llm4data/prompts/utils.py
--rw-r--r--   0        0        0     1030 2023-06-18 23:29:06.836040 llm4data-0.0.3/llm4data/schema/docs/migrate_wbdocs_metadata.py
--rw-r--r--   0        0        0    24359 2023-06-15 20:16:00.901481 llm4data-0.0.3/llm4data/schema/docs/wbdocs.py
--rw-r--r--   0        0        0     1647 2023-06-18 23:29:06.836205 llm4data-0.0.3/llm4data/schema/indicators/create_wdi_text.py
--rw-r--r--   0        0        0     1130 2023-06-18 23:29:06.836396 llm4data-0.0.3/llm4data/schema/schema2info.py
--rw-r--r--   0        0        0        0 2023-06-15 20:16:00.901705 llm4data-0.0.3/llm4data/scripts/__init__.py
--rw-r--r--   0        0        0     1572 2023-06-19 04:14:57.702920 llm4data-0.0.3/llm4data/scripts/indexing/create_field_index.py
--rw-r--r--   0        0        0     1684 2023-06-16 04:24:21.755270 llm4data-0.0.3/llm4data/scripts/indexing/docs/docs.py
--rw-r--r--   0        0        0     3518 2023-06-15 20:16:00.902507 llm4data-0.0.3/llm4data/scripts/indexing/docs/load_docs.py
--rw-r--r--   0        0        0      944 2023-06-18 23:29:06.836656 llm4data-0.0.3/llm4data/scripts/indexing/indicators/indicators.py
--rw-r--r--   0        0        0     2789 2023-06-19 04:14:57.703168 llm4data-0.0.3/llm4data/scripts/indexing/indicators/load_indicators.py
--rw-r--r--   0        0        0     3146 2023-05-27 00:12:24.551761 llm4data-0.0.3/llm4data/sources/indicators/wdi.py
--rw-r--r--   0        0        0        0 2023-05-26 16:41:22.772734 llm4data-0.0.3/llm4data/sources/microdata/.gitkeep
--rw-r--r--   0        0        0   117888 2023-05-24 15:43:46.011357 llm4data-0.0.3/llm4data/wdi2name.json
--rw-r--r--   0        0        0     1353 2023-06-19 04:29:36.903585 llm4data-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    10419 1970-01-01 00:00:00.000000 llm4data-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    30757 2023-05-26 17:27:00.950549 llm4data-0.0.4/LICENSE
+-rw-r--r--   0        0        0     9149 2023-06-05 20:17:16.274426 llm4data-0.0.4/README.md
+-rw-r--r--   0        0        0      289 2023-06-19 20:15:26.275295 llm4data-0.0.4/llm4data/__init__.py
+-rw-r--r--   0        0        0     3172 2023-06-15 20:16:00.899057 llm4data-0.0.4/llm4data/configs.py
+-rw-r--r--   0        0        0      243 2023-05-31 23:34:02.046957 llm4data-0.0.4/llm4data/embeddings/__init__.py
+-rw-r--r--   0        0        0     3186 2023-06-15 20:16:00.899273 llm4data-0.0.4/llm4data/embeddings/base.py
+-rw-r--r--   0        0        0      566 2023-06-15 20:16:00.899473 llm4data-0.0.4/llm4data/embeddings/docs.py
+-rw-r--r--   0        0        0      834 2023-06-15 20:16:00.899679 llm4data-0.0.4/llm4data/embeddings/indicators.py
+-rw-r--r--   0        0        0      841 2023-06-15 20:16:00.899898 llm4data-0.0.4/llm4data/embeddings/microdata.py
+-rw-r--r--   0        0        0      170 2023-06-15 20:16:00.900058 llm4data-0.0.4/llm4data/index/__init__.py
+-rw-r--r--   0        0        0     2680 2023-06-15 20:16:00.900299 llm4data-0.0.4/llm4data/index/qdrant.py
+-rw-r--r--   0        0        0     5838 2023-06-19 04:14:57.702274 llm4data-0.0.4/llm4data/llm/indicators/wdi_sql.py
+-rw-r--r--   0        0        0        0 2023-05-26 16:41:36.283163 llm4data-0.0.4/llm4data/llm/microdata/.gitkeep
+-rw-r--r--   0        0        0     1780 2023-06-15 20:16:00.900797 llm4data-0.0.4/llm4data/prompts/base.py
+-rw-r--r--   0        0        0     2945 2023-06-18 23:29:06.835846 llm4data-0.0.4/llm4data/prompts/context.py
+-rw-r--r--   0        0        0     1663 2023-05-27 17:39:37.424246 llm4data-0.0.4/llm4data/prompts/indicators/templates.py
+-rw-r--r--   0        0        0     5231 2023-06-19 20:13:55.508781 llm4data-0.0.4/llm4data/prompts/indicators/wdi.py
+-rw-r--r--   0        0        0        0 2023-05-26 16:40:23.801226 llm4data-0.0.4/llm4data/prompts/microdata/.gitkeep
+-rw-r--r--   0        0        0      352 2023-05-26 19:58:54.433048 llm4data-0.0.4/llm4data/prompts/utils.py
+-rw-r--r--   0        0        0     1030 2023-06-18 23:29:06.836040 llm4data-0.0.4/llm4data/schema/docs/migrate_wbdocs_metadata.py
+-rw-r--r--   0        0        0    24359 2023-06-15 20:16:00.901481 llm4data-0.0.4/llm4data/schema/docs/wbdocs.py
+-rw-r--r--   0        0        0     1647 2023-06-18 23:29:06.836205 llm4data-0.0.4/llm4data/schema/indicators/create_wdi_text.py
+-rw-r--r--   0        0        0     1130 2023-06-18 23:29:06.836396 llm4data-0.0.4/llm4data/schema/schema2info.py
+-rw-r--r--   0        0        0        0 2023-06-15 20:16:00.901705 llm4data-0.0.4/llm4data/scripts/__init__.py
+-rw-r--r--   0        0        0     1572 2023-06-19 04:14:57.702920 llm4data-0.0.4/llm4data/scripts/indexing/create_field_index.py
+-rw-r--r--   0        0        0     1684 2023-06-16 04:24:21.755270 llm4data-0.0.4/llm4data/scripts/indexing/docs/docs.py
+-rw-r--r--   0        0        0     3518 2023-06-15 20:16:00.902507 llm4data-0.0.4/llm4data/scripts/indexing/docs/load_docs.py
+-rw-r--r--   0        0        0      944 2023-06-18 23:29:06.836656 llm4data-0.0.4/llm4data/scripts/indexing/indicators/indicators.py
+-rw-r--r--   0        0        0     2789 2023-06-19 04:14:57.703168 llm4data-0.0.4/llm4data/scripts/indexing/indicators/load_indicators.py
+-rw-r--r--   0        0        0     3146 2023-05-27 00:12:24.551761 llm4data-0.0.4/llm4data/sources/indicators/wdi.py
+-rw-r--r--   0        0        0        0 2023-05-26 16:41:22.772734 llm4data-0.0.4/llm4data/sources/microdata/.gitkeep
+-rw-r--r--   0        0        0   117888 2023-05-24 15:43:46.011357 llm4data-0.0.4/llm4data/wdi2name.json
+-rw-r--r--   0        0        0     1353 2023-06-19 20:15:26.267232 llm4data-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    10419 1970-01-01 00:00:00.000000 llm4data-0.0.4/PKG-INFO
```

### Comparing `llm4data-0.0.3/LICENSE` & `llm4data-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/README.md` & `llm4data-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/llm4data/configs.py` & `llm4data-0.0.4/llm4data/configs.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/llm4data/embeddings/base.py` & `llm4data-0.0.4/llm4data/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/llm4data/embeddings/docs.py` & `llm4data-0.0.4/llm4data/embeddings/docs.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/llm4data/embeddings/indicators.py` & `llm4data-0.0.4/llm4data/embeddings/indicators.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/llm4data/embeddings/microdata.py` & `llm4data-0.0.4/llm4data/embeddings/microdata.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/llm4data/index/qdrant.py` & `llm4data-0.0.4/llm4data/index/qdrant.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/llm4data/llm/indicators/wdi_sql.py` & `llm4data-0.0.4/llm4data/llm/indicators/wdi_sql.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/llm4data/prompts/base.py` & `llm4data-0.0.4/llm4data/prompts/base.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/llm4data/prompts/context.py` & `llm4data-0.0.4/llm4data/prompts/context.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/llm4data/prompts/indicators/templates.py` & `llm4data-0.0.4/llm4data/prompts/indicators/templates.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/llm4data/prompts/indicators/wdi.py` & `llm4data-0.0.4/llm4data/prompts/indicators/wdi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import json
 import requests
 import pandas as pd
 from typing import Any
 from urllib.parse import urlparse
 from openai_tools.parser import parse_misparsed
 from llm4data.prompts.base import DatedPrompt, APIPrompt
+from llm4data import configs
 
 
 class WDISQLPrompt(DatedPrompt):
     task_label = "WDISQLPrompt"
 
     def __init__(self, input_variables=None, template=None):
         if template is None and input_variables is None:
             input_variables = ["now", "table", "fields"]
             template = (
                 "Current date: {now}\n\n"
                 "I have a database containing data from the WDI indicators."
                 " Write an SQL query for the prompt: ```{{{{user_content}}}}```\n\n"
                 "table: {table}\n"
-                "fields: {fields}\n\n"
-                "Only the indicator can parameterized and you must fill the rest."
+                "fields: {fields}\n"
+                f"dialect: {configs.WDIDBConfig.engine}\n\n"
+                "Pay attention to the dialect when writing the query.\n\n"
+                "Only the indicator can be parameterized and you must fill the rest."
                 " Use the convention `:indicator` and not `?`."
                 " Use country_iso3 when querying, use country in the result.\n\n"
                 "Use the last 10 years if no year is specified."
                 " Drop rows with no value.\n\n"
                 "Return the entire row if useful for the prompt."
                 " If it will help in the analysis and if it makes sense, always add the year in the `SELECT` clause if it is not already there.\n\n"
                 """Return the output as JSON for json.loads: {{"query_string": <SQL>}}"""
```

### Comparing `llm4data-0.0.3/llm4data/schema/docs/migrate_wbdocs_metadata.py` & `llm4data-0.0.4/llm4data/schema/docs/migrate_wbdocs_metadata.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/llm4data/schema/docs/wbdocs.py` & `llm4data-0.0.4/llm4data/schema/docs/wbdocs.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/llm4data/schema/indicators/create_wdi_text.py` & `llm4data-0.0.4/llm4data/schema/indicators/create_wdi_text.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/llm4data/schema/schema2info.py` & `llm4data-0.0.4/llm4data/schema/schema2info.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/llm4data/scripts/indexing/create_field_index.py` & `llm4data-0.0.4/llm4data/scripts/indexing/create_field_index.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/llm4data/scripts/indexing/docs/docs.py` & `llm4data-0.0.4/llm4data/scripts/indexing/docs/docs.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/llm4data/scripts/indexing/docs/load_docs.py` & `llm4data-0.0.4/llm4data/scripts/indexing/docs/load_docs.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/llm4data/scripts/indexing/indicators/indicators.py` & `llm4data-0.0.4/llm4data/scripts/indexing/indicators/indicators.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/llm4data/scripts/indexing/indicators/load_indicators.py` & `llm4data-0.0.4/llm4data/scripts/indexing/indicators/load_indicators.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/llm4data/sources/indicators/wdi.py` & `llm4data-0.0.4/llm4data/sources/indicators/wdi.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/llm4data/wdi2name.json` & `llm4data-0.0.4/llm4data/wdi2name.json`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.3/pyproject.toml` & `llm4data-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm4data"
-version = "0.0.3"
+version = "0.0.4"
 description = "LLM4Data is a Python library designed to facilitate the application of large language models (LLMs) and artificial intelligence for development data and knowledge discovery."
 authors = ["Aivin V. Solatorio <avsolatorio@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2.0.1"
```

### Comparing `llm4data-0.0.3/PKG-INFO` & `llm4data-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4data
-Version: 0.0.3
+Version: 0.0.4
 Summary: LLM4Data is a Python library designed to facilitate the application of large language models (LLMs) and artificial intelligence for development data and knowledge discovery.
 Author: Aivin V. Solatorio
 Author-email: avsolatorio@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

