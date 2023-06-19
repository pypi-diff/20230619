# Comparing `tmp/piel-0.0.25.tar.gz` & `tmp/piel-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piel-0.0.25.tar", last modified: Sun Jun 18 13:59:18 2023, max compression
+gzip compressed data, was "piel-0.0.26.tar", last modified: Mon Jun 19 09:42:09 2023, max compression
```

## Comparing `piel-0.0.25.tar` & `piel-0.0.26.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.652661 piel-0.0.25/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-18 13:59:03.000000 piel-0.0.25/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-18 13:59:03.000000 piel-0.0.25/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-18 13:59:03.000000 piel-0.0.25/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-18 13:59:03.000000 piel-0.0.25/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-18 13:59:03.000000 piel-0.0.25/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-18 13:59:18.652661 piel-0.0.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-18 13:59:03.000000 piel-0.0.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-18 13:59:03.000000 piel-0.0.25/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-18 13:59:03.000000 piel-0.0.25/docs/authors.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/piel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/piel/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/piel/cli/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/piel/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/piel/defaults/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/piel/file_system/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/piel/file_system/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/piel/gdsfactory/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/piel/gdsfactory/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/piel/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/piel/openlane_v1/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/piel/openlane_v1/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/piel/openlane_v2/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/piel/openlane_v2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/piel/parametric/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/piel/parametric/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/piel/piel/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/piel/piel/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/piel/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/piel/simulation/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-18 13:59:03.000000 piel-0.0.25/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-18 13:59:03.000000 piel-0.0.25/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.644661 piel-0.0.25/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.644661 piel-0.0.25/docs/examples/simple_design/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/examples/simple_design/tb/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-18 13:59:03.000000 piel-0.0.25/docs/examples/simple_design/tb/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-18 13:59:03.000000 piel-0.0.25/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-18 13:59:03.000000 piel-0.0.25/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-18 13:59:03.000000 piel-0.0.25/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-18 13:59:03.000000 piel-0.0.25/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-18 13:59:03.000000 piel-0.0.25/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.644661 piel-0.0.25/docs/sections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/sections/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-18 13:59:03.000000 piel-0.0.25/docs/sections/environment/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-18 13:59:03.000000 piel-0.0.25/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/piel/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-18 13:59:03.000000 piel-0.0.25/piel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-18 13:59:03.000000 piel-0.0.25/piel/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-18 13:59:03.000000 piel-0.0.25/piel/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-18 13:59:03.000000 piel-0.0.25/piel/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-18 13:59:03.000000 piel-0.0.25/piel/gdsfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-18 13:59:03.000000 piel-0.0.25/piel/openlane_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-18 13:59:03.000000 piel-0.0.25/piel/openlane_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-18 13:59:03.000000 piel-0.0.25/piel/parametric.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 13:59:03.000000 piel-0.0.25/piel/piel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-18 13:59:03.000000 piel-0.0.25/piel/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.652661 piel-0.0.25/piel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-18 13:59:18.000000 piel-0.0.25/piel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-18 13:59:18.000000 piel-0.0.25/piel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 13:59:18.000000 piel-0.0.25/piel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-18 13:59:18.000000 piel-0.0.25/piel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 13:59:18.000000 piel-0.0.25/piel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-18 13:59:18.000000 piel-0.0.25/piel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-18 13:59:18.000000 piel-0.0.25/piel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-18 13:59:18.652661 piel-0.0.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-18 13:59:03.000000 piel-0.0.25/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.652661 piel-0.0.25/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-18 13:59:03.000000 piel-0.0.25/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-18 13:59:03.000000 piel-0.0.25/tests/test_piel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.537931 piel-0.0.26/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-19 09:41:52.000000 piel-0.0.26/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-19 09:41:52.000000 piel-0.0.26/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-19 09:41:52.000000 piel-0.0.26/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-19 09:41:52.000000 piel-0.0.26/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-19 09:41:52.000000 piel-0.0.26/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-19 09:42:09.537931 piel-0.0.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-19 09:41:52.000000 piel-0.0.26/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-19 09:41:52.000000 piel-0.0.26/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 09:41:52.000000 piel-0.0.26/docs/authors.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/piel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/piel/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/piel/cli/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/piel/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/piel/defaults/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/piel/file_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/piel/file_system/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/piel/gdsfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/piel/gdsfactory/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/piel/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/piel/openlane_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/piel/openlane_v1/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/piel/openlane_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/piel/openlane_v2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/piel/parametric/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/piel/parametric/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/piel/piel/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/piel/piel/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/piel/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/piel/simulation/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-19 09:41:52.000000 piel-0.0.26/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-19 09:41:52.000000 piel-0.0.26/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.529931 piel-0.0.26/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.529931 piel-0.0.26/docs/examples/simple_design/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/examples/simple_design/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-19 09:41:52.000000 piel-0.0.26/docs/examples/simple_design/tb/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-19 09:41:52.000000 piel-0.0.26/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 09:41:52.000000 piel-0.0.26/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-19 09:41:52.000000 piel-0.0.26/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-19 09:41:52.000000 piel-0.0.26/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-19 09:41:52.000000 piel-0.0.26/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.529931 piel-0.0.26/docs/sections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/sections/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-19 09:41:52.000000 piel-0.0.26/docs/sections/environment/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-19 09:41:52.000000 piel-0.0.26/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.537931 piel-0.0.26/piel/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-19 09:41:52.000000 piel-0.0.26/piel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-19 09:41:52.000000 piel-0.0.26/piel/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-19 09:41:52.000000 piel-0.0.26/piel/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-19 09:41:52.000000 piel-0.0.26/piel/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-19 09:41:52.000000 piel-0.0.26/piel/gdsfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-19 09:41:52.000000 piel-0.0.26/piel/openlane_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-19 09:41:52.000000 piel-0.0.26/piel/openlane_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-19 09:41:52.000000 piel-0.0.26/piel/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 09:41:52.000000 piel-0.0.26/piel/piel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-19 09:41:52.000000 piel-0.0.26/piel/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.537931 piel-0.0.26/piel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-19 09:42:09.000000 piel-0.0.26/piel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-19 09:42:09.000000 piel-0.0.26/piel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 09:42:09.000000 piel-0.0.26/piel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-19 09:42:09.000000 piel-0.0.26/piel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 09:42:09.000000 piel-0.0.26/piel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-19 09:42:09.000000 piel-0.0.26/piel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-19 09:42:09.000000 piel-0.0.26/piel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-19 09:42:09.537931 piel-0.0.26/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-19 09:41:52.000000 piel-0.0.26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.537931 piel-0.0.26/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 09:41:52.000000 piel-0.0.26/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-19 09:41:52.000000 piel-0.0.26/tests/test_piel.py
```

### Comparing `piel-0.0.25/CONTRIBUTING.rst` & `piel-0.0.26/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.25/LICENSE` & `piel-0.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `piel-0.0.25/PKG-INFO` & `piel-0.0.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.25
+Version: 0.0.26
 Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `piel-0.0.25/README.md` & `piel-0.0.26/README.md`

 * *Files identical despite different names*

### Comparing `piel-0.0.25/docs/Makefile` & `piel-0.0.26/docs/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.25/docs/autoapi/piel/file_system/index.rst` & `piel-0.0.26/docs/autoapi/piel/file_system/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.25/docs/autoapi/piel/gdsfactory/index.rst` & `piel-0.0.26/docs/autoapi/piel/gdsfactory/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.25/docs/autoapi/piel/index.rst` & `piel-0.0.26/docs/autoapi/piel/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 .. py:data:: __email__
    :value: 'darioaquintero@gmail.com'
 
    
 
 .. py:data:: __version__
-   :value: '0.0.24'
+   :value: '0.0.25'
 
    
 
 .. py:data:: test_spm_open_lane_configuration
```

### Comparing `piel-0.0.25/docs/autoapi/piel/openlane_v2/index.rst` & `piel-0.0.26/docs/autoapi/piel/openlane_v2/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.25/docs/autoapi/piel/parametric/index.rst` & `piel-0.0.26/docs/autoapi/piel/parametric/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.25/docs/autoapi/piel/simulation/index.rst` & `piel-0.0.26/docs/autoapi/piel/simulation/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.25/docs/conf.py` & `piel-0.0.26/docs/conf.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.25/docs/examples/simple_design/tb/Makefile` & `piel-0.0.26/docs/examples/simple_design/tb/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.25/docs/make.bat` & `piel-0.0.26/docs/make.bat`

 * *Files identical despite different names*

### Comparing `piel-0.0.25/piel/defaults.py` & `piel-0.0.26/piel/defaults.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.25/piel/file_system.py` & `piel-0.0.26/piel/file_system.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.25/piel/gdsfactory.py` & `piel-0.0.26/piel/gdsfactory.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.25/piel/openlane_v2.py` & `piel-0.0.26/piel/openlane_v2.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.25/piel/parametric.py` & `piel-0.0.26/piel/parametric.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.25/piel/simulation.py` & `piel-0.0.26/piel/simulation.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.25/piel.egg-info/PKG-INFO` & `piel-0.0.26/piel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.25
+Version: 0.0.26
 Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `piel-0.0.25/piel.egg-info/SOURCES.txt` & `piel-0.0.26/piel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piel-0.0.25/setup.py` & `piel-0.0.26/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,10 +62,10 @@
     include_package_data=True,
     keywords="piel",
     name="piel",
     packages=find_packages(include=["piel", "piel.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url='https://github.com/daquintero/piel',
-    version="0.0.25",
+    version="0.0.26",
     zip_safe=False,
 )
```

### Comparing `piel-0.0.25/tests/test_piel.py` & `piel-0.0.26/tests/test_piel.py`

 * *Files identical despite different names*

