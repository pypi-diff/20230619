# Comparing `tmp/openai-pygenerator-0.4.3.tar.gz` & `tmp/openai-pygenerator-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-pygenerator-0.4.3.tar", last modified: Mon Jun 19 16:39:10 2023, max compression
+gzip compressed data, was "openai-pygenerator-0.4.4.tar", last modified: Mon Jun 19 20:29:48 2023, max compression
```

## Comparing `openai-pygenerator-0.4.3.tar` & `openai-pygenerator-0.4.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:39:10.495666 openai-pygenerator-0.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:39:10.491666 openai-pygenerator-0.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:39:10.491666 openai-pygenerator-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-19 16:39:10.495666 openai-pygenerator-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/mypy-tests.ini
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-19 16:39:10.495666 openai-pygenerator-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:39:10.491666 openai-pygenerator-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:39:10.495666 openai-pygenerator-0.4.3/src/openai_pygenerator/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/src/openai_pygenerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/src/openai_pygenerator/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/src/openai_pygenerator/openai_pygenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:39:10.495666 openai-pygenerator-0.4.3/src/openai_pygenerator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-19 16:39:10.000000 openai-pygenerator-0.4.3/src/openai_pygenerator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-19 16:39:10.000000 openai-pygenerator-0.4.3/src/openai_pygenerator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:39:10.000000 openai-pygenerator-0.4.3/src/openai_pygenerator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-19 16:39:10.000000 openai-pygenerator-0.4.3/src/openai_pygenerator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 16:39:10.000000 openai-pygenerator-0.4.3/src/openai_pygenerator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 16:39:10.000000 openai-pygenerator-0.4.3/src/openai_pygenerator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:39:10.495666 openai-pygenerator-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/tests/test_gpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:29:48.847030 openai-pygenerator-0.4.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:29:48.843029 openai-pygenerator-0.4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:29:48.843029 openai-pygenerator-0.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-19 20:29:48.847030 openai-pygenerator-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/mypy-tests.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-19 20:29:48.847030 openai-pygenerator-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:29:48.843029 openai-pygenerator-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:29:48.847030 openai-pygenerator-0.4.4/src/openai_pygenerator/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/src/openai_pygenerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/src/openai_pygenerator/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/src/openai_pygenerator/openai_pygenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:29:48.847030 openai-pygenerator-0.4.4/src/openai_pygenerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-19 20:29:48.000000 openai-pygenerator-0.4.4/src/openai_pygenerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-19 20:29:48.000000 openai-pygenerator-0.4.4/src/openai_pygenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:29:48.000000 openai-pygenerator-0.4.4/src/openai_pygenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-19 20:29:48.000000 openai-pygenerator-0.4.4/src/openai_pygenerator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 20:29:48.000000 openai-pygenerator-0.4.4/src/openai_pygenerator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 20:29:48.000000 openai-pygenerator-0.4.4/src/openai_pygenerator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:29:48.847030 openai-pygenerator-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/tests/test_gpt.py
```

### Comparing `openai-pygenerator-0.4.3/.github/workflows/python-package.yml` & `openai-pygenerator-0.4.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.3/.github/workflows/python-publish.yml` & `openai-pygenerator-0.4.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.3/.pre-commit-config.yaml` & `openai-pygenerator-0.4.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.3/.pylintrc` & `openai-pygenerator-0.4.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.3/LICENSE.txt` & `openai-pygenerator-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.3/PKG-INFO` & `openai-pygenerator-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-pygenerator
-Version: 0.4.3
+Version: 0.4.4
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai-pygenerator-0.4.3/README.md` & `openai-pygenerator-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.3/pyproject.toml` & `openai-pygenerator-0.4.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools.package-data]
+"*" = ["py.typed"]
+
 [tool.setuptools_scm]
 write_to = "src/version.py"
 
 [tool.pytest.ini_options]
 pythonpath = "src"
 
 [project]
```

### Comparing `openai-pygenerator-0.4.3/src/openai_pygenerator/example.py` & `openai-pygenerator-0.4.4/src/openai_pygenerator/example.py`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.3/src/openai_pygenerator/openai_pygenerator.py` & `openai-pygenerator-0.4.4/src/openai_pygenerator/openai_pygenerator.py`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.3/src/openai_pygenerator.egg-info/PKG-INFO` & `openai-pygenerator-0.4.4/src/openai_pygenerator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-pygenerator
-Version: 0.4.3
+Version: 0.4.4
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai-pygenerator-0.4.3/src/openai_pygenerator.egg-info/SOURCES.txt` & `openai-pygenerator-0.4.4/src/openai_pygenerator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.3/tests/test_gpt.py` & `openai-pygenerator-0.4.4/tests/test_gpt.py`

 * *Files identical despite different names*

