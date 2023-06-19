# Comparing `tmp/datawise-0.0.8.tar.gz` & `tmp/datawise-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawise-0.0.8.tar", max compression
+gzip compressed data, was "datawise-0.0.9.tar", max compression
```

## Comparing `datawise-0.0.8.tar` & `datawise-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.8/LICENSE
--rw-r--r--   0        0        0     4758 2023-06-18 13:38:57.109053 datawise-0.0.8/README.md
--rw-r--r--   0        0        0     3134 2023-06-18 13:40:56.003231 datawise-0.0.8/datawise/__init__.py
--rw-r--r--   0        0        0      481 2023-06-18 12:46:33.125357 datawise-0.0.8/datawise/exceptions.py
--rw-r--r--   0        0        0      517 2023-06-18 13:40:29.606498 datawise-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5284 1970-01-01 00:00:00.000000 datawise-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.9/LICENSE
+-rw-r--r--   0        0        0     5134 2023-06-19 01:15:55.058801 datawise-0.0.9/README.md
+-rw-r--r--   0        0        0     3134 2023-06-18 13:40:56.003231 datawise-0.0.9/datawise/__init__.py
+-rw-r--r--   0        0        0      481 2023-06-18 12:46:33.125357 datawise-0.0.9/datawise/exceptions.py
+-rw-r--r--   0        0        0      517 2023-06-19 01:16:13.723533 datawise-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5660 1970-01-01 00:00:00.000000 datawise-0.0.9/PKG-INFO
```

### Comparing `datawise-0.0.8/LICENSE` & `datawise-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `datawise-0.0.8/README.md` & `datawise-0.0.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -37,24 +37,24 @@
 countries = pd.DataFrame({
     "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
     "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
     "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
 })
 
 datawise = dw.DataWise(api_key="you_api_key_here")
-df = datawise.sql("SELECT COUNT(country) AS NumCountry FROM countries", {
+df = datawise.sql("SELECT COUNT(country) FROM countries", {
   "countries": countries
 }, code=True) # "code=True" will print out the code in addition to transforming dataframe.
 print(df)
 ```
 
 The above code will return the following dataframe:
 
 ```
-   NumCountry
+   count
 0          10
 ```
 
 You can also do joins of multiple dataframes:
 ```python
 import datawise as dw
 import pandas as pd
@@ -89,14 +89,21 @@
 5           Spain   1181205135360             6.40           6
 6          Canada   1607402389504             7.23           7
 7       Australia   1490967855104             7.22           8
 8           Japan   4380756541440             5.87           9
 9           China  14631844184064             5.12          10
 ```
 
+## Limitations
+Most of SQLite syntax of SELECT statements are supported.
+Here are some of the limitations at this moment:
+* We don't support Window functions at the moment: https://www.sqlite.org/windowfunctions.html
+* If your query contains WHERE clause with `LIKE` operator, we might not be able to translate it properly.
+* We might not be able to translate SQL query properly from time to time.
+
 ## Error Handling
 Errors could happen if we cannot translate the SQL query. Consider the following example:
 ```python
 import datawise as dw
 import pandas as pd
 
 countries = pd.DataFrame({
@@ -127,15 +134,15 @@
 poetry install
 poetry run pytest tests/tests.py -s
 
 pip install --upgrade build
 rm -rf dist && python -m build
 
 pip install --upgrade twine
-twine upload --repository pypitest dist/*
+twine upload --repository pypi dist/*
 ```
 
 ## 📜 License
 
 DataWise is licensed under the Apache 2.0 License. See the LICENSE file for more details.
 
 ## Acknowledgements
```

### Comparing `datawise-0.0.8/datawise/__init__.py` & `datawise-0.0.9/datawise/__init__.py`

 * *Files identical despite different names*

### Comparing `datawise-0.0.8/pyproject.toml` & `datawise-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datawise"
-version = "0.0.8"
+version = "0.0.9"
 description = "Testing"
 authors = ["DataWise Team"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 python-dotenv = "^1.0.0"
```

### Comparing `datawise-0.0.8/PKG-INFO` & `datawise-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawise
-Version: 0.0.8
+Version: 0.0.9
 Summary: Testing
 Author: DataWise Team
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -53,24 +53,24 @@
 countries = pd.DataFrame({
     "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
     "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
     "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
 })
 
 datawise = dw.DataWise(api_key="you_api_key_here")
-df = datawise.sql("SELECT COUNT(country) AS NumCountry FROM countries", {
+df = datawise.sql("SELECT COUNT(country) FROM countries", {
   "countries": countries
 }, code=True) # "code=True" will print out the code in addition to transforming dataframe.
 print(df)
 ```
 
 The above code will return the following dataframe:
 
 ```
-   NumCountry
+   count
 0          10
 ```
 
 You can also do joins of multiple dataframes:
 ```python
 import datawise as dw
 import pandas as pd
@@ -105,14 +105,21 @@
 5           Spain   1181205135360             6.40           6
 6          Canada   1607402389504             7.23           7
 7       Australia   1490967855104             7.22           8
 8           Japan   4380756541440             5.87           9
 9           China  14631844184064             5.12          10
 ```
 
+## Limitations
+Most of SQLite syntax of SELECT statements are supported.
+Here are some of the limitations at this moment:
+* We don't support Window functions at the moment: https://www.sqlite.org/windowfunctions.html
+* If your query contains WHERE clause with `LIKE` operator, we might not be able to translate it properly.
+* We might not be able to translate SQL query properly from time to time.
+
 ## Error Handling
 Errors could happen if we cannot translate the SQL query. Consider the following example:
 ```python
 import datawise as dw
 import pandas as pd
 
 countries = pd.DataFrame({
@@ -143,15 +150,15 @@
 poetry install
 poetry run pytest tests/tests.py -s
 
 pip install --upgrade build
 rm -rf dist && python -m build
 
 pip install --upgrade twine
-twine upload --repository pypitest dist/*
+twine upload --repository pypi dist/*
 ```
 
 ## 📜 License
 
 DataWise is licensed under the Apache 2.0 License. See the LICENSE file for more details.
 
 ## Acknowledgements
```

