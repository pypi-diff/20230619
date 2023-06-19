# Comparing `tmp/pynostr_cli-0.1.1.tar.gz` & `tmp/pynostr_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynostr_cli-0.1.1.tar", max compression
+gzip compressed data, was "pynostr_cli-0.1.2.tar", max compression
```

## Comparing `pynostr_cli-0.1.1.tar` & `pynostr_cli-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      352 2023-06-19 06:04:20.047290 pynostr_cli-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-18 22:57:08.975264 pynostr_cli-0.1.1/pynostr_cli/__init__.py
--rw-r--r--   0        0        0     1008 2023-06-19 04:48:30.524816 pynostr_cli-0.1.1/pynostr_cli/cli.py
--rw-r--r--   0        0        0     1320 2023-06-19 05:01:05.336088 pynostr_cli-0.1.1/pynostr_cli/key.py
--rw-r--r--   0        0        0      466 2023-06-19 06:04:47.418747 pynostr_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      780 1970-01-01 00:00:00.000000 pynostr_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      370 2023-06-19 06:08:53.181149 pynostr_cli-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 22:57:08.975264 pynostr_cli-0.1.2/pynostr_cli/__init__.py
+-rw-r--r--   0        0        0     1008 2023-06-19 04:48:30.524816 pynostr_cli-0.1.2/pynostr_cli/cli.py
+-rw-r--r--   0        0        0     1320 2023-06-19 05:01:05.336088 pynostr_cli-0.1.2/pynostr_cli/key.py
+-rw-r--r--   0        0        0      466 2023-06-19 06:09:05.651926 pynostr_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      798 1970-01-01 00:00:00.000000 pynostr_cli-0.1.2/PKG-INFO
```

### Comparing `pynostr_cli-0.1.1/pynostr_cli/cli.py` & `pynostr_cli-0.1.2/pynostr_cli/cli.py`

 * *Files identical despite different names*

### Comparing `pynostr_cli-0.1.1/pynostr_cli/key.py` & `pynostr_cli-0.1.2/pynostr_cli/key.py`

 * *Files identical despite different names*

### Comparing `pynostr_cli-0.1.1/PKG-INFO` & `pynostr_cli-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynostr-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: CLI tool for interacting with the Nostr Protocol
 Author: Kenneth Curtis
 Author-email: kacurtis1616@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
@@ -20,7 +20,9 @@
 - generates public and private key pair in either hex or pem format, with an option to output to a file
 
 For more information, visit https://github.com/nostr-protocol/nostr
 
 # Get started
 
 `pip install pynostr-cli`
+
+`pynostr --help`
```

