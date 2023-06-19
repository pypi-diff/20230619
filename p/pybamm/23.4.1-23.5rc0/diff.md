# Comparing `tmp/pybamm-23.4.1.tar.gz` & `tmp/pybamm-23.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybamm-23.4.1.tar", last modified: Tue May  2 15:24:07 2023, max compression
+gzip compressed data, was "pybamm-23.5rc0.tar", last modified: Mon Jun 19 14:33:45 2023, max compression
```

## Comparing `pybamm-23.4.1.tar` & `pybamm-23.5rc0.tar`

### file list

```diff
@@ -1,457 +1,376 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:07.005808 pybamm-23.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-05-02 15:23:56.000000 pybamm-23.4.1/CMakeBuild.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-02 15:23:56.000000 pybamm-23.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    41858 2023-05-02 15:24:07.005808 pybamm-23.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    38853 2023-05-02 15:23:56.000000 pybamm-23.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.925808 pybamm-23.4.1/pybamm/
--rw-r--r--   0 runner    (1001) docker     (123)    20084 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/CITATIONS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/batch_study.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/citations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.929808 pybamm-23.4.1/pybamm/discretisations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/discretisations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46989 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/discretisations/discretisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/doc_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.929808 pybamm-23.4.1/pybamm/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/experiments/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.937808 pybamm-23.4.1/pybamm/expression_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    12502 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/averages.py
--rw-r--r--   0 runner    (1001) docker     (123)    50702 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/binary_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    21364 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/broadcasts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18611 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/concatenations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15196 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/independent_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/input_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/interpolant.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.937808 pybamm-23.4.1/pybamm/expression_tree/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/operations/convert_to_casadi.py
--rw-r--r--   0 runner    (1001) docker     (123)    26233 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/operations/evaluate_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/operations/jacobian.py
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/operations/latexify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/operations/unpack_symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.941808 pybamm-23.4.1/pybamm/expression_tree/printing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/printing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/printing/print_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/printing/sympy_overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/state_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    32988 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)    39893 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/unary_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/expression_tree/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.941808 pybamm-23.4.1/pybamm/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/geometry/battery_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/geometry/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/geometry/standard_spatial_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.941808 pybamm-23.4.1/pybamm/input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.905808 pybamm-23.4.1/pybamm/input/discharge_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.941808 pybamm-23.4.1/pybamm/input/discharge_data/Ecker2015/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/discharge_data/Ecker2015/Ecker_1C.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/discharge_data/Ecker2015/Ecker_5C.csv
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/discharge_data/Ecker2015/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.949808 pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/
--rw-r--r--   0 runner    (1001) docker     (123)   685399 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_U.txt
--rw-r--r--   0 runner    (1001) docker     (123)   180796 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_displacement.txt
--rw-r--r--   0 runner    (1001) docker     (123)   156316 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_T.txt
--rw-r--r--   0 runner    (1001) docker     (123)   129670 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_U.txt
--rw-r--r--   0 runner    (1001) docker     (123)    38056 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_displacement.txt
--rw-r--r--   0 runner    (1001) docker     (123)   125368 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/1C_discharge_T.txt
--rw-r--r--   0 runner    (1001) docker     (123)    63563 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/1C_discharge_U.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20171 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/1C_discharge_displacement.txt
--rw-r--r--   0 runner    (1001) docker     (123)   158837 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/2C_discharge_T.txt
--rw-r--r--   0 runner    (1001) docker     (123)    30602 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/2C_discharge_U.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/2C_discharge_displacement.txt
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)    13539 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/stn_2C.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    13828 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/stp_2C.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.949808 pybamm-23.4.1/pybamm/input/drive_cycles/
--rw-r--r--   0 runner    (1001) docker     (123)    16846 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/drive_cycles/UDDS.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/drive_cycles/US06.csv
--rw-r--r--   0 runner    (1001) docker     (123)   299508 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/drive_cycles/WLTC.csv
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/drive_cycles/car_current.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.953808 pybamm-23.4.1/pybamm/input/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.953808 pybamm-23.4.1/pybamm/input/parameters/ecm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/ecm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.953808 pybamm-23.4.1/pybamm/input/parameters/ecm/data/
--rw-r--r--   0 runner    (1001) docker     (123)   135520 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/ecm/data/ecm_example_c1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/ecm/data/ecm_example_dudt.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/ecm/data/ecm_example_ocv.csv
--rw-r--r--   0 runner    (1001) docker     (123)   149886 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/ecm/data/ecm_example_r0.csv
--rw-r--r--   0 runner    (1001) docker     (123)   149222 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/ecm/data/ecm_example_r1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/ecm/example_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.957808 pybamm-23.4.1/pybamm/input/parameters/lead_acid/
--rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lead_acid/Sulzer2019.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lead_acid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.961808 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/
--rw-r--r--   0 runner    (1001) docker     (123)    25833 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/Ai2020.py
--rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/Chen2020.py
--rw-r--r--   0 runner    (1001) docker     (123)    17412 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/Chen2020_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)    21798 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/Ecker2015.py
--rw-r--r--   0 runner    (1001) docker     (123)    18917 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/Marquis2019.py
--rw-r--r--   0 runner    (1001) docker     (123)    18050 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/Mohtat2020.py
--rw-r--r--   0 runner    (1001) docker     (123)    17352 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/NCA_Kim2011.py
--rw-r--r--   0 runner    (1001) docker     (123)    25674 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/OKane2022.py
--rw-r--r--   0 runner    (1001) docker     (123)    30791 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/ORegan2022.py
--rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/Prada2013.py
--rw-r--r--   0 runner    (1001) docker     (123)    18649 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/Ramadass2004.py
--rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/Xu2019.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.965808 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/data/
--rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/data/graphite_LGM50_ocp_Chen2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Ecker2015.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Enertech_Ai2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/data/lico2_data_example.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11504 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/data/lico2_ocp_Ai2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/data/measured_graphite_diffusivity_Ecker2015.csv
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/data/measured_nco_diffusivity_Ecker2015.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/data/nca_ocp_Kim2011_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/data/nco_ocp_Ecker2015.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/data/nmc_LGM50_ocp_Chen2020.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.913807 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.965808 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/cells/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.965808 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/cells/Enertech_Ai2020/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/cells/Enertech_Ai2020/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/cells/Enertech_Ai2020/parameters.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/cells/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.965808 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.965808 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_TDF_EC_DMC_1_1_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_base_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_conductivity_EC_DMC_1_1_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_diffusivity_EC_DMC_1_1_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_transference_number_EC_DMC_1_1_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.965808 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_TDF_EC_EMC_3_7_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_base_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_conductivity_EC_EMC_3_7_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_diffusivity_EC_EMC_3_7_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_transference_number_EC_EMC_3_7_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.969808 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_TDF_EMC_FEC_19_1_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_base_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_conductivity_EMC_FEC_19_1_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_diffusivity_EMC_FEC_19_1_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_transference_number_EMC_FEC_19_1_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.969808 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/dlnf_dlnc_Ai2020.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/electrolyte_conductivity_Ai2020.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/electrolyte_diffusivity_Ai2020.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.969808 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/experiments/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.969808 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/experiments/1C_discharge_from_full_Ai2020/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/experiments/1C_discharge_from_full_Ai2020/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/experiments/1C_discharge_from_full_Ai2020/parameters.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.969808 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.969808 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_cracking_rate_Ai2020.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_diffusivity_Dualfoil1998.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_electrolyte_exchange_current_density_Dualfoil1998.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_entropy_Enertech_Ai2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_entropy_Enertech_Ai2020_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_ocp_Enertech_Ai2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_ocp_Enertech_Ai2020_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_volume_change_Ai2020.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.969808 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.973808 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_cracking_rate_Ai2020.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_diffusivity_Dualfoil1998.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_electrolyte_exchange_current_density_Dualfoil1998.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_entropic_change_Ai2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_entropic_change_Ai2020_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_ocp_Ai2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_ocp_Ai2020_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_volume_change_Ai2020.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.913807 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/seis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.973808 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/seis/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/seis/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/seis/example/parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.973808 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/separators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/separators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.973808 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/separators/separator_Ai2020/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/separators/separator_Ai2020/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/input/parameters/lithium_ion/testing_only/separators/separator_Ai2020/parameters.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/install_odes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.973808 pybamm-23.4.1/pybamm/meshes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/meshes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/meshes/meshes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/meshes/one_dimensional_submeshes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/meshes/scikit_fem_submeshes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/meshes/zero_dimensional_submesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.973808 pybamm-23.4.1/pybamm/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47327 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.973808 pybamm-23.4.1/pybamm/models/full_battery_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56548 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/base_battery_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.973808 pybamm-23.4.1/pybamm/models/full_battery_models/equivalent_circuit/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/equivalent_circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/equivalent_circuit/ecm_model_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/equivalent_circuit/thevenin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.977808 pybamm-23.4.1/pybamm/models/full_battery_models/lead_acid/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/lead_acid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/lead_acid/base_lead_acid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/lead_acid/basic_full.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/lead_acid/full.py
--rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/lead_acid/loqs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.977808 pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/Yang2017.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17815 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/base_lithium_ion_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/basic_dfn.py
--rw-r--r--   0 runner    (1001) docker     (123)    16915 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/basic_dfn_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/basic_dfn_half_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/basic_spm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/dfn.py
--rw-r--r--   0 runner    (1001) docker     (123)    26674 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/electrode_soh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/electrode_soh_half_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/mpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/newman_tobias.py
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/spm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/spme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.977808 pybamm-23.4.1/pybamm/models/submodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.977808 pybamm-23.4.1/pybamm/models/submodels/active_material/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/active_material/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/active_material/base_active_material.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/active_material/constant_active_material.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/active_material/loss_active_material.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/active_material/total_active_material.py
--rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/base_submodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.977808 pybamm-23.4.1/pybamm/models/submodels/convection/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/convection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/convection/base_convection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.981808 pybamm-23.4.1/pybamm/models/submodels/convection/through_cell/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/convection/through_cell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/convection/through_cell/base_through_cell_convection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/convection/through_cell/explicit_convection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/convection/through_cell/full_convection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/convection/through_cell/no_convection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.981808 pybamm-23.4.1/pybamm/models/submodels/convection/transverse/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/convection/transverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/convection/transverse/base_transverse_convection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/convection/transverse/full_convection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/convection/transverse/no_convection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/convection/transverse/uniform_convection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.981808 pybamm-23.4.1/pybamm/models/submodels/current_collector/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/current_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/current_collector/base_current_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    14845 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/current_collector/effective_resistance_current_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/current_collector/homogeneous_current_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/current_collector/potential_pair.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.981808 pybamm-23.4.1/pybamm/models/submodels/electrode/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrode/base_electrode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.981808 pybamm-23.4.1/pybamm/models/submodels/electrode/ohm/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrode/ohm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrode/ohm/base_ohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrode/ohm/composite_ohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrode/ohm/full_ohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrode/ohm/leading_ohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrode/ohm/li_metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrode/ohm/surface_form_ohm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.981808 pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/base_electrolyte_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/composite_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/full_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/integrated_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/leading_order_conductivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.985808 pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/composite_surface_form_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/explicit_surface_form_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/full_surface_form_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/leading_surface_form_conductivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.985808 pybamm-23.4.1/pybamm/models/submodels/electrolyte_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrolyte_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrolyte_diffusion/base_electrolyte_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrolyte_diffusion/constant_concentration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrolyte_diffusion/full_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/electrolyte_diffusion/leading_order_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.985808 pybamm-23.4.1/pybamm/models/submodels/equivalent_circuit_elements/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/equivalent_circuit_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/equivalent_circuit_elements/ocv_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/equivalent_circuit_elements/rc_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/equivalent_circuit_elements/resistor_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/equivalent_circuit_elements/thermal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/equivalent_circuit_elements/voltage_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.985808 pybamm-23.4.1/pybamm/models/submodels/external_circuit/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/external_circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/external_circuit/base_external_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/external_circuit/explicit_control_external_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/external_circuit/function_control_external_circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.985808 pybamm-23.4.1/pybamm/models/submodels/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/base_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.985808 pybamm-23.4.1/pybamm/models/submodels/interface/interface_utilisation/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/interface_utilisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/interface_utilisation/base_utilisation.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/interface_utilisation/constant_utilisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/interface_utilisation/current_driven_utilisation.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/interface_utilisation/full_utilisation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.989808 pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/base_kinetics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/butler_volmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/diffusion_limited.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.989808 pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/inverse_kinetics/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/inverse_kinetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/inverse_kinetics/inverse_butler_volmer.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/marcus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/no_reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/tafel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/total_main_kinetics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.989808 pybamm-23.4.1/pybamm/models/submodels/interface/lithium_plating/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/lithium_plating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/lithium_plating/base_plating.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/lithium_plating/no_plating.py
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/lithium_plating/plating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.989808 pybamm-23.4.1/pybamm/models/submodels/interface/open_circuit_potential/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/open_circuit_potential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/open_circuit_potential/base_ocp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/open_circuit_potential/current_sigmoid_ocp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/open_circuit_potential/single_ocp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.989808 pybamm-23.4.1/pybamm/models/submodels/interface/sei/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/sei/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/sei/base_sei.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/sei/constant_sei.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/sei/no_sei.py
--rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/sei/sei_growth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/sei/total_sei.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/interface/total_interfacial_current.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.993808 pybamm-23.4.1/pybamm/models/submodels/oxygen_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/oxygen_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/oxygen_diffusion/base_oxygen_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/oxygen_diffusion/full_oxygen_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/oxygen_diffusion/leading_oxygen_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/oxygen_diffusion/no_oxygen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.993808 pybamm-23.4.1/pybamm/models/submodels/particle/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/particle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17647 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/particle/base_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    13369 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/particle/fickian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    14694 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/particle/polynomial_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/particle/total_particle_concentration.py
--rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/particle/x_averaged_polynomial_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.993808 pybamm-23.4.1/pybamm/models/submodels/particle_mechanics/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/particle_mechanics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/particle_mechanics/base_mechanics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/particle_mechanics/crack_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/particle_mechanics/no_mechanics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/particle_mechanics/swelling_only.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.993808 pybamm-23.4.1/pybamm/models/submodels/porosity/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/porosity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/porosity/base_porosity.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/porosity/constant_porosity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/porosity/reaction_driven_porosity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/porosity/reaction_driven_porosity_ode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.993808 pybamm-23.4.1/pybamm/models/submodels/thermal/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/thermal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/thermal/base_thermal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/thermal/isothermal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/thermal/lumped.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.997808 pybamm-23.4.1/pybamm/models/submodels/thermal/pouch_cell/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/thermal/pouch_cell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_1D_current_collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_2D_current_collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/thermal/x_full.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.997808 pybamm-23.4.1/pybamm/models/submodels/transport_efficiency/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/transport_efficiency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/transport_efficiency/base_transport_efficiency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/models/submodels/transport_efficiency/bruggeman_transport_efficiency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.997808 pybamm-23.4.1/pybamm/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/parameters/base_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/parameters/bpx.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/parameters/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/parameters/ecm_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/parameters/electrical_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/parameters/geometric_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14849 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/parameters/lead_acid_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    24346 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/parameters/lithium_ion_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/parameters/parameter_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)    43817 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/parameters/parameter_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/parameters/process_parameter_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/parameters/size_distribution_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/parameters/thermal_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/parameters_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.997808 pybamm-23.4.1/pybamm/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/plotting/dynamic_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/plotting/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/plotting/plot2D.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/plotting/plot_summary_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/plotting/plot_voltage_components.py
--rw-r--r--   0 runner    (1001) docker     (123)    33580 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/plotting/quick_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    46927 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:07.001808 pybamm-23.4.1/pybamm/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/solvers/algebraic_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    64653 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/solvers/base_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:07.001808 pybamm-23.4.1/pybamm/solvers/c_solvers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/solvers/c_solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/solvers/casadi_algebraic_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    32025 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/solvers/casadi_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/solvers/dummy_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    20772 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/solvers/idaklu_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    39216 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/solvers/jax_bdf_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/solvers/jax_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/solvers/lrudict.py
--rw-r--r--   0 runner    (1001) docker     (123)    18355 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/solvers/processed_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/solvers/scikits_dae_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/solvers/scikits_ode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/solvers/scipy_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    31865 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/solvers/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:07.001808 pybamm-23.4.1/pybamm/spatial_methods/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/spatial_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57884 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/spatial_methods/finite_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/spatial_methods/scikit_finite_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    16777 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/spatial_methods/spatial_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    28643 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/spatial_methods/spectral_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/spatial_methods/zero_dimensional_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 15:23:57.000000 pybamm-23.4.1/pybamm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:24:06.929808 pybamm-23.4.1/pybamm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41858 2023-05-02 15:24:06.000000 pybamm-23.4.1/pybamm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23548 2023-05-02 15:24:06.000000 pybamm-23.4.1/pybamm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:24:06.000000 pybamm-23.4.1/pybamm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-02 15:24:06.000000 pybamm-23.4.1/pybamm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-02 15:24:06.000000 pybamm-23.4.1/pybamm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 15:24:06.000000 pybamm-23.4.1/pybamm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 15:24:07.005808 pybamm-23.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-05-02 15:23:57.000000 pybamm-23.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.928978 pybamm-23.5rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-06-19 14:33:41.000000 pybamm-23.5rc0/CMakeBuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-19 14:33:41.000000 pybamm-23.5rc0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    43200 2023-06-19 14:33:45.928978 pybamm-23.5rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40154 2023-06-19 14:33:41.000000 pybamm-23.5rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.896978 pybamm-23.5rc0/pybamm/
+-rw-r--r--   0 runner    (1001) docker     (123)    20084 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/CITATIONS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/batch_study.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/citations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.896978 pybamm-23.5rc0/pybamm/discretisations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/discretisations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46989 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/discretisations/discretisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/doc_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.896978 pybamm-23.5rc0/pybamm/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/experiment/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.900978 pybamm-23.5rc0/pybamm/expression_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12502 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/averages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50702 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/binary_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21364 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/broadcasts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18611 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/concatenations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15196 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/independent_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/input_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/interpolant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.900978 pybamm-23.5rc0/pybamm/expression_tree/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/operations/convert_to_casadi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26210 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/operations/evaluate_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/operations/jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/operations/latexify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/operations/unpack_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.900978 pybamm-23.5rc0/pybamm/expression_tree/printing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/printing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/printing/print_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/printing/sympy_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/state_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32988 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39893 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/unary_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/expression_tree/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.900978 pybamm-23.5rc0/pybamm/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/geometry/battery_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/geometry/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/geometry/standard_spatial_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.900978 pybamm-23.5rc0/pybamm/input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.888978 pybamm-23.5rc0/pybamm/input/discharge_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.900978 pybamm-23.5rc0/pybamm/input/discharge_data/Ecker2015/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Ecker2015/Ecker_1C.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Ecker2015/Ecker_5C.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Ecker2015/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.904978 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/
+-rw-r--r--   0 runner    (1001) docker     (123)   685399 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   180796 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_displacement.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   156316 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_T.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   129670 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    38056 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_displacement.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   125368 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/1C_discharge_T.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    63563 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/1C_discharge_U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20171 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/1C_discharge_displacement.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   158837 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/2C_discharge_T.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    30602 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/2C_discharge_U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/2C_discharge_displacement.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13539 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/stn_2C.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13828 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/stp_2C.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.904978 pybamm-23.5rc0/pybamm/input/drive_cycles/
+-rw-r--r--   0 runner    (1001) docker     (123)    16846 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/drive_cycles/UDDS.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/drive_cycles/US06.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   299508 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/drive_cycles/WLTC.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/drive_cycles/car_current.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.904978 pybamm-23.5rc0/pybamm/input/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.904978 pybamm-23.5rc0/pybamm/input/parameters/ecm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/ecm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.904978 pybamm-23.5rc0/pybamm/input/parameters/ecm/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   135520 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/ecm/data/ecm_example_c1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/ecm/data/ecm_example_dudt.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/ecm/data/ecm_example_ocv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   149886 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/ecm/data/ecm_example_r0.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   149222 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/ecm/data/ecm_example_r1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/ecm/example_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.908978 pybamm-23.5rc0/pybamm/input/parameters/lead_acid/
+-rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lead_acid/Sulzer2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lead_acid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.908978 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/
+-rw-r--r--   0 runner    (1001) docker     (123)    25833 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Ai2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Chen2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17412 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Chen2020_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21798 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Ecker2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18917 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Marquis2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18050 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Mohtat2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17352 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/NCA_Kim2011.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25674 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/OKane2022.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30791 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/ORegan2022.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Prada2013.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18649 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Ramadass2004.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Xu2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.908978 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/graphite_LGM50_ocp_Chen2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Ecker2015.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Enertech_Ai2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11504 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/lico2_ocp_Ai2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/measured_graphite_diffusivity_Ecker2015.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/measured_nco_diffusivity_Ecker2015.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/nca_ocp_Kim2011_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/nco_ocp_Ecker2015.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/nmc_LGM50_ocp_Chen2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/install_odes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.908978 pybamm-23.5rc0/pybamm/meshes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/meshes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/meshes/meshes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/meshes/one_dimensional_submeshes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/meshes/scikit_fem_submeshes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/meshes/zero_dimensional_submesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.908978 pybamm-23.5rc0/pybamm/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47327 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.908978 pybamm-23.5rc0/pybamm/models/full_battery_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56548 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/base_battery_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.908978 pybamm-23.5rc0/pybamm/models/full_battery_models/equivalent_circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/equivalent_circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/equivalent_circuit/ecm_model_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/equivalent_circuit/thevenin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.912978 pybamm-23.5rc0/pybamm/models/full_battery_models/lead_acid/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lead_acid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lead_acid/base_lead_acid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lead_acid/basic_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lead_acid/full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lead_acid/loqs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.912978 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/Yang2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17815 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/base_lithium_ion_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/basic_dfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16915 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/basic_dfn_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/basic_dfn_half_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/basic_spm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/dfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26674 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/electrode_soh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/electrode_soh_half_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/mpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/newman_tobias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/spm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/spme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.912978 pybamm-23.5rc0/pybamm/models/submodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.912978 pybamm-23.5rc0/pybamm/models/submodels/active_material/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/active_material/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/active_material/base_active_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/active_material/constant_active_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/active_material/loss_active_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/active_material/total_active_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/base_submodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.912978 pybamm-23.5rc0/pybamm/models/submodels/convection/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/base_convection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.912978 pybamm-23.5rc0/pybamm/models/submodels/convection/through_cell/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/through_cell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/through_cell/base_through_cell_convection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/through_cell/explicit_convection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/through_cell/full_convection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/through_cell/no_convection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.912978 pybamm-23.5rc0/pybamm/models/submodels/convection/transverse/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/transverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/transverse/base_transverse_convection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/transverse/full_convection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/transverse/no_convection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/convection/transverse/uniform_convection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.916978 pybamm-23.5rc0/pybamm/models/submodels/current_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/current_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/current_collector/base_current_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14845 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/current_collector/effective_resistance_current_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/current_collector/homogeneous_current_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/current_collector/potential_pair.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.916978 pybamm-23.5rc0/pybamm/models/submodels/electrode/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrode/base_electrode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.916978 pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/base_ohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/composite_ohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/full_ohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/leading_ohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/li_metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/surface_form_ohm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.916978 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/base_electrolyte_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/composite_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/full_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/integrated_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/leading_order_conductivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.916978 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/composite_surface_form_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/explicit_surface_form_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/full_surface_form_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/leading_surface_form_conductivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.916978 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_diffusion/base_electrolyte_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_diffusion/constant_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_diffusion/full_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/electrolyte_diffusion/leading_order_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.916978 pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/ocv_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/rc_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/resistor_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/thermal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/voltage_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.916978 pybamm-23.5rc0/pybamm/models/submodels/external_circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/external_circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/external_circuit/base_external_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/external_circuit/explicit_control_external_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/external_circuit/function_control_external_circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.916978 pybamm-23.5rc0/pybamm/models/submodels/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/base_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.920978 pybamm-23.5rc0/pybamm/models/submodels/interface/interface_utilisation/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/interface_utilisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/interface_utilisation/base_utilisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/interface_utilisation/constant_utilisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/interface_utilisation/current_driven_utilisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/interface_utilisation/full_utilisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.920978 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/base_kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/butler_volmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/diffusion_limited.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.920978 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/inverse_kinetics/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/inverse_kinetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/inverse_kinetics/inverse_butler_volmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/marcus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/no_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/tafel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/total_main_kinetics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.920978 pybamm-23.5rc0/pybamm/models/submodels/interface/lithium_plating/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/lithium_plating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/lithium_plating/base_plating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/lithium_plating/no_plating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/lithium_plating/plating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.920978 pybamm-23.5rc0/pybamm/models/submodels/interface/open_circuit_potential/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/open_circuit_potential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/open_circuit_potential/base_ocp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/open_circuit_potential/current_sigmoid_ocp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/open_circuit_potential/single_ocp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.920978 pybamm-23.5rc0/pybamm/models/submodels/interface/sei/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/sei/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/sei/base_sei.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/sei/constant_sei.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/sei/no_sei.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/sei/sei_growth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/sei/total_sei.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/interface/total_interfacial_current.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.920978 pybamm-23.5rc0/pybamm/models/submodels/oxygen_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/oxygen_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/oxygen_diffusion/base_oxygen_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/oxygen_diffusion/full_oxygen_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/oxygen_diffusion/leading_oxygen_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/oxygen_diffusion/no_oxygen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.920978 pybamm-23.5rc0/pybamm/models/submodels/particle/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17647 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle/base_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13369 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle/fickian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14694 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle/polynomial_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle/total_particle_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle/x_averaged_polynomial_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.924978 pybamm-23.5rc0/pybamm/models/submodels/particle_mechanics/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle_mechanics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle_mechanics/base_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle_mechanics/crack_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle_mechanics/no_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/particle_mechanics/swelling_only.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.924978 pybamm-23.5rc0/pybamm/models/submodels/porosity/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/porosity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/porosity/base_porosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/porosity/constant_porosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/porosity/reaction_driven_porosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/porosity/reaction_driven_porosity_ode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.924978 pybamm-23.5rc0/pybamm/models/submodels/thermal/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/thermal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/thermal/base_thermal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/thermal/isothermal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/thermal/lumped.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.924978 pybamm-23.5rc0/pybamm/models/submodels/thermal/pouch_cell/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/thermal/pouch_cell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_1D_current_collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_2D_current_collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/thermal/x_full.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.924978 pybamm-23.5rc0/pybamm/models/submodels/transport_efficiency/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/transport_efficiency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/transport_efficiency/base_transport_efficiency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/models/submodels/transport_efficiency/bruggeman_transport_efficiency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.924978 pybamm-23.5rc0/pybamm/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/base_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/bpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/ecm_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/electrical_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/geometric_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14849 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/lead_acid_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24346 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/lithium_ion_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/parameter_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32021 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/parameter_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/process_parameter_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/size_distribution_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters/thermal_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/parameters_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.924978 pybamm-23.5rc0/pybamm/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/plotting/dynamic_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/plotting/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/plotting/plot2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/plotting/plot_summary_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/plotting/plot_voltage_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33580 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/plotting/quick_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47298 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.928978 pybamm-23.5rc0/pybamm/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/algebraic_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65427 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/base_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.928978 pybamm-23.5rc0/pybamm/solvers/c_solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/c_solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/casadi_algebraic_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32028 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/casadi_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/dummy_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21833 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/idaklu_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38492 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/jax_bdf_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/jax_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/lrudict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18355 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/processed_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/scikits_dae_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/scikits_ode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/scipy_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33604 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/solvers/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.928978 pybamm-23.5rc0/pybamm/spatial_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/spatial_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57884 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/spatial_methods/finite_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/spatial_methods/scikit_finite_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16777 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/spatial_methods/spatial_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28643 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/spatial_methods/spectral_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/spatial_methods/zero_dimensional_method.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.928978 pybamm-23.5rc0/pybamm/step/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/step/_steps_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/step/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-19 14:33:41.000000 pybamm-23.5rc0/pybamm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:33:45.896978 pybamm-23.5rc0/pybamm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43200 2023-06-19 14:33:45.000000 pybamm-23.5rc0/pybamm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16091 2023-06-19 14:33:45.000000 pybamm-23.5rc0/pybamm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 14:33:45.000000 pybamm-23.5rc0/pybamm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-19 14:33:45.000000 pybamm-23.5rc0/pybamm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-19 14:33:45.000000 pybamm-23.5rc0/pybamm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 14:33:45.000000 pybamm-23.5rc0/pybamm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 14:33:45.928978 pybamm-23.5rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-06-19 14:33:41.000000 pybamm-23.5rc0/setup.py
```

### Comparing `pybamm-23.4.1/CMakeBuild.py` & `pybamm-23.5rc0/CMakeBuild.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/LICENSE.txt` & `pybamm-23.5rc0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/PKG-INFO` & `pybamm-23.5rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: pybamm
-Version: 23.4.1
+Version: 23.5rc0
 Summary: Python Battery Mathematical Modelling.
 Home-page: https://github.com/pybamm-team/PyBaMM
 License: UNKNOWN
 Description: ![PyBaMM_logo](https://user-images.githubusercontent.com/20817509/107091287-8ad46a80-67cf-11eb-86f5-7ebef7c72a1e.png)
         
         #
         
         <div align="center">
         
         [![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](http://numfocus.org)
-        [![Build](https://github.com/pybamm-team/PyBaMM/workflows/PyBaMM/badge.svg)](https://github.com/pybamm-team/PyBaMM/actions?query=workflow%3APyBaMM+branch%3Adevelop)
+        [![Scheduled](https://github.com/pybamm-team/PyBaMM/actions/workflows/run_periodic_tests.yml/badge.svg?branch=develop)](https://github.com/pybamm-team/PyBaMM/actions/workflows/run_periodic_tests.yml)
         [![readthedocs](https://readthedocs.org/projects/pybamm/badge/?version=latest)](https://pybamm.readthedocs.io/en/latest/?badge=latest)
         [![codecov](https://codecov.io/gh/pybamm-team/PyBaMM/branch/main/graph/badge.svg)](https://codecov.io/gh/pybamm-team/PyBaMM)
         [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pybamm-team/PyBaMM/blob/develop/)
         [![DOI](https://zenodo.org/badge/DOI/10.5334/jors.309.svg)](https://doi.org/10.5334/jors.309)
         [![release](https://img.shields.io/github/v/release/pybamm-team/PyBaMM?color=yellow)](https://github.com/pybamm-team/PyBaMM/releases)
         [![black code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
         
         <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-        [![All Contributors](https://img.shields.io/badge/all_contributors-54-orange.svg)](#-contributors)
+        [![All Contributors](https://img.shields.io/badge/all_contributors-58-orange.svg)](#-contributors)
         <!-- ALL-CONTRIBUTORS-BADGE:END -->
         
         </div>
         
         # PyBaMM
         
         PyBaMM (Python Battery Mathematical Modelling) is an open-source battery simulation package
@@ -248,19 +248,24 @@
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/abillscmu"><img src="https://avatars.githubusercontent.com/u/48105066?v=4?s=100" width="100px;" alt="Alec Bills"/><br /><sub><b>Alec Bills</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=abillscmu" title="Code">💻</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/agriyakhetarpal"><img src="https://avatars.githubusercontent.com/u/74401230?v=4?s=100" width="100px;" alt="Agriya Khetarpal"/><br /><sub><b>Agriya Khetarpal</b></sub></a><br /><a href="#infra-agriyakhetarpal" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=agriyakhetarpal" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=agriyakhetarpal" title="Documentation">📖</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/awadell1"><img src="https://avatars.githubusercontent.com/u/5857298?v=4?s=100" width="100px;" alt="Alex Wadell"/><br /><sub><b>Alex Wadell</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=awadell1" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=awadell1" title="Tests">⚠️</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=awadell1" title="Documentation">📖</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/iatzak"><img src="https://avatars.githubusercontent.com/u/112731474?v=4?s=100" width="100px;" alt="iatzak"/><br /><sub><b>iatzak</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=iatzak" title="Documentation">📖</a> <a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Aiatzak" title="Bug reports">🐛</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=iatzak" title="Code">💻</a></td>
             </tr>
             <tr>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/ayeankit"><img src="https://avatars.githubusercontent.com/u/72691866?v=4?s=100" width="100px;" alt="Ankit Kumar"/><br /><sub><b>Ankit Kumar</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=ayeankit" title="Code">💻</a></td>
-              <td align="center" valign="top" width="14.28%"><a href="https://aniketsinghrawat.vercel.app/"><img src="https://avatars.githubusercontent.com/u/31622972?v=4?s=100" width="100px;" alt="Aniket Singh Rawat"/><br /><sub><b>Aniket Singh Rawat</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=dikwickley" title="Code">💻</a></td>
+              <td align="center" valign="top" width="14.28%"><a href="https://aniketsinghrawat.vercel.app/"><img src="https://avatars.githubusercontent.com/u/31622972?v=4?s=100" width="100px;" alt="Aniket Singh Rawat"/><br /><sub><b>Aniket Singh Rawat</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=dikwickley" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=dikwickley" title="Documentation">📖</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/jeromtom"><img src="https://avatars.githubusercontent.com/u/83979298?v=4?s=100" width="100px;" alt="Jerom Palimattom Tom"/><br /><sub><b>Jerom Palimattom Tom</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=jeromtom" title="Documentation">📖</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=jeromtom" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=jeromtom" title="Tests">⚠️</a></td>
               <td align="center" valign="top" width="14.28%"><a href="http://bradyplanden.github.io"><img src="https://avatars.githubusercontent.com/u/55357039?v=4?s=100" width="100px;" alt="Brady Planden"/><br /><sub><b>Brady Planden</b></sub></a><br /><a href="#example-BradyPlanden" title="Examples">💡</a></td>
               <td align="center" valign="top" width="14.28%"><a href="http://www.jsbrittain.com/"><img src="https://avatars.githubusercontent.com/u/98161205?v=4?s=100" width="100px;" alt="jsbrittain"/><br /><sub><b>jsbrittain</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=jsbrittain" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=jsbrittain" title="Tests">⚠️</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/arjxn-py"><img src="https://avatars.githubusercontent.com/u/104268427?v=4?s=100" width="100px;" alt="Arjun"/><br /><sub><b>Arjun</b></sub></a><br /><a href="#infra-arjxn-py" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
+              <td align="center" valign="top" width="14.28%"><a href="https://github.com/chenzhao-py"><img src="https://avatars.githubusercontent.com/u/75906533?v=4?s=100" width="100px;" alt="CHEN ZHAO"/><br /><sub><b>CHEN ZHAO</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Achenzhao-py" title="Bug reports">🐛</a></td>
+            </tr>
+            <tr>
+              <td align="center" valign="top" width="14.28%"><a href="https://www.aboutenergy.io/"><img src="https://avatars.githubusercontent.com/u/91731499?v=4?s=100" width="100px;" alt="darryl-ad"/><br /><sub><b>darryl-ad</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=darryl-ad" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Adarryl-ad" title="Bug reports">🐛</a></td>
+              <td align="center" valign="top" width="14.28%"><a href="https://github.com/julian-evers"><img src="https://avatars.githubusercontent.com/u/133691040?v=4?s=100" width="100px;" alt="julian-evers"/><br /><sub><b>julian-evers</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=julian-evers" title="Code">💻</a></td>
             </tr>
           </tbody>
         </table>
         
         <!-- markdownlint-restore -->
         <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: pybamm Version: 23.4.1 Summary: Python Battery
+Metadata-Version: 2.1 Name: pybamm Version: 23.5rc0 Summary: Python Battery
 Mathematical Modelling. Home-page: https://github.com/pybamm-team/PyBaMM
 License: UNKNOWN Description: ![PyBaMM_logo](https://user-
 images.githubusercontent.com/20817509/107091287-8ad46a80-67cf-11eb-86f5-
 7ebef7c72a1e.png) #
   [![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-
   orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](http://numfocus.org) [!
-  [Build](https://github.com/pybamm-team/PyBaMM/workflows/PyBaMM/badge.svg)]
-                    (https://github.com/pybamm-team/PyBaMM/
-  actions?query=workflow%3APyBaMM+branch%3Adevelop) [![readthedocs](https://
+     [Scheduled](https://github.com/pybamm-team/PyBaMM/actions/workflows/
+ run_periodic_tests.yml/badge.svg?branch=develop)](https://github.com/pybamm-
+team/PyBaMM/actions/workflows/run_periodic_tests.yml) [![readthedocs](https://
        readthedocs.org/projects/pybamm/badge/?version=latest)](https://
 pybamm.readthedocs.io/en/latest/?badge=latest) [![codecov](https://codecov.io/
   gh/pybamm-team/PyBaMM/branch/main/graph/badge.svg)](https://codecov.io/gh/
 pybamm-team/PyBaMM) [![Open In Colab](https://colab.research.google.com/assets/
 colab-badge.svg)](https://colab.research.google.com/github/pybamm-team/PyBaMM/
   blob/develop/) [![DOI](https://zenodo.org/badge/DOI/10.5334/jors.309.svg)]
 (https://doi.org/10.5334/jors.309) [![release](https://img.shields.io/github/v/
    release/pybamm-team/PyBaMM?color=yellow)](https://github.com/pybamm-team/
       PyBaMM/releases) [![black code style](https://img.shields.io/badge/
     code%20style-black-000000.svg)](https://github.com/ambv/black)  [![All
-Contributors](https://img.shields.io/badge/all_contributors-54-orange.svg)](#-
+Contributors](https://img.shields.io/badge/all_contributors-58-orange.svg)](#-
                                 contributors)
 # PyBaMM PyBaMM (Python Battery Mathematical Modelling) is an open-source
 battery simulation package written in Python. Our mission is to accelerate
 battery modelling research by providing open-source tools for multi-
 institutional, interdisciplinary collaboration. Broadly, PyBaMM consists of (i)
 a framework for writing and solving systems of differential equations, (ii) a
 library of battery models and parameters, and (iii) specialized tools for
@@ -144,17 +144,20 @@
                                                          ð ð»                                                                          ð¤                                                                         ð»                                                              ð» â ï¸                                                                   ð» â ï¸                                                            ð» ð¤                                             ð¤ ð» â ï¸ â
                                                         [Chuck_Liu]                                                                              [partben]                                                                    [Gavin_Wiggins]                                                               [Dion_Wilde]                                                                               [Elias_Hohl]                                                                    [KAschad]                                                            [Vaibhav-Chopra-GT]
                                                          Chuck_Liu                                                                                partben                                                                      Gavin_Wiggins                                                                 Dion_Wilde                                                                                 Elias_Hohl                                                                      KAschad                                                              Vaibhav-Chopra-GT
                                                          ð ð»                                                                          ð                                                                     ð ð»                                                            ð ð»                                                                            ð»                                                                      ð                                                                  ð»
                                                        [bardsleypt]                                                                          [ndrewwang]                                                                          [MichaPhilipp]                                                               [Alec_Bills]                                                                  [Agriya_Khetarpal]                                                              [Alex_Wadell]                                                                  [iatzak]
                                                         bardsleypt                                                                            ndrewwang                                                                            MichaPhilipp                                                                 Alec_Bills                                                                    Agriya_Khetarpal                                                                Alex_Wadell                                                                    iatzak
                                                          ð ð»                                                                    ð ð»                                                                        ð                                                                    ð»                                                                    ð ð» ð                                                  ð» â ï¸ ð                                                ð ð ð»
-                                                          [Ankit_Kumar]                                                                   [Aniket_Singh_Rawat]                                                        [Jerom_Palimattom_Tom]                                                                 [Brady_Planden]                                                                      [jsbrittain]                                                                          [Arjun]
-                                                           Ankit_Kumar                                                                     Aniket_Singh_Rawat                                                          Jerom_Palimattom_Tom                                                                   Brady_Planden                                                                        jsbrittain                                                                            Arjun
-                                                              ð»                                                                            ð»                                                               ð ð» â ï¸                                                           ð¡                                                                         ð» â ï¸                                                                 ð
+                                                          [Ankit_Kumar]                                                                  [Aniket_Singh_Rawat]                                                         [Jerom_Palimattom_Tom]                                                                 [Brady_Planden]                                                                      [jsbrittain]                                                                          [Arjun]                                                                   [CHEN_ZHAO]
+                                                           Ankit_Kumar                                                                    Aniket_Singh_Rawat                                                           Jerom_Palimattom_Tom                                                                   Brady_Planden                                                                        jsbrittain                                                                            Arjun                                                                     CHEN_ZHAO
+                                                              ð»                                                                        ð» ð                                                          ð ð» â ï¸                                                           ð¡                                                                         ð» â ï¸                                                                 ð                                                                    ð
+                                                        [darryl-ad]                                                                            [julian-evers]
+                                                         darryl-ad                                                                              julian-evers
+                                                         ð» ð                                                                          ð»
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome! Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
```

### Comparing `pybamm-23.4.1/README.md` & `pybamm-23.5rc0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 ![PyBaMM_logo](https://user-images.githubusercontent.com/20817509/107091287-8ad46a80-67cf-11eb-86f5-7ebef7c72a1e.png)
 
 #
 
 <div align="center">
 
 [![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](http://numfocus.org)
-[![Build](https://github.com/pybamm-team/PyBaMM/workflows/PyBaMM/badge.svg)](https://github.com/pybamm-team/PyBaMM/actions?query=workflow%3APyBaMM+branch%3Adevelop)
+[![Scheduled](https://github.com/pybamm-team/PyBaMM/actions/workflows/run_periodic_tests.yml/badge.svg?branch=develop)](https://github.com/pybamm-team/PyBaMM/actions/workflows/run_periodic_tests.yml)
 [![readthedocs](https://readthedocs.org/projects/pybamm/badge/?version=latest)](https://pybamm.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/pybamm-team/PyBaMM/branch/main/graph/badge.svg)](https://codecov.io/gh/pybamm-team/PyBaMM)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pybamm-team/PyBaMM/blob/develop/)
 [![DOI](https://zenodo.org/badge/DOI/10.5334/jors.309.svg)](https://doi.org/10.5334/jors.309)
 [![release](https://img.shields.io/github/v/release/pybamm-team/PyBaMM?color=yellow)](https://github.com/pybamm-team/PyBaMM/releases)
 [![black code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-54-orange.svg)](#-contributors)
+[![All Contributors](https://img.shields.io/badge/all_contributors-58-orange.svg)](#-contributors)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 </div>
 
 # PyBaMM
 
 PyBaMM (Python Battery Mathematical Modelling) is an open-source battery simulation package
@@ -242,19 +242,24 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/abillscmu"><img src="https://avatars.githubusercontent.com/u/48105066?v=4?s=100" width="100px;" alt="Alec Bills"/><br /><sub><b>Alec Bills</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=abillscmu" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/agriyakhetarpal"><img src="https://avatars.githubusercontent.com/u/74401230?v=4?s=100" width="100px;" alt="Agriya Khetarpal"/><br /><sub><b>Agriya Khetarpal</b></sub></a><br /><a href="#infra-agriyakhetarpal" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=agriyakhetarpal" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=agriyakhetarpal" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/awadell1"><img src="https://avatars.githubusercontent.com/u/5857298?v=4?s=100" width="100px;" alt="Alex Wadell"/><br /><sub><b>Alex Wadell</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=awadell1" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=awadell1" title="Tests">⚠️</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=awadell1" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/iatzak"><img src="https://avatars.githubusercontent.com/u/112731474?v=4?s=100" width="100px;" alt="iatzak"/><br /><sub><b>iatzak</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=iatzak" title="Documentation">📖</a> <a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Aiatzak" title="Bug reports">🐛</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=iatzak" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ayeankit"><img src="https://avatars.githubusercontent.com/u/72691866?v=4?s=100" width="100px;" alt="Ankit Kumar"/><br /><sub><b>Ankit Kumar</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=ayeankit" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://aniketsinghrawat.vercel.app/"><img src="https://avatars.githubusercontent.com/u/31622972?v=4?s=100" width="100px;" alt="Aniket Singh Rawat"/><br /><sub><b>Aniket Singh Rawat</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=dikwickley" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://aniketsinghrawat.vercel.app/"><img src="https://avatars.githubusercontent.com/u/31622972?v=4?s=100" width="100px;" alt="Aniket Singh Rawat"/><br /><sub><b>Aniket Singh Rawat</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=dikwickley" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=dikwickley" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jeromtom"><img src="https://avatars.githubusercontent.com/u/83979298?v=4?s=100" width="100px;" alt="Jerom Palimattom Tom"/><br /><sub><b>Jerom Palimattom Tom</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=jeromtom" title="Documentation">📖</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=jeromtom" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=jeromtom" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://bradyplanden.github.io"><img src="https://avatars.githubusercontent.com/u/55357039?v=4?s=100" width="100px;" alt="Brady Planden"/><br /><sub><b>Brady Planden</b></sub></a><br /><a href="#example-BradyPlanden" title="Examples">💡</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://www.jsbrittain.com/"><img src="https://avatars.githubusercontent.com/u/98161205?v=4?s=100" width="100px;" alt="jsbrittain"/><br /><sub><b>jsbrittain</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=jsbrittain" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=jsbrittain" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/arjxn-py"><img src="https://avatars.githubusercontent.com/u/104268427?v=4?s=100" width="100px;" alt="Arjun"/><br /><sub><b>Arjun</b></sub></a><br /><a href="#infra-arjxn-py" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/chenzhao-py"><img src="https://avatars.githubusercontent.com/u/75906533?v=4?s=100" width="100px;" alt="CHEN ZHAO"/><br /><sub><b>CHEN ZHAO</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Achenzhao-py" title="Bug reports">🐛</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://www.aboutenergy.io/"><img src="https://avatars.githubusercontent.com/u/91731499?v=4?s=100" width="100px;" alt="darryl-ad"/><br /><sub><b>darryl-ad</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=darryl-ad" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Adarryl-ad" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/julian-evers"><img src="https://avatars.githubusercontent.com/u/133691040?v=4?s=100" width="100px;" alt="julian-evers"/><br /><sub><b>julian-evers</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=julian-evers" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
 ![PyBaMM_logo](https://user-images.githubusercontent.com/20817509/107091287-
 8ad46a80-67cf-11eb-86f5-7ebef7c72a1e.png) #
   [![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-
   orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](http://numfocus.org) [!
-  [Build](https://github.com/pybamm-team/PyBaMM/workflows/PyBaMM/badge.svg)]
-                    (https://github.com/pybamm-team/PyBaMM/
-  actions?query=workflow%3APyBaMM+branch%3Adevelop) [![readthedocs](https://
+     [Scheduled](https://github.com/pybamm-team/PyBaMM/actions/workflows/
+ run_periodic_tests.yml/badge.svg?branch=develop)](https://github.com/pybamm-
+team/PyBaMM/actions/workflows/run_periodic_tests.yml) [![readthedocs](https://
        readthedocs.org/projects/pybamm/badge/?version=latest)](https://
 pybamm.readthedocs.io/en/latest/?badge=latest) [![codecov](https://codecov.io/
   gh/pybamm-team/PyBaMM/branch/main/graph/badge.svg)](https://codecov.io/gh/
 pybamm-team/PyBaMM) [![Open In Colab](https://colab.research.google.com/assets/
 colab-badge.svg)](https://colab.research.google.com/github/pybamm-team/PyBaMM/
   blob/develop/) [![DOI](https://zenodo.org/badge/DOI/10.5334/jors.309.svg)]
 (https://doi.org/10.5334/jors.309) [![release](https://img.shields.io/github/v/
    release/pybamm-team/PyBaMM?color=yellow)](https://github.com/pybamm-team/
       PyBaMM/releases) [![black code style](https://img.shields.io/badge/
     code%20style-black-000000.svg)](https://github.com/ambv/black)  [![All
-Contributors](https://img.shields.io/badge/all_contributors-54-orange.svg)](#-
+Contributors](https://img.shields.io/badge/all_contributors-58-orange.svg)](#-
                                 contributors)
 # PyBaMM PyBaMM (Python Battery Mathematical Modelling) is an open-source
 battery simulation package written in Python. Our mission is to accelerate
 battery modelling research by providing open-source tools for multi-
 institutional, interdisciplinary collaboration. Broadly, PyBaMM consists of (i)
 a framework for writing and solving systems of differential equations, (ii) a
 library of battery models and parameters, and (iii) specialized tools for
@@ -141,13 +141,16 @@
                                                          ð ð»                                                                          ð¤                                                                         ð»                                                              ð» â ï¸                                                                   ð» â ï¸                                                            ð» ð¤                                             ð¤ ð» â ï¸ â
                                                         [Chuck_Liu]                                                                              [partben]                                                                    [Gavin_Wiggins]                                                               [Dion_Wilde]                                                                               [Elias_Hohl]                                                                    [KAschad]                                                            [Vaibhav-Chopra-GT]
                                                          Chuck_Liu                                                                                partben                                                                      Gavin_Wiggins                                                                 Dion_Wilde                                                                                 Elias_Hohl                                                                      KAschad                                                              Vaibhav-Chopra-GT
                                                          ð ð»                                                                          ð                                                                     ð ð»                                                            ð ð»                                                                            ð»                                                                      ð                                                                  ð»
                                                        [bardsleypt]                                                                          [ndrewwang]                                                                          [MichaPhilipp]                                                               [Alec_Bills]                                                                  [Agriya_Khetarpal]                                                              [Alex_Wadell]                                                                  [iatzak]
                                                         bardsleypt                                                                            ndrewwang                                                                            MichaPhilipp                                                                 Alec_Bills                                                                    Agriya_Khetarpal                                                                Alex_Wadell                                                                    iatzak
                                                          ð ð»                                                                    ð ð»                                                                        ð                                                                    ð»                                                                    ð ð» ð                                                  ð» â ï¸ ð                                                ð ð ð»
-                                                          [Ankit_Kumar]                                                                   [Aniket_Singh_Rawat]                                                        [Jerom_Palimattom_Tom]                                                                 [Brady_Planden]                                                                      [jsbrittain]                                                                          [Arjun]
-                                                           Ankit_Kumar                                                                     Aniket_Singh_Rawat                                                          Jerom_Palimattom_Tom                                                                   Brady_Planden                                                                        jsbrittain                                                                            Arjun
-                                                              ð»                                                                            ð»                                                               ð ð» â ï¸                                                           ð¡                                                                         ð» â ï¸                                                                 ð
+                                                          [Ankit_Kumar]                                                                  [Aniket_Singh_Rawat]                                                         [Jerom_Palimattom_Tom]                                                                 [Brady_Planden]                                                                      [jsbrittain]                                                                          [Arjun]                                                                   [CHEN_ZHAO]
+                                                           Ankit_Kumar                                                                    Aniket_Singh_Rawat                                                           Jerom_Palimattom_Tom                                                                   Brady_Planden                                                                        jsbrittain                                                                            Arjun                                                                     CHEN_ZHAO
+                                                              ð»                                                                        ð» ð                                                          ð ð» â ï¸                                                           ð¡                                                                         ð» â ï¸                                                                 ð                                                                    ð
+                                                        [darryl-ad]                                                                            [julian-evers]
+                                                         darryl-ad                                                                              julian-evers
+                                                         ð» ð                                                                          ð»
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `pybamm-23.4.1/pybamm/CITATIONS.txt` & `pybamm-23.5rc0/pybamm/CITATIONS.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/__init__.py` & `pybamm-23.5rc0/pybamm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 
 #
 # Utility classes and methods
 #
 from .util import Timer, TimerTime, FuzzyDict
 from .util import (
     root_dir,
-    load_function,
     rmse,
     load,
     is_constant_and_can_evaluate,
 )
 from .util import (
     get_parameters_filepath,
     have_jax,
@@ -216,16 +215,17 @@
 from .solvers.jax_bdf_solver import jax_bdf_integrate
 
 from .solvers.idaklu_solver import IDAKLUSolver, have_idaklu
 
 #
 # Experiments
 #
-from .experiments.experiment import Experiment
-from . import experiments
+from .experiment.experiment import Experiment
+from . import experiment
+
 
 #
 # Plotting
 #
 from .plotting.quick_plot import QuickPlot, close_plots
 from .plotting.plot import plot
 from .plotting.plot2D import plot2D
```

### Comparing `pybamm-23.4.1/pybamm/batch_study.py` & `pybamm-23.5rc0/pybamm/batch_study.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/callbacks.py` & `pybamm-23.5rc0/pybamm/callbacks.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/discretisations/discretisation.py` & `pybamm-23.5rc0/pybamm/discretisations/discretisation.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/doc_utils.py` & `pybamm-23.5rc0/pybamm/doc_utils.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/array.py` & `pybamm-23.5rc0/pybamm/expression_tree/array.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/averages.py` & `pybamm-23.5rc0/pybamm/expression_tree/averages.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/binary_operators.py` & `pybamm-23.5rc0/pybamm/expression_tree/binary_operators.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/broadcasts.py` & `pybamm-23.5rc0/pybamm/expression_tree/broadcasts.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/concatenations.py` & `pybamm-23.5rc0/pybamm/expression_tree/concatenations.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/exceptions.py` & `pybamm-23.5rc0/pybamm/expression_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/functions.py` & `pybamm-23.5rc0/pybamm/expression_tree/functions.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/independent_variable.py` & `pybamm-23.5rc0/pybamm/expression_tree/independent_variable.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/input_parameter.py` & `pybamm-23.5rc0/pybamm/expression_tree/input_parameter.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/interpolant.py` & `pybamm-23.5rc0/pybamm/expression_tree/interpolant.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/matrix.py` & `pybamm-23.5rc0/pybamm/expression_tree/matrix.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/operations/convert_to_casadi.py` & `pybamm-23.5rc0/pybamm/expression_tree/operations/convert_to_casadi.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/operations/evaluate_python.py` & `pybamm-23.5rc0/pybamm/expression_tree/operations/evaluate_python.py`

 * *Files 0% similar despite different names*

```diff
@@ -555,15 +555,15 @@
         ]
 
         # get a list of hashable arguments to make static
         # a jax device array is not hashable
         static_argnums = (
             i
             for i, c in enumerate(constants.values())
-            if not (isinstance(c, jax.interpreters.xla.DeviceArray))
+            if not (isinstance(c, jax.Array))
         )
 
         # store constants
         self._constants = tuple(constants.values())
 
         # indent code
         python_str = "   " + python_str
```

### Comparing `pybamm-23.4.1/pybamm/expression_tree/operations/jacobian.py` & `pybamm-23.5rc0/pybamm/expression_tree/operations/jacobian.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/operations/latexify.py` & `pybamm-23.5rc0/pybamm/expression_tree/operations/latexify.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/operations/unpack_symbols.py` & `pybamm-23.5rc0/pybamm/expression_tree/operations/unpack_symbols.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/parameter.py` & `pybamm-23.5rc0/pybamm/expression_tree/parameter.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/printing/print_name.py` & `pybamm-23.5rc0/pybamm/expression_tree/printing/print_name.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/printing/sympy_overrides.py` & `pybamm-23.5rc0/pybamm/expression_tree/printing/sympy_overrides.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/scalar.py` & `pybamm-23.5rc0/pybamm/expression_tree/scalar.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/state_vector.py` & `pybamm-23.5rc0/pybamm/expression_tree/state_vector.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/symbol.py` & `pybamm-23.5rc0/pybamm/expression_tree/symbol.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/unary_operators.py` & `pybamm-23.5rc0/pybamm/expression_tree/unary_operators.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/variable.py` & `pybamm-23.5rc0/pybamm/expression_tree/variable.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/expression_tree/vector.py` & `pybamm-23.5rc0/pybamm/expression_tree/vector.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/geometry/battery_geometry.py` & `pybamm-23.5rc0/pybamm/geometry/battery_geometry.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/geometry/geometry.py` & `pybamm-23.5rc0/pybamm/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/geometry/standard_spatial_vars.py` & `pybamm-23.5rc0/pybamm/geometry/standard_spatial_vars.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/discharge_data/Ecker2015/Ecker_1C.csv` & `pybamm-23.5rc0/pybamm/input/discharge_data/Ecker2015/Ecker_1C.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/discharge_data/Ecker2015/Ecker_5C.csv` & `pybamm-23.5rc0/pybamm/input/discharge_data/Ecker2015/Ecker_5C.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/discharge_data/Ecker2015/README.md` & `pybamm-23.5rc0/pybamm/input/discharge_data/Ecker2015/README.md`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_U.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_U.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_displacement.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_displacement.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_T.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_T.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_U.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_U.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_displacement.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_displacement.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/1C_discharge_T.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/1C_discharge_T.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/1C_discharge_U.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/1C_discharge_U.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/1C_discharge_displacement.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/1C_discharge_displacement.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/2C_discharge_T.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/2C_discharge_T.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/2C_discharge_U.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/2C_discharge_U.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/2C_discharge_displacement.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/2C_discharge_displacement.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/README.md` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/README.md`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/stn_2C.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/stn_2C.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/discharge_data/Enertech_cells/stp_2C.txt` & `pybamm-23.5rc0/pybamm/input/discharge_data/Enertech_cells/stp_2C.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/drive_cycles/UDDS.csv` & `pybamm-23.5rc0/pybamm/input/drive_cycles/UDDS.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/drive_cycles/US06.csv` & `pybamm-23.5rc0/pybamm/input/drive_cycles/US06.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/drive_cycles/WLTC.csv` & `pybamm-23.5rc0/pybamm/input/drive_cycles/WLTC.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/ecm/data/ecm_example_c1.csv` & `pybamm-23.5rc0/pybamm/input/parameters/ecm/data/ecm_example_c1.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/ecm/data/ecm_example_dudt.csv` & `pybamm-23.5rc0/pybamm/input/parameters/ecm/data/ecm_example_dudt.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/ecm/data/ecm_example_ocv.csv` & `pybamm-23.5rc0/pybamm/input/parameters/ecm/data/ecm_example_ocv.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/ecm/data/ecm_example_r0.csv` & `pybamm-23.5rc0/pybamm/input/parameters/ecm/data/ecm_example_r0.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/ecm/data/ecm_example_r1.csv` & `pybamm-23.5rc0/pybamm/input/parameters/ecm/data/ecm_example_r1.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/ecm/example_set.py` & `pybamm-23.5rc0/pybamm/input/parameters/ecm/example_set.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lead_acid/Sulzer2019.py` & `pybamm-23.5rc0/pybamm/input/parameters/lead_acid/Sulzer2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lithium_ion/Ai2020.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Ai2020.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lithium_ion/Chen2020.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Chen2020.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lithium_ion/Chen2020_composite.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Chen2020_composite.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lithium_ion/Ecker2015.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Ecker2015.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lithium_ion/Marquis2019.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Marquis2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lithium_ion/Mohtat2020.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Mohtat2020.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lithium_ion/NCA_Kim2011.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/NCA_Kim2011.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lithium_ion/OKane2022.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/OKane2022.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lithium_ion/ORegan2022.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/ORegan2022.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lithium_ion/Prada2013.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Prada2013.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lithium_ion/Ramadass2004.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Ramadass2004.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lithium_ion/Xu2019.py` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/Xu2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lithium_ion/data/graphite_LGM50_ocp_Chen2020.csv` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/graphite_LGM50_ocp_Chen2020.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Ecker2015.csv` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Ecker2015.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Enertech_Ai2020.csv` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Enertech_Ai2020.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lithium_ion/data/lico2_ocp_Ai2020.csv` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/lico2_ocp_Ai2020.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lithium_ion/data/measured_graphite_diffusivity_Ecker2015.csv` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/measured_graphite_diffusivity_Ecker2015.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lithium_ion/data/measured_nco_diffusivity_Ecker2015.csv` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/measured_nco_diffusivity_Ecker2015.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lithium_ion/data/nca_ocp_Kim2011_data.csv` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/nca_ocp_Kim2011_data.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lithium_ion/data/nco_ocp_Ecker2015.csv` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/nco_ocp_Ecker2015.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/input/parameters/lithium_ion/data/nmc_LGM50_ocp_Chen2020.csv` & `pybamm-23.5rc0/pybamm/input/parameters/lithium_ion/data/nmc_LGM50_ocp_Chen2020.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/install_odes.py` & `pybamm-23.5rc0/pybamm/install_odes.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     tar = tarfile.open(archive)
     tar.extractall(directory)
 
 
 def install_sundials(download_dir, install_dir):
     # Download the SUNDIALS library and compile it.
     logger = logging.getLogger("scikits.odes setup")
-    sundials_version = "5.1.0"
+    sundials_version = "6.5.0"
 
     try:
         subprocess.run(["cmake", "--version"])
     except OSError:
         raise RuntimeError("CMake must be installed to build SUNDIALS.")
 
     url = (
@@ -64,19 +64,20 @@
         print("\n-" * 10, "Creating build dir", "-" * 40)
         os.makedirs(build_directory)
 
     print("-" * 10, "Running CMake prepare", "-" * 40)
     subprocess.run(
         ["cmake", "../sundials-{}".format(sundials_version)] + cmake_args,
         cwd=build_directory,
+        check=True,
     )
 
     print("-" * 10, "Building the sundials", "-" * 40)
     make_cmd = ["make", "install"]
-    subprocess.run(make_cmd, cwd=build_directory)
+    subprocess.run(make_cmd, cwd=build_directory, check=True)
 
 
 def update_LD_LIBRARY_PATH(install_dir):
     # Look for current python virtual env and add export statement
     # for LD_LIBRARY_PATH in activate script.  If no virtual env found,
     # then the current user's .bashrc file is modified instead.
 
@@ -165,12 +166,12 @@
     update_LD_LIBRARY_PATH(SUNDIALS_LIB_DIR)
 
     # At the time scikits.odes is pip installed, the path to the sundials
     # library must be contained in an env variable SUNDIALS_INST
     # see https://scikits-odes.readthedocs.io/en/latest/installation.html#id1
     os.environ["SUNDIALS_INST"] = SUNDIALS_LIB_DIR
     env = os.environ.copy()
-    subprocess.run(["pip", "install", "scikits.odes"], env=env)
+    subprocess.run(["pip", "install", "scikits.odes"], env=env, check=True)
 
 
 if __name__ == "__main__":
     main(sys.argv[1:])
```

### Comparing `pybamm-23.4.1/pybamm/logger.py` & `pybamm-23.5rc0/pybamm/logger.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/meshes/meshes.py` & `pybamm-23.5rc0/pybamm/meshes/meshes.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/meshes/one_dimensional_submeshes.py` & `pybamm-23.5rc0/pybamm/meshes/one_dimensional_submeshes.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/meshes/scikit_fem_submeshes.py` & `pybamm-23.5rc0/pybamm/meshes/scikit_fem_submeshes.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/meshes/zero_dimensional_submesh.py` & `pybamm-23.5rc0/pybamm/meshes/zero_dimensional_submesh.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/base_model.py` & `pybamm-23.5rc0/pybamm/models/base_model.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/event.py` & `pybamm-23.5rc0/pybamm/models/event.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/full_battery_models/base_battery_model.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/base_battery_model.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/full_battery_models/equivalent_circuit/ecm_model_options.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/equivalent_circuit/ecm_model_options.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/full_battery_models/equivalent_circuit/thevenin.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/equivalent_circuit/thevenin.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/full_battery_models/lead_acid/base_lead_acid_model.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lead_acid/base_lead_acid_model.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/full_battery_models/lead_acid/basic_full.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lead_acid/basic_full.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/full_battery_models/lead_acid/full.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lead_acid/full.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/full_battery_models/lead_acid/loqs.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lead_acid/loqs.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/__init__.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/__init__.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/base_lithium_ion_model.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/base_lithium_ion_model.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/basic_dfn.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/basic_dfn.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/basic_dfn_composite.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/basic_dfn_composite.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/basic_dfn_half_cell.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/basic_dfn_half_cell.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/basic_spm.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/basic_spm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/dfn.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/dfn.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/electrode_soh.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/electrode_soh.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/electrode_soh_half_cell.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/electrode_soh_half_cell.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/mpm.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/mpm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/newman_tobias.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/newman_tobias.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/spm.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/spm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/full_battery_models/lithium_ion/spme.py` & `pybamm-23.5rc0/pybamm/models/full_battery_models/lithium_ion/spme.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/active_material/base_active_material.py` & `pybamm-23.5rc0/pybamm/models/submodels/active_material/base_active_material.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/active_material/constant_active_material.py` & `pybamm-23.5rc0/pybamm/models/submodels/active_material/constant_active_material.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/active_material/loss_active_material.py` & `pybamm-23.5rc0/pybamm/models/submodels/active_material/loss_active_material.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/active_material/total_active_material.py` & `pybamm-23.5rc0/pybamm/models/submodels/active_material/total_active_material.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/base_submodel.py` & `pybamm-23.5rc0/pybamm/models/submodels/base_submodel.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/convection/base_convection.py` & `pybamm-23.5rc0/pybamm/models/submodels/convection/base_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/convection/through_cell/base_through_cell_convection.py` & `pybamm-23.5rc0/pybamm/models/submodels/convection/through_cell/base_through_cell_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/convection/through_cell/explicit_convection.py` & `pybamm-23.5rc0/pybamm/models/submodels/convection/through_cell/explicit_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/convection/through_cell/full_convection.py` & `pybamm-23.5rc0/pybamm/models/submodels/convection/through_cell/full_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/convection/through_cell/no_convection.py` & `pybamm-23.5rc0/pybamm/models/submodels/convection/through_cell/no_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/convection/transverse/base_transverse_convection.py` & `pybamm-23.5rc0/pybamm/models/submodels/convection/transverse/base_transverse_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/convection/transverse/full_convection.py` & `pybamm-23.5rc0/pybamm/models/submodels/convection/transverse/full_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/convection/transverse/no_convection.py` & `pybamm-23.5rc0/pybamm/models/submodels/convection/transverse/no_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/convection/transverse/uniform_convection.py` & `pybamm-23.5rc0/pybamm/models/submodels/convection/transverse/uniform_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/current_collector/base_current_collector.py` & `pybamm-23.5rc0/pybamm/models/submodels/current_collector/base_current_collector.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/current_collector/effective_resistance_current_collector.py` & `pybamm-23.5rc0/pybamm/models/submodels/current_collector/effective_resistance_current_collector.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/current_collector/homogeneous_current_collector.py` & `pybamm-23.5rc0/pybamm/models/submodels/current_collector/homogeneous_current_collector.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/current_collector/potential_pair.py` & `pybamm-23.5rc0/pybamm/models/submodels/current_collector/potential_pair.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/electrode/base_electrode.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrode/base_electrode.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/electrode/ohm/base_ohm.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/base_ohm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/electrode/ohm/composite_ohm.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/composite_ohm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/electrode/ohm/full_ohm.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/full_ohm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/electrode/ohm/leading_ohm.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/leading_ohm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/electrode/ohm/li_metal.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/li_metal.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/electrode/ohm/surface_form_ohm.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrode/ohm/surface_form_ohm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/base_electrolyte_conductivity.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/base_electrolyte_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/composite_conductivity.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/composite_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/full_conductivity.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/full_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/integrated_conductivity.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/integrated_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/leading_order_conductivity.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/leading_order_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/composite_surface_form_conductivity.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/composite_surface_form_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/explicit_surface_form_conductivity.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/explicit_surface_form_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/full_surface_form_conductivity.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/full_surface_form_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/leading_surface_form_conductivity.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/leading_surface_form_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/electrolyte_diffusion/base_electrolyte_diffusion.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_diffusion/base_electrolyte_diffusion.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/electrolyte_diffusion/constant_concentration.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_diffusion/constant_concentration.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/electrolyte_diffusion/full_diffusion.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_diffusion/full_diffusion.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/electrolyte_diffusion/leading_order_diffusion.py` & `pybamm-23.5rc0/pybamm/models/submodels/electrolyte_diffusion/leading_order_diffusion.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/equivalent_circuit_elements/ocv_element.py` & `pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/ocv_element.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/equivalent_circuit_elements/rc_element.py` & `pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/rc_element.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/equivalent_circuit_elements/resistor_element.py` & `pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/resistor_element.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/equivalent_circuit_elements/thermal.py` & `pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/thermal.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/equivalent_circuit_elements/voltage_model.py` & `pybamm-23.5rc0/pybamm/models/submodels/equivalent_circuit_elements/voltage_model.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/external_circuit/base_external_circuit.py` & `pybamm-23.5rc0/pybamm/models/submodels/external_circuit/base_external_circuit.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,57 +9,58 @@
 
     def __init__(self, param, options):
         super().__init__(param, options=options)
 
     def get_fundamental_variables(self):
         Q_Ah = pybamm.Variable("Discharge capacity [A.h]")
         Q_Ah.print_name = "Q_Ah"
-
-        variables = {"Discharge capacity [A.h]": Q_Ah}
+        # Throughput capacity (cumulative)
+        Qt_Ah = pybamm.Variable("Throughput capacity [A.h]")
+        Qt_Ah.print_name = "Qt_Ah"
+
+        variables = {
+            "Discharge capacity [A.h]": Q_Ah,
+            "Throughput capacity [A.h]": Qt_Ah,
+        }
         if self.options["calculate discharge energy"] == "true":
             Q_Wh = pybamm.Variable("Discharge energy [W.h]")
-
-            # Throughput capacity and energy (cumulative)
-            Qt_Ah = pybamm.Variable("Throughput capacity [A.h]")
+            # Throughput energy (cumulative)
             Qt_Wh = pybamm.Variable("Throughput energy [W.h]")
             variables.update(
                 {
                     "Discharge energy [W.h]": Q_Wh,
                     "Throughput energy [W.h]": Qt_Wh,
-                    "Throughput capacity [A.h]": Qt_Ah,
                 }
             )
         else:
             variables.update(
                 {
                     "Discharge energy [W.h]": pybamm.Scalar(0),
                     "Throughput energy [W.h]": pybamm.Scalar(0),
-                    "Throughput capacity [A.h]": pybamm.Scalar(0),
                 }
             )
         return variables
 
     def set_initial_conditions(self, variables):
         Q_Ah = variables["Discharge capacity [A.h]"]
+        Qt_Ah = variables["Throughput capacity [A.h]"]
         self.initial_conditions[Q_Ah] = pybamm.Scalar(0)
+        self.initial_conditions[Qt_Ah] = pybamm.Scalar(0)
         if self.options["calculate discharge energy"] == "true":
             Q_Wh = variables["Discharge energy [W.h]"]
             Qt_Wh = variables["Throughput energy [W.h]"]
-            Qt_Ah = variables["Throughput capacity [A.h]"]
             self.initial_conditions[Q_Wh] = pybamm.Scalar(0)
             self.initial_conditions[Qt_Wh] = pybamm.Scalar(0)
-            self.initial_conditions[Qt_Ah] = pybamm.Scalar(0)
 
     def set_rhs(self, variables):
         # ODEs for discharge capacity and throughput capacity
         Q_Ah = variables["Discharge capacity [A.h]"]
+        Qt_Ah = variables["Throughput capacity [A.h]"]
         I = variables["Current [A]"]
-
-        self.rhs[Q_Ah] = I / 3600
+        self.rhs[Q_Ah] = I / 3600  # Returns to zero after a complete cycle
+        self.rhs[Qt_Ah] = abs(I) / 3600  # Increases with each cycle
         if self.options["calculate discharge energy"] == "true":
             Q_Wh = variables["Discharge energy [W.h]"]
             Qt_Wh = variables["Throughput energy [W.h]"]
-            Qt_Ah = variables["Throughput capacity [A.h]"]
             V = variables["Voltage [V]"]
-            self.rhs[Q_Wh] = I * V / 3600
-            self.rhs[Qt_Wh] = abs(I * V) / 3600
-            self.rhs[Qt_Ah] = abs(I) / 3600
+            self.rhs[Q_Wh] = I * V / 3600  # Returns to zero after a complete cycle
+            self.rhs[Qt_Wh] = abs(I * V) / 3600  # Increases with each cycle
```

### Comparing `pybamm-23.4.1/pybamm/models/submodels/external_circuit/explicit_control_external_circuit.py` & `pybamm-23.5rc0/pybamm/models/submodels/external_circuit/explicit_control_external_circuit.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/external_circuit/function_control_external_circuit.py` & `pybamm-23.5rc0/pybamm/models/submodels/external_circuit/function_control_external_circuit.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/base_interface.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/base_interface.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/interface_utilisation/base_utilisation.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/interface_utilisation/base_utilisation.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/interface_utilisation/constant_utilisation.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/interface_utilisation/constant_utilisation.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/interface_utilisation/current_driven_utilisation.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/interface_utilisation/current_driven_utilisation.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/interface_utilisation/full_utilisation.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/interface_utilisation/full_utilisation.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/__init__.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/__init__.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/base_kinetics.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/base_kinetics.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/butler_volmer.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/butler_volmer.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/diffusion_limited.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/diffusion_limited.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/inverse_kinetics/inverse_butler_volmer.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/inverse_kinetics/inverse_butler_volmer.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/linear.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/linear.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/marcus.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/marcus.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/no_reaction.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/no_reaction.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/tafel.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/tafel.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/kinetics/total_main_kinetics.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/kinetics/total_main_kinetics.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/lithium_plating/base_plating.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/lithium_plating/base_plating.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/lithium_plating/no_plating.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/lithium_plating/no_plating.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/lithium_plating/plating.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/lithium_plating/plating.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/open_circuit_potential/base_ocp.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/open_circuit_potential/base_ocp.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/open_circuit_potential/current_sigmoid_ocp.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/open_circuit_potential/current_sigmoid_ocp.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/open_circuit_potential/single_ocp.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/open_circuit_potential/single_ocp.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             # Bulk OCP is from the average SOC and temperature
             sto_bulk = variables[f"{Domain} electrode {phase_name}stoichiometry"]
             T_bulk = pybamm.xyz_average(pybamm.size_average(T))
             ocp_bulk = self.phase_param.U(sto_bulk, T_bulk)
         elif self.reaction == "lithium metal plating":
             T = variables[f"{Domain} electrode temperature [K]"]
             ocp_surf = 0 * T
-            ocp_bulk = 0 * T
+            ocp_bulk = pybamm.Scalar(0)
             dUdT = 0 * T
         elif self.reaction == "lead-acid main":
             c_e = variables[f"{Domain} electrolyte concentration [mol.m-3]"]
             # If c_e was broadcast, take only the orphan
             if isinstance(c_e, pybamm.Broadcast):
                 c_e = c_e.orphans[0]
             ocp_surf = self.phase_param.U(c_e, self.param.T_init)
```

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/sei/base_sei.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/sei/base_sei.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/sei/constant_sei.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/sei/constant_sei.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/sei/no_sei.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/sei/no_sei.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/sei/sei_growth.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/sei/sei_growth.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/sei/total_sei.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/sei/total_sei.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/interface/total_interfacial_current.py` & `pybamm-23.5rc0/pybamm/models/submodels/interface/total_interfacial_current.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/oxygen_diffusion/base_oxygen_diffusion.py` & `pybamm-23.5rc0/pybamm/models/submodels/oxygen_diffusion/base_oxygen_diffusion.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/oxygen_diffusion/full_oxygen_diffusion.py` & `pybamm-23.5rc0/pybamm/models/submodels/oxygen_diffusion/full_oxygen_diffusion.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/oxygen_diffusion/leading_oxygen_diffusion.py` & `pybamm-23.5rc0/pybamm/models/submodels/oxygen_diffusion/leading_oxygen_diffusion.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/oxygen_diffusion/no_oxygen.py` & `pybamm-23.5rc0/pybamm/models/submodels/oxygen_diffusion/no_oxygen.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/particle/base_particle.py` & `pybamm-23.5rc0/pybamm/models/submodels/particle/base_particle.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/particle/fickian_diffusion.py` & `pybamm-23.5rc0/pybamm/models/submodels/particle/fickian_diffusion.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/particle/polynomial_profile.py` & `pybamm-23.5rc0/pybamm/models/submodels/particle/polynomial_profile.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/particle/total_particle_concentration.py` & `pybamm-23.5rc0/pybamm/models/submodels/particle/total_particle_concentration.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/particle/x_averaged_polynomial_profile.py` & `pybamm-23.5rc0/pybamm/models/submodels/particle/x_averaged_polynomial_profile.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/particle_mechanics/base_mechanics.py` & `pybamm-23.5rc0/pybamm/models/submodels/particle_mechanics/base_mechanics.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/particle_mechanics/crack_propagation.py` & `pybamm-23.5rc0/pybamm/models/submodels/particle_mechanics/crack_propagation.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/particle_mechanics/no_mechanics.py` & `pybamm-23.5rc0/pybamm/models/submodels/particle_mechanics/no_mechanics.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/particle_mechanics/swelling_only.py` & `pybamm-23.5rc0/pybamm/models/submodels/particle_mechanics/swelling_only.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/porosity/base_porosity.py` & `pybamm-23.5rc0/pybamm/models/submodels/porosity/base_porosity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/porosity/constant_porosity.py` & `pybamm-23.5rc0/pybamm/models/submodels/porosity/constant_porosity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/porosity/reaction_driven_porosity.py` & `pybamm-23.5rc0/pybamm/models/submodels/porosity/reaction_driven_porosity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/porosity/reaction_driven_porosity_ode.py` & `pybamm-23.5rc0/pybamm/models/submodels/porosity/reaction_driven_porosity_ode.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/thermal/base_thermal.py` & `pybamm-23.5rc0/pybamm/models/submodels/thermal/base_thermal.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/thermal/isothermal.py` & `pybamm-23.5rc0/pybamm/models/submodels/thermal/isothermal.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/thermal/lumped.py` & `pybamm-23.5rc0/pybamm/models/submodels/thermal/lumped.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_1D_current_collectors.py` & `pybamm-23.5rc0/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_1D_current_collectors.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_2D_current_collectors.py` & `pybamm-23.5rc0/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_2D_current_collectors.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/thermal/x_full.py` & `pybamm-23.5rc0/pybamm/models/submodels/thermal/x_full.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/transport_efficiency/base_transport_efficiency.py` & `pybamm-23.5rc0/pybamm/models/submodels/transport_efficiency/base_transport_efficiency.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/models/submodels/transport_efficiency/bruggeman_transport_efficiency.py` & `pybamm-23.5rc0/pybamm/models/submodels/transport_efficiency/bruggeman_transport_efficiency.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/parameters/base_parameters.py` & `pybamm-23.5rc0/pybamm/parameters/base_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/parameters/bpx.py` & `pybamm-23.5rc0/pybamm/parameters/bpx.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from bpx import BPX, Function, InterpolatedTable
 import pybamm
 import math
 from dataclasses import dataclass
 import numpy as np
 from pybamm import constants
 from pybamm import exp
-import copy
 
 
 import types
 import functools
 
 
 def _copy_func(f):
@@ -40,14 +39,26 @@
     short_pre_name="Negative ",
 )
 positive_electrode = Domain(
     name="positive electrode",
     pre_name="Positive electrode ",
     short_pre_name="Positive ",
 )
+positive_current_collector = Domain(
+    name="positive current collector",
+    pre_name="Positive current collector ",
+    short_pre_name="",
+)
+
+negative_current_collector = Domain(
+    name="negative current collector",
+    pre_name="Negative current collector ",
+    short_pre_name="",
+)
+
 electrolyte = Domain(name="electrolyte", pre_name="Electrolyte ", short_pre_name="")
 separator = Domain(name="separator", pre_name="Separator ", short_pre_name="")
 experiment = Domain(name="experiment", pre_name="", short_pre_name="")
 
 
 def _bpx_to_param_dict(bpx: BPX) -> dict:
     pybamm_dict = {}
@@ -110,19 +121,49 @@
 
     # lumped parameters
     for name in [
         "Specific heat capacity [J.K-1.kg-1]",
         "Density [kg.m-3]",
         "Thermal conductivity [W.m-1.K-1]",
     ]:
-        for domain in [negative_electrode, positive_electrode, separator]:
+        for domain in [
+            negative_electrode,
+            positive_electrode,
+            separator,
+            negative_current_collector,
+            positive_current_collector,
+        ]:
             pybamm_name = domain.pre_name + name[:1].lower() + name[1:]
             if name in pybamm_dict:
                 pybamm_dict[pybamm_name] = pybamm_dict[name]
 
+    # correct BPX specific heat capacity units to be consistent with pybamm
+    for domain in [
+        negative_electrode,
+        positive_electrode,
+        separator,
+        negative_current_collector,
+        positive_current_collector,
+    ]:
+        incorrect_name = domain.pre_name + "specific heat capacity [J.K-1.kg-1]"
+        new_name = domain.pre_name + "specific heat capacity [J.kg-1.K-1]"
+        if incorrect_name in pybamm_dict:
+            pybamm_dict[new_name] = pybamm_dict[incorrect_name]
+            del pybamm_dict[incorrect_name]
+
+    # lumped thermal model requires current collector parameters. Arbitrarily assign
+    for domain in [negative_current_collector, positive_current_collector]:
+        pybamm_dict[domain.pre_name + "thickness [m]"] = 0
+        pybamm_dict[domain.pre_name + "conductivity [S.m-1]"] = 4e7
+
+    # add a default heat transfer coefficient
+    pybamm_dict.update(
+        {"Total heat transfer coefficient [W.m-2.K-1]": 0}, check_already_exists=False
+    )
+
     # BET surface area
     for domain in [negative_electrode, positive_electrode]:
         pybamm_dict[domain.pre_name + "active material volume fraction"] = (
             pybamm_dict[domain.pre_name + "surface area per unit volume [m-1]"]
             * pybamm_dict[domain.short_pre_name + "particle radius [m]"]
         ) / 3.0
 
@@ -130,47 +171,81 @@
     for domain in [negative_electrode, separator, positive_electrode]:
         pybamm_dict[domain.pre_name + "porosity"] = pybamm_dict[
             domain.pre_name + "transport efficiency"
         ] ** (1.0 / 1.5)
 
     # TODO: allow setting function parameters in a loop over domains
 
+    # ocp
+
+    # negative electrode (only need to check for data, other cases pass through)
+    U_n = pybamm_dict[negative_electrode.pre_name + "OCP [V]"]
+    if isinstance(U_n, tuple):
+
+        def _negative_electrode_ocp(sto):
+            name, (x, y) = U_n
+            return pybamm.Interpolant(x, y, sto, name=name, interpolator="linear")
+
+        pybamm_dict[negative_electrode.pre_name + "OCP [V]"] = _negative_electrode_ocp
+
+    # positive electrode (only need to check for data, other cases pass through)
+    U_p = pybamm_dict[positive_electrode.pre_name + "OCP [V]"]
+    if isinstance(U_p, tuple):
+
+        def _positive_electrode_ocp(sto):
+            name, (x, y) = U_p
+            return pybamm.Interpolant(x, y, sto, name=name, interpolator="linear")
+
+        pybamm_dict[positive_electrode.pre_name + "OCP [V]"] = _positive_electrode_ocp
+
     # entropic change
 
     # negative electrode
-    U_n = pybamm_dict[
+    dUdT_n = pybamm_dict[
         negative_electrode.pre_name + "entropic change coefficient [V.K-1]"
     ]
-    if callable(U_n):
+    if callable(dUdT_n):
+
+        def _negative_electrode_entropic_change(sto, c_s_max):
+            return dUdT_n(sto)
+
+    elif isinstance(dUdT_n, tuple):
 
         def _negative_electrode_entropic_change(sto, c_s_max):
-            return U_n(sto)
+            name, (x, y) = dUdT_n
+            return pybamm.Interpolant(x, y, sto, name=name, interpolator="linear")
 
     else:
 
         def _negative_electrode_entropic_change(sto, c_s_max):
-            return U_n
+            return dUdT_n
 
     pybamm_dict[
         negative_electrode.pre_name + "OCP entropic change [V.K-1]"
     ] = _negative_electrode_entropic_change
 
     # positive electrode
-    U_p = pybamm_dict[
+    dUdT_p = pybamm_dict[
         positive_electrode.pre_name + "entropic change coefficient [V.K-1]"
     ]
-    if callable(U_p):
+    if callable(dUdT_p):
 
         def _positive_electrode_entropic_change(sto, c_s_max):
-            return U_p(sto)
+            return dUdT_p(sto)
+
+    elif isinstance(dUdT_p, tuple):
+
+        def _positive_electrode_entropic_change(sto, c_s_max):
+            name, (x, y) = dUdT_p
+            return pybamm.Interpolant(x, y, sto, name=name, interpolator="linear")
 
     else:
 
         def _positive_electrode_entropic_change(sto, c_s_max):
-            return U_p
+            return dUdT_p
 
     pybamm_dict[
         positive_electrode.pre_name + "OCP entropic change [V.K-1]"
     ] = _positive_electrode_entropic_change
 
     # reaction rates in pybamm exchange current is defined j0 = k * sqrt(ce * cs *
     # (cs-cs_max)) in BPX exchange current is defined j0 = F * k_norm * sqrt((ce/ce0) *
@@ -248,14 +323,23 @@
 
     if callable(D_n_ref):
 
         def _negative_electrode_diffusivity(sto, T):
             arrhenius = exp(E_a / constants.R * (1 / T_ref - 1 / T))
             return arrhenius * D_n_ref(sto)
 
+    elif isinstance(D_n_ref, tuple):
+
+        def _negative_electrode_diffusivity(sto, T):
+            arrhenius = exp(E_a / constants.R * (1 / T_ref - 1 / T))
+            name, (x, y) = D_n_ref
+            return arrhenius * pybamm.Interpolant(
+                x, y, sto, name=name, interpolator="linear"
+            )
+
     else:
 
         def _negative_electrode_diffusivity(sto, T):
             arrhenius = exp(E_a / constants.R * (1 / T_ref - 1 / T))
             return arrhenius * D_n_ref
 
     pybamm_dict[negative_electrode.pre_name + "diffusivity [m2.s-1]"] = _copy_func(
@@ -270,14 +354,23 @@
 
     if callable(D_p_ref):
 
         def _positive_electrode_diffusivity(sto, T):
             arrhenius = exp(E_a / constants.R * (1 / T_ref - 1 / T))
             return arrhenius * D_p_ref(sto)
 
+    elif isinstance(D_p_ref, tuple):
+
+        def _positive_electrode_diffusivity(sto, T):
+            arrhenius = exp(E_a / constants.R * (1 / T_ref - 1 / T))
+            name, (x, y) = D_p_ref
+            return arrhenius * pybamm.Interpolant(
+                x, y, sto, name=name, interpolator="linear"
+            )
+
     else:
 
         def _positive_electrode_diffusivity(sto, T):
             arrhenius = exp(E_a / constants.R * (1 / T_ref - 1 / T))
             return arrhenius * D_p_ref
 
     pybamm_dict[positive_electrode.pre_name + "diffusivity [m2.s-1]"] = _copy_func(
@@ -292,45 +385,59 @@
 
     if callable(D_e_ref):
 
         def _electrolyte_diffusivity(sto, T):
             arrhenius = exp(E_a / constants.R * (1 / T_ref - 1 / T))
             return arrhenius * D_e_ref(sto)
 
+    elif isinstance(D_e_ref, tuple):
+
+        def _electrolyte_diffusivity(sto, T):
+            arrhenius = exp(E_a / constants.R * (1 / T_ref - 1 / T))
+            name, (x, y) = D_e_ref
+            return arrhenius * pybamm.Interpolant(
+                x, y, sto, name=name, interpolator="linear"
+            )
+
     else:
 
         def _electrolyte_diffusivity(sto, T):
             arrhenius = exp(E_a / constants.R * (1 / T_ref - 1 / T))
             return arrhenius * D_e_ref
 
     pybamm_dict[electrolyte.pre_name + "diffusivity [m2.s-1]"] = _copy_func(
         _electrolyte_diffusivity
     )
 
     # conductivity
     E_a = pybamm_dict.get(
         electrolyte.pre_name + "conductivity activation energy [J.mol-1]", 0.0
     )
-    C_ref_value = pybamm_dict[electrolyte.pre_name + "conductivity [S.m-1]"]
+    C_e_ref = pybamm_dict[electrolyte.pre_name + "conductivity [S.m-1]"]
+
+    if callable(C_e_ref):
 
-    if callable(C_ref_value):
-        C_ref_fun = copy.copy(C_ref_value)
+        def _conductivity(c_e, T):
+            arrhenius = exp(E_a / constants.R * (1 / T_ref - 1 / T))
+            return arrhenius * C_e_ref(c_e)
+
+    elif isinstance(C_e_ref, tuple):
 
         def _conductivity(c_e, T):
-            C_ref = C_ref_fun(c_e)
             arrhenius = exp(E_a / constants.R * (1 / T_ref - 1 / T))
-            return arrhenius * C_ref
+            name, (x, y) = C_e_ref
+            return arrhenius * pybamm.Interpolant(
+                x, y, c_e, name=name, interpolator="linear"
+            )
 
     else:
-        C_ref_number = C_ref_value
 
         def _conductivity(c_e, T):
-            C_ref = C_ref_number
             arrhenius = exp(E_a / constants.R * (1 / T_ref - 1 / T))
-            return arrhenius * C_ref
+            return arrhenius * C_e_ref
 
     pybamm_dict[electrolyte.pre_name + "conductivity [S.m-1]"] = _copy_func(
         _conductivity
     )
 
     return pybamm_dict
 
@@ -342,20 +449,20 @@
     for name, field in instance.__fields__.items():
         value = getattr(instance, name)
         if value is None:
             continue
         elif isinstance(value, Function):
             value = value.to_python_function(preamble=preamble)
         elif isinstance(value, InterpolatedTable):
+            # return (name, (x, y)) to match the output of
+            # `pybamm.parameters.process_1D_data` we will create an interpolant on a
+            # case-by-case basis to get the correct argument for each parameter
             x = np.array(value.x)
             y = np.array(value.y)
-            interpolator = "linear"
-            value = pybamm.Interpolant(
-                [x], y, pybamm.t, name=name, interpolator=interpolator
-            )
+            value = (name, (x, y))
 
         pybamm_name = field.field_info.alias
         pybamm_name_lower = pybamm_name[:1].lower() + pybamm_name[1:]
         if pybamm_name.startswith("Initial concentration") or pybamm_name.startswith(
             "Maximum concentration"
         ):
             init_len = len("Initial concentration ")
```

### Comparing `pybamm-23.4.1/pybamm/parameters/ecm_parameters.py` & `pybamm-23.5rc0/pybamm/parameters/ecm_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/parameters/electrical_parameters.py` & `pybamm-23.5rc0/pybamm/parameters/electrical_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/parameters/geometric_parameters.py` & `pybamm-23.5rc0/pybamm/parameters/geometric_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/parameters/lead_acid_parameters.py` & `pybamm-23.5rc0/pybamm/parameters/lead_acid_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/parameters/lithium_ion_parameters.py` & `pybamm-23.5rc0/pybamm/parameters/lithium_ion_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/parameters/parameter_sets.py` & `pybamm-23.5rc0/pybamm/parameters/parameter_sets.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/parameters/parameter_values.py` & `pybamm-23.5rc0/pybamm/parameters/parameter_values.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 #
 # Parameter values for a simulation
 #
 import numpy as np
 import pybamm
-import pandas as pd
-import os
 import numbers
-import warnings
 from pprint import pformat
 from collections import defaultdict
-import inspect
-from textwrap import fill
-import shutil
 
 
 class ParameterValues:
     """
     The parameter values for a simulation.
 
     Note that this class does not inherit directly from the python dictionary class as
     this causes issues with saving and loading simulations.
 
     Parameters
     ----------
     values : dict or string
-        Explicit set of parameters, or reference to a file of parameters
+        Explicit set of parameters, or reference to an inbuilt parameter set
         If string and matches one of the inbuilt parameter sets, returns that parameter
-        set. If non-matching string, gets passed to read_parameters_csv to read a file.
+        set.
 
     Examples
     --------
     >>> import pybamm
     >>> values = {"some parameter": 1, "another parameter": 2}
     >>> param = pybamm.ParameterValues(values)
     >>> param["some parameter"]
@@ -56,52 +50,32 @@
                 "Ideal gas constant [J.K-1.mol-1]": pybamm.constants.R.value,
                 "Faraday constant [C.mol-1]": pybamm.constants.F.value,
                 "Boltzmann constant [J.K-1]": pybamm.constants.k_b.value,
                 "Electron charge [C]": pybamm.constants.q_e.value,
             }
         )
 
-        if isinstance(values, dict):
-            if "negative electrode" in values:
-                warnings.warn(
-                    "Creating a parameter set from a dictionary of components has "
-                    "been deprecated and will be removed in a future release. "
-                    "Define the parameter set in a python script instead.",
-                    DeprecationWarning,
-                )
-                self.update_from_chemistry(values)
-            else:
-                # Remove chemistry if present
-                values.pop("chemistry", None)
-                self.update(values, check_already_exists=False)
+        if isinstance(values, (dict, ParameterValues)):
+            # remove the "chemistry" key if it exists
+            values.pop("chemistry", None)
+            self.update(values, check_already_exists=False)
         else:
             # Check if values is a named parameter set
             if isinstance(values, str) and values in pybamm.parameter_sets:
                 values = pybamm.parameter_sets[values]
                 values.pop("chemistry", None)
                 self.update(values, check_already_exists=False)
 
-            else:
-                # In this case it might be a filename, load from that filename
-                file_path = self.find_parameter(values)
-                path = os.path.split(file_path)[0]
-                values = self.read_parameters_csv(file_path)
-                self.update(values, check_already_exists=False, path=path)
-
         # Initialise empty _processed_symbols dict (for caching)
         self._processed_symbols = {}
 
         # save citations
-        citations = []
-        if hasattr(self, "citations"):
-            citations = self.citations
-        elif "citations" in self._dict_items:
-            citations = self._dict_items["citations"]
-        for citation in citations:
-            pybamm.citations.register(citation)
+        if "citations" in self._dict_items:
+            for citation in self._dict_items["citations"]:
+                pybamm.citations.register(citation)
 
     @staticmethod
     def create_from_bpx(filename, target_soc=1):
         """
         Parameters
         ----------
         filename: str
@@ -163,103 +137,31 @@
         """Get the values of the dictionary"""
         return self._dict_items.values()
 
     def items(self):
         """Get the items of the dictionary"""
         return self._dict_items.items()
 
+    def pop(self, *args, **kwargs):
+        self._dict_items.pop(*args, **kwargs)
+
     def copy(self):
         """Returns a copy of the parameter values. Makes sure to copy the internal
         dictionary."""
         new_copy = ParameterValues(self._dict_items.copy())
         return new_copy
 
     def search(self, key, print_values=True):
         """
         Search dictionary for keys containing 'key'.
 
         See :meth:`pybamm.FuzzyDict.search()`.
         """
         return self._dict_items.search(key, print_values)
 
-    def update_from_chemistry(self, chemistry):
-        """
-        Load standard set of components from a 'chemistry' dictionary
-        """
-        self.chemistry = chemistry
-
-        base_chemistry = chemistry["chemistry"]
-
-        # Load each component name
-
-        component_groups = [
-            "cell",
-            "negative electrode",
-            "positive electrode",
-            "separator",
-            "electrolyte",
-            "experiment",
-        ]
-
-        self.component_params_by_group = {}
-
-        # add SEI parameters if provided
-        for extra_group in ["sei", "lithium plating"]:
-            if extra_group in chemistry:
-                component_groups = [extra_group] + component_groups
-
-        for component_group in component_groups:
-            component = chemistry[component_group]
-            # Create path to component and load values
-            component_path = os.path.join(
-                base_chemistry,
-                "testing_only",
-                component_group.replace(" ", "_") + "s",
-                component,
-            )
-            file_path = self.find_parameter(
-                os.path.join(component_path, "parameters.csv")
-            )
-            component_params = self.read_parameters_csv(file_path)
-
-            self.component_params_by_group[component_group] = component_params
-
-            # Update parameters, making sure to check any conflicts
-            self.update(
-                component_params,
-                check_conflict=True,
-                check_already_exists=False,
-                path=os.path.dirname(file_path),
-            )
-
-        # register (list of) citations
-        if "citation" in chemistry:
-            self.citations = chemistry["citation"]
-            if not isinstance(self.citations, list):
-                self.citations = [self.citations]
-
-    def read_parameters_csv(self, filename):
-        """Reads parameters from csv file into dict.
-
-        Parameters
-        ----------
-        filename : str
-            The name of the csv file containing the parameters.
-
-        Returns
-        -------
-        dict
-            {name: value} pairs for the parameters.
-
-        """
-        df = pd.read_csv(filename, comment="#", skip_blank_lines=True)
-        # Drop rows that are all NaN (seems to not work with skip_blank_lines)
-        df.dropna(how="all", inplace=True)
-        return {k: v for (k, v) in zip(df["Name [units]"], df["Value"])}
-
     def update(self, values, check_conflict=False, check_already_exists=True, path=""):
         """
         Update parameter dictionary, while also performing some basic checks.
 
         Parameters
         ----------
         values : dict
@@ -302,37 +204,29 @@
                 except KeyError as err:
                     raise KeyError(
                         "Cannot update parameter '{}' as it does not ".format(name)
                         + "have a default value. ({}). If you are ".format(err.args[0])
                         + "sure you want to update this parameter, use "
                         + "param.update({{name: value}}, check_already_exists=False)"
                     )
-            # if no conflicts, update, loading functions and data if they are specified
-            # Functions are flagged with the string "[function]"
+            # if no conflicts, update
             if isinstance(value, str):
-                if value.startswith("[function]"):
-                    loaded_value = pybamm.load_function(os.path.join(path, value[10:]))
-                    self._dict_items[name] = loaded_value
-                # Data is flagged with the string "[data]" or "[current data]"
-                elif value.startswith("[current data]") or value.startswith("[data]"):
-                    if value.startswith("[current data]"):
-                        data_path = os.path.join(
-                            pybamm.root_dir(), "pybamm", "input", "drive_cycles"
-                        )
-                        filename = os.path.join(data_path, value[14:] + ".csv")
-                    else:
-                        filename = os.path.join(path, value[6:] + ".csv")
-                    filename = pybamm.get_parameters_filepath(filename)
-                    # Save name and data
-                    self._dict_items[name] = pybamm.parameters.process_1D_data(filename)
-                # parse 2D parameter data
-                elif value.startswith("[2D data]"):
-                    filename = os.path.join(path, value[9:] + ".json")
-                    filename = pybamm.get_parameters_filepath(filename)
-                    self._dict_items[name] = pybamm.parameters.process_2D_data(filename)
+                if (
+                    value.startswith("[function]")
+                    or value.startswith("[current data]")
+                    or value.startswith("[data]")
+                    or value.startswith("[2D data]")
+                ):
+                    raise ValueError(
+                        "Specifying parameters via [function], [current data], [data] "
+                        "or [2D data] is no longer supported. For functions, pass in a "
+                        "python function object. For data, pass in a python function "
+                        "that returns a pybamm Interpolant object. "
+                        "See https://tinyurl.com/merv43ss for an example with both."
+                    )
 
                 elif value == "[input]":
                     self._dict_items[name] = pybamm.InputParameter(name)
                 # Anything else should be a converted to a float
                 else:
                     self._dict_items[name] = float(value)
             elif isinstance(value, tuple) and isinstance(value[1], np.ndarray):
@@ -784,29 +678,14 @@
             return processed_symbol.evaluate()
         else:
             raise ValueError("symbol must evaluate to a constant scalar or array")
 
     def _ipython_key_completions_(self):
         return list(self._dict_items.keys())
 
-    def export_csv(self, filename):
-        # process functions and data to output
-        # like they appear in inputs csv files
-        parameter_output = {}
-        for key, val in self.items():
-            if callable(val):
-                val = "[function]" + val.__name__
-            elif isinstance(val, tuple):
-                val = "[data]" + val[0]
-            parameter_output[key] = [val]
-
-        df = pd.DataFrame(parameter_output)
-        df = df.transpose()
-        df.to_csv(filename, header=["Value"], index_label="Name [units]")
-
     def print_parameters(self, parameters, output_file=None):
         """
         Return dictionary of evaluated parameters, and optionally print these evaluated
         parameters to an output file.
 
         Parameters
         ----------
@@ -919,194 +798,7 @@
         s = "{{:>{}}}".format(column_width)
         with open(output_file, "w") as file:
             for name, value in sorted(evaluated_parameters.items()):
                 if 0.001 < abs(value) < 1000:
                     file.write((s + " : {:10.4g}\n").format(name, value))
                 else:
                     file.write((s + " : {:10.3E}\n").format(name, value))
-
-    @staticmethod
-    def find_parameter(path):
-        """Look for parameter file in the different locations
-        in PARAMETER_PATH
-        """
-        # Check for absolute path
-        if os.path.isfile(path) and os.path.isabs(path):
-            pybamm.logger.verbose(f"Using absolute path: '{path}'")
-            return path
-        for location in pybamm.PARAMETER_PATH:
-            trial_path = os.path.join(location, path)
-            if os.path.isfile(trial_path):
-                pybamm.logger.verbose(f"Using path: '{location}' + '{path}'")
-                return trial_path
-        raise FileNotFoundError(
-            f"Could not find parameter {path}. If you have a developer install, try "
-            "re-installing pybamm (e.g. `pip install -e .`) to expose recently-added "
-            "parameter entry points."
-        )
-
-    def export_python_script(
-        self, name, old_parameters_path="", new_parameters_path=""
-    ):
-        """
-        Print a python script that can be used to reproduce the parameter set
-
-        Parameters
-        ----------
-        name : string
-            The name to save the parameter set under
-        old_parameters_path : string, optional
-            Optional path for the location where to find the old parameters.
-        new_parameters_path : string, optional
-            Optional path for the location where to save the new parameters.
-        """
-        # Initialize
-        preamble = "import pybamm\n"
-        function_output = ""
-        data_output = ""
-        dict_output = ""
-
-        component_params_by_group = getattr(
-            self, "component_params_by_group", {"": self}
-        )
-
-        # Loop through each component group and add appropriate functions, data, and
-        # parameters to the relevant strings
-        for component_group, items in component_params_by_group.items():
-            if component_group != "":
-                dict_output += f"\n        # {component_group}"
-            for k in items.keys():
-                v = self[k]
-                if callable(v):
-                    # write the function body to the file
-                    function_output += inspect.getsource(v) + "\n"
-                    v = v.__name__
-                elif isinstance(v, tuple):
-                    # save the data to a separate csv file
-                    # and load it in the parameter set
-                    data_name = v[0]
-                    data_file_old = os.path.join(
-                        old_parameters_path,
-                        component_group.replace(" ", "_") + "s",
-                        self.chemistry[component_group],
-                        f"{data_name}.csv",
-                    )
-                    data_path = os.path.join(new_parameters_path, "data")
-                    if not os.path.exists(data_path):
-                        os.makedirs(data_path)
-                    data_file_new = os.path.join(data_path, f"{data_name}.csv")
-                    shutil.copyfile(data_file_old, data_file_new)
-
-                    # add data output
-                    if data_output == "":
-                        data_output = (
-                            "# Load data in the appropriate format\n"
-                            "path, _ = os.path.split(os.path.abspath(__file__))\n"
-                        )
-                    data_output += (
-                        f"{data_name} = pybamm.parameters.process_1D_data"
-                        f"('{data_name}.csv', path)\n"
-                    )
-                    v = f"pybamm.{data_name}"
-
-                    v = f"{data_name}"
-
-                # add line to the parameter output in the appropriate section
-                line_output = f'\n        "{k}": {v},'
-                if len(line_output) > 88:
-                    # this will be split into multiple lines by black
-                    line_output = f'\n        "{k}""": {v},'
-
-                dict_output += line_output
-
-        # save citation info
-        if hasattr(self, "citations"):
-            dict_output += (
-                "\n        # citations" + f"\n        'citations': {self.citations},"
-            )
-
-        # read README.md if they exist and save info
-        docstring = self._create_docstring_from_readmes(name)
-
-        # construct the output string
-        output = (
-            function_output
-            + data_output
-            + "\n# Call dict via a function to avoid errors when editing in place"
-            + "\ndef get_parameter_values():"
-            + docstring
-            + "\n    return {"
-            + dict_output
-            + "\n    }"
-        )
-
-        # Add more packages to preamble if needed
-        if "os." in output:
-            preamble += "import os\n"
-        output = preamble + "\n\n" + output
-
-        # Add pybamm. to functions that didn't have it in function body before
-        for funcname in [
-            "Parameter",
-            "exp",
-            "tanh",
-            "cosh",
-            "log10",
-            "LeadAcidParameters",
-        ]:
-            # add space or ( before so it doesn't do this for middle-of-word matches
-            output = output.replace(f" {funcname}(", f" pybamm.{funcname}(")
-            output = output.replace(f"({funcname}(", f"(pybamm.{funcname}(")
-        output = output.replace("constants", "pybamm.constants")
-
-        # Process file name
-        filename = name
-        if not filename.endswith(".py"):
-            filename = filename + ".py"
-        filename = os.path.join(new_parameters_path, filename)
-
-        # save to file
-        with open(filename, "w") as f:
-            f.write(output)
-
-    def _create_docstring_from_readmes(self, name):
-        docstring = ""
-
-        if hasattr(self, "chemistry"):
-            chemistry = self.chemistry
-            lines = []
-            for component_group, component in chemistry.items():
-                if component_group in self.component_params_by_group:
-                    readme = os.path.join(
-                        "input",
-                        "parameters",
-                        self.chemistry["chemistry"],
-                        "testing_only",
-                        component_group.replace(" ", "_") + "s",
-                        component,
-                        "README.md",
-                    )
-                    readme = pybamm.get_parameters_filepath(readme)
-                    if os.path.isfile(readme):
-                        with open(readme, "r") as f:
-                            lines += f.readlines()
-
-            # lines, ind = np.unique(lines, return_index=True)
-            # lines = lines[np.argsort(ind)]
-            lines = [
-                fill(
-                    line,
-                    88,
-                    drop_whitespace=False,
-                    initial_indent="    ",
-                    subsequent_indent="    ",
-                )
-                + "\n"
-                for line in lines
-            ]
-            docstring = (
-                f'\n    """\n    # {name} parameter set\n'
-                + "".join(lines)
-                + '    """\n'
-            )
-
-        return docstring
```

### Comparing `pybamm-23.4.1/pybamm/parameters/process_parameter_data.py` & `pybamm-23.5rc0/pybamm/parameters/process_parameter_data.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/parameters/size_distribution_parameters.py` & `pybamm-23.5rc0/pybamm/parameters/size_distribution_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/parameters/thermal_parameters.py` & `pybamm-23.5rc0/pybamm/parameters/thermal_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/plotting/dynamic_plot.py` & `pybamm-23.5rc0/pybamm/plotting/dynamic_plot.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/plotting/plot.py` & `pybamm-23.5rc0/pybamm/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/plotting/plot2D.py` & `pybamm-23.5rc0/pybamm/plotting/plot2D.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/plotting/plot_summary_variables.py` & `pybamm-23.5rc0/pybamm/plotting/plot_summary_variables.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/plotting/plot_voltage_components.py` & `pybamm-23.5rc0/pybamm/plotting/plot_voltage_components.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/plotting/quick_plot.py` & `pybamm-23.5rc0/pybamm/plotting/quick_plot.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/settings.py` & `pybamm-23.5rc0/pybamm/settings.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/simulation.py` & `pybamm-23.5rc0/pybamm/simulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pickle
 import pybamm
 import numpy as np
 import copy
 import warnings
 import sys
 from functools import lru_cache
+from datetime import timedelta
 import tqdm
 
 
 def is_notebook():
     try:
         shell = get_ipython().__class__.__name__
         if shell == "ZMQInteractiveShell":  # pragma: no cover
@@ -32,16 +33,19 @@
 class Simulation:
     """A Simulation class for easy building and running of PyBaMM simulations.
 
     Parameters
     ----------
     model : :class:`pybamm.BaseModel`
         The model to be simulated
-    experiment : :class:`pybamm.Experiment` (optional)
-        The experimental conditions under which to solve the model
+    experiment : :class:`pybamm.Experiment` or string or list (optional)
+        The experimental conditions under which to solve the model. If a string is
+        passed, the experiment is constructed as `pybamm.Experiment([experiment])`. If
+        a list is passed, the experiment is constructed as
+        `pybamm.Experiment(experiment)`.
     geometry: :class:`pybamm.Geometry` (optional)
         The geometry upon which to solve the model
     parameter_values: :class:`pybamm.ParameterValues` (optional)
         Parameters and their corresponding numerical values.
     submesh_types: dict (optional)
         A dictionary of the types of submesh to use on each subdomain
     var_pts: dict (optional)
@@ -91,16 +95,23 @@
                     self._parameter_values.update(
                         {
                             "Current function [A]": self.C_rate
                             * self._parameter_values["Nominal cell capacity [A.h]"]
                         }
                     )
         else:
-            if not isinstance(experiment, pybamm.Experiment):
-                raise TypeError("experiment must be a pybamm `Experiment` instance")
+            if isinstance(experiment, (str, pybamm.step._Step)):
+                experiment = pybamm.Experiment([experiment])
+            elif isinstance(experiment, list):
+                experiment = pybamm.Experiment(experiment)
+            elif not isinstance(experiment, pybamm.Experiment):
+                raise TypeError(
+                    "experiment must be a pybamm `Experiment` instance, a single "
+                    "experiment step, or a list of experiment steps"
+                )
 
             self.operating_mode = "with experiment"
             # Save the experiment
             self.experiment = experiment.copy()
 
         self._unprocessed_model = model
         self.model = model
@@ -154,250 +165,183 @@
         integrating the model successively with each group of inputs, one group at a
         time.
         This needs to be done here and not in the Experiment class because the nominal
         cell capacity (from the parameters) is used to convert C-rate to current.
         """
         # Update experiment using capacity
         capacity = self._parameter_values["Nominal cell capacity [A.h]"]
-        for op_conds in self.experiment.operating_conditions:
-            op_type = op_conds["type"]
-            if op_conds["dc_data"] is not None:
-                # If operating condition includes a drive cycle, define the interpolant
-                drive_cycle_interpolant = pybamm.Interpolant(
-                    op_conds["dc_data"][:, 0],
-                    op_conds["dc_data"][:, 1],
-                    pybamm.t - pybamm.InputParameter("start time"),
-                )
-                if op_type == "current":
-                    op_conds["Current input [A]"] = drive_cycle_interpolant
-                if op_type == "voltage":
-                    op_conds["Voltage input [V]"] = drive_cycle_interpolant
-                if op_type == "power":
-                    op_conds["Power input [W]"] = drive_cycle_interpolant
-            else:
-                if op_type == "C-rate":
-                    Crate = op_conds.pop("C-rate input [-]")
-                    op_conds["type"] = "current"
-                    op_conds["Current input [A]"] = Crate * capacity
-                elif op_type == "current":
-                    Crate = op_conds["Current input [A]"] / capacity
-
-            # Update events
-            events = op_conds.pop("events")
-            if events is not None:
-                event_type = events.pop("type")
-                if event_type == "C-rate":
+        for op_conds in self.experiment.operating_conditions_steps:
+            if op_conds.type == "C-rate":
+                op_conds.type = "current"
+                op_conds.value = op_conds.value * capacity
+
+            # Update terminations
+            termination = op_conds.termination
+            for term in termination:
+                term_type = term["type"]
+                if term_type == "C-rate":
+                    # Change type to current
+                    term["type"] = "current"
                     # Scale C-rate with capacity to obtain current
-                    events["Current input [A]"] = (
-                        events.pop("C-rate input [-]") * capacity
-                    )
-                # Update the dictionary of operating conditions, replacing
-                # "xxx input [unit]" with "xxx cut-off [unit]"
-                op_conds.update(
-                    {
-                        key.replace("input", "cut-off"): value
-                        for key, value in events.items()
-                    }
-                )
+                    term["value"] = term["value"] * capacity
 
             # Add time to the experiment times
-            dt = op_conds["time"]
+            dt = op_conds.duration
             if dt is None:
-                if op_conds["type"] in ["current", "CCCV"]:
-                    # Current control: max simulation time: 3 * max simulation time
-                    # based on C-rate
+                if op_conds.type == "current":
+                    # Current control: max simulation time: 3h / C-rate
+                    Crate = op_conds.value / capacity
                     dt = 3 / abs(Crate) * 3600  # seconds
-                    if op_conds["type"] == "CCCV":
-                        dt *= 5  # 5x longer for CCCV
                 else:
                     # max simulation time: 1 day
                     dt = 24 * 3600  # seconds
-            op_conds["time"] = dt
+                op_conds.duration = dt
 
         # Set up model for experiment
         self.set_up_and_parameterise_model_for_experiment()
 
     def set_up_and_parameterise_model_for_experiment(self):
         """
         Set up self.model to be able to run the experiment (new version).
         In this version, a new model is created for each step.
 
         This increases set-up time since several models to be processed, but
         reduces simulation time since the model formulation is efficient.
         """
-        self.op_type_to_model = {}
-        self.op_string_to_model = {}
-        for op_number, op in enumerate(self.experiment.operating_conditions):
-            # Create model for this operating condition type (current/voltage/power)
-            # if it has not already been seen before
-            if op["type"] not in self.op_type_to_model:
-                if op["type"] == "current":
-                    new_model, submodel = self.model, None
-                else:
-                    # Voltage or power control
-                    # Create a new model where the current density is now a variable
-                    # To do so, we replace all instances of the current density in the
-                    # model with a current density variable, which is obtained from the
-                    # FunctionControl submodel
-                    # check which kind of external circuit model we need (differential
-                    # or algebraic)
-                    if op["type"] == "voltage":
-                        submodel_class = pybamm.external_circuit.VoltageFunctionControl
-                    elif op["type"] == "power":
-                        submodel_class = pybamm.external_circuit.PowerFunctionControl
-                    elif op["type"] == "CCCV":
-                        submodel_class = pybamm.external_circuit.CCCVFunctionControl
-
-                    new_model = self.model.new_copy()
-                    # Build the new submodel and update the model with it
-                    submodel = submodel_class(new_model.param, new_model.options)
-                    variables = new_model.variables
-                    submodel.variables = submodel.get_fundamental_variables()
-                    variables.update(submodel.variables)
-                    submodel.variables.update(submodel.get_coupled_variables(variables))
-                    variables.update(submodel.variables)
-                    submodel.set_rhs(variables)
-                    submodel.set_algebraic(variables)
-                    submodel.set_initial_conditions(variables)
-                    new_model.rhs.update(submodel.rhs)
-                    new_model.algebraic.update(submodel.algebraic)
-                    new_model.initial_conditions.update(submodel.initial_conditions)
-
-                self.op_type_to_model[op["type"]] = (new_model, submodel)
-
-            if op["string"] not in self.op_string_to_model:
-                model, submodel = self.op_type_to_model[op["type"]]
-                # Create a new model for this operating condition, since we will update
-                # the events differently (based on parameter values and inputs) for
-                # different models of the same type (current/voltage/power)
-                new_model = model.new_copy()
-                self.update_new_model_events(new_model, op)
-                # Update parameter values
-                new_parameter_values = self.parameter_values.copy()
-                self._original_temperature = new_parameter_values[
-                    "Ambient temperature [K]"
-                ]
-                experiment_parameter_values = self.get_experiment_parameter_values(
-                    op, op_number
-                )
-                new_parameter_values.update(
-                    experiment_parameter_values, check_already_exists=False
-                )
+        self.experiment_unique_steps_to_model = {}
+        for op_number, op in enumerate(self.experiment.unique_steps):
+            new_model = self.model.new_copy()
+            new_parameter_values = self.parameter_values.copy()
+
+            if op.type != "current":
+                # Voltage or power control
+                # Create a new model where the current density is now a variable
+                # To do so, we replace all instances of the current density in the
+                # model with a current density variable, which is obtained from the
+                # FunctionControl submodel
+                # check which kind of external circuit model we need (differential
+                # or algebraic)
+                if op.type == "voltage":
+                    submodel_class = pybamm.external_circuit.VoltageFunctionControl
+                elif op.type == "power":
+                    submodel_class = pybamm.external_circuit.PowerFunctionControl
+
+                # Build the new submodel and update the model with it
+                submodel = submodel_class(new_model.param, new_model.options)
+                variables = new_model.variables
+                submodel.variables = submodel.get_fundamental_variables()
+                variables.update(submodel.variables)
+                submodel.variables.update(submodel.get_coupled_variables(variables))
+                variables.update(submodel.variables)
+                submodel.set_rhs(variables)
+                submodel.set_algebraic(variables)
+                submodel.set_initial_conditions(variables)
+                new_model.rhs.update(submodel.rhs)
+                new_model.algebraic.update(submodel.algebraic)
+                new_model.initial_conditions.update(submodel.initial_conditions)
+
                 # Set the "current function" to be the variable defined in the submodel
-                if submodel is not None:
-                    new_parameter_values["Current function [A]"] = submodel.variables[
-                        "Current [A]"
-                    ]
-                parameterised_model = new_parameter_values.process_model(
-                    new_model, inplace=False
-                )
-                self.op_string_to_model[op["string"]] = parameterised_model
+                new_parameter_values["Current function [A]"] = submodel.variables[
+                    "Current [A]"
+                ]
+            self.update_new_model_events(new_model, op)
+            # Update parameter values
+            self._original_temperature = new_parameter_values["Ambient temperature [K]"]
+            experiment_parameter_values = self.get_experiment_parameter_values(
+                op, op_number
+            )
+            new_parameter_values.update(
+                experiment_parameter_values, check_already_exists=False
+            )
+            parameterised_model = new_parameter_values.process_model(
+                new_model, inplace=False
+            )
+            self.experiment_unique_steps_to_model[repr(op)] = parameterised_model
+
+        # Set up rest model if experiment has start times
+        if self.experiment.initial_start_time:
+            new_model = self.model.new_copy()
+            # Update parameter values
+            new_parameter_values = self.parameter_values.copy()
+            self._original_temperature = new_parameter_values["Ambient temperature [K]"]
+            new_parameter_values.update(
+                {"Current function [A]": 0, "Ambient temperature [K]": "[input]"},
+                check_already_exists=False,
+            )
+            parameterised_model = new_parameter_values.process_model(
+                new_model, inplace=False
+            )
+            self.experiment_unique_steps_to_model[
+                "Rest for padding"
+            ] = parameterised_model
 
     def update_new_model_events(self, new_model, op):
-        if "Current cut-off [A]" in op:
-            if op["type"] == "CCCV":
-                # for the CCCV model we need to make sure that the current
-                # cut-off is only reached at the end of the CV phase
-                # Current is negative for a charge so this event will be
-                # negative until it is zero
-                # So we take away a large number times a heaviside switch
-                # for the CV phase to make sure that the event can only be
-                # hit during CV
-                new_model.events.append(
-                    pybamm.Event(
-                        "Current cut-off (CCCV) [A] [experiment]",
-                        -new_model.variables["Current [A]"]
-                        - abs(pybamm.InputParameter("Current cut-off [A]"))
-                        + 1e4
-                        * (
-                            new_model.variables["Battery voltage [V]"]
-                            < (pybamm.InputParameter("Voltage input [V]") - 1e-4)
-                        ),
-                    )
-                )
-            else:
+        for term in op.termination:
+            if term["type"] == "current":
                 new_model.events.append(
                     pybamm.Event(
                         "Current cut-off [A] [experiment]",
-                        abs(new_model.variables["Current [A]"])
-                        - pybamm.InputParameter("Current cut-off [A]"),
+                        abs(new_model.variables["Current [A]"]) - term["value"],
                     )
                 )
 
-        # add voltage events to the model
-        if "Voltage cut-off [V]" in op:
-            # The voltage event should be positive at the start of charge/
-            # discharge. We use the sign of the current or power input to
-            # figure out whether the voltage event is greater than the starting
-            # voltage (charge) or less (discharge) and set the sign of the
-            # event accordingly
-            if op["type"] == "power":
-                inp = op["Power input [W]"]
-            else:
-                inp = op["Current input [A]"]
-            sign = np.sign(inp)
-            if sign > 0:
-                name = "Discharge"
-            else:
-                name = "Charge"
-            if sign != 0:
-                # Event should be positive at initial conditions for both
-                # charge and discharge
-                new_model.events.append(
-                    pybamm.Event(
-                        f"{name} voltage cut-off [V] [experiment]",
-                        sign
-                        * (
-                            new_model.variables["Battery voltage [V]"]
-                            - pybamm.InputParameter("Voltage cut-off [V]")
-                        ),
+            # add voltage events to the model
+            if term["type"] == "voltage":
+                # The voltage event should be positive at the start of charge/
+                # discharge. We use the sign of the current or power input to
+                # figure out whether the voltage event is greater than the starting
+                # voltage (charge) or less (discharge) and set the sign of the
+                # event accordingly
+                if isinstance(op.value, pybamm.Interpolant):
+                    sign = np.sign(op.value.y[0])
+                else:
+                    sign = np.sign(op.value)
+                if sign > 0:
+                    name = "Discharge"
+                else:
+                    name = "Charge"
+                if sign != 0:
+                    # Event should be positive at initial conditions for both
+                    # charge and discharge
+                    new_model.events.append(
+                        pybamm.Event(
+                            f"{name} voltage cut-off [V] [experiment]",
+                            sign
+                            * (
+                                new_model.variables["Battery voltage [V]"]
+                                - term["value"]
+                            ),
+                        )
                     )
-                )
 
         # Keep the min and max voltages as safeguards but add some tolerances
         # so that they are not triggered before the voltage limits in the
         # experiment
         for i, event in enumerate(new_model.events):
             if event.name in ["Minimum voltage [V]", "Maximum voltage [V]"]:
                 new_model.events[i] = pybamm.Event(
                     event.name, event.expression + 1, event.event_type
                 )
 
     def get_experiment_parameter_values(self, op, op_number):
-        experiment_parameter_values = {}
-        if op["type"] == "current":
-            experiment_parameter_values.update(
-                {"Current function [A]": op["Current input [A]"]}
-            )
-        if op["type"] == "CCCV":
-            experiment_parameter_values.update(
-                {"CCCV current function [A]": op["Current input [A]"]}
-            )
-        if op["type"] in ["voltage", "CCCV"]:
-            experiment_parameter_values.update(
-                {"Voltage function [V]": op["Voltage input [V]"]}
-            )
-        if op["type"] == "power":
-            experiment_parameter_values.update(
-                {"Power function [W]": op["Power input [W]"]}
-            )
+        experiment_parameter_values = {
+            f"{op.type.capitalize()} function {op.unit}": op.value
+        }
 
-        if op["temperature"] is not None:
-            ambient_temperature = op["temperature"] + 273.15
+        if op.temperature is not None:
+            ambient_temperature = op.temperature
             experiment_parameter_values.update(
                 {"Ambient temperature [K]": ambient_temperature}
             )
 
             # If at the first operation, then the intial temperature
             # should be the ambient temperature.
             if op_number == 0:
                 experiment_parameter_values.update(
-                    {
-                        "Initial temperature [K]": ambient_temperature,
-                    }
+                    {"Initial temperature [K]": ambient_temperature}
                 )
         else:
             experiment_parameter_values.update(
                 {"Ambient temperature [K]": self._original_temperature}
             )
 
         return experiment_parameter_values
@@ -487,15 +431,18 @@
             self._parameter_values.process_geometry(self._geometry)
             # Only needs to set up mesh and discretisation once
             self._mesh = pybamm.Mesh(self._geometry, self._submesh_types, self._var_pts)
             self._disc = pybamm.Discretisation(self._mesh, self._spatial_methods)
             # Process all the different models
             self.op_conds_to_built_models = {}
             self.op_conds_to_built_solvers = {}
-            for op_cond, model_with_set_params in self.op_string_to_model.items():
+            for (
+                op_cond,
+                model_with_set_params,
+            ) in self.experiment_unique_steps_to_model.items():
                 # It's ok to modify the model with set parameters in place as it's
                 # not returned anywhere
                 built_model = self._disc.process_model(
                     model_with_set_params, inplace=True, check_model=check_model
                 )
                 solver = self.solver.copy()
                 self.op_conds_to_built_solvers[op_cond] = solver
@@ -738,32 +685,46 @@
                         isinstance(save_at_cycles, int)
                         and (cycle_num + cycle_offset) % save_at_cycles == 0
                     )
                 )
                 for step_num in range(1, cycle_length + 1):
                     # Use 1-indexing for printing cycle number as it is more
                     # human-intuitive
-                    op_conds = self.experiment.operating_conditions[idx]
-                    dt = op_conds["time"]
-                    op_conds_str = op_conds["string"]
-                    model = self.op_conds_to_built_models[op_conds_str]
-                    solver = self.op_conds_to_built_solvers[op_conds_str]
+                    op_conds = self.experiment.operating_conditions_steps[idx]
+
+                    start_time = current_solution.t[-1]
+
+                    # If step has an end time, dt must take that into account
+                    if op_conds.end_time:
+                        dt = min(
+                            op_conds.duration,
+                            (
+                                op_conds.end_time
+                                - (
+                                    self.experiment.initial_start_time
+                                    + timedelta(seconds=float(start_time))
+                                )
+                            ).total_seconds(),
+                        )
+                    else:
+                        dt = op_conds.duration
+                    op_conds_str = str(op_conds)
+                    model = self.op_conds_to_built_models[repr(op_conds)]
+                    solver = self.op_conds_to_built_solvers[repr(op_conds)]
 
                     logs["step number"] = (step_num, cycle_length)
                     logs["step operating conditions"] = op_conds_str
                     callbacks.on_step_start(logs)
 
-                    start_time = current_solution.t[-1]
                     kwargs["inputs"] = {
                         **user_inputs,
-                        **op_conds,
                         "start time": start_time,
                     }
                     # Make sure we take at least 2 timesteps
-                    npts = max(int(round(dt / op_conds["period"])) + 1, 2)
+                    npts = max(int(round(dt / op_conds.period)) + 1, 2)
                     try:
                         step_solution = solver.step(
                             current_solution,
                             model,
                             dt,
                             npts=npts,
                             save=False,
@@ -783,27 +744,72 @@
                             feasible = False
                             # If none of the cycles worked, raise an error
                             if cycle_num == 1 and step_num == 1:
                                 raise error
                             # Otherwise, just stop this cycle
                             break
 
+                    step_termination = step_solution.termination
+
+                    # Add a padding rest step if necessary
+                    if op_conds.next_start_time is not None:
+                        rest_time = (
+                            op_conds.next_start_time
+                            - (
+                                self.experiment.initial_start_time
+                                + timedelta(seconds=float(step_solution.t[-1]))
+                            )
+                        ).total_seconds()
+                        if rest_time > pybamm.settings.step_start_offset:
+                            start_time = step_solution.t[-1]
+                            # Let me know if you have a better name
+                            op_conds_str = "Rest for padding"
+                            model = self.op_conds_to_built_models[op_conds_str]
+                            solver = self.op_conds_to_built_solvers[op_conds_str]
+
+                            logs["step number"] = (step_num, cycle_length)
+                            logs["step operating conditions"] = op_conds_str
+                            callbacks.on_step_start(logs)
+
+                            ambient_temp = (
+                                op_conds.temperature or self._original_temperature
+                            )
+                            kwargs["inputs"] = {
+                                **user_inputs,
+                                "Ambient temperature [K]": ambient_temp,
+                                "start time": start_time,
+                            }
+                            # Make sure we take at least 2 timesteps
+                            # The period is hardcoded to 10 minutes, the user can
+                            # always override it by adding a rest step
+                            npts = max(int(round(rest_time / 600)) + 1, 2)
+
+                            step_solution_with_rest = solver.step(
+                                step_solution,
+                                model,
+                                rest_time,
+                                npts=npts,
+                                save=False,
+                                **kwargs,
+                            )
+                            step_solution += step_solution_with_rest
+
                     steps.append(step_solution)
 
                     cycle_solution = cycle_solution + step_solution
                     current_solution = cycle_solution
 
                     callbacks.on_step_end(logs)
 
                     logs["termination"] = step_solution.termination
                     # Only allow events specified by experiment
                     if not (
                         isinstance(step_solution, pybamm.EmptySolution)
-                        or step_solution.termination == "final time"
-                        or "[experiment]" in step_solution.termination
+                        or step_termination == "final time"
+                        or "[experiment]" in step_termination
                     ):
                         callbacks.on_experiment_infeasible(logs)
                         feasible = False
                         break
 
                     # Increment index for next iteration
                     idx += 1
@@ -1088,14 +1094,23 @@
             )
         # Clear solver problem (not pickle-able, will automatically be recomputed)
         if (
             isinstance(self._solver, pybamm.CasadiSolver)
             and self._solver.integrator_specs != {}
         ):
             self._solver.integrator_specs = {}
+
+        if self.op_conds_to_built_solvers is not None:
+            for solver in self.op_conds_to_built_solvers.values():
+                if (
+                    isinstance(solver, pybamm.CasadiSolver)
+                    and solver.integrator_specs != {}
+                ):
+                    solver.integrator_specs = {}
+
         with open(filename, "wb") as f:
             pickle.dump(self, f, pickle.HIGHEST_PROTOCOL)
 
 
 def load_sim(filename):
     """Load a saved simulation"""
     return pybamm.load(filename)
```

### Comparing `pybamm-23.4.1/pybamm/solvers/algebraic_solver.py` & `pybamm-23.5rc0/pybamm/solvers/algebraic_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/solvers/base_solver.py` & `pybamm-23.5rc0/pybamm/solvers/base_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,33 +126,50 @@
         )
 
         vars_for_processing = self._get_vars_for_processing(
             model, inputs, calculate_sensitivities_explicit
         )
 
         # Process initial conditions
-        initial_conditions = process(
+        initial_conditions, _, jacp_ic, _ = process(
             model.concatenated_initial_conditions,
             "initial_conditions",
             vars_for_processing,
             use_jacobian=False,
-        )[0]
+        )
         model.initial_conditions_eval = initial_conditions
+        model.jacp_initial_conditions_eval = jacp_ic
 
         # evaluate initial condition
         y0_total_size = (
             model.len_rhs + model.len_rhs_sens + model.len_alg + model.len_alg_sens
         )
         y_zero = np.zeros((y0_total_size, 1))
         if model.convert_to_format == "casadi":
             # stack inputs
             inputs_casadi = casadi.vertcat(*[x for x in inputs.values()])
-            model.y0 = initial_conditions(0, y_zero, inputs_casadi)
+            model.y0 = initial_conditions(0.0, y_zero, inputs_casadi)
+            if jacp_ic is None:
+                model.y0S = None
+            else:
+                model.y0S = jacp_ic(0.0, y_zero, inputs_casadi)
         else:
-            model.y0 = initial_conditions(0, y_zero, inputs)
+            model.y0 = initial_conditions(0.0, y_zero, inputs)
+            if jacp_ic is None:
+                model.y0S = None
+            else:
+                # we are calculating the derivative wrt the inputs
+                # so need to make sure we convert int -> float
+                # This is to satisfy JAX jacfwd function which requires
+                # float inputs
+                inputs_float = {
+                    key: float(value) if isinstance(value, int) else value
+                    for key, value in inputs.items()
+                }
+                model.y0S = jacp_ic(0.0, y_zero, inputs_float)
 
         if ics_only:
             pybamm.logger.info("Finish solver set-up")
             return
 
         # Process rhs, algebraic, residual and event expressions
         # and wrap in callables
```

### Comparing `pybamm-23.4.1/pybamm/solvers/casadi_algebraic_solver.py` & `pybamm-23.5rc0/pybamm/solvers/casadi_algebraic_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/solvers/casadi_solver.py` & `pybamm-23.5rc0/pybamm/solvers/casadi_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,22 +257,23 @@
                             extract_sensitivities_in_solution=False,
                         )
                         first_ts_solved = True
                         solved = True
                     except pybamm.SolverError as error:
                         pybamm.logger.debug("Failed, halving step size")
                         dt /= 2
+                        count += 1
                         # also reduce maximum step size for future global steps,
                         # but skip them in the beginning
                         # sometimes, for the first integrator smaller timesteps are
                         # needed, but this won't affect the global timesteps. The
                         # global timestep will only be reduced after the first timestep.
                         if first_ts_solved:
                             dt_max = dt
-                        if count >= self.max_step_decrease_count:
+                        if count > self.max_step_decrease_count:
                             message = (
                                 "Maximum number of decreased steps occurred at "
                                 f"t={t} (final SolverError: '{error}'). "
                                 "For a full solution try reducing dt_max (currently, "
                                 f"dt_max={dt_max}) and/or reducing the size of the "
                                 "time steps or period of the experiment."
                             )
@@ -283,15 +284,14 @@
                             else:
                                 raise pybamm.SolverError(
                                     message
                                     + " Set `return_solution_if_failed_early=True` to "
                                     "return the solution object up to the point where "
                                     "failure occured."
                                 )
-                    count += 1
                 if termination_due_to_small_dt:
                     break
                 # Check if the sign of an event changes, if so find an accurate
                 # termination point and exit
                 current_step_sol = self._solve_for_event(current_step_sol)
                 # assign temporary solve time
                 current_step_sol.solve_time = np.nan
```

### Comparing `pybamm-23.4.1/pybamm/solvers/dummy_solver.py` & `pybamm-23.5rc0/pybamm/solvers/dummy_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/solvers/idaklu_solver.py` & `pybamm-23.5rc0/pybamm/solvers/idaklu_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,17 @@
                 # for iterative linear solver preconditioner, bandwidth of
                 # approximate jacobian
                 "precon_half_bandwidth": 5,
 
                 # for iterative linear solver preconditioner, bandwidth of
                 # approximate jacobian that is kept
                 "precon_half_bandwidth_keep": 5
+
+                # Number of threads available for OpenMP
+                "num_threads": 1
             }
 
         Note: These options only have an effect if model.convert_to_format == 'casadi'
 
 
     """
 
@@ -96,14 +99,15 @@
             "print_stats": False,
             "jacobian": "sparse",
             "linear_solver": "SUNLinSol_KLU",
             "preconditioner": "BBDP",
             "linsol_max_iterations": 5,
             "precon_half_bandwidth": 5,
             "precon_half_bandwidth_keep": 5,
+            "num_threads": 1,
         }
         if options is None:
             options = default_options
         else:
             for key, value in default_options.items():
                 if key not in options:
                     options[key] = value
@@ -169,14 +173,25 @@
             return inputs_dict
 
         y0 = model.y0
         if isinstance(y0, casadi.DM):
             y0 = y0.full()
         y0 = y0.flatten()
 
+        y0S = model.y0S
+        # only casadi solver needs sensitivity ics
+        if model.convert_to_format != "casadi":
+            y0S = None
+        if y0S is not None:
+            if isinstance(y0S, casadi.DM):
+                y0S = (y0S,)
+
+            y0S = (x.full() for x in y0S)
+            y0S = [x.flatten() for x in y0S]
+
         if ics_only:
             return base_set_up_return
 
         if model.convert_to_format == "jax":
             mass_matrix = model.mass_matrix.entries.toarray()
         elif model.convert_to_format == "casadi":
             if self._options["jacobian"] == "dense":
@@ -476,31 +491,49 @@
 
         # do this here cause y0 is set after set_up (calc consistent conditions)
         y0 = model.y0
         if isinstance(y0, casadi.DM):
             y0 = y0.full()
         y0 = y0.flatten()
 
+        y0S = model.y0S
+        # only casadi solver needs sensitivity ics
+        if model.convert_to_format != "casadi":
+            y0S = None
+        if y0S is not None:
+            if isinstance(y0S, casadi.DM):
+                y0S = (y0S,)
+
+            y0S = (x.full() for x in y0S)
+            y0S = [x.flatten() for x in y0S]
+
         # solver works with ydot0 set to zero
         ydot0 = np.zeros_like(y0)
+        if y0S is not None:
+            ydot0S = [np.zeros_like(y0S_i) for y0S_i in y0S]
+            y0full = np.concatenate([y0, *y0S])
+            ydot0full = np.concatenate([ydot0, *ydot0S])
+        else:
+            y0full = y0
+            ydot0full = ydot0
 
         try:
             atol = model.atol
         except AttributeError:
             atol = self.atol
 
         rtol = self.rtol
         atol = self._check_atol_type(atol, y0.size)
 
         timer = pybamm.Timer()
         if model.convert_to_format == "casadi":
             sol = self._setup["solver"].solve(
                 t_eval,
-                y0,
-                ydot0,
+                y0full,
+                ydot0full,
                 inputs,
             )
         else:
             sol = idaklu.solve_python(
                 t_eval,
                 y0,
                 ydot0,
```

### Comparing `pybamm-23.4.1/pybamm/solvers/jax_bdf_solver.py` & `pybamm-23.5rc0/pybamm/solvers/jax_bdf_solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,37 +5,34 @@
 import numpy as onp
 
 import pybamm
 
 if pybamm.have_jax():
     import jax
     import jax.numpy as jnp
-    from absl import logging
     from jax import core, dtypes
     from jax import linear_util as lu
     from jax.api_util import flatten_fun_nokwargs
     from jax.config import config
     from jax.flatten_util import ravel_pytree
     from jax.interpreters import partial_eval as pe
-    from jax.tree_util import tree_flatten, tree_map, tree_multimap, tree_unflatten
+    from jax.tree_util import tree_flatten, tree_map, tree_unflatten
     from jax.util import cache, safe_map, split_list
 
     config.update("jax_enable_x64", True)
 
-    logging.set_verbosity(logging.ERROR)
-
     MAX_ORDER = 5
     NEWTON_MAXITER = 4
     ROOT_SOLVE_MAXITER = 15
     MIN_FACTOR = 0.2
     MAX_FACTOR = 10
 
     # https://github.com/google/jax/issues/4572#issuecomment-709809897
     def some_hash_function(x):
-        return hash(x.tobytes())
+        return hash(str(x))
 
     class HashableArrayWrapper:
         """wrapper for a numpy array to make it hashable"""
 
         def __init__(self, val):
             self.val = val
 
@@ -46,30 +43,30 @@
             return isinstance(other, HashableArrayWrapper) and onp.all(
                 onp.equal(self.val, other.val)
             )
 
     def gnool_jit(fun, static_array_argnums=(), static_argnums=()):
         """redefinition of jax jit to allow static array args"""
 
-        @partial(jax.jit, static_argnums=static_array_argnums + static_argnums)
+        @partial(jax.jit, static_argnums=static_array_argnums)
         def callee(*args):
             args = list(args)
             for i in static_array_argnums:
                 args[i] = args[i].val
             return fun(*args)
 
         def caller(*args):
             args = list(args)
             for i in static_array_argnums:
                 args[i] = HashableArrayWrapper(args[i])
             return callee(*args)
 
         return caller
 
-    @jax.partial(jax.custom_vjp, nondiff_argnums=(0, 1, 2, 3))
+    @partial(jax.custom_vjp, nondiff_argnums=(0, 1, 2, 3))
     def _bdf_odeint(fun, mass, rtol, atol, y0, t_eval, *args):
         """
         Implements a Backward Difference formula (BDF) implicit multistep integrator.
         The basic algorithm is derived in [2]_. This particular implementation follows
         that implemented in the Matlab routine ode15s described in [1]_ and the SciPy
         implementation [3]_, which features the NDF formulas for improved stability,
         with associated differences in the error constants, and calculates the jacobian
@@ -136,20 +133,21 @@
             _, t_eval, i, _ = state
             return i < len(t_eval)
 
         def body_fun(state):
             stepper, t_eval, i, y_out = state
             stepper = _bdf_step(stepper, fun_bind_inputs, jac_bind_inputs)
             index = jnp.searchsorted(t_eval, stepper.t)
+            index = index.astype(
+                "int" + t_eval.dtype.name[-2:]
+            )  # Coerce index to correct type
 
             def for_body(j, y_out):
                 t = t_eval[j]
-                y_out = jax.ops.index_update(
-                    y_out, jax.ops.index[j, :], _bdf_interpolate(stepper, t)
-                )
+                y_out = y_out.at[jnp.index_exp[j, :]].set(_bdf_interpolate(stepper, t))
                 return y_out
 
             y_out = jax.lax.fori_loop(i, index, for_body, y_out)
             return [stepper, t_eval, index, y_out]
 
         stepper, t_eval, i, y_out = jax.lax.while_loop(cond_fun, body_fun, init_state)
         return y_out
@@ -238,16 +236,16 @@
 
         f0 = fun(y0, t0)
         order = 1
         state["order"] = order
         state["h"] = _select_initial_step(atol, rtol, fun, t0, y0, f0, h0)
         state["n_equal_steps"] = 0
         D = jnp.empty((MAX_ORDER + 1, len(y0)), dtype=y0.dtype)
-        D = jax.ops.index_update(D, jax.ops.index[0, :], y0)
-        D = jax.ops.index_update(D, jax.ops.index[1, :], f0 * state["h"])
+        D = D.at[jnp.index_exp[0, :]].set(y0)
+        D = D.at[jnp.index_exp[1, :]].set(f0 * state["h"])
         state["D"] = D
         state["y0"] = y0
         state["scale_y0"] = scale_y0
 
         # kappa values for difference orders, taken from Table 1 of [1]
         kappa = jnp.array([0, -0.1850, -1 / 9, -0.0823, -0.0415, 0])
         gamma = jnp.hstack((0, jnp.cumsum(1 / jnp.arange(1, MAX_ORDER + 1))))
@@ -289,16 +287,16 @@
 
         Note that the U matrix also defined in the same section can be also be
         found using factor = 1, which corresponds to R with a constant step size
         """
         I = jnp.arange(1, MAX_ORDER + 1).reshape(-1, 1)
         J = jnp.arange(1, MAX_ORDER + 1)
         M = jnp.empty((MAX_ORDER + 1, MAX_ORDER + 1))
-        M = jax.ops.index_update(M, jax.ops.index[1:, 1:], (I - 1 - factor * J) / I)
-        M = jax.ops.index_update(M, jax.ops.index[0], 1)
+        M = M.at[jnp.index_exp[1:, 1:]].set((I - 1 - factor * J) / I)
+        M = M.at[jnp.index_exp[0]].set(1)
         R = jnp.cumprod(M, axis=0)
 
         return R
 
     def _select_initial_conditions(fun, M, t0, y0, tol, scale_y0):
         # identify algebraic variables as zeros on diagonal
         algebraic_variables = onp.diag(M) == 0.0
@@ -312,15 +310,15 @@
         # This follows this reference:
         #
         # Shampine, L. F., Reichelt, M. W., & Kierzenka, J. A. (1999).
         # Solving index-1 DAEs in MATLAB and Simulink. SIAM review, 41(3), 538-552.
 
         # calculate fun_a, function of algebraic variables
         def fun_a(y_a):
-            y_full = jax.ops.index_update(y0, algebraic_variables, y_a)
+            y_full = y0.at[algebraic_variables].set(y_a)
             return fun(y_full, t0)[algebraic_variables]
 
         y0_a = y0[algebraic_variables]
         scale_y0_a = scale_y0[algebraic_variables]
 
         d = jnp.zeros(y0_a.shape[0], dtype=y0.dtype)
         y_a = jnp.array(y0_a, copy=True)
@@ -356,15 +354,15 @@
             dy_norm_old = dy_norm
 
             return [k + 1, converged, dy_norm_old, d, y_a]
 
         k, converged, dy_norm_old, d, y_a = jax.lax.while_loop(
             while_cond, while_body, while_state
         )
-        y_tilde = jax.ops.index_update(y0, algebraic_variables, y_a)
+        y_tilde = y0.at[algebraic_variables].set(y_a)
 
         return y_tilde, converged
 
     def _select_initial_step(atol, rtol, fun, t0, y0, f0, h0):
         """
         Select a good initial step by stepping forward one step of forward euler, and
         comparing the predicted state against that using the provided function.
@@ -421,26 +419,26 @@
         Standard backwards difference gives
         D^{j + 1} y_n = D^{j} y_n - D^{j} y_{n - 1}
 
         Combining these gives the following algorithm
         """
         order = state.order
         D = state.D
-        D = jax.ops.index_update(D, jax.ops.index[order + 2], d - D[order + 1])
-        D = jax.ops.index_update(D, jax.ops.index[order + 1], d)
+        D = D.at[jnp.index_exp[order + 2]].set(d - D[order + 1])
+        D = D.at[jnp.index_exp[order + 1]].set(d)
         i = order
         while_state = [i, D]
 
         def while_cond(while_state):
             i, _ = while_state
             return i >= 0
 
         def while_body(while_state):
             i, D = while_state
-            D = jax.ops.index_add(D, jax.ops.index[i], D[i + 1])
+            D = D.at[jnp.index_exp[i]].add(D[i + 1])
             i -= 1
             return [i, D]
 
         i, D = jax.lax.while_loop(while_cond, while_body, while_state)
 
         return D
 
@@ -639,28 +637,28 @@
 
             # solve BDF equation using y0 as starting point
             converged, n_iter, y, d, state = _newton_iteration(state, fun)
             not_converged = converged == False  # noqa: E712
 
             # newton iteration did not converge, but jacobian has already been
             # evaluated so reduce step size by 0.3 (as per [1]) and try again
-            state = tree_multimap(
+            state = tree_map(
                 partial(jnp.where, not_converged * updated_jacobian),
                 _update_step_size_and_lu(state, 0.3),
                 state,
             )
 
             # if not_converged * updated_jacobian:
             #    print('not converged, update step size by 0.3')
             # if not_converged * (updated_jacobian == False):
             #    print('not converged, update jacobian')
 
             # if not converged and jacobian not updated, then update the jacobian and
             # try again
-            (state, updated_jacobian) = tree_multimap(
+            (state, updated_jacobian) = tree_map(
                 partial(
                     jnp.where, not_converged * (updated_jacobian == False)  # noqa: E712
                 ),
                 (_update_jacobian(state, jac), True),
                 (state, False + updated_jacobian),
             )
 
@@ -684,15 +682,15 @@
             #         "converged, but error is too large",
             #         error_norm,
             #         factor,
             #         d,
             #         scale_y,
             #     )
 
-            (state, step_accepted) = tree_multimap(
+            (state, step_accepted) = tree_map(
                 partial(jnp.where, converged * (error_norm > 1)),  # noqa: E712
                 (_update_step_size_and_lu(state, factor), False),
                 (state, converged),
             )
 
             return [state, step_accepted, updated_jacobian, y, d, n_iter]
 
@@ -706,15 +704,15 @@
 
         # a change in order is only done after running at order k for k + 1 steps
         # (see page 83 of [2])
         n_equal_steps = state.n_equal_steps + 1
 
         state = state._replace(n_equal_steps=n_equal_steps, t=t, n_steps=n_steps)
 
-        state = tree_multimap(
+        state = tree_map(
             partial(jnp.where, n_equal_steps < state.order + 1),
             _prepare_next_step(state, d),
             _prepare_next_step_order_change(state, d, y, n_iter),
         )
 
         return state
 
@@ -815,15 +813,15 @@
         carry = init
         ys = []
         for x in xs:
             carry, y = f(carry, x)
             ys.append(y)
         return carry, onp.stack(ys)
 
-    @jax.partial(gnool_jit, static_array_argnums=(1,), static_argnums=(0, 2, 3))
+    @partial(gnool_jit, static_array_argnums=(0, 1, 2, 3))
     def _bdf_odeint_wrapper(func, mass, rtol, atol, y0, ts, *args):
         y0, unravel = ravel_pytree(y0)
         func = ravel_first_arg(func, unravel)
         out = _bdf_odeint(func, mass, rtol, atol, y0, ts, *args)
         return jax.vmap(unravel)(out)
 
     def _bdf_odeint_fwd(func, mass, rtol, atol, y0, ts, *args):
@@ -872,18 +870,16 @@
 
                 # boolean arguments not implemented in jnp.ix_
                 J_aa = J[onp.ix_(algebraic_variables, algebraic_variables)]
                 J_ad = J[onp.ix_(algebraic_variables, differentiable_variables)]
                 LU = jax.scipy.linalg.lu_factor(J_aa)
                 g0_a = g0[algebraic_variables]
                 invJ_aa = jax.scipy.linalg.lu_solve(LU, g0_a)
-                y_bar = jax.ops.index_update(
-                    g0,
-                    differentiable_variables,
-                    jax.scipy.linalg.lu_solve(LU_invM_dd, g0_a - J_ad @ invJ_aa),
+                y_bar = g0.at[differentiable_variables].set(
+                    jax.scipy.linalg.lu_solve(LU_invM_dd, g0_a - J_ad @ invJ_aa)
                 )
             else:
                 y_bar = jax.scipy.linalg.lu_solve(LU_invM_dd, g0)
             return y_bar
 
         y_bar = initialise(g[-1], ys[-1], ts[-1])
         ts_bar = []
@@ -931,31 +927,23 @@
         ts_bar = jnp.concatenate([jnp.array([t0_bar]), rev_ts_bar[::-1]])
         return (y_bar, ts_bar, *args_bar)
 
     _bdf_odeint.defvjp(_bdf_odeint_fwd, _bdf_odeint_rev)
 
     @cache()
     def closure_convert(fun, in_tree, in_avals):
-        if config.omnistaging_enabled:
-            wrapped_fun, out_tree = flatten_fun_nokwargs(lu.wrap_init(fun), in_tree)
-            jaxpr, _, consts = pe.trace_to_jaxpr_dynamic(wrapped_fun, in_avals)
-        else:
-            in_pvals = [pe.PartialVal.unknown(aval) for aval in in_avals]
-            wrapped_fun, out_tree = flatten_fun_nokwargs(lu.wrap_init(fun), in_tree)
-            with core.initial_style_staging():  # type: ignore
-                jaxpr, _, consts = pe.trace_to_jaxpr(
-                    wrapped_fun, in_pvals, instantiate=True, stage_out=False
-                )  # type: ignore
+        wrapped_fun, out_tree = flatten_fun_nokwargs(lu.wrap_init(fun), in_tree)
+        jaxpr, _, consts = pe.trace_to_jaxpr_dynamic(wrapped_fun, in_avals)
         out_tree = out_tree()
 
         # We only want to closure convert for constants with respect to which we're
         # differentiating. As a proxy for that, we hoist consts with float dtype.
         # TODO(mattjj): revise this approach
         def is_float(c):
-            return dtypes.issubdtype(dtypes.dtype(c), jnp.inexact)
+            return dtypes.issubdtype(type(c), jnp.inexact)
 
         (closure_consts, hoisted_consts), merge = partition_list(is_float, consts)
         num_consts = len(hoisted_consts)
 
         def converted_fun(y, t, *hconsts_args):
             hoisted_consts, args = split_list(hconsts_args, [num_consts])
             consts = merge(closure_consts, hoisted_consts)
```

### Comparing `pybamm-23.4.1/pybamm/solvers/jax_solver.py` & `pybamm-23.5rc0/pybamm/solvers/jax_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/solvers/lrudict.py` & `pybamm-23.5rc0/pybamm/solvers/lrudict.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/solvers/processed_variable.py` & `pybamm-23.5rc0/pybamm/solvers/processed_variable.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/solvers/scikits_dae_solver.py` & `pybamm-23.5rc0/pybamm/solvers/scikits_dae_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/solvers/scikits_ode_solver.py` & `pybamm-23.5rc0/pybamm/solvers/scikits_ode_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/solvers/scipy_solver.py` & `pybamm-23.5rc0/pybamm/solvers/scipy_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/solvers/solution.py` & `pybamm-23.5rc0/pybamm/solvers/solution.py`

 * *Files 10% similar despite different names*

```diff
@@ -531,14 +531,79 @@
         """Save the whole solution using pickle"""
         # No warning here if len(self.data)==0 as solution can be loaded
         # and used to process new variables
 
         with open(filename, "wb") as f:
             pickle.dump(self, f, pickle.HIGHEST_PROTOCOL)
 
+    def get_data_dict(self, variables=None, short_names=None, cycles_and_steps=True):
+        """
+        Construct a (standard python) dictionary of the solution data containing the
+        variables in `variables`. If `variables` is None then all variables are
+        returned. Any variable names in short_names are replaced with the corresponding
+        short name.
+
+        If the solution has cycles, then the cycle numbers and step numbers are also
+        returned in the dictionary.
+
+        Parameters
+        ----------
+        variables : list, optional
+            List of variables to return. If None, returns all variables in solution.data
+        short_names : dict, optional
+            Dictionary of shortened names to use when saving.
+        cycles_and_steps : bool, optional
+            Whether to include the cycle numbers and step numbers in the dictionary
+
+        Returns
+        -------
+        dict
+            A dictionary of the solution data
+        """
+        if variables is None:
+            # variables not explicitly provided -> save all variables that have been
+            # computed
+            data_long_names = self.data
+        else:
+            if isinstance(variables, str):
+                variables = [variables]
+            # otherwise, save only the variables specified
+            data_long_names = {}
+            for name in variables:
+                data_long_names[name] = self[name].data
+        if len(data_long_names) == 0:
+            raise ValueError(
+                """
+                Solution does not have any data. Please provide a list of variables
+                to save.
+                """
+            )
+
+        # Use any short names if provided
+        data_short_names = {}
+        short_names = short_names or {}
+        for name, var in data_long_names.items():
+            name = short_names.get(name, name)  # return name if no short name
+            data_short_names[name] = var
+
+        # Save cycle number and step number if the solution has them
+        if cycles_and_steps and len(self.cycles) > 0:
+            data_short_names["Cycle"] = np.array([])
+            data_short_names["Step"] = np.array([])
+            for i, cycle in enumerate(self.cycles):
+                data_short_names["Cycle"] = np.concatenate(
+                    [data_short_names["Cycle"], i * np.ones_like(cycle.t)]
+                )
+                for j, step in enumerate(cycle.steps):
+                    data_short_names["Step"] = np.concatenate(
+                        [data_short_names["Step"], j * np.ones_like(step.t)]
+                    )
+
+        return data_short_names
+
     def save_data(
         self, filename=None, variables=None, to_format="pickle", short_names=None
     ):
         """
         Save solution data only (raw arrays)
 
         Parameters
@@ -561,54 +626,27 @@
             MATLAB variable names. Note that not all the variables need to be given
             a short name.
 
         Returns
         -------
         data : str, optional
             str if 'csv' or 'json' is chosen and filename is None, otherwise None
-
-
         """
-        if variables is None:
-            # variables not explicitly provided -> save all variables that have been
-            # computed
-            data = self.data
-        else:
-            # otherwise, save only the variables specified
-            data = {}
-            for name in variables:
-                data[name] = self[name].data
-        if len(data) == 0:
-            raise ValueError(
-                """
-                Solution does not have any data. Please provide a list of variables
-                to save.
-                """
-            )
-
-        # Use any short names if provided
-        data_short_names = {}
-        short_names = short_names or {}
-        for name, var in data.items():
-            # change to short name if it exists
-            if name in short_names:
-                data_short_names[short_names[name]] = var
-            else:
-                data_short_names[name] = var
+        data = self.get_data_dict(variables=variables, short_names=short_names)
 
         if to_format == "pickle":
             if filename is None:
                 raise ValueError("pickle format must be written to a file")
             with open(filename, "wb") as f:
-                pickle.dump(data_short_names, f, pickle.HIGHEST_PROTOCOL)
+                pickle.dump(data, f, pickle.HIGHEST_PROTOCOL)
         elif to_format == "matlab":
             if filename is None:
                 raise ValueError("matlab format must be written to a file")
             # Check all the variable names only contain a-z, A-Z or _ or numbers
-            for name in data_short_names.keys():
+            for name in data.keys():
                 # Check the string only contains the following ASCII:
                 # a-z (97-122)
                 # A-Z (65-90)
                 # _ (95)
                 # 0-9 (48-57) but not in the first position
                 for i, s in enumerate(name):
                     if not (
@@ -623,31 +661,31 @@
                             "or 0-9 (except the first position). "
                             "Use the 'short_names' argument to pass an alternative "
                             "variable name, e.g. \n\n"
                             "\tsolution.save_data(filename, "
                             "['Electrolyte concentration'], to_format='matlab, "
                             "short_names={'Electrolyte concentration': 'c_e'})"
                         )
-            savemat(filename, data_short_names)
+            savemat(filename, data)
         elif to_format == "csv":
-            for name, var in data_short_names.items():
+            for name, var in data.items():
                 if var.ndim >= 2:
                     raise ValueError(
                         "only 0D variables can be saved to csv, but '{}' is {}D".format(
                             name, var.ndim - 1
                         )
                     )
-            df = pd.DataFrame(data_short_names)
+            df = pd.DataFrame(data)
             return df.to_csv(filename, index=False)
         elif to_format == "json":
             if filename is None:
-                return json.dumps(data_short_names, cls=NumpyEncoder)
+                return json.dumps(data, cls=NumpyEncoder)
             else:
                 with open(filename, "w") as outfile:
-                    json.dump(data_short_names, outfile, cls=NumpyEncoder)
+                    json.dump(data, outfile, cls=NumpyEncoder)
         else:
             raise ValueError("format '{}' not recognised".format(to_format))
 
     @property
     def sub_solutions(self):
         """List of sub solutions that have been
         concatenated to form the full solution"""
@@ -747,15 +785,15 @@
             return other.copy()
 
     def __radd__(self, other):
         if other is None:
             return self.copy()
 
     def copy(self):
-        return EmptySolution(self.termination)
+        return EmptySolution(termination=self.termination, t=self.t)
 
 
 def make_cycle_solution(step_solutions, esoh_solver=None, save_this_cycle=True):
     """
     Function to create a Solution for an entire cycle, and associated summary variables
 
     Parameters
```

### Comparing `pybamm-23.4.1/pybamm/spatial_methods/finite_volume.py` & `pybamm-23.5rc0/pybamm/spatial_methods/finite_volume.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/spatial_methods/scikit_finite_element.py` & `pybamm-23.5rc0/pybamm/spatial_methods/scikit_finite_element.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/spatial_methods/spatial_method.py` & `pybamm-23.5rc0/pybamm/spatial_methods/spatial_method.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/spatial_methods/spectral_volume.py` & `pybamm-23.5rc0/pybamm/spatial_methods/spectral_volume.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/spatial_methods/zero_dimensional_method.py` & `pybamm-23.5rc0/pybamm/spatial_methods/zero_dimensional_method.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/pybamm/util.py` & `pybamm-23.5rc0/pybamm/util.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 import numpy as np
 import pkg_resources
 
 import pybamm
 
 # versions of jax and jaxlib compatible with PyBaMM
-JAX_VERSION = "0.2.12"
-JAXLIB_VERSION = "0.1.70"
+JAX_VERSION = "0.4.8"
+JAXLIB_VERSION = "0.4.7"
 
 
 def root_dir():
     """return the root directory of the PyBaMM install directory"""
     return str(pathlib.Path(pybamm.__path__[0]).parent)
 
 
@@ -217,75 +217,14 @@
         if isinstance(other, numbers.Number):
             return TimerTime(other / self.value)
 
     def __eq__(self, other):
         return self.value == other.value
 
 
-def load_function(filename, funcname=None):
-    """
-    Load a python function from an absolute or relative path using `importlib`.
-    Example - pybamm.load_function("pybamm/input/example.py")
-
-    Arguments
-    ---------
-    filename : str
-        The path of the file containing the function.
-    funcname : str, optional
-        The name of the function in the file. If None, assumed to be the same as the
-        filename (ignoring the path)
-
-    Returns
-    -------
-    function
-        The python function loaded from the file.
-    """
-    # Remove `.py` from the file name
-    if filename.endswith(".py"):
-        filename = filename.replace(".py", "")
-
-    if funcname is None:
-        # Read funcname by splitting the file (assumes funcname is the same as filename)
-        _, funcname = os.path.split(filename)
-
-    # Store the current working directory
-    orig_dir = os.getcwd()
-
-    # Strip absolute path to pybamm/input/example.py
-    if "pybamm/input/parameters" in filename or "pybamm\\input\\parameters" in filename:
-        root_path = filename[filename.rfind("pybamm") :]
-    # If the function is in the current working directory
-    elif os.getcwd() in filename:  # pragma: no cover
-        root_path = filename.replace(os.getcwd(), "")
-    # If the function is not in the current working directory and the path provided is
-    # absolute
-    elif os.path.isabs(filename) and os.getcwd() not in filename:  # pragma: no cover
-        # Change directory to import the function
-        dir_path = os.path.split(filename)[0]
-        os.chdir(dir_path)
-        root_path = filename.replace(os.getcwd(), "")
-    else:  # pragma: no cover
-        root_path = filename
-
-    # getcwd() returns "C:\\" when in the root drive and "C:\\a\\b\\c" otherwise
-    if root_path[0] == "\\" or root_path[0] == "/":  # pragma: no cover
-        root_path = root_path[1:]
-
-    path = root_path.replace("/", ".")
-    path = path.replace("\\", ".")
-    pybamm.logger.debug(
-        f"Importing function '{funcname}' from file '{filename}' via path '{path}'"
-    )
-    module_object = importlib.import_module(path)
-
-    # Revert back current working directory if it was changed
-    os.chdir(orig_dir)
-    return getattr(module_object, funcname)
-
-
 def rmse(x, y):
     """
     Calculate the root-mean-square-error between two vectors x and y, ignoring NaNs
     """
     # Check lengths
     if len(x) != len(y):
         raise ValueError("Vectors must have the same length")
```

### Comparing `pybamm-23.4.1/pybamm.egg-info/PKG-INFO` & `pybamm-23.5rc0/pybamm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: pybamm
-Version: 23.4.1
+Version: 23.5rc0
 Summary: Python Battery Mathematical Modelling.
 Home-page: https://github.com/pybamm-team/PyBaMM
 License: UNKNOWN
 Description: ![PyBaMM_logo](https://user-images.githubusercontent.com/20817509/107091287-8ad46a80-67cf-11eb-86f5-7ebef7c72a1e.png)
         
         #
         
         <div align="center">
         
         [![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](http://numfocus.org)
-        [![Build](https://github.com/pybamm-team/PyBaMM/workflows/PyBaMM/badge.svg)](https://github.com/pybamm-team/PyBaMM/actions?query=workflow%3APyBaMM+branch%3Adevelop)
+        [![Scheduled](https://github.com/pybamm-team/PyBaMM/actions/workflows/run_periodic_tests.yml/badge.svg?branch=develop)](https://github.com/pybamm-team/PyBaMM/actions/workflows/run_periodic_tests.yml)
         [![readthedocs](https://readthedocs.org/projects/pybamm/badge/?version=latest)](https://pybamm.readthedocs.io/en/latest/?badge=latest)
         [![codecov](https://codecov.io/gh/pybamm-team/PyBaMM/branch/main/graph/badge.svg)](https://codecov.io/gh/pybamm-team/PyBaMM)
         [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pybamm-team/PyBaMM/blob/develop/)
         [![DOI](https://zenodo.org/badge/DOI/10.5334/jors.309.svg)](https://doi.org/10.5334/jors.309)
         [![release](https://img.shields.io/github/v/release/pybamm-team/PyBaMM?color=yellow)](https://github.com/pybamm-team/PyBaMM/releases)
         [![black code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
         
         <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-        [![All Contributors](https://img.shields.io/badge/all_contributors-54-orange.svg)](#-contributors)
+        [![All Contributors](https://img.shields.io/badge/all_contributors-58-orange.svg)](#-contributors)
         <!-- ALL-CONTRIBUTORS-BADGE:END -->
         
         </div>
         
         # PyBaMM
         
         PyBaMM (Python Battery Mathematical Modelling) is an open-source battery simulation package
@@ -248,19 +248,24 @@
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/abillscmu"><img src="https://avatars.githubusercontent.com/u/48105066?v=4?s=100" width="100px;" alt="Alec Bills"/><br /><sub><b>Alec Bills</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=abillscmu" title="Code">💻</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/agriyakhetarpal"><img src="https://avatars.githubusercontent.com/u/74401230?v=4?s=100" width="100px;" alt="Agriya Khetarpal"/><br /><sub><b>Agriya Khetarpal</b></sub></a><br /><a href="#infra-agriyakhetarpal" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=agriyakhetarpal" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=agriyakhetarpal" title="Documentation">📖</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/awadell1"><img src="https://avatars.githubusercontent.com/u/5857298?v=4?s=100" width="100px;" alt="Alex Wadell"/><br /><sub><b>Alex Wadell</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=awadell1" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=awadell1" title="Tests">⚠️</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=awadell1" title="Documentation">📖</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/iatzak"><img src="https://avatars.githubusercontent.com/u/112731474?v=4?s=100" width="100px;" alt="iatzak"/><br /><sub><b>iatzak</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=iatzak" title="Documentation">📖</a> <a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Aiatzak" title="Bug reports">🐛</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=iatzak" title="Code">💻</a></td>
             </tr>
             <tr>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/ayeankit"><img src="https://avatars.githubusercontent.com/u/72691866?v=4?s=100" width="100px;" alt="Ankit Kumar"/><br /><sub><b>Ankit Kumar</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=ayeankit" title="Code">💻</a></td>
-              <td align="center" valign="top" width="14.28%"><a href="https://aniketsinghrawat.vercel.app/"><img src="https://avatars.githubusercontent.com/u/31622972?v=4?s=100" width="100px;" alt="Aniket Singh Rawat"/><br /><sub><b>Aniket Singh Rawat</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=dikwickley" title="Code">💻</a></td>
+              <td align="center" valign="top" width="14.28%"><a href="https://aniketsinghrawat.vercel.app/"><img src="https://avatars.githubusercontent.com/u/31622972?v=4?s=100" width="100px;" alt="Aniket Singh Rawat"/><br /><sub><b>Aniket Singh Rawat</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=dikwickley" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=dikwickley" title="Documentation">📖</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/jeromtom"><img src="https://avatars.githubusercontent.com/u/83979298?v=4?s=100" width="100px;" alt="Jerom Palimattom Tom"/><br /><sub><b>Jerom Palimattom Tom</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=jeromtom" title="Documentation">📖</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=jeromtom" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=jeromtom" title="Tests">⚠️</a></td>
               <td align="center" valign="top" width="14.28%"><a href="http://bradyplanden.github.io"><img src="https://avatars.githubusercontent.com/u/55357039?v=4?s=100" width="100px;" alt="Brady Planden"/><br /><sub><b>Brady Planden</b></sub></a><br /><a href="#example-BradyPlanden" title="Examples">💡</a></td>
               <td align="center" valign="top" width="14.28%"><a href="http://www.jsbrittain.com/"><img src="https://avatars.githubusercontent.com/u/98161205?v=4?s=100" width="100px;" alt="jsbrittain"/><br /><sub><b>jsbrittain</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=jsbrittain" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=jsbrittain" title="Tests">⚠️</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/arjxn-py"><img src="https://avatars.githubusercontent.com/u/104268427?v=4?s=100" width="100px;" alt="Arjun"/><br /><sub><b>Arjun</b></sub></a><br /><a href="#infra-arjxn-py" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
+              <td align="center" valign="top" width="14.28%"><a href="https://github.com/chenzhao-py"><img src="https://avatars.githubusercontent.com/u/75906533?v=4?s=100" width="100px;" alt="CHEN ZHAO"/><br /><sub><b>CHEN ZHAO</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Achenzhao-py" title="Bug reports">🐛</a></td>
+            </tr>
+            <tr>
+              <td align="center" valign="top" width="14.28%"><a href="https://www.aboutenergy.io/"><img src="https://avatars.githubusercontent.com/u/91731499?v=4?s=100" width="100px;" alt="darryl-ad"/><br /><sub><b>darryl-ad</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=darryl-ad" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Adarryl-ad" title="Bug reports">🐛</a></td>
+              <td align="center" valign="top" width="14.28%"><a href="https://github.com/julian-evers"><img src="https://avatars.githubusercontent.com/u/133691040?v=4?s=100" width="100px;" alt="julian-evers"/><br /><sub><b>julian-evers</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=julian-evers" title="Code">💻</a></td>
             </tr>
           </tbody>
         </table>
         
         <!-- markdownlint-restore -->
         <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: pybamm Version: 23.4.1 Summary: Python Battery
+Metadata-Version: 2.1 Name: pybamm Version: 23.5rc0 Summary: Python Battery
 Mathematical Modelling. Home-page: https://github.com/pybamm-team/PyBaMM
 License: UNKNOWN Description: ![PyBaMM_logo](https://user-
 images.githubusercontent.com/20817509/107091287-8ad46a80-67cf-11eb-86f5-
 7ebef7c72a1e.png) #
   [![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-
   orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](http://numfocus.org) [!
-  [Build](https://github.com/pybamm-team/PyBaMM/workflows/PyBaMM/badge.svg)]
-                    (https://github.com/pybamm-team/PyBaMM/
-  actions?query=workflow%3APyBaMM+branch%3Adevelop) [![readthedocs](https://
+     [Scheduled](https://github.com/pybamm-team/PyBaMM/actions/workflows/
+ run_periodic_tests.yml/badge.svg?branch=develop)](https://github.com/pybamm-
+team/PyBaMM/actions/workflows/run_periodic_tests.yml) [![readthedocs](https://
        readthedocs.org/projects/pybamm/badge/?version=latest)](https://
 pybamm.readthedocs.io/en/latest/?badge=latest) [![codecov](https://codecov.io/
   gh/pybamm-team/PyBaMM/branch/main/graph/badge.svg)](https://codecov.io/gh/
 pybamm-team/PyBaMM) [![Open In Colab](https://colab.research.google.com/assets/
 colab-badge.svg)](https://colab.research.google.com/github/pybamm-team/PyBaMM/
   blob/develop/) [![DOI](https://zenodo.org/badge/DOI/10.5334/jors.309.svg)]
 (https://doi.org/10.5334/jors.309) [![release](https://img.shields.io/github/v/
    release/pybamm-team/PyBaMM?color=yellow)](https://github.com/pybamm-team/
       PyBaMM/releases) [![black code style](https://img.shields.io/badge/
     code%20style-black-000000.svg)](https://github.com/ambv/black)  [![All
-Contributors](https://img.shields.io/badge/all_contributors-54-orange.svg)](#-
+Contributors](https://img.shields.io/badge/all_contributors-58-orange.svg)](#-
                                 contributors)
 # PyBaMM PyBaMM (Python Battery Mathematical Modelling) is an open-source
 battery simulation package written in Python. Our mission is to accelerate
 battery modelling research by providing open-source tools for multi-
 institutional, interdisciplinary collaboration. Broadly, PyBaMM consists of (i)
 a framework for writing and solving systems of differential equations, (ii) a
 library of battery models and parameters, and (iii) specialized tools for
@@ -144,17 +144,20 @@
                                                          ð ð»                                                                          ð¤                                                                         ð»                                                              ð» â ï¸                                                                   ð» â ï¸                                                            ð» ð¤                                             ð¤ ð» â ï¸ â
                                                         [Chuck_Liu]                                                                              [partben]                                                                    [Gavin_Wiggins]                                                               [Dion_Wilde]                                                                               [Elias_Hohl]                                                                    [KAschad]                                                            [Vaibhav-Chopra-GT]
                                                          Chuck_Liu                                                                                partben                                                                      Gavin_Wiggins                                                                 Dion_Wilde                                                                                 Elias_Hohl                                                                      KAschad                                                              Vaibhav-Chopra-GT
                                                          ð ð»                                                                          ð                                                                     ð ð»                                                            ð ð»                                                                            ð»                                                                      ð                                                                  ð»
                                                        [bardsleypt]                                                                          [ndrewwang]                                                                          [MichaPhilipp]                                                               [Alec_Bills]                                                                  [Agriya_Khetarpal]                                                              [Alex_Wadell]                                                                  [iatzak]
                                                         bardsleypt                                                                            ndrewwang                                                                            MichaPhilipp                                                                 Alec_Bills                                                                    Agriya_Khetarpal                                                                Alex_Wadell                                                                    iatzak
                                                          ð ð»                                                                    ð ð»                                                                        ð                                                                    ð»                                                                    ð ð» ð                                                  ð» â ï¸ ð                                                ð ð ð»
-                                                          [Ankit_Kumar]                                                                   [Aniket_Singh_Rawat]                                                        [Jerom_Palimattom_Tom]                                                                 [Brady_Planden]                                                                      [jsbrittain]                                                                          [Arjun]
-                                                           Ankit_Kumar                                                                     Aniket_Singh_Rawat                                                          Jerom_Palimattom_Tom                                                                   Brady_Planden                                                                        jsbrittain                                                                            Arjun
-                                                              ð»                                                                            ð»                                                               ð ð» â ï¸                                                           ð¡                                                                         ð» â ï¸                                                                 ð
+                                                          [Ankit_Kumar]                                                                  [Aniket_Singh_Rawat]                                                         [Jerom_Palimattom_Tom]                                                                 [Brady_Planden]                                                                      [jsbrittain]                                                                          [Arjun]                                                                   [CHEN_ZHAO]
+                                                           Ankit_Kumar                                                                    Aniket_Singh_Rawat                                                           Jerom_Palimattom_Tom                                                                   Brady_Planden                                                                        jsbrittain                                                                            Arjun                                                                     CHEN_ZHAO
+                                                              ð»                                                                        ð» ð                                                          ð ð» â ï¸                                                           ð¡                                                                         ð» â ï¸                                                                 ð                                                                    ð
+                                                        [darryl-ad]                                                                            [julian-evers]
+                                                         darryl-ad                                                                              julian-evers
+                                                         ð» ð                                                                          ð»
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome! Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
```

### Comparing `pybamm-23.4.1/pybamm.egg-info/entry_points.txt` & `pybamm-23.5rc0/pybamm.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.4.1/setup.py` & `pybamm-23.5rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,14 +226,15 @@
     extras_require={
         "docs": [
             "sphinx>=1.5",
             "pydata-sphinx-theme",
             "sphinx_design",
             "sphinx-copybutton",
             "myst-parser",
+            "sphinx-inline-tabs",
         ],  # For doc generation
         "dev": [
             "pre-commit",  # For code style checking
             "black",  # For code style auto-formatting
             "jupyter",  # For example notebooks
         ],
     },
```

