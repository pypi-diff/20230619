# Comparing `tmp/feo3mics-0.0.11.tar.gz` & `tmp/feo3mics-0.0.12.tar.gz`

## Comparing `feo3mics-0.0.11.tar` & `feo3mics-0.0.12.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      310 1970-01-01 00:00:00.000000 feo3mics-0.0.11/Cargo.toml
--rw-r--r--   0     1001      123     1506 2023-06-19 00:54:33.000000 feo3mics-0.0.11/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-06-19 00:54:33.000000 feo3mics-0.0.11/.gitignore
--rw-r--r--   0     1001      123     3996 2023-06-19 00:54:33.000000 feo3mics-0.0.11/DOCS.md
--rw-r--r--   0     1001      123     1065 2023-06-19 00:54:33.000000 feo3mics-0.0.11/LICENSE
--rw-r--r--   0     1001      123     1871 2023-06-19 00:54:33.000000 feo3mics-0.0.11/README.md
--rw-r--r--   0     1001      123     5163 2023-06-19 00:54:33.000000 feo3mics-0.0.11/feo3mics.pyi
--rw-r--r--   0     1001      123      339 2023-06-19 00:54:33.000000 feo3mics-0.0.11/pyproject.toml
--rwxr-xr-x   0     1001      123      833 2023-06-19 00:55:04.000000 feo3mics-0.0.11/run-maturin-action.sh
--rw-r--r--   0     1001      123     4274 2023-06-19 00:54:33.000000 feo3mics-0.0.11/src/exposure.rs
--rw-r--r--   0     1001      123      266 2023-06-19 00:54:33.000000 feo3mics-0.0.11/src/lib.rs
--rw-r--r--   0     1001      123     7422 2023-06-19 00:54:33.000000 feo3mics-0.0.11/Cargo.lock
--rw-r--r--   0        0        0     2221 1970-01-01 00:00:00.000000 feo3mics-0.0.11/PKG-INFO
+-rw-r--r--   0        0        0      310 1970-01-01 00:00:00.000000 feo3mics-0.0.12/Cargo.toml
+-rw-r--r--   0     1001      123     1506 2023-06-19 01:36:57.000000 feo3mics-0.0.12/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-06-19 01:36:57.000000 feo3mics-0.0.12/.gitignore
+-rw-r--r--   0     1001      123     3996 2023-06-19 01:36:57.000000 feo3mics-0.0.12/DOCS.md
+-rw-r--r--   0     1001      123     1065 2023-06-19 01:36:57.000000 feo3mics-0.0.12/LICENSE
+-rw-r--r--   0     1001      123     1871 2023-06-19 01:36:57.000000 feo3mics-0.0.12/README.md
+-rw-r--r--   0     1001      123     5990 2023-06-19 01:36:57.000000 feo3mics-0.0.12/feo3mics.pyi
+-rw-r--r--   0     1001      123      804 2023-06-19 01:36:57.000000 feo3mics-0.0.12/pyproject.toml
+-rwxr-xr-x   0     1001      123      833 2023-06-19 01:37:28.000000 feo3mics-0.0.12/run-maturin-action.sh
+-rw-r--r--   0     1001      123     4274 2023-06-19 01:36:57.000000 feo3mics-0.0.12/src/exposure.rs
+-rw-r--r--   0     1001      123      266 2023-06-19 01:36:57.000000 feo3mics-0.0.12/src/lib.rs
+-rw-r--r--   0     1001      123     7422 2023-06-19 01:36:57.000000 feo3mics-0.0.12/Cargo.lock
+-rw-r--r--   0        0        0     2680 1970-01-01 00:00:00.000000 feo3mics-0.0.12/PKG-INFO
```

### Comparing `feo3mics-0.0.11/.github/workflows/CI.yml` & `feo3mics-0.0.12/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `feo3mics-0.0.11/.gitignore` & `feo3mics-0.0.12/.gitignore`

 * *Files identical despite different names*

### Comparing `feo3mics-0.0.11/DOCS.md` & `feo3mics-0.0.12/DOCS.md`

 * *Files identical despite different names*

### Comparing `feo3mics-0.0.11/LICENSE` & `feo3mics-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `feo3mics-0.0.11/README.md` & `feo3mics-0.0.12/README.md`

 * *Files identical despite different names*

### Comparing `feo3mics-0.0.11/feo3mics.pyi` & `feo3mics-0.0.12/feo3mics.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+"""
+feo3mics is an easy-to-use atomics library for Python, providing atomic integer and boolean operations for thread-safe programming.
+
+The package includes two main classes: `AtomicInt` and `AtomicBool`, which allow you to perform atomic operations on shared variables, ensuring thread-safety and preventing race conditions in concurrent programming.
+
+- `AtomicInt` provides atomic operations such as load, store, add, subtract, swap, compare and exchange, multiply, divide, increment, and decrement for integer variables.
+- `AtomicBool` provides atomic operations such as load, store, swap, compare and exchange, and flip for boolean variables.
+
+The atomic operations provided by feo3mics are implemented using synchronization primitives from the `std::sync::atomic` module in Rust, making them efficient and reliable.
+"""
+
 from typing import Any, Callable, Generic, Optional, Tuple, TypeVar
 class AtomicInt:
     """
     Represents an atomic signed integer of 64 bits. Unsigned or other widths are not supported for simplicity.
     """
 
     def __init__(self, value: int = 0) -> 'AtomicInt':
```

### Comparing `feo3mics-0.0.11/run-maturin-action.sh` & `feo3mics-0.0.12/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `feo3mics-0.0.11/src/exposure.rs` & `feo3mics-0.0.12/src/exposure.rs`

 * *Files identical despite different names*

### Comparing `feo3mics-0.0.11/Cargo.lock` & `feo3mics-0.0.12/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "feo3mics"
-version = "0.0.11"
+version = "0.0.12"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
```

### Comparing `feo3mics-0.0.11/PKG-INFO` & `feo3mics-0.0.12/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 Metadata-Version: 2.1
 Name: feo3mics
-Version: 0.0.11
+Version: 0.0.12
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Utilities
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Typing :: Typed
 License-File: LICENSE
+Summary: easy-to-use atomic integer and boolean operations for thread-safe programming
+Author-email: RuneBlaze <liubaqiao@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Homepage, https://github.com/RuneBlaze/feo3mics
+Project-URL: Bug Tracker, https://github.com/RuneBlaze/feo3mics/issues
+Project-URL: Documentation, https://github.com/RuneBlaze/feo3mics/blob/main/DOCS.md
 
 # feo3mics
 
 [![PyPI version](https://badge.fury.io/py/feo3mics.svg)](https://badge.fury.io/py/feo3mics)
 
 feo3mics is an easy-to-use atomics library for Python, providing atomic integer and boolean operations. It allows you to perform atomic operations on shared variables, ensuring thread-safety and preventing race conditions in concurrent programming. Everything is entirely lock-free and is backed by Rust's atomic types.
```

