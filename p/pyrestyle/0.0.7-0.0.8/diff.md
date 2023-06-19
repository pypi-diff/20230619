# Comparing `tmp/pyrestyle-0.0.7.tar.gz` & `tmp/pyrestyle-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrestyle-0.0.7.tar", last modified: Mon Jun 19 11:46:37 2023, max compression
+gzip compressed data, was "pyrestyle-0.0.8.tar", last modified: Mon Jun 19 12:06:14 2023, max compression
```

## Comparing `pyrestyle-0.0.7.tar` & `pyrestyle-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-19 11:46:37.292682 pyrestyle-0.0.7/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1324 2023-06-18 12:32:26.000000 pyrestyle-0.0.7/LICENSE
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      937 2023-06-19 11:46:37.292101 pyrestyle-0.0.7/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:39:22.000000 pyrestyle-0.0.7/README.rst
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-19 11:46:37.291350 pyrestyle-0.0.7/pyrestyle.egg-info/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      937 2023-06-19 11:46:37.000000 pyrestyle-0.0.7/pyrestyle.egg-info/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      240 2023-06-19 11:46:37.000000 pyrestyle-0.0.7/pyrestyle.egg-info/SOURCES.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-19 11:46:37.000000 pyrestyle-0.0.7/pyrestyle.egg-info/dependency_links.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       46 2023-06-19 11:46:37.000000 pyrestyle-0.0.7/pyrestyle.egg-info/entry_points.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-19 11:46:37.000000 pyrestyle-0.0.7/pyrestyle.egg-info/not-zip-safe
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       10 2023-06-19 11:46:37.000000 pyrestyle-0.0.7/pyrestyle.egg-info/top_level.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)   107905 2023-06-19 11:46:17.000000 pyrestyle-0.0.7/pyrestyle.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-19 11:46:37.292897 pyrestyle-0.0.7/setup.cfg
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1784 2023-06-19 11:45:49.000000 pyrestyle-0.0.7/setup.py
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-19 12:06:14.834952 pyrestyle-0.0.8/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1324 2023-06-18 12:32:26.000000 pyrestyle-0.0.8/LICENSE
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      937 2023-06-19 12:06:14.834476 pyrestyle-0.0.8/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:39:22.000000 pyrestyle-0.0.8/README.rst
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      119 2023-06-19 12:02:29.000000 pyrestyle-0.0.8/pyproject.toml
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-19 12:06:14.833636 pyrestyle-0.0.8/pyrestyle.egg-info/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      937 2023-06-19 12:06:14.000000 pyrestyle-0.0.8/pyrestyle.egg-info/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      255 2023-06-19 12:06:14.000000 pyrestyle-0.0.8/pyrestyle.egg-info/SOURCES.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-19 12:06:14.000000 pyrestyle-0.0.8/pyrestyle.egg-info/dependency_links.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       46 2023-06-19 12:06:14.000000 pyrestyle-0.0.8/pyrestyle.egg-info/entry_points.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-19 12:06:14.000000 pyrestyle-0.0.8/pyrestyle.egg-info/not-zip-safe
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       10 2023-06-19 12:06:14.000000 pyrestyle-0.0.8/pyrestyle.egg-info/top_level.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)   107905 2023-06-19 12:03:18.000000 pyrestyle-0.0.8/pyrestyle.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-19 12:06:14.835101 pyrestyle-0.0.8/setup.cfg
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1784 2023-06-19 11:53:19.000000 pyrestyle-0.0.8/setup.py
```

### Comparing `pyrestyle-0.0.7/LICENSE` & `pyrestyle-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrestyle-0.0.7/PKG-INFO` & `pyrestyle-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrestyle
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python style guide checker and This project based on pycodestyle
 Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08/blob/main/pyrestyle.py
 Author: Johann C. Rocholl, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: Expat license
 Keywords: pyrestyle,pep8,PEP 8,PEP-8,PEP8
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyrestyle-0.0.7/pyrestyle.egg-info/PKG-INFO` & `pyrestyle-0.0.8/pyrestyle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrestyle
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python style guide checker and This project based on pycodestyle
 Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08/blob/main/pyrestyle.py
 Author: Johann C. Rocholl, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: Expat license
 Keywords: pyrestyle,pep8,PEP 8,PEP-8,PEP8
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyrestyle-0.0.7/pyrestyle.py` & `pyrestyle-0.0.8/pyrestyle.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 # this is a performance hack.  see https://bugs.python.org/issue43014
 if (
         sys.version_info < (3, 10) and
         callable(getattr(tokenize, '_compile', None))
 ):  # pragma: no cover (<py310)
     tokenize._compile = lru_cache()(tokenize._compile)  # type: ignore
 
-__version__ = '0.0.7'
+__version__ = '0.0.8'
 
 DEFAULT_EXCLUDE = '.svn,CVS,.bzr,.hg,.git,__pycache__,.tox'
 DEFAULT_IGNORE = 'E121,E123,E126,E226,E24,E704,W503,W504'
 try:
     if sys.platform == 'win32':
         USER_CONFIG = os.path.expanduser(r'~\.pycodestyle')
     else:
```

### Comparing `pyrestyle-0.0.7/setup.py` & `pyrestyle-0.0.8/setup.py`

 * *Files identical despite different names*

