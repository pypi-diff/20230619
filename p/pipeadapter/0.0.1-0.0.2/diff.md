# Comparing `tmp/pipeadapter-0.0.1.tar.gz` & `tmp/pipeadapter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeadapter-0.0.1.tar", last modified: Sat Sep  3 22:32:02 2022, max compression
+gzip compressed data, was "pipeadapter-0.0.2.tar", last modified: Mon Jun 19 00:41:32 2023, max compression
```

## Comparing `pipeadapter-0.0.1.tar` & `pipeadapter-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 22:32:02.823812 pipeadapter-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     2317 2022-09-03 22:32:02.823812 pipeadapter-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-09-03 22:31:51.000000 pipeadapter-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 22:32:02.819812 pipeadapter-0.0.1/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 22:32:02.819812 pipeadapter-0.0.1/pkg/pipeadapter/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-09-03 22:31:52.000000 pipeadapter-0.0.1/pkg/pipeadapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5470 2022-09-03 22:31:52.000000 pipeadapter-0.0.1/pkg/pipeadapter/pipeadapter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 22:32:02.823812 pipeadapter-0.0.1/pkg/pipeadapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2317 2022-09-03 22:32:02.000000 pipeadapter-0.0.1/pkg/pipeadapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-09-03 22:32:02.000000 pipeadapter-0.0.1/pkg/pipeadapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-03 22:32:02.000000 pipeadapter-0.0.1/pkg/pipeadapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-03 22:32:02.000000 pipeadapter-0.0.1/pkg/pipeadapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-03 22:32:02.000000 pipeadapter-0.0.1/pkg/pipeadapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-03 22:31:52.000000 pipeadapter-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-09-03 22:32:02.823812 pipeadapter-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:41:32.882585 pipeadapter-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-19 00:41:32.882585 pipeadapter-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-19 00:41:16.000000 pipeadapter-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:41:32.882585 pipeadapter-0.0.2/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:41:32.882585 pipeadapter-0.0.2/pkg/pipeadapter/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-19 00:41:24.000000 pipeadapter-0.0.2/pkg/pipeadapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-19 00:41:24.000000 pipeadapter-0.0.2/pkg/pipeadapter/pipeadapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:41:32.882585 pipeadapter-0.0.2/pkg/pipeadapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-19 00:41:32.000000 pipeadapter-0.0.2/pkg/pipeadapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-19 00:41:32.000000 pipeadapter-0.0.2/pkg/pipeadapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 00:41:32.000000 pipeadapter-0.0.2/pkg/pipeadapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-19 00:41:32.000000 pipeadapter-0.0.2/pkg/pipeadapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 00:41:32.000000 pipeadapter-0.0.2/pkg/pipeadapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-19 00:41:24.000000 pipeadapter-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-19 00:41:32.882585 pipeadapter-0.0.2/setup.cfg
```

### Comparing `pipeadapter-0.0.1/PKG-INFO` & `pipeadapter-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeadapter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pipedream adapter for eons
 Home-page: https://github.com/infrastructure-tech/lib_pipeadapter
 Author: Infrastructure Technologies
 Author-email: support@infrastructure.tech
 Project-URL: Bug Tracker, https://github.com/infrastructure-tech/lib_pipeadapter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pipeadapter-0.0.1/README.md` & `pipeadapter-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pipeadapter-0.0.1/pkg/pipeadapter.egg-info/PKG-INFO` & `pipeadapter-0.0.2/pkg/pipeadapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeadapter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pipedream adapter for eons
 Home-page: https://github.com/infrastructure-tech/lib_pipeadapter
 Author: Infrastructure Technologies
 Author-email: support@infrastructure.tech
 Project-URL: Bug Tracker, https://github.com/infrastructure-tech/lib_pipeadapter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

