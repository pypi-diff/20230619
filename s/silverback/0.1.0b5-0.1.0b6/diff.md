# Comparing `tmp/silverback-0.1.0b5.tar.gz` & `tmp/silverback-0.1.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silverback-0.1.0b5.tar", last modified: Thu Jun 15 19:15:59 2023, max compression
+gzip compressed data, was "silverback-0.1.0b6.tar", last modified: Mon Jun 19 21:57:26 2023, max compression
```

## Comparing `silverback-0.1.0b5.tar` & `silverback-0.1.0b6.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:15:59.244999 silverback-0.1.0b5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:15:59.236999 silverback-0.1.0b5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:15:59.236999 silverback-0.1.0b5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-15 19:14:54.000000 silverback-0.1.0b5/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-15 19:14:54.000000 silverback-0.1.0b5/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-15 19:14:54.000000 silverback-0.1.0b5/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-15 19:14:54.000000 silverback-0.1.0b5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-15 19:14:54.000000 silverback-0.1.0b5/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:15:59.236999 silverback-0.1.0b5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-15 19:14:54.000000 silverback-0.1.0b5/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-15 19:14:54.000000 silverback-0.1.0b5/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-15 19:14:54.000000 silverback-0.1.0b5/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-15 19:14:54.000000 silverback-0.1.0b5/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-15 19:14:54.000000 silverback-0.1.0b5/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-15 19:14:54.000000 silverback-0.1.0b5/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-15 19:14:54.000000 silverback-0.1.0b5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 19:14:54.000000 silverback-0.1.0b5/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-15 19:14:54.000000 silverback-0.1.0b5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-15 19:14:54.000000 silverback-0.1.0b5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-15 19:14:54.000000 silverback-0.1.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-15 19:15:59.244999 silverback-0.1.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-15 19:14:54.000000 silverback-0.1.0b5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-15 19:14:54.000000 silverback-0.1.0b5/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-15 19:14:54.000000 silverback-0.1.0b5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-15 19:15:59.244999 silverback-0.1.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-15 19:14:54.000000 silverback-0.1.0b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:15:59.240999 silverback-0.1.0b5/silverback/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-15 19:14:54.000000 silverback-0.1.0b5/silverback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-15 19:14:54.000000 silverback-0.1.0b5/silverback/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-15 19:14:54.000000 silverback-0.1.0b5/silverback/_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-15 19:14:54.000000 silverback-0.1.0b5/silverback/application.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-15 19:14:54.000000 silverback-0.1.0b5/silverback/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-15 19:14:54.000000 silverback-0.1.0b5/silverback/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:14:54.000000 silverback-0.1.0b5/silverback/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-15 19:14:54.000000 silverback-0.1.0b5/silverback/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-15 19:14:54.000000 silverback-0.1.0b5/silverback/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-15 19:14:54.000000 silverback-0.1.0b5/silverback/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-15 19:15:58.000000 silverback-0.1.0b5/silverback/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:15:59.240999 silverback-0.1.0b5/silverback.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-15 19:15:58.000000 silverback-0.1.0b5/silverback.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-15 19:15:59.000000 silverback-0.1.0b5/silverback.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:15:58.000000 silverback-0.1.0b5/silverback.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 19:15:58.000000 silverback-0.1.0b5/silverback.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:15:58.000000 silverback-0.1.0b5/silverback.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-15 19:15:58.000000 silverback-0.1.0b5/silverback.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 19:15:58.000000 silverback-0.1.0b5/silverback.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:15:59.240999 silverback-0.1.0b5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:14:54.000000 silverback-0.1.0b5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-15 19:14:54.000000 silverback-0.1.0b5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-15 19:14:54.000000 silverback-0.1.0b5/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:57:26.218118 silverback-0.1.0b6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:57:26.214118 silverback-0.1.0b6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:57:26.214118 silverback-0.1.0b6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:57:26.214118 silverback-0.1.0b6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-19 21:56:12.000000 silverback-0.1.0b6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-19 21:56:12.000000 silverback-0.1.0b6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-19 21:56:12.000000 silverback-0.1.0b6/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-19 21:56:12.000000 silverback-0.1.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-19 21:57:26.218118 silverback-0.1.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-19 21:56:12.000000 silverback-0.1.0b6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-19 21:56:12.000000 silverback-0.1.0b6/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-19 21:56:12.000000 silverback-0.1.0b6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-19 21:57:26.218118 silverback-0.1.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-19 21:56:12.000000 silverback-0.1.0b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:57:26.214118 silverback-0.1.0b6/silverback/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-19 21:56:12.000000 silverback-0.1.0b6/silverback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-19 21:56:12.000000 silverback-0.1.0b6/silverback/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-19 21:56:12.000000 silverback-0.1.0b6/silverback/_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-19 21:56:12.000000 silverback-0.1.0b6/silverback/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-19 21:56:12.000000 silverback-0.1.0b6/silverback/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-19 21:56:12.000000 silverback-0.1.0b6/silverback/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:56:12.000000 silverback-0.1.0b6/silverback/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-19 21:56:12.000000 silverback-0.1.0b6/silverback/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-19 21:56:12.000000 silverback-0.1.0b6/silverback/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-19 21:56:12.000000 silverback-0.1.0b6/silverback/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-19 21:57:25.000000 silverback-0.1.0b6/silverback/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:57:26.218118 silverback-0.1.0b6/silverback.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-19 21:57:25.000000 silverback-0.1.0b6/silverback.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-19 21:57:26.000000 silverback-0.1.0b6/silverback.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 21:57:25.000000 silverback-0.1.0b6/silverback.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-19 21:57:25.000000 silverback-0.1.0b6/silverback.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 21:57:25.000000 silverback-0.1.0b6/silverback.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-19 21:57:25.000000 silverback-0.1.0b6/silverback.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-19 21:57:25.000000 silverback-0.1.0b6/silverback.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:57:26.218118 silverback-0.1.0b6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:56:12.000000 silverback-0.1.0b6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-19 21:56:12.000000 silverback-0.1.0b6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-19 21:56:12.000000 silverback-0.1.0b6/tests/test_cli.py
```

### Comparing `silverback-0.1.0b5/.github/ISSUE_TEMPLATE/bug.md` & `silverback-0.1.0b6/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/.github/ISSUE_TEMPLATE/feature.md` & `silverback-0.1.0b6/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/.github/ISSUE_TEMPLATE/work-item.md` & `silverback-0.1.0b6/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/.github/release-drafter.yml` & `silverback-0.1.0b6/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/.github/workflows/codeql.yaml` & `silverback-0.1.0b6/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/.github/workflows/commitlint.yaml` & `silverback-0.1.0b6/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/.github/workflows/prtitle.yaml` & `silverback-0.1.0b6/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/.github/workflows/publish.yaml` & `silverback-0.1.0b6/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/.github/workflows/test.yaml` & `silverback-0.1.0b6/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/.gitignore` & `silverback-0.1.0b6/.gitignore`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/.pre-commit-config.yaml` & `silverback-0.1.0b6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/CONTRIBUTING.md` & `silverback-0.1.0b6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/LICENSE` & `silverback-0.1.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/PKG-INFO` & `silverback-0.1.0b6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.1.0b5
+Version: 0.1.0b6
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/SilverBackLtd/sdk
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
         
@@ -40,14 +40,21 @@
         
         To run your bot against a live network, this SDK includes a simple runner you can use via:
         
         ```sh
         $ silverback run "example:app" --network :mainnet:alchemy
         ```
         
+        ## Docker Usage
+        
+        ```sh
+        $ docker build -t silverback .
+        $ docker run --volume $PWD:/home/harambe/project silverback run "example:app" --network :mainnet:alchemy
+        ```
+        
         ## Development
         
         This project is in development and should be considered a beta.
         Things might not be in their final state and breaking changes may occur.
         Comments, questions, criticisms and pull requests are welcomed.
         
 Keywords: ethereum
```

### Comparing `silverback-0.1.0b5/README.md` & `silverback-0.1.0b6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -32,12 +32,19 @@
 
 To run your bot against a live network, this SDK includes a simple runner you can use via:
 
 ```sh
 $ silverback run "example:app" --network :mainnet:alchemy
 ```
 
+## Docker Usage
+
+```sh
+$ docker build -t silverback .
+$ docker run --volume $PWD:/home/harambe/project silverback run "example:app" --network :mainnet:alchemy
+```
+
 ## Development
 
 This project is in development and should be considered a beta.
 Things might not be in their final state and breaking changes may occur.
 Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `silverback-0.1.0b5/example.py` & `silverback-0.1.0b6/example.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/pyproject.toml` & `silverback-0.1.0b6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/setup.py` & `silverback-0.1.0b6/setup.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/silverback/_cli.py` & `silverback-0.1.0b6/silverback/_cli.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/silverback/_importer.py` & `silverback-0.1.0b6/silverback/_importer.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/silverback/application.py` & `silverback-0.1.0b6/silverback/application.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/silverback/exceptions.py` & `silverback-0.1.0b6/silverback/exceptions.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/silverback/middlewares.py` & `silverback-0.1.0b6/silverback/middlewares.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/silverback/runner.py` & `silverback-0.1.0b6/silverback/runner.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/silverback/settings.py` & `silverback-0.1.0b6/silverback/settings.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/silverback/utils.py` & `silverback-0.1.0b6/silverback/utils.py`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0b5/silverback.egg-info/PKG-INFO` & `silverback-0.1.0b6/silverback.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.1.0b5
+Version: 0.1.0b6
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/SilverBackLtd/sdk
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
         
@@ -40,14 +40,21 @@
         
         To run your bot against a live network, this SDK includes a simple runner you can use via:
         
         ```sh
         $ silverback run "example:app" --network :mainnet:alchemy
         ```
         
+        ## Docker Usage
+        
+        ```sh
+        $ docker build -t silverback .
+        $ docker run --volume $PWD:/home/harambe/project silverback run "example:app" --network :mainnet:alchemy
+        ```
+        
         ## Development
         
         This project is in development and should be considered a beta.
         Things might not be in their final state and breaking changes may occur.
         Comments, questions, criticisms and pull requests are welcomed.
         
 Keywords: ethereum
```

### Comparing `silverback-0.1.0b5/silverback.egg-info/SOURCES.txt` & `silverback-0.1.0b6/silverback.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 .mdformat.toml
 .pre-commit-config.yaml
 CONTRIBUTING.md
+Dockerfile
 LICENSE
 README.md
 example.py
 pyproject.toml
 setup.cfg
 setup.py
 .github/PULL_REQUEST_TEMPLATE.md
```

### Comparing `silverback-0.1.0b5/silverback.egg-info/requires.txt` & `silverback-0.1.0b6/silverback.egg-info/requires.txt`

 * *Files identical despite different names*

