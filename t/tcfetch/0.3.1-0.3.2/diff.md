# Comparing `tmp/tcfetch-0.3.1.tar.gz` & `tmp/tcfetch-0.3.2.tar.gz`

## Comparing `tcfetch-0.3.1.tar` & `tcfetch-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/Cargo.toml
--rw-r--r--   0     1001      123     2459 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/.github/workflows/python.yml
--rw-r--r--   0     1001      123       49 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/.gitignore
--rw-r--r--   0     1001      123     1500 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/LICENSE.md
--rw-r--r--   0     1001      123     1709 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/README.md
--rw-r--r--   0     1001      123       10 2023-06-13 07:18:12.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/dist/tcfetch-0.3.1.tar.gz
--rw-r--r--   0     1001      123     4269 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/src/gh.rs
--rw-r--r--   0     1001      123     1614 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/src/ghwpt.rs
--rw-r--r--   0     1001      123     3141 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/src/hgmo.rs
--rw-r--r--   0     1001      123     5390 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/src/lib.rs
--rw-r--r--   0     1001      123     3038 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/src/main.rs
--rw-r--r--   0     1001      123     5270 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/src/taskcluster.rs
--rw-r--r--   0     1001      123     1417 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/src/utils.rs
--rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 tcfetch-0.3.1/Cargo.toml
--rw-r--r--   0     1001      123     2807 2023-06-13 07:16:01.000000 tcfetch-0.3.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-06-13 07:16:01.000000 tcfetch-0.3.1/.gitignore
--rw-r--r--   0     1001      123      537 2023-06-13 07:16:01.000000 tcfetch-0.3.1/pyproject.toml
--rw-r--r--   0     1001      123     2139 2023-06-13 07:16:01.000000 tcfetch-0.3.1/src/lib.rs
--rw-r--r--   0     1001      123    33086 2023-06-13 07:18:10.000000 tcfetch-0.3.1/Cargo.lock
--rw-r--r--   0        0        0      334 1970-01-01 00:00:00.000000 tcfetch-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 tcfetch-0.3.2/local_dependencies/tc-fetch/Cargo.toml
+-rw-r--r--   0     1001      123     2459 2023-06-19 11:45:52.000000 tcfetch-0.3.2/local_dependencies/tc-fetch/.github/workflows/python.yml
+-rw-r--r--   0     1001      123       49 2023-06-19 11:45:52.000000 tcfetch-0.3.2/local_dependencies/tc-fetch/.gitignore
+-rw-r--r--   0     1001      123     1500 2023-06-19 11:45:52.000000 tcfetch-0.3.2/local_dependencies/tc-fetch/LICENSE.md
+-rw-r--r--   0     1001      123     1709 2023-06-19 11:45:52.000000 tcfetch-0.3.2/local_dependencies/tc-fetch/README.md
+-rw-r--r--   0     1001      123       10 2023-06-19 11:46:00.000000 tcfetch-0.3.2/local_dependencies/tc-fetch/dist/tcfetch-0.3.2.tar.gz
+-rw-r--r--   0     1001      123     4340 2023-06-19 11:45:52.000000 tcfetch-0.3.2/local_dependencies/tc-fetch/src/gh.rs
+-rw-r--r--   0     1001      123     1614 2023-06-19 11:45:52.000000 tcfetch-0.3.2/local_dependencies/tc-fetch/src/ghwpt.rs
+-rw-r--r--   0     1001      123     3141 2023-06-19 11:45:52.000000 tcfetch-0.3.2/local_dependencies/tc-fetch/src/hgmo.rs
+-rw-r--r--   0     1001      123     5390 2023-06-19 11:45:52.000000 tcfetch-0.3.2/local_dependencies/tc-fetch/src/lib.rs
+-rw-r--r--   0     1001      123     3038 2023-06-19 11:45:52.000000 tcfetch-0.3.2/local_dependencies/tc-fetch/src/main.rs
+-rw-r--r--   0     1001      123     5270 2023-06-19 11:45:52.000000 tcfetch-0.3.2/local_dependencies/tc-fetch/src/taskcluster.rs
+-rw-r--r--   0     1001      123     1417 2023-06-19 11:45:52.000000 tcfetch-0.3.2/local_dependencies/tc-fetch/src/utils.rs
+-rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 tcfetch-0.3.2/Cargo.toml
+-rw-r--r--   0     1001      123     2807 2023-06-19 11:45:52.000000 tcfetch-0.3.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-06-19 11:45:52.000000 tcfetch-0.3.2/.gitignore
+-rw-r--r--   0     1001      123      537 2023-06-19 11:45:52.000000 tcfetch-0.3.2/pyproject.toml
+-rw-r--r--   0     1001      123     2139 2023-06-19 11:45:52.000000 tcfetch-0.3.2/src/lib.rs
+-rw-r--r--   0     1001      123    33078 2023-06-19 11:45:58.000000 tcfetch-0.3.2/Cargo.lock
+-rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 tcfetch-0.3.2/PKG-INFO
```

### Comparing `tcfetch-0.3.1/local_dependencies/tc-fetch/Cargo.toml` & `tcfetch-0.3.2/local_dependencies/tc-fetch/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "tc-fetch"
-version = "0.3.1"
+version = "0.3.2"
 authors = ["James Graham <james@hoppipolla.co.uk>"]
 description="Download taskcluster artifacts"
 readme = "README.md"
 edition = "2021"
 license = "BSD-3-Clause"
 
 [lib]
```

### Comparing `tcfetch-0.3.1/local_dependencies/tc-fetch/.github/workflows/python.yml` & `tcfetch-0.3.2/local_dependencies/tc-fetch/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `tcfetch-0.3.1/local_dependencies/tc-fetch/LICENSE.md` & `tcfetch-0.3.2/local_dependencies/tc-fetch/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tcfetch-0.3.1/local_dependencies/tc-fetch/README.md` & `tcfetch-0.3.2/local_dependencies/tc-fetch/README.md`

 * *Files identical despite different names*

### Comparing `tcfetch-0.3.1/local_dependencies/tc-fetch/src/gh.rs` & `tcfetch-0.3.2/local_dependencies/tc-fetch/src/gh.rs`

 * *Files 0% similar despite different names*

```diff
@@ -154,14 +154,15 @@
             None
         };
         let checks_resp: ChecksResponse = get_json(
             client,
             base_url,
             query,
             Some(vec![
+                ("user-agent".to_string(), "tcfetch/0.3".to_string()),
                 (
                     "Accept".to_string(),
                     "application/vnd.github+json".to_string(),
                 ),
                 ("X-GitHub-Api-Version".to_string(), "2022-11-28".to_string()),
             ]),
         )?;
```

### Comparing `tcfetch-0.3.1/local_dependencies/tc-fetch/src/ghwpt.rs` & `tcfetch-0.3.2/local_dependencies/tc-fetch/src/ghwpt.rs`

 * *Files identical despite different names*

### Comparing `tcfetch-0.3.1/local_dependencies/tc-fetch/src/hgmo.rs` & `tcfetch-0.3.2/local_dependencies/tc-fetch/src/hgmo.rs`

 * *Files identical despite different names*

### Comparing `tcfetch-0.3.1/local_dependencies/tc-fetch/src/lib.rs` & `tcfetch-0.3.2/local_dependencies/tc-fetch/src/lib.rs`

 * *Files identical despite different names*

### Comparing `tcfetch-0.3.1/local_dependencies/tc-fetch/src/main.rs` & `tcfetch-0.3.2/local_dependencies/tc-fetch/src/main.rs`

 * *Files identical despite different names*

### Comparing `tcfetch-0.3.1/local_dependencies/tc-fetch/src/taskcluster.rs` & `tcfetch-0.3.2/local_dependencies/tc-fetch/src/taskcluster.rs`

 * *Files identical despite different names*

### Comparing `tcfetch-0.3.1/local_dependencies/tc-fetch/src/utils.rs` & `tcfetch-0.3.2/local_dependencies/tc-fetch/src/utils.rs`

 * *Files identical despite different names*

### Comparing `tcfetch-0.3.1/.github/workflows/CI.yml` & `tcfetch-0.3.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `tcfetch-0.3.1/.gitignore` & `tcfetch-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tcfetch-0.3.1/pyproject.toml` & `tcfetch-0.3.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "tcfetch"
 description = "Download log files from Taskcluster CI systems"
 author = "James Graham"
 author_email = "james@hoppipolla.co.uk"
 license = "BSD-3-Clause"
-version = "0.3.1"
+version = "0.3.2"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
```

### Comparing `tcfetch-0.3.1/src/lib.rs` & `tcfetch-0.3.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `tcfetch-0.3.1/Cargo.lock` & `tcfetch-0.3.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -119,26 +119,26 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "clap"
-version = "4.3.3"
+version = "4.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca8f255e4b8027970e78db75e78831229c9815fdbfa67eb1a1b777a62e24b4a0"
+checksum = "80672091db20273a15cf9fdd4e47ed43b5091ec9841bf4c6145c9dfbbcae09ed"
 dependencies = [
  "clap_builder",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.3"
+version = "4.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acd4f3c17c83b0ba34ffbc4f8bbd74f079413f747f84a6f89292f138057e36ab"
+checksum = "c1458a1df40e1e2afebb7ab60ce55c1fa8f431146205aa5f4887e0b111c27636"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex",
  "strsim",
 ]
@@ -746,17 +746,17 @@
  "libc",
  "linux-raw-sys",
  "windows-sys",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c911ba11bc8433e811ce56fde130ccf32f5127cab0e0194e9c68c5a5b671791e"
+checksum = "e32ca28af694bc1bbf399c33a516dbdf1c90090b8ab23c2bc24f834aa2247f5f"
 dependencies = [
  "log",
  "ring",
  "rustls-webpki",
  "sct",
 ]
 
@@ -822,17 +822,17 @@
  "proc-macro2",
  "quote",
  "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.96"
+version = "1.0.97"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
+checksum = "bdf3bf93142acad5821c99197022e170842cdbc1c30482b98750c688c640842a"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -910,15 +910,15 @@
 name = "target-lexicon"
 version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tc-fetch"
-version = "0.3.1"
+version = "0.3.2"
 dependencies = [
  "clap",
  "regex",
  "reqwest",
  "scoped_threadpool",
  "serde",
  "serde_derive",
@@ -1089,19 +1089,18 @@
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "want"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ce8a968cb1cd110d136ff8b819a556d6fb6d919363c61534f6860c7eb172ba0"
+checksum = "bfa7760aed19e106de2c7c0b581b509f2f25d3dacaf737cb82ac61bc6d760b0e"
 dependencies = [
- "log",
  "try-lock",
 ]
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
```

