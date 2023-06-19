# Comparing `tmp/pubmed_sdk-0.2.tar.gz` & `tmp/pubmed_sdk-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pubmed_sdk-0.2.tar", last modified: Mon Jun 19 19:53:28 2023, max compression
+gzip compressed data, was "pubmed_sdk-0.4.tar", last modified: Mon Jun 19 20:14:30 2023, max compression
```

## Comparing `pubmed_sdk-0.2.tar` & `pubmed_sdk-0.4.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-06-19 19:53:28.320922 pubmed_sdk-0.2/
--rw-rw-r--   0 leo       (1000) leo       (1000)     1066 2023-06-16 19:42:39.000000 pubmed_sdk-0.2/LICENSE
--rw-rw-r--   0 leo       (1000) leo       (1000)     2888 2023-06-19 19:53:28.320922 pubmed_sdk-0.2/PKG-INFO
--rw-rw-r--   0 leo       (1000) leo       (1000)     2167 2023-06-19 19:49:37.000000 pubmed_sdk-0.2/README.md
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-06-19 19:53:28.320922 pubmed_sdk-0.2/pubmed_sdk/
--rw-rw-r--   0 leo       (1000) leo       (1000)       25 2023-06-19 19:13:20.000000 pubmed_sdk-0.2/pubmed_sdk/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     3177 2023-06-16 20:01:45.000000 pubmed_sdk-0.2/pubmed_sdk/pubmed_sdk.py
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-06-19 19:53:28.320922 pubmed_sdk-0.2/pubmed_sdk.egg-info/
--rw-rw-r--   0 leo       (1000) leo       (1000)     2888 2023-06-19 19:53:28.000000 pubmed_sdk-0.2/pubmed_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 leo       (1000) leo       (1000)      306 2023-06-19 19:53:28.000000 pubmed_sdk-0.2/pubmed_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 leo       (1000) leo       (1000)        1 2023-06-19 19:53:28.000000 pubmed_sdk-0.2/pubmed_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 leo       (1000) leo       (1000)      112 2023-06-19 19:53:28.000000 pubmed_sdk-0.2/pubmed_sdk.egg-info/requires.txt
--rw-rw-r--   0 leo       (1000) leo       (1000)       11 2023-06-19 19:53:28.000000 pubmed_sdk-0.2/pubmed_sdk.egg-info/top_level.txt
--rw-rw-r--   0 leo       (1000) leo       (1000)       49 2023-06-19 19:19:54.000000 pubmed_sdk-0.2/pyproject.toml
--rw-rw-r--   0 leo       (1000) leo       (1000)      131 2023-06-16 19:53:44.000000 pubmed_sdk-0.2/requirements.txt
--rw-rw-r--   0 leo       (1000) leo       (1000)      157 2023-06-19 19:53:28.320922 pubmed_sdk-0.2/setup.cfg
--rw-rw-r--   0 leo       (1000) leo       (1000)     1122 2023-06-19 19:53:19.000000 pubmed_sdk-0.2/setup.py
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-06-19 19:53:28.320922 pubmed_sdk-0.2/tests/
--rw-rw-r--   0 leo       (1000) leo       (1000)      869 2023-06-19 19:13:03.000000 pubmed_sdk-0.2/tests/test_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:14:30.201240 pubmed_sdk-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 20:14:18.000000 pubmed_sdk-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-19 20:14:30.201240 pubmed_sdk-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-19 20:14:19.000000 pubmed_sdk-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:14:30.197240 pubmed_sdk-0.4/pubmed_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-19 20:14:19.000000 pubmed_sdk-0.4/pubmed_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-19 20:14:19.000000 pubmed_sdk-0.4/pubmed_sdk/pubmed_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:14:30.201240 pubmed_sdk-0.4/pubmed_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-19 20:14:30.000000 pubmed_sdk-0.4/pubmed_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-19 20:14:30.000000 pubmed_sdk-0.4/pubmed_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:14:30.000000 pubmed_sdk-0.4/pubmed_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-19 20:14:30.000000 pubmed_sdk-0.4/pubmed_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-19 20:14:30.000000 pubmed_sdk-0.4/pubmed_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-19 20:14:19.000000 pubmed_sdk-0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-19 20:14:30.201240 pubmed_sdk-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-19 20:14:19.000000 pubmed_sdk-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:14:30.201240 pubmed_sdk-0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-19 20:14:19.000000 pubmed_sdk-0.4/tests/test_search.py
```

### Comparing `pubmed_sdk-0.2/LICENSE` & `pubmed_sdk-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pubmed_sdk-0.2/PKG-INFO` & `pubmed_sdk-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubmed_sdk
-Version: 0.2
+Version: 0.4
 Summary: A Python SDK for searching PubMed using the NCBI E-Utilities
 Home-page: http://github.com/pubmed-ai/pubmed_sdk
 Author: Leo Sternlicht
 Author-email: lsternlicht@gmail.com
 License: MIT
 Keywords: pubmed ncbi e-utilities sdk,pubmed api
 Classifier: License :: OSI Approved :: MIT License
@@ -69,20 +69,20 @@
 
 
 ### Fetch Article Details
 After searching, you can fetch the details of the articles using the fetch_details method:
 
 ```python
 id_list = results['id_list']    # ['33725716', '33725717']
-details = pubmed.fetch_details(id_list)
+details = pubmed.fetch_details(id_list).get('PubmedArticle')
 ```
 
 This method accepts a list of IDs and returns a list of dictionaries containing the details of each article.
 
 Here's an example of how to iterate through the results and print some information about each article:
 
 ```python
 for detail in details:
-    article = detail['PubmedArticle']['MedlineCitation']['Article']
+    article = detail['MedlineCitation']['Article']
     print(article['ArticleTitle'])
-    print(article['Abstract']['AbstractText'][0])
+    print(article['Abstract']['AbstractText'], '\n\n')
 ```
```

### Comparing `pubmed_sdk-0.2/README.md` & `pubmed_sdk-0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,20 +49,20 @@
 
 
 ### Fetch Article Details
 After searching, you can fetch the details of the articles using the fetch_details method:
 
 ```python
 id_list = results['id_list']    # ['33725716', '33725717']
-details = pubmed.fetch_details(id_list)
+details = pubmed.fetch_details(id_list).get('PubmedArticle')
 ```
 
 This method accepts a list of IDs and returns a list of dictionaries containing the details of each article.
 
 Here's an example of how to iterate through the results and print some information about each article:
 
 ```python
 for detail in details:
-    article = detail['PubmedArticle']['MedlineCitation']['Article']
+    article = detail['MedlineCitation']['Article']
     print(article['ArticleTitle'])
-    print(article['Abstract']['AbstractText'][0])
-```
+    print(article['Abstract']['AbstractText'], '\n\n')
+```
```

### Comparing `pubmed_sdk-0.2/pubmed_sdk/pubmed_sdk.py` & `pubmed_sdk-0.4/pubmed_sdk/pubmed_sdk.py`

 * *Files identical despite different names*

### Comparing `pubmed_sdk-0.2/pubmed_sdk.egg-info/PKG-INFO` & `pubmed_sdk-0.4/pubmed_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubmed-sdk
-Version: 0.2
+Version: 0.4
 Summary: A Python SDK for searching PubMed using the NCBI E-Utilities
 Home-page: http://github.com/pubmed-ai/pubmed_sdk
 Author: Leo Sternlicht
 Author-email: lsternlicht@gmail.com
 License: MIT
 Keywords: pubmed ncbi e-utilities sdk,pubmed api
 Classifier: License :: OSI Approved :: MIT License
@@ -69,20 +69,20 @@
 
 
 ### Fetch Article Details
 After searching, you can fetch the details of the articles using the fetch_details method:
 
 ```python
 id_list = results['id_list']    # ['33725716', '33725717']
-details = pubmed.fetch_details(id_list)
+details = pubmed.fetch_details(id_list).get('PubmedArticle')
 ```
 
 This method accepts a list of IDs and returns a list of dictionaries containing the details of each article.
 
 Here's an example of how to iterate through the results and print some information about each article:
 
 ```python
 for detail in details:
-    article = detail['PubmedArticle']['MedlineCitation']['Article']
+    article = detail['MedlineCitation']['Article']
     print(article['ArticleTitle'])
-    print(article['Abstract']['AbstractText'][0])
+    print(article['Abstract']['AbstractText'], '\n\n')
 ```
```

### Comparing `pubmed_sdk-0.2/setup.py` & `pubmed_sdk-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     required = f.read().splitlines()
 
 with open('README.md', 'rt') as f:
     long_description = f.read()
 
 setup(
     name="pubmed_sdk",
-    version="0.2",
+    version="0.4",
     packages=['pubmed_sdk'],
     install_requires=required,
     author="Leo Sternlicht",
     author_email="lsternlicht@gmail.com",
     description="A Python SDK for searching PubMed using the NCBI E-Utilities",
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `pubmed_sdk-0.2/tests/test_search.py` & `pubmed_sdk-0.4/tests/test_search.py`

 * *Files identical despite different names*

