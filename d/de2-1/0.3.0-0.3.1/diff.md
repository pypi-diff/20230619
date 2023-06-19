# Comparing `tmp/de2_1-0.3.0.tar.gz` & `tmp/de2_1-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "de2_1-0.3.0.tar", max compression
+gzip compressed data, was "de2_1-0.3.1.tar", max compression
```

## Comparing `de2_1-0.3.0.tar` & `de2_1-0.3.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-06-19 17:04:47.288696 de2_1-0.3.0/de2_1/__init__.py
--rw-r--r--   0        0        0     5968 2023-06-19 17:57:10.424231 de2_1-0.3.0/de2_1/main.py
--rw-r--r--   0        0        0      475 2023-06-19 17:57:54.628216 de2_1-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4535 2023-06-12 14:41:20.868524 de2_1-0.3.0/README.md
--rw-r--r--   0        0        0     4860 1970-01-01 00:00:00.000000 de2_1-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-19 17:04:47.288696 de2_1-0.3.1/de2_1/__init__.py
+-rw-r--r--   0        0        0     5400 2023-06-19 19:37:47.713720 de2_1-0.3.1/de2_1/main.py
+-rw-r--r--   0        0        0      475 2023-06-19 19:38:02.533557 de2_1-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4535 2023-06-12 14:41:20.868524 de2_1-0.3.1/README.md
+-rw-r--r--   0        0        0     4860 1970-01-01 00:00:00.000000 de2_1-0.3.1/PKG-INFO
```

### Comparing `de2_1-0.3.0/de2_1/main.py` & `de2_1-0.3.1/de2_1/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,24 +9,15 @@
     Args:
         input_matrix (List[List[float]]): The input matrix to be transposed.
             It is expected to be a 2D list of floats.
 
     Returns:
         List[List[float]]: The transposed matrix as a 2D list of floats.
 
-    Examples:
-        >>> input_matrix = [[1, 2, 3], [4, 5, 6]]
-        >>> result = transpose2d(input_matrix)
-        >>> print(result)
-        [[1, 4], [2, 5], [3, 6]]
-
-        >>> input_matrix = [[1, 2], [3, 4], [5, 6]]
-        >>> result = transpose2d(input_matrix)
-        >>> print(result)
-        [[1, 3, 5], [2, 4, 6]]
+
 
     Notes:
         - The input_matrix should be a 2D list of floats.
         - The function uses the `zip(*input_matrix)` expression to perform the transpose operation.
         - The rows of the input_matrix become the columns of the transposed matrix, and vice versa.
         - The resulting transposed matrix has dimensions (number of columns, number of rows) compared to the input matrix.
         - The function returns the transposed matrix as a 2D list of floats.
@@ -34,71 +25,63 @@
     return list(map(list, zip(*input_matrix)))
 
 def window1d(input_array: List | np.ndarray, size: int, shift: int = 1, stride: int = 1) -> List | np.ndarray:
     """
     Generate overlapping windows of a specified size from a 1D input array.
 
     Args:
-        input_array (Union[List, np.ndarray]): The 1D input array.
+        input_array List or np.ndarray The 1D input array.
         size (int): The size of the window.
         shift (int, optional): The shift value between windows. Default is 1.
         stride (int, optional): The stride value for moving the window. Default is 1.
 
     Returns:
-        List[Union[List, np.ndarray]]: A list of windows, where each window is either a list or a 1D NumPy array.
+        List or  np.ndarray: A list of windows, where each window is either a list or a 1D NumPy array.
 
     Raises:
         TypeError: If the input_array is not a list or a 1D NumPy array.
         ValueError: If the size, shift, or stride is not a positive integer.
 
-    Examples:
-        >>> input_array = [1, 2, 3, 4, 5, 6, 7, 8, 9]
-        >>> size = 3
-        >>> shift = 2
-        >>> stride = 1
-        >>> result = window1d(input_array, size, shift, stride)
-        >>> print(result)
-        [[1, 2, 3], [3, 4, 5], [5, 6, 7], [7, 8, 9]]
-
-        >>> input_array = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9])
-        >>> size = 4
-        >>> shift = 3
-        >>> stride = 2
-        >>> result = window1d(input_array, size, shift, stride)
-        >>> print(result)
-        [array([1, 2, 3, 4]), array([4, 5, 6, 7]), array([7, 8, 9])]
-
     Notes:
         - The input_array should be a 1D array, either a list or a 1D NumPy array.
         - The size represents the length of each window.
         - The shift determines the step size for moving the window starting position.
         - The stride determines the step size for moving the window elements.
         - If the window cannot fit entirely within the input_array, it is skipped.
         - The function returns a list of windows, where each window is either a list or a 1D NumPy array.
     """
-    if not isinstance(input_array, (list, np.ndarray)):
+    if isinstance(input_array, np.ndarray):
+        array_type = np.array
+    elif isinstance(input_array, list):
+        array_type = list
+    else:
         raise TypeError("input_array must be a list or a 1D Numpy array")
 
     if size <= 0 or shift <= 0 or stride <= 0:
         raise ValueError("size, shift, and stride must be positive integers")
 
     if not isinstance(size, int) or not isinstance(shift, int) or not isinstance(stride, int):
-        raise ValueError("size, shift, and stride must be integers")
+        raise ValueError("size, shcat ~/.ssh/id_ed25519.pubift, and stride must be integers")
+
+    if array_type == list : input_array = np.array(input_array)
 
-    result = []
-    index = 0
-    array_length = len(input_array)
-
-    while index + size <= array_length:
-        window = input_array[index:index+size]
-        result.append(window)
-        index += shift
+    n_records = len(input_array)
+    num_windows = (n_records - size) // shift + 1
 
+    new_view_structure = np.lib.stride_tricks.as_strided(
+        input_array,
+        shape=(num_windows, size),
+        strides=(input_array.itemsize * shift * stride, input_array.itemsize * stride),
+        writeable=False
+    )
+
+    result = [array_type(window) for window in new_view_structure]
     return result
 
+
 def convolution2d(input_matrix: np.ndarray, kernel: np.ndarray, stride: int = 1) -> np.ndarray:
     """
     Perform 2D convolution on an input matrix using a given kernel.
 
     Args:
         input_matrix (np.ndarray): The input matrix to convolve.
         kernel (np.ndarray): The convolution kernel.
```

### Comparing `de2_1-0.3.0/README.md` & `de2_1-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `de2_1-0.3.0/PKG-INFO` & `de2_1-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: de2-1
-Version: 0.3.0
+Version: 0.3.1
 Summary: Turing college de2_1 sprint submission. FINAl working version
 Author: JociusTa
 Author-email: tautvydasjocius@live.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
```

