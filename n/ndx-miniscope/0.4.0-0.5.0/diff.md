# Comparing `tmp/ndx-miniscope-0.4.0.tar.gz` & `tmp/ndx-miniscope-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndx-miniscope-0.4.0.tar", last modified: Mon Jun 12 13:53:25 2023, max compression
+gzip compressed data, was "ndx-miniscope-0.5.0.tar", last modified: Mon Jun 19 16:41:29 2023, max compression
```

## Comparing `ndx-miniscope-0.4.0.tar` & `ndx-miniscope-0.5.0.tar`

### file list

```diff
@@ -1,39 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:53:25.741544 ndx-miniscope-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-12 13:53:25.741544 ndx-miniscope-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:53:25.737544 ndx-miniscope-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:53:25.737544 ndx-miniscope-0.4.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/docs/source/conf_doc_autogen.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/docs/source/credits.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/docs/source/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/docs/source/format.rst
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/docs/source/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 13:53:25.741544 ndx-miniscope-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:53:25.737544 ndx-miniscope-0.4.0/spec/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/spec/ndx-miniscope.extensions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/spec/ndx-miniscope.namespace.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:53:25.733544 ndx-miniscope-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:53:25.733544 ndx-miniscope-0.4.0/src/pynwb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:53:25.737544 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope/miniscope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:53:25.737544 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope/spec/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope/spec/ndx-miniscope.extensions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope/spec/ndx-miniscope.namespace.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:53:25.737544 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-12 13:53:25.000000 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-12 13:53:25.000000 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:53:25.000000 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:53:25.000000 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 13:53:25.000000 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 13:53:25.000000 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:41:29.084459 ndx-miniscope-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-19 16:41:29.084459 ndx-miniscope-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:41:29.080458 ndx-miniscope-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:41:29.080458 ndx-miniscope-0.5.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/docs/source/conf_doc_autogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/docs/source/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/docs/source/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/docs/source/format.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/docs/source/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 16:41:29.084459 ndx-miniscope-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:41:29.080458 ndx-miniscope-0.5.0/spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/spec/ndx-miniscope.extensions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/spec/ndx-miniscope.namespace.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:41:29.080458 ndx-miniscope-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:41:29.080458 ndx-miniscope-0.5.0/src/pynwb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:41:29.080458 ndx-miniscope-0.5.0/src/pynwb/ndx_miniscope/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/src/pynwb/ndx_miniscope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:41:29.080458 ndx-miniscope-0.5.0/src/pynwb/ndx_miniscope/spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/src/pynwb/ndx_miniscope/spec/ndx-miniscope.extensions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/src/pynwb/ndx_miniscope/spec/ndx-miniscope.namespace.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:41:29.084459 ndx-miniscope-0.5.0/src/pynwb/ndx_miniscope/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/src/pynwb/ndx_miniscope/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/src/pynwb/ndx_miniscope/utils/notes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/src/pynwb/ndx_miniscope/utils/nwb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/src/pynwb/ndx_miniscope/utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/src/pynwb/ndx_miniscope/utils/timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-19 16:41:21.000000 ndx-miniscope-0.5.0/src/pynwb/ndx_miniscope/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:41:29.080458 ndx-miniscope-0.5.0/src/pynwb/ndx_miniscope.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-19 16:41:29.000000 ndx-miniscope-0.5.0/src/pynwb/ndx_miniscope.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-19 16:41:29.000000 ndx-miniscope-0.5.0/src/pynwb/ndx_miniscope.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:41:29.000000 ndx-miniscope-0.5.0/src/pynwb/ndx_miniscope.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:41:29.000000 ndx-miniscope-0.5.0/src/pynwb/ndx_miniscope.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 16:41:29.000000 ndx-miniscope-0.5.0/src/pynwb/ndx_miniscope.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 16:41:29.000000 ndx-miniscope-0.5.0/src/pynwb/ndx_miniscope.egg-info/top_level.txt
```

### Comparing `ndx-miniscope-0.4.0/LICENSE.txt` & `ndx-miniscope-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ndx-miniscope-0.4.0/docs/Makefile` & `ndx-miniscope-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ndx-miniscope-0.4.0/docs/README.md` & `ndx-miniscope-0.5.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `ndx-miniscope-0.4.0/docs/make.bat` & `ndx-miniscope-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ndx-miniscope-0.4.0/docs/source/conf.py` & `ndx-miniscope-0.5.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ndx-miniscope-0.4.0/docs/source/conf_doc_autogen.py` & `ndx-miniscope-0.5.0/docs/source/conf_doc_autogen.py`

 * *Files identical despite different names*

### Comparing `ndx-miniscope-0.4.0/setup.py` & `ndx-miniscope-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     long_description = f.read()
 
 with open(path / "requirements.txt") as f:
     install_requires = f.readlines()
 
 setup_args = {
     "name": "ndx-miniscope",
-    "version": "0.4.0",
+    "version": "0.5.0",
     "description": "Represent metadata for Miniscope acquisition system.",
     "long_description": long_description,
     "long_description_content_type": "text/markdown",
     "author": "Ben Dichter",
     "author_email": "ben.dichter@catalystneuro.com",
     "url": "https://github.com/catalystneuro/ndx-miniscope",
     "license": "BSD-3",
```

### Comparing `ndx-miniscope-0.4.0/spec/ndx-miniscope.extensions.yaml` & `ndx-miniscope-0.5.0/spec/ndx-miniscope.extensions.yaml`

 * *Files identical despite different names*

### Comparing `ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope/spec/ndx-miniscope.extensions.yaml` & `ndx-miniscope-0.5.0/src/pynwb/ndx_miniscope/spec/ndx-miniscope.extensions.yaml`

 * *Files identical despite different names*

### Comparing `ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope.egg-info/SOURCES.txt` & `ndx-miniscope-0.5.0/src/pynwb/ndx_miniscope.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,16 +13,21 @@
 docs/source/description.rst
 docs/source/format.rst
 docs/source/index.rst
 docs/source/release_notes.rst
 spec/ndx-miniscope.extensions.yaml
 spec/ndx-miniscope.namespace.yaml
 src/pynwb/ndx_miniscope/__init__.py
-src/pynwb/ndx_miniscope/miniscope.py
 src/pynwb/ndx_miniscope.egg-info/PKG-INFO
 src/pynwb/ndx_miniscope.egg-info/SOURCES.txt
 src/pynwb/ndx_miniscope.egg-info/dependency_links.txt
 src/pynwb/ndx_miniscope.egg-info/not-zip-safe
 src/pynwb/ndx_miniscope.egg-info/requires.txt
 src/pynwb/ndx_miniscope.egg-info/top_level.txt
 src/pynwb/ndx_miniscope/spec/ndx-miniscope.extensions.yaml
-src/pynwb/ndx_miniscope/spec/ndx-miniscope.namespace.yaml
+src/pynwb/ndx_miniscope/spec/ndx-miniscope.namespace.yaml
+src/pynwb/ndx_miniscope/utils/__init__.py
+src/pynwb/ndx_miniscope/utils/notes.py
+src/pynwb/ndx_miniscope/utils/nwb.py
+src/pynwb/ndx_miniscope/utils/settings.py
+src/pynwb/ndx_miniscope/utils/timestamps.py
+src/pynwb/ndx_miniscope/utils/video.py
```

