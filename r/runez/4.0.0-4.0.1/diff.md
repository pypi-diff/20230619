# Comparing `tmp/runez-4.0.0.tar.gz` & `tmp/runez-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runez-4.0.0.tar", last modified: Wed May 31 16:44:30 2023, max compression
+gzip compressed data, was "runez-4.0.1.tar", last modified: Mon Jun 19 14:36:50 2023, max compression
```

## Comparing `runez-4.0.0.tar` & `runez-4.0.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:44:30.655542 runez-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-31 16:43:46.000000 runez-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-31 16:43:46.000000 runez-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-31 16:44:30.655542 runez-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-31 16:43:46.000000 runez-4.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-31 16:43:46.000000 runez-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 16:44:30.655542 runez-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-31 16:43:46.000000 runez-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:44:30.647542 runez-4.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:44:30.651542 runez-4.0.0/src/runez/
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/ascii.py
--rw-r--r--   0 runner    (1001) docker     (123)    15102 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/click.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:44:30.655542 runez-4.0.0/src/runez/colors/
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/colors/named.py
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/colors/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)    13751 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17348 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14267 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    13478 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/date.py
--rw-r--r--   0 runner    (1001) docker     (123)    26799 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    38953 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    46450 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/logsetup.py
--rw-r--r--   0 runner    (1001) docker     (123)    24983 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)    35989 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/pyenv.py
--rw-r--r--   0 runner    (1001) docker     (123)    17939 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    11463 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    27665 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    82250 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:44:30.655542 runez-4.0.0/src/runez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-31 16:44:30.000000 runez-4.0.0/src/runez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-31 16:44:30.000000 runez-4.0.0/src/runez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 16:44:30.000000 runez-4.0.0/src/runez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 16:44:30.000000 runez-4.0.0/src/runez.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:44:30.655542 runez-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_cached_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_click.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    25749 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_logsetup.py
--rw-r--r--   0 runner    (1001) docker     (123)    17003 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)    26502 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_pyenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_slotted.py
--rw-r--r--   0 runner    (1001) docker     (123)    31192 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:36:50.547795 runez-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-19 14:36:03.000000 runez-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-19 14:36:03.000000 runez-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-06-19 14:36:50.547795 runez-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-06-19 14:36:03.000000 runez-4.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-19 14:36:03.000000 runez-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 14:36:50.547795 runez-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-19 14:36:03.000000 runez-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:36:50.539795 runez-4.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:36:50.543794 runez-4.0.1/src/runez/
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/ascii.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15102 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/click.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:36:50.543794 runez-4.0.1/src/runez/colors/
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/colors/named.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/colors/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13751 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17348 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14267 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13478 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26799 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38953 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46450 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/logsetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24983 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37142 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/pyenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17939 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11463 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27665 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82291 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-19 14:36:03.000000 runez-4.0.1/src/runez/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:36:50.543794 runez-4.0.1/src/runez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-06-19 14:36:50.000000 runez-4.0.1/src/runez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-19 14:36:50.000000 runez-4.0.1/src/runez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 14:36:50.000000 runez-4.0.1/src/runez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 14:36:50.000000 runez-4.0.1/src/runez.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:36:50.543794 runez-4.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-19 14:36:03.000000 runez-4.0.1/tests/test_cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-06-19 14:36:03.000000 runez-4.0.1/tests/test_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-19 14:36:03.000000 runez-4.0.1/tests/test_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-19 14:36:03.000000 runez-4.0.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-06-19 14:36:03.000000 runez-4.0.1/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-06-19 14:36:03.000000 runez-4.0.1/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-06-19 14:36:03.000000 runez-4.0.1/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-19 14:36:03.000000 runez-4.0.1/tests/test_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-06-19 14:36:03.000000 runez-4.0.1/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-19 14:36:03.000000 runez-4.0.1/tests/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25749 2023-06-19 14:36:03.000000 runez-4.0.1/tests/test_logsetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17003 2023-06-19 14:36:03.000000 runez-4.0.1/tests/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-19 14:36:03.000000 runez-4.0.1/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28609 2023-06-19 14:36:03.000000 runez-4.0.1/tests/test_pyenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-06-19 14:36:03.000000 runez-4.0.1/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-06-19 14:36:03.000000 runez-4.0.1/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-06-19 14:36:03.000000 runez-4.0.1/tests/test_serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-19 14:36:03.000000 runez-4.0.1/tests/test_slotted.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31192 2023-06-19 14:36:03.000000 runez-4.0.1/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-06-19 14:36:03.000000 runez-4.0.1/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-19 14:36:03.000000 runez-4.0.1/tests/test_thread.py
```

### Comparing `runez-4.0.0/LICENSE` & `runez-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/PKG-INFO` & `runez-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runez
-Version: 4.0.0
+Version: 4.0.1
 Summary: Friendly misc/utils/convenience library
 Home-page: https://github.com/codrsquad/runez
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/runez/wiki
 Project-URL: Release notes, https://github.com/codrsquad/runez/wiki/Release-notes
```

### Comparing `runez-4.0.0/README.rst` & `runez-4.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/setup.py` & `runez-4.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/__init__.py` & `runez-4.0.1/src/runez/__init__.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/__main__.py` & `runez-4.0.1/src/runez/__main__.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/ascii.py` & `runez-4.0.1/src/runez/ascii.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/click.py` & `runez-4.0.1/src/runez/click.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/colors/__init__.py` & `runez-4.0.1/src/runez/colors/__init__.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/colors/named.py` & `runez-4.0.1/src/runez/colors/named.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/colors/terminal.py` & `runez-4.0.1/src/runez/colors/terminal.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/config.py` & `runez-4.0.1/src/runez/config.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/conftest.py` & `runez-4.0.1/src/runez/conftest.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/convert.py` & `runez-4.0.1/src/runez/convert.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/date.py` & `runez-4.0.1/src/runez/date.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/file.py` & `runez-4.0.1/src/runez/file.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/heartbeat.py` & `runez-4.0.1/src/runez/heartbeat.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/http.py` & `runez-4.0.1/src/runez/http.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/inspector.py` & `runez-4.0.1/src/runez/inspector.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/logsetup.py` & `runez-4.0.1/src/runez/logsetup.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/program.py` & `runez-4.0.1/src/runez/program.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/prompt.py` & `runez-4.0.1/src/runez/prompt.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/pyenv.py` & `runez-4.0.1/src/runez/pyenv.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,20 +125,18 @@
 
     @classmethod
     def is_acceptable(cls, name):
         """Is 'name' an acceptable pypi package name?"""
         return bool(isinstance(name, str) and name != "UNKNOWN" and cls.RX_ACCEPTABLE_PACKAGE_NAME.match(name))
 
     @classmethod
-    def std_package_name(cls, name, allow_dots=True):
+    def std_package_name(cls, name):
         """Standardized pypi package name, single dashes and alphanumeric chars allowed only"""
         if cls.is_acceptable(name):
-            if not allow_dots:
-                name = name.replace(".", "-")
-
+            name = name.replace(".", "-")
             dashed = cls.RR_PYPI.sub("-", name).lower()
             return cls.RR_PYPI.sub("-", dashed)  # 2nd pass to ensure no `--` remains
 
     @classmethod
     def std_wheel_basename(cls, name):
         """Standardized wheel file base name, single underscores, dots and alphanumeric chars only"""
         if cls.is_acceptable(name):
@@ -329,42 +327,73 @@
         Args:
             color (callable | None): Optional color to use
             compact (str | list | set | tuple | bool | None): Show version only, if `self.family` is mentioned in `compact`
 
         Returns:
             (str): Textual representation of this spec
         """
+        text = self.canonical
         if compact and (compact is True or self.family in compact):
-            return _R.colored(self.version, color)
+            text = self.version.text
+            if self.is_min_spec:
+                text += "+"
 
-        return _R.colored(self.canonical, color)
+        return _R.colored(text, color)
 
     @classmethod
     def from_text(cls, text):
         """
         Args:
             text (str | None): Text to be converted into a PythonSpec() if possible, eg: 3.10, py310, python3.10, conda:3.10
 
         Returns:
             (PythonSpec | None): Parsed spec from given object, if valid
         """
-        if not text or isinstance(text, PythonSpec):
-            return text or None
-
         m = re.match(r"^(py|python|)(?P<version>\d+(\.\d+(.\w+)*)?)?(?P<min_spec>\+?)$", text)
         if m:
             version = Version.from_tox_like(m.group("version"), default="3")
             return cls(CPYTHON, version, is_min_spec=bool(m.group("min_spec"))) if version else None
 
         m = re.match(r"^(?P<family>cpython|conda|pypy):(?P<version>\d+(\.\d+){0,2})(?P<min_spec>\+?)$", text)
         if m:
             version = Version.from_tox_like(m.group("version"))
             return cls(m.group("family"), version, is_min_spec=bool(m.group("min_spec"))) if version else None
 
     @classmethod
+    def from_object(cls, value):
+        """
+        Args:
+            value: Value to transform into a PythonSpec, if possible
+
+        Returns:
+            (PythonSpec | None): Parsed spec from given object, if valid
+        """
+        if not value or isinstance(value, PythonSpec):
+            return value or None
+
+        if isinstance(value, Version):
+            return cls(CPYTHON, value)
+
+        if value:
+            return cls.from_text(str(value))
+
+    @classmethod
+    def to_list(cls, values):
+        """
+        Args:
+            values: Values to transform into a list of PythonSpec-s
+
+        Returns:
+            (list[PythonSpec]): Corresponding list of PythonSpec-s
+        """
+        values = flattened(values, split=",", transform=PythonSpec.from_object)
+        values = [x for x in values if x and x.version]
+        return values
+
+    @classmethod
     def guess_family(cls, text):
         """
         Args:
             text (str | None): Text to examine
 
         Returns:
             (str): Guessed python family from given 'text' (typically path to installation)
@@ -416,35 +445,38 @@
             if python and not python.problem:
                 self.preferred_python = python
                 return
 
     def find_python(self, spec):
         """
         Args:
-            spec (str | pathlib.Path | PythonSpec | None): Example: 3.7, py37, pypy:3.7, /usr/bin/python3
+            spec (str | pathlib.Path | PythonInstallation | PythonSpec | None): Example: 3.7, py37, pypy:3.7, /usr/bin/python3
 
         Returns:
             (PythonInstallation): Object representing python installation (may not be usable, see reported .problem)
         """
+        if isinstance(spec, PythonInstallation):
+            return spec
+
         python = PyInstallInfo.cached_by_path.get(spec)
         if python is None:
             python = self._find_python(spec)
             if python is None:
-                python = PythonInstallation(spec, _info=PyInstallInfo(problem="not available"))
+                python = PythonInstallation(None, short_name=str(spec), _info=PyInstallInfo(problem="not available"))
 
         return python
 
     def _find_python(self, spec):
         if not spec:
             return self.preferred_python or self.invoker
 
         if _is_path(spec):
             return PythonInstallation.from_path(spec)
 
-        spec = PythonSpec.from_text(spec)
+        spec = PythonSpec.from_object(spec)
         if not spec:
             return None
 
         if self.preferred_python and self.preferred_python.satisfies(spec):
             return self.preferred_python
 
         for location in self.locations:
@@ -717,35 +749,34 @@
 
 class PythonInstallation:
     """Models a specific python installation"""
 
     def __init__(self, exe, short_name=None, _info=None):
         """
         Args:
-            exe (str | pathlib.Path): Full path to python executable
+            exe (str | pathlib.Path | None): Full path to python executable
             short_name (str | None): Used to textually represent this installation
             _info (PyInstallInfo | None): Internal use, python installation info, when already known
         """
         exe = resolved_path(exe)
         self._info = _info
-        if ".framework/" in exe:
-            # Simplify macos ridiculous paths
+        if exe and ".framework/" in exe:  # Simplify macos ridiculous paths
             location = "/usr/bin"
             if "Cellar" in exe:
                 i = exe.index("Cellar")
                 location = exe[:i].rstrip("/")
                 if not location.endswith("bin"):
                     location = os.path.join(location, "bin")
 
             m = re.search(r"Versions/(\d)", exe)
             if m:
                 exe = os.path.join(location, "python%s" % m.group(1))
                 short_name = None  # By default, short name if the long folder containing bin/
 
-        self.executable = exe
+        self.executable = exe or short_name
         self.family = PythonSpec.guess_family(exe)
         self.short_name = short_name or short(exe)
 
     def __repr__(self):
         text = joined(self.problem or self.mm_spec, self.is_invoker and "invoker", delimiter=", ")
         return "%s [%s]" % (short(self.short_name), text)
 
@@ -769,15 +800,15 @@
         cached = PyInstallInfo.cached_by_path.get(path)
         if cached is not None:
             return cached
 
         cached = cls(path, short_name=short_name, _info=_info)
         PyInstallInfo.cached_by_path[path] = cached
         PyInstallInfo.cached_by_path[to_path(path)] = cached
-        if cached.executable != path:
+        if cached.executable and cached.executable != path:
             # Can be different on macOS, with simplified from /Library/.../Frameworks/... -> /usr/bin/python3
             PyInstallInfo.cached_by_path[cached.executable] = cached
             PyInstallInfo.cached_by_path[to_path(cached.executable)] = cached
 
         return cached
 
     @classmethod
@@ -799,14 +830,20 @@
             path = os.path.join(exe_folder, "python%s" % (mm[0] if mm else 3))
             if not is_executable(path):
                 path = os.path.join(exe_folder, "python")
 
         return cls.from_exe(path, short_name=short(folder), _info=_info)
 
     @cached_property
+    def folder(self) -> pathlib.Path:
+        """Folder containing python executable"""
+        if self.executable:
+            return to_path(self.executable).parent
+
+    @cached_property
     def full_spec(self):
         """Full spec, can require dynamic inspection of executable"""
         if self.full_version:
             return PythonSpec(self.family, self.full_version)
 
     @cached_property
     def full_version(self):
```

### Comparing `runez-4.0.0/src/runez/render.py` & `runez-4.0.1/src/runez/render.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/schema.py` & `runez-4.0.1/src/runez/schema.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/serialize.py` & `runez-4.0.1/src/runez/serialize.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez/system.py` & `runez-4.0.1/src/runez/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,18 +391,19 @@
         try:
             from importlib import metadata
 
             version = metadata.version(top_level)
             if version:
                 return version
 
-        except (ImportError, Exception) as e:  # Python < 3.8
+        except (ImportError, Exception) as e:
             last_exception = e
 
         try:
+            # TODO: Remove when py3.7 support is dropped
             import pkg_resources
 
             d = pkg_resources.get_distribution(top_level)
             if d and d.version:
                 return d.version
 
         except (ImportError, Exception) as e:
```

### Comparing `runez-4.0.0/src/runez/thread.py` & `runez-4.0.1/src/runez/thread.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/src/runez.egg-info/PKG-INFO` & `runez-4.0.1/src/runez.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runez
-Version: 4.0.0
+Version: 4.0.1
 Summary: Friendly misc/utils/convenience library
 Home-page: https://github.com/codrsquad/runez
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/runez/wiki
 Project-URL: Release notes, https://github.com/codrsquad/runez/wiki/Release-notes
```

### Comparing `runez-4.0.0/src/runez.egg-info/SOURCES.txt` & `runez-4.0.1/src/runez.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/tests/test_cached_property.py` & `runez-4.0.1/tests/test_cached_property.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/tests/test_click.py` & `runez-4.0.1/tests/test_click.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/tests/test_colors.py` & `runez-4.0.1/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/tests/test_config.py` & `runez-4.0.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/tests/test_convert.py` & `runez-4.0.1/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/tests/test_date.py` & `runez-4.0.1/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/tests/test_file.py` & `runez-4.0.1/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/tests/test_heartbeat.py` & `runez-4.0.1/tests/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/tests/test_http.py` & `runez-4.0.1/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/tests/test_inspector.py` & `runez-4.0.1/tests/test_inspector.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/tests/test_logsetup.py` & `runez-4.0.1/tests/test_logsetup.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/tests/test_program.py` & `runez-4.0.1/tests/test_program.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/tests/test_prompt.py` & `runez-4.0.1/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/tests/test_pyenv.py` & `runez-4.0.1/tests/test_pyenv.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,44 @@
 import os
 import sys
 
 import pytest
 
 import runez
 from runez.http import RestClient
-from runez.pyenv import PypiStd, PythonDepot, PythonInstallation, PythonSpec, Version
+from runez.pyenv import ArtifactInfo, PypiStd, PythonDepot, PythonInstallation, PythonSpec, Version
 
 
 PYPI_CLIENT = RestClient("https://example.com/pypi")
 
 
+def test_artifact_info():
+    info = ArtifactInfo.from_basename("E.S.P.-Hadouken-0.2.1.tar.gz")
+    assert str(info) == "e-s-p-hadouken/E.S.P.-Hadouken-0.2.1.tar.gz"
+    assert info.category == "sdist"
+    assert not info.is_dirty
+    assert not info.is_wheel
+    assert info.package_name == "E.S.P.-Hadouken"
+    assert info.pypi_name == "e-s-p-hadouken"
+    assert info.tags is None
+    assert info.version == "0.2.1"
+    assert info.wheel_build_number is None
+
+    info = ArtifactInfo.from_basename("a_b-1!0.0.1-10-py3-none-any.whl", None)
+    assert str(info) == "a-b/a_b-1!0.0.1-10-py3-none-any.whl"
+    assert info.category == "wheel"
+    assert not info.is_dirty
+    assert info.is_wheel
+    assert info.package_name == "a_b"
+    assert info.pypi_name == "a-b"
+    assert info.tags == "py3-none-any"
+    assert info.version == "1!0.0.1"
+    assert info.wheel_build_number == "10"
+
+
 def mk_python(basename, prefix=None, base_prefix=None, executable=True, content=None):
     if basename[0].isdigit():
         version = Version(basename)
         folder = runez.to_path(".pyenv/versions") / basename / "bin"
 
     else:
         version = Version(os.path.basename(basename))
@@ -54,22 +78,24 @@
 
     depot = PythonDepot(".pyenv/versions/**")
     assert len(depot.available_pythons) == 4
 
     assert str(depot.find_python("8.5.4")) == "8.5.4 [not available]"
     invalid = depot.find_python(".pyenv/versions/8.5.4")
     assert str(invalid) == ".pyenv/versions/8.5.4 [internal error: _pv returned 'invalid']"
+    assert invalid.folder == runez.to_path(".pyenv/versions/8.5.4/bin").absolute()
     bad_version = depot.find_python(".pyenv/versions/8.5.5")
     assert str(bad_version) == ".pyenv/versions/8.5.5 [invalid version 'invalid-version']"
 
     versions = [p.mm_spec.canonical for p in depot.available_pythons]
     assert versions == ["pypy:9.8", "cpython:8.7", "cpython:8.6", "conda:9.11"]
 
     # Verify that latest available is found (when under-specified)
     p8 = depot.find_python("8")
+    assert p8.folder == runez.to_path(".pyenv/versions/8.7.2/bin").absolute()
     assert not p8.is_virtualenv
     assert repr(p8) == ".pyenv/versions/8.7.2 [cpython:8.7]"
     assert str(p8) == ".pyenv/versions/8.7.2 [cpython:8.7.2]"
 
     # Verify that preferred python is respected
     depot.set_preferred_python("8.6")
     assert repr(depot.find_python("8")) == ".pyenv/versions/8.6.1 [cpython:8.6]"
@@ -118,16 +144,21 @@
     assert depot.representation() == "No PythonDepot locations configured"
     assert not depot.available_pythons
     invoker = runez.SYS_INFO.invoker_python
     assert ", invoker" in repr(invoker)
     assert ", invoker" in str(invoker)
 
     mm = invoker.mm
+    p95_spec = PythonSpec.from_text("9.5")
+    p95 = depot.find_python(p95_spec)
+    assert p95.problem
     assert depot.find_python(None) is invoker
+    assert depot.find_python("") is invoker
     assert depot.find_python("invoker") is invoker
+    assert depot.find_python(invoker) is invoker
     assert depot.find_python(invoker.executable) is invoker
     assert depot.find_python(runez.to_path(invoker.executable)) is invoker
     assert depot.find_python(PythonSpec("cpython", mm)) is invoker
     assert depot.find_python("python") is invoker
     assert depot.find_python("py%s" % mm) is invoker  # eg: py3.10
     assert depot.find_python("py%s" % mm.text.replace(".", "")) is invoker  # tox style: py310
     assert depot.find_python(mm.text) is invoker
@@ -142,15 +173,21 @@
     assert p.problem == "not available"
     assert p.mm_spec is None
     assert p.major is None
     assert p.full_version is None
 
     # Disabling invoker still finds it explicitly, but not by generic spec
     depot.invoker = None
-    assert depot.find_python("invoker") is invoker  # Found only if explicitly referred to
+
+    # Found only if explicitly referred to
+    assert depot.find_python("invoker") is invoker
+    assert depot.find_python(invoker) is invoker
+
+    assert str(depot.find_python(None)) == "None [not available]"
+    assert str(depot.find_python("")) == "None [not available]"
     assert str(depot.find_python("python")) == "python [not available]"
     assert str(depot.find_python(mm.text)) == "%s [not available]" % mm
 
 
 def test_invoker(monkeypatch):
     from runez.pyenv import PyInstallInfo
 
@@ -196,18 +233,17 @@
     assert PypiStd.std_package_name(None) is None
     assert PypiStd.std_package_name(5) is None
     assert PypiStd.std_package_name("") is None
     assert PypiStd.std_package_name("-a-") is None
     assert PypiStd.std_package_name("a") is None
     assert PypiStd.std_package_name("foo") == "foo"
     assert PypiStd.std_package_name("Foo") == "foo"
-    assert PypiStd.std_package_name("A__b-c_1.0") == "a-b-c-1.0"
+    assert PypiStd.std_package_name("A__b-c_1.0") == "a-b-c-1-0"
     assert PypiStd.std_package_name("some_-Test") == "some-test"
-    assert PypiStd.std_package_name("a_-_-.-_.--b") == "a-.-.-b"
-    assert PypiStd.std_package_name("a_-_-.-_.--b", allow_dots=False) == "a-b"
+    assert PypiStd.std_package_name("a_-_-.-_.--b") == "a-b"
 
     assert PypiStd.std_wheel_basename(None) is None
     assert PypiStd.std_package_name(10.1) is None
     assert PypiStd.std_wheel_basename("") is None
     assert PypiStd.std_wheel_basename("a.b_-_1.5--c") == "a.b_1.5_c"
     assert PypiStd.std_wheel_basename("a.b_-___1.5--c") == "a.b_1.5_c"
 
@@ -291,28 +327,37 @@
     black = sorted(PypiStd.ls_pypi("black"))  # All versions are pre-releases
     assert len(black) == 3
     assert black[0].version.prerelease
 
     funky = sorted(PypiStd.ls_pypi("funky-proj", source=None))
     assert len(funky) == 2
     assert funky[0].package_name == "funky.proj"
-    assert funky[0].pypi_name == "funky.proj"
+    assert funky[0].pypi_name == "funky-proj"
     assert funky[1].is_dirty
     assert black[0] < funky[0]  # Alphabetical sort when both have no source
     assert funky[0] < sample[4]  # Arbitrary: no-source sorts lowest...
 
 
 def test_spec():
     p3 = PythonSpec.from_text("3")
     p3plus = PythonSpec.from_text("3+")
     assert str(p3) == "cpython:3"
     assert str(p3plus) == "cpython:3+"
     assert not p3.is_min_spec
     assert p3plus.is_min_spec
 
+    assert p3 == PythonSpec.from_object(Version("3"))
+
+    p3_rep = p3.represented()
+    p3plus_rep = p3plus.represented()
+    assert isinstance(p3_rep, str)
+    assert isinstance(p3plus_rep, str)
+    assert p3_rep == "3"
+    assert p3plus_rep == "3+"
+
     p38 = PythonSpec.from_text("3.8")
     assert p38.satisfies(p3)
     assert p38.satisfies(p3plus)
 
     p38plus = PythonSpec.from_text("3.8+")
     c38 = PythonSpec.from_text("conda:3.8")
     assert c38 != p38
@@ -355,18 +400,21 @@
     check_equivalent_specs("3+", "py3+", "python3+", "cpython:3+")
     check_equivalent_specs("3.10", "310", "py3.10", "py310", "python3.10", "python310", "cpython:3.10")
     check_equivalent_specs("3.10+", "310+", "py3.10+", "py310+", "python3.10+", "python310+", "cpython:3.10+")
     check_equivalent_specs("3777", "py3.777", "python3.777", "cpython:3.777")
 
 
 def test_spec_invalid():
+    assert PythonSpec.from_object(None) is None
+    assert PythonSpec.from_object([]) is None
+    assert PythonSpec.from_object(["foo"]) is None
+
     def check_spec_invalid(text):
         assert PythonSpec.from_text(text) is None
 
-    check_spec_invalid(None)
     check_spec_invalid("foo")
     check_spec_invalid("foo:3")
     check_spec_invalid("cpython")
     check_spec_invalid("cpython:")
     check_spec_invalid("cpython:3.10.0rc1")
     check_spec_invalid("cpython:+")
     check_spec_invalid("cpython: 3")
@@ -374,14 +422,23 @@
     check_spec_invalid("python:3")
     check_spec_invalid("p3.9")
     check_spec_invalid("pY3")
     check_spec_invalid("3.9.9a")
     check_spec_invalid("3.9.9++")
 
 
+def test_spec_list():
+    assert not PythonSpec.to_list("a,b")
+    x = PythonSpec.to_list("3.10,py39")
+    assert x == [PythonSpec.from_text("3.10"), PythonSpec.from_text("3.9")]
+
+    x = PythonSpec.to_list(["3.10,py36", "foo,py37", 3.8])
+    assert x == [PythonSpec.from_text("3.10"), PythonSpec.from_text("3.6"), PythonSpec.from_text("3.7"), PythonSpec.from_text("3.8")]
+
+
 def test_venv(temp_folder):
     # Simulate an explicit reference to a venv python
     mk_python("./some-venv/bin/8.6.1", prefix="foo", base_prefix=".pyenv/versions/8.6.1")
 
     depot = PythonDepot()
     assert not depot.available_pythons
     pvenv = depot.find_python("./some-venv/bin/python")
```

### Comparing `runez-4.0.0/tests/test_render.py` & `runez-4.0.1/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/tests/test_schema.py` & `runez-4.0.1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/tests/test_serialize.py` & `runez-4.0.1/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/tests/test_slotted.py` & `runez-4.0.1/tests/test_slotted.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/tests/test_system.py` & `runez-4.0.1/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/tests/test_testing.py` & `runez-4.0.1/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `runez-4.0.0/tests/test_thread.py` & `runez-4.0.1/tests/test_thread.py`

 * *Files identical despite different names*

