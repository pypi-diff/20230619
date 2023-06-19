# Comparing `tmp/polywrap_test_cases-0.1.0a30.tar.gz` & `tmp/polywrap_test_cases-0.1.0a31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_test_cases-0.1.0a30.tar", max compression
+gzip compressed data, was "polywrap_test_cases-0.1.0a31.tar", max compression
```

## Comparing `polywrap_test_cases-0.1.0a30.tar` & `polywrap_test_cases-0.1.0a31.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       96 2023-06-19 11:25:19.305153 polywrap_test_cases-0.1.0a30/README.md
--rw-r--r--   0        0        0     1257 2023-06-19 11:25:19.305153 polywrap_test_cases-0.1.0a30/polywrap_test_cases/__init__.py
--rw-r--r--   0        0        0      142 2023-06-19 11:25:19.305153 polywrap_test_cases-0.1.0a30/polywrap_test_cases/__main__.py
--rw-r--r--   0        0        0        0 2023-06-19 11:25:19.305153 polywrap_test_cases-0.1.0a30/polywrap_test_cases/py.typed
--rw-r--r--   0        0        0      991 2023-06-19 11:30:31.540289 polywrap_test_cases-0.1.0a30/pyproject.toml
--rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 polywrap_test_cases-0.1.0a30/PKG-INFO
+-rw-r--r--   0        0        0       96 2023-06-19 12:57:22.870931 polywrap_test_cases-0.1.0a31/README.md
+-rw-r--r--   0        0        0     1257 2023-06-19 12:57:22.870931 polywrap_test_cases-0.1.0a31/polywrap_test_cases/__init__.py
+-rw-r--r--   0        0        0      142 2023-06-19 12:57:22.870931 polywrap_test_cases-0.1.0a31/polywrap_test_cases/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:57:22.870931 polywrap_test_cases-0.1.0a31/polywrap_test_cases/py.typed
+-rw-r--r--   0        0        0      991 2023-06-19 13:01:59.569406 polywrap_test_cases-0.1.0a31/pyproject.toml
+-rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 polywrap_test_cases-0.1.0a31/PKG-INFO
```

### Comparing `polywrap_test_cases-0.1.0a30/polywrap_test_cases/__init__.py` & `polywrap_test_cases-0.1.0a31/polywrap_test_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `polywrap_test_cases-0.1.0a30/pyproject.toml` & `polywrap_test_cases-0.1.0a31/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-test-cases"
-version = "0.1.0a30"
+version = "0.1.0a31"
 description = "Plugin package"
 authors = ["Cesar <cesar@polywrap.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

