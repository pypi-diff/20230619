# Comparing `tmp/obs-cli-0.6.1.tar.gz` & `tmp/obs-cli-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obs-cli-0.6.1.tar", last modified: Tue Jun  6 08:16:39 2023, max compression
+gzip compressed data, was "obs-cli-0.6.2.tar", last modified: Mon Jun 19 09:19:31 2023, max compression
```

## Comparing `obs-cli-0.6.1.tar` & `obs-cli-0.6.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:16:39.679880 obs-cli-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:16:39.679880 obs-cli-0.6.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-06 08:16:27.000000 obs-cli-0.6.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:16:39.679880 obs-cli-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-06 08:16:27.000000 obs-cli-0.6.1/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-06 08:16:27.000000 obs-cli-0.6.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-06 08:16:27.000000 obs-cli-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 08:16:27.000000 obs-cli-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44491 2023-06-06 08:16:39.679880 obs-cli-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-06 08:16:27.000000 obs-cli-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:16:39.679880 obs-cli-0.6.1/obs_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44491 2023-06-06 08:16:39.000000 obs-cli-0.6.1/obs_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-06 08:16:39.000000 obs-cli-0.6.1/obs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:16:39.000000 obs-cli-0.6.1/obs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-06 08:16:39.000000 obs-cli-0.6.1/obs_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 08:16:39.000000 obs-cli-0.6.1/obs_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 08:16:39.000000 obs-cli-0.6.1/obs_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15200 2023-06-06 08:16:27.000000 obs-cli-0.6.1/obs_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-06 08:16:27.000000 obs-cli-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:16:39.679880 obs-cli-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:19:31.467147 obs-cli-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:19:31.463147 obs-cli-0.6.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-19 09:19:19.000000 obs-cli-0.6.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:19:31.463147 obs-cli-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-19 09:19:19.000000 obs-cli-0.6.2/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-19 09:19:19.000000 obs-cli-0.6.2/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-19 09:19:19.000000 obs-cli-0.6.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-19 09:19:19.000000 obs-cli-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-19 09:19:19.000000 obs-cli-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44491 2023-06-19 09:19:31.467147 obs-cli-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-19 09:19:19.000000 obs-cli-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:19:31.467147 obs-cli-0.6.2/obs_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44491 2023-06-19 09:19:31.000000 obs-cli-0.6.2/obs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-19 09:19:31.000000 obs-cli-0.6.2/obs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 09:19:31.000000 obs-cli-0.6.2/obs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-19 09:19:31.000000 obs-cli-0.6.2/obs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 09:19:31.000000 obs-cli-0.6.2/obs_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 09:19:31.000000 obs-cli-0.6.2/obs_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15381 2023-06-19 09:19:19.000000 obs-cli-0.6.2/obs_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-19 09:19:19.000000 obs-cli-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 09:19:31.467147 obs-cli-0.6.2/setup.cfg
```

### Comparing `obs-cli-0.6.1/.github/workflows/release.yaml` & `obs-cli-0.6.2/.github/workflows/pypi.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-name: Upload Python Package
+name: Python Package
 
 on:
   release:
     types: [created]
   push:
     tags:
       - '*'
 
 jobs:
   pypi-publish:
     name: Upload release to PyPI
     runs-on: ubuntu-latest
     environment:
       name: pypi
-      url: https://pypi.org/p/myl
+      url: https://pypi.org/p/obs-cli
     permissions:
       id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python
       uses: actions/setup-python@v4
```

### Comparing `obs-cli-0.6.1/LICENSE` & `obs-cli-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `obs-cli-0.6.1/PKG-INFO` & `obs-cli-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-cli
-Version: 0.6.1
+Version: 0.6.2
 Summary: OBS CLI
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `obs-cli-0.6.1/README.md` & `obs-cli-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `obs-cli-0.6.1/obs_cli.egg-info/PKG-INFO` & `obs-cli-0.6.2/obs_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-cli
-Version: 0.6.1
+Version: 0.6.2
 Summary: OBS CLI
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `obs-cli-0.6.1/obs_cli.py` & `obs-cli-0.6.2/obs_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 import argparse
+import json
 import logging
 import os
 import re
 import sys
 
 import obsws_python as obs
 from rich import print, print_json
@@ -22,15 +23,15 @@
         "-P", "--port", help="port number", type=int, default=4455
     )
     parser.add_argument(
         "-p", "--password", required=False, help="password ($OBS_API_PASSWORD)"
     )
     parser.add_argument("-j", "--json", action="store_true", default=False)
 
-    subparsers = parser.add_subparsers(dest="command")
+    subparsers = parser.add_subparsers(dest="command", required=True)
 
     scene_parser = subparsers.add_parser("scene")
     scene_parser.add_argument(
         "-e", "--exact", action="store_true", default=False, help="Exact match"
     )
     scene_parser.add_argument(
         "-i",
@@ -195,14 +196,19 @@
 
 
 def get_input_settings(cl, input):
     return cl.get_input_settings(input).input_settings
 
 
 def set_input_setting(cl, input, key, value):
+    try:
+        value = json.loads(value)
+    except (ValueError, TypeError):
+        pass
+    LOGGER.debug(f"Setting {key} to {value} ({type(value)})")
     return cl.set_input_settings(input, {key: value}, overlay=True)
 
 
 def get_filters(cl, input):
     return cl.get_source_filter_list(input).filters
```

### Comparing `obs-cli-0.6.1/pyproject.toml` & `obs-cli-0.6.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "obsws-python",
   "rich"
 ]
-version = "0.6.1"
+version = "0.6.2"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 obs-cli = "obs_cli:main"
```

