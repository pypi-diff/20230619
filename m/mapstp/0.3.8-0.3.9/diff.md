# Comparing `tmp/mapstp-0.3.8.tar.gz` & `tmp/mapstp-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapstp-0.3.8.tar", max compression
+gzip compressed data, was "mapstp-0.3.9.tar", max compression
```

## Comparing `mapstp-0.3.8.tar` & `mapstp-0.3.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1063 2022-10-04 14:01:17.892492 mapstp-0.3.8/LICENSE
--rw-r--r--   0        0        0     4098 2022-10-04 14:01:32.105812 mapstp-0.3.8/README.rst
--rw-r--r--   0        0        0     6232 2022-10-04 14:01:32.105812 mapstp-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      708 2022-10-04 14:01:17.896493 mapstp-0.3.8/src/mapstp/__init__.py
--rw-r--r--   0        0        0       35 2022-10-04 14:01:17.896493 mapstp-0.3.8/src/mapstp/cli/__init__.py
--rw-r--r--   0        0        0     2708 2022-10-04 14:01:17.896493 mapstp-0.3.8/src/mapstp/cli/logging.py
--rw-r--r--   0        0        0        0 2022-10-04 14:01:17.896493 mapstp-0.3.8/src/mapstp/cli/py.typed
--rw-r--r--   0        0        0     5797 2022-10-04 14:01:17.896493 mapstp-0.3.8/src/mapstp/cli/runner.py
--rw-r--r--   0        0        0     1934 2022-10-04 14:01:32.105812 mapstp-0.3.8/src/mapstp/config.py
--rw-r--r--   0        0        0    27788 2022-10-04 14:01:17.896493 mapstp-0.3.8/src/mapstp/data/default-material-index.xlsx
--rw-r--r--   0        0        0   158413 2022-10-04 14:01:17.896493 mapstp-0.3.8/src/mapstp/data/materials.txt.zip
--rw-r--r--   0        0        0     1040 2022-10-04 14:01:32.105812 mapstp-0.3.8/src/mapstp/excel.py
--rw-r--r--   0        0        0     1118 2022-10-04 14:01:17.896493 mapstp-0.3.8/src/mapstp/exceptions.py
--rw-r--r--   0        0        0     3723 2022-10-04 14:01:17.896493 mapstp-0.3.8/src/mapstp/extract_info.py
--rw-r--r--   0        0        0     5436 2022-10-04 14:01:32.105812 mapstp-0.3.8/src/mapstp/materials.py
--rw-r--r--   0        0        0     1622 2022-10-04 14:01:32.105812 mapstp-0.3.8/src/mapstp/materials_index.py
--rw-r--r--   0        0        0     7034 2022-10-04 14:01:32.105812 mapstp-0.3.8/src/mapstp/merge.py
--rw-r--r--   0        0        0        0 2022-10-04 14:01:17.896493 mapstp-0.3.8/src/mapstp/py.typed
--rw-r--r--   0        0        0     7892 2022-10-04 14:01:32.105812 mapstp-0.3.8/src/mapstp/stp_parser.py
--rw-r--r--   0        0        0     4311 2022-10-04 14:01:32.105812 mapstp-0.3.8/src/mapstp/tree.py
--rw-r--r--   0        0        0       48 2022-10-04 14:01:17.896493 mapstp-0.3.8/src/mapstp/utils/__init__.py
--rw-r--r--   0        0        0     3399 2022-10-04 14:01:32.109812 mapstp-0.3.8/src/mapstp/utils/io.py
--rw-r--r--   0        0        0        0 2022-10-04 14:01:17.896493 mapstp-0.3.8/src/mapstp/utils/py.typed
--rw-r--r--   0        0        0      652 2022-10-04 14:01:17.896493 mapstp-0.3.8/src/mapstp/utils/re.py
--rw-r--r--   0        0        0     2169 2022-10-04 14:01:32.109812 mapstp-0.3.8/src/mapstp/utils/resource.py
--rw-r--r--   0        0        0     1273 2022-10-04 14:01:17.896493 mapstp-0.3.8/src/mapstp/workflow.py
--rw-r--r--   0        0        0     5156 1970-01-01 00:00:00.000000 mapstp-0.3.8/setup.py
--rw-r--r--   0        0        0     5358 1970-01-01 00:00:00.000000 mapstp-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2022-12-22 11:21:39.737309 mapstp-0.3.9/LICENSE
+-rw-r--r--   0        0        0     4098 2022-12-22 11:21:39.737309 mapstp-0.3.9/README.rst
+-rw-r--r--   0        0        0     6998 2022-12-22 11:22:02.673549 mapstp-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      708 2022-12-22 11:21:39.741309 mapstp-0.3.9/src/mapstp/__init__.py
+-rw-r--r--   0        0        0       35 2022-12-22 11:21:39.741309 mapstp-0.3.9/src/mapstp/cli/__init__.py
+-rw-r--r--   0        0        0     2740 2022-12-22 11:22:02.673549 mapstp-0.3.9/src/mapstp/cli/logging.py
+-rw-r--r--   0        0        0        0 2022-12-22 11:21:39.741309 mapstp-0.3.9/src/mapstp/cli/py.typed
+-rw-r--r--   0        0        0     5797 2022-12-22 11:21:39.741309 mapstp-0.3.9/src/mapstp/cli/runner.py
+-rw-r--r--   0        0        0     1934 2022-12-22 11:21:39.741309 mapstp-0.3.9/src/mapstp/config.py
+-rw-r--r--   0        0        0    27788 2022-12-22 11:21:39.741309 mapstp-0.3.9/src/mapstp/data/default-material-index.xlsx
+-rw-r--r--   0        0        0   158413 2022-12-22 11:21:39.741309 mapstp-0.3.9/src/mapstp/data/materials.txt.zip
+-rw-r--r--   0        0        0     1030 2022-12-22 11:22:02.673549 mapstp-0.3.9/src/mapstp/excel.py
+-rw-r--r--   0        0        0     1118 2022-12-22 11:21:39.741309 mapstp-0.3.9/src/mapstp/exceptions.py
+-rw-r--r--   0        0        0     3723 2022-12-22 11:21:39.741309 mapstp-0.3.9/src/mapstp/extract_info.py
+-rw-r--r--   0        0        0     5431 2022-12-22 11:22:02.673549 mapstp-0.3.9/src/mapstp/materials.py
+-rw-r--r--   0        0        0     1622 2022-12-22 11:21:39.741309 mapstp-0.3.9/src/mapstp/materials_index.py
+-rw-r--r--   0        0        0     7207 2022-12-22 11:22:02.673549 mapstp-0.3.9/src/mapstp/merge.py
+-rw-r--r--   0        0        0        0 2022-12-22 11:21:39.741309 mapstp-0.3.9/src/mapstp/py.typed
+-rw-r--r--   0        0        0     8451 2022-12-22 11:22:02.673549 mapstp-0.3.9/src/mapstp/stp_parser.py
+-rw-r--r--   0        0        0     4903 2022-12-22 11:22:02.673549 mapstp-0.3.9/src/mapstp/tree.py
+-rw-r--r--   0        0        0       48 2022-12-22 11:21:39.741309 mapstp-0.3.9/src/mapstp/utils/__init__.py
+-rw-r--r--   0        0        0     3399 2022-12-22 11:21:39.741309 mapstp-0.3.9/src/mapstp/utils/io.py
+-rw-r--r--   0        0        0        0 2022-12-22 11:21:39.741309 mapstp-0.3.9/src/mapstp/utils/py.typed
+-rw-r--r--   0        0        0      652 2022-12-22 11:21:39.741309 mapstp-0.3.9/src/mapstp/utils/re.py
+-rw-r--r--   0        0        0     2363 2022-12-22 11:22:02.673549 mapstp-0.3.9/src/mapstp/utils/resource.py
+-rw-r--r--   0        0        0     1302 2022-12-22 11:22:02.673549 mapstp-0.3.9/src/mapstp/workflow.py
+-rw-r--r--   0        0        0     5156 1970-01-01 00:00:00.000000 mapstp-0.3.9/setup.py
+-rw-r--r--   0        0        0     5409 1970-01-01 00:00:00.000000 mapstp-0.3.9/PKG-INFO
```

### Comparing `mapstp-0.3.8/LICENSE` & `mapstp-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mapstp-0.3.8/README.rst` & `mapstp-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `mapstp-0.3.8/pyproject.toml` & `mapstp-0.3.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mapstp"
-version = "0.3.8"
+version = "0.3.9"
 description = "Transfers meta information from STP to MCNP"
 authors = ["dvp <dmitri_portnov@yahoo.com>"]
 homepage = "https://github.com/MC-kit/map-stp"
 repository = "https://github.com/MC-kit/map-stp"
 # documentation = "https://mapstp.readthedocs.io
 license = "MIT"
 keywords = ["STP", "MCNP", "SuperMC", "SpaceClaim"]
@@ -39,26 +39,23 @@
 openpyxl = ">=3.0.9"
 pandas = ">=1.4.1"
 tomli = ">=2.0.1"
 
 [tool.poetry.group.dev.dependencies]
 Pygments = ">=2.10.0"
 nox = ">=2022.1.7"
-tomli = ">=2.0.1"
+tomli = { version = ">=2.0.1", python="<3.11" }
 
 #[tool.poetry.group.profile]
 #optional = true
 
 #[tool.poetry.group.profile.dependencies]
 # TODO dvp: apply yappi: https://coderzcolumn.com/tutorials/python/yappi-yet-another-python-profiler
 #yappi = ">=1.3.2"
 
-[tool.poetry.group.safety.dependencies]
-safety = ">=1.10.3"
-
 [tool.poetry.group.pre_commit.dependencies]
 pre-commit = ">=2.15.0"
 rstcheck = ">=3.3.1"
 
 [tool.poetry.group.black.dependencies]
 black = ">=22.8.0"
 
@@ -90,32 +87,35 @@
 numpy = ">=1.23.2"
 
 [tool.poetry.group.flake8.dependencies]
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
 flake8-annotations = ">=2.6.2"
 flake8-bandit = ">=4.1.1"
-flake8-bugbear = ">=22.1.11"
+flake8-bugbear = ">=22.3.23"
 flake8-builtins = ">=1.5.3"
 flake8-colors = ">=0.1.9"
 flake8-commas = ">=2.1.0"
 flake8-comprehensions = ">=3.10.0"
 flake8-docstrings = ">=1.6.0"
 flake8-import-order = ">=0.18.1"
 flake8-print = ">=5.0.0"
-flake8-rst-docstrings = ">=0.2.3"
+flake8-rst-docstrings = ">=0.2.7"
 flake8-use-fstring = ">=1.4"
 tryceratops = ">=1.0.1"
 
+# TODO dvp: check/use flake8-pyprojecttoml plugin
+# https://gitlab.com/durko/flake8-pyprojecttoml/-/blob/master/pyproject.toml
+
 [tool.poetry.group.docs.dependencies]
-sphinx = ">=5.0.2"
-sphinx-autodoc-typehints = ">=1.12.0"
+sphinx = ">=5.3.0"
+sphinx-autodoc-typehints = ">=1.19.5"
 sphinx-autorun = ">=1.1.1"
-sphinx-click = ">=4.0.3"
-sphinx-rtd-theme = ">=1.0.0"
+sphinx-click = ">=4.4.0"
+sphinx-rtd-theme = ">=1.1.1"
 sphinxcontrib-napoleon = ">=0.7"
 
 [tool.poetry.group.docs_auto.dependencies]
 sphinx-autobuild = ">=2021.3.14"
 
 
 [build-system]
@@ -161,32 +161,39 @@
   | \.idea
   | _build
   | build
   | build_configs
   | dist
   | data
   | htmlcov
-  | .egg-info
+  | \.egg-info
   | notebooks
   | wrk
 )
 '''
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 norecursedirs = ".* build dist *.egg-info data"
 python_functions = "test_*  profile_*"
 addopts = "-ra -q --tb=short --doctest-modules --strict-markers --ignore setup.py --failed-first"
 doctest_optionflags = "NORMALIZE_WHITESPACE IGNORE_EXCEPTION_DETAIL ALLOW_UNICODE ALLOW_BYTES"
-testpaths = ["src/tests"]
+testpaths = ["tests"]
 markers = [
     "slow: too slow tests"
 ]
 # xfail tests that pass should fail the test suite
 xfail_strict = true
+filterwarnings = [
+    "ignore:.*not typechecking multipledispatch.dispatcher.*:UserWarning"
+]
+
+[tool.xdoctest]
+quiet = true
+options = ""
 
 # [tool.coverage]
 [tool.coverage.paths]
 source = ["src", ".nox/*/site-packages"]
 
 [tool.coverage.run]
 branch = true
@@ -212,46 +219,70 @@
 ]
 ignore_errors = true
 sort = "Cover"
 
 
 # MyPy config
 # See https://mypy.readthedocs.io/en/stable/config_file.html#using-a-pyproject-toml-file
+#     https://dev.to/tusharsadhwani/the-comprehensive-guide-to-mypy-561m
 [tool.mypy]
 python_version = "3.10"
 # strict = true     # TODO dvp: uncomment this to get strict control
 follow_imports = "silent"
 # namespace_packages = true
 warn_return_any = true
 warn_unused_configs = true
 show_error_codes = true
+enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
+disable_error_code = ["annotation-unchecked"]
 show_error_context = true
 error_summary = true
 warn_redundant_casts = true
 warn_unreachable = true
 warn_unused_ignores = true
 files = "src/mapstp/**/*.py"
-
+plugins = ["numpy.typing.mypy_plugin"]
 
 [[tool.mypy.overrides]]
 module = [
     "click",
     "click.testing",
     "loguru",
     "multipledispatch",
     "nox",
     "numpy.testing",
     "pandas",
     "pytest",
     "scipy.constants",
+    "tomllib",
+    "tomli"
 ]
 ignore_missing_imports = true
 
+[[tool.mypy.overrides]]
+module = [
+    "tomllib",
+    "tomli"
+]
+allow_redefinition = true
+disable_error_code = "no-redef"
+
+[tool.check-manifest]
+ignore = [
+    "tests/*",
+    "tools/*",
+    "*.yaml",
+    "noxfile.py",
+]
+
+[tool.ipdb]
+# For debugging in jupyterlab and ipython
+# see https://github.com/gotcha/ipdb
+context=5
 
 [tool.tryceratops]
 include = ["src"]
-#ignore = ["TC002", "TC200", "TC300"]
 experimental = true
 
 [tool.pycln]
-path = ["src", "tools"]
+path = "src"
 #silence = true
```

### Comparing `mapstp-0.3.8/src/mapstp/__init__.py` & `mapstp-0.3.9/src/mapstp/__init__.py`

 * *Files identical despite different names*

### Comparing `mapstp-0.3.8/src/mapstp/cli/logging.py` & `mapstp-0.3.9/src/mapstp/cli/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,16 @@
             level = logger.level(record.levelname).name
         except ValueError:
             level = logging.getLevelName(record.levelno)
 
         # Find caller from where originated the logged message
         frame = logging.currentframe()
         depth = 2
-        while frame.f_code.co_filename == logging.__file__:
-            frame = frame.f_back  # type: ignore
+        while frame.f_code.co_filename == logging.__file__:  # pragma: no cover
+            frame = frame.f_back  # type: ignore[assignment]
             depth += 1
 
         logger.opt(depth=depth, exception=record.exc_info).log(
             level, record.getMessage()
         )
```

### Comparing `mapstp-0.3.8/src/mapstp/cli/runner.py` & `mapstp-0.3.9/src/mapstp/cli/runner.py`

 * *Files identical despite different names*

### Comparing `mapstp-0.3.8/src/mapstp/config.py` & `mapstp-0.3.9/src/mapstp/config.py`

 * *Files identical despite different names*

### Comparing `mapstp-0.3.8/src/mapstp/data/default-material-index.xlsx` & `mapstp-0.3.9/src/mapstp/data/default-material-index.xlsx`

 * *Files identical despite different names*

### Comparing `mapstp-0.3.8/src/mapstp/data/materials.txt.zip` & `mapstp-0.3.9/src/mapstp/data/materials.txt.zip`

 * *Files identical despite different names*

### Comparing `mapstp-0.3.8/src/mapstp/excel.py` & `mapstp-0.3.9/src/mapstp/excel.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,12 +22,12 @@
         excel: output excel file name
         paths: STP paths for each cell
         path_info: number, density, factor for each cell
         separator: character to separate STP path parts
         start_cell_number: number to start cell numbering in the excel
     """
     df = path_info.copy()
-    df["STP path"] = [lambda x: separator.join(x) for x in paths]
+    df["STP path"] = [separator.join(x) for x in paths]
     df["cell"] = list(range(start_cell_number, len(paths) + start_cell_number))
     df.set_index(keys="cell", inplace=True)
     with pd.ExcelWriter(excel) as xlsx:
         df.to_excel(xlsx, sheet_name="Cells")
```

### Comparing `mapstp-0.3.8/src/mapstp/exceptions.py` & `mapstp-0.3.9/src/mapstp/exceptions.py`

 * *Files identical despite different names*

### Comparing `mapstp-0.3.8/src/mapstp/extract_info.py` & `mapstp-0.3.9/src/mapstp/extract_info.py`

 * *Files identical despite different names*

### Comparing `mapstp-0.3.8/src/mapstp/materials.py` & `mapstp-0.3.9/src/mapstp/materials.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 The map associates material number to its MCNP specification text.
 """
 
 from typing import Callable, Dict, Generator, Iterable, List, TextIO, Union
 
 from collections import defaultdict
 from dataclasses import dataclass, field
+from logging import getLogger
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
-from loguru import logger
 from mapstp.utils.re import CARD_PATTERN, MATERIAL_PATTERN
 
 MaterialsDict = Dict[int, str]
 """Mapping material number -> material MCNP text"""
 
+logger = getLogger()
+
 
 @dataclass
 class _Loader:
     stream: TextIO
     material_no: int = field(default=-1, init=False)
     materials_dict: Dict[int, List[str]] = field(
         default_factory=lambda: defaultdict(list), init=False
@@ -136,21 +138,21 @@
         materials_map:  map number -> spec
 
     Returns:
         method to be used in map extracting material specification.
     """
 
     def _func(used_number: int) -> str:
-        if isinstance(used_number, int) and 0 < used_number:
+        if 0 < used_number:
             text = materials_map.get(used_number)
             if not text:
                 logger.warning(
-                    "Material M{} is not found in provided materials specifications. "
+                    f"Material M{used_number} is not found "
+                    "in provided materials specifications. "
                     "A dummy specification is issued to the tagged model.",
-                    used_number,
                 )
                 text = (
                     f"m{used_number}  "
                     "$ dummy: material was not provided to mapstp\n"
                     "        1.001.31c  1.0\n"
                 )
             return text
```

### Comparing `mapstp-0.3.8/src/mapstp/materials_index.py` & `mapstp-0.3.9/src/mapstp/materials_index.py`

 * *Files identical despite different names*

### Comparing `mapstp-0.3.8/src/mapstp/merge.py` & `mapstp-0.3.9/src/mapstp/merge.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """The module implements algorithms to transform MCNP model.
 
 Inserts end comments with information about path in STP
 corresponding to a cell and sets materials and densities,
 if specified in STP paths.
 
 """
-
 from typing import Generator, Iterable, List, Optional, TextIO, Tuple, Union
 
 import math
 
 from dataclasses import dataclass, field
+from logging import getLogger
 from pathlib import Path
 
 import pandas as pd
 
-from loguru import logger
 from mapstp.exceptions import PathInfoError
 from mapstp.materials import drop_material_cards
 from mapstp.utils.io import read_mcnp_sections
 from mapstp.utils.re import CELL_START_PATTERN
 
+logger = getLogger()
+
 
-def is_defined(number: Union[int, float]) -> bool:
+def is_defined(number: Union[int, float, None]) -> bool:
     """Check if number coming from a DataFrame object cell is not None or NaN.
 
     Args:
         number: value to
 
     Returns:
         true - if `number` is a valid number,
@@ -140,17 +141,16 @@
                 yield line
             else:
                 yield line
         if self.current_path_idx < self.paths_length:
             yield self.format_comment()
         if self.current_path_idx != self.paths_length:
             logger.warning(
-                "Only {} cells merged, STP specifies {} bodies.",
-                self.current_path_idx,
-                self.paths_length,
+                f"Only {self.current_path_idx} cells merged, "
+                f"STP specifies {self.paths_length} bodies."
             )
 
 
 def _merge_lines(
     paths: List[str],
     path_info: pd.DataFrame,
     mcnp_lines: Iterable[str],
@@ -207,14 +207,19 @@
             print("\n\n", file=output)
 
             remainder = mcnp_sections.remainder
             if remainder:
                 print(remainder, file=output, end="")
         else:
             print(used_materials_text, file=output)
+    else:
+        logger.warning(
+            "There are no surfaces in model, "
+            "skipping surfaces and data cards including materials"
+        )
 
 
 def join_paths(paths: List[List[str]], separator: str = "/") -> List[str]:
     """Collect rows of strings to string.
 
     Args:
         paths: list of stp paths defined as list of strings
```

### Comparing `mapstp-0.3.8/src/mapstp/stp_parser.py` & `mapstp-0.3.9/src/mapstp/stp_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -203,36 +203,47 @@
 
     Raises:
         FileError: on invalid file header and if STP protocol is not AP214
     """
     products: List[Product] = []
     links: LinksList = []
     check_header(inp)
+    # normal stp has links and components,
+    # but in q 'simple' case there are bodies only and one product
+    may_have_components = True
     for line_no_minus_3, line in enumerate(inp):
         try:
             match = _SELECT_PATTERN.search(line)
             if match:
                 group = match.lastgroup
                 if group == "solid":
                     body = Body.from_string(line)
                     if not products:
-                        msg = "At least one product is to be loaded at this step"
-                        raise STPParserError(msg)
+                        # msg = "At least one product is to be loaded at this step"
+                        # raise STPParserError(msg)
+
+                        # Case for STP without components, just bodies
+                        products.append(LeafProduct(0, "dummy"))
+                        may_have_components = False
                     last_product = products[-1]
                     if not last_product.is_leaf:
                         products[-1] = last_product = LeafProduct(
                             last_product.number, last_product.name
                         )
                     last_product.append(body)
                 elif group == "link":
+                    if not may_have_components:
+                        msg = "Unexpected `link` is found in `simple` STP"
+                        raise STPParserError(msg)
                     link = Link.from_string(line)
                     links.append((link.src, link.dst))
                 elif group == "product":
-                    product = Product.from_string(line)
-                    products.append(product)
+                    if may_have_components:
+                        product = Product.from_string(line)
+                        products.append(product)
                 else:
                     msg = "Shouldn't be here, check _SELECT_PATTERN"
                     raise STPParserError(msg)
         except STPParserError as exception:
             raise FileError(f"Error in line {line_no_minus_3 + 3}") from exception
     return products, links
```

### Comparing `mapstp-0.3.8/src/mapstp/tree.py` & `mapstp-0.3.9/src/mapstp/tree.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                 parent = self._node_index.get(src)
                 if parent is None:
                     parent = self.__create_node(self._product_index[src])
                 node = self._node_index.get(dst)
                 if node is None:
                     self.__create_node(product, parent)
                 else:
-                    if node.parent is not None:
+                    if node.parent is not None:  # pragma: no cover
                         raise STPParserError()
                     node.parent = parent
 
     def __create_node(self, product: Product, parent: Optional[Node] = None) -> Node:
         """Create and register a node.
 
         Args:
@@ -122,10 +122,26 @@
     Args:
         products: list of product found on parsing STP
         links: pairs denoting links between the products.
 
 
     Returns:
         The list of paths.
+
+    Raises:
+        ValueError: if more then one product is found in STP without components
     """
-    tree = Tree(products, links)
-    return tree.create_bodies_paths()
+    if links:
+        tree = Tree(products, links)
+        return tree.create_bodies_paths()
+    else:  # `simple` STP case
+        ps = list(products)
+        if 1 != len(ps):  # pragma: no cover
+            msg = "Only one product is expected for `simple` stp"
+            raise ValueError(msg)
+        product = cast(LeafProduct, ps[0])
+        bodies_paths = []
+        for b in product.bodies:
+            bodies_paths.append(
+                [b.name]
+            )  # TODO dvp: add transliteration for Russian names
+        return bodies_paths
```

### Comparing `mapstp-0.3.8/src/mapstp/utils/io.py` & `mapstp-0.3.9/src/mapstp/utils/io.py`

 * *Files identical despite different names*

### Comparing `mapstp-0.3.8/src/mapstp/utils/re.py` & `mapstp-0.3.9/src/mapstp/utils/re.py`

 * *Files identical despite different names*

### Comparing `mapstp-0.3.8/src/mapstp/utils/resource.py` & `mapstp-0.3.9/src/mapstp/utils/resource.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,78 @@
 """Utility methods to access a package data."""
 
-from typing import Callable, Optional, cast
-
-import inspect
+from typing import Callable, cast
 
 from pathlib import Path
 
 import pkg_resources as pkg
 
 
-def filename_resolver(package: Optional[str] = None) -> Callable[[str], str]:
+def filename_resolver(package: str) -> Callable[[str], str]:
     """Create method to find data file name.
 
     Uses resource manager to handle all the cases of the deployment.
 
     Args:
         package: the package below which the data is stored.
                  Optional, if not specified, the package of caller will be used.
 
     Returns:
         callable which appends the argument to the package folder.
     """
-    package = _resolve_package(package)
-    resource_manager = pkg.ResourceManager()  # type: ignore
+    # package = _resolve_package(package)
+    resource_manager = pkg.ResourceManager()  # type: ignore[attr-defined]
 
     def func(resource: str) -> str:
         return cast(str, resource_manager.resource_filename(package, resource))
 
     func.__doc__ = f"Computes file names for resources located in {package}"
 
     return func
 
 
-def path_resolver(package: Optional[str] = None) -> Callable[[str], Path]:
+def path_resolver(package: str) -> Callable[[str], Path]:
     """Create method to find data path.
 
-    Uses :meth:`file_resolver`.
+    Uses :py:func:`file_resolver`.
 
     Args:
         package: the package below which the data is stored.
                  Optional, if not specified, the package of caller will be used.
 
     Returns:
         callable which appends the argument to the package folder adt returns as Path.
     """
     # Note: we should define package here to have proper offset in callers stack.
-    package = _resolve_package(package)
+    # package = _resolve_package(package)
     resolver = filename_resolver(package)
 
     def func(resource: str) -> Path:
         filename = resolver(resource)
         return Path(filename)
 
     func.__doc__ = f"Computes Path for resources located in {package}"
 
     return func
 
 
-class PackageNotFoundError(ValueError):
-    """Error when package is not specified and cannot be found."""
-
-    def __init__(self) -> None:
-        super().__init__(self, "Cannot define package.")
-
-
-def _resolve_package(package: Optional[str] = None) -> str:
-    if package is None:
-        module = inspect.getmodule(inspect.stack()[2][0])
-        if module is None:
-            raise PackageNotFoundError()  # pragma: no cover
-        package = module.__name__
-    return package
+# class PackageNotFoundError(ValueError):
+#     """Error when package is not specified and cannot be found."""
+#
+#     def __init__(self) -> None:
+#         super().__init__("Cannot define package.")  # pragma: no cover
+#
+#
+# def _resolve_package(
+#     package,
+# ):
+#     # No typing in this function,
+#     # otherwise typeguard decorates this and
+#     # the frame offset is to be found in a bit
+#     # more complex way.
+#     # ANN202 is ignored for this file (see .flake8)
+#     if package is None:
+#         module = inspect.getmodule(inspect.stack()[2][0])
+#         if module is None:
+#             raise PackageNotFoundError()  # pragma: no cover
+#         package = module.__name__
+#     return package
```

### Comparing `mapstp-0.3.8/src/mapstp/workflow.py` & `mapstp-0.3.9/src/mapstp/workflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 Use imported methods to organize other workflows in notebooks or dependant packages.
 Check the methods defined here as templates for other workflows.
 
 """
 from typing import List, Tuple
 
+from logging import getLogger
 from pathlib import Path
 
 import pandas as pd
 
-from loguru import logger
 from mapstp.extract_info import extract_path_info
 from mapstp.materials_index import load_materials_index
 from mapstp.stp_parser import parse_path
 from mapstp.tree import create_bodies_paths
 
 
 def create_path_info(
@@ -26,14 +26,15 @@
         materials_index: file name of materials index file.
         stp: file name of stp file.
 
     Returns:
         collected paths from the stp file
         table with joined information
     """
+    logger = getLogger()
     _materials_index = load_materials_index(materials_index)
     logger.info("Loaded material index from {}", materials_index)
     _stp = Path(stp)
     products, links = parse_path(_stp)
     logger.info("Loaded STP from {}", stp)
     paths = create_bodies_paths(products, links)
     path_info = extract_path_info(paths, _materials_index)
```

### Comparing `mapstp-0.3.8/setup.py` & `mapstp-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'tomli>=2.0.1']
 
 entry_points = \
 {'console_scripts': ['mapstp = mapstp.cli.runner:mapstp']}
 
 setup_kwargs = {
     'name': 'mapstp',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'Transfers meta information from STP to MCNP',
     'long_description': '==========================================================\n*mapstp*: link STP and MCNP models\n==========================================================\n\n|Maintained| |License| |Versions| |PyPI| |Docs|\n\n\n.. contents::\n\n\nDescription\n-----------\n\nProblem #1\n~~~~~~~~~~\n\nYou are an MCNP model developer. You have created simplified 3D CAD model using SpaceClaim, saved it to STP file, then converted\nit using SuperMC to an MCNP model. At this moment the MCNP model doesn\'t have any information on relation of the MCNP\ncame from cells to the CAD components, there\'s no materials and densities in the cell specifications.\nThe SuperMC (for the time of writing this) doesn\'t transfer this information on exporting to MCNP model.\n\nProblem #2\n~~~~~~~~~~\n\nYou have to provide results of neutron analysis in correspondence with 3D CAD model\ncomponents. For example, you have to create a table describing activation of every component.\nTo do this, you need some tools to associate CAD component with corresponding MCNP cells.\nUsing this table the results of computation for MCNP cells can be aggregated to values for\ncorresponding CAD component.\n\n\nSolution\n~~~~~~~~\n\nUsing SpaceClaim you can add additional properties to components directly in STP file.\nThe properties include: used material, density correction factor, classification tag.\nThe properties are specified as a special label, which you can add to the components names.\nThe properties are propagated over the CAD tree hierarchy from top to down and can be overridden\non lower levels with more specific values. Using SpaceClaim for this is rather intuitive.\n\nThe using *mapstp* you can transfer this information from STP to MCNP:\nThe  *mapstp*:\n\n* sets material numbers and densities in all the cells, where it was specified\n* adds $-comment after each cell denoting its path in STP, with tag "stp:",this lines can be easily removed later, if not needed\n* adds materials specifications, if they are available for *mapstp*\n* creates separate accompanying excel file with list of cells, applied materials, densities and correction factors, classification tag, and paths in STP\n\n\nInstallation\n------------\n\nDocumentation\n-------------\n\nContributing\n------------\n\n.. image:: https://github.com/MC-kit/map-stp/workflows/Tests/badge.svg\n   :target: https://github.com/MC-kit/map-stp/actions\n   :alt: Tests\n.. image:: https://codecov.io/gh/MC-kit/map-stp/branch/master/graph/badge.svg?token=wlqoa368k8\n  :target: https://codecov.io/gh/MC-kit/map-stp\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336\n   :target: https://pycqa.github.io/isort/\n.. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n   :target: https://github.com/pre-commit/pre-commit\n   :alt: pre-commit\n.. image:: https://img.shields.io/badge/try%2Fexcept%20style-tryceratops%20%F0%9F%A6%96%E2%9C%A8-black\n   :target: https://github.com/guilatrova/tryceratops\n   :alt: try/except style: tryceratops\n\n.. .. image:: https://img.shields.io/badge/security-bandit-yellow.svg\n    :target: https://github.com/PyCQA/bandit\n    :alt: Security Status\n\n.. Substitutions\n\n.. |Maintained| image:: https://img.shields.io/badge/Maintained%3F-yes-green.svg\n   :target: https://github.com/MC-kit/map-stp/graphs/commit-activity\n.. |Tests| image:: https://github.com/MC-kit/map-stp/workflows/Tests/badge.svg\n   :target: https://github.com/MC-kit/map-stp/actions?workflow=Tests\n   :alt: Tests\n.. |License| image:: https://img.shields.io/github/license/MC-kit/map-stp\n   :target: https://github.com/MC-kit/map-stp\n.. |Versions| image:: https://img.shields.io/pypi/pyversions/mapstp\n   :alt: PyPI - Python Version\n.. |PyPI| image:: https://img.shields.io/pypi/v/mapstp\n   :target: https://pypi.org/project/mapstp/\n   :alt: PyPI\n.. |Docs| image:: https://readthedocs.org/projects/mapstp/badge/?version=latest\n   :target: https://mapstp.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': 'dvp',
     'author_email': 'dmitri_portnov@yahoo.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/MC-kit/map-stp',
```

### Comparing `mapstp-0.3.8/PKG-INFO` & `mapstp-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapstp
-Version: 0.3.8
+Version: 0.3.9
 Summary: Transfers meta information from STP to MCNP
 Home-page: https://github.com/MC-kit/map-stp
 License: MIT
 Keywords: STP,MCNP,SuperMC,SpaceClaim
 Author: dvp
 Author-email: dmitri_portnov@yahoo.com
 Requires-Python: >=3.8,<4.0
@@ -15,14 +15,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: click (>=8.0.4)
 Requires-Dist: loguru (>=0.6.0)
 Requires-Dist: numpy (>=1.23.2)
 Requires-Dist: openpyxl (>=3.0.9)
 Requires-Dist: pandas (>=1.4.1)
 Requires-Dist: tomli (>=2.0.1)
```

