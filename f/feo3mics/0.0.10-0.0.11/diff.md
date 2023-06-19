# Comparing `tmp/feo3mics-0.0.10.tar.gz` & `tmp/feo3mics-0.0.11.tar.gz`

## Comparing `feo3mics-0.0.10.tar` & `feo3mics-0.0.11.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0      310 1970-01-01 00:00:00.000000 feo3mics-0.0.10/Cargo.toml
--rw-r--r--   0     1001      123     1506 2023-06-19 00:06:26.000000 feo3mics-0.0.10/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-06-19 00:06:26.000000 feo3mics-0.0.10/.gitignore
--rw-r--r--   0     1001      123      130 2023-06-19 00:06:26.000000 feo3mics-0.0.10/README.md
--rw-r--r--   0     1001      123     5175 2023-06-19 00:06:26.000000 feo3mics-0.0.10/feo3mics.pyi
--rw-r--r--   0     1001      123      339 2023-06-19 00:06:26.000000 feo3mics-0.0.10/pyproject.toml
--rwxr-xr-x   0     1001      123      833 2023-06-19 00:07:00.000000 feo3mics-0.0.10/run-maturin-action.sh
--rw-r--r--   0     1001      123     4286 2023-06-19 00:06:26.000000 feo3mics-0.0.10/src/exposure.rs
--rw-r--r--   0     1001      123      266 2023-06-19 00:06:26.000000 feo3mics-0.0.10/src/lib.rs
--rw-r--r--   0     1001      123     7422 2023-06-19 00:06:26.000000 feo3mics-0.0.10/Cargo.lock
--rw-r--r--   0        0        0      458 1970-01-01 00:00:00.000000 feo3mics-0.0.10/PKG-INFO
+-rw-r--r--   0        0        0      310 1970-01-01 00:00:00.000000 feo3mics-0.0.11/Cargo.toml
+-rw-r--r--   0     1001      123     1506 2023-06-19 00:54:33.000000 feo3mics-0.0.11/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-06-19 00:54:33.000000 feo3mics-0.0.11/.gitignore
+-rw-r--r--   0     1001      123     3996 2023-06-19 00:54:33.000000 feo3mics-0.0.11/DOCS.md
+-rw-r--r--   0     1001      123     1065 2023-06-19 00:54:33.000000 feo3mics-0.0.11/LICENSE
+-rw-r--r--   0     1001      123     1871 2023-06-19 00:54:33.000000 feo3mics-0.0.11/README.md
+-rw-r--r--   0     1001      123     5163 2023-06-19 00:54:33.000000 feo3mics-0.0.11/feo3mics.pyi
+-rw-r--r--   0     1001      123      339 2023-06-19 00:54:33.000000 feo3mics-0.0.11/pyproject.toml
+-rwxr-xr-x   0     1001      123      833 2023-06-19 00:55:04.000000 feo3mics-0.0.11/run-maturin-action.sh
+-rw-r--r--   0     1001      123     4274 2023-06-19 00:54:33.000000 feo3mics-0.0.11/src/exposure.rs
+-rw-r--r--   0     1001      123      266 2023-06-19 00:54:33.000000 feo3mics-0.0.11/src/lib.rs
+-rw-r--r--   0     1001      123     7422 2023-06-19 00:54:33.000000 feo3mics-0.0.11/Cargo.lock
+-rw-r--r--   0        0        0     2221 1970-01-01 00:00:00.000000 feo3mics-0.0.11/PKG-INFO
```

### Comparing `feo3mics-0.0.10/.github/workflows/CI.yml` & `feo3mics-0.0.11/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `feo3mics-0.0.10/.gitignore` & `feo3mics-0.0.11/.gitignore`

 * *Files identical despite different names*

### Comparing `feo3mics-0.0.10/feo3mics.pyi` & `feo3mics-0.0.11/feo3mics.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -81,27 +81,27 @@
 
         Returns:
             A tuple containing a boolean indicating if the swap was successful,
             and the previous value of the atomic integer.
         """
         ...
 
-    def fetch_mul(self, value: int) -> int:
+    def mul(self, value: int) -> int:
         """
         Atomically multiplies the atomic integer by the given value and returns the previous value.
 
         Args:
             value: The value to multiply with the atomic integer.
 
         Returns:
             The previous value of the atomic integer.
         """
         ...
 
-    def fetch_div(self, value: int) -> int:
+    def div(self, value: int) -> int:
         """
         Atomically divides the atomic integer by the given value and returns the result.
 
         Args:
             value: The value to divide the atomic integer by.
 
         Returns:
```

### Comparing `feo3mics-0.0.10/run-maturin-action.sh` & `feo3mics-0.0.11/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `feo3mics-0.0.10/src/exposure.rs` & `feo3mics-0.0.11/src/exposure.rs`

 * *Files 2% similar despite different names*

```diff
@@ -43,21 +43,21 @@
             match r {
                 Ok(v) => v,
                 Err(v) => v,
             },
         )
     }
 
-    pub fn fetch_mul(&self, value: i64) -> i64 {
+    pub fn mul(&self, value: i64) -> i64 {
         self.value
             .fetch_update(SeqCst, SeqCst, |v| Some(v * value))
             .unwrap()
     }
 
-    pub fn fetch_div(&self, value: i64) -> PyResult<i64> {
+    pub fn div(&self, value: i64) -> PyResult<i64> {
         let r = self
             .value
             .fetch_update(SeqCst, SeqCst, |v| v.checked_div(value));
         match r {
             Ok(v) => Ok(v),
             Err(_) => Err(PyErr::new::<pyo3::exceptions::PyZeroDivisionError, _>(
                 "division by zero",
```

### Comparing `feo3mics-0.0.10/Cargo.lock` & `feo3mics-0.0.11/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "feo3mics"
-version = "0.0.10"
+version = "0.0.11"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
```

