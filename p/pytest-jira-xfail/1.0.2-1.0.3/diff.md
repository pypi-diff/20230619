# Comparing `tmp/pytest-jira-xfail-1.0.2.tar.gz` & `tmp/pytest-jira-xfail-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-jira-xfail-1.0.2.tar", last modified: Wed Jun 14 12:09:25 2023, max compression
+gzip compressed data, was "pytest-jira-xfail-1.0.3.tar", last modified: Mon Jun 19 15:20:22 2023, max compression
```

## Comparing `pytest-jira-xfail-1.0.2.tar` & `pytest-jira-xfail-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:09:25.523127 pytest-jira-xfail-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-14 12:09:14.000000 pytest-jira-xfail-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-14 12:09:25.523127 pytest-jira-xfail-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-14 12:09:14.000000 pytest-jira-xfail-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:09:25.523127 pytest-jira-xfail-1.0.2/pytest_jira_xfail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:09:14.000000 pytest-jira-xfail-1.0.2/pytest_jira_xfail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-14 12:09:14.000000 pytest-jira-xfail-1.0.2/pytest_jira_xfail/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-14 12:09:14.000000 pytest-jira-xfail-1.0.2/pytest_jira_xfail/jira_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:09:25.523127 pytest-jira-xfail-1.0.2/pytest_jira_xfail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-14 12:09:25.000000 pytest-jira-xfail-1.0.2/pytest_jira_xfail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-14 12:09:25.000000 pytest-jira-xfail-1.0.2/pytest_jira_xfail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:09:25.000000 pytest-jira-xfail-1.0.2/pytest_jira_xfail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-14 12:09:25.000000 pytest-jira-xfail-1.0.2/pytest_jira_xfail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-14 12:09:25.000000 pytest-jira-xfail-1.0.2/pytest_jira_xfail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 12:09:25.523127 pytest-jira-xfail-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-14 12:09:14.000000 pytest-jira-xfail-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:20:22.422586 pytest-jira-xfail-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-19 15:20:07.000000 pytest-jira-xfail-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-19 15:20:22.422586 pytest-jira-xfail-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-19 15:20:07.000000 pytest-jira-xfail-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:20:22.422586 pytest-jira-xfail-1.0.3/pytest_jira_xfail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:20:07.000000 pytest-jira-xfail-1.0.3/pytest_jira_xfail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-19 15:20:07.000000 pytest-jira-xfail-1.0.3/pytest_jira_xfail/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-19 15:20:07.000000 pytest-jira-xfail-1.0.3/pytest_jira_xfail/jira_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:20:22.422586 pytest-jira-xfail-1.0.3/pytest_jira_xfail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-19 15:20:22.000000 pytest-jira-xfail-1.0.3/pytest_jira_xfail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-19 15:20:22.000000 pytest-jira-xfail-1.0.3/pytest_jira_xfail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:20:22.000000 pytest-jira-xfail-1.0.3/pytest_jira_xfail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-19 15:20:22.000000 pytest-jira-xfail-1.0.3/pytest_jira_xfail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 15:20:22.000000 pytest-jira-xfail-1.0.3/pytest_jira_xfail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 15:20:22.422586 pytest-jira-xfail-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-19 15:20:07.000000 pytest-jira-xfail-1.0.3/setup.py
```

### Comparing `pytest-jira-xfail-1.0.2/LICENSE` & `pytest-jira-xfail-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-jira-xfail-1.0.2/PKG-INFO` & `pytest-jira-xfail-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-jira-xfail
-Version: 1.0.2
+Version: 1.0.3
 Summary: Plugin skips (xfail) tests if unresolved Jira issue(s) linked
 Home-page: https://github.com/JamalZeynalov/pytest-jira-xfail
 Author: Jamal Zeinalov
 Author-email: jamal.zeynalov@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytest-jira-xfail-1.0.2/README.md` & `pytest-jira-xfail-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pytest-jira-xfail-1.0.2/pytest_jira_xfail/annotations.py` & `pytest-jira-xfail-1.0.3/pytest_jira_xfail/annotations.py`

 * *Files identical despite different names*

### Comparing `pytest-jira-xfail-1.0.2/pytest_jira_xfail/jira_helper.py` & `pytest-jira-xfail-1.0.3/pytest_jira_xfail/jira_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pytest
 from _pytest.mark import Mark
 from jira import JIRA
 from singleton_decorator import singleton
 from selenium.common.exceptions import *
 from requests import *
+from playwright._impl._api_types import *
 
 
 @singleton
 class PytestJiraHelper:
     def __init__(
         self,
         jira_url: str,
```

### Comparing `pytest-jira-xfail-1.0.2/pytest_jira_xfail.egg-info/PKG-INFO` & `pytest-jira-xfail-1.0.3/pytest_jira_xfail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-jira-xfail
-Version: 1.0.2
+Version: 1.0.3
 Summary: Plugin skips (xfail) tests if unresolved Jira issue(s) linked
 Home-page: https://github.com/JamalZeynalov/pytest-jira-xfail
 Author: Jamal Zeinalov
 Author-email: jamal.zeynalov@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytest-jira-xfail-1.0.2/setup.py` & `pytest-jira-xfail-1.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="pytest-jira-xfail",
-    version="1.0.2",
+    version="1.0.3",
     author="Jamal Zeinalov",
     author_email="jamal.zeynalov@gmail.com",
     description='Plugin skips (xfail) tests if unresolved Jira issue(s) linked',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JamalZeynalov/pytest-jira-xfail",
     packages=find_packages(),
@@ -22,10 +22,11 @@
         "pytest>=7.2.0",
         "requests>=2.28.1",
         "setuptools>=65.5.1",
         "jira>=3.4.1",
         "singleton-decorator>=1.0.0",
         "allure-pytest>=2.11.1",
         "selenium>=4.6.0",
+        "pytest-playwright>=0.3.3",
     ],
     python_requires=">=3.9",
 )
```

