# Comparing `tmp/momotor-engine-options-0.9.0.tar.gz` & `tmp/momotor-engine-options-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momotor-engine-options-0.9.0.tar", last modified: Fri Oct 21 07:07:19 2022, max compression
+gzip compressed data, was "momotor-engine-options-0.9.1.tar", last modified: Thu Oct 27 06:26:52 2022, max compression
```

## Comparing `momotor-engine-options-0.9.0.tar` & `momotor-engine-options-0.9.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-21 07:07:19.000000 momotor-engine-options-0.9.0/
--rw-r--r--   0 root         (0) root         (0)     1779 2022-10-21 07:07:19.000000 momotor-engine-options-0.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      778 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-21 07:07:19.000000 momotor-engine-options-0.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2154 2022-10-06 09:17:27.000000 momotor-engine-options-0.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-21 07:07:19.000000 momotor-engine-options-0.9.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-21 07:07:19.000000 momotor-engine-options-0.9.0/src/momotor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-21 07:07:19.000000 momotor-engine-options-0.9.0/src/momotor/options/
--rw-rw-rw-   0 root         (0) root         (0)      107 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7456 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/convert.py
--rw-rw-rw-   0 root         (0) root         (0)     8228 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/dependencies.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-21 07:07:19.000000 momotor-engine-options-0.9.0/src/momotor/options/domain/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-21 07:06:58.000000 momotor-engine-options-0.9.0/src/momotor/options/domain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-21 07:07:19.000000 momotor-engine-options-0.9.0/src/momotor/options/domain/scheduler/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-21 07:06:58.000000 momotor-engine-options-0.9.0/src/momotor/options/domain/scheduler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/domain/scheduler/_domain.py
--rw-rw-rw-   0 root         (0) root         (0)     7560 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/domain/scheduler/preflight.py
--rw-rw-rw-   0 root         (0) root         (0)     8162 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/domain/scheduler/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     3692 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/domain/scheduler/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-21 07:07:19.000000 momotor-engine-options-0.9.0/src/momotor/options/domain/tools/
--rw-rw-rw-   0 root         (0) root         (0)     5329 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/domain/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       17 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/domain/tools/_domain.py
--rw-rw-rw-   0 root         (0) root         (0)     1696 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/filter_files.py
--rw-rw-rw-   0 root         (0) root         (0)    12223 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/option.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-21 07:07:19.000000 momotor-engine-options-0.9.0/src/momotor/options/parser/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-21 07:06:58.000000 momotor-engine-options-0.9.0/src/momotor/options/parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1681 2022-10-21 07:06:14.000000 momotor-engine-options-0.9.0/src/momotor/options/parser/consts.py
--rw-rw-rw-   0 root         (0) root         (0)     3534 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/parser/keyvalue.py
--rw-rw-rw-   0 root         (0) root         (0)     3510 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/parser/modifier.py
--rw-rw-rw-   0 root         (0) root         (0)     1920 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/parser/placeholders.py
--rw-rw-rw-   0 root         (0) root         (0)    24106 2022-10-21 07:06:14.000000 momotor-engine-options-0.9.0/src/momotor/options/parser/reference.py
--rw-rw-rw-   0 root         (0) root         (0)     8229 2022-10-21 07:06:14.000000 momotor-engine-options-0.9.0/src/momotor/options/parser/selector.py
--rw-rw-rw-   0 root         (0) root         (0)     1059 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/providers.py
--rw-rw-rw-   0 root         (0) root         (0)     6463 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/result_query.py
--rw-rw-rw-   0 root         (0) root         (0)     1434 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/split.py
--rw-rw-rw-   0 root         (0) root         (0)     8926 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/task_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-21 07:07:19.000000 momotor-engine-options-0.9.0/src/momotor/options/tools/
--rw-rw-rw-   0 root         (0) root         (0)      919 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6195 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/tools/registry.py
--rw-rw-rw-   0 root         (0) root         (0)    12426 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/tools/tool.py
--rw-rw-rw-   0 root         (0) root         (0)      464 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/tools/types.py
--rw-rw-rw-   0 root         (0) root         (0)     4780 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/tools/version.py
--rw-rw-rw-   0 root         (0) root         (0)      555 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.0/src/momotor/options/types.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-10-21 07:06:37.000000 momotor-engine-options-0.9.0/src/momotor/options/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-21 07:07:19.000000 momotor-engine-options-0.9.0/src/momotor_engine_options.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1779 2022-10-21 07:07:19.000000 momotor-engine-options-0.9.0/src/momotor_engine_options.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1495 2022-10-21 07:07:19.000000 momotor-engine-options-0.9.0/src/momotor_engine_options.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-21 07:07:19.000000 momotor-engine-options-0.9.0/src/momotor_engine_options.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-21 07:07:19.000000 momotor-engine-options-0.9.0/src/momotor_engine_options.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      152 2022-10-21 07:07:19.000000 momotor-engine-options-0.9.0/src/momotor_engine_options.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-10-21 07:07:19.000000 momotor-engine-options-0.9.0/src/momotor_engine_options.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/
+-rw-r--r--   0 root         (0) root         (0)     1779 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      778 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2154 2022-10-06 09:17:27.000000 momotor-engine-options-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor/options/
+-rw-rw-rw-   0 root         (0) root         (0)      107 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7456 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/convert.py
+-rw-rw-rw-   0 root         (0) root         (0)     8228 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/dependencies.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-27 06:26:31.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-27 06:26:31.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/scheduler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/scheduler/_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     7560 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/scheduler/preflight.py
+-rw-rw-rw-   0 root         (0) root         (0)     8162 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/scheduler/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3692 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/scheduler/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/tools/
+-rw-rw-rw-   0 root         (0) root         (0)     5329 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       17 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/tools/_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     1696 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/filter_files.py
+-rw-rw-rw-   0 root         (0) root         (0)    12223 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/option.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor/options/parser/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-27 06:26:31.000000 momotor-engine-options-0.9.1/src/momotor/options/parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2022-10-21 07:06:14.000000 momotor-engine-options-0.9.1/src/momotor/options/parser/consts.py
+-rw-rw-rw-   0 root         (0) root         (0)     3534 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/parser/keyvalue.py
+-rw-rw-rw-   0 root         (0) root         (0)     3552 2022-10-27 06:25:56.000000 momotor-engine-options-0.9.1/src/momotor/options/parser/modifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     1920 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/parser/placeholders.py
+-rw-rw-rw-   0 root         (0) root         (0)    24419 2022-10-27 06:25:56.000000 momotor-engine-options-0.9.1/src/momotor/options/parser/reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     8308 2022-10-27 06:25:56.000000 momotor-engine-options-0.9.1/src/momotor/options/parser/selector.py
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/providers.py
+-rw-rw-rw-   0 root         (0) root         (0)     6463 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/result_query.py
+-rw-rw-rw-   0 root         (0) root         (0)     1434 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/split.py
+-rw-rw-rw-   0 root         (0) root         (0)     8926 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/task_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor/options/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      919 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6195 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/tools/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    12426 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/tools/tool.py
+-rw-rw-rw-   0 root         (0) root         (0)      464 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/tools/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     4780 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/tools/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      555 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/types.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-10-27 06:26:11.000000 momotor-engine-options-0.9.1/src/momotor/options/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor_engine_options.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1779 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor_engine_options.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1495 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor_engine_options.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor_engine_options.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor_engine_options.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      152 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor_engine_options.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor_engine_options.egg-info/top_level.txt
```

### Comparing `momotor-engine-options-0.9.0/PKG-INFO` & `momotor-engine-options-0.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: momotor-engine-options
-Version: 0.9.0
+Version: 0.9.1
 Summary: Momotor Engine Options Library
 Home-page: https://momotor.org/
 Author: Erik Scheffers
 Author-email: e.t.j.scheffers@tue.nl
-Project-URL: Documentation, https://momotor.org/doc/engine/momotor-engine-options/release/0.9.0/
+Project-URL: Documentation, https://momotor.org/doc/engine/momotor-engine-options/release/0.9.1/
 Project-URL: Source, https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/
 Project-URL: Tracker, https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `momotor-engine-options-0.9.0/README.md` & `momotor-engine-options-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/setup.py` & `momotor-engine-options-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/convert.py` & `momotor-engine-options-0.9.1/src/momotor/options/convert.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/dependencies.py` & `momotor-engine-options-0.9.1/src/momotor/options/dependencies.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/domain/scheduler/preflight.py` & `momotor-engine-options-0.9.1/src/momotor/options/domain/scheduler/preflight.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/domain/scheduler/tasks.py` & `momotor-engine-options-0.9.1/src/momotor/options/domain/scheduler/tasks.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/domain/scheduler/tools.py` & `momotor-engine-options-0.9.1/src/momotor/options/domain/scheduler/tools.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/domain/tools/__init__.py` & `momotor-engine-options-0.9.1/src/momotor/options/domain/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/filter_files.py` & `momotor-engine-options-0.9.1/src/momotor/options/filter_files.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/option.py` & `momotor-engine-options-0.9.1/src/momotor/options/option.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/parser/consts.py` & `momotor-engine-options-0.9.1/src/momotor/options/parser/consts.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/parser/keyvalue.py` & `momotor-engine-options-0.9.1/src/momotor/options/parser/keyvalue.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/parser/modifier.py` & `momotor-engine-options-0.9.1/src/momotor/options/parser/modifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,34 +10,35 @@
 def parse_mod(modded_ref: str) -> typing.Tuple[typing.Optional[str], str]:
     """
 
     >>> parse_mod('')
     (None, '')
 
     >>> parse_mod(' 123')
-    (None, ' 123')
+    (None, '123')
 
     >>> parse_mod('%mod')
     ('mod', '')
 
     >>> parse_mod('%mod 123')
-    ('mod', ' 123')
+    ('mod', '123')
 
-    >>> parse_mod(' %mod 123')
-    ('mod', ' 123')
+    >>> parse_mod(' %mod 123 ')
+    ('mod', '123')
 
     :param modded_ref:
     :return:
     """
+    modded_ref = modded_ref.strip()
     m_mod = MOD_RE.match(modded_ref)
 
     if m_mod:
         mod = m_mod.group('mod')
         if mod:
-            return mod, modded_ref[m_mod.end(m_mod.lastindex):]
+            return mod, modded_ref[m_mod.end(m_mod.lastindex):].strip()
 
     return None, modded_ref
 
 
 def exclude_none(values):
     for v in values:
         if v is not None:
```

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/parser/placeholders.py` & `momotor-engine-options-0.9.1/src/momotor/options/parser/placeholders.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/parser/reference.py` & `momotor-engine-options-0.9.1/src/momotor/options/parser/reference.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
     >>> _split_reference("type[option] ")
     ('type', 'option', ' ')
 
     :param reference:
     :return:
     """
-    m_ref = REFERENCE_RE.match(reference)
+    m_ref = REFERENCE_RE.match(reference.strip())
     if m_ref is None:
         return None, None, reference
 
     type_ = m_ref.group('type')
     ref_option = m_ref.group('opt')
     if ref_option:
         ref_option = ref_option[1:-1].strip()
@@ -177,15 +177,15 @@
     #
     # provider = m_provider.group('provider')
     # if provider:
     #     remaining = ref_option[m_provider.end(m_provider.lastindex):]
     # else:
     #     remaining = ref_option
 
-    remaining = ref_option or ''
+    remaining = (ref_option or '').strip()
     refs: typing.MutableSequence[Reference] = collections.deque()
     any_options = False
     while remaining.strip():
         m_ref = REF_OPTION_RE.match(remaining)
         if not m_ref:
             break
 
@@ -244,15 +244,15 @@
     >>> parse_reference("type[@provider#id,id2:class#name] rest")
     ('type', (Reference(provider='provider', id='id,id2', name='class#name', _source='@provider#id,id2:class#name'),), ' rest')
 
     >>> parse_reference("type[#wildcard.*:class] rest")
     ('type', (Reference(provider=None, id='wildcard.*', name='class', _source='#wildcard.*:class'),), ' rest')
 
     """
-    type_, ref_option, remainder = _split_reference(reference)
+    type_, ref_option, remainder = _split_reference(reference.strip())
 
     refs, ref_remainder = _split_options(ref_option)
     if ref_remainder and ref_remainder.strip():
         raise ValueError(f"Invalid reference {reference.strip()}")
 
     return type_, refs, remainder
 
@@ -305,15 +305,15 @@
 
     >>> _split_name_class('#"spaced name.txt"')
     (None, '"spaced name.txt"')
 
     :param nc:
     :return:
     """
-    parts = list(smart_split(nc))
+    parts = list(smart_split(nc.strip()))
 
     if parts and '#' in parts[0] and parts[0][0] not in {'"', "'"}:
         class_, rest = parts[0].split('#', 1)
         if rest:
             parts[0] = rest
         else:
             parts.pop(0)
@@ -336,14 +336,15 @@
     >>> _split_name_domain('name')
     ('name', None)
 
     >>> _split_name_domain('name@domain')
     ('name', 'domain')
 
     """
+    nd = nd.strip()
 
     if '@' in nd:
         name, domain = nd.split('@', 1)
     else:
         name, domain = nd, None
 
     return name, domain
@@ -353,14 +354,15 @@
         -> typing.Generator[ReferenceMatch, None, None]:
     """ A generator to generate :py:class:`ReferenceMatch` objects for result and outcome references
 
     :param type_: The :token:`~reference:type`
     :param objects:
     :raises ValueError: the reference is invalid
     """
+    type_ = type_.strip()
 
     if type_ == 'result':
         _test = lambda obj: True
 
     elif type_.startswith('not-'):
         try:
             outcome = Outcome(type_[4:])
@@ -484,14 +486,16 @@
     'file': (None, None),
     'opt': (None, None),
 }
 
 
 def _get_bundle_objects(type_: str, refs: typing.Sequence[Reference], bundles: Providers) \
         -> typing.Generator[typing.Tuple[ProviderElement, Reference], None, None]:
+    type_ = type_.strip()
+
     if type_ in DEFAULT_VALID_PROVIDERS:
         default_provider, valid_providers = DEFAULT_VALID_PROVIDERS[type_]
     else:
         default_provider, valid_providers = DEFAULT_VALID_PROVIDERS[None]
 
     for ref in refs:
         provider = ref.provider or default_provider
@@ -546,14 +550,15 @@
 
     Each :py:class:`ReferenceMatch` object generated is a single reference resolved.
 
     :param type_: The reference :token:`~reference:type`
     :param refs: The reference options
     :param bundles: The bundles to resolve the references too
     """
+    type_ = type_.strip()
     objects = _get_bundle_objects(type_, refs, bundles)
 
     if type_ == 'prop':
         yield from _match_prop_reference(objects, bundles.task_id)
 
     elif type_ == 'file':
         yield from _match_file_reference(objects, bundles.task_id)
@@ -573,14 +578,15 @@
     :param bundles: The providers providing the objects that are referenced
     :return: a 3-tuple containing
              the :token:`~reference:type`,
              a tuple of :py:class:`ReferenceMatch` objects, and
              a string with the rest of the `reference` string remaining after parsing.
     :raises ValueError: the reference cannot be parsed
     """
+    reference = reference.strip()
 
     type_, refs, remainder = parse_reference(reference)
     try:
         if type_:
             items = tuple(generate_reference(type_, refs, bundles))
         else:
             items = tuple()
@@ -601,15 +607,15 @@
     :param reference: The reference to parse
     :param results: The results bundle containing the properties
     :param task_id: The task id to expand task references
     :return: a 2-tuple containing
              a tuple of :py:class:`ReferenceMatch` objects, and
              a string with the rest of the `reference` string remaining after parsing.
     """
-
+    reference = reference.strip()
     refs, remainder = _split_options(reference)
 
     try:
         objects = _get_bundle_objects('prop', refs, Providers(results=results, task_id=task_id))
     except ValueError as exc:
         raise ValueError(f"Invalid property reference {reference!r}: {exc}")
 
@@ -624,14 +630,15 @@
 
     :param reference: The reference to parse
     :param bundles: The bundles to resolve the references too
     :return: a 2-tuple containing
              a tuple of :py:class:`ReferenceMatch` objects, and
              a string with the rest of the `reference` string remaining after parsing.
     """
+    reference = reference.strip()
     refs, remainder = _split_options(reference)
 
     try:
         objects = _get_bundle_objects('file', refs, bundles)
     except ValueError as exc:
         raise ValueError(f"Invalid file reference {reference!r}: {exc}")
 
@@ -646,14 +653,15 @@
 
     :param reference:
     :param bundles: The bundles to resolve the references too
     :return: a 2-tuple containing
              a tuple of :py:class:`ReferenceMatch` objects, and
              a string with the rest of the `reference` string remaining after parsing.
     """
+    reference = reference.strip()
     refs, remainder = _split_options(reference)
 
     try:
         objects = _get_bundle_objects('opt', refs, bundles)
     except ValueError as exc:
         raise ValueError(f"Invalid option reference {reference!r}: {exc}")
 
@@ -667,15 +675,15 @@
     """ Resolve a :ref:`reference value <reference value>` string into the value
 
     :param value_reference: The :token:`~reference_value:value_reference`
     :param bundles: The bundles to resolve the references too
     :param default_mod: The default :token:`~reference_value:mod`
     :return: The resolved value
     """
-
+    value_reference = value_reference.strip()
     mod, remaining = parse_mod(value_reference)
     type_, refs, remaining = parse_reference(remaining)
 
     if not type_:
         return None, value_reference
 
     matches = tuple(
```

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/parser/selector.py` & `momotor-engine-options-0.9.1/src/momotor/options/parser/selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     ('prop', (Reference(provider=None, id=None, name='test', _source=':test'),), '==', 'test string', '')
 
     >>> parse_selector('prop[:test]>0 123')
     ('prop', (Reference(provider=None, id=None, name='test', _source=':test'),), '>', 0, ' 123')
 
     :return:
     """
+    selector = selector.strip()
     type_, refs, remainder = parse_reference(selector)
     if not type_:
         # A selector without reference makes no sense
         raise ValueError(f"Invalid selector {selector!r}")
 
     m_oper_value = CONDITION_RE.match(remainder)
 
@@ -130,15 +131,15 @@
              the attribute to get the reference value from (based on :token:`~reference:type`),
              an iterator for :py:class:`~momotor.options.parser.reference.ReferenceMatch` objects,
              the `operator`,
              the `value`, and
              a string with the rest of the `selector` string remaining after parsing.
     :raises ValueError: if the selector is not valid
     """
-
+    selector = selector.strip()
     type_, refs, oper, value, remainder = parse_selector(selector)
 
     try:
         matches = generate_reference(type_, refs, bundles)
     except ValueError as exc:
         raise ValueError(f"Invalid {type_!r} selector {selector!r}: {exc}")
 
@@ -154,15 +155,15 @@
     :param selector: the :token:`~selector:selector` to parse
     :param bundles: The bundles to resolve the references too
     :return: a 2-tuple containing
              a tuple with the selected elements, and
              a string with the rest of the `selector` string remaining after parsing.
     :raises ValueError: if the selector is not valid
     """
-    attr, matches, oper, value, remainder = resolve_selector(selector, bundles)
+    attr, matches, oper, value, remainder = resolve_selector(selector.strip(), bundles)
 
     results: typing.MutableSequence[Element] = collections.deque()
     for match in matches:
         obj_values = [getattr(mv, attr, None) for mv in match.values]
         for obj_value in obj_values:
             if oper(obj_value, value):
                 results.append(match.provider)
@@ -178,15 +179,15 @@
     :param bundles: The bundles to resolve the references too
     :param default_mod: Default 'mod'
     :return: a 2-tuple containing
              a boolean indicating if there was a match, and
              a string with the rest of the `selector` string remaining after parsing.
     :raises ValueError: if the selector is not valid
     """
-    mod, selector = parse_mod(selector)
+    mod, selector = parse_mod(selector.strip())
 
     if not mod:
         mod = default_mod
 
     attr, matches, oper, value, remainder = resolve_selector(selector, bundles)
 
     def _match_all() -> bool:
```

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/providers.py` & `momotor-engine-options-0.9.1/src/momotor/options/providers.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/result_query.py` & `momotor-engine-options-0.9.1/src/momotor/options/result_query.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/split.py` & `momotor-engine-options-0.9.1/src/momotor/options/split.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/task_id.py` & `momotor-engine-options-0.9.1/src/momotor/options/task_id.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/tools/__init__.py` & `momotor-engine-options-0.9.1/src/momotor/options/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/tools/registry.py` & `momotor-engine-options-0.9.1/src/momotor/options/tools/registry.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/tools/tool.py` & `momotor-engine-options-0.9.1/src/momotor/options/tools/tool.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/tools/version.py` & `momotor-engine-options-0.9.1/src/momotor/options/tools/version.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/src/momotor/options/types.py` & `momotor-engine-options-0.9.1/src/momotor/options/types.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.0/src/momotor_engine_options.egg-info/PKG-INFO` & `momotor-engine-options-0.9.1/src/momotor_engine_options.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: momotor-engine-options
-Version: 0.9.0
+Version: 0.9.1
 Summary: Momotor Engine Options Library
 Home-page: https://momotor.org/
 Author: Erik Scheffers
 Author-email: e.t.j.scheffers@tue.nl
-Project-URL: Documentation, https://momotor.org/doc/engine/momotor-engine-options/release/0.9.0/
+Project-URL: Documentation, https://momotor.org/doc/engine/momotor-engine-options/release/0.9.1/
 Project-URL: Source, https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/
 Project-URL: Tracker, https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `momotor-engine-options-0.9.0/src/momotor_engine_options.egg-info/SOURCES.txt` & `momotor-engine-options-0.9.1/src/momotor_engine_options.egg-info/SOURCES.txt`

 * *Files identical despite different names*

