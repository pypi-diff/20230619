# Comparing `tmp/Flask Packer-2.1.5.tar.gz` & `tmp/Flask Packer-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask Packer-2.1.5.tar", last modified: Thu May  4 13:14:12 2023, max compression
+gzip compressed data, was "Flask Packer-2.1.6.tar", last modified: Mon Jun 19 16:53:02 2023, max compression
```

## Comparing `Flask Packer-2.1.5.tar` & `Flask Packer-2.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:14:12.015387 Flask Packer-2.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:14:12.015387 Flask Packer-2.1.5/Flask_Packer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-04 13:14:11.000000 Flask Packer-2.1.5/Flask_Packer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-04 13:14:11.000000 Flask Packer-2.1.5/Flask_Packer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:14:11.000000 Flask Packer-2.1.5/Flask_Packer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-04 13:14:11.000000 Flask Packer-2.1.5/Flask_Packer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 13:14:11.000000 Flask Packer-2.1.5/Flask_Packer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 13:13:57.000000 Flask Packer-2.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-04 13:14:12.015387 Flask Packer-2.1.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:14:12.015387 Flask Packer-2.1.5/flask_packer/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 13:13:57.000000 Flask Packer-2.1.5/flask_packer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-04 13:13:57.000000 Flask Packer-2.1.5/flask_packer/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-04 13:13:57.000000 Flask Packer-2.1.5/flask_packer/_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-04 13:13:57.000000 Flask Packer-2.1.5/flask_packer/_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:14:12.015387 Flask Packer-2.1.5/flask_packer/tags/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-04 13:13:57.000000 Flask Packer-2.1.5/flask_packer/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-04 13:13:57.000000 Flask Packer-2.1.5/flask_packer/tags/css.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-04 13:13:57.000000 Flask Packer-2.1.5/flask_packer/tags/js.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-04 13:14:12.015387 Flask Packer-2.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-04 13:13:57.000000 Flask Packer-2.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:53:02.687064 Flask Packer-2.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:53:02.687064 Flask Packer-2.1.6/Flask_Packer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-19 16:53:02.000000 Flask Packer-2.1.6/Flask_Packer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-19 16:53:02.000000 Flask Packer-2.1.6/Flask_Packer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:53:02.000000 Flask Packer-2.1.6/Flask_Packer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-19 16:53:02.000000 Flask Packer-2.1.6/Flask_Packer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-19 16:53:02.000000 Flask Packer-2.1.6/Flask_Packer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-19 16:52:48.000000 Flask Packer-2.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-19 16:53:02.687064 Flask Packer-2.1.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:53:02.687064 Flask Packer-2.1.6/flask_packer/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-19 16:52:48.000000 Flask Packer-2.1.6/flask_packer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-19 16:52:48.000000 Flask Packer-2.1.6/flask_packer/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-19 16:52:48.000000 Flask Packer-2.1.6/flask_packer/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-06-19 16:52:48.000000 Flask Packer-2.1.6/flask_packer/_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:53:02.687064 Flask Packer-2.1.6/flask_packer/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-19 16:52:48.000000 Flask Packer-2.1.6/flask_packer/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-19 16:52:48.000000 Flask Packer-2.1.6/flask_packer/tags/css.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-19 16:52:48.000000 Flask Packer-2.1.6/flask_packer/tags/js.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-19 16:53:02.687064 Flask Packer-2.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-19 16:52:48.000000 Flask Packer-2.1.6/setup.py
```

### Comparing `Flask Packer-2.1.5/Flask_Packer.egg-info/PKG-INFO` & `Flask Packer-2.1.6/Flask_Packer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: Flask-Packer
-Version: 2.1.5
+Version: 2.1.6
 Summary: A Flask extension to bundle and compress CSS and JS files.
 Home-page: https://github.com/stan5079/flask-packer
 Author: H.P. Mertens
 Author-email: stnmertens@gmail.com
 License: GNU General Public License v3.0
 Keywords: flask,packer,static,compress,bundle,minify,combine
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Build Tools
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 License-File: LICENSE
```

### Comparing `Flask Packer-2.1.5/LICENSE` & `Flask Packer-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask Packer-2.1.5/PKG-INFO` & `Flask Packer-2.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: Flask Packer
-Version: 2.1.5
+Version: 2.1.6
 Summary: A Flask extension to bundle and compress CSS and JS files.
 Home-page: https://github.com/stan5079/flask-packer
 Author: H.P. Mertens
 Author-email: stnmertens@gmail.com
 License: GNU General Public License v3.0
 Keywords: flask,packer,static,compress,bundle,minify,combine
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Build Tools
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 License-File: LICENSE
```

### Comparing `Flask Packer-2.1.5/flask_packer/_base.py` & `Flask Packer-2.1.6/flask_packer/_base.py`

 * *Files identical despite different names*

### Comparing `Flask Packer-2.1.5/flask_packer/_extension.py` & `Flask Packer-2.1.6/flask_packer/_extension.py`

 * *Files identical despite different names*

### Comparing `Flask Packer-2.1.5/flask_packer/tags/css.py` & `Flask Packer-2.1.6/flask_packer/tags/css.py`

 * *Files identical despite different names*

### Comparing `Flask Packer-2.1.5/flask_packer/tags/js.py` & `Flask Packer-2.1.6/flask_packer/tags/js.py`

 * *Files identical despite different names*

### Comparing `Flask Packer-2.1.5/setup.py` & `Flask Packer-2.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,11 +22,11 @@
     ],
     description="A Flask extension to bundle and compress CSS and JS files.",
     install_requires=find_requirements(),
     keywords=["flask", "packer", "static", "compress", "bundle", "minify", "combine"],
     license="GNU General Public License v3.0",
     name="Flask Packer",
     packages=find_packages(),
-    python_requires=">=3.10",
+    python_requires=">=3.11",
     url="https://github.com/stan5079/flask-packer",
     version=__version__,
 )
```

