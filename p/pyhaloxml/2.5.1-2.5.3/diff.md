# Comparing `tmp/pyhaloxml-2.5.1.tar.gz` & `tmp/pyhaloxml-2.5.3.tar.gz`

## Comparing `pyhaloxml-2.5.1.tar` & `pyhaloxml-2.5.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      426 1970-01-01 00:00:00.000000 pyhaloxml-2.5.1/Cargo.toml
--rw-r--r--   0     1001      122      169 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/.github/workflows/black.yml
--rw-r--r--   0     1001      122      507 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/.github/workflows/mypy.yml
--rw-r--r--   0     1001      122      543 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/.github/workflows/publish.yml
--rw-r--r--   0     1001      122      766 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/.github/workflows/pytest.yml
--rw-r--r--   0     1001      122      840 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/.github/workflows/wheels.yml
--rw-r--r--   0     1001      122     1859 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/.gitignore
--rw-r--r--   0     1001      122      245 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/.readthedocs.yaml
--rw-r--r--   0     1001      122    35149 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/LICENSE
--rw-r--r--   0     1001      122     1182 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/README.md
--rw-r--r--   0     1001      122      638 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/docs/Makefile
--rw-r--r--   0     1001      122      764 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/docs/make.bat
--rw-r--r--   0     1001      122      203 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/docs/source/api.rst
--rw-r--r--   0     1001      122      729 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/docs/source/conf.py
--rw-r--r--   0     1001      122      270 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/docs/source/index.rst
--rw-r--r--   0     1001      122      169 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/docs/source/usage.rst
--rw-r--r--   0     1001      122   348115 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/documentation/Indica Labs Annotation format.pdf
--rw-r--r--   0     1001      122    12329 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/exampledata/example.annotations
--rw-r--r--   0     1001      122   206619 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/exampledata/example_holes.annotations
--rw-r--r--   0     1001      122    70137 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/exampledata/multiple_holes.annotations
--rw-r--r--   0     1001      122    38870 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/exampledata/multiple_holes_new.geojson
--rw-r--r--   0     1001      122   176102 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/exampledata/qupath_test.geojson
--rw-r--r--   0     1001      122      950 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/examples/example1.py
--rw-r--r--   0     1001      122      805 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/examples/example2.py
--rw-r--r--   0     1001      122      349 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/examples/example3.py
--rw-r--r--   0     1001      122     1327 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/examples/example4.py
--rw-r--r--   0     1001      122     1887 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/pyproject.toml
--rw-r--r--   0     1001      122       41 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/requirements.txt
--rw-r--r--   0     1001      122     5800 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/src/pyhaloxml/HaloXML.py
--rw-r--r--   0     1001      122     1988 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/src/pyhaloxml/Layer.py
--rw-r--r--   0     1001      122     4743 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/src/pyhaloxml/Region.py
--rw-r--r--   0     1001      122      171 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/src/pyhaloxml/__init__.py
--rw-r--r--   0     1001      122      521 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/src/pyhaloxml/ellipse.py
--rw-r--r--   0     1001      122     2722 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/src/pyhaloxml/misc.py
--rw-r--r--   0     1001      122        0 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/src/pyhaloxml/py.typed
--rw-r--r--   0     1001      122      136 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/src/pyhaloxml/pyhaloxml_rs.pyi
--rw-r--r--   0     1001      122       60 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/src/pyhaloxml/shapely/__init__.py
--rw-r--r--   0     1001      122      891 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/src/pyhaloxml/shapely/to_shapely.py
--rw-r--r--   0     1001      122       22 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/src/pyhaloxml/version.py
--rw-r--r--   0     1001      122     1133 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/src/rust/lib.rs
--rw-r--r--   0     1001      122      454 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/tests/test_layers_and_regions.py
--rw-r--r--   0     1001      122     2748 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/tests/test_points_in_polygons.py
--rw-r--r--   0     1001      122      519 2023-03-13 12:19:48.000000 pyhaloxml-2.5.1/tests/testdata/test1.annotations
--rw-r--r--   0     1001      122     8084 2023-03-13 12:29:55.000000 pyhaloxml-2.5.1/Cargo.lock
--rw-r--r--   0        0        0     2129 1970-01-01 00:00:00.000000 pyhaloxml-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0      426 1970-01-01 00:00:00.000000 pyhaloxml-2.5.3/Cargo.toml
+-rw-r--r--   0     1001      122      169 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/.github/workflows/black.yml
+-rw-r--r--   0     1001      122      507 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/.github/workflows/mypy.yml
+-rw-r--r--   0     1001      122      543 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/.github/workflows/publish.yml
+-rw-r--r--   0     1001      122      766 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/.github/workflows/pytest.yml
+-rw-r--r--   0     1001      122      840 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/.github/workflows/wheels.yml
+-rw-r--r--   0     1001      122     1859 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/.gitignore
+-rw-r--r--   0     1001      122      245 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/.readthedocs.yaml
+-rw-r--r--   0     1001      122    35149 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/LICENSE
+-rw-r--r--   0     1001      122     1402 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/README.md
+-rw-r--r--   0     1001      122      638 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/docs/Makefile
+-rw-r--r--   0     1001      122      764 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/docs/make.bat
+-rw-r--r--   0     1001      122      203 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/docs/source/api.rst
+-rw-r--r--   0     1001      122      729 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/docs/source/conf.py
+-rw-r--r--   0     1001      122      270 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/docs/source/index.rst
+-rw-r--r--   0     1001      122      169 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/docs/source/usage.rst
+-rw-r--r--   0     1001      122   348115 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/documentation/Indica Labs Annotation format.pdf
+-rw-r--r--   0     1001      122    12329 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/exampledata/example.annotations
+-rw-r--r--   0     1001      122   206619 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/exampledata/example_holes.annotations
+-rw-r--r--   0     1001      122    70137 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/exampledata/multiple_holes.annotations
+-rw-r--r--   0     1001      122    38870 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/exampledata/multiple_holes_new.geojson
+-rw-r--r--   0     1001      122   176102 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/exampledata/qupath_test.geojson
+-rw-r--r--   0     1001      122      950 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/examples/example1.py
+-rw-r--r--   0     1001      122      805 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/examples/example2.py
+-rw-r--r--   0     1001      122      349 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/examples/example3.py
+-rw-r--r--   0     1001      122     1327 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/examples/example4.py
+-rw-r--r--   0     1001      122     1926 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/pyproject.toml
+-rw-r--r--   0     1001      122       41 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/requirements.txt
+-rw-r--r--   0     1001      122     6996 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/src/pyhaloxml/HaloXML.py
+-rw-r--r--   0     1001      122     1988 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/src/pyhaloxml/Layer.py
+-rw-r--r--   0     1001      122     4743 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/src/pyhaloxml/Region.py
+-rw-r--r--   0     1001      122      184 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/src/pyhaloxml/__init__.py
+-rw-r--r--   0     1001      122      521 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/src/pyhaloxml/ellipse.py
+-rw-r--r--   0     1001      122     2722 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/src/pyhaloxml/misc.py
+-rw-r--r--   0     1001      122        0 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/src/pyhaloxml/py.typed
+-rw-r--r--   0     1001      122      136 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/src/pyhaloxml/pyhaloxml_rs.pyi
+-rw-r--r--   0     1001      122       60 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/src/pyhaloxml/shapely/__init__.py
+-rw-r--r--   0     1001      122      891 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/src/pyhaloxml/shapely/to_shapely.py
+-rw-r--r--   0     1001      122       22 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/src/pyhaloxml/version.py
+-rw-r--r--   0     1001      122     1133 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/src/rust/lib.rs
+-rw-r--r--   0     1001      122      566 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/tests/test_layers_and_regions.py
+-rw-r--r--   0     1001      122     2748 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/tests/test_points_in_polygons.py
+-rw-r--r--   0     1001      122      519 2023-06-19 14:18:52.000000 pyhaloxml-2.5.3/tests/testdata/test1.annotations
+-rw-r--r--   0     1001      122     7853 2023-06-19 14:23:25.000000 pyhaloxml-2.5.3/Cargo.lock
+-rw-r--r--   0        0        0     2349 1970-01-01 00:00:00.000000 pyhaloxml-2.5.3/PKG-INFO
```

### Comparing `pyhaloxml-2.5.1/.github/workflows/publish.yml` & `pyhaloxml-2.5.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/.github/workflows/pytest.yml` & `pyhaloxml-2.5.3/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/.github/workflows/wheels.yml` & `pyhaloxml-2.5.3/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/.gitignore` & `pyhaloxml-2.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/LICENSE` & `pyhaloxml-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/README.md` & `pyhaloxml-2.5.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -12,7 +12,12 @@
 
 [Example 3](https://github.com/rharkes/pyhaloxml/blob/main/examples/example3.py) : Show the wkt representation of the shapely polygon.
 
 [Example 4](https://github.com/rharkes/pyhaloxml/blob/main/examples/example4.py) : Create a .annotation file from coordinates.
 
 # Installation
 `pip install pyhaloxml`
+
+# Loading speed
+Rust is used to match the negative regions to positive regions, thanks to [Wim Pomp](github.com/wimpomp/)!
+
+It takes 41 seconds to load a 30.9MB file with 856454 vertices in 5769 regions with 731 holes.
```

### Comparing `pyhaloxml-2.5.1/docs/Makefile` & `pyhaloxml-2.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/docs/make.bat` & `pyhaloxml-2.5.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/docs/source/conf.py` & `pyhaloxml-2.5.3/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import pyhaloxml
 
 # -- Project information
 project = "pyhaloxml"
 copyright = "2022, R.Harkes"
 author = "R.Harkes"
 
-release = "2.5.1"
-version = "2.5.1"
+release = "2.5.3"
+version = "2.5.3"
 
 # -- General configuration
 extensions = [
     "sphinx.ext.duration",
     "sphinx.ext.doctest",
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
```

### Comparing `pyhaloxml-2.5.1/documentation/Indica Labs Annotation format.pdf` & `pyhaloxml-2.5.3/documentation/Indica Labs Annotation format.pdf`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/exampledata/example.annotations` & `pyhaloxml-2.5.3/exampledata/example.annotations`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/exampledata/example_holes.annotations` & `pyhaloxml-2.5.3/exampledata/example_holes.annotations`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/exampledata/multiple_holes.annotations` & `pyhaloxml-2.5.3/exampledata/multiple_holes.annotations`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/exampledata/multiple_holes_new.geojson` & `pyhaloxml-2.5.3/exampledata/multiple_holes_new.geojson`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/exampledata/qupath_test.geojson` & `pyhaloxml-2.5.3/exampledata/qupath_test.geojson`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/examples/example1.py` & `pyhaloxml-2.5.3/examples/example1.py`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/examples/example2.py` & `pyhaloxml-2.5.3/examples/example2.py`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/examples/example4.py` & `pyhaloxml-2.5.3/examples/example4.py`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/pyproject.toml` & `pyhaloxml-2.5.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "pyhaloxml"
-version = "2.5.1"
+version = "2.5.3"
 description = "Read and write the annotation files from Halo"
 readme = "README.md"
 authors = [{ name = "Rolf Harkes", email = "r.harkes@nki.nl" }]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -24,15 +24,15 @@
 shapely = ["shapely"]
 dev = ["black", "bumpver", "pytest", "mypy", "setuptools", "build", "twine"]
 
 [project.urls]
 Homepage = "https://github.com/rharkes/pyhaloxml"
 
 [tool.bumpver]
-current_version = "2.5.1"
+current_version = "2.5.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
@@ -73,13 +73,14 @@
 
 [[tool.mypy.overrides]]
 module = "shapely.*"
 ignore_missing_imports  = true
 
 [tool.maturin]
 python-source = "src"
+module-name = "pyhaloxml.pyhaloxml_rs"
 
 [tool.cibuildwheel]
 before-all = "curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y"
 environment = "PATH=$PATH:/root/.cargo/bin"
 build = "cp310-*"
 skip = "*-musllinux_i686"
```

### Comparing `pyhaloxml-2.5.1/src/pyhaloxml/Layer.py` & `pyhaloxml-2.5.3/src/pyhaloxml/Layer.py`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/src/pyhaloxml/Region.py` & `pyhaloxml-2.5.3/src/pyhaloxml/Region.py`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/src/pyhaloxml/ellipse.py` & `pyhaloxml-2.5.3/src/pyhaloxml/ellipse.py`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/src/pyhaloxml/misc.py` & `pyhaloxml-2.5.3/src/pyhaloxml/misc.py`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/src/pyhaloxml/shapely/to_shapely.py` & `pyhaloxml-2.5.3/src/pyhaloxml/shapely/to_shapely.py`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/src/rust/lib.rs` & `pyhaloxml-2.5.3/src/rust/lib.rs`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/tests/test_points_in_polygons.py` & `pyhaloxml-2.5.3/tests/test_points_in_polygons.py`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/tests/testdata/test1.annotations` & `pyhaloxml-2.5.3/tests/testdata/test1.annotations`

 * *Files identical despite different names*

### Comparing `pyhaloxml-2.5.1/Cargo.lock` & `pyhaloxml-2.5.3/Cargo.lock`

 * *Files 11% similar despite different names*

```diff
@@ -30,23 +30,23 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
@@ -55,141 +55,141 @@
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.52"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d0e1ae9e836cc3beddd63db0df682593d7e2d3d891ae8c9083d2113e1744224"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyhaloxml_rs"
 version = "0.1.0"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "python3-dll-a",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "python3-dll-a"
-version = "0.2.6"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a915bd72824962bf190bbd3e8a044cccb695d1409f73ff5493712eda5136c7a8"
+checksum = "212d74540270e3a22eed5f0d4bbc0765dff20958d694e9d4f5ebe6e22778c422"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.24"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50686e0021c4136d1d453b2dfe059902278681512a34d4248435dc34b6b5c8ec"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
@@ -211,88 +211,79 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
-name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets",
-]
-
-[[package]]
 name = "windows-targets"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e2522491fbfcd58cc84d47aeb2958948c4b8982e9a2d8a2a35bbaed431390e7"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `pyhaloxml-2.5.1/PKG-INFO` & `pyhaloxml-2.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhaloxml
-Version: 2.5.1
+Version: 2.5.3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: lxml >= 4.9
 Requires-Dist: geojson>=2.5
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: bumpver; extra == 'dev'
@@ -39,7 +39,12 @@
 [Example 3](https://github.com/rharkes/pyhaloxml/blob/main/examples/example3.py) : Show the wkt representation of the shapely polygon.
 
 [Example 4](https://github.com/rharkes/pyhaloxml/blob/main/examples/example4.py) : Create a .annotation file from coordinates.
 
 # Installation
 `pip install pyhaloxml`
 
+# Loading speed
+Rust is used to match the negative regions to positive regions, thanks to [Wim Pomp](github.com/wimpomp/)!
+
+It takes 41 seconds to load a 30.9MB file with 856454 vertices in 5769 regions with 731 holes.
+
```

