# Comparing `tmp/cdk-redisdb-0.0.31.tar.gz` & `tmp/cdk-redisdb-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-redisdb-0.0.31.tar", last modified: Sun Jun 18 01:04:58 2023, max compression
+gzip compressed data, was "cdk-redisdb-0.0.32.tar", last modified: Mon Jun 19 01:43:38 2023, max compression
```

## Comparing `cdk-redisdb-0.0.31.tar` & `cdk-redisdb-0.0.32.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:04:58.470618 cdk-redisdb-0.0.31/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-18 01:04:43.000000 cdk-redisdb-0.0.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-18 01:04:43.000000 cdk-redisdb-0.0.31/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-18 01:04:58.470618 cdk-redisdb-0.0.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-18 01:04:43.000000 cdk-redisdb-0.0.31/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-18 01:04:43.000000 cdk-redisdb-0.0.31/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 01:04:58.470618 cdk-redisdb-0.0.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-18 01:04:43.000000 cdk-redisdb-0.0.31/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:04:58.466618 cdk-redisdb-0.0.31/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:04:58.470618 cdk-redisdb-0.0.31/src/cdk_redisdb/
--rw-r--r--   0 runner    (1001) docker     (123)    48408 2023-06-18 01:04:43.000000 cdk-redisdb-0.0.31/src/cdk_redisdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:04:58.470618 cdk-redisdb-0.0.31/src/cdk_redisdb/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-18 01:04:43.000000 cdk-redisdb-0.0.31/src/cdk_redisdb/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26105 2023-06-18 01:04:43.000000 cdk-redisdb-0.0.31/src/cdk_redisdb/_jsii/cdk-redisdb@0.0.31.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:04:43.000000 cdk-redisdb-0.0.31/src/cdk_redisdb/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:04:58.470618 cdk-redisdb-0.0.31/src/cdk_redisdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-18 01:04:58.000000 cdk-redisdb-0.0.31/src/cdk_redisdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-18 01:04:58.000000 cdk-redisdb-0.0.31/src/cdk_redisdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:04:58.000000 cdk-redisdb-0.0.31/src/cdk_redisdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-18 01:04:58.000000 cdk-redisdb-0.0.31/src/cdk_redisdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 01:04:58.000000 cdk-redisdb-0.0.31/src/cdk_redisdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 01:43:38.896803 cdk-redisdb-0.0.32/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-19 01:43:27.000000 cdk-redisdb-0.0.32/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-19 01:43:27.000000 cdk-redisdb-0.0.32/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-19 01:43:38.896803 cdk-redisdb-0.0.32/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-19 01:43:27.000000 cdk-redisdb-0.0.32/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-19 01:43:27.000000 cdk-redisdb-0.0.32/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 01:43:38.896803 cdk-redisdb-0.0.32/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-19 01:43:27.000000 cdk-redisdb-0.0.32/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 01:43:38.892802 cdk-redisdb-0.0.32/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 01:43:38.892802 cdk-redisdb-0.0.32/src/cdk_redisdb/
+-rw-r--r--   0 runner    (1001) docker     (123)    48408 2023-06-19 01:43:27.000000 cdk-redisdb-0.0.32/src/cdk_redisdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 01:43:38.896803 cdk-redisdb-0.0.32/src/cdk_redisdb/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-19 01:43:27.000000 cdk-redisdb-0.0.32/src/cdk_redisdb/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26108 2023-06-19 01:43:27.000000 cdk-redisdb-0.0.32/src/cdk_redisdb/_jsii/cdk-redisdb@0.0.32.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 01:43:27.000000 cdk-redisdb-0.0.32/src/cdk_redisdb/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 01:43:38.892802 cdk-redisdb-0.0.32/src/cdk_redisdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-19 01:43:38.000000 cdk-redisdb-0.0.32/src/cdk_redisdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-19 01:43:38.000000 cdk-redisdb-0.0.32/src/cdk_redisdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 01:43:38.000000 cdk-redisdb-0.0.32/src/cdk_redisdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-19 01:43:38.000000 cdk-redisdb-0.0.32/src/cdk_redisdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 01:43:38.000000 cdk-redisdb-0.0.32/src/cdk_redisdb.egg-info/top_level.txt
```

### Comparing `cdk-redisdb-0.0.31/LICENSE` & `cdk-redisdb-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.31/PKG-INFO` & `cdk-redisdb-0.0.32/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-redisdb
-Version: 0.0.31
+Version: 0.0.32
 Summary: Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API
 Home-page: https://github.com/forkfork/cdk-redisdb.git
 Author: Timothy Downs<timothydowns@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/forkfork/cdk-redisdb.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-redisdb-0.0.31/README.md` & `cdk-redisdb-0.0.32/README.md`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.31/setup.py` & `cdk-redisdb-0.0.32/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-redisdb",
-    "version": "0.0.31",
+    "version": "0.0.32",
     "description": "Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API",
     "license": "Apache-2.0",
     "url": "https://github.com/forkfork/cdk-redisdb.git",
     "long_description_content_type": "text/markdown",
     "author": "Timothy Downs<timothydowns@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_redisdb",
         "cdk_redisdb._jsii"
     ],
     "package_data": {
         "cdk_redisdb._jsii": [
-            "cdk-redisdb@0.0.31.jsii.tgz"
+            "cdk-redisdb@0.0.32.jsii.tgz"
         ],
         "cdk_redisdb": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-redisdb-0.0.31/src/cdk_redisdb/__init__.py` & `cdk-redisdb-0.0.32/src/cdk_redisdb/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.31/src/cdk_redisdb.egg-info/PKG-INFO` & `cdk-redisdb-0.0.32/src/cdk_redisdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-redisdb
-Version: 0.0.31
+Version: 0.0.32
 Summary: Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API
 Home-page: https://github.com/forkfork/cdk-redisdb.git
 Author: Timothy Downs<timothydowns@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/forkfork/cdk-redisdb.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

