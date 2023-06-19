# Comparing `tmp/de2_1-0.2.0.tar.gz` & `tmp/de2_1-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "de2_1-0.2.0.tar", max compression
+gzip compressed data, was "de2_1-0.2.1.tar", max compression
```

## Comparing `de2_1-0.2.0.tar` & `de2_1-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       53 2023-06-19 06:18:46.913155 de2_1-0.2.0/de2_1/__init__.py
--rw-r--r--   0        0        0     5834 2023-06-19 16:52:05.238471 de2_1-0.2.0/de2_1/main.py
--rw-r--r--   0        0        0      452 2023-06-19 16:55:16.560286 de2_1-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4535 2023-06-12 14:41:20.868524 de2_1-0.2.0/README.md
--rw-r--r--   0        0        0     4837 1970-01-01 00:00:00.000000 de2_1-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-19 17:04:47.288696 de2_1-0.2.1/de2_1/__init__.py
+-rw-r--r--   0        0        0     5834 2023-06-19 16:52:05.238471 de2_1-0.2.1/de2_1/main.py
+-rw-r--r--   0        0        0      452 2023-06-19 17:05:51.337689 de2_1-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4535 2023-06-12 14:41:20.868524 de2_1-0.2.1/README.md
+-rw-r--r--   0        0        0     4837 1970-01-01 00:00:00.000000 de2_1-0.2.1/PKG-INFO
```

### Comparing `de2_1-0.2.0/de2_1/main.py` & `de2_1-0.2.1/de2_1/main.py`

 * *Files identical despite different names*

### Comparing `de2_1-0.2.0/README.md` & `de2_1-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `de2_1-0.2.0/PKG-INFO` & `de2_1-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: de2-1
-Version: 0.2.0
+Version: 0.2.1
 Summary: Turing college de2_1 sprint submission
 Author: JociusTa
 Author-email: tautvydasjocius@live.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
```

