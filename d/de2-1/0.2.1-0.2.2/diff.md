# Comparing `tmp/de2_1-0.2.1.tar.gz` & `tmp/de2_1-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "de2_1-0.2.1.tar", max compression
+gzip compressed data, was "de2_1-0.2.2.tar", max compression
```

## Comparing `de2_1-0.2.1.tar` & `de2_1-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-19 17:04:47.288696 de2_1-0.2.1/de2_1/__init__.py
--rw-r--r--   0        0        0     5834 2023-06-19 16:52:05.238471 de2_1-0.2.1/de2_1/main.py
--rw-r--r--   0        0        0      452 2023-06-19 17:05:51.337689 de2_1-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4535 2023-06-12 14:41:20.868524 de2_1-0.2.1/README.md
--rw-r--r--   0        0        0     4837 1970-01-01 00:00:00.000000 de2_1-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-19 17:04:47.288696 de2_1-0.2.2/de2_1/__init__.py
+-rw-r--r--   0        0        0     1843 2023-06-19 17:09:39.842339 de2_1-0.2.2/de2_1/convolution2d.py
+-rw-r--r--   0        0        0     1277 2023-06-19 17:08:16.066727 de2_1-0.2.2/de2_1/transpose2d.py
+-rw-r--r--   0        0        0     2751 2023-06-19 17:10:00.416391 de2_1-0.2.2/de2_1/window1d.py
+-rw-r--r--   0        0        0      452 2023-06-19 17:10:23.991477 de2_1-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4535 2023-06-12 14:41:20.868524 de2_1-0.2.2/README.md
+-rw-r--r--   0        0        0     4837 1970-01-01 00:00:00.000000 de2_1-0.2.2/PKG-INFO
```

### Comparing `de2_1-0.2.1/README.md` & `de2_1-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `de2_1-0.2.1/PKG-INFO` & `de2_1-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: de2-1
-Version: 0.2.1
+Version: 0.2.2
 Summary: Turing college de2_1 sprint submission
 Author: JociusTa
 Author-email: tautvydasjocius@live.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
```

