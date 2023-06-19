# Comparing `tmp/web3_input_decoder-0.1.8.tar.gz` & `tmp/web3_input_decoder-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3_input_decoder-0.1.8.tar", max compression
+gzip compressed data, was "web3_input_decoder-0.1.9.tar", max compression
```

## Comparing `web3_input_decoder-0.1.8.tar` & `web3_input_decoder-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2023-03-31 17:23:18.486218 web3_input_decoder-0.1.8/LICENSE
--rw-r--r--   0        0        0     4554 2023-03-31 17:23:18.486218 web3_input_decoder-0.1.8/README.md
--rw-r--r--   0        0        0     1248 2023-03-31 17:23:18.490218 web3_input_decoder-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1380 2023-03-31 17:23:18.490218 web3_input_decoder-0.1.8/web3_input_decoder/__init__.py
--rw-r--r--   0        0        0     1883 2023-03-31 17:23:18.490218 web3_input_decoder-0.1.8/web3_input_decoder/decoder.py
--rw-r--r--   0        0        0      411 2023-03-31 17:23:18.490218 web3_input_decoder-0.1.8/web3_input_decoder/exceptions.py
--rw-r--r--   0        0        0       27 2023-03-31 17:23:18.490218 web3_input_decoder-0.1.8/web3_input_decoder/py.typed
--rw-r--r--   0        0        0     2544 2023-03-31 17:23:18.490218 web3_input_decoder-0.1.8/web3_input_decoder/utils.py
--rw-r--r--   0        0        0     5796 1970-01-01 00:00:00.000000 web3_input_decoder-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-19 13:29:33.380029 web3_input_decoder-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4554 2023-06-19 13:29:33.380029 web3_input_decoder-0.1.9/README.md
+-rw-r--r--   0        0        0     1247 2023-06-19 13:29:33.380029 web3_input_decoder-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1380 2023-06-19 13:29:33.384029 web3_input_decoder-0.1.9/web3_input_decoder/__init__.py
+-rw-r--r--   0        0        0     1883 2023-06-19 13:29:33.384029 web3_input_decoder-0.1.9/web3_input_decoder/decoder.py
+-rw-r--r--   0        0        0      411 2023-06-19 13:29:33.384029 web3_input_decoder-0.1.9/web3_input_decoder/exceptions.py
+-rw-r--r--   0        0        0       27 2023-06-19 13:29:33.384029 web3_input_decoder-0.1.9/web3_input_decoder/py.typed
+-rw-r--r--   0        0        0     2544 2023-06-19 13:29:33.384029 web3_input_decoder-0.1.9/web3_input_decoder/utils.py
+-rw-r--r--   0        0        0     5748 1970-01-01 00:00:00.000000 web3_input_decoder-0.1.9/PKG-INFO
```

### Comparing `web3_input_decoder-0.1.8/LICENSE` & `web3_input_decoder-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `web3_input_decoder-0.1.8/README.md` & `web3_input_decoder-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `web3_input_decoder-0.1.8/pyproject.toml` & `web3_input_decoder-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web3-input-decoder"
-version = "0.1.8"
+version = "0.1.9"
 # doc
 authors = ["Weiliang Li <to.be.impressive@gmail.com>"]
 description = "A simple offline web3 transaction input decoder for functions and constructors"
 license = "MIT"
 maintainers = ["Weiliang Li <to.be.impressive@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/kigawas/web3-input-decoder"
@@ -20,33 +20,33 @@
   "ethereum",
   "web3",
 ]
 # package data: PEP-561
 include = ["web3_input_decoder/py.typed"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.7.2"
 
 # 3rd party
-eth-abi = "^4.0.0b2"
+eth-abi = "^4.0.0"
 eth-utils = "^2.1.0"
-pycryptodome = "^3.15.0"
+pycryptodome = "^3.17.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
-flake8 = {version = "^6.0.0", python = "^3.8.1"}
-ipython = {version = "^8.6.0", python = "^3.8"}
-mypy = "^1.1"
+flake8 = {version = "^6.0.0", python = "^3.9"}
+ipython = {version = "^8.13.1", python = "^3.9"}
+mypy = "^1.2"
 
 # stubs
-eth-typing = "^3.2.0"
+eth-typing = "^3.3.0"
 
 # test
-pyinstrument = "^4.3.0"
-pytest = "^7.2.0"
+pyinstrument = "^4.5.0"
+pytest = "^7.3.0"
 pytest-cov = "^4.0.0"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.isort]
```

### Comparing `web3_input_decoder-0.1.8/web3_input_decoder/__init__.py` & `web3_input_decoder-0.1.9/web3_input_decoder/__init__.py`

 * *Files identical despite different names*

### Comparing `web3_input_decoder-0.1.8/web3_input_decoder/decoder.py` & `web3_input_decoder-0.1.9/web3_input_decoder/decoder.py`

 * *Files identical despite different names*

### Comparing `web3_input_decoder-0.1.8/web3_input_decoder/utils.py` & `web3_input_decoder-0.1.9/web3_input_decoder/utils.py`

 * *Files identical despite different names*

### Comparing `web3_input_decoder-0.1.8/PKG-INFO` & `web3_input_decoder-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: web3-input-decoder
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple offline web3 transaction input decoder for functions and constructors
 Home-page: https://github.com/kigawas/web3-input-decoder
 License: MIT
 Keywords: ethereum,web3
 Author: Weiliang Li
 Author-email: to.be.impressive@gmail.com
 Maintainer: Weiliang Li
 Maintainer-email: to.be.impressive@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7.2,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Dist: eth-abi (>=4.0.0b2,<5.0.0)
+Requires-Dist: eth-abi (>=4.0.0,<5.0.0)
 Requires-Dist: eth-utils (>=2.1.0,<3.0.0)
-Requires-Dist: pycryptodome (>=3.15.0,<4.0.0)
+Requires-Dist: pycryptodome (>=3.17.0,<4.0.0)
 Project-URL: Repository, https://github.com/kigawas/web3-input-decoder
 Description-Content-Type: text/markdown
 
 # web3-input-decoder
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/6f10d5104ef4464797ee94b17c7b9371)](https://www.codacy.com/gh/kigawas/web3-input-decoder/dashboard)
 [![CI](https://img.shields.io/github/actions/workflow/status/kigawas/web3-input-decoder/ci.yml)](https://github.com/kigawas/web3-input-decoder/actions)
```

