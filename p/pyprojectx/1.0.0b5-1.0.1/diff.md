# Comparing `tmp/pyprojectx-1.0.0b5.tar.gz` & `tmp/pyprojectx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprojectx-1.0.0b5.tar", last modified: Mon Jun 19 06:54:04 2023, max compression
+gzip compressed data, was "pyprojectx-1.0.1.tar", last modified: Mon Jun 19 07:31:42 2023, max compression
```

## Comparing `pyprojectx-1.0.0b5.tar` & `pyprojectx-1.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1071 2023-06-19 06:51:31.075466 pyprojectx-1.0.0b5/LICENSE
--rw-r--r--   0        0        0     4601 2023-06-19 06:51:31.075466 pyprojectx-1.0.0b5/README.md
--rw-r--r--   0        0        0     4239 2023-06-19 06:54:04.772715 pyprojectx-1.0.0b5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/__init__.py
--rw-r--r--   0        0        0     5112 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/cli.py
--rw-r--r--   0        0        0     6677 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/config.py
--rw-r--r--   0        0        0     5471 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/env.py
--rw-r--r--   0        0        0        0 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/initializer/__init__.py
--rw-r--r--   0        0        0      348 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/initializer/global-template.toml
--rw-r--r--   0        0        0     7263 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/initializer/initializers.py
--rw-r--r--   0        0        0      839 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/initializer/pdm-template.toml
--rw-r--r--   0        0        0      858 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/initializer/poetry-template.toml
--rw-r--r--   0        0        0       32 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/initializer/poetry.toml
--rw-r--r--   0        0        0      863 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/initializer/project-template.toml
--rw-r--r--   0        0        0      303 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/log.py
--rw-r--r--   0        0        0        0 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/wrapper/__init__.py
--rw-r--r--   0        0        0       30 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/wrapper/pw.bat
--rwxr-xr-x   0        0        0     5949 2023-06-19 06:51:43.723540 pyprojectx-1.0.0b5/src/pyprojectx/wrapper/pw.py
--rwxr-xr-x   0        0        0      253 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/wrapper/px
--rw-r--r--   0        0        0      373 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/wrapper/px.bat
--rwxr-xr-x   0        0        0      275 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/wrapper/pxg
--rw-r--r--   0        0        0      270 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/wrapper/pxg.bat
--rw-r--r--   0        0        0        0 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/__init__.py
--rw-r--r--   0        0        0      905 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/conftest.py
--rw-r--r--   0        0        0      188 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/data/alias-abbreviations.toml
--rw-r--r--   0        0        0       21 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/data/invalid.toml
--rw-r--r--   0        0        0      862 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/data/pw-test.toml
--rw-r--r--   0        0        0       19 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/data/test-no-config.toml
--rw-r--r--   0        0        0       94 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/data/test-no-tool-config.toml
--rw-r--r--   0        0        0      720 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/data/test.toml
--rw-r--r--   0        0        0        0 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/integration/__init__.py
--rw-r--r--   0        0        0     5579 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/integration/test_pw.py
--rw-r--r--   0        0        0     4008 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/integration/test_px.py
--rw-r--r--   0        0        0        0 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/unit/__init__.py
--rw-r--r--   0        0        0     6968 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/unit/test_cli.py
--rw-r--r--   0        0        0     4166 2023-06-19 06:51:31.083466 pyprojectx-1.0.0b5/tests/unit/test_config.py
--rw-r--r--   0        0        0     3142 2023-06-19 06:51:31.083466 pyprojectx-1.0.0b5/tests/unit/test_env.py
--rw-r--r--   0        0        0     5412 1970-01-01 00:00:00.000000 pyprojectx-1.0.0b5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-19 07:29:44.630202 pyprojectx-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4601 2023-06-19 07:29:44.630202 pyprojectx-1.0.1/README.md
+-rw-r--r--   0        0        0     4282 2023-06-19 07:31:42.543924 pyprojectx-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-19 07:29:44.634202 pyprojectx-1.0.1/src/pyprojectx/__init__.py
+-rw-r--r--   0        0        0     5112 2023-06-19 07:29:44.634202 pyprojectx-1.0.1/src/pyprojectx/cli.py
+-rw-r--r--   0        0        0     6677 2023-06-19 07:29:44.634202 pyprojectx-1.0.1/src/pyprojectx/config.py
+-rw-r--r--   0        0        0     5471 2023-06-19 07:29:44.634202 pyprojectx-1.0.1/src/pyprojectx/env.py
+-rw-r--r--   0        0        0        0 2023-06-19 07:29:44.634202 pyprojectx-1.0.1/src/pyprojectx/initializer/__init__.py
+-rw-r--r--   0        0        0      348 2023-06-19 07:29:44.634202 pyprojectx-1.0.1/src/pyprojectx/initializer/global-template.toml
+-rw-r--r--   0        0        0     7263 2023-06-19 07:29:44.634202 pyprojectx-1.0.1/src/pyprojectx/initializer/initializers.py
+-rw-r--r--   0        0        0      839 2023-06-19 07:29:44.634202 pyprojectx-1.0.1/src/pyprojectx/initializer/pdm-template.toml
+-rw-r--r--   0        0        0      858 2023-06-19 07:29:44.634202 pyprojectx-1.0.1/src/pyprojectx/initializer/poetry-template.toml
+-rw-r--r--   0        0        0       32 2023-06-19 07:29:44.634202 pyprojectx-1.0.1/src/pyprojectx/initializer/poetry.toml
+-rw-r--r--   0        0        0      863 2023-06-19 07:29:44.634202 pyprojectx-1.0.1/src/pyprojectx/initializer/project-template.toml
+-rw-r--r--   0        0        0      303 2023-06-19 07:29:44.634202 pyprojectx-1.0.1/src/pyprojectx/log.py
+-rw-r--r--   0        0        0        0 2023-06-19 07:29:44.634202 pyprojectx-1.0.1/src/pyprojectx/wrapper/__init__.py
+-rw-r--r--   0        0        0       30 2023-06-19 07:29:44.634202 pyprojectx-1.0.1/src/pyprojectx/wrapper/pw.bat
+-rwxr-xr-x   0        0        0     5947 2023-06-19 07:29:51.846304 pyprojectx-1.0.1/src/pyprojectx/wrapper/pw.py
+-rwxr-xr-x   0        0        0      253 2023-06-19 07:29:44.634202 pyprojectx-1.0.1/src/pyprojectx/wrapper/px
+-rw-r--r--   0        0        0      373 2023-06-19 07:29:44.634202 pyprojectx-1.0.1/src/pyprojectx/wrapper/px.bat
+-rwxr-xr-x   0        0        0      275 2023-06-19 07:29:44.638202 pyprojectx-1.0.1/src/pyprojectx/wrapper/pxg
+-rw-r--r--   0        0        0      270 2023-06-19 07:29:44.638202 pyprojectx-1.0.1/src/pyprojectx/wrapper/pxg.bat
+-rw-r--r--   0        0        0        0 2023-06-19 07:29:44.638202 pyprojectx-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0      905 2023-06-19 07:29:44.638202 pyprojectx-1.0.1/tests/conftest.py
+-rw-r--r--   0        0        0      188 2023-06-19 07:29:44.638202 pyprojectx-1.0.1/tests/data/alias-abbreviations.toml
+-rw-r--r--   0        0        0       21 2023-06-19 07:29:44.638202 pyprojectx-1.0.1/tests/data/invalid.toml
+-rw-r--r--   0        0        0      862 2023-06-19 07:29:44.638202 pyprojectx-1.0.1/tests/data/pw-test.toml
+-rw-r--r--   0        0        0       19 2023-06-19 07:29:44.638202 pyprojectx-1.0.1/tests/data/test-no-config.toml
+-rw-r--r--   0        0        0       94 2023-06-19 07:29:44.638202 pyprojectx-1.0.1/tests/data/test-no-tool-config.toml
+-rw-r--r--   0        0        0      720 2023-06-19 07:29:44.638202 pyprojectx-1.0.1/tests/data/test.toml
+-rw-r--r--   0        0        0        0 2023-06-19 07:29:44.638202 pyprojectx-1.0.1/tests/integration/__init__.py
+-rw-r--r--   0        0        0     5579 2023-06-19 07:29:44.638202 pyprojectx-1.0.1/tests/integration/test_pw.py
+-rw-r--r--   0        0        0     4008 2023-06-19 07:29:44.638202 pyprojectx-1.0.1/tests/integration/test_px.py
+-rw-r--r--   0        0        0        0 2023-06-19 07:29:44.638202 pyprojectx-1.0.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0     6968 2023-06-19 07:29:44.638202 pyprojectx-1.0.1/tests/unit/test_cli.py
+-rw-r--r--   0        0        0     4166 2023-06-19 07:29:44.638202 pyprojectx-1.0.1/tests/unit/test_config.py
+-rw-r--r--   0        0        0     3142 2023-06-19 07:29:44.638202 pyprojectx-1.0.1/tests/unit/test_env.py
+-rw-r--r--   0        0        0     5410 1970-01-01 00:00:00.000000 pyprojectx-1.0.1/PKG-INFO
```

### Comparing `pyprojectx-1.0.0b5/LICENSE` & `pyprojectx-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b5/README.md` & `pyprojectx-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b5/pyproject.toml` & `pyprojectx-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyprojectx"
-version = "1.0.0b5"
+version = "1.0.1"
 description = "Execute scripts from pyproject.toml, installing tools on-the-fly"
 authors = [
     { name = "Houbie", email = "ivo@houbrechts-it.be" },
 ]
 readme = "README.md"
 keywords = [
     "build",
@@ -188,21 +188,32 @@
 outdated = "pdm update --outdated"
 clean = "rm -r .venv .pytest_cache dist"
 clean-all = "pw@clean\nrm -r .pyprojectx"
 black = "black src tests"
 isort = "isort src tests"
 unit-test = "pdm run pytest tests/unit"
 integration-test = "pdm run pytest tests/integration"
-test = "pw@unit-test && pw@integration-test"
+test = [
+    "pw@unit-test",
+    "pw@integration-test",
+]
 check-ruff = "ruff check src tests"
 check-black = "black src tests --check"
-check = "pw@check-black && pw@check-ruff && pw@test"
-build = "pw@install && pw@check && pw@pdm build"
+check = [
+    "pw@check-black",
+    "pw@check-ruff",
+    "pw@test",
+]
+build = [
+    "pw@install",
+    "pw@check",
+    "pw@pdm build",
+]
 publish = "pdm publish --username __token__"
-prep-release = "# cleanup\nrm -f wrappers.zip .changelog.md\n# extract version from tag\nRELEASE_VERSION=\"${GITHUB_REF_NAME}\"\n# replace __version__ in wrapper\nsed -i -e \"s/__version__/${RELEASE_VERSION}/g\" src/pyprojectx/wrapper/pw.py\nsed -i -e \"s/1.0.0b5/${RELEASE_VERSION}/g\" pyproject.toml\n# cleanup sed backup\nrm -r src/pyprojectx/wrapper/pw.py?*\nrm -r pyproject.toml?*\nmkdir -p dist-zip\ncp src/pyprojectx/wrapper/pw.py dist-zip/pw\ncp src/pyprojectx/wrapper/pw.bat dist-zip/pw.bat\nzip -j wrappers.zip dist-zip/pw*\nawk '/-{3,}/{flag=1;next}/Release/{if (flag==1)exit}flag' CHANGELOG.md > .changelog.md\n"
+prep-release = "# cleanup\nrm -f wrappers.zip .changelog.md\n# extract version from tag\nRELEASE_VERSION=\"${GITHUB_REF_NAME}\"\n# replace __version__ in wrapper\nsed -i -e \"s/__version__/${RELEASE_VERSION}/g\" src/pyprojectx/wrapper/pw.py\nsed -i -e \"s/1.0.1/${RELEASE_VERSION}/g\" pyproject.toml\n# cleanup sed backup\nrm -r src/pyprojectx/wrapper/pw.py?*\nrm -r pyproject.toml?*\nmkdir -p dist-zip\ncp src/pyprojectx/wrapper/pw.py dist-zip/pw\ncp src/pyprojectx/wrapper/pw.bat dist-zip/pw.bat\nzip -j wrappers.zip dist-zip/pw*\nawk '/-{3,}/{flag=1;next}/Release/{if (flag==1)exit}flag' CHANGELOG.md > .changelog.md\n"
 generate-usage = "pw@ --help > docs/docs/usage.txt"
 serve-docs = "@mkdocs: cd docs && mkdocs serve"
 generate-docs = "@mkdocs: pw@generate-usage && cd docs && mkdocs build"
 deploy-docs = "@mkdocs: cd docs && mkdocs gh-deploy"
 
 [tool.pyprojectx.os.win.aliases]
 clean = "rmdir /s/q .venv .pytest_cache dist"
```

### Comparing `pyprojectx-1.0.0b5/src/pyprojectx/cli.py` & `pyprojectx-1.0.1/src/pyprojectx/cli.py`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b5/src/pyprojectx/config.py` & `pyprojectx-1.0.1/src/pyprojectx/config.py`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b5/src/pyprojectx/env.py` & `pyprojectx-1.0.1/src/pyprojectx/env.py`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b5/src/pyprojectx/initializer/initializers.py` & `pyprojectx-1.0.1/src/pyprojectx/initializer/initializers.py`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b5/src/pyprojectx/initializer/pdm-template.toml` & `pyprojectx-1.0.1/src/pyprojectx/initializer/pdm-template.toml`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b5/src/pyprojectx/initializer/poetry-template.toml` & `pyprojectx-1.0.1/src/pyprojectx/initializer/poetry-template.toml`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b5/src/pyprojectx/initializer/project-template.toml` & `pyprojectx-1.0.1/src/pyprojectx/initializer/project-template.toml`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b5/src/pyprojectx/wrapper/pw.py` & `pyprojectx-1.0.1/src/pyprojectx/wrapper/pw.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import argparse
 import os
 import subprocess
 import sys
 from pathlib import Path
 from venv import EnvBuilder
 
-VERSION = "1.0.0b5"
+VERSION = "1.0.1"
 
 PYPROJECTX_INSTALL_DIR_ENV_VAR = "PYPROJECTX_INSTALL_DIR"
 PYPROJECTX_PACKAGE_ENV_VAR = "PYPROJECTX_PACKAGE"
 PYPROJECT_TOML = "pyproject.toml"
 DEFAULT_INSTALL_DIR = ".pyprojectx"
 
 CYAN = "\033[96m"
```

### Comparing `pyprojectx-1.0.0b5/tests/conftest.py` & `pyprojectx-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b5/tests/data/pw-test.toml` & `pyprojectx-1.0.1/tests/data/pw-test.toml`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b5/tests/data/test.toml` & `pyprojectx-1.0.1/tests/data/test.toml`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b5/tests/integration/test_pw.py` & `pyprojectx-1.0.1/tests/integration/test_pw.py`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b5/tests/integration/test_px.py` & `pyprojectx-1.0.1/tests/integration/test_px.py`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b5/tests/unit/test_cli.py` & `pyprojectx-1.0.1/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b5/tests/unit/test_config.py` & `pyprojectx-1.0.1/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b5/tests/unit/test_env.py` & `pyprojectx-1.0.1/tests/unit/test_env.py`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b5/PKG-INFO` & `pyprojectx-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprojectx
-Version: 1.0.0b5
+Version: 1.0.1
 Summary: Execute scripts from pyproject.toml, installing tools on-the-fly
 Keywords: build dependency pyprojectx
 Home-page: https://github.com/pyprojectx/pyprojectx
 Author-Email: Houbie <ivo@houbrechts-it.be>
 License: MIT
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

