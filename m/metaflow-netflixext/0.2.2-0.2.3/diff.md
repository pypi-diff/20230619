# Comparing `tmp/metaflow-netflixext-0.2.2.tar.gz` & `tmp/metaflow-netflixext-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow-netflixext-0.2.2.tar", last modified: Thu Jun 15 21:17:42 2023, max compression
+gzip compressed data, was "metaflow-netflixext-0.2.3.tar", last modified: Mon Jun 19 12:14:49 2023, max compression
```

## Comparing `metaflow-netflixext-0.2.2.tar` & `metaflow-netflixext-0.2.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.669591 metaflow-netflixext-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-06-15 21:17:42.669591 metaflow-netflixext-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26486 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.665591 metaflow-netflixext-0.2.2/metaflow_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.665591 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.665591 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/cmd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.665591 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/cmd/environment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/cmd/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35592 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/cmd/environment/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/cmd/mfextinit_netflixext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.665591 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/generate_vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.669591 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.669591 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   182021 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    50529 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py
--rw-r--r--   0 runner    (1001) docker     (123)    37939 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.669591 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg
--rw-r--r--   0 runner    (1001) docker     (123)   113678 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    21000 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20971 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/environment_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/mfextinit_netflixext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.669591 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/toplevel/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/toplevel/mfextinit_netflixext.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/toplevel/netflixext_toplevel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.665591 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.669591 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)    39124 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.669591 metaflow-netflixext-0.2.2/metaflow_netflixext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-06-15 21:17:42.000000 metaflow-netflixext-0.2.2/metaflow_netflixext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-15 21:17:42.000000 metaflow-netflixext-0.2.2/metaflow_netflixext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:17:42.000000 metaflow-netflixext-0.2.2/metaflow_netflixext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 21:17:42.000000 metaflow-netflixext-0.2.2/metaflow_netflixext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 21:17:42.000000 metaflow-netflixext-0.2.2/metaflow_netflixext.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 21:17:42.669591 metaflow-netflixext-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:14:49.791461 metaflow-netflixext-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-06-19 12:14:49.791461 metaflow-netflixext-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26486 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:14:49.779461 metaflow-netflixext-0.2.3/metaflow_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:14:49.783461 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:14:49.783461 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/cmd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:14:49.783461 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/cmd/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/cmd/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35592 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/cmd/environment/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/cmd/mfextinit_netflixext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:14:49.783461 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/generate_vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:14:49.787461 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:14:49.787461 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182212 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50529 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37939 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:14:49.787461 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   113678 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21000 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20971 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/environment_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/mfextinit_netflixext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:14:49.787461 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/toplevel/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/toplevel/mfextinit_netflixext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/toplevel/netflixext_toplevel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:14:49.783461 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:14:49.791461 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39124 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:14:49.791461 metaflow-netflixext-0.2.3/metaflow_netflixext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-06-19 12:14:49.000000 metaflow-netflixext-0.2.3/metaflow_netflixext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-19 12:14:49.000000 metaflow-netflixext-0.2.3/metaflow_netflixext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 12:14:49.000000 metaflow-netflixext-0.2.3/metaflow_netflixext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-19 12:14:49.000000 metaflow-netflixext-0.2.3/metaflow_netflixext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-19 12:14:49.000000 metaflow-netflixext-0.2.3/metaflow_netflixext.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 12:14:49.791461 metaflow-netflixext-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-19 12:14:40.000000 metaflow-netflixext-0.2.3/setup.py
```

### Comparing `metaflow-netflixext-0.2.2/LICENSE` & `metaflow-netflixext-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/PKG-INFO` & `metaflow-netflixext-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-netflixext
-Version: 0.2.2
+Version: 0.2.3
 Summary: EXPERIMENTAL Metaflow extensions from Netflix
 Author: Netflix Metaflow Developers
 Author-email: metaflow-dev@netflix.com
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow-nflx-extensions
 Project-URL: Tracker, https://github.com/Netflix/metaflow-nflx-extensions/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `metaflow-netflixext-0.2.2/README.md` & `metaflow-netflixext-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/cmd/environment/utils.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/cmd/environment/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/generate_vendor.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/generate_vendor.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/conda.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/conda.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,22 +76,20 @@
     CondaStepException,
     arch_id,
     auth_from_urls,
     change_pip_package_version,
     correct_splitext,
     get_conda_root,
     is_alias_mutable,
-    merge_dep_dicts,
     parse_explicit_url_conda,
     parse_explicit_url_pip,
     parse_explicit_path_pip,
     pip_tags_from_arch,
     plural_marker,
     resolve_env_alias,
-    split_into_dict,
 )
 
 from .env_descr import (
     CondaCachePackage,
     CondaPackageSpecification,
     EnvID,
     EnvType,
@@ -2056,14 +2054,16 @@
                 # full of packages that we may not want to use so we will create symlinks
                 # to packages we already have and download the others
                 base_local_pip_packages = os.path.join(self._package_dirs[0], "pip")
                 tmp_local_pip_packages = os.path.realpath(
                     os.path.join(pip_dir, "local_packages", "pip")
                 )
                 os.makedirs(tmp_local_pip_packages)
+                # Create this in case we need to move the local packages at some point
+                os.makedirs(base_local_pip_packages, exist_ok=True)
                 new_local_packages = []  # type: List[PackageSpecification]
                 for p in local_packages:
                     for fmt in PipPackageSpecification.allowed_formats():
                         filename = "%s%s" % (p.filename, fmt)
                         if os.path.isfile(
                             os.path.join(base_local_pip_packages, filename)
                         ):
@@ -2819,25 +2819,27 @@
         # Value: list of possible cache paths
         possible_wheels = {}  # type: Dict[str, List[str]]
         for cache_path, is_file in found_files:
             cache_path = cast(str, cache_path).rstrip("/")
             is_file = cast(bool, is_file)
             if is_file:
                 raise CondaException("Invalid cache content at '%s'" % cache_path)
-            keys_to_check.add(cache_path)
             base_cache_path, cache_filename_with_ext = os.path.split(cache_path)
-            cache_format = os.path.splitext(cache_filename_with_ext)[1]
+            cache_format = correct_splitext(cache_filename_with_ext)[1]
             if cache_format != ".whl":
                 # This is a source format -- we add it to the keys_to_check so we can
                 keys_to_check.add(cache_path)
+                debug.conda_exec("Found source package at '%s'" % cache_path)
             else:
                 # There may be multiple wheel files so we want to pick the best one
                 # so we record for now and then we will pick the best one.
                 possible_wheels.setdefault(base_cache_path, []).append(cache_path)
-            debug.conda_exec("Found potential pre-built package at '%s'" % cache_path)
+                debug.conda_exec(
+                    "Found potential pre-built package at '%s'" % cache_path
+                )
 
         # We now check and pick the best wheel if one is compatible and then we will
         # check it further
         for key, wheel_potentials in possible_wheels.items():
             for t in supported_tags:
                 # Tags are ordered from most-preferred to least preferred
                 for p in wheel_potentials:
```

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/utils.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/conda/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/environment_cli.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/plugins/environment_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/markers.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/tags.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/utils.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/version.py` & `metaflow-netflixext-0.2.3/metaflow_extensions/netflix_ext/vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/metaflow_netflixext.egg-info/PKG-INFO` & `metaflow-netflixext-0.2.3/metaflow_netflixext.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-netflixext
-Version: 0.2.2
+Version: 0.2.3
 Summary: EXPERIMENTAL Metaflow extensions from Netflix
 Author: Netflix Metaflow Developers
 Author-email: metaflow-dev@netflix.com
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow-nflx-extensions
 Project-URL: Tracker, https://github.com/Netflix/metaflow-nflx-extensions/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `metaflow-netflixext-0.2.2/metaflow_netflixext.egg-info/SOURCES.txt` & `metaflow-netflixext-0.2.3/metaflow_netflixext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.2/setup.py` & `metaflow-netflixext-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_namespace_packages
 
-version = "0.2.2"
+version = "0.2.3"
 
 setup(
     name="metaflow-netflixext",
     version=version,
     description="EXPERIMENTAL Metaflow extensions from Netflix",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

