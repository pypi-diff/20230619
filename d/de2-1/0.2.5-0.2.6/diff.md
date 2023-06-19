# Comparing `tmp/de2_1-0.2.5.tar.gz` & `tmp/de2_1-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "de2_1-0.2.5.tar", max compression
+gzip compressed data, was "de2_1-0.2.6.tar", max compression
```

## Comparing `de2_1-0.2.5.tar` & `de2_1-0.2.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-06-19 17:04:47.288696 de2_1-0.2.5/de2_1/__init__.py
--rw-r--r--   0        0        0     6225 2023-06-19 17:40:54.867622 de2_1-0.2.5/de2_1/main.py
--rw-r--r--   0        0        0      452 2023-06-19 17:41:12.651332 de2_1-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     4535 2023-06-12 14:41:20.868524 de2_1-0.2.5/README.md
--rw-r--r--   0        0        0     4837 1970-01-01 00:00:00.000000 de2_1-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-19 17:04:47.288696 de2_1-0.2.6/de2_1/__init__.py
+-rw-r--r--   0        0        0     6122 2023-06-19 17:43:23.725694 de2_1-0.2.6/de2_1/main.py
+-rw-r--r--   0        0        0      452 2023-06-19 17:43:47.517466 de2_1-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     4535 2023-06-12 14:41:20.868524 de2_1-0.2.6/README.md
+-rw-r--r--   0        0        0     4837 1970-01-01 00:00:00.000000 de2_1-0.2.6/PKG-INFO
```

### Comparing `de2_1-0.2.5/de2_1/main.py` & `de2_1-0.2.6/de2_1/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,24 +133,23 @@
     input_shape = input_matrix.shape
     kernel_shape = kernel.shape
     if input_shape[0] < kernel_shape[0] or input_shape[1] < kernel_shape[1]:
         raise ValueError("Dimensions of the input matrix and kernel are incompatible.")
     
     padding_rows = kernel_shape[0] - 1
     padding_cols = kernel_shape[1] - 1
-    padded_input = np.pad(input_matrix, ((padding_rows, padding_rows), (padding_cols, padding_cols)))
 
     output_rows = (input_shape[0] - kernel_shape[0]) // stride + 1
     output_cols = (input_shape[1] - kernel_shape[1]) // stride + 1
     
     output = np.zeros((output_rows, output_cols), dtype=np.float64)
     
     for i in range(output_rows):
         for j in range(output_cols):
-            window = padded_input[
+            window = input_matrix[
                 i * stride : i * stride + kernel_shape[0],
                 j * stride : j * stride + kernel_shape[1]
             ].astype(np.float64)
 
             output[i, j] = np.sum(window * kernel)
     
     return output
```

### Comparing `de2_1-0.2.5/README.md` & `de2_1-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `de2_1-0.2.5/PKG-INFO` & `de2_1-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: de2-1
-Version: 0.2.5
+Version: 0.2.6
 Summary: Turing college de2_1 sprint submission
 Author: JociusTa
 Author-email: tautvydasjocius@live.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
```

