# Comparing `tmp/pyrestyle-0.0.6.tar.gz` & `tmp/pyrestyle-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrestyle-0.0.6.tar", last modified: Mon Jun 19 11:38:24 2023, max compression
+gzip compressed data, was "pyrestyle-0.0.7.tar", last modified: Mon Jun 19 11:46:37 2023, max compression
```

## Comparing `pyrestyle-0.0.6.tar` & `pyrestyle-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-19 11:38:24.367753 pyrestyle-0.0.6/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1324 2023-06-18 12:32:26.000000 pyrestyle-0.0.6/LICENSE
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      937 2023-06-19 11:38:24.367091 pyrestyle-0.0.6/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:39:22.000000 pyrestyle-0.0.6/README.rst
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-19 11:38:24.365959 pyrestyle-0.0.6/pyrestyle.egg-info/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      937 2023-06-19 11:38:24.000000 pyrestyle-0.0.6/pyrestyle.egg-info/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      240 2023-06-19 11:38:24.000000 pyrestyle-0.0.6/pyrestyle.egg-info/SOURCES.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-19 11:38:24.000000 pyrestyle-0.0.6/pyrestyle.egg-info/dependency_links.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       46 2023-06-19 11:38:24.000000 pyrestyle-0.0.6/pyrestyle.egg-info/entry_points.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 13:18:03.000000 pyrestyle-0.0.6/pyrestyle.egg-info/not-zip-safe
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       10 2023-06-19 11:38:24.000000 pyrestyle-0.0.6/pyrestyle.egg-info/top_level.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)   107905 2023-06-19 11:37:19.000000 pyrestyle-0.0.6/pyrestyle.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-19 11:38:24.367975 pyrestyle-0.0.6/setup.cfg
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1701 2023-06-18 13:14:10.000000 pyrestyle-0.0.6/setup.py
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-19 11:46:37.292682 pyrestyle-0.0.7/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1324 2023-06-18 12:32:26.000000 pyrestyle-0.0.7/LICENSE
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      937 2023-06-19 11:46:37.292101 pyrestyle-0.0.7/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:39:22.000000 pyrestyle-0.0.7/README.rst
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-19 11:46:37.291350 pyrestyle-0.0.7/pyrestyle.egg-info/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      937 2023-06-19 11:46:37.000000 pyrestyle-0.0.7/pyrestyle.egg-info/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      240 2023-06-19 11:46:37.000000 pyrestyle-0.0.7/pyrestyle.egg-info/SOURCES.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-19 11:46:37.000000 pyrestyle-0.0.7/pyrestyle.egg-info/dependency_links.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       46 2023-06-19 11:46:37.000000 pyrestyle-0.0.7/pyrestyle.egg-info/entry_points.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-19 11:46:37.000000 pyrestyle-0.0.7/pyrestyle.egg-info/not-zip-safe
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       10 2023-06-19 11:46:37.000000 pyrestyle-0.0.7/pyrestyle.egg-info/top_level.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)   107905 2023-06-19 11:46:17.000000 pyrestyle-0.0.7/pyrestyle.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-19 11:46:37.292897 pyrestyle-0.0.7/setup.cfg
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1784 2023-06-19 11:45:49.000000 pyrestyle-0.0.7/setup.py
```

### Comparing `pyrestyle-0.0.6/LICENSE` & `pyrestyle-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrestyle-0.0.6/PKG-INFO` & `pyrestyle-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrestyle
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python style guide checker and This project based on pycodestyle
 Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08/blob/main/pyrestyle.py
 Author: Johann C. Rocholl, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: Expat license
 Keywords: pyrestyle,pep8,PEP 8,PEP-8,PEP8
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyrestyle-0.0.6/pyrestyle.egg-info/PKG-INFO` & `pyrestyle-0.0.7/pyrestyle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrestyle
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python style guide checker and This project based on pycodestyle
 Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08/blob/main/pyrestyle.py
 Author: Johann C. Rocholl, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: Expat license
 Keywords: pyrestyle,pep8,PEP 8,PEP-8,PEP8
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyrestyle-0.0.6/pyrestyle.py` & `pyrestyle-0.0.7/pyrestyle.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 # this is a performance hack.  see https://bugs.python.org/issue43014
 if (
         sys.version_info < (3, 10) and
         callable(getattr(tokenize, '_compile', None))
 ):  # pragma: no cover (<py310)
     tokenize._compile = lru_cache()(tokenize._compile)  # type: ignore
 
-__version__ = '0.0.6'
+__version__ = '0.0.7'
 
 DEFAULT_EXCLUDE = '.svn,CVS,.bzr,.hg,.git,__pycache__,.tox'
 DEFAULT_IGNORE = 'E121,E123,E126,E226,E24,E704,W503,W504'
 try:
     if sys.platform == 'win32':
         USER_CONFIG = os.path.expanduser(r'~\.pycodestyle')
     else:
```

### Comparing `pyrestyle-0.0.6/setup.py` & `pyrestyle-0.0.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 
 """Setup for pyrestyle."""
 import io
 from setuptools import setup
 
 # read the contents of your README file
 
+INSTALL_REQUIRES = (
+    ['tabulate >= 0.9.0', 'tomli; python_version < "3.11"']
+)
 
 def get_version():
     with open('pyrestyle.py') as f:
         for line in f:
             if line.startswith('__version__'):
                 return eval(line.split('=')[-1])
```

