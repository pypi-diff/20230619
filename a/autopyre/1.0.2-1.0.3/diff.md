# Comparing `tmp/autopyre-1.0.2.tar.gz` & `tmp/autopyre-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopyre-1.0.2.tar", last modified: Mon Jun 19 12:03:58 2023, max compression
+gzip compressed data, was "autopyre-1.0.3.tar", last modified: Mon Jun 19 12:05:00 2023, max compression
```

## Comparing `autopyre-1.0.2.tar` & `autopyre-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-19 12:03:58.625499 autopyre-1.0.2/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1250 2023-06-18 12:46:39.000000 autopyre-1.0.2/LICENSE
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-19 12:03:58.624659 autopyre-1.0.2/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:48:08.000000 autopyre-1.0.2/README.rst
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-19 12:03:58.623387 autopyre-1.0.2/autopyre.egg-info/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-19 12:03:58.000000 autopyre-1.0.2/autopyre.egg-info/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      264 2023-06-19 12:03:58.000000 autopyre-1.0.2/autopyre.egg-info/SOURCES.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-19 12:03:58.000000 autopyre-1.0.2/autopyre.egg-info/dependency_links.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       43 2023-06-19 12:03:58.000000 autopyre-1.0.2/autopyre.egg-info/entry_points.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-19 12:03:58.000000 autopyre-1.0.2/autopyre.egg-info/not-zip-safe
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       51 2023-06-19 12:03:58.000000 autopyre-1.0.2/autopyre.egg-info/requires.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        9 2023-06-19 12:03:58.000000 autopyre-1.0.2/autopyre.egg-info/top_level.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)   192441 2023-06-19 12:03:39.000000 autopyre-1.0.2/autopyre.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-19 12:03:58.625710 autopyre-1.0.2/setup.cfg
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     2098 2023-06-19 11:49:20.000000 autopyre-1.0.2/setup.py
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-19 12:05:00.941667 autopyre-1.0.3/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1250 2023-06-18 12:46:39.000000 autopyre-1.0.3/LICENSE
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-19 12:05:00.939970 autopyre-1.0.3/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:48:08.000000 autopyre-1.0.3/README.rst
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-19 12:05:00.936236 autopyre-1.0.3/autopyre.egg-info/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-19 12:05:00.000000 autopyre-1.0.3/autopyre.egg-info/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      264 2023-06-19 12:05:00.000000 autopyre-1.0.3/autopyre.egg-info/SOURCES.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-19 12:05:00.000000 autopyre-1.0.3/autopyre.egg-info/dependency_links.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       43 2023-06-19 12:05:00.000000 autopyre-1.0.3/autopyre.egg-info/entry_points.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-19 12:05:00.000000 autopyre-1.0.3/autopyre.egg-info/not-zip-safe
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       51 2023-06-19 12:05:00.000000 autopyre-1.0.3/autopyre.egg-info/requires.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        9 2023-06-19 12:05:00.000000 autopyre-1.0.3/autopyre.egg-info/top_level.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)   192441 2023-06-19 12:04:51.000000 autopyre-1.0.3/autopyre.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-19 12:05:00.941944 autopyre-1.0.3/setup.cfg
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     2098 2023-06-19 12:04:43.000000 autopyre-1.0.3/setup.py
```

### Comparing `autopyre-1.0.2/LICENSE` & `autopyre-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autopyre-1.0.2/PKG-INFO` & `autopyre-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopyre
-Version: 1.0.2
+Version: 1.0.3
 Summary: A tool that automatically formats Python code to conform to the PEP 8 style guide and This project based on autopep8
 Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08/autopyre.py
 Author: Hideo Hattori, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: MIT
 Keywords: automation,pep8,format,pycodestyle,autopyre,pyrestyle
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autopyre-1.0.2/autopyre.egg-info/PKG-INFO` & `autopyre-1.0.3/autopyre.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopyre
-Version: 1.0.2
+Version: 1.0.3
 Summary: A tool that automatically formats Python code to conform to the PEP 8 style guide and This project based on autopep8
 Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08/autopyre.py
 Author: Hideo Hattori, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: MIT
 Keywords: automation,pep8,format,pycodestyle,autopyre,pyrestyle
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autopyre-1.0.2/autopyre.py` & `autopyre-1.0.3/autopyre.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 import pyrestyle
 from pyrestyle import STARTSWITH_INDENT_STATEMENT_REGEX
 
 import libcst as cst  # pip install libcst
 import string
 from termcolor import colored  # pip install termcolor
 
-__version__ = '1.0.2'
+__version__ = '1.0.3'
 
 
 CR = '\r'
 LF = '\n'
 CRLF = '\r\n'
```

### Comparing `autopyre-1.0.2/setup.py` & `autopyre-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import io
 
 from setuptools import setup
 
 # read the contents of your README file
 
 INSTALL_REQUIRES = (
-    ['pyrestyle >= 0.0.7', 'tomli; python_version < "3.11"']
+    ['pyrestyle >= 0.0.8', 'tomli; python_version < "3.11"']
 )
 
 
 def version():
     """Return version string."""
     with io.open('autopyre.py') as input_file:
         for line in input_file:
```

