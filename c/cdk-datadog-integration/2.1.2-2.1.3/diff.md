# Comparing `tmp/cdk-datadog-integration-2.1.2.tar.gz` & `tmp/cdk-datadog-integration-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-datadog-integration-2.1.2.tar", last modified: Sat Jun  3 21:26:43 2023, max compression
+gzip compressed data, was "cdk-datadog-integration-2.1.3.tar", last modified: Mon Jun 19 00:23:26 2023, max compression
```

## Comparing `cdk-datadog-integration-2.1.2.tar` & `cdk-datadog-integration-2.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:26:43.857070 cdk-datadog-integration-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-03 21:26:33.000000 cdk-datadog-integration-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-03 21:26:33.000000 cdk-datadog-integration-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-03 21:26:43.857070 cdk-datadog-integration-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-06-03 21:26:33.000000 cdk-datadog-integration-2.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-03 21:26:33.000000 cdk-datadog-integration-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 21:26:43.857070 cdk-datadog-integration-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-03 21:26:33.000000 cdk-datadog-integration-2.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:26:43.853070 cdk-datadog-integration-2.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:26:43.857070 cdk-datadog-integration-2.1.2/src/cdk_datadog_integration/
--rw-r--r--   0 runner    (1001) docker     (123)    61591 2023-06-03 21:26:33.000000 cdk-datadog-integration-2.1.2/src/cdk_datadog_integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:26:43.857070 cdk-datadog-integration-2.1.2/src/cdk_datadog_integration/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-03 21:26:33.000000 cdk-datadog-integration-2.1.2/src/cdk_datadog_integration/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35294 2023-06-03 21:26:33.000000 cdk-datadog-integration-2.1.2/src/cdk_datadog_integration/_jsii/cdk-datadog-integration@2.1.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 21:26:33.000000 cdk-datadog-integration-2.1.2/src/cdk_datadog_integration/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:26:43.857070 cdk-datadog-integration-2.1.2/src/cdk_datadog_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-03 21:26:43.000000 cdk-datadog-integration-2.1.2/src/cdk_datadog_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-03 21:26:43.000000 cdk-datadog-integration-2.1.2/src/cdk_datadog_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 21:26:43.000000 cdk-datadog-integration-2.1.2/src/cdk_datadog_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-03 21:26:43.000000 cdk-datadog-integration-2.1.2/src/cdk_datadog_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-03 21:26:43.000000 cdk-datadog-integration-2.1.2/src/cdk_datadog_integration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:23:26.472894 cdk-datadog-integration-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-19 00:23:12.000000 cdk-datadog-integration-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-19 00:23:12.000000 cdk-datadog-integration-2.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-19 00:23:26.472894 cdk-datadog-integration-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-06-19 00:23:12.000000 cdk-datadog-integration-2.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-19 00:23:12.000000 cdk-datadog-integration-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 00:23:26.472894 cdk-datadog-integration-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-19 00:23:12.000000 cdk-datadog-integration-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:23:26.468894 cdk-datadog-integration-2.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:23:26.472894 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)    61591 2023-06-19 00:23:12.000000 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:23:26.472894 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-19 00:23:12.000000 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35298 2023-06-19 00:23:12.000000 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration/_jsii/cdk-datadog-integration@2.1.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 00:23:12.000000 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:23:26.472894 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-19 00:23:26.000000 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-19 00:23:26.000000 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 00:23:26.000000 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-19 00:23:26.000000 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-19 00:23:26.000000 cdk-datadog-integration-2.1.3/src/cdk_datadog_integration.egg-info/top_level.txt
```

### Comparing `cdk-datadog-integration-2.1.2/LICENSE` & `cdk-datadog-integration-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-datadog-integration-2.1.2/PKG-INFO` & `cdk-datadog-integration-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-datadog-integration
-Version: 2.1.2
+Version: 2.1.3
 Summary: cdk-datadog-integration
 Home-page: https://github.com/blimmer/cdk-datadog-integration.git
 Author: Ben Limmer
 License: Apache-2.0
 Project-URL: Source, https://github.com/blimmer/cdk-datadog-integration.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-datadog-integration-2.1.2/README.md` & `cdk-datadog-integration-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cdk-datadog-integration-2.1.2/setup.py` & `cdk-datadog-integration-2.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-datadog-integration",
-    "version": "2.1.2",
+    "version": "2.1.3",
     "description": "cdk-datadog-integration",
     "license": "Apache-2.0",
     "url": "https://github.com/blimmer/cdk-datadog-integration.git",
     "long_description_content_type": "text/markdown",
     "author": "Ben Limmer",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_datadog_integration",
         "cdk_datadog_integration._jsii"
     ],
     "package_data": {
         "cdk_datadog_integration._jsii": [
-            "cdk-datadog-integration@2.1.2.jsii.tgz"
+            "cdk-datadog-integration@2.1.3.jsii.tgz"
         ],
         "cdk_datadog_integration": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.56.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.82.0, <2.0.0",
+        "jsii>=1.84.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk-datadog-integration-2.1.2/src/cdk_datadog_integration/__init__.py` & `cdk-datadog-integration-2.1.3/src/cdk_datadog_integration/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-datadog-integration-2.1.2/src/cdk_datadog_integration.egg-info/PKG-INFO` & `cdk-datadog-integration-2.1.3/src/cdk_datadog_integration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-datadog-integration
-Version: 2.1.2
+Version: 2.1.3
 Summary: cdk-datadog-integration
 Home-page: https://github.com/blimmer/cdk-datadog-integration.git
 Author: Ben Limmer
 License: Apache-2.0
 Project-URL: Source, https://github.com/blimmer/cdk-datadog-integration.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

