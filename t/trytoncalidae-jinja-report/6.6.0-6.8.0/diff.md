# Comparing `tmp/trytoncalidae_jinja_report-6.6.0.tar.gz` & `tmp/trytoncalidae_jinja_report-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytoncalidae_jinja_report-6.6.0.tar", last modified: Fri Nov  4 09:40:56 2022, max compression
+gzip compressed data, was "trytoncalidae_jinja_report-6.8.0.tar", last modified: Mon Jun 19 07:44:56 2023, max compression
```

## Comparing `trytoncalidae_jinja_report-6.6.0.tar` & `trytoncalidae_jinja_report-6.8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 09:40:56.814465 trytoncalidae_jinja_report-6.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-11-04 09:40:45.000000 trytoncalidae_jinja_report-6.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-11-04 09:40:45.000000 trytoncalidae_jinja_report-6.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2656 2022-11-04 09:40:56.814465 trytoncalidae_jinja_report-6.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-11-04 09:40:45.000000 trytoncalidae_jinja_report-6.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-11-04 09:40:45.000000 trytoncalidae_jinja_report-6.6.0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2891 2022-11-04 09:40:45.000000 trytoncalidae_jinja_report-6.6.0/report.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-04 09:40:56.814465 trytoncalidae_jinja_report-6.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3568 2022-11-04 09:40:45.000000 trytoncalidae_jinja_report-6.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 09:40:56.814465 trytoncalidae_jinja_report-6.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 09:40:45.000000 trytoncalidae_jinja_report-6.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2932 2022-11-04 09:40:45.000000 trytoncalidae_jinja_report-6.6.0/tests/test_jinja_report.py
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-11-04 09:40:45.000000 trytoncalidae_jinja_report-6.6.0/tryton.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 09:40:56.814465 trytoncalidae_jinja_report-6.6.0/trytoncalidae_jinja_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2656 2022-11-04 09:40:56.000000 trytoncalidae_jinja_report-6.6.0/trytoncalidae_jinja_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-11-04 09:40:56.000000 trytoncalidae_jinja_report-6.6.0/trytoncalidae_jinja_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 09:40:56.000000 trytoncalidae_jinja_report-6.6.0/trytoncalidae_jinja_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-04 09:40:56.000000 trytoncalidae_jinja_report-6.6.0/trytoncalidae_jinja_report.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 09:40:56.000000 trytoncalidae_jinja_report-6.6.0/trytoncalidae_jinja_report.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-04 09:40:56.000000 trytoncalidae_jinja_report-6.6.0/trytoncalidae_jinja_report.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-04 09:40:56.000000 trytoncalidae_jinja_report-6.6.0/trytoncalidae_jinja_report.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:56.512503 trytoncalidae_jinja_report-6.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-19 07:44:47.000000 trytoncalidae_jinja_report-6.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-19 07:44:47.000000 trytoncalidae_jinja_report-6.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-19 07:44:56.512503 trytoncalidae_jinja_report-6.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-19 07:44:47.000000 trytoncalidae_jinja_report-6.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-19 07:44:47.000000 trytoncalidae_jinja_report-6.8.0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-19 07:44:47.000000 trytoncalidae_jinja_report-6.8.0/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 07:44:56.512503 trytoncalidae_jinja_report-6.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-19 07:44:47.000000 trytoncalidae_jinja_report-6.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:56.508503 trytoncalidae_jinja_report-6.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:47.000000 trytoncalidae_jinja_report-6.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-19 07:44:47.000000 trytoncalidae_jinja_report-6.8.0/tests/test_jinja_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-19 07:44:47.000000 trytoncalidae_jinja_report-6.8.0/tryton.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:56.512503 trytoncalidae_jinja_report-6.8.0/trytoncalidae_jinja_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-19 07:44:56.000000 trytoncalidae_jinja_report-6.8.0/trytoncalidae_jinja_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-19 07:44:56.000000 trytoncalidae_jinja_report-6.8.0/trytoncalidae_jinja_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 07:44:56.000000 trytoncalidae_jinja_report-6.8.0/trytoncalidae_jinja_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-19 07:44:56.000000 trytoncalidae_jinja_report-6.8.0/trytoncalidae_jinja_report.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 07:44:56.000000 trytoncalidae_jinja_report-6.8.0/trytoncalidae_jinja_report.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-19 07:44:56.000000 trytoncalidae_jinja_report-6.8.0/trytoncalidae_jinja_report.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 07:44:56.000000 trytoncalidae_jinja_report-6.8.0/trytoncalidae_jinja_report.egg-info/top_level.txt
```

### Comparing `trytoncalidae_jinja_report-6.6.0/LICENSE` & `trytoncalidae_jinja_report-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytoncalidae_jinja_report-6.6.0/PKG-INFO` & `trytoncalidae_jinja_report-6.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytoncalidae_jinja_report
-Version: 6.6.0
+Version: 6.8.0
 Summary: Create Tryton reports based on jinja2 python library
 Home-page: https://github.com/calidae/
 Download-URL: https://github.com/calidae/jinja_report
 Author: Calidae
 Author-email: dev@calidae.com
 License: GPL-3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `trytoncalidae_jinja_report-6.6.0/README.md` & `trytoncalidae_jinja_report-6.8.0/README.md`

 * *Files identical despite different names*

### Comparing `trytoncalidae_jinja_report-6.6.0/report.py` & `trytoncalidae_jinja_report-6.8.0/report.py`

 * *Files identical despite different names*

### Comparing `trytoncalidae_jinja_report-6.6.0/setup.py` & `trytoncalidae_jinja_report-6.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytoncalidae_jinja_report-6.6.0/tests/test_jinja_report.py` & `trytoncalidae_jinja_report-6.8.0/tests/test_jinja_report.py`

 * *Files identical despite different names*

### Comparing `trytoncalidae_jinja_report-6.6.0/trytoncalidae_jinja_report.egg-info/PKG-INFO` & `trytoncalidae_jinja_report-6.8.0/trytoncalidae_jinja_report.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytoncalidae-jinja-report
-Version: 6.6.0
+Version: 6.8.0
 Summary: Create Tryton reports based on jinja2 python library
 Home-page: https://github.com/calidae/
 Download-URL: https://github.com/calidae/jinja_report
 Author: Calidae
 Author-email: dev@calidae.com
 License: GPL-3
 Classifier: Development Status :: 5 - Production/Stable
```

