# Comparing `tmp/pydistcheck-0.4.0.tar.gz` & `tmp/pydistcheck-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydistcheck-0.4.0.tar", last modified: Sun Apr 30 02:48:36 2023, max compression
+gzip compressed data, was "pydistcheck-0.5.0.tar", last modified: Mon Jun 19 06:23:41 2023, max compression
```

## Comparing `pydistcheck-0.4.0.tar` & `pydistcheck-0.5.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:48:36.468651 pydistcheck-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:48:36.464651 pydistcheck-0.4.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/LICENSES/DELOCATE_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-30 02:48:36.468651 pydistcheck-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-30 02:48:36.468651 pydistcheck-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:48:36.464651 pydistcheck-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:48:36.464651 pydistcheck-0.4.0/src/pydistcheck/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/src/pydistcheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/src/pydistcheck/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/src/pydistcheck/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/src/pydistcheck/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/src/pydistcheck/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/src/pydistcheck/distribution_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/src/pydistcheck/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/src/pydistcheck/shared_lib_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/src/pydistcheck/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:48:36.464651 pydistcheck-0.4.0/src/pydistcheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-30 02:48:36.000000 pydistcheck-0.4.0/src/pydistcheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-30 02:48:36.000000 pydistcheck-0.4.0/src/pydistcheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 02:48:36.000000 pydistcheck-0.4.0/src/pydistcheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-30 02:48:36.000000 pydistcheck-0.4.0/src/pydistcheck.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-30 02:48:36.000000 pydistcheck-0.4.0/src/pydistcheck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-30 02:48:36.000000 pydistcheck-0.4.0/src/pydistcheck.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 02:48:36.468651 pydistcheck-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    18439 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/tests/test_distribution_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-30 02:48:28.000000 pydistcheck-0.4.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:23:41.448229 pydistcheck-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-19 06:23:29.000000 pydistcheck-0.5.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:23:41.444229 pydistcheck-0.5.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-19 06:23:29.000000 pydistcheck-0.5.0/LICENSES/DELOCATE_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-19 06:23:29.000000 pydistcheck-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-06-19 06:23:41.448229 pydistcheck-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-06-19 06:23:29.000000 pydistcheck-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-19 06:23:29.000000 pydistcheck-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-19 06:23:41.448229 pydistcheck-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:23:41.444229 pydistcheck-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:23:41.448229 pydistcheck-0.5.0/src/pydistcheck/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-19 06:23:29.000000 pydistcheck-0.5.0/src/pydistcheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-19 06:23:29.000000 pydistcheck-0.5.0/src/pydistcheck/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-06-19 06:23:29.000000 pydistcheck-0.5.0/src/pydistcheck/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-06-19 06:23:29.000000 pydistcheck-0.5.0/src/pydistcheck/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-19 06:23:29.000000 pydistcheck-0.5.0/src/pydistcheck/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-06-19 06:23:29.000000 pydistcheck-0.5.0/src/pydistcheck/distribution_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-19 06:23:29.000000 pydistcheck-0.5.0/src/pydistcheck/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-06-19 06:23:29.000000 pydistcheck-0.5.0/src/pydistcheck/shared_lib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-19 06:23:29.000000 pydistcheck-0.5.0/src/pydistcheck/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:23:41.448229 pydistcheck-0.5.0/src/pydistcheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-06-19 06:23:41.000000 pydistcheck-0.5.0/src/pydistcheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-19 06:23:41.000000 pydistcheck-0.5.0/src/pydistcheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 06:23:41.000000 pydistcheck-0.5.0/src/pydistcheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-19 06:23:41.000000 pydistcheck-0.5.0/src/pydistcheck.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-19 06:23:41.000000 pydistcheck-0.5.0/src/pydistcheck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 06:23:41.000000 pydistcheck-0.5.0/src/pydistcheck.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:23:41.448229 pydistcheck-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-19 06:23:29.000000 pydistcheck-0.5.0/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-06-19 06:23:29.000000 pydistcheck-0.5.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-06-19 06:23:29.000000 pydistcheck-0.5.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-06-19 06:23:29.000000 pydistcheck-0.5.0/tests/test_distribution_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-19 06:23:29.000000 pydistcheck-0.5.0/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-19 06:23:29.000000 pydistcheck-0.5.0/tests/test_utils.py
```

### Comparing `pydistcheck-0.4.0/LICENSE` & `pydistcheck-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.4.0/LICENSES/DELOCATE_LICENSE` & `pydistcheck-0.5.0/LICENSES/DELOCATE_LICENSE`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.4.0/PKG-INFO` & `pydistcheck-0.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydistcheck
-Version: 0.4.0
+Version: 0.5.0
 Summary: Inspect Python package distributions and raise warnings on common problems.
 Author-email: James Lamb <jaylamb20@gmail.com>
 Maintainer-email: James Lamb <jaylamb20@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, James Lamb
         All rights reserved.
@@ -72,15 +72,17 @@
 `pydistcheck` is a command line interface (CLI) for:
 
 * inspecting the contents of Python package distributions during development
 * enforcing constraints on Python package distributions in continuous integration
 
 It's inspired by R's `R CMD check`.
 
-For more background on the value of such a tool, see the SciPY 2022 talk "Does that CSV Belong on PyPI? Probably Not" ([video link](https://www.youtube.com/watch?v=1a7g5l_g_U8)).
+See ["How to Test a Python Distribution"](https://pydistcheck.readthedocs.io/en/latest/how-to-test-a-python-distribution.html) to see how it and similar tools like [`auditwheel`](https://github.com/pypa/auditwheel), [`check-wheel-contents`](https://github.com/jwodder/check-wheel-contents), and [`twine check`](https://twine.readthedocs.io/en/stable/#twine-check) fit into Python development workflows.
+
+For more background on the value of such a tool, see the SciPy 2022 talk "Does that CSV Belong on PyPI? Probably Not" ([video link](https://www.youtube.com/watch?v=1a7g5l_g_U8)).
 
 ## Installation
 
 Install with `pipx`.
 
 ```shell
 pipx install pydistcheck
@@ -131,15 +133,10 @@
 ------------ check results -----------
 1. [compiled-objects-have-debug-symbols] Found compiled object containing debug symbols. For details, extract the distribution contents and run 'objdump --all-headers "lib/lib_baseballmetrics.so"'.
 errors found while checking: 1
 ```
 
 See https://pydistcheck.readthedocs.io/en/latest/ to learn more.
 
-## Related Projects
-
-* https://pypi.org/project/inspect4py/
-* https://github.com/regebro/pyroma
-
 ## References
 
 * Python packaging guides: https://packaging.python.org/en/latest/guides/#
```

### Comparing `pydistcheck-0.4.0/README.md` & `pydistcheck-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 `pydistcheck` is a command line interface (CLI) for:
 
 * inspecting the contents of Python package distributions during development
 * enforcing constraints on Python package distributions in continuous integration
 
 It's inspired by R's `R CMD check`.
 
-For more background on the value of such a tool, see the SciPY 2022 talk "Does that CSV Belong on PyPI? Probably Not" ([video link](https://www.youtube.com/watch?v=1a7g5l_g_U8)).
+See ["How to Test a Python Distribution"](https://pydistcheck.readthedocs.io/en/latest/how-to-test-a-python-distribution.html) to see how it and similar tools like [`auditwheel`](https://github.com/pypa/auditwheel), [`check-wheel-contents`](https://github.com/jwodder/check-wheel-contents), and [`twine check`](https://twine.readthedocs.io/en/stable/#twine-check) fit into Python development workflows.
+
+For more background on the value of such a tool, see the SciPy 2022 talk "Does that CSV Belong on PyPI? Probably Not" ([video link](https://www.youtube.com/watch?v=1a7g5l_g_U8)).
 
 ## Installation
 
 Install with `pipx`.
 
 ```shell
 pipx install pydistcheck
@@ -72,15 +74,10 @@
 ------------ check results -----------
 1. [compiled-objects-have-debug-symbols] Found compiled object containing debug symbols. For details, extract the distribution contents and run 'objdump --all-headers "lib/lib_baseballmetrics.so"'.
 errors found while checking: 1
 ```
 
 See https://pydistcheck.readthedocs.io/en/latest/ to learn more.
 
-## Related Projects
-
-* https://pypi.org/project/inspect4py/
-* https://github.com/regebro/pyroma
-
 ## References
 
 * Python packaging guides: https://packaging.python.org/en/latest/guides/#
```

### Comparing `pydistcheck-0.4.0/pyproject.toml` & `pydistcheck-0.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -28,29 +28,32 @@
 license = {file = "LICENSE"}
 maintainers = [
   {name = "James Lamb", email = "jaylamb20@gmail.com"}
 ]
 name = "pydistcheck"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.4.0"
+dynamic = ["version"]
+
+[tool.setuptools.dynamic]
+version = {attr = "pydistcheck.__version__"}
 
 [project.scripts]
 pydistcheck = "pydistcheck.cli:check"
 
 [project.urls]
 homepage = "https://pydistcheck.readthedocs.io/en/latest/"
 documentation = "https://pydistcheck.readthedocs.io/en/latest/"
 repository = "https://github.com/jameslamb/pydistcheck"
 changelog = "https://github.com/jameslamb/pydistcheck/releases"
 
 [build-system]
 
 requires = [
-    "setuptools>=63",
+    "setuptools>=67",
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 100
 
 [tool.isort]
```

### Comparing `pydistcheck-0.4.0/src/pydistcheck/checks.py` & `pydistcheck-0.5.0/src/pydistcheck/checks.py`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.4.0/src/pydistcheck/cli.py` & `pydistcheck-0.5.0/src/pydistcheck/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 import sys
 from typing import List
 
 import click
 
+from pydistcheck import __version__ as _VERSION
 from pydistcheck.checks import (
     ALL_CHECKS,
     _CompiledObjectsDebugSymbolCheck,
     _DistroTooLargeCompressedCheck,
     _DistroTooLargeUnCompressedCheck,
     _FileCountCheck,
     _FilesOnlyDifferByCaseCheck,
@@ -28,14 +29,30 @@
 @click.command()
 @click.argument(
     "filepaths",
     type=click.Path(exists=True),
     nargs=-1,
 )
 @click.option(
+    "--version",
+    is_flag=True,
+    show_default=False,
+    default=False,
+    help="Print the version of pydistcheck and exit.",
+)
+@click.option(
+    "--config",
+    type=click.Path(exists=True),
+    default=None,
+    help=(
+        "Path to a TOML file containing a [tool.pydistcheck] table. "
+        "If provided, pyproject.toml will be ignored."
+    ),
+)
+@click.option(
     "--ignore",
     type=str,
     default=_Config.ignore,
     help=(
         "comma-separated list of checks to skip, e.g. "
         "``distro-too-large-compressed,path-contains-spaces``."
     ),
@@ -102,67 +119,76 @@
         "comma-delimited list of patterns matching files that are not expected "
         "to be found in the distribution. Patterns should be in the format understood "
         "by ``fnmatch.fnmatchcase()``. See https://docs.python.org/3/library/fnmatch.html."
     ),
 )
 def check(  # pylint: disable=too-many-arguments
     filepaths: str,
+    version: bool,
+    config: str,
     ignore: str,
     inspect: bool,
     max_allowed_files: int,
     max_allowed_size_compressed: str,
     max_allowed_size_uncompressed: str,
     unexpected_directory_patterns: str,
     unexpected_file_patterns: str,
 ) -> None:
     """
     Run the contents of a distribution through a set of checks, and warn about
     any problematic characteristics that are detected.
     """
+    if version:
+        print(f"pydistcheck {_VERSION}")
+        sys.exit(0)
+
     print("==================== running pydistcheck ====================")
     filepaths_to_check = [click.format_filename(f) for f in filepaths]
-    config = _Config()
+    conf = _Config()
     kwargs = {
         "ignore": ignore,
         "inspect": inspect,
         "max_allowed_files": max_allowed_files,
         "max_allowed_size_compressed": max_allowed_size_compressed,
         "max_allowed_size_uncompressed": max_allowed_size_uncompressed,
         "unexpected_directory_patterns": unexpected_directory_patterns,
         "unexpected_file_patterns": unexpected_file_patterns,
     }
     kwargs_that_differ_from_defaults = {}
     for k, v in kwargs.items():
-        if v != getattr(config, k):
+        if v != getattr(conf, k):
             kwargs_that_differ_from_defaults[k] = v
-    config.update_from_toml(toml_file="pyproject.toml")
-    config.update_from_dict(input_dict=kwargs_that_differ_from_defaults)
+    if config is not None:
+        conf.update_from_toml(toml_file=click.format_filename(config))
+    else:
+        conf.update_from_toml(toml_file="pyproject.toml")
+    conf.update_from_dict(input_dict=kwargs_that_differ_from_defaults)
 
-    checks_to_ignore = {x for x in config.ignore.split(",") if x.strip() != ""}
+    checks_to_ignore = {x for x in conf.ignore.split(",") if x.strip() != ""}
     unrecognized_checks = checks_to_ignore - ALL_CHECKS
     if unrecognized_checks:
         # converting to list + sorting here so outputs are deterministic
         # (since sets don't guarantee ordering)
         error_str = ",".join(sorted(unrecognized_checks))
         print(f"ERROR: found the following unrecognized checks passed via '--ignore': {error_str}")
         sys.exit(1)
 
     checks = [
         _CompiledObjectsDebugSymbolCheck(),
         _DistroTooLargeCompressedCheck(
             max_allowed_size_bytes=_FileSize.from_string(
-                size_str=config.max_allowed_size_compressed
+                size_str=conf.max_allowed_size_compressed
             ).total_size_bytes
         ),
         _DistroTooLargeUnCompressedCheck(
             max_allowed_size_bytes=_FileSize.from_string(
-                size_str=config.max_allowed_size_uncompressed
+                size_str=conf.max_allowed_size_uncompressed
             ).total_size_bytes
         ),
-        _FileCountCheck(max_allowed_files=config.max_allowed_files),
+        _FileCountCheck(max_allowed_files=conf.max_allowed_files),
         _FilesOnlyDifferByCaseCheck(),
         _MixedFileExtensionCheck(),
         _SpacesInPathCheck(),
         _UnexpectedFilesCheck(
             unexpected_directory_patterns=unexpected_directory_patterns.split(","),
             unexpected_file_patterns=unexpected_file_patterns.split(","),
         ),
@@ -172,15 +198,15 @@
     # filter out ignored checks
     checks = [c for c in checks if c.check_name not in checks_to_ignore]
 
     any_errors_found = False
     for filepath in filepaths_to_check:
         print(f"\nchecking '{filepath}'")
 
-        if config.inspect:
+        if conf.inspect:
             print("----- package inspection summary -----")
             inspect_distribution(filepath=filepath)
 
         print("------------ check results -----------")
         summary = _DistributionSummary.from_file(filename=filepath)
         errors: List[str] = []
         for this_check in checks:
```

### Comparing `pydistcheck-0.4.0/src/pydistcheck/config.py` & `pydistcheck-0.5.0/src/pydistcheck/config.py`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.4.0/src/pydistcheck/distribution_summary.py` & `pydistcheck-0.5.0/src/pydistcheck/distribution_summary.py`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.4.0/src/pydistcheck/inspect.py` & `pydistcheck-0.5.0/src/pydistcheck/inspect.py`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.4.0/src/pydistcheck/shared_lib_utils.py` & `pydistcheck-0.5.0/src/pydistcheck/shared_lib_utils.py`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.4.0/src/pydistcheck/utils.py` & `pydistcheck-0.5.0/src/pydistcheck/utils.py`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.4.0/src/pydistcheck.egg-info/PKG-INFO` & `pydistcheck-0.5.0/src/pydistcheck.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydistcheck
-Version: 0.4.0
+Version: 0.5.0
 Summary: Inspect Python package distributions and raise warnings on common problems.
 Author-email: James Lamb <jaylamb20@gmail.com>
 Maintainer-email: James Lamb <jaylamb20@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, James Lamb
         All rights reserved.
@@ -72,15 +72,17 @@
 `pydistcheck` is a command line interface (CLI) for:
 
 * inspecting the contents of Python package distributions during development
 * enforcing constraints on Python package distributions in continuous integration
 
 It's inspired by R's `R CMD check`.
 
-For more background on the value of such a tool, see the SciPY 2022 talk "Does that CSV Belong on PyPI? Probably Not" ([video link](https://www.youtube.com/watch?v=1a7g5l_g_U8)).
+See ["How to Test a Python Distribution"](https://pydistcheck.readthedocs.io/en/latest/how-to-test-a-python-distribution.html) to see how it and similar tools like [`auditwheel`](https://github.com/pypa/auditwheel), [`check-wheel-contents`](https://github.com/jwodder/check-wheel-contents), and [`twine check`](https://twine.readthedocs.io/en/stable/#twine-check) fit into Python development workflows.
+
+For more background on the value of such a tool, see the SciPy 2022 talk "Does that CSV Belong on PyPI? Probably Not" ([video link](https://www.youtube.com/watch?v=1a7g5l_g_U8)).
 
 ## Installation
 
 Install with `pipx`.
 
 ```shell
 pipx install pydistcheck
@@ -131,15 +133,10 @@
 ------------ check results -----------
 1. [compiled-objects-have-debug-symbols] Found compiled object containing debug symbols. For details, extract the distribution contents and run 'objdump --all-headers "lib/lib_baseballmetrics.so"'.
 errors found while checking: 1
 ```
 
 See https://pydistcheck.readthedocs.io/en/latest/ to learn more.
 
-## Related Projects
-
-* https://pypi.org/project/inspect4py/
-* https://github.com/regebro/pyroma
-
 ## References
 
 * Python packaging guides: https://packaging.python.org/en/latest/guides/#
```

### Comparing `pydistcheck-0.4.0/src/pydistcheck.egg-info/SOURCES.txt` & `pydistcheck-0.5.0/src/pydistcheck.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.4.0/tests/test_checks.py` & `pydistcheck-0.5.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.4.0/tests/test_cli.py` & `pydistcheck-0.5.0/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,31 @@
 @pytest.mark.parametrize("distro_file", BASE_PACKAGES + BASE_WHEELS)
 def test_check_runs_without_error(distro_file):
     runner = CliRunner()
     result = runner.invoke(check, [os.path.join(TEST_DATA_DIR, distro_file)])
     assert result.exit_code == 0
 
 
+def test_version_flag_works():
+    runner = CliRunner()
+    result = runner.invoke(
+        check,
+        [
+            "--version",
+        ],
+    )
+    assert result.exit_code == 0
+
+    _assert_log_matches_pattern(
+        result=result,
+        pattern=(r"^pydistcheck [0-9]{1}\.[0-9]{1,2}\.[0-9]{1,2}\.*[0-9]*$"),
+        num_times=1,
+    )
+
+
 def test_check_fails_with_informative_error_if_file_doesnt_exist():
     runner = CliRunner()
     result = runner.invoke(check, ["some-garbage.exe"])
     assert result.exit_code > 0
     _assert_log_matches_pattern(result, r"Path 'some\-garbage\.exe' does not exist\.$")
 
 
@@ -304,15 +321,15 @@
             [os.path.join(TEST_DATA_DIR, distro_file), "--max-allowed-files=1"],
         )
         assert result.exit_code == 0
         _assert_log_matches_pattern(result, "errors found while checking\\: 0")
 
 
 @pytest.mark.parametrize("distro_file", BASE_PACKAGES)
-def test_check_prefers_keyword_args_to_pyrpoject_toml_and_defaults(distro_file, tmp_path):
+def test_check_prefers_keyword_args_to_pyproject_toml_and_defaults(distro_file, tmp_path):
     runner = CliRunner()
     with runner.isolated_filesystem(temp_dir=tmp_path):
         with open("pyproject.toml", "w") as f:
             f.write("[tool.pylint]\n[tool.pydistcheck]\nmax_allowed_size_uncompressed = '7B'\n")
         result = runner.invoke(
             check,
             [os.path.join(TEST_DATA_DIR, distro_file), "--max-allowed-size-uncompressed=123B"],
@@ -325,14 +342,41 @@
             r"^1\. \[distro\-too\-large\-uncompressed\] Uncompressed size [0-9]+\.[0-9]+K is "
             r"larger than the allowed size \(0\.1K\)\.$"
         ),
     )
     _assert_log_matches_pattern(result, "errors found while checking\\: 1")
 
 
+@pytest.mark.parametrize("distro_file", BASE_PACKAGES)
+def test_check_prefers_custom_toml_file_to_root_pyproject_toml(distro_file, tmp_path):
+    runner = CliRunner()
+    with runner.isolated_filesystem(temp_dir=tmp_path):
+        with open("pyproject.toml", "w") as f:
+            f.write("[tool.pylint]\n[tool.pydistcheck]\nmax_allowed_size_uncompressed = '10GB'\n")
+        other_dir = os.path.join(tmp_path, "cool-files")
+        other_config = os.path.join(other_dir, "stuff.toml")
+        os.mkdir(other_dir)
+        with open(other_config, "w") as f:
+            f.write("[tool.pylint]\n[tool.pydistcheck]\nmax_allowed_size_uncompressed = '7B'\n")
+        result = runner.invoke(
+            check,
+            [os.path.join(TEST_DATA_DIR, distro_file), f"--config={other_config}"],
+        )
+
+    assert result.exit_code == 1
+    _assert_log_matches_pattern(
+        result,
+        (
+            r"^1\. \[distro\-too\-large\-uncompressed\] Uncompressed size [0-9]+\.[0-9]+K is "
+            r"larger than the allowed size \(7\.0B\)\.$"
+        ),
+    )
+    _assert_log_matches_pattern(result, "errors found while checking\\: 1")
+
+
 @pytest.mark.parametrize("distro_file", PROBLEMATIC_PACKAGES)
 def test_files_only_differ_by_case_works(distro_file):
     runner = CliRunner()
     result = runner.invoke(
         check,
         [os.path.join(TEST_DATA_DIR, distro_file)],
     )
```

### Comparing `pydistcheck-0.4.0/tests/test_config.py` & `pydistcheck-0.5.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.4.0/tests/test_distribution_summary.py` & `pydistcheck-0.5.0/tests/test_distribution_summary.py`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.4.0/tests/test_docs.py` & `pydistcheck-0.5.0/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `pydistcheck-0.4.0/tests/test_utils.py` & `pydistcheck-0.5.0/tests/test_utils.py`

 * *Files identical despite different names*

