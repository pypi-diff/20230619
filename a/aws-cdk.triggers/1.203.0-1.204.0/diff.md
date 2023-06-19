# Comparing `tmp/aws-cdk.triggers-1.203.0.tar.gz` & `tmp/aws-cdk.triggers-1.204.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src637092372/src/packages/@aws-cdk/triggers/dist/python/aws-cdk.triggers-1.203.0.tar", last modified: Wed May 31 18:49:57 2023, max compression
+gzip compressed data, was "/codebuild/output/src348153380/src/packages/@aws-cdk/triggers/dist/python/aws-cdk.triggers-1.204.0.tar", last modified: Mon Jun 19 16:37:53 2023, max compression
```

## Comparing `aws-cdk.triggers-1.203.0.tar` & `aws-cdk.triggers-1.204.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:49:57.000000 aws-cdk.triggers-1.203.0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-05-31 18:49:51.000000 aws-cdk.triggers-1.203.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-31 18:49:51.000000 aws-cdk.triggers-1.203.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-31 18:49:51.000000 aws-cdk.triggers-1.203.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4210 2023-05-31 18:49:57.000000 aws-cdk.triggers-1.203.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3233 2023-05-31 18:49:51.000000 aws-cdk.triggers-1.203.0/README.md
--rw-r--r--   0 root         (0) root         (0)      236 2023-05-31 18:49:51.000000 aws-cdk.triggers-1.203.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 18:49:57.000000 aws-cdk.triggers-1.203.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1814 2023-05-31 18:49:51.000000 aws-cdk.triggers-1.203.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:49:57.000000 aws-cdk.triggers-1.203.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:49:57.000000 aws-cdk.triggers-1.203.0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:49:57.000000 aws-cdk.triggers-1.203.0/src/aws_cdk/triggers/
--rw-r--r--   0 root         (0) root         (0)    98712 2023-05-31 18:49:51.000000 aws-cdk.triggers-1.203.0/src/aws_cdk/triggers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:49:57.000000 aws-cdk.triggers-1.203.0/src/aws_cdk/triggers/_jsii/
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-31 18:49:51.000000 aws-cdk.triggers-1.203.0/src/aws_cdk/triggers/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29771 2023-05-31 18:49:51.000000 aws-cdk.triggers-1.203.0/src/aws_cdk/triggers/_jsii/triggers@1.203.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 18:49:51.000000 aws-cdk.triggers-1.203.0/src/aws_cdk/triggers/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:49:57.000000 aws-cdk.triggers-1.203.0/src/aws_cdk.triggers.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4210 2023-05-31 18:49:57.000000 aws-cdk.triggers-1.203.0/src/aws_cdk.triggers.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      434 2023-05-31 18:49:57.000000 aws-cdk.triggers-1.203.0/src/aws_cdk.triggers.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 18:49:57.000000 aws-cdk.triggers-1.203.0/src/aws_cdk.triggers.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 18:49:57.000000 aws-cdk.triggers-1.203.0/src/aws_cdk.triggers.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-31 18:49:57.000000 aws-cdk.triggers-1.203.0/src/aws_cdk.triggers.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:37:53.000000 aws-cdk.triggers-1.204.0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-06-19 16:37:44.000000 aws-cdk.triggers-1.204.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-19 16:37:44.000000 aws-cdk.triggers-1.204.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-19 16:37:44.000000 aws-cdk.triggers-1.204.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4505 2023-06-19 16:37:53.000000 aws-cdk.triggers-1.204.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3506 2023-06-19 16:37:44.000000 aws-cdk.triggers-1.204.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-19 16:37:44.000000 aws-cdk.triggers-1.204.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 16:37:53.000000 aws-cdk.triggers-1.204.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1855 2023-06-19 16:37:44.000000 aws-cdk.triggers-1.204.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:37:53.000000 aws-cdk.triggers-1.204.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:37:53.000000 aws-cdk.triggers-1.204.0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:37:53.000000 aws-cdk.triggers-1.204.0/src/aws_cdk/triggers/
+-rw-r--r--   0 root         (0) root         (0)    98985 2023-06-19 16:37:44.000000 aws-cdk.triggers-1.204.0/src/aws_cdk/triggers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:37:53.000000 aws-cdk.triggers-1.204.0/src/aws_cdk/triggers/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      433 2023-06-19 16:37:44.000000 aws-cdk.triggers-1.204.0/src/aws_cdk/triggers/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30117 2023-06-19 16:37:44.000000 aws-cdk.triggers-1.204.0/src/aws_cdk/triggers/_jsii/triggers@1.204.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 16:37:44.000000 aws-cdk.triggers-1.204.0/src/aws_cdk/triggers/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:37:53.000000 aws-cdk.triggers-1.204.0/src/aws_cdk.triggers.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4505 2023-06-19 16:37:53.000000 aws-cdk.triggers-1.204.0/src/aws_cdk.triggers.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      434 2023-06-19 16:37:53.000000 aws-cdk.triggers-1.204.0/src/aws_cdk.triggers.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 16:37:53.000000 aws-cdk.triggers-1.204.0/src/aws_cdk.triggers.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2023-06-19 16:37:53.000000 aws-cdk.triggers-1.204.0/src/aws_cdk.triggers.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-19 16:37:53.000000 aws-cdk.triggers-1.204.0/src/aws_cdk.triggers.egg-info/top_level.txt
```

### Comparing `aws-cdk.triggers-1.203.0/LICENSE` & `aws-cdk.triggers-1.204.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.triggers-1.203.0/PKG-INFO` & `aws-cdk.triggers-1.204.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 Metadata-Version: 2.1
 Name: aws-cdk.triggers
-Version: 1.203.0
+Version: 1.204.0
 Summary: Execute AWS Lambda functions during deployment
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 7 - Inactive
 Classifier: License :: OSI Approved
 Classifier: Framework :: AWS CDK
 Classifier: Framework :: AWS CDK :: 1
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # Triggers
 
 <!--BEGIN STABILITY BANNER-->---
 
 
-![cdk-constructs: Stable](https://img.shields.io/badge/cdk--constructs-stable-success.svg?style=for-the-badge)
+![End-of-Support](https://img.shields.io/badge/End--of--Support-critical.svg?style=for-the-badge)
+
+> AWS CDK v1 has reached End-of-Support on 2023-06-01.
+> This package is no longer being updated, and users should migrate to AWS CDK v2.
+>
+> For more information on how to migrate, see the [*Migrating to AWS CDK v2* guide](https://docs.aws.amazon.com/cdk/v2/guide/migrating-v2.html).
 
 ---
 <!--END STABILITY BANNER-->
 
 Triggers allows you to execute code during deployments. This can be used for a
 variety of use cases such as:
 
@@ -114,9 +119,7 @@
 In the future we will consider adding support for additional re-execution modes:
 
 * `executeOnEveryDeployment: boolean` - re-executes every time the stack is
   deployed (add random "salt" during synthesis).
 * `executeOnResourceChange: Construct[]` - re-executes when one of the resources
   under the specified scopes has changed (add the hash the CloudFormation
   resource specs).
-
-
```

### Comparing `aws-cdk.triggers-1.203.0/README.md` & `aws-cdk.triggers-1.204.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # Triggers
 
 <!--BEGIN STABILITY BANNER-->---
 
 
-![cdk-constructs: Stable](https://img.shields.io/badge/cdk--constructs-stable-success.svg?style=for-the-badge)
+![End-of-Support](https://img.shields.io/badge/End--of--Support-critical.svg?style=for-the-badge)
+
+> AWS CDK v1 has reached End-of-Support on 2023-06-01.
+> This package is no longer being updated, and users should migrate to AWS CDK v2.
+>
+> For more information on how to migrate, see the [*Migrating to AWS CDK v2* guide](https://docs.aws.amazon.com/cdk/v2/guide/migrating-v2.html).
 
 ---
 <!--END STABILITY BANNER-->
 
 Triggers allows you to execute code during deployments. This can be used for a
 variety of use cases such as:
```

### Comparing `aws-cdk.triggers-1.203.0/setup.py` & `aws-cdk.triggers-1.204.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.triggers",
-    "version": "1.203.0",
+    "version": "1.204.0",
     "description": "Execute AWS Lambda functions during deployment",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,40 +22,41 @@
     },
     "packages": [
         "aws_cdk.triggers",
         "aws_cdk.triggers._jsii"
     ],
     "package_data": {
         "aws_cdk.triggers._jsii": [
-            "triggers@1.203.0.jsii.tgz"
+            "triggers@1.204.0.jsii.tgz"
         ],
         "aws_cdk.triggers": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk.aws-lambda==1.203.0",
-        "aws-cdk.core==1.203.0",
+        "aws-cdk.aws-lambda==1.204.0",
+        "aws-cdk.core==1.204.0",
         "constructs>=3.3.69, <4.0.0",
-        "jsii>=1.74.0, <2.0.0",
+        "jsii>=1.84.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
-        "Development Status :: 5 - Production/Stable",
+        "Development Status :: 7 - Inactive",
         "License :: OSI Approved",
         "Framework :: AWS CDK",
         "Framework :: AWS CDK :: 1"
     ],
     "scripts": []
 }
 """
```

### Comparing `aws-cdk.triggers-1.203.0/src/aws_cdk/triggers/__init__.py` & `aws-cdk.triggers-1.204.0/src/aws_cdk/triggers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 '''
 # Triggers
 
 <!--BEGIN STABILITY BANNER-->---
 
 
-![cdk-constructs: Stable](https://img.shields.io/badge/cdk--constructs-stable-success.svg?style=for-the-badge)
+![End-of-Support](https://img.shields.io/badge/End--of--Support-critical.svg?style=for-the-badge)
+
+> AWS CDK v1 has reached End-of-Support on 2023-06-01.
+> This package is no longer being updated, and users should migrate to AWS CDK v2.
+>
+> For more information on how to migrate, see the [*Migrating to AWS CDK v2* guide](https://docs.aws.amazon.com/cdk/v2/guide/migrating-v2.html).
 
 ---
 <!--END STABILITY BANNER-->
 
 Triggers allows you to execute code during deployments. This can be used for a
 variety of use cases such as:
```

### Comparing `aws-cdk.triggers-1.203.0/src/aws_cdk.triggers.egg-info/PKG-INFO` & `aws-cdk.triggers-1.204.0/src/aws_cdk.triggers.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 Metadata-Version: 2.1
 Name: aws-cdk.triggers
-Version: 1.203.0
+Version: 1.204.0
 Summary: Execute AWS Lambda functions during deployment
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 7 - Inactive
 Classifier: License :: OSI Approved
 Classifier: Framework :: AWS CDK
 Classifier: Framework :: AWS CDK :: 1
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # Triggers
 
 <!--BEGIN STABILITY BANNER-->---
 
 
-![cdk-constructs: Stable](https://img.shields.io/badge/cdk--constructs-stable-success.svg?style=for-the-badge)
+![End-of-Support](https://img.shields.io/badge/End--of--Support-critical.svg?style=for-the-badge)
+
+> AWS CDK v1 has reached End-of-Support on 2023-06-01.
+> This package is no longer being updated, and users should migrate to AWS CDK v2.
+>
+> For more information on how to migrate, see the [*Migrating to AWS CDK v2* guide](https://docs.aws.amazon.com/cdk/v2/guide/migrating-v2.html).
 
 ---
 <!--END STABILITY BANNER-->
 
 Triggers allows you to execute code during deployments. This can be used for a
 variety of use cases such as:
 
@@ -114,9 +119,7 @@
 In the future we will consider adding support for additional re-execution modes:
 
 * `executeOnEveryDeployment: boolean` - re-executes every time the stack is
   deployed (add random "salt" during synthesis).
 * `executeOnResourceChange: Construct[]` - re-executes when one of the resources
   under the specified scopes has changed (add the hash the CloudFormation
   resource specs).
-
-
```

