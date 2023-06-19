# Comparing `tmp/nrt-logging-1.3.3.tar.gz` & `tmp/nrt-logging-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrt-logging-1.3.3.tar", last modified: Wed Jun 14 06:33:30 2023, max compression
+gzip compressed data, was "nrt-logging-1.3.4.tar", last modified: Mon Jun 19 15:45:18 2023, max compression
```

## Comparing `nrt-logging-1.3.3.tar` & `nrt-logging-1.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 06:33:30.202990 nrt-logging-1.3.3/
--rw-rw-rw-   0        0        0     1088 2022-11-23 08:09:14.000000 nrt-logging-1.3.3/LICENSE.md
--rw-rw-rw-   0        0        0     7760 2023-06-14 06:33:30.202990 nrt-logging-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     6762 2023-06-14 06:13:12.000000 nrt-logging-1.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 06:33:30.196476 nrt-logging-1.3.3/nrt_logging/
--rw-rw-rw-   0        0        0      298 2023-06-14 06:13:43.000000 nrt-logging-1.3.3/nrt_logging/__init__.py
--rw-rw-rw-   0        0        0    14373 2022-11-23 08:09:14.000000 nrt-logging-1.3.3/nrt_logging/config.py
--rw-rw-rw-   0        0        0      237 2022-11-23 08:09:14.000000 nrt-logging-1.3.3/nrt_logging/exceptions.py
--rw-rw-rw-   0        0        0     1851 2022-11-23 08:09:14.000000 nrt-logging-1.3.3/nrt_logging/log_format.py
--rw-rw-rw-   0        0        0      990 2022-11-23 08:09:14.000000 nrt-logging-1.3.3/nrt_logging/log_level.py
--rw-rw-rw-   0        0        0     5905 2022-11-26 09:18:33.000000 nrt-logging-1.3.3/nrt_logging/logger.py
--rw-rw-rw-   0        0        0    11456 2022-11-26 18:50:22.000000 nrt-logging-1.3.3/nrt_logging/logger_manager.py
--rw-rw-rw-   0        0        0    45309 2022-12-10 22:13:13.000000 nrt-logging-1.3.3/nrt_logging/logger_stream_handlers.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:33:30.201990 nrt-logging-1.3.3/nrt_logging.egg-info/
--rw-rw-rw-   0        0        0     7760 2023-06-14 06:33:30.000000 nrt-logging-1.3.3/nrt_logging.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-06-14 06:33:30.000000 nrt-logging-1.3.3/nrt_logging.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 06:33:30.000000 nrt-logging-1.3.3/nrt_logging.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-14 06:33:30.000000 nrt-logging-1.3.3/nrt_logging.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-14 06:33:30.000000 nrt-logging-1.3.3/nrt_logging.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      983 2023-06-14 06:14:10.000000 nrt-logging-1.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       31 2022-11-23 08:09:14.000000 nrt-logging-1.3.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 06:33:30.202990 nrt-logging-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1236 2022-11-23 08:09:14.000000 nrt-logging-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:45:18.200834 nrt-logging-1.3.4/
+-rw-rw-rw-   0        0        0     1088 2022-11-23 08:09:14.000000 nrt-logging-1.3.4/LICENSE.md
+-rw-rw-rw-   0        0        0     7753 2023-06-19 15:45:18.200834 nrt-logging-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6755 2023-06-19 15:29:43.000000 nrt-logging-1.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 15:45:18.195148 nrt-logging-1.3.4/nrt_logging/
+-rw-rw-rw-   0        0        0      298 2023-06-19 14:57:47.000000 nrt-logging-1.3.4/nrt_logging/__init__.py
+-rw-rw-rw-   0        0        0    14373 2022-11-23 08:09:14.000000 nrt-logging-1.3.4/nrt_logging/config.py
+-rw-rw-rw-   0        0        0      237 2022-11-23 08:09:14.000000 nrt-logging-1.3.4/nrt_logging/exceptions.py
+-rw-rw-rw-   0        0        0     1851 2022-11-23 08:09:14.000000 nrt-logging-1.3.4/nrt_logging/log_format.py
+-rw-rw-rw-   0        0        0      990 2022-11-23 08:09:14.000000 nrt-logging-1.3.4/nrt_logging/log_level.py
+-rw-rw-rw-   0        0        0     5905 2022-11-26 09:18:33.000000 nrt-logging-1.3.4/nrt_logging/logger.py
+-rw-rw-rw-   0        0        0    11456 2022-11-26 18:50:22.000000 nrt-logging-1.3.4/nrt_logging/logger_manager.py
+-rw-rw-rw-   0        0        0    45309 2022-12-10 22:13:13.000000 nrt-logging-1.3.4/nrt_logging/logger_stream_handlers.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:45:18.199817 nrt-logging-1.3.4/nrt_logging.egg-info/
+-rw-rw-rw-   0        0        0     7753 2023-06-19 15:45:18.000000 nrt-logging-1.3.4/nrt_logging.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-06-19 15:45:18.000000 nrt-logging-1.3.4/nrt_logging.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 15:45:18.000000 nrt-logging-1.3.4/nrt_logging.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-19 15:45:18.000000 nrt-logging-1.3.4/nrt_logging.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-19 15:45:18.000000 nrt-logging-1.3.4/nrt_logging.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      983 2023-06-19 15:06:52.000000 nrt-logging-1.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       31 2022-11-23 08:09:14.000000 nrt-logging-1.3.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 15:45:18.201821 nrt-logging-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1236 2022-11-23 08:09:14.000000 nrt-logging-1.3.4/setup.py
```

### Comparing `nrt-logging-1.3.3/LICENSE.md` & `nrt-logging-1.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nrt-logging-1.3.3/PKG-INFO` & `nrt-logging-1.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrt-logging
-Version: 1.3.3
+Version: 1.3.4
 Summary: Hierarchical logging in yaml format
 Home-page: https://github.com/etuzon/Python-NRT-Logging
 Author: Eyal Tuzon
 Author-email: Eyal Tuzon <eyal.tuzon.dev@gmail.com>
 Project-URL: Homepage, https://github.com/etuzon/Python-NRT-Logging
 Project-URL: Bug Tracker, https://github.com/etuzon/Python-NRT-Logging/issues
 Project-URL: documentation, https://github.com/etuzon/Python-NRT-Logging/wiki
@@ -22,18 +22,18 @@
 # Hierarchical logging in yaml format.
 
 ![PyPI](https://img.shields.io/pypi/v/nrt-logging?color=blueviolet&style=plastic)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nrt-logging?color=greens&style=plastic)
 ![PyPI - License](https://img.shields.io/pypi/l/nrt-logging?color=blue&style=plastic)
 ![PyPI - Downloads](https://img.shields.io/pypi/dd/nrt-logging?style=plastic)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/nrt-logging?color=yellow&style=plastic)
-[![Coverage Status](https://coveralls.io/repos/github/etuzon/Python-NRT-Logging/badge.svg)](https://coveralls.io/github/etuzon/Python-NRT-Logging)
-![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/etuzon/Python-NRT-Logging?style=plastic)
-![GitHub last commit](https://img.shields.io/github/last-commit/etuzon/Python-NRT-Logging?style=plastic)
-[![DeepSource](https://deepsource.io/gh/etuzon/Python-NRT-Logging.svg/?label=active+issues&token=3pUgM1IEwZG6Gpuc065dKDxM)](https://deepsource.io/gh/etuzon/Python-NRT-Logging/?ref=repository-badge)
+[![Coverage Status](https://coveralls.io/repos/github/etuzon/nrt-logging/badge.svg)](https://coveralls.io/github/etuzon/pytohn-nrt-logging)
+![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/etuzon/python-nrt-logging?style=plastic)
+![GitHub last commit](https://img.shields.io/github/last-commit/etuzon/python-nrt-logging?style=plastic)
+[![DeepSource](https://deepsource.io/gh/etuzon/python-nrt-logging.svg/?label=active+issues&token=3pUgM1IEwZG6Gpuc065dKDxM)](https://deepsource.io/gh/etuzon/python-nrt-logging/?ref=repository-badge)
 
 Hierarchical logging help to group logs that are related to the same code flow.
 
 Log style can be styled in Yaml format or in Line format.
 
 ### Examples:
```

### Comparing `nrt-logging-1.3.3/README.md` & `nrt-logging-1.3.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Hierarchical logging in yaml format.
 
 ![PyPI](https://img.shields.io/pypi/v/nrt-logging?color=blueviolet&style=plastic)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nrt-logging?color=greens&style=plastic)
 ![PyPI - License](https://img.shields.io/pypi/l/nrt-logging?color=blue&style=plastic)
 ![PyPI - Downloads](https://img.shields.io/pypi/dd/nrt-logging?style=plastic)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/nrt-logging?color=yellow&style=plastic)
-[![Coverage Status](https://coveralls.io/repos/github/etuzon/Python-NRT-Logging/badge.svg)](https://coveralls.io/github/etuzon/Python-NRT-Logging)
-![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/etuzon/Python-NRT-Logging?style=plastic)
-![GitHub last commit](https://img.shields.io/github/last-commit/etuzon/Python-NRT-Logging?style=plastic)
-[![DeepSource](https://deepsource.io/gh/etuzon/Python-NRT-Logging.svg/?label=active+issues&token=3pUgM1IEwZG6Gpuc065dKDxM)](https://deepsource.io/gh/etuzon/Python-NRT-Logging/?ref=repository-badge)
+[![Coverage Status](https://coveralls.io/repos/github/etuzon/nrt-logging/badge.svg)](https://coveralls.io/github/etuzon/pytohn-nrt-logging)
+![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/etuzon/python-nrt-logging?style=plastic)
+![GitHub last commit](https://img.shields.io/github/last-commit/etuzon/python-nrt-logging?style=plastic)
+[![DeepSource](https://deepsource.io/gh/etuzon/python-nrt-logging.svg/?label=active+issues&token=3pUgM1IEwZG6Gpuc065dKDxM)](https://deepsource.io/gh/etuzon/python-nrt-logging/?ref=repository-badge)
 
 Hierarchical logging help to group logs that are related to the same code flow.
 
 Log style can be styled in Yaml format or in Line format.
 
 ### Examples:
```

### Comparing `nrt-logging-1.3.3/nrt_logging/config.py` & `nrt-logging-1.3.4/nrt_logging/config.py`

 * *Files identical despite different names*

### Comparing `nrt-logging-1.3.3/nrt_logging/log_format.py` & `nrt-logging-1.3.4/nrt_logging/log_format.py`

 * *Files identical despite different names*

### Comparing `nrt-logging-1.3.3/nrt_logging/log_level.py` & `nrt-logging-1.3.4/nrt_logging/log_level.py`

 * *Files identical despite different names*

### Comparing `nrt-logging-1.3.3/nrt_logging/logger.py` & `nrt-logging-1.3.4/nrt_logging/logger.py`

 * *Files identical despite different names*

### Comparing `nrt-logging-1.3.3/nrt_logging/logger_manager.py` & `nrt-logging-1.3.4/nrt_logging/logger_manager.py`

 * *Files identical despite different names*

### Comparing `nrt-logging-1.3.3/nrt_logging/logger_stream_handlers.py` & `nrt-logging-1.3.4/nrt_logging/logger_stream_handlers.py`

 * *Files identical despite different names*

### Comparing `nrt-logging-1.3.3/nrt_logging.egg-info/PKG-INFO` & `nrt-logging-1.3.4/nrt_logging.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrt-logging
-Version: 1.3.3
+Version: 1.3.4
 Summary: Hierarchical logging in yaml format
 Home-page: https://github.com/etuzon/Python-NRT-Logging
 Author: Eyal Tuzon
 Author-email: Eyal Tuzon <eyal.tuzon.dev@gmail.com>
 Project-URL: Homepage, https://github.com/etuzon/Python-NRT-Logging
 Project-URL: Bug Tracker, https://github.com/etuzon/Python-NRT-Logging/issues
 Project-URL: documentation, https://github.com/etuzon/Python-NRT-Logging/wiki
@@ -22,18 +22,18 @@
 # Hierarchical logging in yaml format.
 
 ![PyPI](https://img.shields.io/pypi/v/nrt-logging?color=blueviolet&style=plastic)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nrt-logging?color=greens&style=plastic)
 ![PyPI - License](https://img.shields.io/pypi/l/nrt-logging?color=blue&style=plastic)
 ![PyPI - Downloads](https://img.shields.io/pypi/dd/nrt-logging?style=plastic)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/nrt-logging?color=yellow&style=plastic)
-[![Coverage Status](https://coveralls.io/repos/github/etuzon/Python-NRT-Logging/badge.svg)](https://coveralls.io/github/etuzon/Python-NRT-Logging)
-![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/etuzon/Python-NRT-Logging?style=plastic)
-![GitHub last commit](https://img.shields.io/github/last-commit/etuzon/Python-NRT-Logging?style=plastic)
-[![DeepSource](https://deepsource.io/gh/etuzon/Python-NRT-Logging.svg/?label=active+issues&token=3pUgM1IEwZG6Gpuc065dKDxM)](https://deepsource.io/gh/etuzon/Python-NRT-Logging/?ref=repository-badge)
+[![Coverage Status](https://coveralls.io/repos/github/etuzon/nrt-logging/badge.svg)](https://coveralls.io/github/etuzon/pytohn-nrt-logging)
+![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/etuzon/python-nrt-logging?style=plastic)
+![GitHub last commit](https://img.shields.io/github/last-commit/etuzon/python-nrt-logging?style=plastic)
+[![DeepSource](https://deepsource.io/gh/etuzon/python-nrt-logging.svg/?label=active+issues&token=3pUgM1IEwZG6Gpuc065dKDxM)](https://deepsource.io/gh/etuzon/python-nrt-logging/?ref=repository-badge)
 
 Hierarchical logging help to group logs that are related to the same code flow.
 
 Log style can be styled in Yaml format or in Line format.
 
 ### Examples:
```

### Comparing `nrt-logging-1.3.3/pyproject.toml` & `nrt-logging-1.3.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name='nrt-logging'
-version='1.3.3'
+version='1.3.4'
 authors=[
 { name='Eyal Tuzon', email='eyal.tuzon.dev@gmail.com' },
 ]
 description='Hierarchical logging in yaml format'
 keywords=[
 'python', 'python3', 'python-3', 'logging', 'logger', 'log', 'loggers',
 'hierarchical', 'logging-library', 'logging-framework', 'hierarchy', 'yaml',
```

### Comparing `nrt-logging-1.3.3/setup.py` & `nrt-logging-1.3.4/setup.py`

 * *Files identical despite different names*

