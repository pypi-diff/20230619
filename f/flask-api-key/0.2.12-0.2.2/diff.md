# Comparing `tmp/flask-api-key-0.2.12.tar.gz` & `tmp/flask-api-key-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-api-key-0.2.12.tar", last modified: Mon Jun 19 00:05:14 2023, max compression
+gzip compressed data, was "flask-api-key-0.2.2.tar", last modified: Thu Jun 16 04:06:31 2022, max compression
```

## Comparing `flask-api-key-0.2.12.tar` & `flask-api-key-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:05:14.789851 flask-api-key-0.2.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-19 00:04:52.000000 flask-api-key-0.2.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-06-19 00:05:14.785851 flask-api-key-0.2.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-19 00:04:52.000000 flask-api-key-0.2.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:05:14.785851 flask-api-key-0.2.12/flask_api_key/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-19 00:04:52.000000 flask-api-key-0.2.12/flask_api_key/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-19 00:04:52.000000 flask-api-key-0.2.12/flask_api_key/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-06-19 00:04:52.000000 flask-api-key-0.2.12/flask_api_key/api_key_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-19 00:04:52.000000 flask-api-key-0.2.12/flask_api_key/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-19 00:04:52.000000 flask-api-key-0.2.12/flask_api_key/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-19 00:04:52.000000 flask-api-key-0.2.12/flask_api_key/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:05:14.785851 flask-api-key-0.2.12/flask_api_key.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-06-19 00:05:14.000000 flask-api-key-0.2.12/flask_api_key.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-19 00:05:14.000000 flask-api-key-0.2.12/flask_api_key.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 00:05:14.000000 flask-api-key-0.2.12/flask_api_key.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-19 00:05:14.000000 flask-api-key-0.2.12/flask_api_key.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 00:05:14.000000 flask-api-key-0.2.12/flask_api_key.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-19 00:04:52.000000 flask-api-key-0.2.12/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 00:05:14.789851 flask-api-key-0.2.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-19 00:04:52.000000 flask-api-key-0.2.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 04:06:31.548684 flask-api-key-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-06-16 04:06:16.000000 flask-api-key-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     5618 2022-06-16 04:06:31.548684 flask-api-key-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5234 2022-06-16 04:06:16.000000 flask-api-key-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 04:06:31.544684 flask-api-key-0.2.2/flask_api_key/
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2022-06-16 04:06:16.000000 flask-api-key-0.2.2/flask_api_key/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4335 2022-06-16 04:06:16.000000 flask-api-key-0.2.2/flask_api_key/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8140 2022-06-16 04:06:16.000000 flask-api-key-0.2.2/flask_api_key/api_key_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1520 2022-06-16 04:06:16.000000 flask-api-key-0.2.2/flask_api_key/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2233 2022-06-16 04:06:16.000000 flask-api-key-0.2.2/flask_api_key/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      682 2022-06-16 04:06:16.000000 flask-api-key-0.2.2/flask_api_key/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 04:06:31.548684 flask-api-key-0.2.2/flask_api_key.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5618 2022-06-16 04:06:30.000000 flask-api-key-0.2.2/flask_api_key.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      379 2022-06-16 04:06:31.000000 flask-api-key-0.2.2/flask_api_key.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-16 04:06:30.000000 flask-api-key-0.2.2/flask_api_key.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-06-16 04:06:31.000000 flask-api-key-0.2.2/flask_api_key.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-16 04:06:31.000000 flask-api-key-0.2.2/flask_api_key.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-06-16 04:06:16.000000 flask-api-key-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-16 04:06:31.548684 flask-api-key-0.2.2/setup.cfg
```

### Comparing `flask-api-key-0.2.12/LICENSE` & `flask-api-key-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-api-key-0.2.12/PKG-INFO` & `flask-api-key-0.2.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,20 @@
-Metadata-Version: 2.1
-Name: flask-api-key
-Version: 0.2.12
-Summary: Provide api-key based auth for your apis.
-License: MIT
-Keywords: api,auth
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Flask
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit) 
-[![Build and publish pkg](https://github.com/jthop/flask-api-key/actions/workflows/python-publish.yml/badge.svg)](https://github.com/jthop/flask-api-key/actions/workflows/python-publish.yml)
-[![PyPI version](https://badge.fury.io/py/flask-api-key.svg)](https://badge.fury.io/py/flask-api-key)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit) [![PyPI version](https://badge.fury.io/py/flask-api-key.svg)](https://badge.fury.io/py/flask-api-key)
+[![GitHub last commit](https://img.shields.io/github/last-commit/jthop/flask-api-key)](./)
+[![saythanks](https://img.shields.io/badge/say-thanks-brightgreen.svg)](https://saythanks.io/to/jthop)
+[![Whos your daddy](https://img.shields.io/badge/whos%20your%20daddy-2.0.7rc3-brightgreen.svg)](https://14.do/)
+[![Visitors](https://api.visitorbadge.io/api/visitors?path=jhopper%2Fflask-api-key&label=visitors&countColor=%2337d67a&style=flat)](https://visitorbadge.io/status?path=jhopper%2Fflask-api-key)
+[![Awesome Badges](https://img.shields.io/badge/badges-awesome-green.svg)](https://github.com/Naereen/badges)
+[![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
-[![GitHub last commit](https://img.shields.io/github/last-commit/jthop/flask-api-key)](https://github.com/jthop/flask-api-key)
-[![GitHub repo size](https://img.shields.io/github/repo-size/jthop/flask-api-key?style=flat)](https://github.com/jthop/flask-api-key)
-[![GitHub language count](https://img.shields.io/github/languages/count/jthop/flask-api-key?style=flat)](https://github.com/jthop/flask-api-key)
+[![GitHub repo size](https://img.shields.io/github/repo-size/jthop/flask-api-key?style=flat)](./)
+[![GitHub language count](https://img.shields.io/github/languages/count/jthop/flask-api-key?style=flat)](./)
 [![GitHub top language](https://img.shields.io/github/languages/top/jthop/flask-api-key?style=flat)](https://python.org)
 [![Profile View Counter](https://komarev.com/ghpvc/?username=jthop)](./)
-[![Visitors](https://api.visitorbadge.io/api/visitors?path=jhopper%2Fflask-api-key&label=visitors&countColor=%234c1&style=flat)](https://visitorbadge.io/status?path=jhopper%2Fflask-api-key)
-[![Whos your daddy](https://img.shields.io/badge/whos%20your%20daddy-2.0.7rc3-brightgreen.svg)](https://14.do/)
-[![volkswagen status](https://auchenberg.github.io/volkswagen/volkswargen_ci.svg?v=1)](https://github.com/auchenberg/volkswagen)
-[![works badge](https://cdn.jsdelivr.net/gh/nikku/works-on-my-machine@v0.2.0/badge.svg)](https://github.com/nikku/works-on-my-machine)
-<!-- [![No Maintenance Intended](http://unmaintained.tech/badge.svg)](http://unmaintained.tech/) -->
-
-
-# flask-api-key #
+[![No Maintenance Intended](http://unmaintained.tech/badge.svg)](http://unmaintained.tech/)
 
 Simple Flask Extension to easily add api auth using the good tried and tested api key model.
 
 ## Why :man_shrugging: ##
 
 JWTs can be great.  Especially if you have 100 microservices and are growing at the rate of Facebook.
```

### Comparing `flask-api-key-0.2.12/README.md` & `flask-api-key-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,33 @@
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit) 
-[![Build and publish pkg](https://github.com/jthop/flask-api-key/actions/workflows/python-publish.yml/badge.svg)](https://github.com/jthop/flask-api-key/actions/workflows/python-publish.yml)
-[![PyPI version](https://badge.fury.io/py/flask-api-key.svg)](https://badge.fury.io/py/flask-api-key)
+Metadata-Version: 2.1
+Name: flask-api-key
+Version: 0.2.2
+Summary: Provide api-key based auth for your apis.
+License: MIT
+Keywords: api,auth
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Flask
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit) [![PyPI version](https://badge.fury.io/py/flask-api-key.svg)](https://badge.fury.io/py/flask-api-key)
+[![GitHub last commit](https://img.shields.io/github/last-commit/jthop/flask-api-key)](./)
+[![saythanks](https://img.shields.io/badge/say-thanks-brightgreen.svg)](https://saythanks.io/to/jthop)
+[![Whos your daddy](https://img.shields.io/badge/whos%20your%20daddy-2.0.7rc3-brightgreen.svg)](https://14.do/)
+[![Visitors](https://api.visitorbadge.io/api/visitors?path=jhopper%2Fflask-api-key&label=visitors&countColor=%2337d67a&style=flat)](https://visitorbadge.io/status?path=jhopper%2Fflask-api-key)
+[![Awesome Badges](https://img.shields.io/badge/badges-awesome-green.svg)](https://github.com/Naereen/badges)
+[![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
-[![GitHub last commit](https://img.shields.io/github/last-commit/jthop/flask-api-key)](https://github.com/jthop/flask-api-key)
-[![GitHub repo size](https://img.shields.io/github/repo-size/jthop/flask-api-key?style=flat)](https://github.com/jthop/flask-api-key)
-[![GitHub language count](https://img.shields.io/github/languages/count/jthop/flask-api-key?style=flat)](https://github.com/jthop/flask-api-key)
+[![GitHub repo size](https://img.shields.io/github/repo-size/jthop/flask-api-key?style=flat)](./)
+[![GitHub language count](https://img.shields.io/github/languages/count/jthop/flask-api-key?style=flat)](./)
 [![GitHub top language](https://img.shields.io/github/languages/top/jthop/flask-api-key?style=flat)](https://python.org)
 [![Profile View Counter](https://komarev.com/ghpvc/?username=jthop)](./)
-[![Visitors](https://api.visitorbadge.io/api/visitors?path=jhopper%2Fflask-api-key&label=visitors&countColor=%234c1&style=flat)](https://visitorbadge.io/status?path=jhopper%2Fflask-api-key)
-[![Whos your daddy](https://img.shields.io/badge/whos%20your%20daddy-2.0.7rc3-brightgreen.svg)](https://14.do/)
-[![volkswagen status](https://auchenberg.github.io/volkswagen/volkswargen_ci.svg?v=1)](https://github.com/auchenberg/volkswagen)
-[![works badge](https://cdn.jsdelivr.net/gh/nikku/works-on-my-machine@v0.2.0/badge.svg)](https://github.com/nikku/works-on-my-machine)
-<!-- [![No Maintenance Intended](http://unmaintained.tech/badge.svg)](http://unmaintained.tech/) -->
-
-
-# flask-api-key #
+[![No Maintenance Intended](http://unmaintained.tech/badge.svg)](http://unmaintained.tech/)
 
 Simple Flask Extension to easily add api auth using the good tried and tested api key model.
 
 ## Why :man_shrugging: ##
 
 JWTs can be great.  Especially if you have 100 microservices and are growing at the rate of Facebook.
```

### Comparing `flask-api-key-0.2.12/flask_api_key/api_key.py` & `flask-api-key-0.2.2/flask_api_key/api_key.py`

 * *Files identical despite different names*

### Comparing `flask-api-key-0.2.12/flask_api_key/api_key_manager.py` & `flask-api-key-0.2.2/flask_api_key/api_key_manager.py`

 * *Files identical despite different names*

### Comparing `flask-api-key-0.2.12/flask_api_key/decorators.py` & `flask-api-key-0.2.2/flask_api_key/decorators.py`

 * *Files identical despite different names*

### Comparing `flask-api-key-0.2.12/flask_api_key/exceptions.py` & `flask-api-key-0.2.2/flask_api_key/exceptions.py`

 * *Files identical despite different names*

### Comparing `flask-api-key-0.2.12/flask_api_key/utils.py` & `flask-api-key-0.2.2/flask_api_key/utils.py`

 * *Files identical despite different names*

### Comparing `flask-api-key-0.2.12/flask_api_key.egg-info/PKG-INFO` & `flask-api-key-0.2.2/flask_api_key.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: flask-api-key
-Version: 0.2.12
+Version: 0.2.2
 Summary: Provide api-key based auth for your apis.
 License: MIT
 Keywords: api,auth
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit) 
-[![Build and publish pkg](https://github.com/jthop/flask-api-key/actions/workflows/python-publish.yml/badge.svg)](https://github.com/jthop/flask-api-key/actions/workflows/python-publish.yml)
-[![PyPI version](https://badge.fury.io/py/flask-api-key.svg)](https://badge.fury.io/py/flask-api-key)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit) [![PyPI version](https://badge.fury.io/py/flask-api-key.svg)](https://badge.fury.io/py/flask-api-key)
+[![GitHub last commit](https://img.shields.io/github/last-commit/jthop/flask-api-key)](./)
+[![saythanks](https://img.shields.io/badge/say-thanks-brightgreen.svg)](https://saythanks.io/to/jthop)
+[![Whos your daddy](https://img.shields.io/badge/whos%20your%20daddy-2.0.7rc3-brightgreen.svg)](https://14.do/)
+[![Visitors](https://api.visitorbadge.io/api/visitors?path=jhopper%2Fflask-api-key&label=visitors&countColor=%2337d67a&style=flat)](https://visitorbadge.io/status?path=jhopper%2Fflask-api-key)
+[![Awesome Badges](https://img.shields.io/badge/badges-awesome-green.svg)](https://github.com/Naereen/badges)
+[![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
-[![GitHub last commit](https://img.shields.io/github/last-commit/jthop/flask-api-key)](https://github.com/jthop/flask-api-key)
-[![GitHub repo size](https://img.shields.io/github/repo-size/jthop/flask-api-key?style=flat)](https://github.com/jthop/flask-api-key)
-[![GitHub language count](https://img.shields.io/github/languages/count/jthop/flask-api-key?style=flat)](https://github.com/jthop/flask-api-key)
+[![GitHub repo size](https://img.shields.io/github/repo-size/jthop/flask-api-key?style=flat)](./)
+[![GitHub language count](https://img.shields.io/github/languages/count/jthop/flask-api-key?style=flat)](./)
 [![GitHub top language](https://img.shields.io/github/languages/top/jthop/flask-api-key?style=flat)](https://python.org)
 [![Profile View Counter](https://komarev.com/ghpvc/?username=jthop)](./)
-[![Visitors](https://api.visitorbadge.io/api/visitors?path=jhopper%2Fflask-api-key&label=visitors&countColor=%234c1&style=flat)](https://visitorbadge.io/status?path=jhopper%2Fflask-api-key)
-[![Whos your daddy](https://img.shields.io/badge/whos%20your%20daddy-2.0.7rc3-brightgreen.svg)](https://14.do/)
-[![volkswagen status](https://auchenberg.github.io/volkswagen/volkswargen_ci.svg?v=1)](https://github.com/auchenberg/volkswagen)
-[![works badge](https://cdn.jsdelivr.net/gh/nikku/works-on-my-machine@v0.2.0/badge.svg)](https://github.com/nikku/works-on-my-machine)
-<!-- [![No Maintenance Intended](http://unmaintained.tech/badge.svg)](http://unmaintained.tech/) -->
-
-
-# flask-api-key #
+[![No Maintenance Intended](http://unmaintained.tech/badge.svg)](http://unmaintained.tech/)
 
 Simple Flask Extension to easily add api auth using the good tried and tested api key model.
 
 ## Why :man_shrugging: ##
 
 JWTs can be great.  Especially if you have 100 microservices and are growing at the rate of Facebook.
```

### Comparing `flask-api-key-0.2.12/pyproject.toml` & `flask-api-key-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -18,11 +18,8 @@
     "flask",
     "passlib",
     'importlib-metadata; python_version<"3.8"',
 ]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
-version = {attr = "flask_api_key.__public_version__"}
-
-[tool.black]
-line-length = 88
+version = {attr = "flask_api_key.__version__"}
```

