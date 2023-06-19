# Comparing `tmp/dpamber-0.2.2.tar.gz` & `tmp/dpamber-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpamber-0.2.2.tar", last modified: Mon Oct 10 20:56:13 2022, max compression
+gzip compressed data, was "dpamber-0.3.1.tar", last modified: Mon Jun 19 07:38:21 2023, max compression
```

## Comparing `dpamber-0.2.2.tar` & `dpamber-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 20:56:13.297727 dpamber-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 20:56:13.297727 dpamber-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 20:56:13.297727 dpamber-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-10-10 20:56:04.000000 dpamber-0.2.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-10-10 20:56:04.000000 dpamber-0.2.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-10-10 20:56:13.297727 dpamber-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-10-10 20:56:04.000000 dpamber-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 20:56:13.297727 dpamber-0.2.2/dpamber/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 20:56:04.000000 dpamber-0.2.2/dpamber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3690 2022-10-10 20:56:04.000000 dpamber-0.2.2/dpamber/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2980 2022-10-10 20:56:04.000000 dpamber-0.2.2/dpamber/corr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2226 2022-10-10 20:56:04.000000 dpamber-0.2.2/dpamber/model_devi.py
--rw-r--r--   0 runner    (1001) docker     (121)     4944 2022-10-10 20:56:04.000000 dpamber-0.2.2/dpamber/qmbuffer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1890 2022-10-10 20:56:04.000000 dpamber-0.2.2/dpamber/qmwater_corr.py
--rw-r--r--   0 runner    (1001) docker     (121)     5847 2022-10-10 20:56:04.000000 dpamber-0.2.2/dpamber/read_amber.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 20:56:13.297727 dpamber-0.2.2/dpamber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-10-10 20:56:13.000000 dpamber-0.2.2/dpamber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-10-10 20:56:13.000000 dpamber-0.2.2/dpamber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-10 20:56:13.000000 dpamber-0.2.2/dpamber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-10-10 20:56:13.000000 dpamber-0.2.2/dpamber.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-10-10 20:56:13.000000 dpamber-0.2.2/dpamber.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-10 20:56:13.000000 dpamber-0.2.2/dpamber.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-10-10 20:56:04.000000 dpamber-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-10 20:56:13.297727 dpamber-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-10 20:56:04.000000 dpamber-0.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.883931 dpamber-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.875931 dpamber-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.879931 dpamber-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-19 07:38:12.000000 dpamber-0.3.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-19 07:38:12.000000 dpamber-0.3.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-19 07:38:12.000000 dpamber-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-19 07:38:12.000000 dpamber-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-19 07:38:21.883931 dpamber-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-19 07:38:12.000000 dpamber-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.879931 dpamber-0.3.1/dpamber/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-19 07:38:12.000000 dpamber-0.3.1/dpamber/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-19 07:38:12.000000 dpamber-0.3.1/dpamber/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-19 07:38:12.000000 dpamber-0.3.1/dpamber/corr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-19 07:38:12.000000 dpamber-0.3.1/dpamber/model_devi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-19 07:38:12.000000 dpamber-0.3.1/dpamber/qmbuffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-19 07:38:12.000000 dpamber-0.3.1/dpamber/qmwater_corr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-06-19 07:38:12.000000 dpamber-0.3.1/dpamber/read_amber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-19 07:38:12.000000 dpamber-0.3.1/dpamber/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.879931 dpamber-0.3.1/dpamber.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-19 07:38:21.000000 dpamber-0.3.1/dpamber.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-19 07:38:21.000000 dpamber-0.3.1/dpamber.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 07:38:21.000000 dpamber-0.3.1/dpamber.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-19 07:38:21.000000 dpamber-0.3.1/dpamber.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-19 07:38:21.000000 dpamber-0.3.1/dpamber.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 07:38:21.000000 dpamber-0.3.1/dpamber.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-19 07:38:12.000000 dpamber-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-19 07:38:12.000000 dpamber-0.3.1/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 07:38:21.883931 dpamber-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.879931 dpamber-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.883931 dpamber-0.3.1/tests/corr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.875931 dpamber-0.3.1/tests/corr/dataset/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.883931 dpamber-0.3.1/tests/corr/dataset/C6H11HW168O6OW83P1/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/dataset/C6H11HW168O6OW83P1/box.raw
+-rw-r--r--   0 runner    (1001) docker     (123)    20625 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/dataset/C6H11HW168O6OW83P1/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/dataset/C6H11HW168O6OW83P1/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (123)    21026 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/dataset/C6H11HW168O6OW83P1/force.raw
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/dataset/C6H11HW168O6OW83P1/nopbc
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/dataset/C6H11HW168O6OW83P1/type.raw
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/dataset/C6H11HW168O6OW83P1/type_map.raw
+-rw-r--r--   0 runner    (1001) docker     (123)    73252 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/high_level.mdfrc
+-rw-r--r--   0 runner    (1001) docker     (123)    27097 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/high_level.mdout
+-rw-r--r--   0 runner    (1001) docker     (123)    73252 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/low_level.mdfrc
+-rw-r--r--   0 runner    (1001) docker     (123)    27017 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/low_level.mdout
+-rw-r--r--   0 runner    (1001) docker     (123)  1036937 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/qmmm.parm7
+-rw-r--r--   0 runner    (1001) docker     (123)    97988 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/rc.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.883931 dpamber-0.3.1/tests/md/
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/md/md.mdout
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/test_corr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/test_model_devi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.883931 dpamber-0.3.1/tests/uncoverage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/uncoverage/uncoverage.mdout
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-19 07:38:12.000000 dpamber-0.3.1/tox.ini
```

### Comparing `dpamber-0.2.2/PKG-INFO` & `dpamber-0.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: dpamber
-Version: 0.2.2
+Version: 0.3.1
 Summary: Some useful tools related to Amber and DP.
 Project-URL: Homepage, https://github.com/njzjz/dpamber
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dpcpu
+Provides-Extra: dpgpu
 
 # dpamber
 
 Some useful tools related to Amber and DP.
 
 ## Installation
 
@@ -45,7 +48,17 @@
 An example of the command is
 ```sh
 dpamber corr --cutoff 6. --qm_region ":1" --parm7_file some_param.param7 --nc some_coord.nc --hl high_level --ll low_level --out dataset
 ```
 where `--cutoff` takes cutoff radius of the QM/MM interaction for training. `--qm_region` takes AMBER mask format for the QM region. `--parm7_file` and `--nc` take the PARM7 file and the trajectory (NetCDF) file, respectively. `--ll` and `--hl` are the prefixes of low-level and high-level files, including the mdout file (`.mdout`), the mden file (`.mden`) and the mdfrc file (`.mdfrc`). The output dataset directory should be put in `--out`.
 
 See details from `dpamber corr -h`.
+
+### model-devi: calculate model deviation
+
+`model-devi` can be used to calculate the model deviation of a given trajectory.
+You need to install DeePMD-kit using
+```sh
+pip install dpamber[dpgpu]
+```
+
+See `dpamber model-devi -h` for details.
```

### Comparing `dpamber-0.2.2/README.md` & `dpamber-0.3.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -35,7 +35,17 @@
 An example of the command is
 ```sh
 dpamber corr --cutoff 6. --qm_region ":1" --parm7_file some_param.param7 --nc some_coord.nc --hl high_level --ll low_level --out dataset
 ```
 where `--cutoff` takes cutoff radius of the QM/MM interaction for training. `--qm_region` takes AMBER mask format for the QM region. `--parm7_file` and `--nc` take the PARM7 file and the trajectory (NetCDF) file, respectively. `--ll` and `--hl` are the prefixes of low-level and high-level files, including the mdout file (`.mdout`), the mden file (`.mden`) and the mdfrc file (`.mdfrc`). The output dataset directory should be put in `--out`.
 
 See details from `dpamber corr -h`.
+
+### model-devi: calculate model deviation
+
+`model-devi` can be used to calculate the model deviation of a given trajectory.
+You need to install DeePMD-kit using
+```sh
+pip install dpamber[dpgpu]
+```
+
+See `dpamber model-devi -h` for details.
```

### Comparing `dpamber-0.2.2/dpamber/cli.py` & `dpamber-0.3.1/dpamber/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,88 @@
 import argparse
 
-from .model_devi import run as model_devi_run
 from .corr import run as corr_run
+from .model_devi import run as model_devi_run
 from .qmbuffer import run as qmwater_run
 from .qmwater_corr import run as qmwater_corr_run
 
 
 def run():
     parser = argparse.ArgumentParser()
     subparsers = parser.add_subparsers()
     parser_model_devi = subparsers.add_parser(
-        "devi", help="Calculate model deviations.")
-    parser_model_devi.add_argument('--models', type=str, nargs='+',
-                                   help="models")
-    parser_model_devi.add_argument('--cutoff', type=float,
-                                   help="cutoff")
-    parser_model_devi.add_argument('--parm7_file', type=str, default="qmmm.parm7",
-                                   help="parm7_file")
-    parser_model_devi.add_argument('--qm_region', type=str, default=":1",
-                                   help="qm_region")
+        "devi", help="Calculate model deviations."
+    )
+    parser_model_devi.add_argument("--models", type=str, nargs="+", help="Models")
+    parser_model_devi.add_argument("--cutoff", type=float, help="QM/MM cutoff radius")
+    parser_model_devi.add_argument(
+        "--parm7_file", type=str, default="qmmm.parm7", help="AMBER parm file"
+    )
+    parser_model_devi.add_argument(
+        "--qm_region",
+        type=str,
+        default=":1",
+        help="QM region with AMBER mask. Add quote if containing space",
+    )
+    parser_model_devi.add_argument("--prefix", type=str, help="prefix to the .nc file")
     parser_model_devi.set_defaults(func=model_devi_run)
 
-    parser_corr = subparsers.add_parser(
-        "corr", help="Generate systems for DPRc.")
-    parser_corr.add_argument('--cutoff', type=float,
-                             help="QM/MM cutoff radius")
-    parser_corr.add_argument('--parm7_file', type=str, default="qmmm.parm7",
-                             help="AMBER parm file")
-    parser_corr.add_argument('--qm_region', type=str, default=":1",
-                             help="QM region with AMBER mask. Add quote if containing space")
-    parser_corr.add_argument('--nc', type=str,
-                             help="AMBER coordinates (nc) file")
-    parser_corr.add_argument('--hl', type=str,
-                             help="Prefix to high-level files, including .mdout, .mdfrc")
-    parser_corr.add_argument('--ll', type=str,
-                             help="Prefix to low-level files, including .mdout, .mdfrc")
-    parser_corr.add_argument('--out', type=str, default="dataset",
-                             help="output directory or hdf5 file for DeePMD-kit data (default is dataset)")
-    parser_corr.add_argument('--suffix_mdfrc', type=str,
-                             help="suffix of mdfrc file")
+    parser_corr = subparsers.add_parser("corr", help="Generate systems for DPRc.")
+    parser_corr.add_argument("--cutoff", type=float, help="QM/MM cutoff radius")
+    parser_corr.add_argument(
+        "--parm7_file", type=str, default="qmmm.parm7", help="AMBER parm file"
+    )
+    parser_corr.add_argument(
+        "--qm_region",
+        type=str,
+        default=":1",
+        help="QM region with AMBER mask. Add quote if containing space",
+    )
+    parser_corr.add_argument("--nc", type=str, help="AMBER coordinates (nc) file")
+    parser_corr.add_argument(
+        "--hl", type=str, help="Prefix to high-level files, including .mdout, .mdfrc"
+    )
+    parser_corr.add_argument(
+        "--ll", type=str, help="Prefix to low-level files, including .mdout, .mdfrc"
+    )
+    parser_corr.add_argument(
+        "--out",
+        type=str,
+        default="dataset",
+        help="output directory or hdf5 file for DeePMD-kit data (default is dataset)",
+    )
+    parser_corr.add_argument("--suffix_mdfrc", type=str, help="suffix of mdfrc file")
     parser_corr.set_defaults(func=corr_run)
 
     parser_qmwater = subparsers.add_parser(
-        "qmwater", help="Generate QM water parm and mdin file.")
-    parser_qmwater.add_argument('--cutoff', type=float,
-                             help="cutoff")
-    parser_qmwater.add_argument('--parm7_file', type=str, default="qmmm.parm7",
-                             help="parm7_file")
-    parser_qmwater.add_argument('--qm_region', type=str, default=":1",
-                             help="qm_region")
-    parser_qmwater.add_argument('--nc', type=str,
-                             help="nc file")
-    parser_qmwater.add_argument('--hl', type=str,
-                             help="high level mdin file")
-    parser_qmwater.add_argument('--ll', type=str,
-                             help="low level mdin file")
-    parser_qmwater.add_argument('--charge', type=str, default="dataset",
-                             help="Charge of QM region")
+        "qmwater", help="Generate QM water parm and mdin file."
+    )
+    parser_qmwater.add_argument("--cutoff", type=float, help="cutoff")
+    parser_qmwater.add_argument(
+        "--parm7_file", type=str, default="qmmm.parm7", help="parm7_file"
+    )
+    parser_qmwater.add_argument("--qm_region", type=str, default=":1", help="qm_region")
+    parser_qmwater.add_argument("--nc", type=str, help="nc file")
+    parser_qmwater.add_argument("--hl", type=str, help="high level mdin file")
+    parser_qmwater.add_argument("--ll", type=str, help="low level mdin file")
+    parser_qmwater.add_argument(
+        "--charge", type=str, default="dataset", help="Charge of QM region"
+    )
     parser_qmwater.set_defaults(func=qmwater_run)
 
     parser_qmwater_corr = subparsers.add_parser(
-        "qmwater_corr", help="Generate systems for QM water.")
-    parser_qmwater_corr.add_argument('--cutoff', type=float,
-                             help="cutoff")
-    parser_qmwater_corr.add_argument('--qm_region', type=str, default=":1",
-                             help="qm_region")
-    parser_qmwater_corr.add_argument('--out', type=str, default="dataset",
-                             help="output directory (default is dataset)")
+        "qmwater_corr", help="Generate systems for QM water."
+    )
+    parser_qmwater_corr.add_argument("--cutoff", type=float, help="cutoff")
+    parser_qmwater_corr.add_argument(
+        "--qm_region", type=str, default=":1", help="qm_region"
+    )
+    parser_qmwater_corr.add_argument(
+        "--out",
+        type=str,
+        default="dataset",
+        help="output directory (default is dataset)",
+    )
     parser_qmwater_corr.set_defaults(func=qmwater_corr_run)
 
     args = parser.parse_args()
     args.func(args)
```

### Comparing `dpamber-0.2.2/dpamber/corr.py` & `dpamber-0.3.1/dpamber/corr.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+from typing import Union
+
 import dpdata
 import numpy as np
+from ase.geometry import Cell, get_distances, wrap_positions
 from dpdata.amber.mask import pick_by_amber_mask
-from ase.geometry import wrap_positions, Cell
-from typing import Union
 
 
-def get_amber_fp(cutoff: float,
-                 parmfile: str,
-                 ncfile: str,
-                 ll: str,
-                 hl: str,
-                 target: str = ":1",
-                 out: str = None,
-                 idx: Union[slice, list, int] = None,
-                 suffix_mdfrc = None,
-            ) -> dpdata.MultiSystems:
+def get_amber_fp(
+    cutoff: float,
+    parmfile: str,
+    ncfile: str,
+    ll: str,
+    hl: str,
+    target: str = ":1",
+    out: str = None,
+    idx: Union[slice, list, int] = None,
+    suffix_mdfrc=None,
+) -> dpdata.MultiSystems:
     """Use Ambertools to do correction calculation between a high level potential and a low level potential.
 
     Parameters
     ----------
     cutoff: float
         The QM/MM cutoff radius.
     parmfile: str
@@ -40,61 +42,94 @@
 
     Returns
     -------
     ms: dpdata.MultiSystems
         The output MultiSystems
     """
     ms = dpdata.MultiSystems()
-    ep = r'@%EP'
-    if cutoff > 0.:
-        interactwith = "(%s)<@%f&!%s" % (target, cutoff, ep)
+    ep = r"@%EP"
+    if cutoff > 0.0:
+        interactwith = f"({target})<@{cutoff:f}&!{ep}"
     else:
         interactwith = target
 
     if suffix_mdfrc is not None:
         ll_frc = ll + suffix_mdfrc
         hl_frc = hl + suffix_mdfrc
     else:
         ll_frc = None
         hl_frc = None
 
     s_ll = dpdata.LabeledSystem(
-        ll, nc_file=ncfile, mdfrc_file=ll_frc, parm7_file=parmfile, fmt='amber/md/qmmm', qm_region=target)
+        ll,
+        nc_file=ncfile,
+        mdfrc_file=ll_frc,
+        parm7_file=parmfile,
+        fmt="amber/md/qmmm",
+        qm_region=target,
+        exclude_unconverged=False,
+    )
     s_hl = dpdata.LabeledSystem(
-        hl, nc_file=ncfile, mdfrc_file=hl_frc, parm7_file=parmfile, fmt='amber/md/qmmm', qm_region=target)
+        hl,
+        nc_file=ncfile,
+        mdfrc_file=hl_frc,
+        parm7_file=parmfile,
+        fmt="amber/md/qmmm",
+        qm_region=target,
+        exclude_unconverged=False,
+    )
     if idx is not None:
         s_ll = s_ll[idx]
         s_hl = s_hl[idx]
 
     s_corr = s_ll.correction(s_hl)
+
+    # remove unconverged frames
+    idx_pick = ~np.logical_or(
+        np.isnan(s_corr["energies"]), np.isnan(s_corr["forces"]).any(axis=(1, 2))
+    )
+    s_corr = s_corr[idx_pick]
+
     # wrap the coords...
     qm_index = pick_by_amber_mask(parmfile, target)
+    qm_coords = s_corr["coords"][:, qm_index, :]
     for ii in range(len(s_corr)):
-        cell = Cell(s_corr['cells'][ii])
-        wraped_coords = wrap_positions(s_corr['coords'][ii], cell=s_corr['cells'][ii], pbc=True, center=cell.scaled_positions(np.mean(s_corr['coords'][ii, qm_index], axis=0)))
-        s_corr['coords'][ii, :, :] = wraped_coords
+        cell = Cell(s_corr["cells"][ii])
+        qm_coord = qm_coords[ii]
+        qm_distances = get_distances(qm_coord, cell=cell, pbc=True)[1]
+        # find the coord that has the minimal total distance as the center
+        center = qm_coords[ii, np.argmin(np.sum(qm_distances, axis=1))]
+        wraped_coords = wrap_positions(
+            s_corr["coords"][ii],
+            cell=s_corr["cells"][ii],
+            pbc=True,
+            center=cell.scaled_positions(center),
+        )
+        s_corr["coords"][ii, :, :] = wraped_coords
 
     s_corr = s_corr.pick_by_amber_mask(
-        parmfile, interactwith, pass_coords=True, nopbc=True)
+        parmfile, interactwith, pass_coords=True, nopbc=True
+    )
     for ss in s_corr:
-        if 'EP' in ss['atom_names']:
-            ss = ss.remove_atom_names('EP')
+        if "EP" in ss["atom_names"]:
+            ss = ss.remove_atom_names("EP")
         ms.append(ss)
 
     if out:
         if out.endswith(".hdf5"):
             ms.to_deepmd_hdf5(out)
         else:
             ms.to_deepmd_npy(out)
     return ms
 
 
 def run(args):
-    get_amber_fp(cutoff=args.cutoff,
-                 parmfile=args.parm7_file,
-                 ncfile=args.nc,
-                 ll=args.ll,
-                 hl=args.hl,
-                 target=args.qm_region,
-                 out=args.out,
-                 suffix_mdfrc=args.suffix_mdfrc,
-                 )
+    get_amber_fp(
+        cutoff=args.cutoff,
+        parmfile=args.parm7_file,
+        ncfile=args.nc,
+        ll=args.ll,
+        hl=args.hl,
+        target=args.qm_region,
+        out=args.out,
+        suffix_mdfrc=args.suffix_mdfrc,
+    )
```

### Comparing `dpamber-0.2.2/dpamber/qmbuffer.py` & `dpamber-0.3.1/dpamber/qmbuffer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,50 @@
+from copy import copy
+
 import dpdata
-from dpdata.amber.mask import load_param_file, pick_by_amber_mask
 import parmed.tools as PT
-from copy import copy
+from dpdata.amber.mask import load_param_file, pick_by_amber_mask
 
 
-def qmbuffer(cutoff: float,
-              ncfile: str,
-              parmfile: str,
-              hl_mdinfile: str,
-              ll_mdinfile: str,
-              target: str = ":1",
-              targetcharge: int = -2):
-    """
-    Assume there is only one frame.
-    cutoff = 4.5
+def qmbuffer(
+    cutoff: float,
+    ncfile: str,
+    parmfile: str,
+    hl_mdinfile: str,
+    ll_mdinfile: str,
+    target: str = ":1",
+    targetcharge: int = -2,
+):
+    """Assume there is only one frame.
+    cutoff = 4.5.
     """
-    mask_str = "((%s)<:%.1f) & !(%s)" % (target, cutoff, target)
-    s = dpdata.System("",
-        nc_file=ncfile, parm7_file=parmfile, fmt='amber/md', use_element_symbols=target)
+    mask_str = f"(({target})<:{cutoff:.1f}) & !({target})"
+    s = dpdata.System(
+        "",
+        nc_file=ncfile,
+        parm7_file=parmfile,
+        fmt="amber/md",
+        use_element_symbols=target,
+    )
     # systems with nearby waters
     parm = load_param_file(parmfile)
-    target_idx = pick_by_amber_mask(parm, target, s['coords'][0])
-    nearby_idx = pick_by_amber_mask(parm, mask_str, s['coords'][0])
+    target_idx = pick_by_amber_mask(parm, target, s["coords"][0])
+    nearby_idx = pick_by_amber_mask(parm, mask_str, s["coords"][0])
     parm = reorder(parm, target_idx, nearby_idx)
     # Here we need to generate 4 new parms:
     # 1. reordered, QM water
     # 2. reordered, QM water, no target
     # 3. reordered, MM water
     # 4. reordered, MM water, no target
     # parm 1
     new_nearby_idx = range(len(target_idx), len(target_idx) + len(nearby_idx))
     parm_qm = copy(parm)
     parm_qm, nwater = remove_epw(parm_qm, new_nearby_idx)
-    water_mask = "(:2-%d)" % (nwater+1)
-    qmmask = "(%s)|(%s)" % (target, water_mask)
+    water_mask = "(:2-%d)" % (nwater + 1)
+    qmmask = f"({target})|({water_mask})"
     sort_parm(parm_qm)
     write_parm(parm_qm, "qmwater", hl_mdinfile, qmmask, target, charge=targetcharge)
 
     # parm2
     parm_qm_not = strip_atoms(parm_qm, target)
     water_mask = "(:1-%d)" % (nwater)
     sort_parm(parm_qm_not)
@@ -57,39 +64,39 @@
     parm_noep = copy(parm)
     parm_noep, _ = remove_epw(parm_noep, range(len(target_idx), s.get_natoms()))
     sort_parm(parm_mm)
     parm_noep.write_parm("noepw.parm7")
 
 
 def label_atoms(parm, target_idx, qmwater_idx):
-    """set qwt"""
+    """Set qwt."""
     for ii in range(len(parm.atoms)):
         atom = parm.atoms[ii]
         if ii in target_idx:
             atom._sorted = 0
         elif ii in qmwater_idx:
             atom._sorted = 1
         else:
             atom._sorted = 2
-        
+
 
 def remove_epw(parm, idx):
-    """Remove all EP atoms in water in idx"""
+    """Remove all EP atoms in water in idx."""
     nwater = 0
     ep = []
     for ii in idx:
         atom = parm.atoms[ii]
         res = atom.residue
         if atom.type == "EP":
             ep.append(ii)
             nwater += 1
             if res.atoms[0].name == "O":
                 res.name = "qwt"
                 res.atoms[0].charge += atom.charge
-                #print(atom.charge, res.atoms[0].charge)
+                # print(atom.charge, res.atoms[0].charge)
                 atom.charge = 0
                 # remove from res
                 res.atoms.pop(res.atoms.index(atom))
             else:
                 raise RuntimeError()
             # remove bonds
             for bond in atom.bonds:
@@ -104,49 +111,61 @@
                     p.delete()
             for _ in range(len(atom._exclusion_partners)):
                 atom._exclusion_partners.pop()
             for p in atom.children:
                 if p.type == "EP":
                     atom.children.pop(atom.children.index(p))
 
-    mask = "@" + ",".join([ str(ii+1) for ii in ep])
+    mask = "@" + ",".join([str(ii + 1) for ii in ep])
     parm = strip_atoms(parm, mask)
     return parm, nwater
 
+
 def strip_atoms(parm, mask):
     parm.strip(mask)
     return parm
 
+
 def reorder(parm, target_idx, nearby_idx):
     label_atoms(parm, target_idx, qmwater_idx=nearby_idx)
     parm.atoms.sort(key=lambda a: a._sorted)
     return parm
 
+
 def sort_parm(parm):
     # sort residues
     parm.residues.sort(key=sort_residues)
 
+
 def write_parm(parm, fn, mdinfile, qmmask, target, charge=0):
     parm.write_parm("%s.parm7" % fn)
     parm.write_rst7("%s.rst7" % fn)
-    PT.writeCoordinates(parm, '%s.nc' % fn).execute()
-    ifqnt = str(int(target!=""))
-    with open(mdinfile) as f, open("%s.mdin" % fn, 'w') as fw:
-        fw.write(f.read().replace("%QMMASK%", qmmask).replace("%NOSHAKEMASK%", target).replace("%CHARGE%", str(charge)).replace("%IFQNT%", ifqnt))
+    PT.writeCoordinates(parm, "%s.nc" % fn).execute()
+    ifqnt = str(int(target != ""))
+    with open(mdinfile) as f, open("%s.mdin" % fn, "w") as fw:
+        fw.write(
+            f.read()
+            .replace("%QMMASK%", qmmask)
+            .replace("%NOSHAKEMASK%", target)
+            .replace("%CHARGE%", str(charge))
+            .replace("%IFQNT%", ifqnt)
+        )
 
 
 def sort_residues(res):
     keys = {
         "qwt": 1,
         "WAT": 2,
     }
     return keys.get(res.name, 0)
 
+
 def run(args):
-    qmbuffer(cutoff=args.cutoff,
-            parmfile=args.parm7_file,
-            ncfile=args.nc,
-            ll_mdinfile=args.ll,
-            hl_mdinfile=args.hl,
-            target=args.qm_region,
-            targetcharge=args.charge,
-            )
+    qmbuffer(
+        cutoff=args.cutoff,
+        parmfile=args.parm7_file,
+        ncfile=args.nc,
+        ll_mdinfile=args.ll,
+        hl_mdinfile=args.hl,
+        target=args.qm_region,
+        targetcharge=args.charge,
+    )
```

### Comparing `dpamber-0.2.2/dpamber/qmwater_corr.py` & `dpamber-0.3.1/dpamber/qmwater_corr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 import dpdata
 import numpy as np
 
 
-def get_amber_fp(cutoff: float,
-                 target: str = ":1",
-                 out: str = None,
-            ) -> dpdata.MultiSystems:
+def get_amber_fp(
+    cutoff: float,
+    target: str = ":1",
+    out: str = None,
+) -> dpdata.MultiSystems:
     """(qmwater-qmwater_not)-(mmwater-mmwater_not)
-    = (qmwater-mmwater) - (qmwater_not-mmwater_not)
+    = (qmwater-mmwater) - (qmwater_not-mmwater_not).
     """
     ms = dpdata.MultiSystems()
-    ep = r'@%EP'
-    if cutoff > 0.:
-        interactwith = "(%s)<@%f&!%s" % (target, cutoff, ep)
+    ep = r"@%EP"
+    if cutoff > 0.0:
+        interactwith = f"({target})<@{cutoff:f}&!{ep}"
     else:
         interactwith = target
 
-    s_qmwater = dpdata.LabeledSystem(
-        "qmwater", fmt='amber/md/qmmm', qm_region=target)
-    s_qmwater = s_qmwater.remove_atom_names('EP')
-    s_mmwater = dpdata.LabeledSystem(
-        "mmwater", fmt='amber/md/qmmm', qm_region=target)
-    s_mmwater = s_mmwater.remove_atom_names('EP')
-    assert(np.all(s_qmwater['coords']==s_mmwater['coords']))
+    s_qmwater = dpdata.LabeledSystem("qmwater", fmt="amber/md/qmmm", qm_region=target)
+    s_qmwater = s_qmwater.remove_atom_names("EP")
+    s_mmwater = dpdata.LabeledSystem("mmwater", fmt="amber/md/qmmm", qm_region=target)
+    s_mmwater = s_mmwater.remove_atom_names("EP")
+    assert np.all(s_qmwater["coords"] == s_mmwater["coords"])
     s_allcorr = s_mmwater.correction(s_qmwater)
-    
-    s_qmwaternot = dpdata.LabeledSystem(
-        "qmwater_not", fmt='amber/md/qmmm')
-    s_qmwaternot = s_qmwaternot.remove_atom_names('EP')
-    s_mmwaternot = dpdata.LabeledSystem(
-        "mmwater_not", fmt='amber/md/qmmm')
-    s_mmwaternot = s_mmwaternot.remove_atom_names('EP')
-    assert(np.all(s_qmwaternot['coords']==s_mmwaternot['coords']))
+
+    s_qmwaternot = dpdata.LabeledSystem("qmwater_not", fmt="amber/md/qmmm")
+    s_qmwaternot = s_qmwaternot.remove_atom_names("EP")
+    s_mmwaternot = dpdata.LabeledSystem("mmwater_not", fmt="amber/md/qmmm")
+    s_mmwaternot = s_mmwaternot.remove_atom_names("EP")
+    assert np.all(s_qmwaternot["coords"] == s_mmwaternot["coords"])
     s_notcorr = s_mmwaternot.correction(s_qmwaternot)
 
     # manually process
     natom_not = s_notcorr.get_natoms()
-    assert(np.all(s_allcorr['coords'][:,-natom_not:]==s_notcorr['coords']))
-    s_allcorr.data['energies'] -= s_notcorr['energies']
-    s_allcorr.data['forces'][:,-natom_not:] -= s_notcorr['forces']
+    assert np.all(s_allcorr["coords"][:, -natom_not:] == s_notcorr["coords"])
+    s_allcorr.data["energies"] -= s_notcorr["energies"]
+    s_allcorr.data["forces"][:, -natom_not:] -= s_notcorr["forces"]
 
     s_allcorr = s_allcorr.pick_by_amber_mask(
-        "noepw.parm7", interactwith, pass_coords=True, nopbc=True)
+        "noepw.parm7", interactwith, pass_coords=True, nopbc=True
+    )
     for ss in s_allcorr:
         ms.append(ss)
 
     if out:
         ms.to_deepmd_npy(out)
     return ms
 
 
 def run(args):
-    get_amber_fp(cutoff=args.cutoff,
-                 target=args.qm_region,
-                 out=args.out,
-                 )
+    get_amber_fp(
+        cutoff=args.cutoff,
+        target=args.qm_region,
+        out=args.out,
+    )
```

### Comparing `dpamber-0.2.2/dpamber/read_amber.py` & `dpamber-0.3.1/dpamber/read_amber.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,68 @@
-import re
 import os
-from scipy.io import netcdf
+import re
+
 import numpy as np
+from ase.geometry import cellpar_to_cell
 from dpdata.amber.mask import pick_by_amber_mask
-from dpdata.unit import EnergyConversion
-from dpdata.periodic_table import ELEMENTS
 from dpdata.format import Format
+from dpdata.periodic_table import ELEMENTS
 from dpdata.plugins.amber import AmberMDFormat
-from ase.geometry import cellpar_to_cell
-
+from dpdata.unit import EnergyConversion
+from scipy.io import netcdf
 
 kcalmol2eV = EnergyConversion("kcal_mol", "eV").value()
-symbols = ['X'] + ELEMENTS
+symbols = ["X"] + ELEMENTS
 
 energy_convert = kcalmol2eV
 force_convert = energy_convert
 
 
-def read_amber_traj(parm7_file, nc_file, mdfrc_file=None, mden_file=None, mdout_file=None,
-                    qm_region=None, labeled=True,
-                    ):
-    """The amber trajectory includes:
+def read_amber_traj(
+    parm7_file,
+    nc_file,
+    mdfrc_file=None,
+    mden_file=None,
+    mdout_file=None,
+    qm_region=None,
+    labeled=True,
+    exclude_unconverged=True,
+):
+    """Read amber trajectory.
+
+    The amber trajectory includes:
     * nc, NetCDF format, stores coordinates
     * mdfrc, NetCDF format, stores forces
     * mden (optional), text format, stores energies
     * mdout (optional), text format, may store energies if there is no mden_file
-    * parm7, text format, stores types
+    * parm7, text format, stores types.
 
     Parameters
     ----------
     parm7_file, nc_file, mdfrc_file, mden_file, mdout_file: str
-      filenames
+        filenames
     qm_region: None or list or str
-      amber mask
+        amber mask
+    labeled: bool
+        the output is a dpdata.LabeledSystem or dpdata.System
+    exclude_unconverged: bool
+        exclude unconverged frames
     """
-
     flag_atom_type = False
     flag_atom_numb = False
     amber_types = []
     atomic_number = []
     with open(parm7_file) as f:
         for line in f:
             if line.startswith("%FLAG"):
                 flag_atom_type = line.startswith("%FLAG AMBER_ATOM_TYPE")
                 flag_atom_numb = line.startswith("%FLAG ATOMIC_NUMBER")
             elif flag_atom_type or flag_atom_numb:
                 if line.startswith("%FORMAT"):
-                    fmt = re.findall(r'\d+', line)
+                    fmt = re.findall(r"\d+", line)
                     fmt0 = int(fmt[0])
                     fmt1 = int(fmt[1])
                 else:
                     for ii in range(fmt0):
                         start_index = ii * fmt1
                         end_index = (ii + 1) * fmt1
                         if end_index >= len(line):
@@ -61,94 +73,139 @@
                         elif flag_atom_numb:
                             atomic_number.append(int(content))
     ml_types = []
     if qm_region is None:
         qm_region = []
 
     if isinstance(qm_region, str):
-        qm_region = pick_by_amber_mask(
-            parm7_file, qm_region)
-    
+        qm_region = pick_by_amber_mask(parm7_file, qm_region)
+
     for ii, (tt, nn) in enumerate(zip(amber_types, atomic_number)):
         if ii in qm_region:
             ml_types.append(symbols[nn])
         elif tt in ("OW", "HW", "EP"):
             ml_types.append(tt)
         else:
             ml_types.append("m" + symbols[nn])
 
-    with netcdf.netcdf_file(nc_file, 'r') as f:
+    with netcdf.netcdf_file(nc_file, "r") as f:
         coords = np.array(f.variables["coordinates"][:])
-        cell_lengths = np.array(f.variables["cell_lengths"][:])
-        cell_angles = np.array(f.variables["cell_angles"][:])
-        shape = cell_lengths.shape
+        shape = coords.shape
         cells = np.zeros((shape[0], 3, 3))
-        for ii in range(cell_lengths.shape[0]):
-            cells[ii, :, :] = cellpar_to_cell([*cell_lengths[ii], *cell_angles[ii]])
+        if "cell_lengths" in f.variables:
+            nopbc = False
+            cell_lengths = np.array(f.variables["cell_lengths"][:])
+            cell_angles = np.array(f.variables["cell_angles"][:])
+            for ii in range(cell_lengths.shape[0]):
+                cells[ii, :, :] = cellpar_to_cell([*cell_lengths[ii], *cell_angles[ii]])
+        else:
+            nopbc = True
 
     if labeled:
-        with netcdf.netcdf_file(mdfrc_file, 'r') as f:
+        with netcdf.netcdf_file(mdfrc_file, "r") as f:
             forces = np.array(f.variables["forces"][:])
 
         # load energy from mden_file or mdout_file
         energies = []
-        if mden_file is not None and os.path.isfile(mden_file):
+        if mdout_file is not None and os.path.isfile(mdout_file):
+            is_coverage = True
+            with open(mdout_file) as f:
+                for line in f:
+                    if (
+                        line.strip()
+                        == "QMMM SCC-DFTB: Convergence could not be achieved in this step."
+                    ):
+                        is_coverage = False
+                    elif line.strip().startswith("A V E R A G E S   O V E R"):
+                        # end of MD simulation
+                        break
+                    elif "EPtot" in line:
+                        if is_coverage:
+                            s = line.split()
+                            energies.append(float(s[-1]))
+                        else:
+                            energies.append(np.nan)
+                            is_coverage = True
+        elif mden_file is not None and os.path.isfile(mden_file):
             with open(mden_file) as f:
                 for line in f:
                     if line.startswith("L6"):
                         s = line.split()
                         if s[2] != "E_pot":
                             energies.append(float(s[2]))
-        elif mdout_file is not None and os.path.isfile(mdout_file):
-            with open(mdout_file) as f:
-                for line in f:
-                    if "EPtot" in line:
-                        s = line.split()
-                        energies.append(float(s[-1]))
         else:
-            raise RuntimeError(
-                "Please provide one of mden_file and mdout_file")
+            raise RuntimeError("Please provide one of mden_file and mdout_file")
 
     atom_names, atom_types, atom_numbs = np.unique(
-        ml_types, return_inverse=True, return_counts=True)
+        ml_types, return_inverse=True, return_counts=True
+    )
 
     data = {}
-    data['atom_names'] = list(atom_names)
-    data['atom_numbs'] = list(atom_numbs)
-    data['atom_types'] = atom_types
+    data["atom_names"] = list(atom_names)
+    data["atom_numbs"] = list(atom_numbs)
+    data["atom_types"] = atom_types
+    data["coords"] = coords
+    data["cells"] = cells
     if labeled:
-        if np.isnan(forces).any() or np.isnan(energies).any():
-            return {
-                'energies': [],
-                'forces': [],
-            }
-        data['forces'] = forces * force_convert
-        data['energies'] = np.array(energies) * energy_convert
-    data['coords'] = coords
-    data['cells'] = cells
-    data['orig'] = np.array([0, 0, 0])
+        data["forces"] = forces * force_convert
+        data["energies"] = np.array(energies) * energy_convert
+        if exclude_unconverged:
+            # exclude nan index
+            idx_pick = ~np.logical_or(
+                np.isnan(data["energies"]), np.isnan(data["forces"]).any(axis=(1, 2))
+            )
+            data["coords"] = data["coords"][idx_pick, :, :]
+            data["cells"] = data["cells"][idx_pick, :, :]
+            data["energies"] = data["energies"][idx_pick]
+            data["forces"] = data["forces"][idx_pick, :, :]
+    data["orig"] = np.array([0, 0, 0])
+    if nopbc:
+        data["nopbc"] = True
     return data
 
 
 @Format.register("amber/md/qmmm")
 class AmberMDQMMMFormat(AmberMDFormat):
-    def from_system(self, file_name=None, parm7_file=None, nc_file=None, qm_region=None, **kwargs):
+    def from_system(
+        self, file_name=None, parm7_file=None, nc_file=None, qm_region=None, **kwargs
+    ):
         # assume the prefix is the same if the spefic name is not given
         if parm7_file is None:
             parm7_file = file_name + ".parm7"
         if nc_file is None:
             nc_file = file_name + ".nc"
-        return read_amber_traj(parm7_file=parm7_file, nc_file=nc_file, qm_region=qm_region, labeled=False)
-
-    def from_labeled_system(self, file_name=None, parm7_file=None, nc_file=None, mdfrc_file=None, mden_file=None, mdout_file=None, qm_region=None, **kwargs):
+        return read_amber_traj(
+            parm7_file=parm7_file, nc_file=nc_file, qm_region=qm_region, labeled=False
+        )
+
+    def from_labeled_system(
+        self,
+        file_name=None,
+        parm7_file=None,
+        nc_file=None,
+        mdfrc_file=None,
+        mden_file=None,
+        mdout_file=None,
+        qm_region=None,
+        exclude_unconverged=True,
+        **kwargs,
+    ):
         # assume the prefix is the same if the spefic name is not given
         if parm7_file is None:
             parm7_file = file_name + ".parm7"
         if nc_file is None:
             nc_file = file_name + ".nc"
         if mdfrc_file is None:
             mdfrc_file = file_name + ".mdfrc"
         if mden_file is None:
             mden_file = file_name + ".mden"
         if mdout_file is None:
             mdout_file = file_name + ".mdout"
-        return read_amber_traj(parm7_file, nc_file, mdfrc_file, mden_file, mdout_file, qm_region)
+        return read_amber_traj(
+            parm7_file,
+            nc_file,
+            mdfrc_file,
+            mden_file,
+            mdout_file,
+            qm_region,
+            exclude_unconverged=exclude_unconverged,
+        )
```

### Comparing `dpamber-0.2.2/dpamber.egg-info/PKG-INFO` & `dpamber-0.3.1/dpamber.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: dpamber
-Version: 0.2.2
+Version: 0.3.1
 Summary: Some useful tools related to Amber and DP.
 Project-URL: Homepage, https://github.com/njzjz/dpamber
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dpcpu
+Provides-Extra: dpgpu
 
 # dpamber
 
 Some useful tools related to Amber and DP.
 
 ## Installation
 
@@ -45,7 +48,17 @@
 An example of the command is
 ```sh
 dpamber corr --cutoff 6. --qm_region ":1" --parm7_file some_param.param7 --nc some_coord.nc --hl high_level --ll low_level --out dataset
 ```
 where `--cutoff` takes cutoff radius of the QM/MM interaction for training. `--qm_region` takes AMBER mask format for the QM region. `--parm7_file` and `--nc` take the PARM7 file and the trajectory (NetCDF) file, respectively. `--ll` and `--hl` are the prefixes of low-level and high-level files, including the mdout file (`.mdout`), the mden file (`.mden`) and the mdfrc file (`.mdfrc`). The output dataset directory should be put in `--out`.
 
 See details from `dpamber corr -h`.
+
+### model-devi: calculate model deviation
+
+`model-devi` can be used to calculate the model deviation of a given trajectory.
+You need to install DeePMD-kit using
+```sh
+pip install dpamber[dpgpu]
+```
+
+See `dpamber model-devi -h` for details.
```

