# Comparing `tmp/spark_llm-0.1.3.tar.gz` & `tmp/spark_llm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_llm-0.1.3.tar", max compression
+gzip compressed data, was "spark_llm-0.1.4.tar", max compression
```

## Comparing `spark_llm-0.1.3.tar` & `spark_llm-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 spark_llm-0.1.3/LICENSE
--rw-r--r--   0        0        0     1847 2023-06-10 06:58:48.977364 spark_llm-0.1.3/README.md
--rw-r--r--   0        0        0      903 2023-06-10 07:02:10.271109 spark_llm-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      131 2023-06-09 17:49:03.120504 spark_llm-0.1.3/spark_llm/__init__.py
--rw-r--r--   0        0        0     5272 2023-06-09 17:49:03.119511 spark_llm-0.1.3/spark_llm/prompt.py
--rw-r--r--   0        0        0     9146 2023-06-10 06:14:57.409593 spark_llm-0.1.3/spark_llm/spark_llm_assistant.py
--rw-r--r--   0        0        0     2993 1970-01-01 00:00:00.000000 spark_llm-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 spark_llm-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2328 2023-06-19 20:17:51.380866 spark_llm-0.1.4/README.md
+-rw-r--r--   0        0        0      926 2023-06-19 20:19:09.082658 spark_llm-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      131 2023-06-09 17:49:03.120504 spark_llm-0.1.4/spark_llm/__init__.py
+-rw-r--r--   0        0        0     2668 2023-06-16 21:50:36.340803 spark_llm-0.1.4/spark_llm/cache.py
+-rw-r--r--   0        0        0     1093 2023-06-16 21:50:36.341090 spark_llm-0.1.4/spark_llm/llm_chain_with_cache.py
+-rw-r--r--   0        0        0     3023 2023-06-19 20:17:59.831335 spark_llm-0.1.4/spark_llm/llm_utils.py
+-rw-r--r--   0        0        0     6900 2023-06-19 20:17:59.833736 spark_llm-0.1.4/spark_llm/prompt.py
+-rw-r--r--   0        0        0      688 2023-06-16 21:50:36.342058 spark_llm-0.1.4/spark_llm/search_tool_with_cache.py
+-rw-r--r--   0        0        0    12623 2023-06-19 20:17:59.879989 spark_llm-0.1.4/spark_llm/spark_llm_assistant.py
+-rw-r--r--   0        0        0     3492 1970-01-01 00:00:00.000000 spark_llm-0.1.4/PKG-INFO
```

### Comparing `spark_llm-0.1.3/LICENSE` & `spark_llm-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.3/README.md` & `spark_llm-0.1.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -26,31 +26,48 @@
 |------|-----------|---------------|----------------------|
 | 1    | Toyota    | 1849751       | -9                   |
 | 2    | Ford      | 1767439       | -2                   |
 | 3    | Chevrolet | 1502389       | 6                    |
 | 4    | Honda     | 881201        | -33                  |
 | 5    | Hyundai   | 724265        | -2                   |
 
+### Plot
+```python
+auto_df.llm.plot()
+```
+![2022 USA national auto sales by brand](docs/_static/auto_sales.png)
+
+To plot with an instruction:
+```python
+auto_df.llm.plot("pie char for top 5 brands and the others' market shares")
+```
+![2022 USA national auto sales_market_share by brand](docs/_static/auto_sales_pie_char.png)
 ### DataFrame Transformation
 ```python
-auto_top_growth_df=auto_df.llm_transform("top brand with the highest growth")
+auto_top_growth_df=auto_df.llm.transform("top brand with the highest growth")
 auto_top_growth_df.show()
 ```
 | brand    | us_sales_2022 | sales_change_vs_2021 |
 |----------|---------------|----------------------|
 | Cadillac | 134726        | 14                   |
 
 ### DataFrame Explanation
 ```python
-auto_top_growth_df.llm_explain()
+auto_top_growth_df.llm.explain()
 ```
 
 > In summary, this dataframe is retrieving the brand with the highest sales change in 2022 compared to 2021. It presents the results sorted by sales change in descending order and only returns the top result.
 
 Refer to [example.ipynb](https://github.com/gengliangwang/spark-llm/blob/main/examples/example.ipynb) for more detailed usage examples.
 
+### DataFrame Attribute Verification
+```python
+auto_top_growth_df.llm.verify("expect sales change percentage to be between -100 to 100")
+```
+
+> result: True
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 Licensed under the Apache License 2.0.
```

### Comparing `spark_llm-0.1.3/pyproject.toml` & `spark_llm-0.1.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "spark-llm"
-version = "0.1.3"
+version = "0.1.4"
 description = "LLM assistant for the development of Spark applications"
 authors = ["Gengliang Wang <gengliang@apache.org>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/gengliangwang/spark-llm"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-requests = "*"
-tiktoken = "*"
-beautifulsoup4 = "*"
-langchain = "*"
-pyspark = "*"
+python = "^3.8.1"
+requests = "^2.31.0"
+tiktoken = "0.4.0"
+beautifulsoup4 = "^4.12.2"
+pyspark = "^3.4.0"
+openai = "^0.27.8"
+langchain = "^0.0.201"
+pandas = "^2.0.2"
+
 
 [tool.poetry.dev-dependencies]
```

### Comparing `spark_llm-0.1.3/spark_llm/prompt.py` & `spark_llm-0.1.4/spark_llm/prompt.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 I got the following answer from a web page:
 ```
 {web_content}
 ```
 Now help me write a SQL query to store the answer into a temp view.
 Here is an example of how to store data into a temp view:
 ```
-CREATE OR REPLACE TEMP VIEW movies AS SELECT * FROM VALUES(('Citizen Kane', 1941), ('Schindler\'s List', 1993)) AS v1(title, year)
+CREATE OR REPLACE TEMP VIEW movies AS SELECT * FROM VALUES('Citizen Kane', 1941), ('Schindler\'s List', 1993) AS v1(title, year)
 ```
 {columns}
 The answer MUST contain query only.
 """
 
 SQL_PROMPT = PromptTemplate(
     input_variables=["query", "web_content", "columns"], template=SQL_TEMPLATE
@@ -110,7 +110,60 @@
     examples=_explain_examples,
     example_prompt=_example_prompt,
     prefix=EXPLAIN_PREFIX,
     suffix=EXPLAIN_SUFFIX,
     input_variables=["input"],
     example_separator="\n\n",
 )
+
+PLOT_PROMPT_TEMPLATE = """
+Given a pyspark dataframe `df`.
+The output columns of `df`:
+{columns}
+
+{explain}
+
+Now help me write python code to visualize the result of `df` using plotly:
+1. All the code MUST be in one code block.
+2. There is no need to install any package with pip.
+3. Show the plot directly, instead of saving into a HTML.
+{instruction}
+"""
+
+PLOT_PROMPT = PromptTemplate(
+    input_variables=["columns", "explain", "instruction"], template=PLOT_PROMPT_TEMPLATE
+)
+
+VERIFY_TEMPLATE = """
+Given 1) a PySpark dataframe, df, and 2) a description of expected properties, desc,
+generate a Python function to test whether the given dataframe satisfies the expected properties.
+Your generated function should take 1 parameter, df, and the return type should be a boolean.
+You will call the function, passing in df as the parameter, and return the output (True/False).
+
+In total, your output must follow the format below, exactly (no explanation words):
+1. function definition f, in Python
+2. 1 blank new line
+3. Call f on df and assign the result to a variable, result: result = name_of_f(df)
+
+For example:
+Input:
+df = DataFrame[name: string, age: int]
+desc = "expect 5 columns"
+
+Output:
+"def has_5_columns(df) -> bool:
+    # Get the number of columns in the DataFrame
+    num_columns = len(df.columns)
+
+    # Check if the number of columns is equal to 5
+    if num_columns == 5:
+        return True
+    else:
+        return False
+
+result = has_5_columns(df)"
+
+Here is your input df: {df}
+Here is your input description: {desc}
+"""
+
+VERIFY_PROMPT = PromptTemplate(input_variables=["df", "desc"], template=VERIFY_TEMPLATE)
```

### Comparing `spark_llm-0.1.3/spark_llm/spark_llm_assistant.py` & `spark_llm-0.1.4/spark_llm/spark_llm_assistant.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 import re
-from functools import partial
+import types
+from functools import partialmethod
 from typing import Callable, Optional, List
 from urllib.parse import urlparse
 
 import requests
 import tiktoken
 from bs4 import BeautifulSoup
-from langchain import LLMChain, GoogleSearchAPIWrapper
+from langchain import LLMChain, GoogleSearchAPIWrapper, BasePromptTemplate
 from langchain.base_language import BaseLanguageModel
 from pyspark.sql import SparkSession, DataFrame
 from tiktoken import Encoding
 
+from spark_llm.cache import Cache
+from spark_llm.llm_chain_with_cache import LLMChainWithCache
 from spark_llm.prompt import (
     SEARCH_PROMPT,
     SQL_PROMPT,
     EXPLAIN_DF_PROMPT,
     TRANSFORM_PROMPT,
+    PLOT_PROMPT,
+    VERIFY_PROMPT,
 )
+from spark_llm.search_tool_with_cache import SearchToolWithCache
+from spark_llm.llm_utils import LLMUtils
 
 
 class SparkLLMAssistant:
     _HTTP_HEADER = {
         "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36"
         " (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36",
         "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
@@ -28,14 +35,15 @@
     }
 
     def __init__(
         self,
         llm: BaseLanguageModel,
         web_search_tool: Optional[Callable[[str], str]] = None,
         spark_session: Optional[SparkSession] = None,
+        enable_cache: bool = True,
         encoding: Optional[Encoding] = None,
         max_tokens_of_web_content: int = 3000,
         verbose: bool = False,
     ) -> None:
         """
         Initialize the SparkLLMAssistant object with the provided parameters.
 
@@ -46,22 +54,37 @@
         :param spark_session: optional SparkSession, a new one will be created if not provided
         :param encoding: optional Encoding, cl100k_base will be used if not provided
         :param max_tokens_of_web_content: maximum tokens of web content after encoding
         """
         self._spark = spark_session or SparkSession.builder.getOrCreate()
         self._llm = llm
         self._web_search_tool = web_search_tool or self._default_web_search_tool
+        if enable_cache:
+            self._cache = Cache()
+            self._web_search_tool = SearchToolWithCache(
+                self._web_search_tool, self._cache
+            ).search
+        else:
+            self._cache = None
         self._encoding = encoding or tiktoken.get_encoding("cl100k_base")
         self._max_tokens_of_web_content = max_tokens_of_web_content
-        self._search_llm_chain = LLMChain(llm=self._llm, prompt=SEARCH_PROMPT)
-        self._sql_llm_chain = LLMChain(llm=self._llm, prompt=SQL_PROMPT)
-        self._explain_chain = LLMChain(llm=llm, prompt=EXPLAIN_DF_PROMPT)
-        self._transform_chain = LLMChain(llm=llm, prompt=TRANSFORM_PROMPT)
+        self._search_llm_chain = self._create_llm_chain(prompt=SEARCH_PROMPT)
+        self._sql_llm_chain = self._create_llm_chain(prompt=SQL_PROMPT)
+        self._explain_chain = self._create_llm_chain(prompt=EXPLAIN_DF_PROMPT)
+        self._transform_chain = self._create_llm_chain(prompt=TRANSFORM_PROMPT)
+        self._plot_chain = self._create_llm_chain(prompt=PLOT_PROMPT)
+        self._verify_chain = self._create_llm_chain(prompt=VERIFY_PROMPT)
         self._verbose = verbose
 
+    def _create_llm_chain(self, prompt: BasePromptTemplate):
+        if self._cache is None:
+            return LLMChain(llm=self._llm, prompt=prompt)
+
+        return LLMChainWithCache(llm=self._llm, prompt=prompt, cache=self._cache)
+
     @staticmethod
     def _extract_view_name(query: str) -> str:
         """
         Extract the view name from the provided SQL query.
 
         :param query: SQL query as a string
         :return: view name as a string
@@ -98,14 +121,33 @@
 
     @staticmethod
     def _is_http_or_https_url(s: str):
         result = urlparse(s)  # Parse the URL
         # Check if the scheme is 'http' or 'https'
         return result.scheme in ["http", "https"]
 
+    @staticmethod
+    def _extract_code_blocks(text) -> List[str]:
+        code_block_pattern = re.compile(r"```(.*?)```", re.DOTALL)
+        code_blocks = re.findall(code_block_pattern, text)
+        if code_blocks:
+            # If there are code blocks, strip them and remove language specifiers.
+            extracted_blocks = []
+            for block in code_blocks:
+                block = block.strip()
+                if block.startswith("python"):
+                    block = block.replace("python\n", "", 1)
+                elif block.startswith("sql"):
+                    block = block.replace("sql\n", "", 1)
+                extracted_blocks.append(block)
+            return extracted_blocks
+        else:
+            # If there are no code blocks, treat the whole text as a single block of code.
+            return [text]
+
     def log(self, message: str) -> None:
         if self._verbose:
             print(message)
 
     def _trim_text_from_end(self, text: str, max_tokens: int) -> str:
         """
         Trim text from the end based on the maximum number of tokens allowed.
@@ -134,24 +176,42 @@
         web_content = self._trim_text_from_end(
             clean_text, self._max_tokens_of_web_content
         )
 
         sql_columns_hint = self._generate_sql_prompt(columns)
 
         # Run the LLM chain to get an ingestion SQL query
-        sql_query = self._sql_llm_chain.run(
+        llm_result = self._sql_llm_chain.run(
             query=desc, web_content=web_content, columns=sql_columns_hint
         )
+        sql_query = self._extract_code_blocks(llm_result)[0]
         self.log(f"SQL query for the ingestion:\n {sql_query}\n")
 
         view_name = self._extract_view_name(sql_query)
         self.log(f"Storing data into temp view: {view_name}\n")
         self._spark.sql(sql_query)
         return self._spark.table(view_name)
 
+    def _get_df_schema(self, df: DataFrame) -> str:
+        return "\n".join([f"{name}: {dtype}" for name, dtype in df.dtypes])
+
+    @staticmethod
+    def _trim_hash_id(analyzed_plan):
+        # Pattern to find strings like #59 or #2021
+        pattern = r"#\d+"
+
+        # Remove matching patterns
+        trimmed_plan = re.sub(pattern, "", analyzed_plan)
+
+        return trimmed_plan
+
+    def _get_df_explain(self, df: DataFrame) -> str:
+        raw_analyzed_str = df._jdf.queryExecution().analyzed().toString()
+        return self._explain_chain.run(input=self._trim_hash_id(raw_analyzed_str))
+
     def create_df(self, desc: str, columns: Optional[List[str]] = None) -> DataFrame:
         """
         Create a Spark DataFrame by querying an LLM from web search result.
 
         :param desc: the description of the result DataFrame, which will be used for
                      web searching
         :param columns: the expected column names in the result DataFrame
@@ -187,38 +247,71 @@
         :param df: The Spark DataFrame that is to be transformed.
         :param desc: A natural language string that outlines the specific transformation to be applied on the DataFrame.
 
         :return: Returns a new Spark DataFrame that is the result of applying the specified transformation on the input DataFrame.
         """
         temp_view_name = "temp_view_for_transform"
         df.createOrReplaceTempView(temp_view_name)
-        schema_str = "\n".join([f"{name}: {dtype}" for name, dtype in df.dtypes])
-        sql_query = self._transform_chain.run(
+        schema_str = self._get_df_schema(df)
+        llm_result = self._transform_chain.run(
             view_name=temp_view_name, columns=schema_str, desc=desc
         )
+        sql_query = self._extract_code_blocks(llm_result)[0]
         self.log(f"SQL query for the transform:\n{sql_query}")
         return self._spark.sql(sql_query)
 
     def explain_df(self, df: DataFrame) -> str:
         """
         This method generates a natural language explanation of the SQL plan of the input Spark DataFrame.
 
         :param df: The Spark DataFrame to be explained.
 
         :return: A string explanation of the DataFrame's SQL plan, detailing what the DataFrame is intended to retrieve.
         """
-        explain_result = self._explain_chain.run(
-            df._jdf.queryExecution().analyzed().toString()
-        )
+        explain_result = self._get_df_explain(df)
         # If there is code block in the explain result, ignore it.
         if "```" in explain_result:
             summary = explain_result.split("```")[-1]
             return summary.strip()
         else:
             return explain_result
 
+    def plot_df(self, df: DataFrame, desc: Optional[str] = None) -> None:
+        instruction = f"The purpose of the plot: {desc}" if desc is not None else ""
+        response = self._plot_chain.run(
+            columns=self._get_df_schema(df),
+            explain=self._get_df_explain(df),
+            instruction=instruction,
+        )
+        self.log(response)
+        codeblocks = self._extract_code_blocks(response)
+        for code in codeblocks:
+            exec(code)
+
+    def verify_df(self, df: DataFrame, desc: str) -> None:
+        """
+        This method creates and runs test cases for the provided PySpark dataframe transformation function.
+
+        :param df: The Spark DataFrame to be verified
+        :param desc: A description of the expectation to be verified
+        """
+        llm_output = self._verify_chain.run(df=df, desc=desc)
+
+        self.log(f"Generated code:\n{llm_output}")
+
+        locals_ = {}
+        exec(llm_output, {"df": df}, locals_)
+
+        self.log(f"\nResult: {locals_['result']}")
+
     def activate(self):
         """
         Activates LLM utility functions for Spark DataFrame.
         """
-        DataFrame.llm_transform = lambda df_instance, desc: self.transform_df(df_instance, desc)
-        DataFrame.llm_explain = lambda df_instance: self.explain_df(df_instance)
+        DataFrame.llm = LLMUtils(self)
+
+    def commit(self):
+        """
+        Commit the staging in-memory cache into persistent cache, if cache is enabled.
+        """
+        if self._cache is not None:
+            self._cache.commit()
```

### Comparing `spark_llm-0.1.3/PKG-INFO` & `spark_llm-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: spark-llm
-Version: 0.1.3
+Version: 0.1.4
 Summary: LLM assistant for the development of Spark applications
 Home-page: https://github.com/gengliangwang/spark-llm
 License: Apache-2.0
 Author: Gengliang Wang
 Author-email: gengliang@apache.org
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: beautifulsoup4
-Requires-Dist: langchain
-Requires-Dist: pyspark
-Requires-Dist: requests
-Requires-Dist: tiktoken
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: langchain (>=0.0.201,<0.0.202)
+Requires-Dist: openai (>=0.27.8,<0.28.0)
+Requires-Dist: pandas (>=2.0.2,<3.0.0)
+Requires-Dist: pyspark (>=3.4.0,<4.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: tiktoken (==0.4.0)
 Description-Content-Type: text/markdown
 
 # LLM Assistant for Apache Spark
 
 ## Installation
 
 ```bash
@@ -56,32 +55,49 @@
 |------|-----------|---------------|----------------------|
 | 1    | Toyota    | 1849751       | -9                   |
 | 2    | Ford      | 1767439       | -2                   |
 | 3    | Chevrolet | 1502389       | 6                    |
 | 4    | Honda     | 881201        | -33                  |
 | 5    | Hyundai   | 724265        | -2                   |
 
+### Plot
+```python
+auto_df.llm.plot()
+```
+![2022 USA national auto sales by brand](docs/_static/auto_sales.png)
+
+To plot with an instruction:
+```python
+auto_df.llm.plot("pie char for top 5 brands and the others' market shares")
+```
+![2022 USA national auto sales_market_share by brand](docs/_static/auto_sales_pie_char.png)
 ### DataFrame Transformation
 ```python
-auto_top_growth_df=auto_df.llm_transform("top brand with the highest growth")
+auto_top_growth_df=auto_df.llm.transform("top brand with the highest growth")
 auto_top_growth_df.show()
 ```
 | brand    | us_sales_2022 | sales_change_vs_2021 |
 |----------|---------------|----------------------|
 | Cadillac | 134726        | 14                   |
 
 ### DataFrame Explanation
 ```python
-auto_top_growth_df.llm_explain()
+auto_top_growth_df.llm.explain()
 ```
 
 > In summary, this dataframe is retrieving the brand with the highest sales change in 2022 compared to 2021. It presents the results sorted by sales change in descending order and only returns the top result.
 
 Refer to [example.ipynb](https://github.com/gengliangwang/spark-llm/blob/main/examples/example.ipynb) for more detailed usage examples.
 
+### DataFrame Attribute Verification
+```python
+auto_top_growth_df.llm.verify("expect sales change percentage to be between -100 to 100")
+```
+
+> result: True
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 Licensed under the Apache License 2.0.
```

