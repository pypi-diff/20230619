# Comparing `tmp/pandasai-0.6.0.tar.gz` & `tmp/pandasai-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.6.0.tar", max compression
+gzip compressed data, was "pandasai-0.6.1.tar", max compression
```

## Comparing `pandasai-0.6.0.tar` & `pandasai-0.6.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1055 2023-06-18 23:39:45.080769 pandasai-0.6.0/LICENSE
--rw-r--r--   0        0        0     7705 2023-06-18 23:39:45.080769 pandasai-0.6.0/README.md
--rw-r--r--   0        0        0    23095 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/__init__.py
--rw-r--r--   0        0        0     1440 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/constants.py
--rw-r--r--   0        0        0     1509 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3814 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5434 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1742 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1493 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3252 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     4369 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0        0 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4354 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    10885 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1213 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     1828 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      577 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     1482 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     2932 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      663 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      558 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      653 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      647 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1697 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1262 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1514 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      460 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1343 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1712 2023-06-18 23:39:45.092769 pandasai-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     8807 1970-01-01 00:00:00.000000 pandasai-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-06-19 08:52:18.570412 pandasai-0.6.1/LICENSE
+-rw-r--r--   0        0        0     7705 2023-06-19 08:52:18.574412 pandasai-0.6.1/README.md
+-rw-r--r--   0        0        0    23083 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/__init__.py
+-rw-r--r--   0        0        0     1440 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3814 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5434 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1742 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1493 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3252 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     4369 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0        0 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4354 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    10885 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1213 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     1828 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      577 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     1482 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     2932 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      663 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      558 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      653 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      647 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1697 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1262 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1514 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      460 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1343 2023-06-19 08:52:18.578413 pandasai-0.6.1/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1712 2023-06-19 08:52:18.582413 pandasai-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     8807 1970-01-01 00:00:00.000000 pandasai-0.6.1/PKG-INFO
```

### Comparing `pandasai-0.6.0/LICENSE` & `pandasai-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/README.md` & `pandasai-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/__init__.py` & `pandasai-0.6.1/pandasai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -621,15 +621,15 @@
                         raise e
 
                     count += 1
 
                     code_to_run = self._retry_run_code(code, e, multiple)
 
         captured_output = output.getvalue().strip()
-        if len(captured_output.split("\n")) > 1:
+        if code.count("print(") > 1:
             return captured_output
 
         # Evaluate the last line and return its value or the captured output
         # We do this because we want to return the right value and the right
         # type of the value. For example, if the last line is `df.head()`, we
         # want to return the head of the dataframe, not the captured output.
         lines = code.strip().split("\n")
```

### Comparing `pandasai-0.6.0/pandasai/constants.py` & `pandasai-0.6.1/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/exceptions.py` & `pandasai-0.6.1/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/helpers/_optional.py` & `pandasai-0.6.1/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/helpers/anonymizer.py` & `pandasai-0.6.1/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/helpers/cache.py` & `pandasai-0.6.1/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/helpers/from_excel.py` & `pandasai-0.6.1/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/helpers/notebook.py` & `pandasai-0.6.1/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/helpers/save_chart.py` & `pandasai-0.6.1/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/helpers/shortcuts.py` & `pandasai-0.6.1/pandasai/helpers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/llm/azure_openai.py` & `pandasai-0.6.1/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/llm/base.py` & `pandasai-0.6.1/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/llm/fake.py` & `pandasai-0.6.1/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/llm/falcon.py` & `pandasai-0.6.1/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/llm/google_palm.py` & `pandasai-0.6.1/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/llm/langchain.py` & `pandasai-0.6.1/pandasai/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/llm/open_assistant.py` & `pandasai-0.6.1/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/llm/openai.py` & `pandasai-0.6.1/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/llm/starcoder.py` & `pandasai-0.6.1/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/middlewares/base.py` & `pandasai-0.6.1/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/middlewares/charts.py` & `pandasai-0.6.1/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/middlewares/streamlit.py` & `pandasai-0.6.1/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/prompts/base.py` & `pandasai-0.6.1/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/prompts/correct_error_prompt.py` & `pandasai-0.6.1/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/prompts/correct_multiples_prompt.py` & `pandasai-0.6.1/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/prompts/generate_python_code.py` & `pandasai-0.6.1/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pandasai/prompts/multiple_dataframes.py` & `pandasai-0.6.1/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.0/pyproject.toml` & `pandasai-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.6.0"
+version = "0.6.1"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pandasai-0.6.0/PKG-INFO` & `pandasai-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.6.0
+Version: 0.6.1
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

