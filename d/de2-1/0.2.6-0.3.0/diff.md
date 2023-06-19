# Comparing `tmp/de2_1-0.2.6.tar.gz` & `tmp/de2_1-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "de2_1-0.2.6.tar", max compression
+gzip compressed data, was "de2_1-0.3.0.tar", max compression
```

## Comparing `de2_1-0.2.6.tar` & `de2_1-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-06-19 17:04:47.288696 de2_1-0.2.6/de2_1/__init__.py
--rw-r--r--   0        0        0     6122 2023-06-19 17:43:23.725694 de2_1-0.2.6/de2_1/main.py
--rw-r--r--   0        0        0      452 2023-06-19 17:43:47.517466 de2_1-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     4535 2023-06-12 14:41:20.868524 de2_1-0.2.6/README.md
--rw-r--r--   0        0        0     4837 1970-01-01 00:00:00.000000 de2_1-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-19 17:04:47.288696 de2_1-0.3.0/de2_1/__init__.py
+-rw-r--r--   0        0        0     5968 2023-06-19 17:57:10.424231 de2_1-0.3.0/de2_1/main.py
+-rw-r--r--   0        0        0      475 2023-06-19 17:57:54.628216 de2_1-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4535 2023-06-12 14:41:20.868524 de2_1-0.3.0/README.md
+-rw-r--r--   0        0        0     4860 1970-01-01 00:00:00.000000 de2_1-0.3.0/PKG-INFO
```

### Comparing `de2_1-0.2.6/de2_1/main.py` & `de2_1-0.3.0/de2_1/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,34 +71,30 @@
         - The input_array should be a 1D array, either a list or a 1D NumPy array.
         - The size represents the length of each window.
         - The shift determines the step size for moving the window starting position.
         - The stride determines the step size for moving the window elements.
         - If the window cannot fit entirely within the input_array, it is skipped.
         - The function returns a list of windows, where each window is either a list or a 1D NumPy array.
     """
-    if isinstance(input_array, np.ndarray):
-        array_type = np.ndarray
-    elif isinstance(input_array, list):
-        array_type = list
-    else:
+    if not isinstance(input_array, (list, np.ndarray)):
         raise TypeError("input_array must be a list or a 1D Numpy array")
 
     if size <= 0 or shift <= 0 or stride <= 0:
         raise ValueError("size, shift, and stride must be positive integers")
 
     if not isinstance(size, int) or not isinstance(shift, int) or not isinstance(stride, int):
-        raise ValueError("size, shcat ~/.ssh/id_ed25519.pubift, and stride must be integers")
+        raise ValueError("size, shift, and stride must be integers")
 
     result = []
     index = 0
     array_length = len(input_array)
 
     while index + size <= array_length:
-        window = input_array[index:index+size:stride]
-        result.append(array_type(window))
+        window = input_array[index:index+size]
+        result.append(window)
         index += shift
 
     return result
 
 def convolution2d(input_matrix: np.ndarray, kernel: np.ndarray, stride: int = 1) -> np.ndarray:
     """
     Perform 2D convolution on an input matrix using a given kernel.
@@ -131,25 +127,26 @@
     """
     
     input_shape = input_matrix.shape
     kernel_shape = kernel.shape
     if input_shape[0] < kernel_shape[0] or input_shape[1] < kernel_shape[1]:
         raise ValueError("Dimensions of the input matrix and kernel are incompatible.")
     
-    padding_rows = kernel_shape[0] - 1
-    padding_cols = kernel_shape[1] - 1
 
     output_rows = (input_shape[0] - kernel_shape[0]) // stride + 1
     output_cols = (input_shape[1] - kernel_shape[1]) // stride + 1
     
     output = np.zeros((output_rows, output_cols), dtype=np.float64)
     
     for i in range(output_rows):
         for j in range(output_cols):
-            window = input_matrix[
+            window = np.lib.stride_tricks.as_strided(input_matrix[
                 i * stride : i * stride + kernel_shape[0],
                 j * stride : j * stride + kernel_shape[1]
-            ].astype(np.float64)
+            ].astype(np.float64),
+            shape=kernel_shape)
 
             output[i, j] = np.sum(window * kernel)
     
     return output
+
+
```

### Comparing `de2_1-0.2.6/README.md` & `de2_1-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `de2_1-0.2.6/PKG-INFO` & `de2_1-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: de2-1
-Version: 0.2.6
-Summary: Turing college de2_1 sprint submission
+Version: 0.3.0
+Summary: Turing college de2_1 sprint submission. FINAl working version
 Author: JociusTa
 Author-email: tautvydasjocius@live.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
```

