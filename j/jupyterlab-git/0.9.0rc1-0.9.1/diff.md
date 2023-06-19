# Comparing `tmp/jupyterlab_git-0.9.0rc1.tar.gz` & `tmp/jupyterlab_git-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jupyterlab_git-0.9.0rc1.tar", last modified: Wed Dec  4 20:41:57 2019, max compression
+gzip compressed data, was "dist/jupyterlab_git-0.9.1.tar", last modified: Tue Mar 24 16:43:09 2020, max compression
```

## Comparing `jupyterlab_git-0.9.0rc1.tar` & `jupyterlab_git-0.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 tel        (501) staff       (20)        0 2019-12-04 20:41:57.000000 jupyterlab_git-0.9.0rc1/
--rw-r--r--   0 tel        (501) staff       (20)     1528 2019-12-04 15:52:46.000000 jupyterlab_git-0.9.0rc1/LICENSE
--rw-r--r--   0 tel        (501) staff       (20)     5084 2019-12-04 20:41:57.000000 jupyterlab_git-0.9.0rc1/PKG-INFO
--rw-r--r--   0 tel        (501) staff       (20)     3514 2019-12-03 16:26:11.000000 jupyterlab_git-0.9.0rc1/README.md
-drwxr-xr-x   0 tel        (501) staff       (20)        0 2019-12-04 20:41:57.000000 jupyterlab_git-0.9.0rc1/jupyter-config/
-drwxr-xr-x   0 tel        (501) staff       (20)        0 2019-12-04 20:41:57.000000 jupyterlab_git-0.9.0rc1/jupyter-config/jupyter_notebook_config.d/
--rw-r--r--   0 tel        (501) staff       (20)      102 2019-10-15 06:12:10.000000 jupyterlab_git-0.9.0rc1/jupyter-config/jupyter_notebook_config.d/jupyterlab_git.json
-drwxr-xr-x   0 tel        (501) staff       (20)        0 2019-12-04 20:41:57.000000 jupyterlab_git-0.9.0rc1/jupyterlab_git/
--rw-r--r--   0 tel        (501) staff       (20)      680 2019-09-12 23:02:28.000000 jupyterlab_git-0.9.0rc1/jupyterlab_git/__init__.py
--rw-r--r--   0 tel        (501) staff       (20)      186 2019-12-04 20:28:41.000000 jupyterlab_git-0.9.0rc1/jupyterlab_git/_version.py
--rw-r--r--   0 tel        (501) staff       (20)    32748 2019-12-04 20:29:06.000000 jupyterlab_git-0.9.0rc1/jupyterlab_git/git.py
--rw-r--r--   0 tel        (501) staff       (20)    15678 2019-11-25 17:37:59.000000 jupyterlab_git-0.9.0rc1/jupyterlab_git/handlers.py
-drwxr-xr-x   0 tel        (501) staff       (20)        0 2019-12-04 20:41:57.000000 jupyterlab_git-0.9.0rc1/jupyterlab_git/labextension/
--rw-r--r--   0 tel        (501) staff       (20)   120392 2019-12-04 20:41:50.000000 jupyterlab_git-0.9.0rc1/jupyterlab_git/labextension/jupyterlab-git-0.9.0-rc.1.tgz
-drwxr-xr-x   0 tel        (501) staff       (20)        0 2019-12-04 20:41:57.000000 jupyterlab_git-0.9.0rc1/jupyterlab_git/tests/
--rw-r--r--   0 tel        (501) staff       (20)        0 2019-10-15 06:12:10.000000 jupyterlab_git-0.9.0rc1/jupyterlab_git/tests/__init__.py
--rw-r--r--   0 tel        (501) staff       (20)    28465 2019-12-03 16:26:11.000000 jupyterlab_git-0.9.0rc1/jupyterlab_git/tests/test_branch.py
--rw-r--r--   0 tel        (501) staff       (20)     5565 2019-10-15 06:12:10.000000 jupyterlab_git-0.9.0rc1/jupyterlab_git/tests/test_clone.py
--rw-r--r--   0 tel        (501) staff       (20)     2959 2019-10-15 06:12:10.000000 jupyterlab_git-0.9.0rc1/jupyterlab_git/tests/test_config.py
--rw-r--r--   0 tel        (501) staff       (20)     2863 2019-10-20 07:31:32.000000 jupyterlab_git-0.9.0rc1/jupyterlab_git/tests/test_detailed_log.py
--rw-r--r--   0 tel        (501) staff       (20)     2848 2019-10-15 06:12:10.000000 jupyterlab_git-0.9.0rc1/jupyterlab_git/tests/test_diff.py
--rw-r--r--   0 tel        (501) staff       (20)     8478 2019-11-19 21:10:30.000000 jupyterlab_git-0.9.0rc1/jupyterlab_git/tests/test_handlers.py
--rw-r--r--   0 tel        (501) staff       (20)     7626 2019-10-15 06:12:10.000000 jupyterlab_git-0.9.0rc1/jupyterlab_git/tests/test_pushpull.py
--rw-r--r--   0 tel        (501) staff       (20)     2593 2019-12-03 16:26:11.000000 jupyterlab_git-0.9.0rc1/setup.py
--rw-r--r--   0 tel        (501) staff       (20)    21978 2019-11-27 22:20:24.000000 jupyterlab_git-0.9.0rc1/setupbase.py
+drwxr-xr-x   0 stslve   (1919889055) ANT\Domain Users (1896053708)        0 2020-03-24 16:43:09.327792 jupyterlab_git-0.9.1/
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)     1528 2020-03-24 16:15:47.219808 jupyterlab_git-0.9.1/LICENSE
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)     5081 2020-03-24 16:43:09.332265 jupyterlab_git-0.9.1/PKG-INFO
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)     3514 2020-03-24 16:16:58.420819 jupyterlab_git-0.9.1/README.md
+drwxr-xr-x   0 stslve   (1919889055) ANT\Domain Users (1896053708)        0 2020-03-24 16:43:09.310972 jupyterlab_git-0.9.1/jupyter-config/
+drwxr-xr-x   0 stslve   (1919889055) ANT\Domain Users (1896053708)        0 2020-03-24 16:43:09.318478 jupyterlab_git-0.9.1/jupyter-config/jupyter_notebook_config.d/
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)      102 2020-03-24 16:15:47.382190 jupyterlab_git-0.9.1/jupyter-config/jupyter_notebook_config.d/jupyterlab_git.json
+drwxr-xr-x   0 stslve   (1919889055) ANT\Domain Users (1896053708)        0 2020-03-24 16:43:09.321179 jupyterlab_git-0.9.1/jupyterlab_git/
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)      680 2020-03-24 16:16:58.421542 jupyterlab_git-0.9.1/jupyterlab_git/__init__.py
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)      165 2020-03-24 16:25:22.284604 jupyterlab_git-0.9.1/jupyterlab_git/_version.py
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)    32748 2020-03-24 16:16:58.423177 jupyterlab_git-0.9.1/jupyterlab_git/git.py
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)    15678 2020-03-24 16:16:58.424119 jupyterlab_git-0.9.1/jupyterlab_git/handlers.py
+drwxr-xr-x   0 stslve   (1919889055) ANT\Domain Users (1896053708)        0 2020-03-24 16:43:09.322291 jupyterlab_git-0.9.1/jupyterlab_git/labextension/
+-rw-r--r--   0 stslve   (1919889055) wheel        (0)   120388 2020-03-24 16:43:02.002777 jupyterlab_git-0.9.1/jupyterlab_git/labextension/jupyterlab-git-0.9.1.tgz
+drwxr-xr-x   0 stslve   (1919889055) ANT\Domain Users (1896053708)        0 2020-03-24 16:43:09.327600 jupyterlab_git-0.9.1/jupyterlab_git/tests/
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)        0 2020-03-24 16:15:47.384345 jupyterlab_git-0.9.1/jupyterlab_git/tests/__init__.py
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)    28465 2020-03-24 16:16:58.424842 jupyterlab_git-0.9.1/jupyterlab_git/tests/test_branch.py
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)     5565 2020-03-24 16:16:58.425451 jupyterlab_git-0.9.1/jupyterlab_git/tests/test_clone.py
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)     2959 2020-03-24 16:16:58.425982 jupyterlab_git-0.9.1/jupyterlab_git/tests/test_config.py
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)     2863 2020-03-24 16:16:58.426469 jupyterlab_git-0.9.1/jupyterlab_git/tests/test_detailed_log.py
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)     2848 2020-03-24 16:16:58.426949 jupyterlab_git-0.9.1/jupyterlab_git/tests/test_diff.py
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)     8478 2020-03-24 16:16:58.427496 jupyterlab_git-0.9.1/jupyterlab_git/tests/test_handlers.py
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)     7626 2020-03-24 16:16:58.428214 jupyterlab_git-0.9.1/jupyterlab_git/tests/test_pushpull.py
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)     2602 2020-03-24 16:18:59.048821 jupyterlab_git-0.9.1/setup.py
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)    21978 2020-03-24 16:15:47.391018 jupyterlab_git-0.9.1/setupbase.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jupyterlab_git-0.9.0rc1/LICENSE` & `jupyterlab_git-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_git-0.9.0rc1/PKG-INFO` & `jupyterlab_git-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_git
-Version: 0.9.0rc1
+Version: 0.9.1
 Summary: A server extension for JupyterLab's git extension
 Home-page: https://github.com/jupyterlab/jupyterlab-git
 Author: Jupyter Development Team
 License: BSD
 Description: # jupyterlab-git
         
         [![Binder](https://beta.mybinder.org/badge.svg)](https://mybinder.org/v2/gh/jupyterlab/jupyterlab-git/master?urlpath=lab) [![Build Status](https://travis-ci.org/jupyterlab/jupyterlab-git.svg?branch=master)](https://travis-ci.org/jupyterlab/jupyterlab-git) [![Version](https://img.shields.io/npm/v/@jupyterlab/git.svg)](https://www.npmjs.com/package/@jupyterlab/git) [![Version](https://img.shields.io/pypi/v/jupyterlab-git.svg)](https://pypi.org/project/jupyterlab-git/) [![Downloads](https://img.shields.io/npm/dm/@jupyterlab/git.svg)](https://www.npmjs.com/package/@jupyterlab/git) [![Version](https://img.shields.io/conda/vn/conda-forge/jupyterlab-git.svg)](https://anaconda.org/conda-forge/jupyterlab-git) [![Downloads](https://img.shields.io/conda/dn/conda-forge/jupyterlab-git.svg)](https://anaconda.org/conda-forge/jupyterlab-git)
```

### Comparing `jupyterlab_git-0.9.0rc1/README.md` & `jupyterlab_git-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_git-0.9.0rc1/jupyterlab_git/__init__.py` & `jupyterlab_git-0.9.1/jupyterlab_git/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_git-0.9.0rc1/jupyterlab_git/git.py` & `jupyterlab_git-0.9.1/jupyterlab_git/git.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_git-0.9.0rc1/jupyterlab_git/handlers.py` & `jupyterlab_git-0.9.1/jupyterlab_git/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_git-0.9.0rc1/jupyterlab_git/tests/test_branch.py` & `jupyterlab_git-0.9.1/jupyterlab_git/tests/test_branch.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_git-0.9.0rc1/jupyterlab_git/tests/test_clone.py` & `jupyterlab_git-0.9.1/jupyterlab_git/tests/test_clone.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_git-0.9.0rc1/jupyterlab_git/tests/test_config.py` & `jupyterlab_git-0.9.1/jupyterlab_git/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_git-0.9.0rc1/jupyterlab_git/tests/test_detailed_log.py` & `jupyterlab_git-0.9.1/jupyterlab_git/tests/test_detailed_log.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_git-0.9.0rc1/jupyterlab_git/tests/test_diff.py` & `jupyterlab_git-0.9.1/jupyterlab_git/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_git-0.9.0rc1/jupyterlab_git/tests/test_handlers.py` & `jupyterlab_git-0.9.1/jupyterlab_git/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_git-0.9.0rc1/jupyterlab_git/tests/test_pushpull.py` & `jupyterlab_git-0.9.1/jupyterlab_git/tests/test_pushpull.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_git-0.9.0rc1/setup.py` & `jupyterlab_git-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Framework :: Jupyter',
     ],
     install_requires = [
         'notebook',
-        'nbdime >= 1.1.0',
+        'nbdime >= 1.1.0, < 2.0.0',
         'pexpect'
     ],
     extras_require = {
         'test': [
             'pytest',
             'jupyterlab~=1.1',
         ],
```

### Comparing `jupyterlab_git-0.9.0rc1/setupbase.py` & `jupyterlab_git-0.9.1/setupbase.py`

 * *Files identical despite different names*

