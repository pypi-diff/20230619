# Comparing `tmp/pandasai-0.5.5.tar.gz` & `tmp/pandasai-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.5.5.tar", max compression
+gzip compressed data, was "pandasai-0.6.0.tar", max compression
```

## Comparing `pandasai-0.5.5.tar` & `pandasai-0.6.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     1055 2023-06-16 23:11:12.698732 pandasai-0.5.5/LICENSE
--rw-r--r--   0        0        0     7123 2023-06-16 23:11:12.702732 pandasai-0.5.5/README.md
--rw-r--r--   0        0        0    21016 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/__init__.py
--rw-r--r--   0        0        0     1440 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/constants.py
--rw-r--r--   0        0        0     1509 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3814 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5434 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1742 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1493 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3252 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0        0 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4354 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    10885 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1213 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     1828 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      577 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     1482 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     2932 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      663 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      558 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      653 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      647 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1697 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1262 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1514 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      460 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1343 2023-06-16 23:11:12.706732 pandasai-0.5.5/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1712 2023-06-16 23:11:12.706732 pandasai-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     8225 1970-01-01 00:00:00.000000 pandasai-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-06-18 23:39:45.080769 pandasai-0.6.0/LICENSE
+-rw-r--r--   0        0        0     7705 2023-06-18 23:39:45.080769 pandasai-0.6.0/README.md
+-rw-r--r--   0        0        0    23095 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/__init__.py
+-rw-r--r--   0        0        0     1440 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3814 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5434 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1742 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1493 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3252 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     4369 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0        0 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4354 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    10885 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1213 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     1828 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      577 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     1482 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     2932 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      663 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      558 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      653 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      647 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1697 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1262 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1514 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      460 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1343 2023-06-18 23:39:45.088769 pandasai-0.6.0/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1712 2023-06-18 23:39:45.092769 pandasai-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     8807 1970-01-01 00:00:00.000000 pandasai-0.6.0/PKG-INFO
```

### Comparing `pandasai-0.5.5/LICENSE` & `pandasai-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/README.md` & `pandasai-0.6.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -129,14 +129,34 @@
 
 ```
 Oh, Olivia gets paid the most.
 ```
 
 You can find more examples in the [examples](examples) directory.
 
+### ⚡️ Shortcuts
+
+PandasAI also provides a number of shortcuts (beta) to make it easier to ask questions to your data. For example, you can ask PandasAI to `clean_data`, `impute_missing_values`, `generate_features`, `plot_histogram`, and many many more.
+
+```python
+# Clean data
+pandas_ai.clean_data(df)
+
+# Impute missing values
+pandas_ai.impute_missing_values(df)
+
+# Generate features
+pandas_ai.generate_features(df)
+
+# Plot histogram
+pandas_ai.plot_histogram(df, column="gdp")
+```
+
+Learn more about the shortcuts [here](https://pandas-ai.readthedocs.io/en/latest/shortcuts/).
+
 ## 🔒 Privacy & Security
 
 In order to generate the Python code to run, we take the dataframe head, we randomize it (using random generation for sensitive data and shuffling for non-sensitive data) and send just the head.
 
 Also, if you want to enforce further your privacy you can instantiate PandasAI with `enforce_privacy = True` which will not send the head (but just column names) to the LLM.
 
 ## ⚙️ Command-Line Tool
```

### Comparing `pandasai-0.5.5/pandasai/__init__.py` & `pandasai-0.6.0/pandasai/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 """
 import ast
 import io
 import logging
 import re
 import sys
 import uuid
+import time
 from contextlib import redirect_stdout
 from typing import List, Optional, Union
 
 import astor
 import pandas as pd
 from .constants import (
     WHITELISTED_BUILTINS,
@@ -50,26 +51,27 @@
 )
 from .exceptions import BadImportError, LLMNotFoundError
 from .helpers._optional import import_dependency
 from .helpers.anonymizer import anonymize_dataframe_head
 from .helpers.cache import Cache
 from .helpers.notebook import Notebook
 from .helpers.save_chart import add_save_chart
+from .helpers.shortcuts import Shortcuts
 from .llm.base import LLM
 from .llm.langchain import LangchainLLM
 from .middlewares.base import Middleware
 from .middlewares.charts import ChartsMiddleware
 from .prompts.correct_error_prompt import CorrectErrorPrompt
 from .prompts.correct_multiples_prompt import CorrectMultipleDataframesErrorPrompt
 from .prompts.generate_python_code import GeneratePythonCodePrompt
 from .prompts.generate_response import GenerateResponsePrompt
 from .prompts.multiple_dataframes import MultipleDataframesPrompt
 
 
-class PandasAI:
+class PandasAI(Shortcuts):
     """
     PandasAI is a wrapper around a LLM to make dataframes conversational.
 
 
     This is an entry point of `pandasai` object. This class consists of methods
     to interface the LLMs with Pandas     dataframes. A pandas dataframe metadata i.e.
     df.head() and prompt is passed on to chosen LLMs API end point to generate a Python
@@ -87,14 +89,23 @@
         _enforce_privacy (bool, optional): Do not display the data on prompt in case of
         Sensitive data. Default to False
         _max_retries (int, optional): max no. of tries to generate code on failure.
         Default to 3
         _is_notebook (bool, optional): Whether to run code in notebook. Default to False
         _original_instructions (dict, optional): The dict of instruction to run. Default
         to None
+        _cache (Cache, optional): Cache object to store the results. Default to None
+        _enable_cache (bool, optional): Whether to enable cache. Default to True
+        _prompt_id (str, optional): Unique ID to differentiate calls. Default to None
+        _middlewares (List[Middleware], optional): List of middlewares to run. Default
+        to [ChartsMiddleware()]
+        _additional_dependencies (List[dict], optional): List of additional dependencies
+        to be added. Default to []
+        _custom_whitelisted_dependencies (List[str], optional): List of custom
+        whitelisted dependencies. Default to []
         last_code_generated (str, optional): Pass last Code if generated. Default to
         None
         last_code_executed (str, optional): Pass the last execution / run. Default to
         None
         code_output (str, optional): The code output if any. Default to None
         last_error (str, optional): Error of running code last time. Default to None
         prompt_id (str, optional): Unique ID to differentiate calls. Default to None
@@ -118,14 +129,15 @@
     }
     _cache: Cache = None
     _enable_cache: bool = True
     _prompt_id: Optional[str] = None
     _middlewares: List[Middleware] = [ChartsMiddleware()]
     _additional_dependencies: List[dict] = []
     _custom_whitelisted_dependencies: List[str] = []
+    _start_time: float = 0
     last_code_generated: Optional[str] = None
     last_code_executed: Optional[str] = None
     code_output: Optional[str] = None
     last_error: Optional[str] = None
 
     def __init__(
         self,
@@ -260,14 +272,16 @@
             use_error_correction_framework (bool): Turn on Error Correction mechanism.
             Default to True
 
         Returns (str): Answer to the Input Questions about the DataFrame
 
         """
 
+        self._start_time = time.time()
+
         self.log(f"Running PandasAI with {self._llm.type} LLM...")
 
         self._prompt_id = str(uuid.uuid4())
         self.log(f"Prompt ID: {self._prompt_id}")
 
         try:
             if self._enable_cache and self._cache and self._cache.get(prompt):
@@ -346,14 +360,17 @@
             self.log(f"Answer: {answer}")
 
             if is_conversational_answer is None:
                 is_conversational_answer = self._is_conversational_answer
             if is_conversational_answer:
                 answer = self.conversational_answer(prompt, answer)
                 self.log(f"Conversational answer: {answer}")
+
+            self.log(f"Executed in: {time.time() - self._start_time}s")
+
             return answer
         except Exception as exception:
             self.last_error = str(exception)
             print(exception)
             return (
                 "Unfortunately, I was not able to answer your question, "
                 "because of the following error:\n"
@@ -487,14 +504,66 @@
             if self._is_df_overwrite(node):
                 continue
             new_body.append(node)
 
         new_tree = ast.Module(body=new_body)
         return astor.to_source(new_tree).strip()
 
+    def _get_environment(self) -> dict:
+        """
+        Returns the environment for the code to be executed.
+
+        Returns (dict): A dictionary of environment variables
+        """
+
+        return {
+            "pd": pd,
+            **{
+                lib["alias"]: getattr(import_dependency(lib["module"]), lib["name"])
+                if hasattr(import_dependency(lib["module"]), lib["name"])
+                else import_dependency(lib["module"])
+                for lib in self._additional_dependencies
+            },
+            "__builtins__": {
+                **{builtin: __builtins__[builtin] for builtin in WHITELISTED_BUILTINS},
+            },
+        }
+
+    def _retry_run_code(self, code: str, e: Exception, multiple: bool = False):
+        """
+        A method to retry the code execution with error correction framework.
+
+        Args:
+            code (str): A python code
+            e (Exception): An exception
+            multiple (bool): A boolean to indicate if the code is for multiple
+            dataframes
+
+        Returns (str): A python code
+        """
+
+        if multiple:
+            error_correcting_instruction = CorrectMultipleDataframesErrorPrompt(
+                code=code,
+                error_returned=e,
+                question=self._original_instructions["question"],
+                df_head=self._original_instructions["df_head"],
+            )
+        else:
+            error_correcting_instruction = CorrectErrorPrompt(
+                code=code,
+                error_returned=e,
+                question=self._original_instructions["question"],
+                df_head=self._original_instructions["df_head"],
+                num_rows=self._original_instructions["num_rows"],
+                num_columns=self._original_instructions["num_columns"],
+            )
+
+        return self._llm.generate_code(error_correcting_instruction, "")
+
     def run_code(
         self,
         code: str,
         data_frame: pd.DataFrame,
         use_error_correction_framework: bool = True,
     ) -> str:
         """
@@ -525,32 +594,20 @@
             f"""
 Code running:
 ```
 {code_to_run}
 ```"""
         )
 
-        environment: dict = {
-            "pd": pd,
-            **{
-                lib["alias"]: getattr(import_dependency(lib["module"]), lib["name"])
-                if hasattr(import_dependency(lib["module"]), lib["name"])
-                else import_dependency(lib["module"])
-                for lib in self._additional_dependencies
-            },
-            "__builtins__": {
-                **{builtin: __builtins__[builtin] for builtin in WHITELISTED_BUILTINS},
-            },
-        }
+        environment: dict = self._get_environment()
 
         if multiple:
             environment.update(
                 {f"df{i}": dataframe for i, dataframe in enumerate(data_frame, start=1)}
             )
-
         else:
             environment["df"] = data_frame
 
         # Redirect standard output to a StringIO buffer
         with redirect_stdout(io.StringIO()) as output:
             count = 0
             while count < self._max_retries:
@@ -561,50 +618,41 @@
                     break
                 except Exception as e:
                     if not use_error_correction_framework:
                         raise e
 
                     count += 1
 
-                    if multiple:
-                        error_correcting_instruction = (
-                            CorrectMultipleDataframesErrorPrompt(
-                                code=code,
-                                error_returned=e,
-                                question=self._original_instructions["question"],
-                                df_head=self._original_instructions["df_head"],
-                            )
-                        )
-
-                    else:
-                        error_correcting_instruction = CorrectErrorPrompt(
-                            code=code,
-                            error_returned=e,
-                            question=self._original_instructions["question"],
-                            df_head=self._original_instructions["df_head"],
-                            num_rows=self._original_instructions["num_rows"],
-                            num_columns=self._original_instructions["num_columns"],
-                        )
+                    code_to_run = self._retry_run_code(code, e, multiple)
 
-                    code_to_run = self._llm.generate_code(
-                        error_correcting_instruction, ""
-                    )
-
-        captured_output = output.getvalue()
+        captured_output = output.getvalue().strip()
+        if len(captured_output.split("\n")) > 1:
+            return captured_output
 
         # Evaluate the last line and return its value or the captured output
+        # We do this because we want to return the right value and the right
+        # type of the value. For example, if the last line is `df.head()`, we
+        # want to return the head of the dataframe, not the captured output.
         lines = code.strip().split("\n")
         last_line = lines[-1].strip()
 
         match = re.match(r"^print\((.*)\)$", last_line)
         if match:
             last_line = match.group(1)
 
         try:
-            return eval(last_line, environment)
+            result = eval(last_line, environment)
+
+            # In some cases, the result is a tuple of values. For example, when
+            # the last line is `print("Hello", "World")`, the result is a tuple
+            # of two strings. In this case, we want to return a string
+            if isinstance(result, tuple):
+                result = " ".join([str(element) for element in result])
+
+            return result
         except Exception:
             return captured_output
 
     def log(self, message: str):
         """Log a message"""
         self._logger.info(message)
 
@@ -613,7 +661,13 @@
         return self._process_id
 
     def last_prompt_id(self) -> str:
         """Return the id of the last prompt that was run."""
         if self._prompt_id is None:
             raise ValueError("Pandas AI has not been run yet.")
         return self._prompt_id
+
+    @property
+    def last_prompt(self) -> str:
+        """Return the last prompt that was executed."""
+        if self._llm:
+            return self._llm.last_prompt
```

### Comparing `pandasai-0.5.5/pandasai/constants.py` & `pandasai-0.6.0/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/exceptions.py` & `pandasai-0.6.0/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/helpers/_optional.py` & `pandasai-0.6.0/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/helpers/anonymizer.py` & `pandasai-0.6.0/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/helpers/cache.py` & `pandasai-0.6.0/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/helpers/from_excel.py` & `pandasai-0.6.0/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/helpers/notebook.py` & `pandasai-0.6.0/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/helpers/save_chart.py` & `pandasai-0.6.0/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/llm/azure_openai.py` & `pandasai-0.6.0/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/llm/base.py` & `pandasai-0.6.0/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/llm/fake.py` & `pandasai-0.6.0/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/llm/falcon.py` & `pandasai-0.6.0/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/llm/google_palm.py` & `pandasai-0.6.0/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/llm/langchain.py` & `pandasai-0.6.0/pandasai/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/llm/open_assistant.py` & `pandasai-0.6.0/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/llm/openai.py` & `pandasai-0.6.0/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/llm/starcoder.py` & `pandasai-0.6.0/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/middlewares/base.py` & `pandasai-0.6.0/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/middlewares/charts.py` & `pandasai-0.6.0/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/middlewares/streamlit.py` & `pandasai-0.6.0/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/prompts/base.py` & `pandasai-0.6.0/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/prompts/correct_error_prompt.py` & `pandasai-0.6.0/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/prompts/correct_multiples_prompt.py` & `pandasai-0.6.0/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/prompts/generate_python_code.py` & `pandasai-0.6.0/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pandasai/prompts/multiple_dataframes.py` & `pandasai-0.6.0/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.5/pyproject.toml` & `pandasai-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.5.5"
+version = "0.6.0"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pandasai-0.5.5/PKG-INFO` & `pandasai-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.5.5
+Version: 0.6.0
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -154,14 +154,34 @@
 
 ```
 Oh, Olivia gets paid the most.
 ```
 
 You can find more examples in the [examples](examples) directory.
 
+### ⚡️ Shortcuts
+
+PandasAI also provides a number of shortcuts (beta) to make it easier to ask questions to your data. For example, you can ask PandasAI to `clean_data`, `impute_missing_values`, `generate_features`, `plot_histogram`, and many many more.
+
+```python
+# Clean data
+pandas_ai.clean_data(df)
+
+# Impute missing values
+pandas_ai.impute_missing_values(df)
+
+# Generate features
+pandas_ai.generate_features(df)
+
+# Plot histogram
+pandas_ai.plot_histogram(df, column="gdp")
+```
+
+Learn more about the shortcuts [here](https://pandas-ai.readthedocs.io/en/latest/shortcuts/).
+
 ## 🔒 Privacy & Security
 
 In order to generate the Python code to run, we take the dataframe head, we randomize it (using random generation for sensitive data and shuffling for non-sensitive data) and send just the head.
 
 Also, if you want to enforce further your privacy you can instantiate PandasAI with `enforce_privacy = True` which will not send the head (but just column names) to the LLM.
 
 ## ⚙️ Command-Line Tool
```

