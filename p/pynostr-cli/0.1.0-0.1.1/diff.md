# Comparing `tmp/pynostr_cli-0.1.0.tar.gz` & `tmp/pynostr_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynostr_cli-0.1.0.tar", max compression
+gzip compressed data, was "pynostr_cli-0.1.1.tar", max compression
```

## Comparing `pynostr_cli-0.1.0.tar` & `pynostr_cli-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      310 2023-06-19 05:40:00.073616 pynostr_cli-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-18 22:57:08.975264 pynostr_cli-0.1.0/pynostr_cli/__init__.py
--rw-r--r--   0        0        0     1008 2023-06-19 04:48:30.524816 pynostr_cli-0.1.0/pynostr_cli/cli.py
--rw-r--r--   0        0        0     1320 2023-06-19 05:01:05.336088 pynostr_cli-0.1.0/pynostr_cli/key.py
--rw-r--r--   0        0        0      412 2023-06-19 05:34:03.324305 pynostr_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 pynostr_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      352 2023-06-19 06:04:20.047290 pynostr_cli-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 22:57:08.975264 pynostr_cli-0.1.1/pynostr_cli/__init__.py
+-rw-r--r--   0        0        0     1008 2023-06-19 04:48:30.524816 pynostr_cli-0.1.1/pynostr_cli/cli.py
+-rw-r--r--   0        0        0     1320 2023-06-19 05:01:05.336088 pynostr_cli-0.1.1/pynostr_cli/key.py
+-rw-r--r--   0        0        0      466 2023-06-19 06:04:47.418747 pynostr_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      780 1970-01-01 00:00:00.000000 pynostr_cli-0.1.1/PKG-INFO
```

### Comparing `pynostr_cli-0.1.0/pynostr_cli/cli.py` & `pynostr_cli-0.1.1/pynostr_cli/cli.py`

 * *Files identical despite different names*

### Comparing `pynostr_cli-0.1.0/pynostr_cli/key.py` & `pynostr_cli-0.1.1/pynostr_cli/key.py`

 * *Files identical despite different names*

### Comparing `pynostr_cli-0.1.0/PKG-INFO` & `pynostr_cli-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynostr-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: CLI tool for interacting with the Nostr Protocol
 Author: Kenneth Curtis
 Author-email: kacurtis1616@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
@@ -16,7 +16,11 @@
 Very early work in progress of a cli tool that will interface with the nostr protocol
 
 Currently supported functionality:
 
 - generates public and private key pair in either hex or pem format, with an option to output to a file
 
 For more information, visit https://github.com/nostr-protocol/nostr
+
+# Get started
+
+`pip install pynostr-cli`
```

