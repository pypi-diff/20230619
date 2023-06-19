# Comparing `tmp/hayloft-0.1.7.tar.gz` & `tmp/hayloft-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hayloft-0.1.7.tar", max compression
+gzip compressed data, was "hayloft-0.1.8.tar", max compression
```

## Comparing `hayloft-0.1.7.tar` & `hayloft-0.1.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.1.7/LICENSE
--rw-r--r--   0        0        0      908 2023-06-18 15:56:02.291486 hayloft-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.1.7/hayloft/__init__.py
--rw-r--r--   0        0        0     3269 2023-06-18 15:54:20.457801 hayloft-0.1.7/hayloft/app.py
--rw-r--r--   0        0        0      477 2023-06-18 13:29:30.706385 hayloft-0.1.7/hayloft/logger.py
--rw-r--r--   0        0        0    18224 2023-06-18 15:55:10.311304 hayloft-0.1.7/hayloft/public/assets/index-7630e259.css
--rw-r--r--   0        0        0   175056 2023-06-18 15:55:10.311304 hayloft-0.1.7/hayloft/public/assets/index-be461c13.js
--rw-r--r--   0        0        0      384 2023-06-18 15:55:15.047987 hayloft-0.1.7/hayloft/public/index.html
--rw-r--r--   0        0        0     1367 2023-06-13 15:26:48.605765 hayloft-0.1.7/hayloft/schema.py
--rw-r--r--   0        0        0      430 2023-06-18 15:56:23.424894 hayloft-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 hayloft-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.1.8/LICENSE
+-rw-r--r--   0        0        0      908 2023-06-18 15:56:02.291486 hayloft-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.1.8/hayloft/__init__.py
+-rw-r--r--   0        0        0     3269 2023-06-18 15:54:20.457801 hayloft-0.1.8/hayloft/app.py
+-rw-r--r--   0        0        0      669 2023-06-19 12:12:50.488202 hayloft-0.1.8/hayloft/logger.py
+-rw-r--r--   0        0        0    18224 2023-06-18 15:55:10.311304 hayloft-0.1.8/hayloft/public/assets/index-7630e259.css
+-rw-r--r--   0        0        0   175056 2023-06-18 15:55:10.311304 hayloft-0.1.8/hayloft/public/assets/index-be461c13.js
+-rw-r--r--   0        0        0      384 2023-06-18 15:55:15.047987 hayloft-0.1.8/hayloft/public/index.html
+-rw-r--r--   0        0        0     1367 2023-06-13 15:26:48.605765 hayloft-0.1.8/hayloft/schema.py
+-rw-r--r--   0        0        0      430 2023-06-19 12:15:27.918544 hayloft-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 hayloft-0.1.8/PKG-INFO
```

### Comparing `hayloft-0.1.7/LICENSE` & `hayloft-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.7/README.md` & `hayloft-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.7/hayloft/app.py` & `hayloft-0.1.8/hayloft/app.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.7/hayloft/public/assets/index-7630e259.css` & `hayloft-0.1.8/hayloft/public/assets/index-7630e259.css`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.7/hayloft/public/assets/index-be461c13.js` & `hayloft-0.1.8/hayloft/public/assets/index-be461c13.js`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.7/hayloft/schema.py` & `hayloft-0.1.8/hayloft/schema.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.7/PKG-INFO` & `hayloft-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hayloft
-Version: 0.1.7
+Version: 0.1.8
 Summary: UI tool for LLM frameworks
 License: MIT
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

