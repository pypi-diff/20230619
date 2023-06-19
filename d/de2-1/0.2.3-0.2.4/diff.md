# Comparing `tmp/de2_1-0.2.3.tar.gz` & `tmp/de2_1-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "de2_1-0.2.3.tar", max compression
+gzip compressed data, was "de2_1-0.2.4.tar", max compression
```

## Comparing `de2_1-0.2.3.tar` & `de2_1-0.2.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-06-19 17:04:47.288696 de2_1-0.2.3/de2_1/__init__.py
--rw-r--r--   0        0        0     5834 2023-06-19 17:12:36.594094 de2_1-0.2.3/de2_1/main.py
--rw-r--r--   0        0        0      452 2023-06-19 17:13:27.461115 de2_1-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     4535 2023-06-12 14:41:20.868524 de2_1-0.2.3/README.md
--rw-r--r--   0        0        0     4837 1970-01-01 00:00:00.000000 de2_1-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-19 17:04:47.288696 de2_1-0.2.4/de2_1/__init__.py
+-rw-r--r--   0        0        0     6062 2023-06-19 17:32:58.456707 de2_1-0.2.4/de2_1/main.py
+-rw-r--r--   0        0        0      452 2023-06-19 17:33:09.109268 de2_1-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4535 2023-06-12 14:41:20.868524 de2_1-0.2.4/README.md
+-rw-r--r--   0        0        0     4837 1970-01-01 00:00:00.000000 de2_1-0.2.4/PKG-INFO
```

### Comparing `de2_1-0.2.3/de2_1/main.py` & `de2_1-0.2.4/de2_1/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,18 +132,22 @@
     
     input_shape = input_matrix.shape
     kernel_shape = kernel.shape
     
     output_rows = (input_shape[0] - kernel_shape[0]) // stride + 1
     output_cols = (input_shape[1] - kernel_shape[1]) // stride + 1
     
-    output = np.zeros((output_rows, output_cols))
+    output = np.zeros((output_rows, output_cols), dtype=np.float64)
     
     for i in range(output_rows):
         for j in range(output_cols):
             window = input_matrix[
                 i * stride : i * stride + kernel_shape[0],
-                j * stride : j * stride + kernel_shape[1]]
+                j * stride : j * stride + kernel_shape[1]
+                ].astype(np.float64)
             
             output[i, j] = np.sum(window * kernel)
     
+    if input_shape[0] < kernel_shape[0] or input_shape[1] < kernel_shape[1]:
+        raise ValueError("Dimensions of the input matrix and kernel are incompatible.")
+    
     return output
```

### Comparing `de2_1-0.2.3/README.md` & `de2_1-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `de2_1-0.2.3/PKG-INFO` & `de2_1-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: de2-1
-Version: 0.2.3
+Version: 0.2.4
 Summary: Turing college de2_1 sprint submission
 Author: JociusTa
 Author-email: tautvydasjocius@live.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
```

