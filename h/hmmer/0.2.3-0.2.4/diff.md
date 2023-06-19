# Comparing `tmp/hmmer-0.2.3.tar.gz` & `tmp/hmmer-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmmer-0.2.3.tar", max compression
+gzip compressed data, was "hmmer-0.2.4.tar", max compression
```

## Comparing `hmmer-0.2.3.tar` & `hmmer-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-02-28 16:07:17.651923 hmmer-0.2.3/LICENSE
--rw-r--r--   0        0        0        8 2023-02-28 16:07:17.651923 hmmer-0.2.3/README.md
--rw-r--r--   0        0        0      203 2023-02-28 16:07:17.651923 hmmer-0.2.3/build_hmmer.py
--rwxr-xr-x   0        0        0      923 2023-02-28 16:07:17.651923 hmmer-0.2.3/build_hmmer.sh
--rw-r--r--   0        0        0     1838 2023-02-28 16:07:17.651923 hmmer-0.2.3/hmmer/__init__.py
--rw-r--r--   0        0        0     1344 2023-02-28 16:07:17.651923 hmmer-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 hmmer-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-19 08:17:56.691118 hmmer-0.2.4/LICENSE
+-rw-r--r--   0        0        0        8 2023-06-19 08:17:56.691118 hmmer-0.2.4/README.md
+-rw-r--r--   0        0        0      203 2023-06-19 08:17:56.691118 hmmer-0.2.4/build_hmmer.py
+-rwxr-xr-x   0        0        0      923 2023-06-19 08:17:56.691118 hmmer-0.2.4/build_hmmer.sh
+-rw-r--r--   0        0        0     1838 2023-06-19 08:17:56.691118 hmmer-0.2.4/hmmer/__init__.py
+-rw-r--r--   0        0        0     1398 2023-06-19 08:17:56.691118 hmmer-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 hmmer-0.2.4/PKG-INFO
```

### Comparing `hmmer-0.2.3/LICENSE` & `hmmer-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hmmer-0.2.3/build_hmmer.sh` & `hmmer-0.2.4/build_hmmer.sh`

 * *Files identical despite different names*

### Comparing `hmmer-0.2.3/hmmer/__init__.py` & `hmmer-0.2.4/hmmer/__init__.py`

 * *Files identical despite different names*

### Comparing `hmmer-0.2.3/pyproject.toml` & `hmmer-0.2.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "hmmer"
-version = "0.2.3"
+version = "0.2.4"
 description = "HMMER binaries."
-authors = ["Danilo Horta <danilo.horta@pm.me>"]
+authors = ["Danilo Horta <horta@ebi.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "hmmer" }]
 exclude = [{ path = "hmmer/data/bin/*", format = "sdist" }]
 include = [
   { path = "hmmer/data/bin/*", format = "wheel" },
   { path = "build_hmmer.py", format = "sdist" },
@@ -16,14 +16,17 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 
 [tool.poetry.build]
 script = "build_hmmer.py"
 generate-setup-file = false
 
+[tool.poetry.group.dev.dependencies]
+pytest = ">=7.3.2"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 alimask = 'hmmer:alimask'
 hmmalign = 'hmmer:hmmalign'
```

