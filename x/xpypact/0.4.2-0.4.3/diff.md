# Comparing `tmp/xpypact-0.4.2.tar.gz` & `tmp/xpypact-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpypact-0.4.2.tar", max compression
+gzip compressed data, was "xpypact-0.4.3.tar", max compression
```

## Comparing `xpypact-0.4.2.tar` & `xpypact-0.4.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1063 2023-06-06 15:30:37.781278 xpypact-0.4.2/LICENSE
--rw-r--r--   0        0        0     3296 2023-06-06 15:30:37.781278 xpypact-0.4.2/README.rst
--rw-r--r--   0        0        0    17279 2023-06-06 15:30:56.133574 xpypact-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1199 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/__init__.py
--rw-r--r--   0        0        0      174 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/dao/__init__.py
--rw-r--r--   0        0        0     2241 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/dao/api.py
--rw-r--r--   0        0        0      234 2023-06-06 15:30:56.133574 xpypact-0.4.2/src/xpypact/dao/duckdb/__init__.py
--rw-r--r--   0        0        0     2870 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/dao/duckdb/create_schema.sql
--rw-r--r--   0        0        0     9057 2023-06-06 15:30:56.133574 xpypact-0.4.2/src/xpypact/dao/duckdb/implementation.py
--rw-r--r--   0        0        0    14156 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/data_arrays.py
--rw-r--r--   0        0        0     5307 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/data_frames.py
--rw-r--r--   0        0        0    12337 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/fluxes.py
--rw-r--r--   0        0        0     5862 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/inventory.py
--rw-r--r--   0        0        0     1965 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/nuclide.py
--rw-r--r--   0        0        0        0 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/py.typed
--rw-r--r--   0        0        0      515 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/run_data.py
--rw-r--r--   0        0        0     4924 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/time_step.py
--rw-r--r--   0        0        0       29 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/utils/__init__.py
--rw-r--r--   0        0        0      809 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/utils/io.py
--rw-r--r--   0        0        0        0 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/utils/py.typed
--rw-r--r--   0        0        0      768 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/utils/resource.py
--rw-r--r--   0        0        0      270 2023-06-06 15:30:37.785277 xpypact-0.4.2/src/xpypact/utils/types.py
--rw-r--r--   0        0        0     4789 1970-01-01 00:00:00.000000 xpypact-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-19 11:35:28.979937 xpypact-0.4.3/LICENSE
+-rw-r--r--   0        0        0     3296 2023-06-19 11:35:28.979937 xpypact-0.4.3/README.rst
+-rw-r--r--   0        0        0    17232 2023-06-19 11:35:44.148120 xpypact-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1199 2023-06-19 11:35:28.987937 xpypact-0.4.3/src/xpypact/__init__.py
+-rw-r--r--   0        0        0      174 2023-06-19 11:35:28.987937 xpypact-0.4.3/src/xpypact/dao/__init__.py
+-rw-r--r--   0        0        0     2241 2023-06-19 11:35:28.987937 xpypact-0.4.3/src/xpypact/dao/api.py
+-rw-r--r--   0        0        0      234 2023-06-19 11:35:28.987937 xpypact-0.4.3/src/xpypact/dao/duckdb/__init__.py
+-rw-r--r--   0        0        0     2870 2023-06-19 11:35:28.987937 xpypact-0.4.3/src/xpypact/dao/duckdb/create_schema.sql
+-rw-r--r--   0        0        0     9057 2023-06-19 11:35:28.987937 xpypact-0.4.3/src/xpypact/dao/duckdb/implementation.py
+-rw-r--r--   0        0        0    14156 2023-06-19 11:35:28.987937 xpypact-0.4.3/src/xpypact/data_arrays.py
+-rw-r--r--   0        0        0     5307 2023-06-19 11:35:28.987937 xpypact-0.4.3/src/xpypact/data_frames.py
+-rw-r--r--   0        0        0    12337 2023-06-19 11:35:28.987937 xpypact-0.4.3/src/xpypact/fluxes.py
+-rw-r--r--   0        0        0     5862 2023-06-19 11:35:28.987937 xpypact-0.4.3/src/xpypact/inventory.py
+-rw-r--r--   0        0        0     1965 2023-06-19 11:35:28.987937 xpypact-0.4.3/src/xpypact/nuclide.py
+-rw-r--r--   0        0        0        0 2023-06-19 11:35:28.987937 xpypact-0.4.3/src/xpypact/py.typed
+-rw-r--r--   0        0        0      515 2023-06-19 11:35:28.987937 xpypact-0.4.3/src/xpypact/run_data.py
+-rw-r--r--   0        0        0     4924 2023-06-19 11:35:28.987937 xpypact-0.4.3/src/xpypact/time_step.py
+-rw-r--r--   0        0        0       29 2023-06-19 11:35:28.987937 xpypact-0.4.3/src/xpypact/utils/__init__.py
+-rw-r--r--   0        0        0      809 2023-06-19 11:35:28.987937 xpypact-0.4.3/src/xpypact/utils/io.py
+-rw-r--r--   0        0        0        0 2023-06-19 11:35:28.987937 xpypact-0.4.3/src/xpypact/utils/py.typed
+-rw-r--r--   0        0        0      768 2023-06-19 11:35:28.987937 xpypact-0.4.3/src/xpypact/utils/resource.py
+-rw-r--r--   0        0        0      270 2023-06-19 11:35:28.987937 xpypact-0.4.3/src/xpypact/utils/types.py
+-rw-r--r--   0        0        0     4789 1970-01-01 00:00:00.000000 xpypact-0.4.3/PKG-INFO
```

### Comparing `xpypact-0.4.2/LICENSE` & `xpypact-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.2/README.rst` & `xpypact-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.2/pyproject.toml` & `xpypact-0.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xpypact"
-version = "0.4.2"
+version = "0.4.3"
 description = "\"Python tools to work with elements and isotopes\""
 authors = ["dvp <dmitri_portnov@yahoo.com>"]
 license = "MIT"
 homepage = "https://github.com/MC-kit/xpypact"
 repository = "https://github.com/MC-kit/xpypact"
 documentation = "https://xpypact.readthedocs.io"
 keywords = [
@@ -67,22 +67,21 @@
 #[tool.poetry.group.profile.dependencies]
 # TODO dvp: apply yappi: https://coderzcolumn.com/tutorials/python/yappi-yet-another-python-profiler
 #yappi = ">=1.3.2"
 
 [tool.poetry.group.pre_commit.dependencies]
 pre-commit = ">=2.15.0"
 rstcheck = ">=3.3.1"
-pydocstringformatter = "^0.7.3"
+pydocstringformatter = ">=0.7.3"
 
 [tool.poetry.group.black.dependencies]
 black = ">=22.8.0"  #TODO dvp: update with safety and packaging
 
 [tool.poetry.group.isort.dependencies]
 isort = ">=5.9.3"
-pycln = {version = "^2.1.1", extras = ["click"]}
 
 [tool.poetry.group.test.dependencies]
 pytest = ">=7.1"
 pytest-cache = ">=1.0"
 pytest-cov = ">=4.0"
 pytest-mock = ">=3.9"
 pytest-randomly = ">=3.12"
@@ -324,15 +323,15 @@
     "xarray.*"
 ]
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = [
     "tomllib",
-    "tomli"
+    "tomli",
 ]
 allow_redefinition = true
 disable_error_code = "no-redef"
 
 [tool.check-manifest]
 ignore = [
     "tests/*",
```

### Comparing `xpypact-0.4.2/src/xpypact/__init__.py` & `xpypact-0.4.3/src/xpypact/__init__.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.2/src/xpypact/dao/api.py` & `xpypact-0.4.3/src/xpypact/dao/api.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.2/src/xpypact/dao/duckdb/create_schema.sql` & `xpypact-0.4.3/src/xpypact/dao/duckdb/create_schema.sql`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.2/src/xpypact/dao/duckdb/implementation.py` & `xpypact-0.4.3/src/xpypact/dao/duckdb/implementation.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.2/src/xpypact/data_arrays.py` & `xpypact-0.4.3/src/xpypact/data_arrays.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.2/src/xpypact/data_frames.py` & `xpypact-0.4.3/src/xpypact/data_frames.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.2/src/xpypact/fluxes.py` & `xpypact-0.4.3/src/xpypact/fluxes.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.2/src/xpypact/inventory.py` & `xpypact-0.4.3/src/xpypact/inventory.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.2/src/xpypact/nuclide.py` & `xpypact-0.4.3/src/xpypact/nuclide.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.2/src/xpypact/run_data.py` & `xpypact-0.4.3/src/xpypact/run_data.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.2/src/xpypact/time_step.py` & `xpypact-0.4.3/src/xpypact/time_step.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.2/src/xpypact/utils/io.py` & `xpypact-0.4.3/src/xpypact/utils/io.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.2/src/xpypact/utils/resource.py` & `xpypact-0.4.3/src/xpypact/utils/resource.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.2/PKG-INFO` & `xpypact-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpypact
-Version: 0.4.2
+Version: 0.4.3
 Summary: "Python tools to work with elements and isotopes"
 Home-page: https://github.com/MC-kit/xpypact
 License: MIT
 Keywords: element,nuclide,isotope,abundance,FISPACT,activation,duckdb,parquet
 Author: dvp
 Author-email: dmitri_portnov@yahoo.com
 Requires-Python: >=3.8.1,<4.0
```

