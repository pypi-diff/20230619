# Comparing `tmp/hmmer_tables-0.1.1.tar.gz` & `tmp/hmmer_tables-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmmer_tables-0.1.1.tar", max compression
+gzip compressed data, was "hmmer_tables-0.1.2.tar", max compression
```

## Comparing `hmmer_tables-0.1.1.tar` & `hmmer_tables-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1063 2023-06-12 15:39:46.426268 hmmer_tables-0.1.1/LICENSE
--rw-r--r--   0        0        0       15 2023-06-12 15:39:46.427467 hmmer_tables-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-12 15:39:56.207600 hmmer_tables-0.1.1/hmmer_tables/__init__.py
--rw-r--r--   0        0        0      319 2023-06-12 15:39:56.208378 hmmer_tables-0.1.1/hmmer_tables/csv_iter.py
--rw-r--r--   0        0        0     3038 2023-06-12 15:49:25.111691 hmmer_tables-0.1.1/hmmer_tables/domtbl.py
--rw-r--r--   0        0        0     1866 2023-06-12 15:39:56.206656 hmmer_tables-0.1.1/hmmer_tables/interval.py
--rw-r--r--   0        0        0       72 2023-06-12 15:39:56.205996 hmmer_tables-0.1.1/hmmer_tables/path_like.py
--rw-r--r--   0        0        0     1747 2023-06-12 15:51:43.511951 hmmer_tables-0.1.1/hmmer_tables/tbl.py
--rw-r--r--   0        0        0      468 2023-06-12 15:52:49.194535 hmmer_tables-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 hmmer_tables-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-19 10:44:39.025516 hmmer_tables-0.1.2/LICENSE
+-rw-r--r--   0        0        0       15 2023-06-19 10:44:39.025516 hmmer_tables-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-19 10:44:39.025516 hmmer_tables-0.1.2/hmmer_tables/__init__.py
+-rw-r--r--   0        0        0      319 2023-06-19 10:44:39.025516 hmmer_tables-0.1.2/hmmer_tables/csv_iter.py
+-rw-r--r--   0        0        0     3038 2023-06-19 10:44:39.025516 hmmer_tables-0.1.2/hmmer_tables/domtbl.py
+-rw-r--r--   0        0        0     1885 2023-06-19 10:44:39.025516 hmmer_tables-0.1.2/hmmer_tables/interval.py
+-rw-r--r--   0        0        0       72 2023-06-19 10:44:39.025516 hmmer_tables-0.1.2/hmmer_tables/path_like.py
+-rw-r--r--   0        0        0     1747 2023-06-19 10:44:39.025516 hmmer_tables-0.1.2/hmmer_tables/tbl.py
+-rw-r--r--   0        0        0      442 2023-06-19 10:44:39.025516 hmmer_tables-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 hmmer_tables-0.1.2/PKG-INFO
```

### Comparing `hmmer_tables-0.1.1/LICENSE` & `hmmer_tables-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hmmer_tables-0.1.1/hmmer_tables/domtbl.py` & `hmmer_tables-0.1.2/hmmer_tables/domtbl.py`

 * *Files identical despite different names*

### Comparing `hmmer_tables-0.1.1/hmmer_tables/interval.py` & `hmmer_tables-0.1.2/hmmer_tables/interval.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,61 +8,61 @@
 @dataclass(frozen=True)
 class PyInterval:
     """
     Python interval.
 
     A Python interval is an 0-start, half-open interval. It means that:
     - The elements of a sequence have the coordinates `0, 1, 2, ...`.
-    - An interval `PyInterval(start, end)` is defined by the coordinates
-      `start, start+1, ..., end-2, end-1`.
+    - An interval `PyInterval(start, stop)` is defined by the coordinates
+      `start, start+1, ..., stop-2, stop-1`.
 
     Attributes
     ----------
     start
-        Start of interval. Valid values are `0, 1, ..., end`.
-    end
+        Start of interval. Valid values are `0, 1, ..., stop`.
+    stop
         End of interval. Valid values are `start, start+1, ...`.
     """
 
     start: int
-    end: int
+    stop: int
 
     def __post_init__(self):
-        if self.start > self.end:
-            raise ValueError(f"Invalid PyInterval({self.start}, {self.end}).")
+        if self.start > self.stop:
+            raise ValueError(f"Invalid PyInterval({self.start}, {self.stop}).")
 
     def to_rinterval(self) -> RInterval:
-        return RInterval(self.start + 1, self.end)
+        return RInterval(self.start + 1, self.stop)
 
     def to_slice(self) -> slice:
-        return slice(self.start, self.end)
+        return slice(self.start, self.stop)
 
     def offset(self, offset: int) -> PyInterval:
-        return PyInterval(self.start + offset, self.end + offset)
+        return PyInterval(self.start + offset, self.stop + offset)
 
 
 @dataclass(frozen=True)
 class RInterval:
     """
     R interval.
 
     An R interval is an 1-start, fully-closed. It means that:
     - The elements of a sequence have the coordinates `1, 2, 3, ...`.
-    - An interval `RInterval(start, end)` is defined by the coordinates
-      `start, start+1, ..., end-1, end`.
+    - An interval `RInterval(start, stop)` is defined by the coordinates
+      `start, start+1, ..., stop-1, stop`.
     """
 
     start: int
-    end: int
+    stop: int
 
     def __post_init__(self):
-        if self.start > self.end:
-            raise ValueError(f"Invalid RInterval({self.start}, {self.end}).")
+        if self.start > self.stop:
+            raise ValueError(f"Invalid RInterval({self.start}, {self.stop}).")
 
     def to_pyinterval(self) -> PyInterval:
-        return PyInterval(self.start - 1, self.end)
+        return PyInterval(self.start - 1, self.stop)
 
     def to_slice(self) -> slice:
         return self.to_pyinterval().to_slice()
 
     def offset(self, offset: int) -> RInterval:
-        return RInterval(self.start + offset, self.end + offset)
+        return RInterval(self.start + offset, self.stop + offset)
```

### Comparing `hmmer_tables-0.1.1/hmmer_tables/tbl.py` & `hmmer_tables-0.1.2/hmmer_tables/tbl.py`

 * *Files identical despite different names*

### Comparing `hmmer_tables-0.1.1/PKG-INFO` & `hmmer_tables-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmmer-tables
-Version: 0.1.1
+Version: 0.1.2
 Summary: Read tables produced by HMMER software.
 License: MIT
 Author: Danilo Horta
 Author-email: horta@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

