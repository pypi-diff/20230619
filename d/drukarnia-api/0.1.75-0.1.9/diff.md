# Comparing `tmp/drukarnia-api-0.1.75.tar.gz` & `tmp/drukarnia-api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drukarnia-api-0.1.75.tar", last modified: Mon Jun 19 10:08:14 2023, max compression
+gzip compressed data, was "drukarnia-api-0.1.9.tar", last modified: Mon Jun 19 13:02:01 2023, max compression
```

## Comparing `drukarnia-api-0.1.75.tar` & `drukarnia-api-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:08:14.609060 drukarnia-api-0.1.75/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-19 10:08:01.000000 drukarnia-api-0.1.75/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-19 10:08:14.609060 drukarnia-api-0.1.75/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-19 10:08:01.000000 drukarnia-api-0.1.75/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:08:14.609060 drukarnia-api-0.1.75/drukarnia_api/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-19 10:08:01.000000 drukarnia-api-0.1.75/drukarnia_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-06-19 10:08:01.000000 drukarnia-api-0.1.75/drukarnia_api/article.py
--rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-06-19 10:08:01.000000 drukarnia-api-0.1.75/drukarnia_api/author.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-19 10:08:01.000000 drukarnia-api-0.1.75/drukarnia_api/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-06-19 10:08:01.000000 drukarnia-api-0.1.75/drukarnia_api/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:08:14.609060 drukarnia-api-0.1.75/drukarnia_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-19 10:08:14.000000 drukarnia-api-0.1.75/drukarnia_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-19 10:08:14.000000 drukarnia-api-0.1.75/drukarnia_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 10:08:14.000000 drukarnia-api-0.1.75/drukarnia_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-19 10:08:14.000000 drukarnia-api-0.1.75/drukarnia_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 10:08:14.000000 drukarnia-api-0.1.75/drukarnia_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 10:08:14.609060 drukarnia-api-0.1.75/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-19 10:08:01.000000 drukarnia-api-0.1.75/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:02:01.468697 drukarnia-api-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-19 13:01:52.000000 drukarnia-api-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-19 13:02:01.468697 drukarnia-api-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-19 13:01:52.000000 drukarnia-api-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:02:01.464697 drukarnia-api-0.1.9/drukarnia_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-19 13:01:52.000000 drukarnia-api-0.1.9/drukarnia_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-06-19 13:01:52.000000 drukarnia-api-0.1.9/drukarnia_api/article.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-06-19 13:01:52.000000 drukarnia-api-0.1.9/drukarnia_api/author.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:02:01.468697 drukarnia-api-0.1.9/drukarnia_api/drukarnia_base/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-19 13:01:52.000000 drukarnia-api-0.1.9/drukarnia_api/drukarnia_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-06-19 13:01:52.000000 drukarnia-api-0.1.9/drukarnia_api/drukarnia_base/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-19 13:01:52.000000 drukarnia-api-0.1.9/drukarnia_api/drukarnia_base/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-19 13:01:52.000000 drukarnia-api-0.1.9/drukarnia_api/drukarnia_base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-19 13:01:52.000000 drukarnia-api-0.1.9/drukarnia_api/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:02:01.468697 drukarnia-api-0.1.9/drukarnia_api/shortcuts/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-19 13:01:52.000000 drukarnia-api-0.1.9/drukarnia_api/shortcuts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-19 13:01:52.000000 drukarnia-api-0.1.9/drukarnia_api/shortcuts/class_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-19 13:01:52.000000 drukarnia-api-0.1.9/drukarnia_api/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:02:01.464697 drukarnia-api-0.1.9/drukarnia_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-19 13:02:01.000000 drukarnia-api-0.1.9/drukarnia_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-19 13:02:01.000000 drukarnia-api-0.1.9/drukarnia_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:02:01.000000 drukarnia-api-0.1.9/drukarnia_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-19 13:02:01.000000 drukarnia-api-0.1.9/drukarnia_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 13:02:01.000000 drukarnia-api-0.1.9/drukarnia_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 13:02:01.468697 drukarnia-api-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-19 13:01:52.000000 drukarnia-api-0.1.9/setup.py
```

### Comparing `drukarnia-api-0.1.75/LICENSE` & `drukarnia-api-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.75/PKG-INFO` & `drukarnia-api-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drukarnia-api
-Version: 0.1.75
+Version: 0.1.9
 Summary: wrapper for the Drukarnia API
 Home-page: https://github.com/androu-sys/drukarnia-api
 Author: Andrii Herts
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `drukarnia-api-0.1.75/README.md` & `drukarnia-api-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.75/drukarnia_api/article.py` & `drukarnia-api-0.1.9/drukarnia_api/article.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from datetime import datetime
 from warnings import warn
 from aiohttp import ClientSession
-from drukarnia_api.drukarnia_base.element import DrukarniaElement
-from drukarnia_api.shortcuts.class_generator import data2authors, data2articles, data2tags
+
+from drukarnia_api.drukarnia_base import DrukarniaElement
+from drukarnia_api.shortcuts import data2authors, data2articles, data2tags
+
 from typing import TYPE_CHECKING, Tuple, Dict, List
 
 if TYPE_CHECKING:   # always False, used for type hints
     from drukarnia_api.author import Author
     from drukarnia_api.tag import Tag
```

### Comparing `drukarnia-api-0.1.75/drukarnia_api/author.py` & `drukarnia-api-0.1.9/drukarnia_api/author.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import re
 from datetime import datetime
 from typing import Dict, Tuple, List
 from warnings import warn
 from aiohttp import ClientSession
-from drukarnia_api.drukarnia_base.element import DrukarniaElement
-from drukarnia_api.shortcuts.class_generator import data2authors, data2articles, data2tags
+
+from drukarnia_api.drukarnia_base import DrukarniaElement
+from drukarnia_api.shortcuts import data2authors, data2articles, data2tags
 
 from typing import TYPE_CHECKING
+
 if TYPE_CHECKING:   # always False, used for type hints
     from drukarnia_api.article import Article
     from drukarnia_api.tag import Tag
 
 
 class Author(DrukarniaElement):
     def __init__(self, username: str = None, author_id: str = None, *args, **kwargs):
```

### Comparing `drukarnia-api-0.1.75/drukarnia_api/search.py` & `drukarnia-api-0.1.9/drukarnia_api/search.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-import asyncio
-
-from drukarnia_api.drukarnia_base.connection import Connection
-from drukarnia_api.shortcuts.class_generator import data2authors, data2articles, data2tags
+from drukarnia_api.drukarnia_base import Connection
+from drukarnia_api.shortcuts import data2authors, data2articles, data2tags
 
 from typing import TYPE_CHECKING, Tuple, Dict
 
 if TYPE_CHECKING:   # always False, used for type hints
     from drukarnia_api.article import Article
     from drukarnia_api.tag import Tag
     from drukarnia_api.author import Author
```

### Comparing `drukarnia-api-0.1.75/drukarnia_api/tag.py` & `drukarnia-api-0.1.9/drukarnia_api/tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from aiohttp import ClientSession
-from drukarnia_api.drukarnia_base.element import DrukarniaElement
-from drukarnia_api.shortcuts.class_generator import data2articles
+
+from drukarnia_api.drukarnia_base import DrukarniaElement
+from drukarnia_api.shortcuts import data2articles
+
 from typing import TYPE_CHECKING, Tuple, Dict
 
 if TYPE_CHECKING:   # always False, used for type hints
     from drukarnia_api.article import Article
 
 
 class Tag(DrukarniaElement):
```

### Comparing `drukarnia-api-0.1.75/drukarnia_api.egg-info/PKG-INFO` & `drukarnia-api-0.1.9/drukarnia_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drukarnia-api
-Version: 0.1.75
+Version: 0.1.9
 Summary: wrapper for the Drukarnia API
 Home-page: https://github.com/androu-sys/drukarnia-api
 Author: Andrii Herts
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `drukarnia-api-0.1.75/setup.py` & `drukarnia-api-0.1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Get requirements
 with open(path.join(HERE, 'requirements.txt')) as f:
     requirements = f.read().splitlines()
 
 # This call to setup() does all the work
 setup(
     name="drukarnia-api",
-    version="0.1.75",
+    version="0.1.9",
     description="wrapper for the Drukarnia API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/androu-sys/drukarnia-api",
     author="Andrii Herts",
     license="MIT",
     classifiers=[
@@ -33,11 +33,11 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
-    packages=["drukarnia_api"],
+    packages=["drukarnia_api", "drukarnia_api.drukarnia_base", "drukarnia_api.shortcuts"],
     include_package_data=True,
     install_requires=requirements
 )
```

