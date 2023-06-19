# Comparing `tmp/circlecigen-0.0.3.tar.gz` & `tmp/circlecigen-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circlecigen-0.0.3.tar", last modified: Tue Apr  4 01:01:08 2023, max compression
+gzip compressed data, was "circlecigen-0.0.4.tar", last modified: Mon Jun 19 15:35:52 2023, max compression
```

## Comparing `circlecigen-0.0.3.tar` & `circlecigen-0.0.4.tar`

### file list

```diff
@@ -1,48 +1,55 @@
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-04 01:01:08.514539 circlecigen-0.0.3/
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-04 01:01:08.514539 circlecigen-0.0.3/.circleci/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4147 2023-04-04 01:01:03.000000 circlecigen-0.0.3/.circleci/config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      350 2023-04-04 01:01:03.000000 circlecigen-0.0.3/.codeclimate.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      108 2023-04-04 01:01:03.000000 circlecigen-0.0.3/.gitignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)      866 2023-04-04 01:01:03.000000 circlecigen-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18369 2023-04-04 01:01:03.000000 circlecigen-0.0.3/.pylintrc
--rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2023-04-04 01:01:03.000000 circlecigen-0.0.3/.python-version
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-04-04 01:01:03.000000 circlecigen-0.0.3/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23213 2023-04-04 01:01:08.514539 circlecigen-0.0.3/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      388 2023-04-04 01:01:03.000000 circlecigen-0.0.3/Pipfile
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22577 2023-04-04 01:01:03.000000 circlecigen-0.0.3/README.md
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-04 01:01:08.514539 circlecigen-0.0.3/env_test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6309 2023-04-04 01:01:03.000000 circlecigen-0.0.3/env_test/config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      121 2023-04-04 01:01:03.000000 circlecigen-0.0.3/env_test/default.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      318 2023-04-04 01:01:03.000000 circlecigen-0.0.3/env_test/multi.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      581 2023-04-04 01:01:03.000000 circlecigen-0.0.3/env_test/post-approve.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      337 2023-04-04 01:01:03.000000 circlecigen-0.0.3/env_test/pre-approve.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       51 2023-04-04 01:01:03.000000 circlecigen-0.0.3/env_test/qa.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3866 2023-04-04 01:01:03.000000 circlecigen-0.0.3/notes.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2023-04-04 01:01:03.000000 circlecigen-0.0.3/op.env
--rw-r--r--   0 circleci  (3434) circleci  (3434)      711 2023-04-04 01:01:03.000000 circlecigen-0.0.3/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      365 2023-04-04 01:01:03.000000 circlecigen-0.0.3/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-04 01:01:08.514539 circlecigen-0.0.3/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      791 2023-04-04 01:01:03.000000 circlecigen-0.0.3/setup.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-04 01:01:08.514539 circlecigen-0.0.3/src/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-04 01:01:03.000000 circlecigen-0.0.3/src/__init__.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-04 01:01:08.514539 circlecigen-0.0.3/src/circlecigen.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23213 2023-04-04 01:01:08.000000 circlecigen-0.0.3/src/circlecigen.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      869 2023-04-04 01:01:08.000000 circlecigen-0.0.3/src/circlecigen.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-04 01:01:08.000000 circlecigen-0.0.3/src/circlecigen.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2023-04-04 01:01:08.000000 circlecigen-0.0.3/src/circlecigen.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-04 01:01:08.000000 circlecigen-0.0.3/src/circlecigen.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2423 2023-04-04 01:01:03.000000 circlecigen-0.0.3/src/circlecigen.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5414 2023-04-04 01:01:03.000000 circlecigen-0.0.3/src/template.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1636 2023-04-04 01:01:03.000000 circlecigen-0.0.3/src/tfvars.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-04-04 01:01:03.000000 circlecigen-0.0.3/src/utils.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-04 01:01:08.514539 circlecigen-0.0.3/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6383 2023-04-04 01:01:03.000000 circlecigen-0.0.3/test/generated_config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2410 2023-04-04 01:01:03.000000 circlecigen-0.0.3/test/generated_config_setup.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      112 2023-04-04 01:01:03.000000 circlecigen-0.0.3/test/preview-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      112 2023-04-04 01:01:03.000000 circlecigen-0.0.3/test/preview-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      114 2023-04-04 01:01:03.000000 circlecigen-0.0.3/test/qa-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      114 2023-04-04 01:01:03.000000 circlecigen-0.0.3/test/qa-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2204 2023-04-04 01:01:03.000000 circlecigen-0.0.3/test/test_circlecigen.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1895 2023-04-04 01:01:03.000000 circlecigen-0.0.3/test/test_template.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1925 2023-04-04 01:01:03.000000 circlecigen-0.0.3/test/test_tfvars.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1486 2023-04-04 01:01:03.000000 circlecigen-0.0.3/test/test_utils.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-19 15:35:52.652210 circlecigen-0.0.4/
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-19 15:35:52.648210 circlecigen-0.0.4/.circleci/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4013 2023-06-19 15:35:47.000000 circlecigen-0.0.4/.circleci/config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      350 2023-06-19 15:35:47.000000 circlecigen-0.0.4/.codeclimate.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-19 15:35:47.000000 circlecigen-0.0.4/.gitignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      866 2023-06-19 15:35:47.000000 circlecigen-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18369 2023-06-19 15:35:47.000000 circlecigen-0.0.4/.pylintrc
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2023-06-19 15:35:47.000000 circlecigen-0.0.4/.python-version
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-06-19 15:35:47.000000 circlecigen-0.0.4/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22062 2023-06-19 15:35:52.652210 circlecigen-0.0.4/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      432 2023-06-19 15:35:47.000000 circlecigen-0.0.4/Pipfile
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21426 2023-06-19 15:35:47.000000 circlecigen-0.0.4/README.md
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-19 15:35:52.648210 circlecigen-0.0.4/env_test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3037 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       82 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/default.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       39 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/dev.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5415 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/generated_config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/multi.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/nonprod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/nonprod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/nonprod.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      556 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/post-approve.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      312 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/pre-approve.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/prod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/prod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2023-06-19 15:35:47.000000 circlecigen-0.0.4/env_test/prod.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      313 2023-06-19 15:35:47.000000 circlecigen-0.0.4/notes.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2023-06-19 15:35:47.000000 circlecigen-0.0.4/op.env
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      711 2023-06-19 15:35:47.000000 circlecigen-0.0.4/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      365 2023-06-19 15:35:47.000000 circlecigen-0.0.4/requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-19 15:35:52.652210 circlecigen-0.0.4/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      791 2023-06-19 15:35:47.000000 circlecigen-0.0.4/setup.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-19 15:35:52.652210 circlecigen-0.0.4/src/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-19 15:35:47.000000 circlecigen-0.0.4/src/__init__.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-19 15:35:52.652210 circlecigen-0.0.4/src/circlecigen.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22062 2023-06-19 15:35:52.000000 circlecigen-0.0.4/src/circlecigen.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1088 2023-06-19 15:35:52.000000 circlecigen-0.0.4/src/circlecigen.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-19 15:35:52.000000 circlecigen-0.0.4/src/circlecigen.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2023-06-19 15:35:52.000000 circlecigen-0.0.4/src/circlecigen.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-19 15:35:52.000000 circlecigen-0.0.4/src/circlecigen.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2573 2023-06-19 15:35:47.000000 circlecigen-0.0.4/src/circlecigen.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5572 2023-06-19 15:35:47.000000 circlecigen-0.0.4/src/template.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2091 2023-06-19 15:35:47.000000 circlecigen-0.0.4/src/tfvars.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-06-19 15:35:47.000000 circlecigen-0.0.4/src/utils.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-19 15:35:52.652210 circlecigen-0.0.4/test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5415 2023-06-19 15:35:47.000000 circlecigen-0.0.4/test/generated_config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1592 2023-06-19 15:35:47.000000 circlecigen-0.0.4/test/generated_config_setup.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-19 15:35:47.000000 circlecigen-0.0.4/test/nonprod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-19 15:35:47.000000 circlecigen-0.0.4/test/nonprod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-19 15:35:47.000000 circlecigen-0.0.4/test/prod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-19 15:35:47.000000 circlecigen-0.0.4/test/prod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2262 2023-06-19 15:35:47.000000 circlecigen-0.0.4/test/test_circlecigen.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2334 2023-06-19 15:35:47.000000 circlecigen-0.0.4/test/test_template.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2336 2023-06-19 15:35:47.000000 circlecigen-0.0.4/test/test_tfvars.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1486 2023-06-19 15:35:47.000000 circlecigen-0.0.4/test/test_utils.py
```

### Comparing `circlecigen-0.0.3/.circleci/config.yml` & `circlecigen-0.0.4/.circleci/config.yml`

 * *Files 27% similar despite different names*

```diff
@@ -3,19 +3,16 @@
 
 orbs:
   op: twdps/onepassword@1.0.0
   do: twdps/pipeline-events@0.1.0
 
 # ================================================================= global configuration
 
-parameters:
-  context:
-    description: circleci context for all jobs
-    type: string
-    default: twdps-core-labs-team
+globals:
+  - &context twdps-core-labs-team
 
 on-push-main: &on-push-main
   branches:
     only: /main/
   tags:
     ignore: /.*/
 
@@ -112,15 +109,15 @@
           env-file: op.env
       - set-credentials:
           environment: test
       - run:
           name: Build
           command: |
             sudo pip install -r requirements.txt
-            python -m build
+            PYTHONPATH=.:./src python -m build
       - run:
           name: upload to test.pypi
           command: python -m twine upload --repository testpypi dist/*
       - persist_to_workspace:
           root: .
           paths:
             - dist/
@@ -148,19 +145,19 @@
 workflows:
   version: 2
 
   python package pipeline:
     jobs:
 
       - static code analysis and unit tests:
-          context: << pipeline.parameters.context >>
+          context: *context
           filters: *on-push-main
 
       - build package and integration test:
-          context: << pipeline.parameters.context >>
+          context: *context
           filters: *on-tag-main
 
       - publish:
-          context: << pipeline.parameters.context >>
+          context: *context
           requires:
             - build package and integration test
           filters: *on-tag-main
```

### Comparing `circlecigen-0.0.3/.pre-commit-config.yaml` & `circlecigen-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.3/.pylintrc` & `circlecigen-0.0.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.3/LICENSE` & `circlecigen-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.3/PKG-INFO` & `circlecigen-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circlecigen
-Version: 0.0.3
+Version: 0.0.4
 Summary: Opinionated generation of continuation pipelines
 Home-page: https://github.com/ThoughtWorks-DPS/circlecigen
 Author: Nic Cheneweth
 Author-email: Nic Cheneweth <nchenewe@thoughtworks.com>
 Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/circlecigen
 Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/circlecigen/issues
 Classifier: Programming Language :: Python :: 3
@@ -34,81 +34,128 @@
 pip install circlecigen
 ```
 
 ### How it works
 
 The circleci [continuation orb](https://circleci.com/developer/orbs/orb/circleci/continuation) is somewhat limited in terms of flexability in use, but when you automate the creation of the resulting new pipeline you open up some interesting opportunities. 
 
-The primary inspiration for this package is in automatically generating terraform deployment pipelines for multi-regional environment infrastructure. Imagine you support a globally-available microservice architecure that runs on EKS. This means you must create multiple EKS instances, spanning the supported regions, for potentially more than a single _environment_ role. What if Production required eks clusters in 3 localities around the world, with additionally 2 regions per locality where traffic is geo-location routed to the closest in proximity. This results in six (6) clusters, that together actually make up just one environment - Production. While this is approaching a scale where a more robust infrastructre control-plane is required, a common intermediate step is to simply continue orchestrating this infrastructure via an infrastructure-pipeline while a decision or implementation around a more complex evolution is undertaken.  
+The primary inspiration for this package is in automatically generating terraform deployment pipelines for multi-regional environment infrastructure. Imagine you support a globally-available microservice architecure that runs on EKS. This means you must create multiple EKS instances, spanning the supported regions, for potentially more than a single _environment_ role. What if Production required eks clusters in 3 localities around the world, with additionally 2 regions per locality where traffic is geo-location routed to the closest in proximity. This results in six (6) clusters, that together actually make up just one platform _environment_ - Production. While this is approaching a scale where a more robust infrastructre control-plane is required, a common intermediate step is to simply increase the dynamic deployment capabilities of the release pipeline.  
 
 In order to maintain DRYness in the terraform code, avoiding duplication of multiple instances of otherwise identical pipeline workflow jobs for each environment, what if instead you could define all the instances of a particular environment category in a single json file and the deployment pipeline is then generated to match at runtime?
 
 That is what this tool enables.  
 
-In simplest terms, you define templates of _pre-approval_ and _post-approval_ circleci jobs that includes jinja2 style variable-substitution formatting. 
+Let's call the multi-instance environments `Roles`.  
 
-For all instances of each desired role, circlecigen will generate a deployment pipeline that has:  
+In simplest terms, you define templates of _pre-approval_ and _post-approval_ circleci workflow jobs that include jinja2 style variable-substitution formatting. 
+
+For all instances of each desired Role, circlecigen will generate a deployment pipeline that has:  
 * a pre-approve job for each instance, followed by
 * an approval step, followed by
 * a post-approve job for each instance
 
-#### Setup example for terraform
+#### Setup example for a terraform EKS pipeline
 
-Let's stay with the EKS example mentioned above. Assume that Production requires six (6) clusters in six different regions, Nonproduction likewise requires cluster in each of the same six regions, and an additional four clusters spanning two global locality are required to support the software-defined lifecycle of this infrastructure. Therefore we have three environment roles; prod, nonprod, infra-dev  
+Let's stay with the EKS example mentioned above. Assume that Production requires six (6) clusters in six different regions, Nonproduction likewise requires cluster in each of the same six regions, and an additional three clusters spanning nearby global localities are required to support the software-defined lifecycle of this infrastructure. Therefore we have three environment Roles: infra-dev role that is deployed on git-push, and the nonprod and prod roles that release consequtively upon git-tag.  
 
-First, let's define the roles and number of instances per role.  
+Given the output of the actual deployment pipelines, this tool also supports generating the tfvar files for each cluster deployment.  
 
-**environments/dev-deploy.json**  
+First, let's define the top level pipelines, roles, and instances definition.   
 
-The infra-dev role requires four environments, each in a unique region, and in two different global localities. While the overall infrastructure we have described ultimately spans a much wider area, a reasonable subset is sufficient for fully testing the build/deploy logic. Notice that we also specify a filter. This is a reference to the circleci filter used to trigger the pipeline. See the example config.yml below for full description.  
+**environments/multi.json**  
 
+The top-level json definition groups roles by the circleci filter that will trigger the deployment of the associated Roles. Within each Role, define the instances that should exist. And finally list any particular settings associated with an individual instances.  
 
-```json
-{
-  "filter": "*on-push-main",
-  "infra-dev": {
-    "infra-dev-us-west-2": {},
-    "infra-dev-us-east-2": {},
-    "infra-dev-eu-west-1": {},
-    "infra-dev-eu-central-2": {}
-  }
-}
-```
+This multi-environment definition also defines the top-level pipeline structure for other pipelines with the same infrastructure path to production and should probably be maintained in a globally accessible location rather than duplicating the file in multiple repositories. For this example we assume this configuration has already been added locally as a file.  
 
-**environments/release.json**  
-The release pipeline now covers all the remaining infrastructure instances. And note it is triggered by tag rather than push.  
 ```json
 {
-  "filter": "*on-tag-main",
-  "nonprod": {
-    "nonprod-us-west-2": {},
-    "nonprod-us-east-2": {},
-    "nonprod-eu-west-1": {},
-    "nonprod-eu-central-2": {},
-    "nonprod-ap-southeast-2": {},
-    "nonprod-ap-southwest-1": {}
+  "infradev": {
+    "filter": "*on-push-main",
+    "infradev": {
+      "infradev-us-east-2": {
+        "aws_region": "us-east-2",
+        "aws_account_id": "10100000000"
+      },
+      "infradev-eu-west-3": {
+        "aws_region": "us-east-2",
+        "aws_account_id": "10100000000"
+      },
+      "infradev-ap-southeast-3": {
+        "aws_region": "eu-west-1",
+        "aws_account_id": "10100000000"
+      }
+    }
   },
-  "prod": {
-    "prod-us-west-2": {},
-    "prod-us-east-2": {},
-    "prod-eu-west-1": {},
-    "prod-eu-central-2": {},
-    "prod-ap-southeast-2": {},
-    "prod-ap-southwest-1": {}
+  "release": {
+    "filter": "*on-tag-main",
+    "nonprod": {
+      "nonprod-us-west-2": {
+        "aws_region": "us-west-2",
+        "aws_account_id": "20100000000"
+      },
+      "nonprod-us-east-2": {
+        "aws_region": "us-east-2",
+        "aws_account_id": "20100000000"
+      },
+      "nonprod-eu-west-1": {
+        "aws_region": "eu-west-1",
+        "aws_account_id": "20100000000"
+      },
+      "nonprod-eu-central-1": {
+        "aws_region": "eu-central-1",
+        "aws_account_id": "20100000000"
+      },
+      "nonprod-ap-southeast-2": {
+        "aws_region": "ap-southeast-2",
+        "aws_account_id": "20100000000"
+      },
+      "nonprod-ap-southwest-1": {
+        "aws_region": "ap-southwest-1",
+        "aws_account_id": "20100000000"
+      }
+    },
+    "prod": {
+      "prod-us-west-2": {
+        "aws_region": "us-west-2",
+        "aws_account_id": "30100000000"
+      },
+      "prod-us-east-2": {
+        "aws_region": "us-east-2",
+        "aws_account_id": "30100000000"
+      },
+      "prod-eu-west-1": {
+        "aws_region": "eu-west-1",
+        "aws_account_id": "30100000000"
+      },
+      "prod-eu-central-1": {
+        "aws_region": "eu-central-1",
+        "aws_account_id": "30100000000"
+      },
+      "prod-ap-southeast-2": {
+        "aws_region": "ap-southeast-2",
+        "aws_account_id": "30100000000"
+      },
+      "prod-ap-southwest-1": {
+        "aws_region": "ap-southwest-1",
+        "aws_account_id": "30100000000"
+      }
+    }
   }
 }
 ```
 
 **environments/default.json**   
 
-Next, create the default tfvars values. Usually, this is best populated with the shared-values for the initial deployment target environment, usually _dev_. Such as:  
+
+Now, define the default values. These are settings to be applied to all instances of all roles:  
 ```json
 {
-  "aws_account_id": "000000000000",
   "cluster_eks_version": "1.25",
+  "cluster_enabled_log_types": ["api", "audit", "authenticator", "controllerManager", "scheduler"],
   "aws_efs_csi_driver_chart_version": "2.4.0",
   "metrics_server_chart_version": "6.2.14",
   "kube_state_metrics_chart_version": "3.3.4",
   "cluster_autoscaler_chart_version": "9.26.0",
 
   "AL2_x86_64_instance_types": [
     "t2.2xlarge",
@@ -125,154 +172,101 @@
   ],
 
   "management_node_group_name": "management-x86-al2-mng",
   "management_node_group_role": "management",
   "management_node_group_ami_type": "AL2_x86_64",
   "management_node_group_platform": "linux",
   "management_node_group_disk_size": "50",
-  "management_node_group_capacity_type": "SPOT",
-  "management_node_group_desired_size": "3",
-  "management_node_group_max_size": "5",
-  "management_node_group_min_size": "3",
 
   "baseline_node_group_name": "baseline-arm-rkt-mng",
   "baseline_node_group_role": "baseline",
   "baseline_node_group_ami_type": "BOTTLEROCKET_ARM_64",
   "baseline_node_group_platform": "bottlerocket",
   "baseline_node_group_disk_size": "50",
-  "baseline_node_group_capacity_type": "SPOT",
-  "baseline_node_group_desired_size": "3",
-  "baseline_node_group_max_size": "5",
-  "baseline_node_group_min_size": "3",
 
   "surge_node_group_name": "surge-arm-rkt-mng",
   "surge_node_group_role": "surge",
   "surge_node_group_ami_type": "BOTTLEROCKET_ARM_64",
   "surge_node_group_platform": "bottlerocket",
   "surge_node_group_disk_size": "50",
-  "surge_node_group_capacity_type": "SPOT",
-  "surge_node_group_desired_size": "1",
-  "surge_node_group_max_size": "3",
-  "surge_node_group_min_size": "1"
+  
 }
 ```
-Next, define environment role overrides. In our example, we have three. infra-dev is the first deployment target and can use the above defaults. However, nonprod and prod need different values - though these are shared across the role. So we will create the following two role configuration override files.  
 
-**environments/prod.json**  
-In prod we must override the baseline nodegroup to use more and ON_DEMAND instances for the baseline (or _persistent_) pool in order to support the currently experienced traffic at acceptable scale up/down wiat frequency. The surge pool can use spot, but we want a minimum of 1, and larger surge potential than for infra-dev, while still constraining just how far it can grow based. And, since all of our production environments are in one AWS account, we can set that here as well.   
+Next, define Role overrides.
+
+**environments/infradev.json**  
+
 ```json
 {
-  "aws_account_id": "111111111111",
-  "baseline_node_group_capacity_type": "ON_DEMAND",
-  "baseline_node_group_desired_size": "30",
-  "baseline_node_group_max_size": "35",
-  "baseline_node_group_min_size": "30",
+  "cluster_log_retention": "10",
+  "alert_channel": "dev",
 
-  "surge_node_group_desired_size": "3",
-  "surge_node_group_max_size": "60",
-  "surge_node_group_min_size": "1"
+  "management_node_group_capacity_type": "SPOT",
+  "management_node_group_desired_size": "3",
+  "management_node_group_max_size": "5",
+  "management_node_group_min_size": "3",
+
+  "baseline_node_group_capacity_type": "SPOT",
+  "baseline_node_group_desired_size": "3",
+  "baseline_node_group_max_size": "5",
+  "baseline_node_group_min_size": "3",
+
+  "surge_node_group_capacity_type": "SPOT",
+  "surge_node_group_desired_size": "0",
+  "surge_node_group_max_size": "0",
+  "surge_node_group_min_size": "0"
 }
 ```
 
 **environments/nonprod.json**  
-
-In nonprod, though we modify similar overrides, the needs are different. Our developers only live/work in a single global area. So a variety of activities will only take place in the US regions. However, there are naturally a series of integration and functional tests that must span all the locals where the application will run, hence we do need somewhat larger scale everwhere. We will use instance specific overrides to address the primary dev region needs.   
+   
 ```json
 {
-  "aws_account_id": "2222222222222",
+  "cluster_log_retention": "30",
+  "alert_channel": "nonprod",
+
+  "management_node_group_capacity_type": "ON_DEMAND",
+  "management_node_group_desired_size": "8",
+  "management_node_group_max_size": "12",
+  "management_node_group_min_size": "8",
+
   "baseline_node_group_capacity_type": "ON_DEMAND",
-  "baseline_node_group_desired_size": "10",
-  "baseline_node_group_max_size": "12",
-  "baseline_node_group_min_size": "10",
+  "baseline_node_group_desired_size": "30",
+  "baseline_node_group_max_size": "32",
+  "baseline_node_group_min_size": "30",
 
-  "surge_node_group_desired_size": "3",
+  "surge_node_group_capacity_type": "SPOT",
+  "surge_node_group_desired_size": "1",
   "surge_node_group_max_size": "100",
   "surge_node_group_min_size": "1"
 }
 ```
 
-Now, we return to the role/instance json to add instance specific info. In this case that means region details and the additional default overrides for the primary development regions.
+**environments/prod.json**  
 
-**environments/dev-deploy.json**  
 ```json
 {
-  "filter": "*on-push-main",
-  "infra-dev": {
-    "infra-dev-us-west-2": {
-      "aws_region": "us-west-2"
-    },
-    "infra-dev-us-east-2": {
-      "aws_region": "us-east-2"
-      },
-    "infra-dev-eu-west-1": {
-      "aws_region": "eu-west-1"
-    },
-    "infra-dev-eu-central-1": {
-      "aws_region": "eu-central-2"
-    }
-  }
-}
-```
+  "cluster_log_retention": "90",
+  "alert_channel": "prod",
 
-**environments/release.json**   
-```json
-{
-  "filter": "*on-tag-main",
-  "nonprod": {
-    "nonprod1-us-west-2": {
-      "aws_region": "us-west-2",
-      "baseline_node_group_desired_size": "30",
-      "baseline_node_group_max_size": "35",
-      "baseline_node_group_min_size": "30",
-      "surge_node_group_desired_size": "30",
-      "surge_node_group_max_size": "150",
-      "surge_node_group_min_size": "1"
-    },
-    "nonprod1-us-east-2": {
-      "aws_region": "us-east-2",
-      "baseline_node_group_desired_size": "30",
-      "baseline_node_group_max_size": "35",
-      "baseline_node_group_min_size": "30",
-      "surge_node_group_desired_size": "3",
-      "surge_node_group_max_size": "150",
-      "surge_node_group_min_size": "1"
-    },
-    "nonprod1-eu-west-1": {
-      "aws_region": "eu-west-1"
-    },
-    "nonprod1-eu-central-1": {
-      "aws_region": "eu-central-1"
-    },
-    "nonprod1-ap-southeast-2": {
-      "aws_region": "ap-southeast-2"
-    },
-    "nonprod1-ap-southwest-1": {
-      "aws_region": "ap-southwest-1"
-    }
-  },
-  "prod": {
-    "prod1-us-west-2": {
-      "aws_region": "us-west-2"
-    },
-    "prod1-us-east-2": {
-      "aws_region": "us-east-2"
-    },
-    "prod1-eu-west-1": {
-      "aws_region": "eu-west-1"
-    },
-    "prod1-eu-central-1": {
-      "aws_region": "eu-central-1"
-    },
-    "prod1-ap-southeast-2": {
-      "aws_region": "ap-southeast-2"
-    },
-    "prod1-ap-southwest-1": {
-      "aws_region": "ap-southwest-1"
-    }
-  }
+  "management_node_group_capacity_type": "ON_DEMAND",
+  "management_node_group_desired_size": "5",
+  "management_node_group_max_size": "12",
+  "management_node_group_min_size": "5",
+
+  "baseline_node_group_capacity_type": "ON_DEMAND",
+  "baseline_node_group_desired_size": "15",
+  "baseline_node_group_max_size": "17",
+  "baseline_node_group_min_size": "15",
+
+  "surge_node_group_capacity_type": "SPOT",
+  "surge_node_group_desired_size": "1",
+  "surge_node_group_max_size": "100",
+  "surge_node_group_min_size": "1"
 }
 ```
 
 From the above files, circlecigen will generate each specific _instance_.tfvars.json file for use as a -var-file by terraform.  
 
 Next, the pipeline files.  
 
@@ -426,15 +420,15 @@
       - launch-dynamic-pipeline:
           name: release candidate
           workflow-name: release-pipeline
           multi-config: release.json
           filters: *on-tag-main
 ```
 
-Below is a notional example of the resulting pipeline from a git-tag trigger. As you can see, this level of complexity in an infrastructure release pipeline already is likely to inspire the evolution towards a more sophisticated infrastructure management release process. The keyword being evolve. Let actual need be the cause of adoption of the more elaborate release system, but as is nearly always the case, the need to deploy will have deadlines that will be sooner than such an adoption. Use of a tool like circlecigen provides an interim step that avoids typos by maintaining a higher level of DRY.  
+Below is a notional example of the resulting pipeline from a git-tag trigger, which is labeled `release` in out multi.json. As you can see, this level of complexity in an infrastructure release pipeline already is likely to inspire the evolution towards a more sophisticated infrastructure management release process. The keyword being evolve. Let actual need be the cause of adoption of the more elaborate release system, but as is nearly always the case, the need to deploy will have deadlines that will be sooner than such an adoption.
 
 ```yaml
 version: 2.1
 
 orbs:
   continuation: circleci/continuation@0.3.1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: circlecigen Version: 0.0.3 Summary: Opinionated
+Metadata-Version: 2.1 Name: circlecigen Version: 0.0.4 Summary: Opinionated
 generation of continuation pipelines Home-page: https://github.com/
 ThoughtWorks-DPS/circlecigen Author: Nic Cheneweth Author-email: Nic Cheneweth
 thoughtworks.com> Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/
 circlecigen Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/
 circlecigen/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.10 Description-Content-Type: text/markdown
@@ -24,129 +24,116 @@
 automatically generating terraform deployment pipelines for multi-regional
 environment infrastructure. Imagine you support a globally-available
 microservice architecure that runs on EKS. This means you must create multiple
 EKS instances, spanning the supported regions, for potentially more than a
 single _environment_ role. What if Production required eks clusters in 3
 localities around the world, with additionally 2 regions per locality where
 traffic is geo-location routed to the closest in proximity. This results in six
-(6) clusters, that together actually make up just one environment - Production.
-While this is approaching a scale where a more robust infrastructre control-
-plane is required, a common intermediate step is to simply continue
-orchestrating this infrastructure via an infrastructure-pipeline while a
-decision or implementation around a more complex evolution is undertaken. In
-order to maintain DRYness in the terraform code, avoiding duplication of
-multiple instances of otherwise identical pipeline workflow jobs for each
-environment, what if instead you could define all the instances of a particular
-environment category in a single json file and the deployment pipeline is then
-generated to match at runtime? That is what this tool enables. In simplest
-terms, you define templates of _pre-approval_ and _post-approval_ circleci jobs
-that includes jinja2 style variable-substitution formatting. For all instances
-of each desired role, circlecigen will generate a deployment pipeline that has:
-* a pre-approve job for each instance, followed by * an approval step, followed
-by * a post-approve job for each instance #### Setup example for terraform
-Let's stay with the EKS example mentioned above. Assume that Production
-requires six (6) clusters in six different regions, Nonproduction likewise
-requires cluster in each of the same six regions, and an additional four
-clusters spanning two global locality are required to support the software-
-defined lifecycle of this infrastructure. Therefore we have three environment
-roles; prod, nonprod, infra-dev First, let's define the roles and number of
-instances per role. **environments/dev-deploy.json** The infra-dev role
-requires four environments, each in a unique region, and in two different
-global localities. While the overall infrastructure we have described
-ultimately spans a much wider area, a reasonable subset is sufficient for fully
-testing the build/deploy logic. Notice that we also specify a filter. This is a
-reference to the circleci filter used to trigger the pipeline. See the example
-config.yml below for full description. ```json { "filter": "*on-push-main",
-"infra-dev": { "infra-dev-us-west-2": {}, "infra-dev-us-east-2": {}, "infra-
-dev-eu-west-1": {}, "infra-dev-eu-central-2": {} } } ``` **environments/
-release.json** The release pipeline now covers all the remaining infrastructure
-instances. And note it is triggered by tag rather than push. ```json
-{ "filter": "*on-tag-main", "nonprod": { "nonprod-us-west-2": {}, "nonprod-us-
-east-2": {}, "nonprod-eu-west-1": {}, "nonprod-eu-central-2": {}, "nonprod-ap-
-southeast-2": {}, "nonprod-ap-southwest-1": {} }, "prod": { "prod-us-west-2":
-{}, "prod-us-east-2": {}, "prod-eu-west-1": {}, "prod-eu-central-2": {}, "prod-
-ap-southeast-2": {}, "prod-ap-southwest-1": {} } } ``` **environments/
-default.json** Next, create the default tfvars values. Usually, this is best
-populated with the shared-values for the initial deployment target environment,
-usually _dev_. Such as: ```json { "aws_account_id": "000000000000",
-"cluster_eks_version": "1.25", "aws_efs_csi_driver_chart_version": "2.4.0",
+(6) clusters, that together actually make up just one platform _environment_ -
+Production. While this is approaching a scale where a more robust infrastructre
+control-plane is required, a common intermediate step is to simply increase the
+dynamic deployment capabilities of the release pipeline. In order to maintain
+DRYness in the terraform code, avoiding duplication of multiple instances of
+otherwise identical pipeline workflow jobs for each environment, what if
+instead you could define all the instances of a particular environment category
+in a single json file and the deployment pipeline is then generated to match at
+runtime? That is what this tool enables. Let's call the multi-instance
+environments `Roles`. In simplest terms, you define templates of _pre-approval_
+and _post-approval_ circleci workflow jobs that include jinja2 style variable-
+substitution formatting. For all instances of each desired Role, circlecigen
+will generate a deployment pipeline that has: * a pre-approve job for each
+instance, followed by * an approval step, followed by * a post-approve job for
+each instance #### Setup example for a terraform EKS pipeline Let's stay with
+the EKS example mentioned above. Assume that Production requires six (6)
+clusters in six different regions, Nonproduction likewise requires cluster in
+each of the same six regions, and an additional three clusters spanning nearby
+global localities are required to support the software-defined lifecycle of
+this infrastructure. Therefore we have three environment Roles: infra-dev role
+that is deployed on git-push, and the nonprod and prod roles that release
+consequtively upon git-tag. Given the output of the actual deployment
+pipelines, this tool also supports generating the tfvar files for each cluster
+deployment. First, let's define the top level pipelines, roles, and instances
+definition. **environments/multi.json** The top-level json definition groups
+roles by the circleci filter that will trigger the deployment of the associated
+Roles. Within each Role, define the instances that should exist. And finally
+list any particular settings associated with an individual instances. This
+multi-environment definition also defines the top-level pipeline structure for
+other pipelines with the same infrastructure path to production and should
+probably be maintained in a globally accessible location rather than
+duplicating the file in multiple repositories. For this example we assume this
+configuration has already been added locally as a file. ```json { "infradev":
+{ "filter": "*on-push-main", "infradev": { "infradev-us-east-2":
+{ "aws_region": "us-east-2", "aws_account_id": "10100000000" }, "infradev-eu-
+west-3": { "aws_region": "us-east-2", "aws_account_id": "10100000000" },
+"infradev-ap-southeast-3": { "aws_region": "eu-west-1", "aws_account_id":
+"10100000000" } } }, "release": { "filter": "*on-tag-main", "nonprod":
+{ "nonprod-us-west-2": { "aws_region": "us-west-2", "aws_account_id":
+"20100000000" }, "nonprod-us-east-2": { "aws_region": "us-east-2",
+"aws_account_id": "20100000000" }, "nonprod-eu-west-1": { "aws_region": "eu-
+west-1", "aws_account_id": "20100000000" }, "nonprod-eu-central-1":
+{ "aws_region": "eu-central-1", "aws_account_id": "20100000000" }, "nonprod-ap-
+southeast-2": { "aws_region": "ap-southeast-2", "aws_account_id": "20100000000"
+}, "nonprod-ap-southwest-1": { "aws_region": "ap-southwest-1",
+"aws_account_id": "20100000000" } }, "prod": { "prod-us-west-2":
+{ "aws_region": "us-west-2", "aws_account_id": "30100000000" }, "prod-us-east-
+2": { "aws_region": "us-east-2", "aws_account_id": "30100000000" }, "prod-eu-
+west-1": { "aws_region": "eu-west-1", "aws_account_id": "30100000000" }, "prod-
+eu-central-1": { "aws_region": "eu-central-1", "aws_account_id": "30100000000"
+}, "prod-ap-southeast-2": { "aws_region": "ap-southeast-2", "aws_account_id":
+"30100000000" }, "prod-ap-southwest-1": { "aws_region": "ap-southwest-1",
+"aws_account_id": "30100000000" } } } } ``` **environments/default.json** Now,
+define the default values. These are settings to be applied to all instances of
+all roles: ```json { "cluster_eks_version": "1.25",
+"cluster_enabled_log_types": ["api", "audit", "authenticator",
+"controllerManager", "scheduler"], "aws_efs_csi_driver_chart_version": "2.4.0",
 "metrics_server_chart_version": "6.2.14", "kube_state_metrics_chart_version":
 "3.3.4", "cluster_autoscaler_chart_version": "9.26.0",
 "AL2_x86_64_instance_types": [ "t2.2xlarge", "t3.2xlarge", "t3a.2xlarge",
 "m5n.2xlarge", "m5.2xlarge", "m4.2xlarge" ],
 "BOTTLEROCKET_ARM_64_instance_types": [ "m7g.2xlarge", "m6g.2xlarge",
 "t4g.2xlarge" ], "management_node_group_name": "management-x86-al2-mng",
 "management_node_group_role": "management", "management_node_group_ami_type":
 "AL2_x86_64", "management_node_group_platform": "linux",
-"management_node_group_disk_size": "50", "management_node_group_capacity_type":
-"SPOT", "management_node_group_desired_size": "3",
-"management_node_group_max_size": "5", "management_node_group_min_size": "3",
-"baseline_node_group_name": "baseline-arm-rkt-mng", "baseline_node_group_role":
-"baseline", "baseline_node_group_ami_type": "BOTTLEROCKET_ARM_64",
+"management_node_group_disk_size": "50", "baseline_node_group_name": "baseline-
+arm-rkt-mng", "baseline_node_group_role": "baseline",
+"baseline_node_group_ami_type": "BOTTLEROCKET_ARM_64",
 "baseline_node_group_platform": "bottlerocket",
-"baseline_node_group_disk_size": "50", "baseline_node_group_capacity_type":
-"SPOT", "baseline_node_group_desired_size": "3",
-"baseline_node_group_max_size": "5", "baseline_node_group_min_size": "3",
-"surge_node_group_name": "surge-arm-rkt-mng", "surge_node_group_role": "surge",
-"surge_node_group_ami_type": "BOTTLEROCKET_ARM_64",
-"surge_node_group_platform": "bottlerocket", "surge_node_group_disk_size":
-"50", "surge_node_group_capacity_type": "SPOT",
-"surge_node_group_desired_size": "1", "surge_node_group_max_size": "3",
-"surge_node_group_min_size": "1" } ``` Next, define environment role overrides.
-In our example, we have three. infra-dev is the first deployment target and can
-use the above defaults. However, nonprod and prod need different values -
-though these are shared across the role. So we will create the following two
-role configuration override files. **environments/prod.json** In prod we must
-override the baseline nodegroup to use more and ON_DEMAND instances for the
-baseline (or _persistent_) pool in order to support the currently experienced
-traffic at acceptable scale up/down wiat frequency. The surge pool can use
-spot, but we want a minimum of 1, and larger surge potential than for infra-
-dev, while still constraining just how far it can grow based. And, since all of
-our production environments are in one AWS account, we can set that here as
-well. ```json { "aws_account_id": "111111111111",
+"baseline_node_group_disk_size": "50", "surge_node_group_name": "surge-arm-rkt-
+mng", "surge_node_group_role": "surge", "surge_node_group_ami_type":
+"BOTTLEROCKET_ARM_64", "surge_node_group_platform": "bottlerocket",
+"surge_node_group_disk_size": "50", } ``` Next, define Role overrides.
+**environments/infradev.json** ```json { "cluster_log_retention": "10",
+"alert_channel": "dev", "management_node_group_capacity_type": "SPOT",
+"management_node_group_desired_size": "3", "management_node_group_max_size":
+"5", "management_node_group_min_size": "3",
+"baseline_node_group_capacity_type": "SPOT",
+"baseline_node_group_desired_size": "3", "baseline_node_group_max_size": "5",
+"baseline_node_group_min_size": "3", "surge_node_group_capacity_type": "SPOT",
+"surge_node_group_desired_size": "0", "surge_node_group_max_size": "0",
+"surge_node_group_min_size": "0" } ``` **environments/nonprod.json** ```json
+{ "cluster_log_retention": "30", "alert_channel": "nonprod",
+"management_node_group_capacity_type": "ON_DEMAND",
+"management_node_group_desired_size": "8", "management_node_group_max_size":
+"12", "management_node_group_min_size": "8",
 "baseline_node_group_capacity_type": "ON_DEMAND",
-"baseline_node_group_desired_size": "30", "baseline_node_group_max_size": "35",
-"baseline_node_group_min_size": "30", "surge_node_group_desired_size": "3",
-"surge_node_group_max_size": "60", "surge_node_group_min_size": "1" } ```
-**environments/nonprod.json** In nonprod, though we modify similar overrides,
-the needs are different. Our developers only live/work in a single global area.
-So a variety of activities will only take place in the US regions. However,
-there are naturally a series of integration and functional tests that must span
-all the locals where the application will run, hence we do need somewhat larger
-scale everwhere. We will use instance specific overrides to address the primary
-dev region needs. ```json { "aws_account_id": "2222222222222",
+"baseline_node_group_desired_size": "30", "baseline_node_group_max_size": "32",
+"baseline_node_group_min_size": "30", "surge_node_group_capacity_type": "SPOT",
+"surge_node_group_desired_size": "1", "surge_node_group_max_size": "100",
+"surge_node_group_min_size": "1" } ``` **environments/prod.json** ```json
+{ "cluster_log_retention": "90", "alert_channel": "prod",
+"management_node_group_capacity_type": "ON_DEMAND",
+"management_node_group_desired_size": "5", "management_node_group_max_size":
+"12", "management_node_group_min_size": "5",
 "baseline_node_group_capacity_type": "ON_DEMAND",
-"baseline_node_group_desired_size": "10", "baseline_node_group_max_size": "12",
-"baseline_node_group_min_size": "10", "surge_node_group_desired_size": "3",
-"surge_node_group_max_size": "100", "surge_node_group_min_size": "1" } ``` Now,
-we return to the role/instance json to add instance specific info. In this case
-that means region details and the additional default overrides for the primary
-development regions. **environments/dev-deploy.json** ```json { "filter": "*on-
-push-main", "infra-dev": { "infra-dev-us-west-2": { "aws_region": "us-west-2"
-}, "infra-dev-us-east-2": { "aws_region": "us-east-2" }, "infra-dev-eu-west-1":
-{ "aws_region": "eu-west-1" }, "infra-dev-eu-central-1": { "aws_region": "eu-
-central-2" } } } ``` **environments/release.json** ```json { "filter": "*on-
-tag-main", "nonprod": { "nonprod1-us-west-2": { "aws_region": "us-west-2",
-"baseline_node_group_desired_size": "30", "baseline_node_group_max_size": "35",
-"baseline_node_group_min_size": "30", "surge_node_group_desired_size": "30",
-"surge_node_group_max_size": "150", "surge_node_group_min_size": "1" },
-"nonprod1-us-east-2": { "aws_region": "us-east-2",
-"baseline_node_group_desired_size": "30", "baseline_node_group_max_size": "35",
-"baseline_node_group_min_size": "30", "surge_node_group_desired_size": "3",
-"surge_node_group_max_size": "150", "surge_node_group_min_size": "1" },
-"nonprod1-eu-west-1": { "aws_region": "eu-west-1" }, "nonprod1-eu-central-1":
-{ "aws_region": "eu-central-1" }, "nonprod1-ap-southeast-2": { "aws_region":
-"ap-southeast-2" }, "nonprod1-ap-southwest-1": { "aws_region": "ap-southwest-1"
-} }, "prod": { "prod1-us-west-2": { "aws_region": "us-west-2" }, "prod1-us-
-east-2": { "aws_region": "us-east-2" }, "prod1-eu-west-1": { "aws_region": "eu-
-west-1" }, "prod1-eu-central-1": { "aws_region": "eu-central-1" }, "prod1-ap-
-southeast-2": { "aws_region": "ap-southeast-2" }, "prod1-ap-southwest-1":
-{ "aws_region": "ap-southwest-1" } } } ``` From the above files, circlecigen
-will generate each specific _instance_.tfvars.json file for use as a -var-file
-by terraform. Next, the pipeline files. **.circleci/config.yml** Of course you
+"baseline_node_group_desired_size": "15", "baseline_node_group_max_size": "17",
+"baseline_node_group_min_size": "15", "surge_node_group_capacity_type": "SPOT",
+"surge_node_group_desired_size": "1", "surge_node_group_max_size": "100",
+"surge_node_group_min_size": "1" } ``` From the above files, circlecigen will
+generate each specific _instance_.tfvars.json file for use as a -var-file by
+terraform. Next, the pipeline files. **.circleci/config.yml** Of course you
 must have the regular circleci pipeline file that responds to triggers and
 actually forms the basis of the generated pipeline. Everything in this file up
 through the Jobs: or workflow: directive (whichever comes first) forms the
 starting point for the generated pipeline. **.circleci/pre-approve.yml** This
 file is a template that will be populate with instance specific info when the
 pipeline is generated from within the config.yml pipeline. ```yaml - terraform/
 plan: name: {{env_instance}} change plan context: <<
@@ -199,70 +186,70 @@
 launch will use the dev-deploy.json so as to only # deploy to infra-dev
 instances. - launch-dynamic-pipeline: name: dev-build workflow-name: dev-
 environment-deployment multi-config: dev-deploy.json requires: - first job
 filters: *on-push-main # this continutation is only called when the repo is
 tagged and # passes the release.json to generate the full release pipeline -
 launch-dynamic-pipeline: name: release candidate workflow-name: release-
 pipeline multi-config: release.json filters: *on-tag-main ``` Below is a
-notional example of the resulting pipeline from a git-tag trigger. As you can
-see, this level of complexity in an infrastructure release pipeline already is
-likely to inspire the evolution towards a more sophisticated infrastructure
-management release process. The keyword being evolve. Let actual need be the
-cause of adoption of the more elaborate release system, but as is nearly always
-the case, the need to deploy will have deadlines that will be sooner than such
-an adoption. Use of a tool like circlecigen provides an interim step that
-avoids typos by maintaining a higher level of DRY. ```yaml version: 2.1 orbs:
-continuation: circleci/continuation@0.3.1 on-push-main: &on-push-main branches:
-only: /main/ tags: ignore: /.*/ on-tag-main: &on-tag-main branches: ignore:
-/.*/ tags: only: /.*/ commands: setup-commands: parameters: ... steps: ...
-static-code-test-commands: parameters: ... steps: ... before-deployment-
-commands: parameters: ... steps: ... after-deployment-commands: parameters: ...
-steps: ... workflows: version: 2 release-pipeline: jobs: - terraform/plan:
-name: nonprod-us-west-2 change plan context: << pipeline.parameters.context >>
-workspace: nonprod-us-west-2 var-file: env_test/nonprod-us-west-2.tfvars.json
-before-terraform: - set-environment filters: *on-tag-main - terraform/plan:
-name: nonprod-us-east-2 change plan context: << pipeline.parameters.context >>
-workspace: nonprod-us-east-2 var-file: env_test/nonprod-us-east-2.tfvars.json
-before-terraform: - set-environment filters: *on-tag-main - terraform/plan:
-name: nonprod-eu-west-1 change plan ... filters: *on-tag-main - terraform/plan:
-name: nonprod-eu-central-1 change plan ... filters: *on-tag-main - terraform/
-plan: name: nonprod-ap-southeast-2 change plan ... filters: *on-tag-main -
-terraform/plan: name: nonprod-ap-southwest-1 change plan ... filters: *on-tag-
-main - approve nonprod changes: type: approval requires: - nonprod-us-west-
-2 change plan - nonprod-us-east-2 change plan - nonprod-eu-west-1 change plan -
-nonprod-eu-central-1 change plan - nonprod-ap-southeast-2 change plan -
-nonprod-ap-southwest-1 change plan filters: *on-tag-main - terraform/apply:
+notional example of the resulting pipeline from a git-tag trigger, which is
+labeled `release` in out multi.json. As you can see, this level of complexity
+in an infrastructure release pipeline already is likely to inspire the
+evolution towards a more sophisticated infrastructure management release
+process. The keyword being evolve. Let actual need be the cause of adoption of
+the more elaborate release system, but as is nearly always the case, the need
+to deploy will have deadlines that will be sooner than such an adoption.
+```yaml version: 2.1 orbs: continuation: circleci/continuation@0.3.1 on-push-
+main: &on-push-main branches: only: /main/ tags: ignore: /.*/ on-tag-main: &on-
+tag-main branches: ignore: /.*/ tags: only: /.*/ commands: setup-commands:
+parameters: ... steps: ... static-code-test-commands: parameters: ... steps:
+... before-deployment-commands: parameters: ... steps: ... after-deployment-
+commands: parameters: ... steps: ... workflows: version: 2 release-pipeline:
+jobs: - terraform/plan: name: nonprod-us-west-2 change plan context: <<
+pipeline.parameters.context >> workspace: nonprod-us-west-2 var-file: env_test/
+nonprod-us-west-2.tfvars.json before-terraform: - set-environment filters: *on-
+tag-main - terraform/plan: name: nonprod-us-east-2 change plan context: <<
+pipeline.parameters.context >> workspace: nonprod-us-east-2 var-file: env_test/
+nonprod-us-east-2.tfvars.json before-terraform: - set-environment filters: *on-
+tag-main - terraform/plan: name: nonprod-eu-west-1 change plan ... filters:
+*on-tag-main - terraform/plan: name: nonprod-eu-central-1 change plan ...
+filters: *on-tag-main - terraform/plan: name: nonprod-ap-southeast-2 change
+plan ... filters: *on-tag-main - terraform/plan: name: nonprod-ap-southwest-
+1 change plan ... filters: *on-tag-main - approve nonprod changes: type:
+approval requires: - nonprod-us-west-2 change plan - nonprod-us-east-2 change
+plan - nonprod-eu-west-1 change plan - nonprod-eu-central-1 change plan -
+nonprod-ap-southeast-2 change plan - nonprod-ap-southwest-1 change plan
+filters: *on-tag-main - terraform/apply: name: apply nonprod-us-west-2 change
+plan context: << pipeline.parameters.context >> workspace: nonprod-us-west-
+2 var-file: env_test/nonprod-us-west-2.tfvars.json before-terraform: - set-
+environment after-terraform: - after-deployment-commands requires: - approve
+nonprod changes filters: *on-tag-main - terraform/apply: name: apply nonprod-
+us-east-2 change plan ... filters: *on-tag-main - terraform/apply: name: apply
+nonprod-eu-west-1 change plan ... filters: *on-tag-main - terraform/apply:
+name: apply nonprod-eu-central-1 change plan ... filters: *on-tag-main -
+terraform/apply: name: apply nonprod-ap-southeast-2 change plan ... filters:
+*on-tag-main - terraform/apply: name: apply nonprod-ap-southwest-1 change plan
+... filters: *on-tag-main - terraform/plan: name: prod-us-west-2 change plan
+context: << pipeline.parameters.context >> workspace: prod-us-west-2 var-file:
+env_test/prod-us-west-2.tfvars.json before-terraform: - set-environment
+filters: *on-tag-main requires: - approve nonprod changes - terraform/plan:
+name: nonprod-us-east-2 change plan ... filters: *on-tag-main requires: -
+approve nonprod changes - terraform/plan: name: nonprod-eu-west-1 change plan
+... filters: *on-tag-main requires: - approve nonprod changes - terraform/plan:
+name: nonprod-eu-central-1 change plan ... filters: *on-tag-main requires: -
+approve nonprod changes - terraform/plan: name: nonprod-ap-southeast-2 change
+plan ... filters: *on-tag-main requires: - approve nonprod changes - terraform/
+plan: name: nonprod-ap-southwest-1 change plan ... filters: *on-tag-main
+requires: - approve nonprod changes - approve prod changes: type: approval
+requires: - prod-us-west-2 change plan - prod-us-east-2 change plan - prod-eu-
+west-1 change plan - prod-eu-central-1 change plan - prod-ap-southeast-2 change
+plan - prod-ap-southwest-1 change plan filters: *on-tag-main - terraform/apply:
 name: apply nonprod-us-west-2 change plan context: <<
 pipeline.parameters.context >> workspace: nonprod-us-west-2 var-file: env_test/
 nonprod-us-west-2.tfvars.json before-terraform: - set-environment after-
 terraform: - after-deployment-commands requires: - approve nonprod changes
 filters: *on-tag-main - terraform/apply: name: apply nonprod-us-east-2 change
 plan ... filters: *on-tag-main - terraform/apply: name: apply nonprod-eu-west-
 1 change plan ... filters: *on-tag-main - terraform/apply: name: apply nonprod-
 eu-central-1 change plan ... filters: *on-tag-main - terraform/apply: name:
 apply nonprod-ap-southeast-2 change plan ... filters: *on-tag-main - terraform/
 apply: name: apply nonprod-ap-southwest-1 change plan ... filters: *on-tag-main
-- terraform/plan: name: prod-us-west-2 change plan context: <<
-pipeline.parameters.context >> workspace: prod-us-west-2 var-file: env_test/
-prod-us-west-2.tfvars.json before-terraform: - set-environment filters: *on-
-tag-main requires: - approve nonprod changes - terraform/plan: name: nonprod-
-us-east-2 change plan ... filters: *on-tag-main requires: - approve nonprod
-changes - terraform/plan: name: nonprod-eu-west-1 change plan ... filters: *on-
-tag-main requires: - approve nonprod changes - terraform/plan: name: nonprod-
-eu-central-1 change plan ... filters: *on-tag-main requires: - approve nonprod
-changes - terraform/plan: name: nonprod-ap-southeast-2 change plan ... filters:
-*on-tag-main requires: - approve nonprod changes - terraform/plan: name:
-nonprod-ap-southwest-1 change plan ... filters: *on-tag-main requires: -
-approve nonprod changes - approve prod changes: type: approval requires: -
-prod-us-west-2 change plan - prod-us-east-2 change plan - prod-eu-west-1 change
-plan - prod-eu-central-1 change plan - prod-ap-southeast-2 change plan - prod-
-ap-southwest-1 change plan filters: *on-tag-main - terraform/apply: name: apply
-nonprod-us-west-2 change plan context: << pipeline.parameters.context >>
-workspace: nonprod-us-west-2 var-file: env_test/nonprod-us-west-2.tfvars.json
-before-terraform: - set-environment after-terraform: - after-deployment-
-commands requires: - approve nonprod changes filters: *on-tag-main - terraform/
-apply: name: apply nonprod-us-east-2 change plan ... filters: *on-tag-main -
-terraform/apply: name: apply nonprod-eu-west-1 change plan ... filters: *on-
-tag-main - terraform/apply: name: apply nonprod-eu-central-1 change plan ...
-filters: *on-tag-main - terraform/apply: name: apply nonprod-ap-southeast-
-2 change plan ... filters: *on-tag-main - terraform/apply: name: apply nonprod-
-ap-southwest-1 change plan ... filters: *on-tag-main ```
+```
```

### Comparing `circlecigen-0.0.3/README.md` & `circlecigen-0.0.4/src/circlecigen.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: circlecigen
+Version: 0.0.4
+Summary: Opinionated generation of continuation pipelines
+Home-page: https://github.com/ThoughtWorks-DPS/circlecigen
+Author: Nic Cheneweth
+Author-email: Nic Cheneweth <nchenewe@thoughtworks.com>
+Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/circlecigen
+Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/circlecigen/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
 	<p>
 		<img alt="Thoughtworks Logo" src="https://raw.githubusercontent.com/ThoughtWorks-DPS/static/master/thoughtworks_flamingo_wave.png?sanitize=true" width=200 />
     <br />
 		<img alt="DPS Title" src="https://raw.githubusercontent.com/ThoughtWorks-DPS/static/master/EMPCPlatformStarterKitsImage.png?sanitize=true" width=350/>
 	</p>
   <br />
@@ -18,81 +34,128 @@
 pip install circlecigen
 ```
 
 ### How it works
 
 The circleci [continuation orb](https://circleci.com/developer/orbs/orb/circleci/continuation) is somewhat limited in terms of flexability in use, but when you automate the creation of the resulting new pipeline you open up some interesting opportunities. 
 
-The primary inspiration for this package is in automatically generating terraform deployment pipelines for multi-regional environment infrastructure. Imagine you support a globally-available microservice architecure that runs on EKS. This means you must create multiple EKS instances, spanning the supported regions, for potentially more than a single _environment_ role. What if Production required eks clusters in 3 localities around the world, with additionally 2 regions per locality where traffic is geo-location routed to the closest in proximity. This results in six (6) clusters, that together actually make up just one environment - Production. While this is approaching a scale where a more robust infrastructre control-plane is required, a common intermediate step is to simply continue orchestrating this infrastructure via an infrastructure-pipeline while a decision or implementation around a more complex evolution is undertaken.  
+The primary inspiration for this package is in automatically generating terraform deployment pipelines for multi-regional environment infrastructure. Imagine you support a globally-available microservice architecure that runs on EKS. This means you must create multiple EKS instances, spanning the supported regions, for potentially more than a single _environment_ role. What if Production required eks clusters in 3 localities around the world, with additionally 2 regions per locality where traffic is geo-location routed to the closest in proximity. This results in six (6) clusters, that together actually make up just one platform _environment_ - Production. While this is approaching a scale where a more robust infrastructre control-plane is required, a common intermediate step is to simply increase the dynamic deployment capabilities of the release pipeline.  
 
 In order to maintain DRYness in the terraform code, avoiding duplication of multiple instances of otherwise identical pipeline workflow jobs for each environment, what if instead you could define all the instances of a particular environment category in a single json file and the deployment pipeline is then generated to match at runtime?
 
 That is what this tool enables.  
 
-In simplest terms, you define templates of _pre-approval_ and _post-approval_ circleci jobs that includes jinja2 style variable-substitution formatting. 
+Let's call the multi-instance environments `Roles`.  
+
+In simplest terms, you define templates of _pre-approval_ and _post-approval_ circleci workflow jobs that include jinja2 style variable-substitution formatting. 
 
-For all instances of each desired role, circlecigen will generate a deployment pipeline that has:  
+For all instances of each desired Role, circlecigen will generate a deployment pipeline that has:  
 * a pre-approve job for each instance, followed by
 * an approval step, followed by
 * a post-approve job for each instance
 
-#### Setup example for terraform
+#### Setup example for a terraform EKS pipeline
 
-Let's stay with the EKS example mentioned above. Assume that Production requires six (6) clusters in six different regions, Nonproduction likewise requires cluster in each of the same six regions, and an additional four clusters spanning two global locality are required to support the software-defined lifecycle of this infrastructure. Therefore we have three environment roles; prod, nonprod, infra-dev  
+Let's stay with the EKS example mentioned above. Assume that Production requires six (6) clusters in six different regions, Nonproduction likewise requires cluster in each of the same six regions, and an additional three clusters spanning nearby global localities are required to support the software-defined lifecycle of this infrastructure. Therefore we have three environment Roles: infra-dev role that is deployed on git-push, and the nonprod and prod roles that release consequtively upon git-tag.  
 
-First, let's define the roles and number of instances per role.  
+Given the output of the actual deployment pipelines, this tool also supports generating the tfvar files for each cluster deployment.  
 
-**environments/dev-deploy.json**  
+First, let's define the top level pipelines, roles, and instances definition.   
 
-The infra-dev role requires four environments, each in a unique region, and in two different global localities. While the overall infrastructure we have described ultimately spans a much wider area, a reasonable subset is sufficient for fully testing the build/deploy logic. Notice that we also specify a filter. This is a reference to the circleci filter used to trigger the pipeline. See the example config.yml below for full description.  
+**environments/multi.json**  
 
+The top-level json definition groups roles by the circleci filter that will trigger the deployment of the associated Roles. Within each Role, define the instances that should exist. And finally list any particular settings associated with an individual instances.  
 
-```json
-{
-  "filter": "*on-push-main",
-  "infra-dev": {
-    "infra-dev-us-west-2": {},
-    "infra-dev-us-east-2": {},
-    "infra-dev-eu-west-1": {},
-    "infra-dev-eu-central-2": {}
-  }
-}
-```
+This multi-environment definition also defines the top-level pipeline structure for other pipelines with the same infrastructure path to production and should probably be maintained in a globally accessible location rather than duplicating the file in multiple repositories. For this example we assume this configuration has already been added locally as a file.  
 
-**environments/release.json**  
-The release pipeline now covers all the remaining infrastructure instances. And note it is triggered by tag rather than push.  
 ```json
 {
-  "filter": "*on-tag-main",
-  "nonprod": {
-    "nonprod-us-west-2": {},
-    "nonprod-us-east-2": {},
-    "nonprod-eu-west-1": {},
-    "nonprod-eu-central-2": {},
-    "nonprod-ap-southeast-2": {},
-    "nonprod-ap-southwest-1": {}
+  "infradev": {
+    "filter": "*on-push-main",
+    "infradev": {
+      "infradev-us-east-2": {
+        "aws_region": "us-east-2",
+        "aws_account_id": "10100000000"
+      },
+      "infradev-eu-west-3": {
+        "aws_region": "us-east-2",
+        "aws_account_id": "10100000000"
+      },
+      "infradev-ap-southeast-3": {
+        "aws_region": "eu-west-1",
+        "aws_account_id": "10100000000"
+      }
+    }
   },
-  "prod": {
-    "prod-us-west-2": {},
-    "prod-us-east-2": {},
-    "prod-eu-west-1": {},
-    "prod-eu-central-2": {},
-    "prod-ap-southeast-2": {},
-    "prod-ap-southwest-1": {}
+  "release": {
+    "filter": "*on-tag-main",
+    "nonprod": {
+      "nonprod-us-west-2": {
+        "aws_region": "us-west-2",
+        "aws_account_id": "20100000000"
+      },
+      "nonprod-us-east-2": {
+        "aws_region": "us-east-2",
+        "aws_account_id": "20100000000"
+      },
+      "nonprod-eu-west-1": {
+        "aws_region": "eu-west-1",
+        "aws_account_id": "20100000000"
+      },
+      "nonprod-eu-central-1": {
+        "aws_region": "eu-central-1",
+        "aws_account_id": "20100000000"
+      },
+      "nonprod-ap-southeast-2": {
+        "aws_region": "ap-southeast-2",
+        "aws_account_id": "20100000000"
+      },
+      "nonprod-ap-southwest-1": {
+        "aws_region": "ap-southwest-1",
+        "aws_account_id": "20100000000"
+      }
+    },
+    "prod": {
+      "prod-us-west-2": {
+        "aws_region": "us-west-2",
+        "aws_account_id": "30100000000"
+      },
+      "prod-us-east-2": {
+        "aws_region": "us-east-2",
+        "aws_account_id": "30100000000"
+      },
+      "prod-eu-west-1": {
+        "aws_region": "eu-west-1",
+        "aws_account_id": "30100000000"
+      },
+      "prod-eu-central-1": {
+        "aws_region": "eu-central-1",
+        "aws_account_id": "30100000000"
+      },
+      "prod-ap-southeast-2": {
+        "aws_region": "ap-southeast-2",
+        "aws_account_id": "30100000000"
+      },
+      "prod-ap-southwest-1": {
+        "aws_region": "ap-southwest-1",
+        "aws_account_id": "30100000000"
+      }
+    }
   }
 }
 ```
 
 **environments/default.json**   
 
-Next, create the default tfvars values. Usually, this is best populated with the shared-values for the initial deployment target environment, usually _dev_. Such as:  
+
+Now, define the default values. These are settings to be applied to all instances of all roles:  
 ```json
 {
-  "aws_account_id": "000000000000",
   "cluster_eks_version": "1.25",
+  "cluster_enabled_log_types": ["api", "audit", "authenticator", "controllerManager", "scheduler"],
   "aws_efs_csi_driver_chart_version": "2.4.0",
   "metrics_server_chart_version": "6.2.14",
   "kube_state_metrics_chart_version": "3.3.4",
   "cluster_autoscaler_chart_version": "9.26.0",
 
   "AL2_x86_64_instance_types": [
     "t2.2xlarge",
@@ -109,154 +172,101 @@
   ],
 
   "management_node_group_name": "management-x86-al2-mng",
   "management_node_group_role": "management",
   "management_node_group_ami_type": "AL2_x86_64",
   "management_node_group_platform": "linux",
   "management_node_group_disk_size": "50",
-  "management_node_group_capacity_type": "SPOT",
-  "management_node_group_desired_size": "3",
-  "management_node_group_max_size": "5",
-  "management_node_group_min_size": "3",
 
   "baseline_node_group_name": "baseline-arm-rkt-mng",
   "baseline_node_group_role": "baseline",
   "baseline_node_group_ami_type": "BOTTLEROCKET_ARM_64",
   "baseline_node_group_platform": "bottlerocket",
   "baseline_node_group_disk_size": "50",
-  "baseline_node_group_capacity_type": "SPOT",
-  "baseline_node_group_desired_size": "3",
-  "baseline_node_group_max_size": "5",
-  "baseline_node_group_min_size": "3",
 
   "surge_node_group_name": "surge-arm-rkt-mng",
   "surge_node_group_role": "surge",
   "surge_node_group_ami_type": "BOTTLEROCKET_ARM_64",
   "surge_node_group_platform": "bottlerocket",
   "surge_node_group_disk_size": "50",
-  "surge_node_group_capacity_type": "SPOT",
-  "surge_node_group_desired_size": "1",
-  "surge_node_group_max_size": "3",
-  "surge_node_group_min_size": "1"
+  
 }
 ```
-Next, define environment role overrides. In our example, we have three. infra-dev is the first deployment target and can use the above defaults. However, nonprod and prod need different values - though these are shared across the role. So we will create the following two role configuration override files.  
 
-**environments/prod.json**  
-In prod we must override the baseline nodegroup to use more and ON_DEMAND instances for the baseline (or _persistent_) pool in order to support the currently experienced traffic at acceptable scale up/down wiat frequency. The surge pool can use spot, but we want a minimum of 1, and larger surge potential than for infra-dev, while still constraining just how far it can grow based. And, since all of our production environments are in one AWS account, we can set that here as well.   
+Next, define Role overrides.
+
+**environments/infradev.json**  
+
 ```json
 {
-  "aws_account_id": "111111111111",
-  "baseline_node_group_capacity_type": "ON_DEMAND",
-  "baseline_node_group_desired_size": "30",
-  "baseline_node_group_max_size": "35",
-  "baseline_node_group_min_size": "30",
+  "cluster_log_retention": "10",
+  "alert_channel": "dev",
 
-  "surge_node_group_desired_size": "3",
-  "surge_node_group_max_size": "60",
-  "surge_node_group_min_size": "1"
+  "management_node_group_capacity_type": "SPOT",
+  "management_node_group_desired_size": "3",
+  "management_node_group_max_size": "5",
+  "management_node_group_min_size": "3",
+
+  "baseline_node_group_capacity_type": "SPOT",
+  "baseline_node_group_desired_size": "3",
+  "baseline_node_group_max_size": "5",
+  "baseline_node_group_min_size": "3",
+
+  "surge_node_group_capacity_type": "SPOT",
+  "surge_node_group_desired_size": "0",
+  "surge_node_group_max_size": "0",
+  "surge_node_group_min_size": "0"
 }
 ```
 
 **environments/nonprod.json**  
-
-In nonprod, though we modify similar overrides, the needs are different. Our developers only live/work in a single global area. So a variety of activities will only take place in the US regions. However, there are naturally a series of integration and functional tests that must span all the locals where the application will run, hence we do need somewhat larger scale everwhere. We will use instance specific overrides to address the primary dev region needs.   
+   
 ```json
 {
-  "aws_account_id": "2222222222222",
+  "cluster_log_retention": "30",
+  "alert_channel": "nonprod",
+
+  "management_node_group_capacity_type": "ON_DEMAND",
+  "management_node_group_desired_size": "8",
+  "management_node_group_max_size": "12",
+  "management_node_group_min_size": "8",
+
   "baseline_node_group_capacity_type": "ON_DEMAND",
-  "baseline_node_group_desired_size": "10",
-  "baseline_node_group_max_size": "12",
-  "baseline_node_group_min_size": "10",
+  "baseline_node_group_desired_size": "30",
+  "baseline_node_group_max_size": "32",
+  "baseline_node_group_min_size": "30",
 
-  "surge_node_group_desired_size": "3",
+  "surge_node_group_capacity_type": "SPOT",
+  "surge_node_group_desired_size": "1",
   "surge_node_group_max_size": "100",
   "surge_node_group_min_size": "1"
 }
 ```
 
-Now, we return to the role/instance json to add instance specific info. In this case that means region details and the additional default overrides for the primary development regions.
+**environments/prod.json**  
 
-**environments/dev-deploy.json**  
 ```json
 {
-  "filter": "*on-push-main",
-  "infra-dev": {
-    "infra-dev-us-west-2": {
-      "aws_region": "us-west-2"
-    },
-    "infra-dev-us-east-2": {
-      "aws_region": "us-east-2"
-      },
-    "infra-dev-eu-west-1": {
-      "aws_region": "eu-west-1"
-    },
-    "infra-dev-eu-central-1": {
-      "aws_region": "eu-central-2"
-    }
-  }
-}
-```
+  "cluster_log_retention": "90",
+  "alert_channel": "prod",
 
-**environments/release.json**   
-```json
-{
-  "filter": "*on-tag-main",
-  "nonprod": {
-    "nonprod1-us-west-2": {
-      "aws_region": "us-west-2",
-      "baseline_node_group_desired_size": "30",
-      "baseline_node_group_max_size": "35",
-      "baseline_node_group_min_size": "30",
-      "surge_node_group_desired_size": "30",
-      "surge_node_group_max_size": "150",
-      "surge_node_group_min_size": "1"
-    },
-    "nonprod1-us-east-2": {
-      "aws_region": "us-east-2",
-      "baseline_node_group_desired_size": "30",
-      "baseline_node_group_max_size": "35",
-      "baseline_node_group_min_size": "30",
-      "surge_node_group_desired_size": "3",
-      "surge_node_group_max_size": "150",
-      "surge_node_group_min_size": "1"
-    },
-    "nonprod1-eu-west-1": {
-      "aws_region": "eu-west-1"
-    },
-    "nonprod1-eu-central-1": {
-      "aws_region": "eu-central-1"
-    },
-    "nonprod1-ap-southeast-2": {
-      "aws_region": "ap-southeast-2"
-    },
-    "nonprod1-ap-southwest-1": {
-      "aws_region": "ap-southwest-1"
-    }
-  },
-  "prod": {
-    "prod1-us-west-2": {
-      "aws_region": "us-west-2"
-    },
-    "prod1-us-east-2": {
-      "aws_region": "us-east-2"
-    },
-    "prod1-eu-west-1": {
-      "aws_region": "eu-west-1"
-    },
-    "prod1-eu-central-1": {
-      "aws_region": "eu-central-1"
-    },
-    "prod1-ap-southeast-2": {
-      "aws_region": "ap-southeast-2"
-    },
-    "prod1-ap-southwest-1": {
-      "aws_region": "ap-southwest-1"
-    }
-  }
+  "management_node_group_capacity_type": "ON_DEMAND",
+  "management_node_group_desired_size": "5",
+  "management_node_group_max_size": "12",
+  "management_node_group_min_size": "5",
+
+  "baseline_node_group_capacity_type": "ON_DEMAND",
+  "baseline_node_group_desired_size": "15",
+  "baseline_node_group_max_size": "17",
+  "baseline_node_group_min_size": "15",
+
+  "surge_node_group_capacity_type": "SPOT",
+  "surge_node_group_desired_size": "1",
+  "surge_node_group_max_size": "100",
+  "surge_node_group_min_size": "1"
 }
 ```
 
 From the above files, circlecigen will generate each specific _instance_.tfvars.json file for use as a -var-file by terraform.  
 
 Next, the pipeline files.  
 
@@ -410,15 +420,15 @@
       - launch-dynamic-pipeline:
           name: release candidate
           workflow-name: release-pipeline
           multi-config: release.json
           filters: *on-tag-main
 ```
 
-Below is a notional example of the resulting pipeline from a git-tag trigger. As you can see, this level of complexity in an infrastructure release pipeline already is likely to inspire the evolution towards a more sophisticated infrastructure management release process. The keyword being evolve. Let actual need be the cause of adoption of the more elaborate release system, but as is nearly always the case, the need to deploy will have deadlines that will be sooner than such an adoption. Use of a tool like circlecigen provides an interim step that avoids typos by maintaining a higher level of DRY.  
+Below is a notional example of the resulting pipeline from a git-tag trigger, which is labeled `release` in out multi.json. As you can see, this level of complexity in an infrastructure release pipeline already is likely to inspire the evolution towards a more sophisticated infrastructure management release process. The keyword being evolve. Let actual need be the cause of adoption of the more elaborate release system, but as is nearly always the case, the need to deploy will have deadlines that will be sooner than such an adoption.
 
 ```yaml
 version: 2.1
 
 orbs:
   continuation: circleci/continuation@0.3.1
 
@@ -643,8 +653,8 @@
           ...
           filters: *on-tag-main
 
       - terraform/apply:
           name: apply nonprod-ap-southwest-1 change plan
           ...
           filters: *on-tag-main
-```
+```
```

#### html2text {}

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1 Name: circlecigen Version: 0.0.4 Summary: Opinionated
+generation of continuation pipelines Home-page: https://github.com/
+ThoughtWorks-DPS/circlecigen Author: Nic Cheneweth Author-email: Nic Cheneweth
+thoughtworks.com> Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/
+circlecigen Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/
+circlecigen/issues Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3.10 Description-Content-Type: text/markdown
+License-File: LICENSE
                              [Thoughtworks Logo]
                                   [DPS Title]
 
                              **** circlecigen ****
 [https://dl.circleci.com/status-badge/img/gh/ThoughtWorks-DPS/circlecigen/tree/
   main.svg?style=shield] [https://img.shields.io/badge/license-MIT-blue.svg]
 
@@ -15,129 +24,116 @@
 automatically generating terraform deployment pipelines for multi-regional
 environment infrastructure. Imagine you support a globally-available
 microservice architecure that runs on EKS. This means you must create multiple
 EKS instances, spanning the supported regions, for potentially more than a
 single _environment_ role. What if Production required eks clusters in 3
 localities around the world, with additionally 2 regions per locality where
 traffic is geo-location routed to the closest in proximity. This results in six
-(6) clusters, that together actually make up just one environment - Production.
-While this is approaching a scale where a more robust infrastructre control-
-plane is required, a common intermediate step is to simply continue
-orchestrating this infrastructure via an infrastructure-pipeline while a
-decision or implementation around a more complex evolution is undertaken. In
-order to maintain DRYness in the terraform code, avoiding duplication of
-multiple instances of otherwise identical pipeline workflow jobs for each
-environment, what if instead you could define all the instances of a particular
-environment category in a single json file and the deployment pipeline is then
-generated to match at runtime? That is what this tool enables. In simplest
-terms, you define templates of _pre-approval_ and _post-approval_ circleci jobs
-that includes jinja2 style variable-substitution formatting. For all instances
-of each desired role, circlecigen will generate a deployment pipeline that has:
-* a pre-approve job for each instance, followed by * an approval step, followed
-by * a post-approve job for each instance #### Setup example for terraform
-Let's stay with the EKS example mentioned above. Assume that Production
-requires six (6) clusters in six different regions, Nonproduction likewise
-requires cluster in each of the same six regions, and an additional four
-clusters spanning two global locality are required to support the software-
-defined lifecycle of this infrastructure. Therefore we have three environment
-roles; prod, nonprod, infra-dev First, let's define the roles and number of
-instances per role. **environments/dev-deploy.json** The infra-dev role
-requires four environments, each in a unique region, and in two different
-global localities. While the overall infrastructure we have described
-ultimately spans a much wider area, a reasonable subset is sufficient for fully
-testing the build/deploy logic. Notice that we also specify a filter. This is a
-reference to the circleci filter used to trigger the pipeline. See the example
-config.yml below for full description. ```json { "filter": "*on-push-main",
-"infra-dev": { "infra-dev-us-west-2": {}, "infra-dev-us-east-2": {}, "infra-
-dev-eu-west-1": {}, "infra-dev-eu-central-2": {} } } ``` **environments/
-release.json** The release pipeline now covers all the remaining infrastructure
-instances. And note it is triggered by tag rather than push. ```json
-{ "filter": "*on-tag-main", "nonprod": { "nonprod-us-west-2": {}, "nonprod-us-
-east-2": {}, "nonprod-eu-west-1": {}, "nonprod-eu-central-2": {}, "nonprod-ap-
-southeast-2": {}, "nonprod-ap-southwest-1": {} }, "prod": { "prod-us-west-2":
-{}, "prod-us-east-2": {}, "prod-eu-west-1": {}, "prod-eu-central-2": {}, "prod-
-ap-southeast-2": {}, "prod-ap-southwest-1": {} } } ``` **environments/
-default.json** Next, create the default tfvars values. Usually, this is best
-populated with the shared-values for the initial deployment target environment,
-usually _dev_. Such as: ```json { "aws_account_id": "000000000000",
-"cluster_eks_version": "1.25", "aws_efs_csi_driver_chart_version": "2.4.0",
+(6) clusters, that together actually make up just one platform _environment_ -
+Production. While this is approaching a scale where a more robust infrastructre
+control-plane is required, a common intermediate step is to simply increase the
+dynamic deployment capabilities of the release pipeline. In order to maintain
+DRYness in the terraform code, avoiding duplication of multiple instances of
+otherwise identical pipeline workflow jobs for each environment, what if
+instead you could define all the instances of a particular environment category
+in a single json file and the deployment pipeline is then generated to match at
+runtime? That is what this tool enables. Let's call the multi-instance
+environments `Roles`. In simplest terms, you define templates of _pre-approval_
+and _post-approval_ circleci workflow jobs that include jinja2 style variable-
+substitution formatting. For all instances of each desired Role, circlecigen
+will generate a deployment pipeline that has: * a pre-approve job for each
+instance, followed by * an approval step, followed by * a post-approve job for
+each instance #### Setup example for a terraform EKS pipeline Let's stay with
+the EKS example mentioned above. Assume that Production requires six (6)
+clusters in six different regions, Nonproduction likewise requires cluster in
+each of the same six regions, and an additional three clusters spanning nearby
+global localities are required to support the software-defined lifecycle of
+this infrastructure. Therefore we have three environment Roles: infra-dev role
+that is deployed on git-push, and the nonprod and prod roles that release
+consequtively upon git-tag. Given the output of the actual deployment
+pipelines, this tool also supports generating the tfvar files for each cluster
+deployment. First, let's define the top level pipelines, roles, and instances
+definition. **environments/multi.json** The top-level json definition groups
+roles by the circleci filter that will trigger the deployment of the associated
+Roles. Within each Role, define the instances that should exist. And finally
+list any particular settings associated with an individual instances. This
+multi-environment definition also defines the top-level pipeline structure for
+other pipelines with the same infrastructure path to production and should
+probably be maintained in a globally accessible location rather than
+duplicating the file in multiple repositories. For this example we assume this
+configuration has already been added locally as a file. ```json { "infradev":
+{ "filter": "*on-push-main", "infradev": { "infradev-us-east-2":
+{ "aws_region": "us-east-2", "aws_account_id": "10100000000" }, "infradev-eu-
+west-3": { "aws_region": "us-east-2", "aws_account_id": "10100000000" },
+"infradev-ap-southeast-3": { "aws_region": "eu-west-1", "aws_account_id":
+"10100000000" } } }, "release": { "filter": "*on-tag-main", "nonprod":
+{ "nonprod-us-west-2": { "aws_region": "us-west-2", "aws_account_id":
+"20100000000" }, "nonprod-us-east-2": { "aws_region": "us-east-2",
+"aws_account_id": "20100000000" }, "nonprod-eu-west-1": { "aws_region": "eu-
+west-1", "aws_account_id": "20100000000" }, "nonprod-eu-central-1":
+{ "aws_region": "eu-central-1", "aws_account_id": "20100000000" }, "nonprod-ap-
+southeast-2": { "aws_region": "ap-southeast-2", "aws_account_id": "20100000000"
+}, "nonprod-ap-southwest-1": { "aws_region": "ap-southwest-1",
+"aws_account_id": "20100000000" } }, "prod": { "prod-us-west-2":
+{ "aws_region": "us-west-2", "aws_account_id": "30100000000" }, "prod-us-east-
+2": { "aws_region": "us-east-2", "aws_account_id": "30100000000" }, "prod-eu-
+west-1": { "aws_region": "eu-west-1", "aws_account_id": "30100000000" }, "prod-
+eu-central-1": { "aws_region": "eu-central-1", "aws_account_id": "30100000000"
+}, "prod-ap-southeast-2": { "aws_region": "ap-southeast-2", "aws_account_id":
+"30100000000" }, "prod-ap-southwest-1": { "aws_region": "ap-southwest-1",
+"aws_account_id": "30100000000" } } } } ``` **environments/default.json** Now,
+define the default values. These are settings to be applied to all instances of
+all roles: ```json { "cluster_eks_version": "1.25",
+"cluster_enabled_log_types": ["api", "audit", "authenticator",
+"controllerManager", "scheduler"], "aws_efs_csi_driver_chart_version": "2.4.0",
 "metrics_server_chart_version": "6.2.14", "kube_state_metrics_chart_version":
 "3.3.4", "cluster_autoscaler_chart_version": "9.26.0",
 "AL2_x86_64_instance_types": [ "t2.2xlarge", "t3.2xlarge", "t3a.2xlarge",
 "m5n.2xlarge", "m5.2xlarge", "m4.2xlarge" ],
 "BOTTLEROCKET_ARM_64_instance_types": [ "m7g.2xlarge", "m6g.2xlarge",
 "t4g.2xlarge" ], "management_node_group_name": "management-x86-al2-mng",
 "management_node_group_role": "management", "management_node_group_ami_type":
 "AL2_x86_64", "management_node_group_platform": "linux",
-"management_node_group_disk_size": "50", "management_node_group_capacity_type":
-"SPOT", "management_node_group_desired_size": "3",
-"management_node_group_max_size": "5", "management_node_group_min_size": "3",
-"baseline_node_group_name": "baseline-arm-rkt-mng", "baseline_node_group_role":
-"baseline", "baseline_node_group_ami_type": "BOTTLEROCKET_ARM_64",
+"management_node_group_disk_size": "50", "baseline_node_group_name": "baseline-
+arm-rkt-mng", "baseline_node_group_role": "baseline",
+"baseline_node_group_ami_type": "BOTTLEROCKET_ARM_64",
 "baseline_node_group_platform": "bottlerocket",
-"baseline_node_group_disk_size": "50", "baseline_node_group_capacity_type":
-"SPOT", "baseline_node_group_desired_size": "3",
-"baseline_node_group_max_size": "5", "baseline_node_group_min_size": "3",
-"surge_node_group_name": "surge-arm-rkt-mng", "surge_node_group_role": "surge",
-"surge_node_group_ami_type": "BOTTLEROCKET_ARM_64",
-"surge_node_group_platform": "bottlerocket", "surge_node_group_disk_size":
-"50", "surge_node_group_capacity_type": "SPOT",
-"surge_node_group_desired_size": "1", "surge_node_group_max_size": "3",
-"surge_node_group_min_size": "1" } ``` Next, define environment role overrides.
-In our example, we have three. infra-dev is the first deployment target and can
-use the above defaults. However, nonprod and prod need different values -
-though these are shared across the role. So we will create the following two
-role configuration override files. **environments/prod.json** In prod we must
-override the baseline nodegroup to use more and ON_DEMAND instances for the
-baseline (or _persistent_) pool in order to support the currently experienced
-traffic at acceptable scale up/down wiat frequency. The surge pool can use
-spot, but we want a minimum of 1, and larger surge potential than for infra-
-dev, while still constraining just how far it can grow based. And, since all of
-our production environments are in one AWS account, we can set that here as
-well. ```json { "aws_account_id": "111111111111",
+"baseline_node_group_disk_size": "50", "surge_node_group_name": "surge-arm-rkt-
+mng", "surge_node_group_role": "surge", "surge_node_group_ami_type":
+"BOTTLEROCKET_ARM_64", "surge_node_group_platform": "bottlerocket",
+"surge_node_group_disk_size": "50", } ``` Next, define Role overrides.
+**environments/infradev.json** ```json { "cluster_log_retention": "10",
+"alert_channel": "dev", "management_node_group_capacity_type": "SPOT",
+"management_node_group_desired_size": "3", "management_node_group_max_size":
+"5", "management_node_group_min_size": "3",
+"baseline_node_group_capacity_type": "SPOT",
+"baseline_node_group_desired_size": "3", "baseline_node_group_max_size": "5",
+"baseline_node_group_min_size": "3", "surge_node_group_capacity_type": "SPOT",
+"surge_node_group_desired_size": "0", "surge_node_group_max_size": "0",
+"surge_node_group_min_size": "0" } ``` **environments/nonprod.json** ```json
+{ "cluster_log_retention": "30", "alert_channel": "nonprod",
+"management_node_group_capacity_type": "ON_DEMAND",
+"management_node_group_desired_size": "8", "management_node_group_max_size":
+"12", "management_node_group_min_size": "8",
 "baseline_node_group_capacity_type": "ON_DEMAND",
-"baseline_node_group_desired_size": "30", "baseline_node_group_max_size": "35",
-"baseline_node_group_min_size": "30", "surge_node_group_desired_size": "3",
-"surge_node_group_max_size": "60", "surge_node_group_min_size": "1" } ```
-**environments/nonprod.json** In nonprod, though we modify similar overrides,
-the needs are different. Our developers only live/work in a single global area.
-So a variety of activities will only take place in the US regions. However,
-there are naturally a series of integration and functional tests that must span
-all the locals where the application will run, hence we do need somewhat larger
-scale everwhere. We will use instance specific overrides to address the primary
-dev region needs. ```json { "aws_account_id": "2222222222222",
+"baseline_node_group_desired_size": "30", "baseline_node_group_max_size": "32",
+"baseline_node_group_min_size": "30", "surge_node_group_capacity_type": "SPOT",
+"surge_node_group_desired_size": "1", "surge_node_group_max_size": "100",
+"surge_node_group_min_size": "1" } ``` **environments/prod.json** ```json
+{ "cluster_log_retention": "90", "alert_channel": "prod",
+"management_node_group_capacity_type": "ON_DEMAND",
+"management_node_group_desired_size": "5", "management_node_group_max_size":
+"12", "management_node_group_min_size": "5",
 "baseline_node_group_capacity_type": "ON_DEMAND",
-"baseline_node_group_desired_size": "10", "baseline_node_group_max_size": "12",
-"baseline_node_group_min_size": "10", "surge_node_group_desired_size": "3",
-"surge_node_group_max_size": "100", "surge_node_group_min_size": "1" } ``` Now,
-we return to the role/instance json to add instance specific info. In this case
-that means region details and the additional default overrides for the primary
-development regions. **environments/dev-deploy.json** ```json { "filter": "*on-
-push-main", "infra-dev": { "infra-dev-us-west-2": { "aws_region": "us-west-2"
-}, "infra-dev-us-east-2": { "aws_region": "us-east-2" }, "infra-dev-eu-west-1":
-{ "aws_region": "eu-west-1" }, "infra-dev-eu-central-1": { "aws_region": "eu-
-central-2" } } } ``` **environments/release.json** ```json { "filter": "*on-
-tag-main", "nonprod": { "nonprod1-us-west-2": { "aws_region": "us-west-2",
-"baseline_node_group_desired_size": "30", "baseline_node_group_max_size": "35",
-"baseline_node_group_min_size": "30", "surge_node_group_desired_size": "30",
-"surge_node_group_max_size": "150", "surge_node_group_min_size": "1" },
-"nonprod1-us-east-2": { "aws_region": "us-east-2",
-"baseline_node_group_desired_size": "30", "baseline_node_group_max_size": "35",
-"baseline_node_group_min_size": "30", "surge_node_group_desired_size": "3",
-"surge_node_group_max_size": "150", "surge_node_group_min_size": "1" },
-"nonprod1-eu-west-1": { "aws_region": "eu-west-1" }, "nonprod1-eu-central-1":
-{ "aws_region": "eu-central-1" }, "nonprod1-ap-southeast-2": { "aws_region":
-"ap-southeast-2" }, "nonprod1-ap-southwest-1": { "aws_region": "ap-southwest-1"
-} }, "prod": { "prod1-us-west-2": { "aws_region": "us-west-2" }, "prod1-us-
-east-2": { "aws_region": "us-east-2" }, "prod1-eu-west-1": { "aws_region": "eu-
-west-1" }, "prod1-eu-central-1": { "aws_region": "eu-central-1" }, "prod1-ap-
-southeast-2": { "aws_region": "ap-southeast-2" }, "prod1-ap-southwest-1":
-{ "aws_region": "ap-southwest-1" } } } ``` From the above files, circlecigen
-will generate each specific _instance_.tfvars.json file for use as a -var-file
-by terraform. Next, the pipeline files. **.circleci/config.yml** Of course you
+"baseline_node_group_desired_size": "15", "baseline_node_group_max_size": "17",
+"baseline_node_group_min_size": "15", "surge_node_group_capacity_type": "SPOT",
+"surge_node_group_desired_size": "1", "surge_node_group_max_size": "100",
+"surge_node_group_min_size": "1" } ``` From the above files, circlecigen will
+generate each specific _instance_.tfvars.json file for use as a -var-file by
+terraform. Next, the pipeline files. **.circleci/config.yml** Of course you
 must have the regular circleci pipeline file that responds to triggers and
 actually forms the basis of the generated pipeline. Everything in this file up
 through the Jobs: or workflow: directive (whichever comes first) forms the
 starting point for the generated pipeline. **.circleci/pre-approve.yml** This
 file is a template that will be populate with instance specific info when the
 pipeline is generated from within the config.yml pipeline. ```yaml - terraform/
 plan: name: {{env_instance}} change plan context: <<
@@ -190,70 +186,70 @@
 launch will use the dev-deploy.json so as to only # deploy to infra-dev
 instances. - launch-dynamic-pipeline: name: dev-build workflow-name: dev-
 environment-deployment multi-config: dev-deploy.json requires: - first job
 filters: *on-push-main # this continutation is only called when the repo is
 tagged and # passes the release.json to generate the full release pipeline -
 launch-dynamic-pipeline: name: release candidate workflow-name: release-
 pipeline multi-config: release.json filters: *on-tag-main ``` Below is a
-notional example of the resulting pipeline from a git-tag trigger. As you can
-see, this level of complexity in an infrastructure release pipeline already is
-likely to inspire the evolution towards a more sophisticated infrastructure
-management release process. The keyword being evolve. Let actual need be the
-cause of adoption of the more elaborate release system, but as is nearly always
-the case, the need to deploy will have deadlines that will be sooner than such
-an adoption. Use of a tool like circlecigen provides an interim step that
-avoids typos by maintaining a higher level of DRY. ```yaml version: 2.1 orbs:
-continuation: circleci/continuation@0.3.1 on-push-main: &on-push-main branches:
-only: /main/ tags: ignore: /.*/ on-tag-main: &on-tag-main branches: ignore:
-/.*/ tags: only: /.*/ commands: setup-commands: parameters: ... steps: ...
-static-code-test-commands: parameters: ... steps: ... before-deployment-
-commands: parameters: ... steps: ... after-deployment-commands: parameters: ...
-steps: ... workflows: version: 2 release-pipeline: jobs: - terraform/plan:
-name: nonprod-us-west-2 change plan context: << pipeline.parameters.context >>
-workspace: nonprod-us-west-2 var-file: env_test/nonprod-us-west-2.tfvars.json
-before-terraform: - set-environment filters: *on-tag-main - terraform/plan:
-name: nonprod-us-east-2 change plan context: << pipeline.parameters.context >>
-workspace: nonprod-us-east-2 var-file: env_test/nonprod-us-east-2.tfvars.json
-before-terraform: - set-environment filters: *on-tag-main - terraform/plan:
-name: nonprod-eu-west-1 change plan ... filters: *on-tag-main - terraform/plan:
-name: nonprod-eu-central-1 change plan ... filters: *on-tag-main - terraform/
-plan: name: nonprod-ap-southeast-2 change plan ... filters: *on-tag-main -
-terraform/plan: name: nonprod-ap-southwest-1 change plan ... filters: *on-tag-
-main - approve nonprod changes: type: approval requires: - nonprod-us-west-
-2 change plan - nonprod-us-east-2 change plan - nonprod-eu-west-1 change plan -
-nonprod-eu-central-1 change plan - nonprod-ap-southeast-2 change plan -
-nonprod-ap-southwest-1 change plan filters: *on-tag-main - terraform/apply:
+notional example of the resulting pipeline from a git-tag trigger, which is
+labeled `release` in out multi.json. As you can see, this level of complexity
+in an infrastructure release pipeline already is likely to inspire the
+evolution towards a more sophisticated infrastructure management release
+process. The keyword being evolve. Let actual need be the cause of adoption of
+the more elaborate release system, but as is nearly always the case, the need
+to deploy will have deadlines that will be sooner than such an adoption.
+```yaml version: 2.1 orbs: continuation: circleci/continuation@0.3.1 on-push-
+main: &on-push-main branches: only: /main/ tags: ignore: /.*/ on-tag-main: &on-
+tag-main branches: ignore: /.*/ tags: only: /.*/ commands: setup-commands:
+parameters: ... steps: ... static-code-test-commands: parameters: ... steps:
+... before-deployment-commands: parameters: ... steps: ... after-deployment-
+commands: parameters: ... steps: ... workflows: version: 2 release-pipeline:
+jobs: - terraform/plan: name: nonprod-us-west-2 change plan context: <<
+pipeline.parameters.context >> workspace: nonprod-us-west-2 var-file: env_test/
+nonprod-us-west-2.tfvars.json before-terraform: - set-environment filters: *on-
+tag-main - terraform/plan: name: nonprod-us-east-2 change plan context: <<
+pipeline.parameters.context >> workspace: nonprod-us-east-2 var-file: env_test/
+nonprod-us-east-2.tfvars.json before-terraform: - set-environment filters: *on-
+tag-main - terraform/plan: name: nonprod-eu-west-1 change plan ... filters:
+*on-tag-main - terraform/plan: name: nonprod-eu-central-1 change plan ...
+filters: *on-tag-main - terraform/plan: name: nonprod-ap-southeast-2 change
+plan ... filters: *on-tag-main - terraform/plan: name: nonprod-ap-southwest-
+1 change plan ... filters: *on-tag-main - approve nonprod changes: type:
+approval requires: - nonprod-us-west-2 change plan - nonprod-us-east-2 change
+plan - nonprod-eu-west-1 change plan - nonprod-eu-central-1 change plan -
+nonprod-ap-southeast-2 change plan - nonprod-ap-southwest-1 change plan
+filters: *on-tag-main - terraform/apply: name: apply nonprod-us-west-2 change
+plan context: << pipeline.parameters.context >> workspace: nonprod-us-west-
+2 var-file: env_test/nonprod-us-west-2.tfvars.json before-terraform: - set-
+environment after-terraform: - after-deployment-commands requires: - approve
+nonprod changes filters: *on-tag-main - terraform/apply: name: apply nonprod-
+us-east-2 change plan ... filters: *on-tag-main - terraform/apply: name: apply
+nonprod-eu-west-1 change plan ... filters: *on-tag-main - terraform/apply:
+name: apply nonprod-eu-central-1 change plan ... filters: *on-tag-main -
+terraform/apply: name: apply nonprod-ap-southeast-2 change plan ... filters:
+*on-tag-main - terraform/apply: name: apply nonprod-ap-southwest-1 change plan
+... filters: *on-tag-main - terraform/plan: name: prod-us-west-2 change plan
+context: << pipeline.parameters.context >> workspace: prod-us-west-2 var-file:
+env_test/prod-us-west-2.tfvars.json before-terraform: - set-environment
+filters: *on-tag-main requires: - approve nonprod changes - terraform/plan:
+name: nonprod-us-east-2 change plan ... filters: *on-tag-main requires: -
+approve nonprod changes - terraform/plan: name: nonprod-eu-west-1 change plan
+... filters: *on-tag-main requires: - approve nonprod changes - terraform/plan:
+name: nonprod-eu-central-1 change plan ... filters: *on-tag-main requires: -
+approve nonprod changes - terraform/plan: name: nonprod-ap-southeast-2 change
+plan ... filters: *on-tag-main requires: - approve nonprod changes - terraform/
+plan: name: nonprod-ap-southwest-1 change plan ... filters: *on-tag-main
+requires: - approve nonprod changes - approve prod changes: type: approval
+requires: - prod-us-west-2 change plan - prod-us-east-2 change plan - prod-eu-
+west-1 change plan - prod-eu-central-1 change plan - prod-ap-southeast-2 change
+plan - prod-ap-southwest-1 change plan filters: *on-tag-main - terraform/apply:
 name: apply nonprod-us-west-2 change plan context: <<
 pipeline.parameters.context >> workspace: nonprod-us-west-2 var-file: env_test/
 nonprod-us-west-2.tfvars.json before-terraform: - set-environment after-
 terraform: - after-deployment-commands requires: - approve nonprod changes
 filters: *on-tag-main - terraform/apply: name: apply nonprod-us-east-2 change
 plan ... filters: *on-tag-main - terraform/apply: name: apply nonprod-eu-west-
 1 change plan ... filters: *on-tag-main - terraform/apply: name: apply nonprod-
 eu-central-1 change plan ... filters: *on-tag-main - terraform/apply: name:
 apply nonprod-ap-southeast-2 change plan ... filters: *on-tag-main - terraform/
 apply: name: apply nonprod-ap-southwest-1 change plan ... filters: *on-tag-main
-- terraform/plan: name: prod-us-west-2 change plan context: <<
-pipeline.parameters.context >> workspace: prod-us-west-2 var-file: env_test/
-prod-us-west-2.tfvars.json before-terraform: - set-environment filters: *on-
-tag-main requires: - approve nonprod changes - terraform/plan: name: nonprod-
-us-east-2 change plan ... filters: *on-tag-main requires: - approve nonprod
-changes - terraform/plan: name: nonprod-eu-west-1 change plan ... filters: *on-
-tag-main requires: - approve nonprod changes - terraform/plan: name: nonprod-
-eu-central-1 change plan ... filters: *on-tag-main requires: - approve nonprod
-changes - terraform/plan: name: nonprod-ap-southeast-2 change plan ... filters:
-*on-tag-main requires: - approve nonprod changes - terraform/plan: name:
-nonprod-ap-southwest-1 change plan ... filters: *on-tag-main requires: -
-approve nonprod changes - approve prod changes: type: approval requires: -
-prod-us-west-2 change plan - prod-us-east-2 change plan - prod-eu-west-1 change
-plan - prod-eu-central-1 change plan - prod-ap-southeast-2 change plan - prod-
-ap-southwest-1 change plan filters: *on-tag-main - terraform/apply: name: apply
-nonprod-us-west-2 change plan context: << pipeline.parameters.context >>
-workspace: nonprod-us-west-2 var-file: env_test/nonprod-us-west-2.tfvars.json
-before-terraform: - set-environment after-terraform: - after-deployment-
-commands requires: - approve nonprod changes filters: *on-tag-main - terraform/
-apply: name: apply nonprod-us-east-2 change plan ... filters: *on-tag-main -
-terraform/apply: name: apply nonprod-eu-west-1 change plan ... filters: *on-
-tag-main - terraform/apply: name: apply nonprod-eu-central-1 change plan ...
-filters: *on-tag-main - terraform/apply: name: apply nonprod-ap-southeast-
-2 change plan ... filters: *on-tag-main - terraform/apply: name: apply nonprod-
-ap-southwest-1 change plan ... filters: *on-tag-main ```
+```
```

### Comparing `circlecigen-0.0.3/env_test/post-approve.yml` & `circlecigen-0.0.4/env_test/post-approve.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
       - terraform/apply:
           name: apply {{env_instance}} change plan
-          context: << pipeline.parameters.context >>
+          context: *context
           workspace: {{env_instance}}
           var-file: {{envpath}}/{{env_instance}}.tfvars.json
           before-terraform:
             - set-environment
           after-terraform:
             - store-system-credentials:
                 region: {{env_instance}}
```

### Comparing `circlecigen-0.0.3/pyproject.toml` & `circlecigen-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.3/setup.py` & `circlecigen-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.3/src/circlecigen.egg-info/PKG-INFO` & `circlecigen-0.0.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: circlecigen
-Version: 0.0.3
-Summary: Opinionated generation of continuation pipelines
-Home-page: https://github.com/ThoughtWorks-DPS/circlecigen
-Author: Nic Cheneweth
-Author-email: Nic Cheneweth <nchenewe@thoughtworks.com>
-Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/circlecigen
-Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/circlecigen/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
 	<p>
 		<img alt="Thoughtworks Logo" src="https://raw.githubusercontent.com/ThoughtWorks-DPS/static/master/thoughtworks_flamingo_wave.png?sanitize=true" width=200 />
     <br />
 		<img alt="DPS Title" src="https://raw.githubusercontent.com/ThoughtWorks-DPS/static/master/EMPCPlatformStarterKitsImage.png?sanitize=true" width=350/>
 	</p>
   <br />
@@ -34,81 +18,128 @@
 pip install circlecigen
 ```
 
 ### How it works
 
 The circleci [continuation orb](https://circleci.com/developer/orbs/orb/circleci/continuation) is somewhat limited in terms of flexability in use, but when you automate the creation of the resulting new pipeline you open up some interesting opportunities. 
 
-The primary inspiration for this package is in automatically generating terraform deployment pipelines for multi-regional environment infrastructure. Imagine you support a globally-available microservice architecure that runs on EKS. This means you must create multiple EKS instances, spanning the supported regions, for potentially more than a single _environment_ role. What if Production required eks clusters in 3 localities around the world, with additionally 2 regions per locality where traffic is geo-location routed to the closest in proximity. This results in six (6) clusters, that together actually make up just one environment - Production. While this is approaching a scale where a more robust infrastructre control-plane is required, a common intermediate step is to simply continue orchestrating this infrastructure via an infrastructure-pipeline while a decision or implementation around a more complex evolution is undertaken.  
+The primary inspiration for this package is in automatically generating terraform deployment pipelines for multi-regional environment infrastructure. Imagine you support a globally-available microservice architecure that runs on EKS. This means you must create multiple EKS instances, spanning the supported regions, for potentially more than a single _environment_ role. What if Production required eks clusters in 3 localities around the world, with additionally 2 regions per locality where traffic is geo-location routed to the closest in proximity. This results in six (6) clusters, that together actually make up just one platform _environment_ - Production. While this is approaching a scale where a more robust infrastructre control-plane is required, a common intermediate step is to simply increase the dynamic deployment capabilities of the release pipeline.  
 
 In order to maintain DRYness in the terraform code, avoiding duplication of multiple instances of otherwise identical pipeline workflow jobs for each environment, what if instead you could define all the instances of a particular environment category in a single json file and the deployment pipeline is then generated to match at runtime?
 
 That is what this tool enables.  
 
-In simplest terms, you define templates of _pre-approval_ and _post-approval_ circleci jobs that includes jinja2 style variable-substitution formatting. 
+Let's call the multi-instance environments `Roles`.  
+
+In simplest terms, you define templates of _pre-approval_ and _post-approval_ circleci workflow jobs that include jinja2 style variable-substitution formatting. 
 
-For all instances of each desired role, circlecigen will generate a deployment pipeline that has:  
+For all instances of each desired Role, circlecigen will generate a deployment pipeline that has:  
 * a pre-approve job for each instance, followed by
 * an approval step, followed by
 * a post-approve job for each instance
 
-#### Setup example for terraform
+#### Setup example for a terraform EKS pipeline
 
-Let's stay with the EKS example mentioned above. Assume that Production requires six (6) clusters in six different regions, Nonproduction likewise requires cluster in each of the same six regions, and an additional four clusters spanning two global locality are required to support the software-defined lifecycle of this infrastructure. Therefore we have three environment roles; prod, nonprod, infra-dev  
+Let's stay with the EKS example mentioned above. Assume that Production requires six (6) clusters in six different regions, Nonproduction likewise requires cluster in each of the same six regions, and an additional three clusters spanning nearby global localities are required to support the software-defined lifecycle of this infrastructure. Therefore we have three environment Roles: infra-dev role that is deployed on git-push, and the nonprod and prod roles that release consequtively upon git-tag.  
 
-First, let's define the roles and number of instances per role.  
+Given the output of the actual deployment pipelines, this tool also supports generating the tfvar files for each cluster deployment.  
 
-**environments/dev-deploy.json**  
+First, let's define the top level pipelines, roles, and instances definition.   
 
-The infra-dev role requires four environments, each in a unique region, and in two different global localities. While the overall infrastructure we have described ultimately spans a much wider area, a reasonable subset is sufficient for fully testing the build/deploy logic. Notice that we also specify a filter. This is a reference to the circleci filter used to trigger the pipeline. See the example config.yml below for full description.  
+**environments/multi.json**  
 
+The top-level json definition groups roles by the circleci filter that will trigger the deployment of the associated Roles. Within each Role, define the instances that should exist. And finally list any particular settings associated with an individual instances.  
 
-```json
-{
-  "filter": "*on-push-main",
-  "infra-dev": {
-    "infra-dev-us-west-2": {},
-    "infra-dev-us-east-2": {},
-    "infra-dev-eu-west-1": {},
-    "infra-dev-eu-central-2": {}
-  }
-}
-```
+This multi-environment definition also defines the top-level pipeline structure for other pipelines with the same infrastructure path to production and should probably be maintained in a globally accessible location rather than duplicating the file in multiple repositories. For this example we assume this configuration has already been added locally as a file.  
 
-**environments/release.json**  
-The release pipeline now covers all the remaining infrastructure instances. And note it is triggered by tag rather than push.  
 ```json
 {
-  "filter": "*on-tag-main",
-  "nonprod": {
-    "nonprod-us-west-2": {},
-    "nonprod-us-east-2": {},
-    "nonprod-eu-west-1": {},
-    "nonprod-eu-central-2": {},
-    "nonprod-ap-southeast-2": {},
-    "nonprod-ap-southwest-1": {}
+  "infradev": {
+    "filter": "*on-push-main",
+    "infradev": {
+      "infradev-us-east-2": {
+        "aws_region": "us-east-2",
+        "aws_account_id": "10100000000"
+      },
+      "infradev-eu-west-3": {
+        "aws_region": "us-east-2",
+        "aws_account_id": "10100000000"
+      },
+      "infradev-ap-southeast-3": {
+        "aws_region": "eu-west-1",
+        "aws_account_id": "10100000000"
+      }
+    }
   },
-  "prod": {
-    "prod-us-west-2": {},
-    "prod-us-east-2": {},
-    "prod-eu-west-1": {},
-    "prod-eu-central-2": {},
-    "prod-ap-southeast-2": {},
-    "prod-ap-southwest-1": {}
+  "release": {
+    "filter": "*on-tag-main",
+    "nonprod": {
+      "nonprod-us-west-2": {
+        "aws_region": "us-west-2",
+        "aws_account_id": "20100000000"
+      },
+      "nonprod-us-east-2": {
+        "aws_region": "us-east-2",
+        "aws_account_id": "20100000000"
+      },
+      "nonprod-eu-west-1": {
+        "aws_region": "eu-west-1",
+        "aws_account_id": "20100000000"
+      },
+      "nonprod-eu-central-1": {
+        "aws_region": "eu-central-1",
+        "aws_account_id": "20100000000"
+      },
+      "nonprod-ap-southeast-2": {
+        "aws_region": "ap-southeast-2",
+        "aws_account_id": "20100000000"
+      },
+      "nonprod-ap-southwest-1": {
+        "aws_region": "ap-southwest-1",
+        "aws_account_id": "20100000000"
+      }
+    },
+    "prod": {
+      "prod-us-west-2": {
+        "aws_region": "us-west-2",
+        "aws_account_id": "30100000000"
+      },
+      "prod-us-east-2": {
+        "aws_region": "us-east-2",
+        "aws_account_id": "30100000000"
+      },
+      "prod-eu-west-1": {
+        "aws_region": "eu-west-1",
+        "aws_account_id": "30100000000"
+      },
+      "prod-eu-central-1": {
+        "aws_region": "eu-central-1",
+        "aws_account_id": "30100000000"
+      },
+      "prod-ap-southeast-2": {
+        "aws_region": "ap-southeast-2",
+        "aws_account_id": "30100000000"
+      },
+      "prod-ap-southwest-1": {
+        "aws_region": "ap-southwest-1",
+        "aws_account_id": "30100000000"
+      }
+    }
   }
 }
 ```
 
 **environments/default.json**   
 
-Next, create the default tfvars values. Usually, this is best populated with the shared-values for the initial deployment target environment, usually _dev_. Such as:  
+
+Now, define the default values. These are settings to be applied to all instances of all roles:  
 ```json
 {
-  "aws_account_id": "000000000000",
   "cluster_eks_version": "1.25",
+  "cluster_enabled_log_types": ["api", "audit", "authenticator", "controllerManager", "scheduler"],
   "aws_efs_csi_driver_chart_version": "2.4.0",
   "metrics_server_chart_version": "6.2.14",
   "kube_state_metrics_chart_version": "3.3.4",
   "cluster_autoscaler_chart_version": "9.26.0",
 
   "AL2_x86_64_instance_types": [
     "t2.2xlarge",
@@ -125,154 +156,101 @@
   ],
 
   "management_node_group_name": "management-x86-al2-mng",
   "management_node_group_role": "management",
   "management_node_group_ami_type": "AL2_x86_64",
   "management_node_group_platform": "linux",
   "management_node_group_disk_size": "50",
-  "management_node_group_capacity_type": "SPOT",
-  "management_node_group_desired_size": "3",
-  "management_node_group_max_size": "5",
-  "management_node_group_min_size": "3",
 
   "baseline_node_group_name": "baseline-arm-rkt-mng",
   "baseline_node_group_role": "baseline",
   "baseline_node_group_ami_type": "BOTTLEROCKET_ARM_64",
   "baseline_node_group_platform": "bottlerocket",
   "baseline_node_group_disk_size": "50",
-  "baseline_node_group_capacity_type": "SPOT",
-  "baseline_node_group_desired_size": "3",
-  "baseline_node_group_max_size": "5",
-  "baseline_node_group_min_size": "3",
 
   "surge_node_group_name": "surge-arm-rkt-mng",
   "surge_node_group_role": "surge",
   "surge_node_group_ami_type": "BOTTLEROCKET_ARM_64",
   "surge_node_group_platform": "bottlerocket",
   "surge_node_group_disk_size": "50",
-  "surge_node_group_capacity_type": "SPOT",
-  "surge_node_group_desired_size": "1",
-  "surge_node_group_max_size": "3",
-  "surge_node_group_min_size": "1"
+  
 }
 ```
-Next, define environment role overrides. In our example, we have three. infra-dev is the first deployment target and can use the above defaults. However, nonprod and prod need different values - though these are shared across the role. So we will create the following two role configuration override files.  
 
-**environments/prod.json**  
-In prod we must override the baseline nodegroup to use more and ON_DEMAND instances for the baseline (or _persistent_) pool in order to support the currently experienced traffic at acceptable scale up/down wiat frequency. The surge pool can use spot, but we want a minimum of 1, and larger surge potential than for infra-dev, while still constraining just how far it can grow based. And, since all of our production environments are in one AWS account, we can set that here as well.   
+Next, define Role overrides.
+
+**environments/infradev.json**  
+
 ```json
 {
-  "aws_account_id": "111111111111",
-  "baseline_node_group_capacity_type": "ON_DEMAND",
-  "baseline_node_group_desired_size": "30",
-  "baseline_node_group_max_size": "35",
-  "baseline_node_group_min_size": "30",
+  "cluster_log_retention": "10",
+  "alert_channel": "dev",
 
-  "surge_node_group_desired_size": "3",
-  "surge_node_group_max_size": "60",
-  "surge_node_group_min_size": "1"
+  "management_node_group_capacity_type": "SPOT",
+  "management_node_group_desired_size": "3",
+  "management_node_group_max_size": "5",
+  "management_node_group_min_size": "3",
+
+  "baseline_node_group_capacity_type": "SPOT",
+  "baseline_node_group_desired_size": "3",
+  "baseline_node_group_max_size": "5",
+  "baseline_node_group_min_size": "3",
+
+  "surge_node_group_capacity_type": "SPOT",
+  "surge_node_group_desired_size": "0",
+  "surge_node_group_max_size": "0",
+  "surge_node_group_min_size": "0"
 }
 ```
 
 **environments/nonprod.json**  
-
-In nonprod, though we modify similar overrides, the needs are different. Our developers only live/work in a single global area. So a variety of activities will only take place in the US regions. However, there are naturally a series of integration and functional tests that must span all the locals where the application will run, hence we do need somewhat larger scale everwhere. We will use instance specific overrides to address the primary dev region needs.   
+   
 ```json
 {
-  "aws_account_id": "2222222222222",
+  "cluster_log_retention": "30",
+  "alert_channel": "nonprod",
+
+  "management_node_group_capacity_type": "ON_DEMAND",
+  "management_node_group_desired_size": "8",
+  "management_node_group_max_size": "12",
+  "management_node_group_min_size": "8",
+
   "baseline_node_group_capacity_type": "ON_DEMAND",
-  "baseline_node_group_desired_size": "10",
-  "baseline_node_group_max_size": "12",
-  "baseline_node_group_min_size": "10",
+  "baseline_node_group_desired_size": "30",
+  "baseline_node_group_max_size": "32",
+  "baseline_node_group_min_size": "30",
 
-  "surge_node_group_desired_size": "3",
+  "surge_node_group_capacity_type": "SPOT",
+  "surge_node_group_desired_size": "1",
   "surge_node_group_max_size": "100",
   "surge_node_group_min_size": "1"
 }
 ```
 
-Now, we return to the role/instance json to add instance specific info. In this case that means region details and the additional default overrides for the primary development regions.
+**environments/prod.json**  
 
-**environments/dev-deploy.json**  
 ```json
 {
-  "filter": "*on-push-main",
-  "infra-dev": {
-    "infra-dev-us-west-2": {
-      "aws_region": "us-west-2"
-    },
-    "infra-dev-us-east-2": {
-      "aws_region": "us-east-2"
-      },
-    "infra-dev-eu-west-1": {
-      "aws_region": "eu-west-1"
-    },
-    "infra-dev-eu-central-1": {
-      "aws_region": "eu-central-2"
-    }
-  }
-}
-```
+  "cluster_log_retention": "90",
+  "alert_channel": "prod",
 
-**environments/release.json**   
-```json
-{
-  "filter": "*on-tag-main",
-  "nonprod": {
-    "nonprod1-us-west-2": {
-      "aws_region": "us-west-2",
-      "baseline_node_group_desired_size": "30",
-      "baseline_node_group_max_size": "35",
-      "baseline_node_group_min_size": "30",
-      "surge_node_group_desired_size": "30",
-      "surge_node_group_max_size": "150",
-      "surge_node_group_min_size": "1"
-    },
-    "nonprod1-us-east-2": {
-      "aws_region": "us-east-2",
-      "baseline_node_group_desired_size": "30",
-      "baseline_node_group_max_size": "35",
-      "baseline_node_group_min_size": "30",
-      "surge_node_group_desired_size": "3",
-      "surge_node_group_max_size": "150",
-      "surge_node_group_min_size": "1"
-    },
-    "nonprod1-eu-west-1": {
-      "aws_region": "eu-west-1"
-    },
-    "nonprod1-eu-central-1": {
-      "aws_region": "eu-central-1"
-    },
-    "nonprod1-ap-southeast-2": {
-      "aws_region": "ap-southeast-2"
-    },
-    "nonprod1-ap-southwest-1": {
-      "aws_region": "ap-southwest-1"
-    }
-  },
-  "prod": {
-    "prod1-us-west-2": {
-      "aws_region": "us-west-2"
-    },
-    "prod1-us-east-2": {
-      "aws_region": "us-east-2"
-    },
-    "prod1-eu-west-1": {
-      "aws_region": "eu-west-1"
-    },
-    "prod1-eu-central-1": {
-      "aws_region": "eu-central-1"
-    },
-    "prod1-ap-southeast-2": {
-      "aws_region": "ap-southeast-2"
-    },
-    "prod1-ap-southwest-1": {
-      "aws_region": "ap-southwest-1"
-    }
-  }
+  "management_node_group_capacity_type": "ON_DEMAND",
+  "management_node_group_desired_size": "5",
+  "management_node_group_max_size": "12",
+  "management_node_group_min_size": "5",
+
+  "baseline_node_group_capacity_type": "ON_DEMAND",
+  "baseline_node_group_desired_size": "15",
+  "baseline_node_group_max_size": "17",
+  "baseline_node_group_min_size": "15",
+
+  "surge_node_group_capacity_type": "SPOT",
+  "surge_node_group_desired_size": "1",
+  "surge_node_group_max_size": "100",
+  "surge_node_group_min_size": "1"
 }
 ```
 
 From the above files, circlecigen will generate each specific _instance_.tfvars.json file for use as a -var-file by terraform.  
 
 Next, the pipeline files.  
 
@@ -426,15 +404,15 @@
       - launch-dynamic-pipeline:
           name: release candidate
           workflow-name: release-pipeline
           multi-config: release.json
           filters: *on-tag-main
 ```
 
-Below is a notional example of the resulting pipeline from a git-tag trigger. As you can see, this level of complexity in an infrastructure release pipeline already is likely to inspire the evolution towards a more sophisticated infrastructure management release process. The keyword being evolve. Let actual need be the cause of adoption of the more elaborate release system, but as is nearly always the case, the need to deploy will have deadlines that will be sooner than such an adoption. Use of a tool like circlecigen provides an interim step that avoids typos by maintaining a higher level of DRY.  
+Below is a notional example of the resulting pipeline from a git-tag trigger, which is labeled `release` in out multi.json. As you can see, this level of complexity in an infrastructure release pipeline already is likely to inspire the evolution towards a more sophisticated infrastructure management release process. The keyword being evolve. Let actual need be the cause of adoption of the more elaborate release system, but as is nearly always the case, the need to deploy will have deadlines that will be sooner than such an adoption.
 
 ```yaml
 version: 2.1
 
 orbs:
   continuation: circleci/continuation@0.3.1
 
@@ -659,8 +637,8 @@
           ...
           filters: *on-tag-main
 
       - terraform/apply:
           name: apply nonprod-ap-southwest-1 change plan
           ...
           filters: *on-tag-main
-```
+```
```

#### html2text {}

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1 Name: circlecigen Version: 0.0.3 Summary: Opinionated
-generation of continuation pipelines Home-page: https://github.com/
-ThoughtWorks-DPS/circlecigen Author: Nic Cheneweth Author-email: Nic Cheneweth
-thoughtworks.com> Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/
-circlecigen Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/
-circlecigen/issues Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.10 Description-Content-Type: text/markdown
-License-File: LICENSE
                              [Thoughtworks Logo]
                                   [DPS Title]
 
                              **** circlecigen ****
 [https://dl.circleci.com/status-badge/img/gh/ThoughtWorks-DPS/circlecigen/tree/
   main.svg?style=shield] [https://img.shields.io/badge/license-MIT-blue.svg]
 
@@ -24,129 +15,116 @@
 automatically generating terraform deployment pipelines for multi-regional
 environment infrastructure. Imagine you support a globally-available
 microservice architecure that runs on EKS. This means you must create multiple
 EKS instances, spanning the supported regions, for potentially more than a
 single _environment_ role. What if Production required eks clusters in 3
 localities around the world, with additionally 2 regions per locality where
 traffic is geo-location routed to the closest in proximity. This results in six
-(6) clusters, that together actually make up just one environment - Production.
-While this is approaching a scale where a more robust infrastructre control-
-plane is required, a common intermediate step is to simply continue
-orchestrating this infrastructure via an infrastructure-pipeline while a
-decision or implementation around a more complex evolution is undertaken. In
-order to maintain DRYness in the terraform code, avoiding duplication of
-multiple instances of otherwise identical pipeline workflow jobs for each
-environment, what if instead you could define all the instances of a particular
-environment category in a single json file and the deployment pipeline is then
-generated to match at runtime? That is what this tool enables. In simplest
-terms, you define templates of _pre-approval_ and _post-approval_ circleci jobs
-that includes jinja2 style variable-substitution formatting. For all instances
-of each desired role, circlecigen will generate a deployment pipeline that has:
-* a pre-approve job for each instance, followed by * an approval step, followed
-by * a post-approve job for each instance #### Setup example for terraform
-Let's stay with the EKS example mentioned above. Assume that Production
-requires six (6) clusters in six different regions, Nonproduction likewise
-requires cluster in each of the same six regions, and an additional four
-clusters spanning two global locality are required to support the software-
-defined lifecycle of this infrastructure. Therefore we have three environment
-roles; prod, nonprod, infra-dev First, let's define the roles and number of
-instances per role. **environments/dev-deploy.json** The infra-dev role
-requires four environments, each in a unique region, and in two different
-global localities. While the overall infrastructure we have described
-ultimately spans a much wider area, a reasonable subset is sufficient for fully
-testing the build/deploy logic. Notice that we also specify a filter. This is a
-reference to the circleci filter used to trigger the pipeline. See the example
-config.yml below for full description. ```json { "filter": "*on-push-main",
-"infra-dev": { "infra-dev-us-west-2": {}, "infra-dev-us-east-2": {}, "infra-
-dev-eu-west-1": {}, "infra-dev-eu-central-2": {} } } ``` **environments/
-release.json** The release pipeline now covers all the remaining infrastructure
-instances. And note it is triggered by tag rather than push. ```json
-{ "filter": "*on-tag-main", "nonprod": { "nonprod-us-west-2": {}, "nonprod-us-
-east-2": {}, "nonprod-eu-west-1": {}, "nonprod-eu-central-2": {}, "nonprod-ap-
-southeast-2": {}, "nonprod-ap-southwest-1": {} }, "prod": { "prod-us-west-2":
-{}, "prod-us-east-2": {}, "prod-eu-west-1": {}, "prod-eu-central-2": {}, "prod-
-ap-southeast-2": {}, "prod-ap-southwest-1": {} } } ``` **environments/
-default.json** Next, create the default tfvars values. Usually, this is best
-populated with the shared-values for the initial deployment target environment,
-usually _dev_. Such as: ```json { "aws_account_id": "000000000000",
-"cluster_eks_version": "1.25", "aws_efs_csi_driver_chart_version": "2.4.0",
+(6) clusters, that together actually make up just one platform _environment_ -
+Production. While this is approaching a scale where a more robust infrastructre
+control-plane is required, a common intermediate step is to simply increase the
+dynamic deployment capabilities of the release pipeline. In order to maintain
+DRYness in the terraform code, avoiding duplication of multiple instances of
+otherwise identical pipeline workflow jobs for each environment, what if
+instead you could define all the instances of a particular environment category
+in a single json file and the deployment pipeline is then generated to match at
+runtime? That is what this tool enables. Let's call the multi-instance
+environments `Roles`. In simplest terms, you define templates of _pre-approval_
+and _post-approval_ circleci workflow jobs that include jinja2 style variable-
+substitution formatting. For all instances of each desired Role, circlecigen
+will generate a deployment pipeline that has: * a pre-approve job for each
+instance, followed by * an approval step, followed by * a post-approve job for
+each instance #### Setup example for a terraform EKS pipeline Let's stay with
+the EKS example mentioned above. Assume that Production requires six (6)
+clusters in six different regions, Nonproduction likewise requires cluster in
+each of the same six regions, and an additional three clusters spanning nearby
+global localities are required to support the software-defined lifecycle of
+this infrastructure. Therefore we have three environment Roles: infra-dev role
+that is deployed on git-push, and the nonprod and prod roles that release
+consequtively upon git-tag. Given the output of the actual deployment
+pipelines, this tool also supports generating the tfvar files for each cluster
+deployment. First, let's define the top level pipelines, roles, and instances
+definition. **environments/multi.json** The top-level json definition groups
+roles by the circleci filter that will trigger the deployment of the associated
+Roles. Within each Role, define the instances that should exist. And finally
+list any particular settings associated with an individual instances. This
+multi-environment definition also defines the top-level pipeline structure for
+other pipelines with the same infrastructure path to production and should
+probably be maintained in a globally accessible location rather than
+duplicating the file in multiple repositories. For this example we assume this
+configuration has already been added locally as a file. ```json { "infradev":
+{ "filter": "*on-push-main", "infradev": { "infradev-us-east-2":
+{ "aws_region": "us-east-2", "aws_account_id": "10100000000" }, "infradev-eu-
+west-3": { "aws_region": "us-east-2", "aws_account_id": "10100000000" },
+"infradev-ap-southeast-3": { "aws_region": "eu-west-1", "aws_account_id":
+"10100000000" } } }, "release": { "filter": "*on-tag-main", "nonprod":
+{ "nonprod-us-west-2": { "aws_region": "us-west-2", "aws_account_id":
+"20100000000" }, "nonprod-us-east-2": { "aws_region": "us-east-2",
+"aws_account_id": "20100000000" }, "nonprod-eu-west-1": { "aws_region": "eu-
+west-1", "aws_account_id": "20100000000" }, "nonprod-eu-central-1":
+{ "aws_region": "eu-central-1", "aws_account_id": "20100000000" }, "nonprod-ap-
+southeast-2": { "aws_region": "ap-southeast-2", "aws_account_id": "20100000000"
+}, "nonprod-ap-southwest-1": { "aws_region": "ap-southwest-1",
+"aws_account_id": "20100000000" } }, "prod": { "prod-us-west-2":
+{ "aws_region": "us-west-2", "aws_account_id": "30100000000" }, "prod-us-east-
+2": { "aws_region": "us-east-2", "aws_account_id": "30100000000" }, "prod-eu-
+west-1": { "aws_region": "eu-west-1", "aws_account_id": "30100000000" }, "prod-
+eu-central-1": { "aws_region": "eu-central-1", "aws_account_id": "30100000000"
+}, "prod-ap-southeast-2": { "aws_region": "ap-southeast-2", "aws_account_id":
+"30100000000" }, "prod-ap-southwest-1": { "aws_region": "ap-southwest-1",
+"aws_account_id": "30100000000" } } } } ``` **environments/default.json** Now,
+define the default values. These are settings to be applied to all instances of
+all roles: ```json { "cluster_eks_version": "1.25",
+"cluster_enabled_log_types": ["api", "audit", "authenticator",
+"controllerManager", "scheduler"], "aws_efs_csi_driver_chart_version": "2.4.0",
 "metrics_server_chart_version": "6.2.14", "kube_state_metrics_chart_version":
 "3.3.4", "cluster_autoscaler_chart_version": "9.26.0",
 "AL2_x86_64_instance_types": [ "t2.2xlarge", "t3.2xlarge", "t3a.2xlarge",
 "m5n.2xlarge", "m5.2xlarge", "m4.2xlarge" ],
 "BOTTLEROCKET_ARM_64_instance_types": [ "m7g.2xlarge", "m6g.2xlarge",
 "t4g.2xlarge" ], "management_node_group_name": "management-x86-al2-mng",
 "management_node_group_role": "management", "management_node_group_ami_type":
 "AL2_x86_64", "management_node_group_platform": "linux",
-"management_node_group_disk_size": "50", "management_node_group_capacity_type":
-"SPOT", "management_node_group_desired_size": "3",
-"management_node_group_max_size": "5", "management_node_group_min_size": "3",
-"baseline_node_group_name": "baseline-arm-rkt-mng", "baseline_node_group_role":
-"baseline", "baseline_node_group_ami_type": "BOTTLEROCKET_ARM_64",
+"management_node_group_disk_size": "50", "baseline_node_group_name": "baseline-
+arm-rkt-mng", "baseline_node_group_role": "baseline",
+"baseline_node_group_ami_type": "BOTTLEROCKET_ARM_64",
 "baseline_node_group_platform": "bottlerocket",
-"baseline_node_group_disk_size": "50", "baseline_node_group_capacity_type":
-"SPOT", "baseline_node_group_desired_size": "3",
-"baseline_node_group_max_size": "5", "baseline_node_group_min_size": "3",
-"surge_node_group_name": "surge-arm-rkt-mng", "surge_node_group_role": "surge",
-"surge_node_group_ami_type": "BOTTLEROCKET_ARM_64",
-"surge_node_group_platform": "bottlerocket", "surge_node_group_disk_size":
-"50", "surge_node_group_capacity_type": "SPOT",
-"surge_node_group_desired_size": "1", "surge_node_group_max_size": "3",
-"surge_node_group_min_size": "1" } ``` Next, define environment role overrides.
-In our example, we have three. infra-dev is the first deployment target and can
-use the above defaults. However, nonprod and prod need different values -
-though these are shared across the role. So we will create the following two
-role configuration override files. **environments/prod.json** In prod we must
-override the baseline nodegroup to use more and ON_DEMAND instances for the
-baseline (or _persistent_) pool in order to support the currently experienced
-traffic at acceptable scale up/down wiat frequency. The surge pool can use
-spot, but we want a minimum of 1, and larger surge potential than for infra-
-dev, while still constraining just how far it can grow based. And, since all of
-our production environments are in one AWS account, we can set that here as
-well. ```json { "aws_account_id": "111111111111",
+"baseline_node_group_disk_size": "50", "surge_node_group_name": "surge-arm-rkt-
+mng", "surge_node_group_role": "surge", "surge_node_group_ami_type":
+"BOTTLEROCKET_ARM_64", "surge_node_group_platform": "bottlerocket",
+"surge_node_group_disk_size": "50", } ``` Next, define Role overrides.
+**environments/infradev.json** ```json { "cluster_log_retention": "10",
+"alert_channel": "dev", "management_node_group_capacity_type": "SPOT",
+"management_node_group_desired_size": "3", "management_node_group_max_size":
+"5", "management_node_group_min_size": "3",
+"baseline_node_group_capacity_type": "SPOT",
+"baseline_node_group_desired_size": "3", "baseline_node_group_max_size": "5",
+"baseline_node_group_min_size": "3", "surge_node_group_capacity_type": "SPOT",
+"surge_node_group_desired_size": "0", "surge_node_group_max_size": "0",
+"surge_node_group_min_size": "0" } ``` **environments/nonprod.json** ```json
+{ "cluster_log_retention": "30", "alert_channel": "nonprod",
+"management_node_group_capacity_type": "ON_DEMAND",
+"management_node_group_desired_size": "8", "management_node_group_max_size":
+"12", "management_node_group_min_size": "8",
 "baseline_node_group_capacity_type": "ON_DEMAND",
-"baseline_node_group_desired_size": "30", "baseline_node_group_max_size": "35",
-"baseline_node_group_min_size": "30", "surge_node_group_desired_size": "3",
-"surge_node_group_max_size": "60", "surge_node_group_min_size": "1" } ```
-**environments/nonprod.json** In nonprod, though we modify similar overrides,
-the needs are different. Our developers only live/work in a single global area.
-So a variety of activities will only take place in the US regions. However,
-there are naturally a series of integration and functional tests that must span
-all the locals where the application will run, hence we do need somewhat larger
-scale everwhere. We will use instance specific overrides to address the primary
-dev region needs. ```json { "aws_account_id": "2222222222222",
+"baseline_node_group_desired_size": "30", "baseline_node_group_max_size": "32",
+"baseline_node_group_min_size": "30", "surge_node_group_capacity_type": "SPOT",
+"surge_node_group_desired_size": "1", "surge_node_group_max_size": "100",
+"surge_node_group_min_size": "1" } ``` **environments/prod.json** ```json
+{ "cluster_log_retention": "90", "alert_channel": "prod",
+"management_node_group_capacity_type": "ON_DEMAND",
+"management_node_group_desired_size": "5", "management_node_group_max_size":
+"12", "management_node_group_min_size": "5",
 "baseline_node_group_capacity_type": "ON_DEMAND",
-"baseline_node_group_desired_size": "10", "baseline_node_group_max_size": "12",
-"baseline_node_group_min_size": "10", "surge_node_group_desired_size": "3",
-"surge_node_group_max_size": "100", "surge_node_group_min_size": "1" } ``` Now,
-we return to the role/instance json to add instance specific info. In this case
-that means region details and the additional default overrides for the primary
-development regions. **environments/dev-deploy.json** ```json { "filter": "*on-
-push-main", "infra-dev": { "infra-dev-us-west-2": { "aws_region": "us-west-2"
-}, "infra-dev-us-east-2": { "aws_region": "us-east-2" }, "infra-dev-eu-west-1":
-{ "aws_region": "eu-west-1" }, "infra-dev-eu-central-1": { "aws_region": "eu-
-central-2" } } } ``` **environments/release.json** ```json { "filter": "*on-
-tag-main", "nonprod": { "nonprod1-us-west-2": { "aws_region": "us-west-2",
-"baseline_node_group_desired_size": "30", "baseline_node_group_max_size": "35",
-"baseline_node_group_min_size": "30", "surge_node_group_desired_size": "30",
-"surge_node_group_max_size": "150", "surge_node_group_min_size": "1" },
-"nonprod1-us-east-2": { "aws_region": "us-east-2",
-"baseline_node_group_desired_size": "30", "baseline_node_group_max_size": "35",
-"baseline_node_group_min_size": "30", "surge_node_group_desired_size": "3",
-"surge_node_group_max_size": "150", "surge_node_group_min_size": "1" },
-"nonprod1-eu-west-1": { "aws_region": "eu-west-1" }, "nonprod1-eu-central-1":
-{ "aws_region": "eu-central-1" }, "nonprod1-ap-southeast-2": { "aws_region":
-"ap-southeast-2" }, "nonprod1-ap-southwest-1": { "aws_region": "ap-southwest-1"
-} }, "prod": { "prod1-us-west-2": { "aws_region": "us-west-2" }, "prod1-us-
-east-2": { "aws_region": "us-east-2" }, "prod1-eu-west-1": { "aws_region": "eu-
-west-1" }, "prod1-eu-central-1": { "aws_region": "eu-central-1" }, "prod1-ap-
-southeast-2": { "aws_region": "ap-southeast-2" }, "prod1-ap-southwest-1":
-{ "aws_region": "ap-southwest-1" } } } ``` From the above files, circlecigen
-will generate each specific _instance_.tfvars.json file for use as a -var-file
-by terraform. Next, the pipeline files. **.circleci/config.yml** Of course you
+"baseline_node_group_desired_size": "15", "baseline_node_group_max_size": "17",
+"baseline_node_group_min_size": "15", "surge_node_group_capacity_type": "SPOT",
+"surge_node_group_desired_size": "1", "surge_node_group_max_size": "100",
+"surge_node_group_min_size": "1" } ``` From the above files, circlecigen will
+generate each specific _instance_.tfvars.json file for use as a -var-file by
+terraform. Next, the pipeline files. **.circleci/config.yml** Of course you
 must have the regular circleci pipeline file that responds to triggers and
 actually forms the basis of the generated pipeline. Everything in this file up
 through the Jobs: or workflow: directive (whichever comes first) forms the
 starting point for the generated pipeline. **.circleci/pre-approve.yml** This
 file is a template that will be populate with instance specific info when the
 pipeline is generated from within the config.yml pipeline. ```yaml - terraform/
 plan: name: {{env_instance}} change plan context: <<
@@ -199,70 +177,70 @@
 launch will use the dev-deploy.json so as to only # deploy to infra-dev
 instances. - launch-dynamic-pipeline: name: dev-build workflow-name: dev-
 environment-deployment multi-config: dev-deploy.json requires: - first job
 filters: *on-push-main # this continutation is only called when the repo is
 tagged and # passes the release.json to generate the full release pipeline -
 launch-dynamic-pipeline: name: release candidate workflow-name: release-
 pipeline multi-config: release.json filters: *on-tag-main ``` Below is a
-notional example of the resulting pipeline from a git-tag trigger. As you can
-see, this level of complexity in an infrastructure release pipeline already is
-likely to inspire the evolution towards a more sophisticated infrastructure
-management release process. The keyword being evolve. Let actual need be the
-cause of adoption of the more elaborate release system, but as is nearly always
-the case, the need to deploy will have deadlines that will be sooner than such
-an adoption. Use of a tool like circlecigen provides an interim step that
-avoids typos by maintaining a higher level of DRY. ```yaml version: 2.1 orbs:
-continuation: circleci/continuation@0.3.1 on-push-main: &on-push-main branches:
-only: /main/ tags: ignore: /.*/ on-tag-main: &on-tag-main branches: ignore:
-/.*/ tags: only: /.*/ commands: setup-commands: parameters: ... steps: ...
-static-code-test-commands: parameters: ... steps: ... before-deployment-
-commands: parameters: ... steps: ... after-deployment-commands: parameters: ...
-steps: ... workflows: version: 2 release-pipeline: jobs: - terraform/plan:
-name: nonprod-us-west-2 change plan context: << pipeline.parameters.context >>
-workspace: nonprod-us-west-2 var-file: env_test/nonprod-us-west-2.tfvars.json
-before-terraform: - set-environment filters: *on-tag-main - terraform/plan:
-name: nonprod-us-east-2 change plan context: << pipeline.parameters.context >>
-workspace: nonprod-us-east-2 var-file: env_test/nonprod-us-east-2.tfvars.json
-before-terraform: - set-environment filters: *on-tag-main - terraform/plan:
-name: nonprod-eu-west-1 change plan ... filters: *on-tag-main - terraform/plan:
-name: nonprod-eu-central-1 change plan ... filters: *on-tag-main - terraform/
-plan: name: nonprod-ap-southeast-2 change plan ... filters: *on-tag-main -
-terraform/plan: name: nonprod-ap-southwest-1 change plan ... filters: *on-tag-
-main - approve nonprod changes: type: approval requires: - nonprod-us-west-
-2 change plan - nonprod-us-east-2 change plan - nonprod-eu-west-1 change plan -
-nonprod-eu-central-1 change plan - nonprod-ap-southeast-2 change plan -
-nonprod-ap-southwest-1 change plan filters: *on-tag-main - terraform/apply:
+notional example of the resulting pipeline from a git-tag trigger, which is
+labeled `release` in out multi.json. As you can see, this level of complexity
+in an infrastructure release pipeline already is likely to inspire the
+evolution towards a more sophisticated infrastructure management release
+process. The keyword being evolve. Let actual need be the cause of adoption of
+the more elaborate release system, but as is nearly always the case, the need
+to deploy will have deadlines that will be sooner than such an adoption.
+```yaml version: 2.1 orbs: continuation: circleci/continuation@0.3.1 on-push-
+main: &on-push-main branches: only: /main/ tags: ignore: /.*/ on-tag-main: &on-
+tag-main branches: ignore: /.*/ tags: only: /.*/ commands: setup-commands:
+parameters: ... steps: ... static-code-test-commands: parameters: ... steps:
+... before-deployment-commands: parameters: ... steps: ... after-deployment-
+commands: parameters: ... steps: ... workflows: version: 2 release-pipeline:
+jobs: - terraform/plan: name: nonprod-us-west-2 change plan context: <<
+pipeline.parameters.context >> workspace: nonprod-us-west-2 var-file: env_test/
+nonprod-us-west-2.tfvars.json before-terraform: - set-environment filters: *on-
+tag-main - terraform/plan: name: nonprod-us-east-2 change plan context: <<
+pipeline.parameters.context >> workspace: nonprod-us-east-2 var-file: env_test/
+nonprod-us-east-2.tfvars.json before-terraform: - set-environment filters: *on-
+tag-main - terraform/plan: name: nonprod-eu-west-1 change plan ... filters:
+*on-tag-main - terraform/plan: name: nonprod-eu-central-1 change plan ...
+filters: *on-tag-main - terraform/plan: name: nonprod-ap-southeast-2 change
+plan ... filters: *on-tag-main - terraform/plan: name: nonprod-ap-southwest-
+1 change plan ... filters: *on-tag-main - approve nonprod changes: type:
+approval requires: - nonprod-us-west-2 change plan - nonprod-us-east-2 change
+plan - nonprod-eu-west-1 change plan - nonprod-eu-central-1 change plan -
+nonprod-ap-southeast-2 change plan - nonprod-ap-southwest-1 change plan
+filters: *on-tag-main - terraform/apply: name: apply nonprod-us-west-2 change
+plan context: << pipeline.parameters.context >> workspace: nonprod-us-west-
+2 var-file: env_test/nonprod-us-west-2.tfvars.json before-terraform: - set-
+environment after-terraform: - after-deployment-commands requires: - approve
+nonprod changes filters: *on-tag-main - terraform/apply: name: apply nonprod-
+us-east-2 change plan ... filters: *on-tag-main - terraform/apply: name: apply
+nonprod-eu-west-1 change plan ... filters: *on-tag-main - terraform/apply:
+name: apply nonprod-eu-central-1 change plan ... filters: *on-tag-main -
+terraform/apply: name: apply nonprod-ap-southeast-2 change plan ... filters:
+*on-tag-main - terraform/apply: name: apply nonprod-ap-southwest-1 change plan
+... filters: *on-tag-main - terraform/plan: name: prod-us-west-2 change plan
+context: << pipeline.parameters.context >> workspace: prod-us-west-2 var-file:
+env_test/prod-us-west-2.tfvars.json before-terraform: - set-environment
+filters: *on-tag-main requires: - approve nonprod changes - terraform/plan:
+name: nonprod-us-east-2 change plan ... filters: *on-tag-main requires: -
+approve nonprod changes - terraform/plan: name: nonprod-eu-west-1 change plan
+... filters: *on-tag-main requires: - approve nonprod changes - terraform/plan:
+name: nonprod-eu-central-1 change plan ... filters: *on-tag-main requires: -
+approve nonprod changes - terraform/plan: name: nonprod-ap-southeast-2 change
+plan ... filters: *on-tag-main requires: - approve nonprod changes - terraform/
+plan: name: nonprod-ap-southwest-1 change plan ... filters: *on-tag-main
+requires: - approve nonprod changes - approve prod changes: type: approval
+requires: - prod-us-west-2 change plan - prod-us-east-2 change plan - prod-eu-
+west-1 change plan - prod-eu-central-1 change plan - prod-ap-southeast-2 change
+plan - prod-ap-southwest-1 change plan filters: *on-tag-main - terraform/apply:
 name: apply nonprod-us-west-2 change plan context: <<
 pipeline.parameters.context >> workspace: nonprod-us-west-2 var-file: env_test/
 nonprod-us-west-2.tfvars.json before-terraform: - set-environment after-
 terraform: - after-deployment-commands requires: - approve nonprod changes
 filters: *on-tag-main - terraform/apply: name: apply nonprod-us-east-2 change
 plan ... filters: *on-tag-main - terraform/apply: name: apply nonprod-eu-west-
 1 change plan ... filters: *on-tag-main - terraform/apply: name: apply nonprod-
 eu-central-1 change plan ... filters: *on-tag-main - terraform/apply: name:
 apply nonprod-ap-southeast-2 change plan ... filters: *on-tag-main - terraform/
 apply: name: apply nonprod-ap-southwest-1 change plan ... filters: *on-tag-main
-- terraform/plan: name: prod-us-west-2 change plan context: <<
-pipeline.parameters.context >> workspace: prod-us-west-2 var-file: env_test/
-prod-us-west-2.tfvars.json before-terraform: - set-environment filters: *on-
-tag-main requires: - approve nonprod changes - terraform/plan: name: nonprod-
-us-east-2 change plan ... filters: *on-tag-main requires: - approve nonprod
-changes - terraform/plan: name: nonprod-eu-west-1 change plan ... filters: *on-
-tag-main requires: - approve nonprod changes - terraform/plan: name: nonprod-
-eu-central-1 change plan ... filters: *on-tag-main requires: - approve nonprod
-changes - terraform/plan: name: nonprod-ap-southeast-2 change plan ... filters:
-*on-tag-main requires: - approve nonprod changes - terraform/plan: name:
-nonprod-ap-southwest-1 change plan ... filters: *on-tag-main requires: -
-approve nonprod changes - approve prod changes: type: approval requires: -
-prod-us-west-2 change plan - prod-us-east-2 change plan - prod-eu-west-1 change
-plan - prod-eu-central-1 change plan - prod-ap-southeast-2 change plan - prod-
-ap-southwest-1 change plan filters: *on-tag-main - terraform/apply: name: apply
-nonprod-us-west-2 change plan context: << pipeline.parameters.context >>
-workspace: nonprod-us-west-2 var-file: env_test/nonprod-us-west-2.tfvars.json
-before-terraform: - set-environment after-terraform: - after-deployment-
-commands requires: - approve nonprod changes filters: *on-tag-main - terraform/
-apply: name: apply nonprod-us-east-2 change plan ... filters: *on-tag-main -
-terraform/apply: name: apply nonprod-eu-west-1 change plan ... filters: *on-
-tag-main - terraform/apply: name: apply nonprod-eu-central-1 change plan ...
-filters: *on-tag-main - terraform/apply: name: apply nonprod-ap-southeast-
-2 change plan ... filters: *on-tag-main - terraform/apply: name: apply nonprod-
-ap-southwest-1 change plan ... filters: *on-tag-main ```
+```
```

### Comparing `circlecigen-0.0.3/src/circlecigen.egg-info/SOURCES.txt` & `circlecigen-0.0.4/src/circlecigen.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -10,31 +10,38 @@
 op.env
 pyproject.toml
 requirements.txt
 setup.py
 .circleci/config.yml
 env_test/config.yml
 env_test/default.json
+env_test/dev.json
+env_test/generated_config.yml
 env_test/multi.json
+env_test/nonprod-us-east-2.tfvars.json
+env_test/nonprod-us-west-2.tfvars.json
+env_test/nonprod.json
 env_test/post-approve.yml
 env_test/pre-approve.yml
-env_test/qa.tfvars.json
+env_test/prod-us-east-2.tfvars.json
+env_test/prod-us-west-2.tfvars.json
+env_test/prod.json
 src/__init__.py
 src/circlecigen.py
 src/template.py
 src/tfvars.py
 src/utils.py
 src/circlecigen.egg-info/PKG-INFO
 src/circlecigen.egg-info/SOURCES.txt
 src/circlecigen.egg-info/dependency_links.txt
 src/circlecigen.egg-info/entry_points.txt
 src/circlecigen.egg-info/top_level.txt
 test/generated_config.yml
 test/generated_config_setup.yml
-test/preview-us-east-2.tfvars.json
-test/preview-us-west-2.tfvars.json
-test/qa-us-east-2.tfvars.json
-test/qa-us-west-2.tfvars.json
+test/nonprod-us-east-2.tfvars.json
+test/nonprod-us-west-2.tfvars.json
+test/prod-us-east-2.tfvars.json
+test/prod-us-west-2.tfvars.json
 test/test_circlecigen.py
 test/test_template.py
 test/test_tfvars.py
 test/test_utils.py
```

### Comparing `circlecigen-0.0.3/src/circlecigen.py` & `circlecigen-0.0.4/src/circlecigen.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,47 +23,53 @@
     help="Generate tfvars.json files for all role/instances. Default is true")
 @click.option("--workflow", default="continuation-generated-workflow",
     help="Name for generated config. Default continuation-generated-workflow",
     callback=validate_filename_arg)
 @click.option("--pipepath", default=".circleci",
     help="Override default config.yml location for testing",
     callback=validate_filepath_arg)
-def cli(outfile, envpath, multifile, defaultparams, tfvars, workflow, pipepath):
-    """Opinionated generation of continuation pipelines.
-    See https://github.com/ThoughtWorks-DPS/circlecigen
-    for detailed usage instructions.
+@click.argument('pipeline', nargs=1)
+def cli(pipeline, outfile, envpath, multifile, defaultparams, tfvars, workflow, pipepath):
+    """
 
     Inputs 
 
-      .circleci/template.yml
+      .circleci/pre_approve.yml
+      .circleci/post_approve.yml
 
       environments/
 
-        default.tfvars.json
+        muilti.json
+        default.json
 
-        [role].tfvars.json
+        [role].json (optional)
 
-        [instance].tfvars.json
+        [instance].json (optional)
 
     Outputs:
 
       .circleci/generated_config.yml
 
       environments/
 
         [for each instance].tfvars.json
+
+    Opinionated generation of continuation pipelines.
+    See https://github.com/ThoughtWorks-DPS/circlecigen
+    for detailed usage instructions.
     """
     validate_filepath(envpath, "envpath")
     validate_filepath(pipepath, "pipepath")
 
     if tfvars:
-        result = generate_environment_tfvar_files(envpath,
+        result = generate_environment_tfvar_files(pipeline, envpath,
                  read_json_file(envpath, multifile),
                  read_json_file(envpath, defaultparams))
         click.echo(f"{result} tfvars created in {envpath}/")
     else:
         click.echo("Not generating tfvars.json files")
-    generate_config(pipepath,
+    generate_config(pipeline, 
+                    pipepath,
                     outfile,
                     envpath,
                     read_json_file(envpath, multifile),
-                    workflow)
+                    workflow)
```

### Comparing `circlecigen-0.0.3/src/template.py` & `circlecigen-0.0.4/src/template.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,59 +19,62 @@
 """
 
 PRIOR_APPROVAL="""
           requires:
             - approve {} changes
 """
 
-def generate_config(pipepath, outfile, envpath, environs, workflow):
+def generate_config(use_pipeline, pipepath, outfile, envpath, environs, workflow):
     """create generated_config.yaml for continuation orb"""
 
+    # use the specified filter to generate a pipeline only for the desired trigger
+    pipeline = environs[use_pipeline]
+
     # copy everything but the jobs and workflows from config.yml into generated_config.yml
     setup_generated_config_outfile(pipepath, outfile, workflow)
 
     # setup the jinja templates
     je = Environment(loader=FileSystemLoader(f"{pipepath}/"), autoescape=True)
     pre, approve, post = get_templates(je, pipepath)
 
     # setup Dict for the approval job template 
     approve_vars = {}
-    approve_vars["filter"] = environs["filter"]
+    approve_vars["filter"] = pipeline["filter"]
 
     # all pre-approval jobs created accept for the first role must wait for
     # the prior role approval set this as blank to start then populate
     # with the list of all instance plans jobs in the role
     priorapprovalrequired = ""
     approvalrequiredjobs = ""
 
     # open the outfile for appeand and start processing roles/instances
     with open(f"{pipepath}/{outfile}", 'a', encoding="utf-8") as f:
-        for role in environs:
+        for role in pipeline:
             # skip the filter definition
             if role == "filter":
                 continue
             # when the approval template is generate, it must be populated with
             # a list of all instances for which a pre-approval template is
             # generated. That is returned by this job.
-            approvalrequiredjobs =  generate_pre_approval_jobs(f, envpath, pre, environs, role, priorapprovalrequired)
+            approvalrequiredjobs =  generate_pre_approval_jobs(f, envpath, pre, pipeline, role, priorapprovalrequired)
             # generate approval job for the current role, a human will trigger the post- phase
             generate_approval_jobs(f, approve, approve_vars, approvalrequiredjobs, role)
-            generate_post_approval_jobs(f, envpath, post, environs, role)
+            generate_post_approval_jobs(f, envpath, post, pipeline, role)
             # record the current role, to provide 'requires:' list in any subsequent pre- jobs
             priorapprovalrequired = role
 
-def generate_pre_approval_jobs(f, envpath, pre, environs, role, priorapprovalrequired):
+def generate_pre_approval_jobs(f, envpath, pre, pipeline, role, priorapprovalrequired):
     # generate a pre-approval job for each instance in the role,
     # if a pre-approval.yml file exists
     if pre:
         approvalrequiredjobs = "requires:"
-        for instance in environs[role]:
+        for instance in pipeline[role]:
             instance_vars=read_json_file(envpath, f"{instance}.tfvars.json")
             instance_vars.update({
-                "filters": environs["filter"],
+                "filters": pipeline["filter"],
                 "role": role,
                 "envpath": envpath
             })
             if priorapprovalrequired:
                 instance_vars.update({
                     "priorapprovalrequired": PRIOR_APPROVAL.format(priorapprovalrequired)
                 })
@@ -83,22 +86,22 @@
 def generate_approval_jobs(f, approve, approve_vars, approvalrequiredjobs, role):
     approve_vars.update ({
         "role": role,
         "approvalrequiredjobs": approvalrequiredjobs
     })
     f.write(approve.render(approve_vars))
 
-def generate_post_approval_jobs(f, envpath, post, environs, role):
+def generate_post_approval_jobs(f, envpath, post, pipeline, role):
     # generate a post-approval job for each instance in the role,
     # if a post-approval.yml file exists
     if post:
-        for instance in environs[role]:
+        for instance in pipeline[role]:
             instance_vars=read_json_file(envpath, f"{instance}.tfvars.json")
             instance_vars.update({
-                "filters": environs["filter"],
+                "filters": pipeline["filter"],
                 "role": role,
                 "envpath": envpath
             })
             f.write(post.render(instance_vars))
 
 def get_templates(je, pipepath):
     """setup the jinja templates"""
@@ -115,14 +118,15 @@
             if not _line_starts_with_setup(line):
                 yield line
 
 
 def _read_until_jobs_or_workflows(f):
     """Generator that reads lines from file object f until it encounters a line starting with 'jobs:' or 'workflows:'"""
     for line in f:
+        # initially, 
         if line.startswith("jobs:") or line.startswith("workflows:"):
             break
         yield line
 
 def _line_starts_with_setup(line):
     """Return True if the given line starts with 'setup:', False otherwise"""
     return line.startswith("setup:")
```

### Comparing `circlecigen-0.0.3/src/utils.py` & `circlecigen-0.0.4/src/utils.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.3/test/test_template.py` & `circlecigen-0.0.4/test/test_template.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,43 @@
 import os
 import filecmp
 from jinja2 import Environment, FileSystemLoader, Template
 from template import setup_generated_config_outfile, get_templates, generate_config
 
-mock_environs = {
-  "filter": "*on-push-main",
-  "qa": {
-    "qa-us-west-2": {
-      "aws_region": "us-west-2"
-    },
-    "qa-us-east-2": {
-      "aws_region": "us-east-2"
+mock_multi = {
+  "sandbox": {
+    "filter": "*on-push-main",
+    "dev": {
+      "dev-us-east-2": {
+        "aws_region": "us-east-2",
+        "aws_account_id": "10100000000"
+      }
     }
   },
-  "preview": {
-    "preview-us-east-2": {
-      "aws_region": "us-east-2"
+  "release": {
+    "filter": "*on-tag-main",
+    "nonprod": {
+      "nonprod-us-west-2": {
+        "aws_region": "us-west-2",
+        "aws_account_id": "20100000000"
+      },
+      "nonprod-us-east-2": {
+        "aws_region": "us-east-2",
+        "aws_account_id": "20100000000"
+      }
     },
-    "preview-us-west-2": {
-      "aws_region": "us-west-2"
+    "prod": {
+      "prod-us-west-2": {
+        "aws_region": "us-west-2",
+        "aws_account_id": "30100000000"
+      },
+      "prod-us-east-2": {
+        "aws_region": "us-east-2",
+        "aws_account_id": "30100000000"
+      }
     }
   }
 }
 
 # this is as ugly as the tfvars file output tests
 def test_setup_generated_config_outfile():
     mock_pipepath = "env_test"
@@ -43,18 +58,19 @@
     
     assert isinstance(pre, Template)
     assert isinstance(post, Template)
     assert isinstance(approve, Template)
 
 # this is as ugly as the tfvars file output tests
 def test_generate_config():
+    mock_pipeline = "release"
     mock_pipepath = "env_test"
     mock_envpath = "env_test"
     mock_outfile = "generated_config.yml"
     mock_workflow = "continuation-generated-workflow"
 
-    generate_config(mock_pipepath, mock_outfile, mock_envpath, mock_environs, mock_workflow)
+    generate_config(mock_pipeline, mock_pipepath, mock_outfile, mock_envpath, mock_multi, mock_workflow)
     assert os.path.isfile(os.path.join(mock_pipepath, mock_outfile))
     assert filecmp.cmp(os.path.join(mock_pipepath,
                        mock_outfile),
                        os.path.join("test",
                        mock_outfile))
```

### Comparing `circlecigen-0.0.3/test/test_utils.py` & `circlecigen-0.0.4/test/test_utils.py`

 * *Files identical despite different names*

