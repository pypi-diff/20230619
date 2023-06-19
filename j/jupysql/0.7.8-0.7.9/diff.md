# Comparing `tmp/jupysql-0.7.8.tar.gz` & `tmp/jupysql-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupysql-0.7.8.tar", last modified: Thu Jun  1 17:36:52 2023, max compression
+gzip compressed data, was "jupysql-0.7.9.tar", last modified: Mon Jun 19 15:52:22 2023, max compression
```

## Comparing `jupysql-0.7.8.tar` & `jupysql-0.7.9.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:52.236551 jupysql-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-06-01 17:36:31.000000 jupysql-0.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-01 17:36:31.000000 jupysql-0.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-01 17:36:52.236551 jupysql-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-01 17:36:31.000000 jupysql-0.7.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-01 17:36:31.000000 jupysql-0.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-01 17:36:52.236551 jupysql-0.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-01 17:36:31.000000 jupysql-0.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:52.228551 jupysql-0.7.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:52.232551 jupysql-0.7.8/src/jupysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-01 17:36:51.000000 jupysql-0.7.8/src/jupysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-01 17:36:51.000000 jupysql-0.7.8/src/jupysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:36:51.000000 jupysql-0.7.8/src/jupysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:36:51.000000 jupysql-0.7.8/src/jupysql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-01 17:36:51.000000 jupysql-0.7.8/src/jupysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-01 17:36:51.000000 jupysql-0.7.8/src/jupysql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:52.232551 jupysql-0.7.8/src/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/column_guesser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    21805 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/error_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:52.236551 jupysql-0.7.8/src/sql/ggplot/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/ggplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/ggplot/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/ggplot/facet_wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:52.236551 jupysql-0.7.8/src/sql/ggplot/geom/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/ggplot/geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/ggplot/geom/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/ggplot/geom/geom_boxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/ggplot/geom/geom_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/ggplot/ggplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/magic_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/magic_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    24145 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    18171 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/store.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:52.236551 jupysql-0.7.8/src/sql/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:52.236551 jupysql-0.7.8/src/sql/widgets/table_widget/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/widgets/table_widget/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:52.236551 jupysql-0.7.8/src/sql/widgets/table_widget/css/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/widgets/table_widget/css/tableWidget.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:52.236551 jupysql-0.7.8/src/sql/widgets/table_widget/js/
--rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/widgets/table_widget/js/tableWidget.js
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/widgets/table_widget/table_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/widgets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:22.880631 jupysql-0.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-06-19 15:52:03.000000 jupysql-0.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-19 15:52:03.000000 jupysql-0.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-19 15:52:22.880631 jupysql-0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-19 15:52:03.000000 jupysql-0.7.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-19 15:52:03.000000 jupysql-0.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-19 15:52:22.880631 jupysql-0.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-19 15:52:03.000000 jupysql-0.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:22.872631 jupysql-0.7.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:22.876631 jupysql-0.7.9/src/jupysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-19 15:52:22.000000 jupysql-0.7.9/src/jupysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-19 15:52:22.000000 jupysql-0.7.9/src/jupysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:52:22.000000 jupysql-0.7.9/src/jupysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:52:22.000000 jupysql-0.7.9/src/jupysql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-19 15:52:22.000000 jupysql-0.7.9/src/jupysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-19 15:52:22.000000 jupysql-0.7.9/src/jupysql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:22.876631 jupysql-0.7.9/src/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/column_guesser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22348 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/error_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:22.880631 jupysql-0.7.9/src/sql/ggplot/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/ggplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/ggplot/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/ggplot/facet_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:22.880631 jupysql-0.7.9/src/sql/ggplot/geom/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/ggplot/geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/ggplot/geom/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/ggplot/geom/geom_boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/ggplot/geom/geom_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/ggplot/ggplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20484 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/magic_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/magic_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25298 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/query_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/sqlcmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:22.880631 jupysql-0.7.9/src/sql/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:22.880631 jupysql-0.7.9/src/sql/widgets/table_widget/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/widgets/table_widget/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:22.880631 jupysql-0.7.9/src/sql/widgets/table_widget/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/widgets/table_widget/css/tableWidget.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:22.880631 jupysql-0.7.9/src/sql/widgets/table_widget/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    13553 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/widgets/table_widget/js/tableWidget.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/widgets/table_widget/table_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/widgets/utils.py
```

### Comparing `jupysql-0.7.8/LICENSE` & `jupysql-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.8/PKG-INFO` & `jupysql-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql
-Version: 0.7.8
+Version: 0.7.9
 Summary: Better SQL in Jupyter
 Home-page: https://github.com/ploomber/jupysql
 Author: Ploomber
 Author-email: contact@ploomber.io
 Project-URL: Source, https://github.com/ploomber/jupysql
 Keywords: database ipython postgresql mysql duckdb
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupysql Version: 0.7.8 Summary: Better SQL in
+Metadata-Version: 2.1 Name: jupysql Version: 0.7.9 Summary: Better SQL in
 Jupyter Home-page: https://github.com/ploomber/jupysql Author: Ploomber Author-
 email: contact@ploomber.io Project-URL: Source, https://github.com/ploomber/
 jupysql Keywords: database ipython postgresql mysql duckdb Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Topic ::
 Database Classifier: Topic :: Database :: Front-Ends Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `jupysql-0.7.8/README.md` & `jupysql-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.8/pyproject.toml` & `jupysql-0.7.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.8/setup.py` & `jupysql-0.7.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     "sqlparse",
     "ipython-genutils>=0.1.0",
     "sqlglot",
     "jinja2",
     "sqlglot>=11.3.7",
     "ploomber-core>=0.2.7",
     'importlib-metadata;python_version<"3.8"',
-    "psutil",
 ]
 
 DEV = [
     "flake8",
     "pytest",
     "pandas",
     "polars==0.17.2",  # 04/18/23 this breaks our CI
@@ -46,14 +45,15 @@
     # sql.plot module tests
     "matplotlib",
     "black",
     # for %%sql --interact
     "ipywidgets",
     # for running tests for %sqlcmd explore --table
     "js2py",
+    "jupysql-plugin",
 ]
 
 # dependencies for running integration tests
 INTEGRATION = [
     "dockerctx",
     "pyarrow",
     "psycopg2-binary",
```

### Comparing `jupysql-0.7.8/src/jupysql.egg-info/PKG-INFO` & `jupysql-0.7.9/src/jupysql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql
-Version: 0.7.8
+Version: 0.7.9
 Summary: Better SQL in Jupyter
 Home-page: https://github.com/ploomber/jupysql
 Author: Ploomber
 Author-email: contact@ploomber.io
 Project-URL: Source, https://github.com/ploomber/jupysql
 Keywords: database ipython postgresql mysql duckdb
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupysql Version: 0.7.8 Summary: Better SQL in
+Metadata-Version: 2.1 Name: jupysql Version: 0.7.9 Summary: Better SQL in
 Jupyter Home-page: https://github.com/ploomber/jupysql Author: Ploomber Author-
 email: contact@ploomber.io Project-URL: Source, https://github.com/ploomber/
 jupysql Keywords: database ipython postgresql mysql duckdb Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Topic ::
 Database Classifier: Topic :: Database :: Front-Ends Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `jupysql-0.7.8/src/jupysql.egg-info/SOURCES.txt` & `jupysql-0.7.9/src/jupysql.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 src/sql/exceptions.py
 src/sql/inspect.py
 src/sql/magic.py
 src/sql/magic_cmd.py
 src/sql/magic_plot.py
 src/sql/parse.py
 src/sql/plot.py
+src/sql/query_util.py
 src/sql/run.py
+src/sql/sqlcmd.py
 src/sql/store.py
 src/sql/telemetry.py
 src/sql/util.py
 src/sql/ggplot/__init__.py
 src/sql/ggplot/aes.py
 src/sql/ggplot/facet_wrap.py
 src/sql/ggplot/ggplot.py
```

### Comparing `jupysql-0.7.8/src/jupysql.egg-info/requires.txt` & `jupysql-0.7.9/src/jupysql.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 sqlalchemy
 sqlparse
 ipython-genutils>=0.1.0
 sqlglot
 jinja2
 sqlglot>=11.3.7
 ploomber-core>=0.2.7
-psutil
 
 [:python_version < "3.8"]
 importlib-metadata
 
 [:python_version <= "3.8"]
 ipython<=8.12.0
 
@@ -26,14 +25,15 @@
 duckdb<0.8.0
 duckdb-engine
 pyodbc
 matplotlib
 black
 ipywidgets
 js2py
+jupysql-plugin
 
 [integration]
 flake8
 pytest
 pandas
 polars==0.17.2
 invoke
@@ -42,14 +42,15 @@
 duckdb<0.8.0
 duckdb-engine
 pyodbc
 matplotlib
 black
 ipywidgets
 js2py
+jupysql-plugin
 dockerctx
 pyarrow
 psycopg2-binary
 pymysql
 pgspecial==2.0.1
 snowflake-sqlalchemy
 oracledb
```

### Comparing `jupysql-0.7.8/src/sql/_patch.py` & `jupysql-0.7.9/src/sql/_patch.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.8/src/sql/_testing.py` & `jupysql-0.7.9/src/sql/_testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         "root_password": "ploomber_app_root_password",
         "database": "db",
         "host": "localhost",
         "port": "33309",
         "alias": "mariaDBTest",
         "docker_ct": {
             "name": "mariadb",
-            "image": "mariadb",
+            "image": "mariadb:10.4.30",
             "ports": {3306: 33309},
         },
         "query": {},
     },
     "SQLite": {
         "drivername": "sqlite",
         "username": None,
@@ -377,15 +377,15 @@
             ready_test=lambda: database_ready(database="oracle"),
         ) as container:
             yield container
 
 
 def main():
     print("Starting test containers...")
-    with oracle():
+    with postgres(), mysql(), mariadb(), mssql(), oracle():
         print("Press CTRL+C to exit")
         try:
             while True:
                 time.sleep(5)
         except KeyboardInterrupt:
             print("Exit, containers will be killed")
             sys.exit()
```

### Comparing `jupysql-0.7.8/src/sql/column_guesser.py` & `jupysql-0.7.9/src/sql/column_guesser.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.8/src/sql/command.py` & `jupysql-0.7.9/src/sql/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,18 +67,14 @@
 
         if add_conn:
             self.parsed["connection"] = user_ns[self.args.line[0]]
 
         if add_alias:
             self.parsed["connection"] = self.args.line[0]
 
-        if self.args.with_:
-            final = store.render(self.parsed["sql"], with_=self.args.with_)
-            self.parsed["sql"] = str(final)
-
     @property
     def sql(self):
         """
         Returns the SQL query to execute, without any other options or arguments
         """
         return self.parsed["sql"]
 
@@ -108,7 +104,19 @@
         return Template(sql).render(user_ns)
 
     def __repr__(self) -> str:
         return (
             f"{type(self).__name__}(line={self._line!r}, cell={self._cell!r}) -> "
             f"({self.sql!r}, {self.sql_original!r})"
         )
+
+    def set_sql_with(self, with_):
+        """
+        Sets the final rendered SQL query using the WITH clause
+
+        Parameters
+        ----------
+        with_ : list
+        list of all subqueries needed to render the query
+        """
+        final = store.render(self.parsed["sql"], with_)
+        self.parsed["sql"] = str(final)
```

### Comparing `jupysql-0.7.8/src/sql/connection.py` & `jupysql-0.7.9/src/sql/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 from difflib import get_close_matches
+import atexit
 
 import sqlalchemy
 from sqlalchemy.engine import Engine
 from sqlalchemy.exc import NoSuchModuleError, OperationalError
 from IPython.core.error import UsageError
 import difflib
 import sqlglot
@@ -355,52 +356,57 @@
         Set the current database connection. This method is called from the magic to
         determine which connection to use (either use an existing one or open a new one)
         """
         connect_args = connect_args or {}
 
         if descriptor:
             is_custom_connection_ = Connection.is_custom_connection(descriptor)
-
             if isinstance(descriptor, Connection):
                 cls.current = descriptor
             elif isinstance(descriptor, Engine):
                 cls.current = Connection(descriptor, alias=alias)
             elif is_custom_connection_:
                 cls.current = CustomConnection(descriptor, alias=alias)
             else:
                 existing = rough_dict_get(cls.connections, descriptor)
-
                 # NOTE: I added one indentation level, otherwise
                 # the "existing" variable would not exist if
                 # passing an engine object as descriptor.
                 # Since I never saw this breaking, my guess
                 # is that we're missing some unit tests
                 # when descriptor is a connection object
                 # http://docs.sqlalchemy.org/en/rel_0_9/core/engines.html#custom-dbapi-connect-arguments # noqa
-                cls.current = existing or Connection.from_connect_str(
-                    connect_str=descriptor,
-                    connect_args=connect_args,
-                    creator=creator,
-                    alias=alias,
-                )
+                # if same alias found
+                if existing and existing.alias == alias:
+                    cls.current = existing
+                # if just switching connections
+                elif existing and alias is None:
+                    cls.current = existing
+                # if new alias connection
+                elif existing is None or existing.alias != alias:
+                    cls.current = Connection.from_connect_str(
+                        connect_str=descriptor,
+                        connect_args=connect_args,
+                        creator=creator,
+                        alias=alias,
+                    )
 
         else:
             if cls.connections:
                 if displaycon:
                     cls.display_current_connection()
             elif os.getenv("DATABASE_URL"):
                 cls.current = Connection.from_connect_str(
                     connect_str=os.getenv("DATABASE_URL"),
                     connect_args=connect_args,
                     creator=creator,
                     alias=alias,
                 )
             else:
                 raise cls._error_no_connection()
-
         return cls.current
 
     @classmethod
     def assign_name(cls, engine):
         name = "%s@%s" % (engine.url.username or "", engine.url.database)
         return name
 
@@ -472,20 +478,23 @@
         else:
             cls.connections.pop(
                 str(conn.metadata.bind.url) if IS_SQLALCHEMY_ONE else str(conn.url)
             )
             conn.session.close()
 
     @classmethod
-    def close_all(cls):
+    def close_all(cls, verbose=False):
         """Close all active connections"""
         connections = Connection.connections.copy()
         for key, conn in connections.items():
             conn.close(key)
 
+            if verbose:
+                print(f"Closing {key}")
+
         cls.connections = {}
 
     def is_custom_connection(conn=None) -> bool:
         """
         Checks if given connection is custom
         """
         is_custom_connection_ = False
@@ -641,14 +650,17 @@
         """
         Executes SQL query on a given connection
         """
         query = self._prepare_query(query, with_)
         return self.session.execute(query)
 
 
+atexit.register(Connection.close_all, verbose=True)
+
+
 class CustomSession(sqlalchemy.engine.base.Connection):
     """
     Custom sql alchemy session
     """
 
     def __init__(self, connection, engine):
         self.engine = engine
```

### Comparing `jupysql-0.7.8/src/sql/display.py` & `jupysql-0.7.9/src/sql/display.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.8/src/sql/error_message.py` & `jupysql-0.7.9/src/sql/error_message.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,41 @@
 import sqlglot
 import sqlparse
 
 SYNTAX_ERROR = "\nLooks like there is a syntax error in your query."
 ORIGINAL_ERROR = "\nOriginal error message from DB driver:\n"
 
 
+def parse_sqlglot_error(e, q):
+    """
+    Function to parse the error message from sqlglot
+
+    Parameters
+    ----------
+    e: sqlglot.errors.ParseError, exception
+            while parsing through sqlglot
+    q : str, user query
+
+    Returns
+    -------
+    str
+        Formatted error message containing description
+        and positions
+    """
+    err = e.errors
+    position = ""
+    for item in err:
+        position += (
+            f"Syntax Error in {q}: {item['description']} at "
+            f"Line {item['line']}, Column {item['col']}\n"
+        )
+    msg = "Possible reason: \n" + position if position else ""
+    return msg
+
+
 def detail(original_error, query=None):
     original_error = str(original_error)
     return_msg = SYNTAX_ERROR
     if "syntax error" in original_error:
         query_list = sqlparse.split(query)
         for q in query_list:
             try:
@@ -21,26 +48,16 @@
                 return_msg = (
                     return_msg + "Possible reason: \n" + suggestions
                     if suggestions
                     else return_msg
                 )
 
             except sqlglot.errors.ParseError as e:
-                err = e.errors
-                position = ""
-                for item in err:
-                    position += (
-                        f"Syntax Error in {q}: {item['description']} at "
-                        f"Line {item['line']}, Column {item['col']}\n"
-                    )
-                return_msg = (
-                    return_msg + "Possible reason: \n" + position
-                    if position
-                    else return_msg
-                )
+                parse_msg = parse_sqlglot_error(e, q)
+                return_msg = return_msg + parse_msg if parse_msg else return_msg
 
         return return_msg + "\n" + ORIGINAL_ERROR + original_error + "\n"
 
     if "fe_sendauth: no password supplied" in original_error:
         return (
             "\nLooks like you have run into some issues. "
             "Review our DB connection via URL strings guide: "
```

### Comparing `jupysql-0.7.8/src/sql/exceptions.py` & `jupysql-0.7.9/src/sql/exceptions.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.8/src/sql/ggplot/facet_wrap.py` & `jupysql-0.7.9/src/sql/ggplot/facet_wrap.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,18 @@
             """
         )
         query = template.render(table=table, column=column)
 
         conn = sql.connection.Connection.current
 
         values = conn.execute(query, with_).fetchall()
+        # Added to make histogram more inclusive to NULLs
+        # Filter out NULL values
+        # If value[0] is NULL we skip it
+        values = [value for value in values if value[0] is not None]
         n_plots = len(values)
         n_cols = len(values) if len(values) < 3 else 3
         n_rows = math.ceil(n_plots / n_cols)
         return values, n_rows, n_cols
 
 
 class facet_wrap(facet):
```

### Comparing `jupysql-0.7.8/src/sql/ggplot/geom/geom_histogram.py` & `jupysql-0.7.9/src/sql/ggplot/geom/geom_histogram.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.8/src/sql/ggplot/ggplot.py` & `jupysql-0.7.9/src/sql/ggplot/ggplot.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.8/src/sql/inspect.py` & `jupysql-0.7.9/src/sql/inspect.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.8/src/sql/magic.py` & `jupysql-0.7.9/src/sql/magic.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,29 +14,35 @@
     needs_local_scope,
     no_var_expand,
 )
 from IPython.core.magic_arguments import argument, magic_arguments, parse_argstring
 from sqlalchemy.exc import OperationalError, ProgrammingError, DatabaseError
 
 import warnings
+import shlex
+from difflib import get_close_matches
 import sql.connection
 import sql.parse
 import sql.run
+from sql.parse import _option_strings_from_parser
 from sql import display, exceptions
 from sql.store import store
 from sql.command import SQLCommand
 from sql.magic_plot import SqlPlotMagic
 from sql.magic_cmd import SqlCmdMagic
 from sql._patch import patch_ipython_usage_error
+from sql import query_util
+from sql.util import get_suggestions_message, show_deprecation_warning
 from ploomber_core.dependencies import check_installed
 
 from sql.error_message import detail
 from traitlets.config.configurable import Configurable
 from traitlets import Bool, Int, TraitError, Unicode, Dict, observe, validate
 
+
 try:
     from pandas.core.frame import DataFrame, Series
 except ModuleNotFoundError:
     DataFrame = None
     Series = None
 
 from sql.telemetry import telemetry
@@ -83,15 +89,16 @@
         help="Automatically limit the size of the returned result sets",
     )
     style = Unicode(
         "DEFAULT",
         config=True,
         help=(
             "Set the table printing style to any of prettytable's "
-            "defined styles (currently DEFAULT, MSWORD_FRIENDLY, PLAIN_COLUMNS, RANDOM)"
+            "defined styles (currently DEFAULT, MSWORD_FRIENDLY, PLAIN_COLUMNS, "
+            "RANDOM, SINGLE_BORDER, DOUBLE_BORDER, MARKDOWN )"
         ),
     )
     short_errors = Bool(
         True,
         config=True,
         help="Don't display the full traceback on SQL Programming Error",
     )
@@ -172,14 +179,38 @@
         # other one in case it was enabled and print a warning
         if change["new"]:
             other = "autopolars" if change["name"] == "autopandas" else "autopandas"
             if getattr(self, other):
                 setattr(self, other, False)
                 print(f"Disabled '{other}' since '{change['name']}' was enabled.")
 
+    def check_random_arguments(self, line="", cell=""):
+        # check only for cell magic
+        if cell != "":
+            tokens = shlex.split(line, posix=False)
+            arguments = []
+
+            # Iterate through the tokens to separate arguments and SQL code
+            # If the token starts with "--", it is an argument
+            breakLoop = False
+            for token in tokens:
+                if token.startswith("--") or token.startswith("-"):
+                    arguments.append(token)
+                    breakLoop = True
+                else:
+                    if breakLoop:
+                        break
+
+            declared_argument = _option_strings_from_parser(SqlMagic.execute.parser)
+            for check_argument in arguments:
+                if check_argument not in declared_argument:
+                    raise exceptions.UsageError(
+                        "Unrecognized argument(s): {}".format(check_argument)
+                    )
+
     @no_var_expand
     @needs_local_scope
     @line_magic("sql")
     @cell_magic("sql")
     @line_magic("jupysql")
     @cell_magic("jupysql")
     @magic_arguments()
@@ -307,26 +338,36 @@
         # Examples
 
         # %sql {line}
         # note that line magic has no body
 
         # %%sql {line}
         # {cell}
+
+        self.check_random_arguments(line, cell)
+
         if local_ns is None:
             local_ns = {}
 
         # save globals and locals so they can be referenced in bind vars
         user_ns = self.shell.user_ns.copy()
         user_ns.update(local_ns)
 
         command = SQLCommand(self, user_ns, line, cell)
         # args.line: contains the line after the magic with all options removed
 
         args = command.args
 
+        with_ = self._store.infer_dependencies(command.sql_original, args.save)
+        if with_:
+            command.set_sql_with(with_)
+            print(f"Generating CTE with stored snippets : {', '.join(with_)}")
+        else:
+            with_ = None
+
         # Create the interactive slider
         if args.interact and not is_interactive_mode:
             check_installed(["ipywidgets"], "--interactive argument")
             interactive_dict = {}
             for key in args.interact:
                 interactive_dict[key] = local_ns[key]
             print(
@@ -406,25 +447,27 @@
         if args.append:
             return self._persist_dataframe(
                 command.sql, conn, user_ns, append=True, index=not args.no_index
             )
 
         if not command.sql:
             return
+        if args.with_:
+            show_deprecation_warning()
         # store the query if needed
         if args.save:
             if "-" in args.save:
                 warnings.warn(
                     "Using hyphens will be deprecated soon, "
                     "please use "
                     + str(args.save.replace("-", "_"))
                     + " instead for the save argument.",
                     FutureWarning,
                 )
-            self._store.store(args.save, command.sql_original, with_=args.with_)
+            self._store.store(args.save, command.sql_original, with_=with_)
 
         if args.no_execute:
             display.message("Skipping execution...")
             return
 
         try:
             result = sql.run.run(conn, command.sql, self)
@@ -465,14 +508,27 @@
         except (ProgrammingError, OperationalError, DatabaseError) as e:
             # Sqlite apparently return all errors as OperationalError :/
             detailed_msg = detail(e, command.sql)
             if self.short_errors:
                 if detailed_msg is not None:
                     err = exceptions.UsageError(detailed_msg)
                     raise err
+                    # TODO: move to error_messages.py
+                    # Added here due to circular dependency issue (#545)
+                elif "no such table" in str(e):
+                    tables = query_util.extract_tables_from_query(command.sql)
+                    for table in tables:
+                        suggestions = get_close_matches(table, list(self._store))
+                        if len(suggestions) > 0:
+                            err_message = f"There is no table with name {table!r}."
+                            suggestions_message = get_suggestions_message(suggestions)
+                            raise exceptions.TableNotFoundError(
+                                f"{err_message}{suggestions_message}"
+                            )
+                    print(e)
                 else:
                     print(e)
             else:
                 if detailed_msg is not None:
                     print(detailed_msg)
                 e.modify_exception = True
                 raise e
```

### Comparing `jupysql-0.7.8/src/sql/magic_cmd.py` & `jupysql-0.7.9/src/sql/magic_cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,18 @@
         if message:
             self._print_message(message, sys.stderr)
 
     def error(self, message):
         raise exceptions.UsageError(message)
 
 
+# Added here due to circular dependencies (#545)
+from sql.sqlcmd import sqlcmd_snippets  # noqa
+
+
 @magics_class
 class SqlCmdMagic(Magics, Configurable):
     """%sqlcmd magic"""
 
     @line_magic("sqlcmd")
     @magic_arguments()
     @argument("line", type=str, help="Command name")
@@ -46,21 +50,30 @@
         Function to validate %sqlcmd inputs.
         Raises UsageError in case of an invalid input, executes command otherwise.
         """
 
         # We rely on SQLAlchemy when inspecting tables
         util.support_only_sql_alchemy_connection("%sqlcmd")
 
-        AVAILABLE_SQLCMD_COMMANDS = ["tables", "columns", "test", "profile", "explore"]
+        AVAILABLE_SQLCMD_COMMANDS = [
+            "tables",
+            "columns",
+            "test",
+            "profile",
+            "explore",
+            "snippets",
+        ]
+
+        VALID_COMMANDS_MSG = (
+            f"Missing argument for %sqlcmd. "
+            f"Valid commands are: {', '.join(AVAILABLE_SQLCMD_COMMANDS)}"
+        )
 
         if line == "":
-            raise exceptions.UsageError(
-                "Missing argument for %sqlcmd. "
-                "Valid commands are: {}".format(", ".join(AVAILABLE_SQLCMD_COMMANDS))
-            )
+            raise exceptions.UsageError(VALID_COMMANDS_MSG)
         else:
             split = arg_split(line)
             command, others = split[0].strip(), split[1:]
 
             if command in AVAILABLE_SQLCMD_COMMANDS:
                 return self.execute(command, others)
             else:
@@ -219,14 +232,17 @@
                 "-t", "--table", type=str, help="Table name", required=True
             )
             args = parser.parse_args(others)
 
             table_widget = TableWidget(args.table)
             display(table_widget)
 
+        elif cmd_name == "snippets":
+            return sqlcmd_snippets(others)
+
 
 def return_test_results(args, conn, query):
     try:
         columns = []
         column_data = conn.execute(text(query)).cursor.description
         res = conn.execute(text(query)).fetchall()
         for column in column_data:
```

### Comparing `jupysql-0.7.8/src/sql/magic_plot.py` & `jupysql-0.7.9/src/sql/magic_plot.py`

 * *Files 13% similar despite different names*

```diff
@@ -79,52 +79,61 @@
                 f"{plot_str}\n"
                 "Example: %sqlplot histogram"
             )
 
         column = util.sanitize_identifier(column)
         table = util.sanitize_identifier(cmd.args.table)
 
+        if cmd.args.with_:
+            util.show_deprecation_warning()
         if cmd.args.line[0] in {"box", "boxplot"}:
-            util.is_table_exists(table, with_=cmd.args.with_)
+            with_ = self._check_table_exists(table)
+
             return plot.boxplot(
                 table=table,
                 column=column,
-                with_=cmd.args.with_,
+                with_=with_,
                 orient=cmd.args.orient,
                 conn=None,
             )
         elif cmd.args.line[0] in {"hist", "histogram"}:
-            util.is_table_exists(table, with_=cmd.args.with_)
-
+            with_ = self._check_table_exists(table)
             return plot.histogram(
                 table=table,
                 column=column,
                 bins=cmd.args.bins,
-                with_=cmd.args.with_,
+                with_=with_,
                 conn=None,
             )
         elif cmd.args.line[0] in {"bar"}:
-            util.is_table_exists(table, with_=cmd.args.with_)
-
+            with_ = self._check_table_exists(table)
             return plot.bar(
                 table=table,
                 column=column,
-                with_=cmd.args.with_,
+                with_=with_,
                 orient=cmd.args.orient,
                 show_num=cmd.args.show_numbers,
                 conn=None,
             )
         elif cmd.args.line[0] in {"pie"}:
-            util.is_table_exists(table, with_=cmd.args.with_)
-
+            with_ = self._check_table_exists(table)
             return plot.pie(
                 table=table,
                 column=column,
-                with_=cmd.args.with_,
+                with_=with_,
                 show_num=cmd.args.show_numbers,
                 conn=None,
             )
         else:
             plot_str = util.pretty_print(SUPPORTED_PLOTS, last_delimiter="or")
             raise exceptions.UsageError(
                 f"Unknown plot {cmd.args.line[0]!r}. Must be any of: " f"{plot_str}"
             )
+
+    @staticmethod
+    def _check_table_exists(table):
+        with_ = None
+        if util.is_saved_snippet(table):
+            with_ = [table]
+        else:
+            util.is_table_exists(table)
+        return with_
```

### Comparing `jupysql-0.7.8/src/sql/parse.py` & `jupysql-0.7.9/src/sql/parse.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.8/src/sql/plot.py` & `jupysql-0.7.9/src/sql/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -357,15 +357,17 @@
 
     Notes
     -----
     .. versionchanged:: 0.5.2
         Added plot title and axis labels. Allowing to pass lists in ``column``.
         Function returns a ``matplotlib.Axes`` object.
 
-    .. versionadded:: 0.4.4
+    .. versionchanged:: 0.7.9
+        Added support for NULL values, additional filter query with new logic.
+        Skips the rows with NULL in the column, does not raise ValueError
 
     Returns
     -------
     ax : matplotlib.Axes
         Generated plot
 
     Examples
@@ -497,15 +499,20 @@
     if not conn:
         conn = sql.connection.Connection.current
     use_backticks = conn.is_use_backtick_template()
 
     # FIXME: we're computing all the with elements twice
     min_, max_ = _min_max(conn, table, column, with_=with_, use_backticks=use_backticks)
 
-    filter_query = f"WHERE {facet['key']} == '{facet['value']}'" if facet else ""
+    # Define all relevant filters here
+    filter_query_1 = f'"{column}" IS NOT NULL'
+
+    filter_query_2 = f"{facet['key']} == '{facet['value']}'" if facet else None
+
+    filter_query = _filter_aggregate(filter_query_1, filter_query_2)
 
     bin_size = None
 
     if _are_numeric_values(min_, max_):
         if not isinstance(bins, int):
             raise ValueError(
                 f"bins are '{bins}'. Please specify a valid number of bins."
@@ -549,17 +556,14 @@
 
         query = template.render(table=table, column=column, filter_query=filter_query)
 
     data = conn.execute(query, with_).fetchall()
 
     bin_, height = zip(*data)
 
-    if bin_[0] is None:
-        raise ValueError("Data contains NULLs")
-
     return bin_, height, bin_size
 
 
 @modify_exceptions
 def _histogram_stacked(
     table,
     column,
@@ -578,15 +582,19 @@
     for bin in bins:
         case = f'SUM(CASE WHEN FLOOR({column}/{bin_size})*{bin_size} = {bin} \
                  THEN 1 ELSE 0 END) AS "{bin}",'
         cases.append(case)
 
     cases = " ".join(cases)
 
-    filter_query = f"WHERE {facet['key']} == '{facet['value']}'" if facet else ""
+    filter_query_1 = f'"{column}" IS NOT NULL'
+
+    filter_query_2 = f"{facet['key']} == '{facet['value']}'" if facet else None
+
+    filter_query = _filter_aggregate(filter_query_1, filter_query_2)
 
     template = Template(
         """
         SELECT {{category}},
         {{cases}}
         FROM "{{table}}"
         {{filter_query}}
@@ -604,14 +612,46 @@
 
     data = conn.execute(query, with_).fetchall()
 
     return data
 
 
 @modify_exceptions
+def _filter_aggregate(*filter_queries):
+    """Return a single filter query based on multiple queries.
+
+    Parameters:
+    ----------
+    *filter_queries (str):
+    Variable length argument list of filter queries.
+    Filter query is  string with a filtering condition in SQL
+    (e.g., "age > 25").
+    (e.g., "column is NULL").
+
+    Notes
+    -----
+    .. versionadded:: 0.7.9
+
+    Returns:
+    -----
+    final_filter (str):
+    A string that represents a SQL WHERE clause
+
+    """
+    final_filter = ""
+    for idx, query in enumerate(filter_queries):
+        if query is not None:
+            if idx == 0:
+                final_filter = f"{final_filter}WHERE {query}"
+                continue
+            final_filter = f"{final_filter} AND {query}"
+    return final_filter
+
+
+@modify_exceptions
 def _bar(table, column, with_=None, conn=None):
     """get x and height for bar plot"""
     if not conn:
         conn = sql.connection.Connection.current
     use_backticks = conn.is_use_backtick_template()
 
     if isinstance(column, list):
```

### Comparing `jupysql-0.7.8/src/sql/run.py` & `jupysql-0.7.9/src/sql/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,14 @@
     Can access rows listwise, or by string value of leftmost column.
     """
 
     def __init__(self, sqlaproxy, config):
         self.config = config
         self.keys = {}
         self._results = []
-
         # https://peps.python.org/pep-0249/#description
         is_dbapi_results = hasattr(sqlaproxy, "description")
 
         self.pretty = None
 
         if is_dbapi_results:
             should_try_fetch_results = True
@@ -139,18 +138,19 @@
                 else:
                     self._results = sqlaproxy.fetchall()
 
                 self.field_names = unduplicate_field_names(self.keys)
 
                 _style = None
 
+                self.pretty = PrettyTable(self.field_names)
+
                 if isinstance(config.style, str):
                     _style = prettytable.__dict__[config.style.upper()]
-
-                self.pretty = PrettyTable(self.field_names, style=_style)
+                    self.pretty.set_style(_style)
 
     def _repr_html_(self):
         _cell_with_spaces_pattern = re.compile(r"(<td>)( {2,})")
         if self.pretty:
             self.pretty.add_rows(self)
             result = self.pretty.get_html_string()
             # to create clickable links
```

### Comparing `jupysql-0.7.8/src/sql/store.py` & `jupysql-0.7.9/src/sql/store.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from collections.abc import MutableMapping
 from jinja2 import Template
 from ploomber_core.exceptions import modify_exceptions
 import sql.connection
 import difflib
 
 from sql import exceptions
+from sql import query_util
 
 
 class SQLStore(MutableMapping):
     """Stores SQL scripts to render large queries with CTEs
 
     Notes
     -----
@@ -64,14 +65,26 @@
     def __delitem__(self, key: str) -> None:
         del self._data[key]
 
     def render(self, query, with_=None):
         # TODO: if with is false, WITH should not appear
         return SQLQuery(self, query, with_)
 
+    def infer_dependencies(self, query, key):
+        dependencies = []
+        saved_keys = [
+            saved_key for saved_key in list(self._data.keys()) if saved_key != key
+        ]
+        if saved_keys and query:
+            tables = query_util.extract_tables_from_query(query)
+            for table in tables:
+                if table in saved_keys:
+                    dependencies.append(table)
+        return dependencies
+
     @modify_exceptions
     def store(self, key, query, with_=None):
         if "-" in key:
             raise exceptions.UsageError(
                 "Using hyphens (-) in save argument isn't allowed."
                 " Please use underscores (_) instead"
             )
@@ -134,14 +147,23 @@
     """Get a list of all dependencies to reconstruct the CTEs in keys"""
     # get the dependencies for each key
     deps = _flatten([_get_dependencies_for_key(store, key) for key in keys])
     # remove duplicates but preserve order
     return list(dict.fromkeys(deps + keys))
 
 
+def _get_dependents_for_key(store, key):
+    key_dependents = []
+    for k in list(store):
+        deps = _get_dependencies_for_key(store, k)
+        if key in deps:
+            key_dependents.append(k)
+    return key_dependents
+
+
 def _get_dependencies_for_key(store, key):
     """Retrieve dependencies for a single key"""
     deps = store[key]._with_
     deps_of_deps = _flatten([_get_dependencies_for_key(store, dep) for dep in deps])
     return deps_of_deps + deps
```

### Comparing `jupysql-0.7.8/src/sql/util.py` & `jupysql-0.7.9/src/sql/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import warnings
 import sql
 from sql import inspect
 import difflib
 from sql.connection import Connection
-from sql.store import store
+from sql.store import store, _get_dependents_for_key
 from sql import exceptions
 import json
 
 SINGLE_QUOTE = "'"
 DOUBLE_QUOTE = '"'
 
 
@@ -48,35 +49,39 @@
     if "." in str(num):
         split_by_decimal = str(num).split(".")
         if len(split_by_decimal[0]) > 10 or len(split_by_decimal[1]) > 10:
             return True
     return False
 
 
+def get_suggestions_message(suggestions):
+    suggestions_message = ""
+    if len(suggestions) > 0:
+        _suggestions_string = pretty_print(suggestions, last_delimiter="or")
+        suggestions_message = f"\nDid you mean : {_suggestions_string}"
+    return suggestions_message
+
+
 def is_table_exists(
     table: str,
     schema: str = None,
     ignore_error: bool = False,
-    with_: str = None,
     conn=None,
 ) -> bool:
     """
     Checks if a given table exists for a given connection
 
     Parameters
     ----------
     table: str
         Table name
 
     schema: str, default None
         Schema name
 
-    with_: list, default None
-        Temporary table
-
     ignore_error: bool, default False
         Avoid raising a ValueError
     """
     if table is None:
         if ignore_error:
             return False
         else:
@@ -89,15 +94,15 @@
     table = strip_multiple_chars(table, "\"'")
 
     if schema:
         table_ = f"{schema}.{table}"
     else:
         table_ = table
 
-    _is_exist = _is_table_exists(table_, with_, conn)
+    _is_exist = _is_table_exists(table_, conn)
 
     if not _is_exist:
         if not ignore_error:
             try_find_suggestions = not Connection.is_custom_connection(conn)
             expected = []
             existing_schemas = []
             existing_tables = []
@@ -120,30 +125,20 @@
                     f"There is no table with name {table!r} in schema {schema!r}"
                 )
             else:
                 err_message = (
                     f"There is no table with name {table!r} in the default schema"
                 )
 
-            if table in list(store):
-                # Suggest user use --with when given table
-                # is in the store
-                suggestion_message = (
-                    ", but there is a stored query."
-                    f"\nDid you miss passing --with {table}?"
-                )
-                err_message = f"{err_message}{suggestion_message}"
-            else:
-                suggestions = difflib.get_close_matches(invalid_input, expected)
-
-                if len(suggestions) > 0:
-                    _suggestions_string = pretty_print(suggestions, last_delimiter="or")
-                    suggestions_message = f"\nDid you mean : {_suggestions_string}"
-                    err_message = f"{err_message}{suggestions_message}"
-
+            suggestions = difflib.get_close_matches(invalid_input, expected)
+            suggestions_store = difflib.get_close_matches(invalid_input, list(store))
+            suggestions.extend(suggestions_store)
+            suggestions_message = get_suggestions_message(suggestions)
+            if suggestions_message:
+                err_message = f"{err_message}{suggestions_message}"
             raise exceptions.TableNotFoundError(err_message)
 
     return _is_exist
 
 
 def _get_list_of_existing_tables() -> list:
     """
@@ -178,38 +173,40 @@
 def strip_multiple_chars(string: str, chars: str) -> str:
     """
     Trims characters from the start and end of the string
     """
     return string.translate(str.maketrans("", "", chars))
 
 
-def _is_table_exists(table: str, with_: str, conn) -> bool:
+def is_saved_snippet(table: str) -> bool:
+    if table in list(store):
+        print(f"Plotting using saved snippet : {table}")
+        return True
+    return False
+
+
+def _is_table_exists(table: str, conn) -> bool:
     """
     Runs a SQL query to check if table exists
     """
     if not conn:
         conn = Connection.current
 
     identifiers = conn.get_curr_identifiers()
 
-    if with_:
-        return table in list(store)
-    else:
-        for iden in identifiers:
-            if isinstance(iden, tuple):
-                query = "SELECT * FROM {0}{1}{2} WHERE 1=0".format(
-                    iden[0], table, iden[1]
-                )
-            else:
-                query = "SELECT * FROM {0}{1}{0} WHERE 1=0".format(iden, table)
-            try:
-                conn.execute(query)
-                return True
-            except Exception:
-                pass
+    for iden in identifiers:
+        if isinstance(iden, tuple):
+            query = "SELECT * FROM {0}{1}{2} WHERE 1=0".format(iden[0], table, iden[1])
+        else:
+            query = "SELECT * FROM {0}{1}{0} WHERE 1=0".format(iden, table)
+        try:
+            conn.execute(query)
+            return True
+        except Exception:
+            pass
 
     return False
 
 
 def flatten(src, ltypes=(list, tuple)):
     """The flatten function creates a new tuple / list
     with all sub-tuple / sub-list elements concatenated into it recursively
@@ -301,7 +298,65 @@
     """
     dicts = [dict(zip(list(columns), row)) for row in rows]
     rows_json = json.dumps(dicts, indent=4, sort_keys=True, default=str).replace(
         "null", '"None"'
     )
 
     return rows_json
+
+
+def get_all_keys():
+    """
+
+    Returns
+    -------
+    All stored snippets in the current session
+    """
+    return list(store)
+
+
+def get_key_dependents(key: str) -> list:
+    """
+    Function to find the stored snippets dependent on key
+    Parameters
+    ----------
+    key : str, name of the table
+
+    Returns
+    -------
+    list
+        List of snippets dependent on key
+
+    """
+    deps = _get_dependents_for_key(store, key)
+    return deps
+
+
+def del_saved_key(key: str) -> str:
+    """
+    Deletes a stored snippet
+    Parameters
+    ----------
+    key : str, name of the snippet to be deleted
+
+    Returns
+    -------
+    list
+        Remaining stored snippets
+    """
+    all_keys = get_all_keys()
+    if key not in all_keys:
+        raise exceptions.UsageError(f"No such saved snippet found : {key}")
+    del store[key]
+    return get_all_keys()
+
+
+def show_deprecation_warning():
+    """
+    Raises CTE deprecation warning
+    """
+    warnings.warn(
+        "CTE dependencies are now automatically inferred, "
+        "you can omit the --with arguments. Using --with will "
+        "raise an exception in the next major release so please remove it.",
+        FutureWarning,
+    )
```

### Comparing `jupysql-0.7.8/src/sql/widgets/table_widget/js/tableWidget.js` & `jupysql-0.7.9/src/sql/widgets/table_widget/js/tableWidget.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -398,15 +398,15 @@
         </thead>
 
         <tbody>
         </tbody>
     </table>
 
 
-    <div>
+    <div style="padding-bottom: 20px;">
         <button onclick="prevPageClick(this)">Previous</button>
         <div
             id = "pagesButtons"
             class = "pages-buttons"
             style = "display: inline-flex">
         </div>
         <button onclick="nextPageClick(this)">Next</button>
```

### Comparing `jupysql-0.7.8/src/sql/widgets/table_widget/table_widget.py` & `jupysql-0.7.9/src/sql/widgets/table_widget/table_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,18 +151,17 @@
         )
 
     def register_comm(self):
         """
         Register communication between the frontend and the kernel.
         """
 
-        if utils.is_jupyterlab_session():
-            check_installed(
-                ["jupysql_plugin"], "jupysql-plugin", pip_names=["jupysql-plugin"]
-            )
+        check_installed(
+            ["jupysql_plugin"], "jupysql-plugin", pip_names=["jupysql-plugin"]
+        )
 
         def comm_handler(comm, open_msg):
             """
             Handle received messages from the frontend
             """
 
             @comm.on_msg
```

