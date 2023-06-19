# Comparing `tmp/irnl-rdt-correction-1.0.0.tar.gz` & `tmp/irnl-rdt-correction-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/irnl_rdt_correction/irnl_rdt_correction/dist/.tmp-sdobovi5/irnl-rdt-correction-1.0.0.tar", last modified: Fri Jan 20 10:11:42 2023, max compression
+gzip compressed data, was "irnl-rdt-correction-1.1.0.tar", last modified: Mon Jun 19 14:25:04 2023, max compression
```

## Comparing `irnl-rdt-correction-1.0.0.tar` & `irnl-rdt-correction-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 10:11:42.000000 irnl-rdt-correction-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-20 10:11:25.000000 irnl-rdt-correction-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-01-20 10:11:42.000000 irnl-rdt-correction-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-01-20 10:11:25.000000 irnl-rdt-correction-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 10:11:42.000000 irnl-rdt-correction-1.0.0/irnl_rdt_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-01-20 10:11:25.000000 irnl-rdt-correction-1.0.0/irnl_rdt_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-20 10:11:25.000000 irnl-rdt-correction-1.0.0/irnl_rdt_correction/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-01-20 10:11:25.000000 irnl-rdt-correction-1.0.0/irnl_rdt_correction/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    26181 2023-01-20 10:11:25.000000 irnl-rdt-correction-1.0.0/irnl_rdt_correction/equation_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-01-20 10:11:25.000000 irnl-rdt-correction-1.0.0/irnl_rdt_correction/input_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-01-20 10:11:25.000000 irnl-rdt-correction-1.0.0/irnl_rdt_correction/io_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-01-20 10:11:25.000000 irnl-rdt-correction-1.0.0/irnl_rdt_correction/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-01-20 10:11:25.000000 irnl-rdt-correction-1.0.0/irnl_rdt_correction/rdt_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-01-20 10:11:25.000000 irnl-rdt-correction-1.0.0/irnl_rdt_correction/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 10:11:42.000000 irnl-rdt-correction-1.0.0/irnl_rdt_correction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-01-20 10:11:42.000000 irnl-rdt-correction-1.0.0/irnl_rdt_correction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-01-20 10:11:42.000000 irnl-rdt-correction-1.0.0/irnl_rdt_correction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 10:11:42.000000 irnl-rdt-correction-1.0.0/irnl_rdt_correction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-01-20 10:11:42.000000 irnl-rdt-correction-1.0.0/irnl_rdt_correction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-20 10:11:42.000000 irnl-rdt-correction-1.0.0/irnl_rdt_correction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-01-20 10:11:42.000000 irnl-rdt-correction-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-01-20 10:11:25.000000 irnl-rdt-correction-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:25:04.226297 irnl-rdt-correction-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-19 14:24:43.000000 irnl-rdt-correction-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-06-19 14:25:04.226297 irnl-rdt-correction-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-06-19 14:24:43.000000 irnl-rdt-correction-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:25:04.222297 irnl-rdt-correction-1.1.0/irnl_rdt_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-19 14:24:43.000000 irnl-rdt-correction-1.1.0/irnl_rdt_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 14:24:43.000000 irnl-rdt-correction-1.1.0/irnl_rdt_correction/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-19 14:24:43.000000 irnl-rdt-correction-1.1.0/irnl_rdt_correction/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26181 2023-06-19 14:24:43.000000 irnl-rdt-correction-1.1.0/irnl_rdt_correction/equation_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-06-19 14:24:43.000000 irnl-rdt-correction-1.1.0/irnl_rdt_correction/input_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-06-19 14:24:43.000000 irnl-rdt-correction-1.1.0/irnl_rdt_correction/io_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-06-19 14:24:43.000000 irnl-rdt-correction-1.1.0/irnl_rdt_correction/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-06-19 14:24:43.000000 irnl-rdt-correction-1.1.0/irnl_rdt_correction/rdt_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-19 14:24:43.000000 irnl-rdt-correction-1.1.0/irnl_rdt_correction/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:25:04.226297 irnl-rdt-correction-1.1.0/irnl_rdt_correction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-06-19 14:25:04.000000 irnl-rdt-correction-1.1.0/irnl_rdt_correction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-19 14:25:04.000000 irnl-rdt-correction-1.1.0/irnl_rdt_correction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 14:25:04.000000 irnl-rdt-correction-1.1.0/irnl_rdt_correction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-19 14:25:04.000000 irnl-rdt-correction-1.1.0/irnl_rdt_correction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-19 14:25:04.000000 irnl-rdt-correction-1.1.0/irnl_rdt_correction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-19 14:25:04.226297 irnl-rdt-correction-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-19 14:24:43.000000 irnl-rdt-correction-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:25:04.226297 irnl-rdt-correction-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-06-19 14:24:43.000000 irnl-rdt-correction-1.1.0/tests/test_dual_optics_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-06-19 14:24:43.000000 irnl-rdt-correction-1.1.0/tests/test_feeddown_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-06-19 14:24:43.000000 irnl-rdt-correction-1.1.0/tests/test_rdts_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-06-19 14:24:43.000000 irnl-rdt-correction-1.1.0/tests/test_standard_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-06-19 14:24:43.000000 irnl-rdt-correction-1.1.0/tests/test_unit_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-06-19 14:24:43.000000 irnl-rdt-correction-1.1.0/tests/test_units.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `irnl-rdt-correction-1.0.0/LICENSE` & `irnl-rdt-correction-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `irnl-rdt-correction-1.0.0/PKG-INFO` & `irnl-rdt-correction-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: irnl-rdt-correction
-Version: 1.0.0
+Version: 1.1.0
 Summary: Correction script to power the nonlinear correctors in the (HL-)LHC insertion regions based on RDTs.
 Home-page: https://github.com/pylhc/irnl_rdt_correction
 Author: pylhc
 Author-email: pylhc@github.com
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: all
```

### Comparing `irnl-rdt-correction-1.0.0/README.md` & `irnl-rdt-correction-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `irnl-rdt-correction-1.0.0/irnl_rdt_correction/__init__.py` & `irnl-rdt-correction-1.1.0/irnl_rdt_correction/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 
 Correction script to power the nonlinear correctors in the (HL-)LHC insertion regions based on RDTs.
 
 :copyright: pyLHC/OMC-Team working group.
 :license: MIT, see the LICENSE.md file for details.
 """
 from irnl_rdt_correction.main import irnl_rdt_correction
+from irnl_rdt_correction.input_options import InputOptions
 
 __title__ = "irnl-rdt-correction"
 __description__ = "Correction script to power the nonlinear correctors in the (HL-)LHC insertion regions based on RDTs."
 __url__ = "https://github.com/pylhc/irnl_rdt_correction"
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 __author__ = "pylhc"
 __author_email__ = "pylhc@github.com"
 __license__ = "MIT"
 
-__all__ = [irnl_rdt_correction, __version__]
+__all__ = [irnl_rdt_correction, InputOptions, __version__]
```

### Comparing `irnl-rdt-correction-1.0.0/irnl_rdt_correction/constants.py` & `irnl-rdt-correction-1.1.0/irnl_rdt_correction/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,8 +30,9 @@
 
 # File Extensions ---
 EXT_TFS = ".tfs"  # suffix for dataframe file
 EXT_MADX = ".madx"  # suffix for madx-command file
 
 # Types ---
 StrOrPathOrDataFrame = Union[str, Path, DataFrame, TfsDataFrame]
+StrOrPathOrDataFrameOrNone = Union[str, Path, DataFrame, TfsDataFrame, None]
 RDTInputTypes = Union[Sequence[str], Dict[str, Sequence[str]]]
```

### Comparing `irnl-rdt-correction-1.0.0/irnl_rdt_correction/equation_system.py` & `irnl-rdt-correction-1.1.0/irnl_rdt_correction/equation_system.py`

 * *Files identical despite different names*

### Comparing `irnl-rdt-correction-1.0.0/irnl_rdt_correction/input_options.py` & `irnl-rdt-correction-1.1.0/irnl_rdt_correction/input_options.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,88 +2,55 @@
 Input Options
 -------------
 
 Handles the input parameters, contains their default values
 and checks for their validity.
 """
 import argparse
+from dataclasses import dataclass, fields
 import logging
 from pathlib import Path
-from typing import Iterable, Sized, Union
+from typing import Iterable, Optional, Sequence, Sized, Union, Tuple
 
 import pandas as pd
 import tfs
 
-from irnl_rdt_correction.constants import EXT_TFS, EXT_MADX
+from irnl_rdt_correction.constants import EXT_TFS, EXT_MADX, StrOrPathOrDataFrame, StrOrPathOrDataFrameOrNone
 from irnl_rdt_correction.equation_system import SOLVER_MAP
-from irnl_rdt_correction.utilities import list2str, DotDict
+from irnl_rdt_correction.utilities import list2str
 
 LOG = logging.getLogger(__name__)
 
 
-# Default Values ---------------------------------------------------------------
-
-DEFAULTS = {'feeddown': 0,
-            'ips': [1, 2, 5, 8],
-            'accel': 'lhc',
-            'solver': 'lstsq',
-            'update_optics': True,
-            'iterations': 1,
-            'ignore_corrector_settings': False,
-            'rdts2': None,
-            'ignore_missing_columns': False,
-            'output': None,
-            }
-
-DEFAULT_RDTS = {
-    'lhc': ('F0003', 'F0003*',  # correct a3 errors with F0003
-            'F1002', 'F1002*',  # correct b3 errors with F1002
-            'F1003', 'F3001',  # correct a4 errors with F1003 and F3001
-            'F4000', 'F0004',  # correct b4 errors with F4000 and F0004
-            'F6000', 'F0006',  # correct b6 errors with F6000 and F0006
-            ),
-    'hllhc': ('F0003', 'F0003*',  # correct a3 errors with F0003
-              'F1002', 'F1002*',  # correct b3 errors with F1002
-              'F1003', 'F3001',  # correct a4 errors with F1003 and F3001
-              'F0004', 'F4000',  # correct b4 errors with F0004 and F4000
-              'F0005', 'F0005*',  # correct a5 errors with F0005
-              'F5000', 'F5000*',  # correct b5 errors with F5000
-              'F5001', 'F1005',  # correct a6 errors with F5001 and F1005
-              'F6000', 'F0006',  # correct b6 errors with F6000 and F0006
-              ),
-}
-
-
 # Parser -----------------------------------------------------------------------
 
 def get_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser()
     parser.add_argument(
+        "--beams",
+        dest="beams",
+        type=int,
+        nargs="+",
+        help="Which beam the files come from (1, 2 or 4)",
+        required=True,
+    )
+    parser.add_argument(
         "--twiss",
         dest="twiss",
         nargs="+",
         help="Path(s) to twiss file(s), in the format of MAD-X `twiss` output. "
              "Defines which elements to correct for,"
              "meaning all given elements contribute to the correction!",
         required=True,
     )
     parser.add_argument(
         "--errors",
         dest="errors",
         nargs="+",
         help="Path(s) to error file(s), in the format of MAD-X `esave` output.",
-        required=True,
-    )
-    parser.add_argument(
-        "--beams",
-        dest="beams",
-        type=int,
-        nargs="+",
-        help="Which beam the files come from (1, 2 or 4)",
-        required=True,
     )
     parser.add_argument(
         "--output",
         dest="output",
         help=("Path to write command and tfs_df file. "
               f"Extension (if given) is ignored and replaced with {EXT_TFS} and {EXT_MADX} "
               "for the Dataframe and the command file respectively."
@@ -105,58 +72,58 @@
         help=("RDTs to correct for second beam/file, if different from first."
               " Same format rules as for `rdts`."),
     )
     parser.add_argument(
         "--accel",
         dest="accel",
         type=str.lower,
-        choices=list(DEFAULT_RDTS.keys()),
-        default=DEFAULTS['accel'],
+        choices=list(InputOptions.DEFAULT_RDTS.keys()),
+        default=InputOptions.accel,
         help="Which accelerator we have.",
     )
     parser.add_argument(
         "--feeddown",
         dest="feeddown",
         type=int,
         help="Order of Feeddown to include.",
-        default=DEFAULTS['feeddown'],
+        default=InputOptions.feeddown,
     )
     parser.add_argument(
         "--ips",
         dest="ips",
         nargs="+",
         help="In which IPs to correct.",
         type=int,
-        default=DEFAULTS['ips'],
+        default=list(InputOptions.ips),
     )
     parser.add_argument(
         "--solver",
         dest="solver",
         help="Solving method to use.",
         type=str.lower,
         choices=list(SOLVER_MAP.keys()),
-        default=DEFAULTS['solver'],
+        default=InputOptions.solver,
     )
     parser.add_argument(
         "--update_optics",
         dest="update_optics",
         type=bool,
         help=("Sorts the RDTs to start with the highest order and updates the "
               "corrector strengths in the optics after calculation, so the "
               "feeddown to lower order correctors is included."
               ),
-        default=DEFAULTS["update_optics"]
+        default=InputOptions.update_optics
     )
     parser.add_argument(
         "--iterations",
         dest="iterations",
         type=int,
         help=("Reiterate correction, "
               "starting with the previously calculated values."),
-        default=DEFAULTS["iterations"]
+        default=InputOptions.iterations
     )
     parser.add_argument(
         "--ignore_corrector_settings",
         dest="ignore_corrector_settings",
         help=("Ignore the current settings of the correctors. If this is not set "
               "the corrector values of the optics are used as initial conditions."),
         action="store_true",
@@ -166,82 +133,163 @@
         dest="ignore_missing_columns",
         help=("If set, missing strength columns in any of the input files "
               "are assumed to be zero, instead of raising an error."),
         action="store_true",
     )
     return parser
 
+# InputOptions and Defaults ---------------------------------------------------------------
 
-# Checks -----------------------------------------------------------------------
-
-def check_opt(opt: Union[dict, DotDict]) -> DotDict:
-    """ Asserts that the input parameters make sense and adds what's missing.
-    If the input is empty, arguments will be parsed from commandline.
+@dataclass
+class InputOptions:
+    """ DataClass to store the input options.
+    On creation it asserts that the input parameters make sense and adds what's missing.
     Checks include:
-        - Set defaults (see ``DEFAULTS``) if option not given.
         - Check accelerator name is valid
         - Set default RDTs if not given (see ``DEFAULT_RDTS``)
         - Check required parameters are present (twiss, errors, beams, rdts)
         - Check feeddown and iterations
 
-    TODO: Replace DotDict with dataclass and have class check most of this...
-
-    Args:
-        opt (Union[dict, DotDict]): Function options in dictionary format.
-                                Description of the arguments are given in
-                                :func:`irnl_rdt_correction.main.irnl_rdt_correction`.
-
-    Returns:
-        DotDict: (Parsed and) checked options.
-
     """
-    # check for unkown input
-    parser = get_parser()
-    if not len(opt):
-        opt = vars(parser.parse_args())
-    opt = DotDict(opt)
-    known_opts = [a.dest for a in parser._actions if not isinstance(a, argparse._HelpAction)]  # best way I could figure out
-    unknown_opts = [k for k in opt.keys() if k not in known_opts]
-    if len(unknown_opts):
-        raise AttributeError(f"Unknown arguments found: '{list2str(unknown_opts)}'.\n"
-                             f"Allowed input parameters are: '{list2str(known_opts)}'")
-
-    # Set defaults
-    for name, default in DEFAULTS.items():
-        if opt.get(name) is None:
-            LOG.debug(f"Setting input '{name}' to default value '{default}'.")
-            opt[name] = default
-
-    # check accel
-    opt.accel = opt.accel.lower()  # let's not care about case
-    if opt.accel not in DEFAULT_RDTS.keys():
-        raise ValueError(f"Parameter 'accel' needs to be one of '{list2str(list(DEFAULT_RDTS.keys()))}' "
-                         f"but was '{opt.accel}' instead.")
-
-    # Set rdts:
-    if opt.get('rdts') is None:
-        opt.rdts = DEFAULT_RDTS[opt.accel]
-
-    # Check required and rdts:
-    for name in ('twiss', 'errors', 'beams', 'rdts'):
-        inputs = opt.get(name)
-        if inputs is None or isinstance(inputs, str) or not isinstance(inputs, (Iterable, Sized)):
-            raise ValueError(f"Parameter '{name}' is required and needs to be "
-                             "iterable, even if only of length 1. "
-                             f"Instead was '{inputs}'.")
-
-    # Check twiss and errors input type
-    for name in ('twiss', 'errors'):
-        inputs = opt.get(name)
-        for element in inputs:
-            if not isinstance(element, (str, Path, pd.DataFrame, tfs.TfsDataFrame)):
-                raise TypeError(f"Not all elements of '{name}' are DataFrames or paths to DataFrames!")
-
-    if opt.feeddown < 0 or not (opt.feeddown == int(opt.feeddown)):
-        raise ValueError("'feeddown' needs to be a positive integer.")
-
-    if opt.iterations < 1:
-        raise ValueError("At least one iteration (see: 'iterations') needs to "
-                         "be done for correction.")
-    return opt
-
+    DEFAULT_RDTS = {
+        'lhc': ('F0003', 'F0003*',  # correct a3 errors with F0003
+                'F1002', 'F1002*',  # correct b3 errors with F1002
+                'F1003', 'F3001',  # correct a4 errors with F1003 and F3001
+                'F4000', 'F0004',  # correct b4 errors with F4000 and F0004
+                'F6000', 'F0006',  # correct b6 errors with F6000 and F0006
+                ),
+        'hllhc': ('F0003', 'F0003*',  # correct a3 errors with F0003
+                'F1002', 'F1002*',  # correct b3 errors with F1002
+                'F1003', 'F3001',  # correct a4 errors with F1003 and F3001
+                'F0004', 'F4000',  # correct b4 errors with F0004 and F4000
+                'F0005', 'F0005*',  # correct a5 errors with F0005
+                'F5000', 'F5000*',  # correct b5 errors with F5000
+                'F5001', 'F1005',  # correct a6 errors with F5001 and F1005
+                'F6000', 'F0006',  # correct b6 errors with F6000 and F0006
+                ),
+    }
+
+    beams: Sequence[int]
+    twiss: Sequence[StrOrPathOrDataFrame]
+    errors: Sequence[StrOrPathOrDataFrameOrNone] = None
+    rdts: Sequence[str] = None
+    rdts2: Sequence[str] = None
+    accel: str = 'lhc'
+    feeddown: int = 0
+    ips: Sequence[int] = (1, 2, 5, 8)
+    solver: str ='lstsq'
+    update_optics: bool = True
+    iterations: int = 1
+    ignore_corrector_settings: bool = False
+    ignore_missing_columns: bool = False
+    output: str = None
+
+    def __post_init__(self):
+        self.check_all()
+
+    def __getitem__(self, item):
+        return getattr(self, item)
+    
+    @classmethod
+    def keys(cls):
+        return (f.name for f in fields(cls))
+
+    def values(self):
+        return (getattr(self, f.name) for f in fields(self))
+    
+    def items(self):
+        return ((f.name, getattr(self, f.name)) for f in fields(self))
+
+    def check_all(self):
+        self.check_accel()
+        self.check_twiss()
+        self.check_errors()
+        self.check_beams()
+        self.check_rdts()
+        self.check_feeddown()
+        self.check_iterations()
+
+    def check_accel(self):
+        if self.accel not in self.DEFAULT_RDTS:
+            raise ValueError(f"Parameter 'accel' needs to be one of '{list2str(list(self.DEFAULT_RDTS.keys()))}' "
+                            f"but was '{self.accel}' instead.")
+
+    def check_twiss(self):
+        if self.twiss is None:
+            raise ValueError("Parameter 'twiss' needs to be set.")
 
+        self._check_iterable('twiss') 
+        for element in self.twiss:
+            if not isinstance(element, (str, Path, pd.DataFrame, tfs.TfsDataFrame)):
+                raise TypeError(f"Not all elements of 'twiss' are DataFrames or paths to DataFrames!")
+    
+    def check_errors(self):
+        if self.errors is None:
+            self.errors = tuple([None] * len(self.twiss))
+            return
+
+        self._check_iterable('errors')
+        for element in self.errors:
+            if not isinstance(element, (str, Path, pd.DataFrame, tfs.TfsDataFrame, type(None))):
+                raise TypeError(f"Not all elements of 'errors' are DataFrames or paths to DataFrames or None!")
+    
+    def check_beams(self):
+        if self.beams is None:
+            raise ValueError("Parameter 'beams' needs to be set.")
+        self._check_iterable('beams') 
+    
+    def check_rdts(self):
+        if self.rdts is None:
+            self.rdts = self.DEFAULT_RDTS[self.accel]
+        else:
+            self._check_iterable('rdts')
+    
+    def check_feeddown(self):
+        if self.feeddown < 0 or not (self.feeddown == int(self.feeddown)):
+            raise ValueError("'feeddown' needs to be a positive integer.")
+
+    def check_iterations(self):
+        if self.iterations < 1:
+            raise ValueError("At least one iteration (see: 'iterations') needs to "
+                            "be done for correction.")
+
+    def _check_iterable(self, name):
+        inputs = getattr(self, name)
+        if isinstance(inputs, str) or not isinstance(inputs, (Iterable, Sized)):
+            raise ValueError(f"Parameter '{name}' needs to be iterable, "
+                             f"even if only of length 1. Instead was '{inputs}'.")
+
+    @classmethod
+    def from_args_or_dict(cls, opt: Optional[Union[dict, 'InputOptions']] = None) -> 'InputOptions':
+        """Create an InputOptions instance from the given dictionary.
+        If the input is empty, arguments will be parsed from commandline.
+
+        Args:
+            opt (Union[dict, DotDict]): Function options in dictionary format.
+                                    Description of the arguments are given in
+                                    :func:`irnl_rdt_correction.main.irnl_rdt_correction`.
+                                    Optional, if not given parses commandline args
+
+        Returns:
+            InputOptions: (Parsed and) checked options.
+        """
+        if isinstance(opt, InputOptions):
+            return opt
+
+        if opt is None or not len(opt):
+            parser = get_parser()
+            opt = vars(parser.parse_args())
+            
+        return cls(**opt)
+
+
+def allow_commandline_and_kwargs(func):
+    """ Decorator to allow a function to take options from the commandline
+    or via kwargs, or given an InputOptions instance. 
+    """
+    def wrapper(opt: Optional[Union[InputOptions, dict]] = None, **kwargs) -> Tuple[str, tfs.TfsDataFrame]:
+        if not isinstance(opt, InputOptions):
+            if opt is None:
+                opt = kwargs
+            opt = InputOptions.from_args_or_dict(opt)
+        return func(opt)
+    return wrapper
```

### Comparing `irnl-rdt-correction-1.0.0/irnl_rdt_correction/io_handling.py` & `irnl-rdt-correction-1.1.0/irnl_rdt_correction/io_handling.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,50 +3,52 @@
 -----------
 
 Functions for reading input and writing output.
 
 """
 import logging
 from pathlib import Path
-from typing import Sequence, Iterable, Tuple, Union
+from typing import Optional, Sequence, Iterable, Tuple, Union
 
 import pandas as pd
 import tfs
 from pandas import DataFrame
 from tfs import TfsDataFrame
 
-from irnl_rdt_correction.constants import PLANES, DELTA, EXT_MADX, EXT_TFS, StrOrPathOrDataFrame
+from irnl_rdt_correction.constants import PLANES, DELTA, EXT_MADX, EXT_TFS, StrOrPathOrDataFrame, StrOrPathOrDataFrameOrNone
 from irnl_rdt_correction.utilities import is_anti_mirror_symmetric, idx2str, list2str, Optics
 from irnl_rdt_correction.rdt_handling import IRCorrector
 
 LOG = logging.getLogger(__name__)
 X, Y = PLANES
 
 
 # Input ------------------------------------------------------------------------
 
 
 def get_optics(beams: Sequence[int],
-               twiss: Sequence[StrOrPathOrDataFrame], errors: Sequence[StrOrPathOrDataFrame],
+               twiss: Sequence[StrOrPathOrDataFrame], errors: Sequence[StrOrPathOrDataFrameOrNone],
                orders: Sequence[int], ignore_missing_columns: bool) -> Tuple[Optics]:
     """Get the Optics instances from beams, twiss and errors.
     Also checks the DataFrames for containing needed information.
 
     Args:
         beams (Sequence[int]): Beam number the twiss/errors refer to
-        twiss (Sequence[StrOrPathOrDataFrame]): 
-        errors (Sequence[StrOrPathOrDataFrame]):
+        twiss (Sequence[StrOrPathOrDataFrame]): Sequence of twiss TfsDataFrames or paths to the tfs files.
+        errors (Sequence[StrOrPathOrDataFrame]): Sequence of errors TfsDataFrames or paths to the tfs files. Can be `None`.
         orders (Sequence[int]): Orders needed for calculations (used to check DataFrames)
         ignore_missing_columns (bool): If set, fills missing columns with zeros.
 
     Returns:
         Sequence[Optics]: Tuple of Optics objects containing combined information
                           about beam, twiss and errors.
     """
     twiss_dfs = get_tfs(twiss)
+
+    errors = _check_errors(errors, ignore_missing_columns)  
     errors_dfs = get_tfs(errors)
 
     beams, twiss_dfs, errors_dfs = _check_dfs(
         beams=beams, twiss_dfs=twiss_dfs, errors_dfs=errors_dfs,
         orders=orders, ignore_missing_columns=ignore_missing_columns
     )
     optics_seq = tuple(Optics(beam=b, twiss=o, errors=e) for b, o, e in zip(beams, twiss_dfs, errors_dfs))
@@ -177,27 +179,59 @@
     """ Write the correction dataframe as TFS-file. """
     out_path_df = out_path.with_suffix(EXT_TFS)
     tfs.write(out_path_df, correction_df)
 
 
 # Utils ------------------------------------------------------------------------
 
+
+def _check_errors(errors: Sequence[StrOrPathOrDataFrameOrNone], 
+                  ignore_missing_columns: bool = False) -> Tuple[StrOrPathOrDataFrame, ...]:
+    """Check the given errors for None-type and fill with empty dataframes.
+    This only makes sense if `ignore_missing_columns` is set to `True` 
+    as these DataFrames obviously have all columns missing, so we check for that here as well.
+
+    Args:
+        errors (Sequence[StrOrPathOrDataFrameOrNone]): Sequence of given errors, 
+                                                       i.e. either DataFrames or paths to tfs files.
+        ignore_missing_columns (bool, optional): Whether to ignore missing columns. Defaults to False.
+
+    Returns:
+        tuple[StrOrPathOrDataFrame, ...]: Tuple with Nones filled with empty TfsDataFrames. 
+    """
+    if all(e is not None for e in errors):
+        return errors
+
+    if not ignore_missing_columns:
+        raise ValueError("None-type errors given, but `ignore_missing_columns` is set to `False`. "
+        "Either specify errors or set `ignore_missing_columns` to `True`.")
+
+    return tuple(TfsDataFrame() if e is None else e for e in errors)
+
+
 def _check_dfs(beams: Sequence[int], twiss_dfs: Sequence[DataFrame], errors_dfs: Sequence[DataFrame],
                orders: Sequence[int], ignore_missing_columns: bool
                ) -> Tuple[Sequence[int], Sequence[DataFrame], Sequence[DataFrame]]:
     """ Check the read optics and error dataframes for validity.
     Checks:
         - Maximum 2 optics
         - Equal lenghts for twiss/errors/beams
         - All elements in errors are also in twiss -> Error if not
         - All elements in twiss are also in errors -> Debug msg if not
         - All needed field strengths are present in twiss
           -> either Error or Warning depending on ``ignore_missing_columns``.
     """
-    twiss_dfs, errors_dfs = tuple(tuple(df.copy() for df in dfs) for dfs in (twiss_dfs, errors_dfs))
+    twiss_dfs, errors_dfs = tuple(tuple(df.copy() for df in dfs) 
+                                  for dfs in (twiss_dfs, errors_dfs))
+
+    needed_twiss = list(PLANES)
+    needed_errors = [f"{DELTA}{p}" for p in PLANES]
+    needed_k = [f"K{order-1:d}{orientation}L"  # -1 for madx-order
+                for order in orders
+                for orientation in ("S", "")]
 
     if len(twiss_dfs) > 2 or len(errors_dfs) > 2:
         raise NotImplementedError("A maximum of two optics can be corrected "
                                   "at the same time, for now.")
 
     if len(twiss_dfs) != len(errors_dfs):
         raise ValueError(f"The number of given optics ({len(twiss_dfs):d}) "
@@ -206,45 +240,43 @@
 
     if len(twiss_dfs) != len(beams):
         raise ValueError(f"The number of given optics ({len(twiss_dfs):d}) "
                          "does not equal the number of given beams "
                          f"({len(beams):d}). Please specify a beam for each "
                          "optics.")
 
-    for idx_file, (optics, errors) in enumerate(zip(twiss_dfs, errors_dfs)):
-        not_found_errors = errors.index.difference(optics.index)
+    for idx_file, (twiss, errors) in enumerate(zip(twiss_dfs, errors_dfs)):
+        not_found_errors = errors.index.difference(twiss.index)
         if len(not_found_errors):
             raise IOError("The following elements were found in the "
                           f"{idx2str(idx_file)} given errors file but not in"
                           f"the optics: {list2str(not_found_errors.to_list())}")
 
-        not_found_optics = optics.index.difference(errors.index)
+        not_found_optics = twiss.index.difference(errors.index)
         if len(not_found_optics):
             LOG.debug("The following elements were found in the "
                       f"{idx2str(idx_file)} given optics file but not in "
                       f"the errors: {list2str(not_found_optics.to_list())}."
                       f"They are assumed to be zero.")
             for indx in not_found_optics:
                 errors.loc[indx, :] = 0
 
-        needed_values = [f"K{order-1:d}{orientation}L"  # -1 for madx-order
-                         for order in orders
-                         for orientation in ("S", "")]
-
-        for df, file_type in ((optics, "optics"), (errors, "error")):
-            not_found_strengths = [s for s in needed_values if s not in df.columns]
-            if len(not_found_strengths):
-                text = ("Some strength values were not found in the "
+        for df, needed_cols, file_type in ((
+            twiss, needed_twiss, "twiss"), (errors, needed_errors, "error")
+            ):
+            missing_cols = [s for s in needed_cols + needed_k if s not in df.columns]
+            if len(missing_cols):
+                text = ("Some strength values/columns were not found in the "
                         f"{idx2str(idx_file)} given {file_type} file: "
-                        f"{list2str(not_found_strengths)}.")
+                        f"{list2str(missing_cols)}.")
 
                 if not ignore_missing_columns:
                     raise IOError(text)
                 LOG.warning(text + " They are assumed to be zero.")
-                for kl in not_found_strengths:
+                for kl in missing_cols:
                     df[kl] = 0
     return beams, twiss_dfs, errors_dfs
 
 
 def maybe_switch_signs(optics: Optics):
     """ Switch the signs for Beam optics.
      This is due to the switch in direction between beam and
```

### Comparing `irnl-rdt-correction-1.0.0/irnl_rdt_correction/main.py` & `irnl-rdt-correction-1.1.0/irnl_rdt_correction/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,14 @@
 Performs local correction of the Resonance Driving Terms (RDTs)
 in the Insertion Regions (IRs) based on the principle described in
 [BruningDynamicApertureStudies2004]_ with the addition of correcting
 feed-down and using feed-down to correct lower order RDTs.
 Details can be found in [DillyNonlinearIRCorrections2023]_ .
 
 TODO:
- - [easy] Allow not giving errors (need to be `None` in list,
-   so that the list lengths are still the same and there is a
-   clear correspondence twiss-errors-beams).
-   Should then be assumed all zero.
  - [easy] Allow for more than two optics given
    (e.g. find corrections for 15cm and 30cm for both beams)
  - [medium] Maybe sort RDTs by highest corrector instead of highest RDT order?
    This should allow for correctors that correct via feed-down
    to be assigned before lower order RDTs are calculated.
    Might cause other problems, though. To be thought about.
  - [medium] Consider switching the signs all into the reference frame of Beam 1.
@@ -54,36 +50,36 @@
 """
 import logging
 from typing import Tuple
 
 import tfs
 
 from irnl_rdt_correction.equation_system import solve
-from irnl_rdt_correction.input_options import check_opt
+from irnl_rdt_correction.input_options import InputOptions, allow_commandline_and_kwargs
 from irnl_rdt_correction.io_handling import get_and_write_output, get_optics
 from irnl_rdt_correction.rdt_handling import sort_rdts, check_corrector_order, get_needed_orders
 from irnl_rdt_correction.utilities import Timer, log_setup
 
 LOG = logging.getLogger(__name__)
 
-
-def irnl_rdt_correction(**opt) -> Tuple[str, tfs.TfsDataFrame]:
+@allow_commandline_and_kwargs
+def irnl_rdt_correction(opt: InputOptions) -> Tuple[str, tfs.TfsDataFrame]:
     """ Get correctors and their optimal powering to minimize the given RDTs.
 
     Keyword Args:
 
         twiss (list[str/Path/DataFrame]): Path(s) to twiss file(s) or DataFrame(s) of optics.
                                            Needs to contain only the elements to be corrected
                                            (e.g. only the ones in the IRs).
                                            All elements from the error-files need to be present.
                                            Required!
-        errors (list[str/Path/DataFrame]): Path(s) to error file(s) or DataFrame(s) of errors.
-                                           Can contain less elements than the optics files,
-                                           these elements are then assumed to have no errors.
-                                           Required!
+        errors (list[str/Path/DataFrame/None]): Path(s) to error file(s) or DataFrame(s) of errors.
+                                                Can contain less elements than the optics files,
+                                                these elements are then assumed to have no errors.
+                                                Optional! 
         beams (list[int]): Which beam the files come from (1, 2 or 4).
                            Required!
         output (str/Path): Path to write command and tfs_df file.
                            Extension (if given) is ignored and replaced with '.tfs' and '.madx'
                            for the Dataframe and the command file respectively.
                            Default: ``None``.
         rdts (list[str], dict[str, list[str]):
@@ -96,15 +92,15 @@
                           where the keys are the RDT names as before, and the values are a list
                           of correctors to use, e.g. 'b5' for normal decapole corrector,
                           'a3' for skew sextupole, etc.
                           If the order of the corrector is higher than the order of the RDT,
                           the feed-down from the corrector is used for correction.
                           In the case where multiple orders of correctors are used,
                           increasing ``iterations`` might be useful.
-                          Default: Standard RDTs for given ``accel`` (see ``DEFAULT_RDTS`` in this file).
+                          Default: Standard RDTs for given ``accel`` (see ``InputOptions.DEFAULT_RDTS``).
         rdts2 (list[str], dict[str, list[str]):
                            RDTs to correct for second beam/file, if different from first.
                            Same format rules as for ``rdts``. Default: ``None``.
         accel (str): Which accelerator we have. One of 'lhc', 'hllhc'.
                      Default: ``lhc``.
         feeddown (int): Order of Feeddown to include.
                         Default: ``0``.
@@ -135,16 +131,14 @@
 
         tuple[string, Dataframe]:
         the string contains the madx-commands used to power the correctors;
         the dataframe contains the same values in a pandas DataFrame.
     """
     LOG.info("Starting IRNL Correction.")
     timer = Timer("Start", print_fun=LOG.debug)
-    opt = check_opt(opt)
-    timer.step("Opt Parsed.")
 
     rdt_maps = sort_rdts(opt.rdts, opt.rdts2)
     check_corrector_order(rdt_maps, update_optics=opt.update_optics, feed_down=opt.feeddown)
     needed_orders = get_needed_orders(rdt_maps, opt.feeddown)
     timer.step("RDT Sorted.")
 
     optics = get_optics(
@@ -170,12 +164,13 @@
     timer.summary()
     if len(correctors) == 0:
         raise EnvironmentError('No correctors found in input optics.')
 
     return get_and_write_output(opt.output, correctors)
 
 
+
 # Script Mode ------------------------------------------------------------------
 
 if __name__ == '__main__':
     log_setup()
     irnl_rdt_correction()
```

### Comparing `irnl-rdt-correction-1.0.0/irnl_rdt_correction/rdt_handling.py` & `irnl-rdt-correction-1.1.0/irnl_rdt_correction/rdt_handling.py`

 * *Files identical despite different names*

### Comparing `irnl-rdt-correction-1.0.0/irnl_rdt_correction/utilities.py` & `irnl-rdt-correction-1.1.0/irnl_rdt_correction/utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,32 +15,14 @@
 from tfs import TfsDataFrame
 
 from irnl_rdt_correction.constants import SKEW_NAME_MAP, SKEW_FIELD_MAP, FIELD_SKEW_MAP
 
 
 # Classes ----------------------------------------------------------------------
 
-class DotDict(dict):
-    """ Make dict fields accessible by attributes.
-    TODO: Replace with dataclass.
-    """
-    def __init__(self, *args, **kwargs):
-        super(DotDict, self).__init__(*args, **kwargs)
-
-    __setattr__ = dict.__setitem__
-    __delattr__ = dict.__delitem__
-
-    def __getattr__(self, key):
-        """ Needed to raise the correct exceptions """
-        try:
-            return super(DotDict, self).__getitem__(key)
-        except KeyError as e:
-            raise AttributeError(e).with_traceback(e.__traceback__) from e
-
-
 class Timer:
     """ Collect Times and print a summary at the end. """
     def __init__(self, name: str = "start", print_fun: Callable[[str], None] = print):
         self.steps = {}
         self.step(name)
         self.print = print_fun
```

### Comparing `irnl-rdt-correction-1.0.0/irnl_rdt_correction.egg-info/PKG-INFO` & `irnl-rdt-correction-1.1.0/irnl_rdt_correction.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: irnl-rdt-correction
-Version: 1.0.0
+Version: 1.1.0
 Summary: Correction script to power the nonlinear correctors in the (HL-)LHC insertion regions based on RDTs.
 Home-page: https://github.com/pylhc/irnl_rdt_correction
 Author: pylhc
 Author-email: pylhc@github.com
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: all
```

### Comparing `irnl-rdt-correction-1.0.0/setup.py` & `irnl-rdt-correction-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -65,18 +65,18 @@
     license=ABOUT_PYLHC["__license__"],
     classifiers=[
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Physics",
         "Topic :: Scientific/Engineering :: Visualization",
     ],
     packages=setuptools.find_packages(exclude=["tests*", "doc"]),
     include_package_data=True,
     install_requires=DEPENDENCIES,
     tests_require=EXTRA_DEPENDENCIES["test"],
```

