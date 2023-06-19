# Comparing `tmp/drukarnia-api-0.1.61.tar.gz` & `tmp/drukarnia-api-0.1.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drukarnia-api-0.1.61.tar", last modified: Fri Jun  2 06:09:08 2023, max compression
+gzip compressed data, was "drukarnia-api-0.1.75.tar", last modified: Mon Jun 19 10:08:14 2023, max compression
```

## Comparing `drukarnia-api-0.1.61.tar` & `drukarnia-api-0.1.75.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 andrej5    (501) staff       (20)        0 2023-06-02 06:09:08.035804 drukarnia-api-0.1.61/
--rw-r--r--   0 andrej5    (501) staff       (20)     1063 2023-06-02 04:09:32.000000 drukarnia-api-0.1.61/LICENSE
--rw-r--r--   0 andrej5    (501) staff       (20)     1956 2023-06-02 06:09:08.035388 drukarnia-api-0.1.61/PKG-INFO
--rw-r--r--   0 andrej5    (501) staff       (20)     1273 2023-06-02 06:08:31.000000 drukarnia-api-0.1.61/README.md
-drwxr-xr-x   0 andrej5    (501) staff       (20)        0 2023-06-02 06:09:08.029048 drukarnia-api-0.1.61/drukarnia_api/
--rw-r--r--   0 andrej5    (501) staff       (20)      100 2023-06-02 06:07:38.000000 drukarnia-api-0.1.61/drukarnia_api/__init__.py
--rw-r--r--   0 andrej5    (501) staff       (20)      569 2023-06-02 06:07:38.000000 drukarnia-api-0.1.61/drukarnia_api/article.py
--rw-r--r--   0 andrej5    (501) staff       (20)     3264 2023-06-02 06:07:38.000000 drukarnia-api-0.1.61/drukarnia_api/author.py
--rw-r--r--   0 andrej5    (501) staff       (20)      680 2023-06-02 04:04:41.000000 drukarnia-api-0.1.61/drukarnia_api/connection.py
--rw-r--r--   0 andrej5    (501) staff       (20)      890 2023-06-02 06:07:38.000000 drukarnia-api-0.1.61/drukarnia_api/drukarnia_api.py
-drwxr-xr-x   0 andrej5    (501) staff       (20)        0 2023-06-02 06:09:08.033807 drukarnia-api-0.1.61/drukarnia_api.egg-info/
--rw-r--r--   0 andrej5    (501) staff       (20)     1956 2023-06-02 06:09:07.000000 drukarnia-api-0.1.61/drukarnia_api.egg-info/PKG-INFO
--rw-r--r--   0 andrej5    (501) staff       (20)      344 2023-06-02 06:09:07.000000 drukarnia-api-0.1.61/drukarnia_api.egg-info/SOURCES.txt
--rw-r--r--   0 andrej5    (501) staff       (20)        1 2023-06-02 06:09:07.000000 drukarnia-api-0.1.61/drukarnia_api.egg-info/dependency_links.txt
--rw-r--r--   0 andrej5    (501) staff       (20)      213 2023-06-02 06:09:07.000000 drukarnia-api-0.1.61/drukarnia_api.egg-info/requires.txt
--rw-r--r--   0 andrej5    (501) staff       (20)       14 2023-06-02 06:09:07.000000 drukarnia-api-0.1.61/drukarnia_api.egg-info/top_level.txt
--rw-r--r--   0 andrej5    (501) staff       (20)       38 2023-06-02 06:09:08.035985 drukarnia-api-0.1.61/setup.cfg
--rw-r--r--   0 andrej5    (501) staff       (20)     1387 2023-06-02 06:07:52.000000 drukarnia-api-0.1.61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:08:14.609060 drukarnia-api-0.1.75/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-19 10:08:01.000000 drukarnia-api-0.1.75/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-19 10:08:14.609060 drukarnia-api-0.1.75/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-19 10:08:01.000000 drukarnia-api-0.1.75/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:08:14.609060 drukarnia-api-0.1.75/drukarnia_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-19 10:08:01.000000 drukarnia-api-0.1.75/drukarnia_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-06-19 10:08:01.000000 drukarnia-api-0.1.75/drukarnia_api/article.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-06-19 10:08:01.000000 drukarnia-api-0.1.75/drukarnia_api/author.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-19 10:08:01.000000 drukarnia-api-0.1.75/drukarnia_api/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-06-19 10:08:01.000000 drukarnia-api-0.1.75/drukarnia_api/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:08:14.609060 drukarnia-api-0.1.75/drukarnia_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-19 10:08:14.000000 drukarnia-api-0.1.75/drukarnia_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-19 10:08:14.000000 drukarnia-api-0.1.75/drukarnia_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 10:08:14.000000 drukarnia-api-0.1.75/drukarnia_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-19 10:08:14.000000 drukarnia-api-0.1.75/drukarnia_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 10:08:14.000000 drukarnia-api-0.1.75/drukarnia_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 10:08:14.609060 drukarnia-api-0.1.75/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-19 10:08:01.000000 drukarnia-api-0.1.75/setup.py
```

### Comparing `drukarnia-api-0.1.61/LICENSE` & `drukarnia-api-0.1.75/LICENSE`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.61/PKG-INFO` & `drukarnia-api-0.1.75/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drukarnia-api
-Version: 0.1.61
+Version: 0.1.75
 Summary: wrapper for the Drukarnia API
 Home-page: https://github.com/androu-sys/drukarnia-api
 Author: Andrii Herts
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -19,23 +19,53 @@
 
 # drukarnia-api
 
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/androu-sys/drukarnia-api/blob/main/LICENSE)
 
 ## Overview
-`drukarnia-api` is a Python library designed as a wrapper for the ***Drukarnia API***, which provides various functionalities for interacting with the Drukarnia platform. It simplifies the process of accessing and manipulating data from the ***Drukarnia API***, allowing users to integrate Drukarnia's features seamlessly into their applications.
+`drukarnia-api` is a Python library designed as a wrapper for the ***Drukarnia API***, providing various functionalities for interacting with the Drukarnia platform. It simplifies the process of accessing and manipulating data from the Drukarnia API, enabling users to seamlessly integrate Drukarnia's features into their applications. The library is actively being developed and already includes almost all of the necessary features. We are working diligently to implement the remaining features as quickly as possible.
 
-Please note that the library is currently in its early development stages and supports only information search. However, future updates will expand its capabilities to include posting articles, comments, and more.
 
-For a detailed overview of the available functionalities and how to use them, please refer to the [***Functionality Overview File***](https://github.com/androu-sys/drukarnia-api/blob/main/overview.ipynb).
+## Simple Usage
+```python
+from drukarnia_api import Search
+
+
+async def get_author_article_titles():
+    # Retrieve all results
+    authors = await Search().find_author('cupomanka')
+    # Get the first search result
+    author = authors[0]
+
+    # Collect all data about the user
+    await author.collect_data()
+
+    # Get user articles
+    articles = await author.articles
+
+    # Print all titles
+    for article in articles:
+        print(article.title)
+
+    # Close the session (we are still considering the best way to make it seamless)
+    await author.close_session()
+
+
+if __name__ == '__main__':
+    import asyncio
+
+    loop = asyncio.get_event_loop()
+    loop.run_until_complete(get_author_article_titles())
+```
+
 
 ## Installation
 You can install `drukarnia-api` using pip:
 
 ```bash
-pip install drukarnia-api==0.1.61
+pip install drukarnia-api
 ```
 
 ## Contributing
 
 Contributions to `drukarnia-api` are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request on the GitHub repository: https://github.com/androu-sys/drukarnia-api.
```

### Comparing `drukarnia-api-0.1.61/drukarnia_api.egg-info/PKG-INFO` & `drukarnia-api-0.1.75/drukarnia_api.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drukarnia-api
-Version: 0.1.61
+Version: 0.1.75
 Summary: wrapper for the Drukarnia API
 Home-page: https://github.com/androu-sys/drukarnia-api
 Author: Andrii Herts
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -19,23 +19,53 @@
 
 # drukarnia-api
 
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/androu-sys/drukarnia-api/blob/main/LICENSE)
 
 ## Overview
-`drukarnia-api` is a Python library designed as a wrapper for the ***Drukarnia API***, which provides various functionalities for interacting with the Drukarnia platform. It simplifies the process of accessing and manipulating data from the ***Drukarnia API***, allowing users to integrate Drukarnia's features seamlessly into their applications.
+`drukarnia-api` is a Python library designed as a wrapper for the ***Drukarnia API***, providing various functionalities for interacting with the Drukarnia platform. It simplifies the process of accessing and manipulating data from the Drukarnia API, enabling users to seamlessly integrate Drukarnia's features into their applications. The library is actively being developed and already includes almost all of the necessary features. We are working diligently to implement the remaining features as quickly as possible.
 
-Please note that the library is currently in its early development stages and supports only information search. However, future updates will expand its capabilities to include posting articles, comments, and more.
 
-For a detailed overview of the available functionalities and how to use them, please refer to the [***Functionality Overview File***](https://github.com/androu-sys/drukarnia-api/blob/main/overview.ipynb).
+## Simple Usage
+```python
+from drukarnia_api import Search
+
+
+async def get_author_article_titles():
+    # Retrieve all results
+    authors = await Search().find_author('cupomanka')
+    # Get the first search result
+    author = authors[0]
+
+    # Collect all data about the user
+    await author.collect_data()
+
+    # Get user articles
+    articles = await author.articles
+
+    # Print all titles
+    for article in articles:
+        print(article.title)
+
+    # Close the session (we are still considering the best way to make it seamless)
+    await author.close_session()
+
+
+if __name__ == '__main__':
+    import asyncio
+
+    loop = asyncio.get_event_loop()
+    loop.run_until_complete(get_author_article_titles())
+```
+
 
 ## Installation
 You can install `drukarnia-api` using pip:
 
 ```bash
-pip install drukarnia-api==0.1.61
+pip install drukarnia-api
 ```
 
 ## Contributing
 
 Contributions to `drukarnia-api` are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request on the GitHub repository: https://github.com/androu-sys/drukarnia-api.
```

### Comparing `drukarnia-api-0.1.61/setup.py` & `drukarnia-api-0.1.75/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Get requirements
 with open(path.join(HERE, 'requirements.txt')) as f:
     requirements = f.read().splitlines()
 
 # This call to setup() does all the work
 setup(
     name="drukarnia-api",
-    version="0.1.61",
+    version="0.1.75",
     description="wrapper for the Drukarnia API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/androu-sys/drukarnia-api",
     author="Andrii Herts",
     license="MIT",
     classifiers=[
```

