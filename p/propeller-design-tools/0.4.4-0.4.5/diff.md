# Comparing `tmp/propeller_design_tools-0.4.4.tar.gz` & `tmp/propeller_design_tools-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propeller_design_tools-0.4.4.tar", last modified: Mon Jun 19 03:44:55 2023, max compression
+gzip compressed data, was "propeller_design_tools-0.4.5.tar", last modified: Mon Jun 19 06:52:00 2023, max compression
```

## Comparing `propeller_design_tools-0.4.4.tar` & `propeller_design_tools-0.4.5.tar`

### file list

```diff
@@ -1,220 +1,220 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 03:44:55.175137 propeller_design_tools-0.4.4/
--rw-rw-rw-   0        0        0    35801 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/LICENSE
--rw-rw-rw-   0        0        0     1419 2023-06-19 03:41:46.000000 propeller_design_tools-0.4.4/MANIFEST.in
--rw-rw-rw-   0        0        0    51157 2023-06-19 03:44:55.175137 propeller_design_tools-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     8625 2023-06-19 03:15:02.000000 propeller_design_tools-0.4.4/README.md
--rw-rw-rw-   0        0        0     1668 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/TODO.md
-drwxrwxrwx   0        0        0        0 2023-06-19 03:44:53.515376 propeller_design_tools-0.4.4/propeller_design_tools/
--rw-rw-rw-   0        0        0      479 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.4/propeller_design_tools/__init__.py
--rw-rw-rw-   0        0        0    28820 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.4/propeller_design_tools/airfoil.py
--rw-rw-rw-   0        0        0     4871 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/custom_opengl_classes.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:44:53.574919 propeller_design_tools-0.4.4/propeller_design_tools/foil_database/
--rw-rw-rw-   0        0        0     1132 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/foil_database/arad13.dat
--rw-rw-rw-   0        0        0     2730 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/foil_database/clarky.dat
--rw-rw-rw-   0        0        0     1520 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/foil_database/e855.dat
--rw-rw-rw-   0        0        0     2778 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/foil_database/hs1606.dat
--rw-rw-rw-   0        0        0     2768 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/foil_database/mrc-16.dat
--rwxrwxrwx   0        0        0  1002125 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/foil_database/xfoil.exe
--rw-rw-rw-   0        0        0    18378 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.4/propeller_design_tools/foil_ui_classes.py
--rw-rw-rw-   0        0        0    50416 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.4/propeller_design_tools/funcs.py
--rw-rw-rw-   0        0        0    17861 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.4/propeller_design_tools/helper_ui_classes.py
--rw-rw-rw-   0        0        0    16315 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.4/propeller_design_tools/helper_ui_subclasses.py
--rw-rw-rw-   0        0        0      401 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.4/propeller_design_tools/opt_ui_classes.py
--rw-rw-rw-   0        0        0    11040 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.4/propeller_design_tools/optimizations.py
--rw-rw-rw-   0        0        0    15622 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_analysis_ui_classes.py
--rw-rw-rw-   0        0        0    36995 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_creation_ui_classes.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:44:53.574919 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/
-drwxrwxrwx   0        0        0        0 2023-06-19 03:44:53.600307 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/
--rw-rw-rw-   0        0        0    25993 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta
--rw-rw-rw-   0        0        0     8599 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop
--rw-rw-rw-   0        0        0     6239 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr
-drwxrwxrwx   0        0        0        0 2023-06-19 03:44:55.135231 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/
--rw-rw-rw-   0        0        0     3813 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt
--rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt
--rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt
--rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt
--rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt
--rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt
--rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt
--rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt
--rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt
--rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt
--rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt
--rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt
--rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt
--rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt
--rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt
--rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt
--rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt
--rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt
--rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt
--rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt
--rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt
--rw-rw-rw-   0        0        0     3807 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt
--rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt
--rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt
--rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt
--rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt
--rw-rw-rw-   0        0        0     3808 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt
--rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt
--rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 03:44:55.145241 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/station_polars/
--rw-rw-rw-   0        0        0     4595 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar
-drwxrwxrwx   0        0        0        0 2023-06-19 03:44:53.620085 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/
--rw-rw-rw-   0        0        0    13191 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta
--rw-rw-rw-   0        0        0     4923 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop
--rw-rw-rw-   0        0        0     3593 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr
-drwxrwxrwx   0        0        0        0 2023-06-19 03:44:53.965057 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/
--rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt
--rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt
--rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt
--rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt
--rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt
--rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt
--rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt
--rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt
--rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt
--rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt
--rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt
--rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt
--rw-rw-rw-   0        0        0     2064 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt
--rw-rw-rw-   0        0        0     2064 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt
--rw-rw-rw-   0        0        0     2064 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt
--rw-rw-rw-   0        0        0     2064 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt
--rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt
--rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt
--rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt
--rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt
--rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt
--rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt
--rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt
--rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt
--rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt
--rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt
--rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt
--rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt
--rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt
--rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 03:44:53.973241 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/station_polars/
--rw-rw-rw-   0        0        0     5160 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar
-drwxrwxrwx   0        0        0        0 2023-06-19 03:44:53.984976 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/
--rw-rw-rw-   0        0        0    13630 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta
--rw-rw-rw-   0        0        0     4875 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop
--rw-rw-rw-   0        0        0     3593 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr
-drwxrwxrwx   0        0        0        0 2023-06-19 03:44:54.775049 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/
--rw-rw-rw-   0        0        0     3771 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt
--rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt
--rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt
--rw-rw-rw-   0        0        0     3765 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt
--rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt
--rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt
--rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt
--rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt
--rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt
--rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt
--rw-rw-rw-   0        0        0     3768 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt
--rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt
--rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt
--rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt
--rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt
--rw-rw-rw-   0        0        0     3770 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt
--rw-rw-rw-   0        0        0     3771 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt
--rw-rw-rw-   0        0        0     3771 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt
--rw-rw-rw-   0        0        0     3774 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt
--rw-rw-rw-   0        0        0     3775 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt
--rw-rw-rw-   0        0        0     3777 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt
--rw-rw-rw-   0        0        0     3778 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt
--rw-rw-rw-   0        0        0     3781 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt
--rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt
--rw-rw-rw-   0        0        0     3784 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt
--rw-rw-rw-   0        0        0     3795 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt
--rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt
--rw-rw-rw-   0        0        0     3795 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt
--rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt
--rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt
--rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt
--rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt
--rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt
--rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt
--rw-rw-rw-   0        0        0     3768 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt
--rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt
--rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt
--rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt
--rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt
--rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt
--rw-rw-rw-   0        0        0     3792 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt
--rw-rw-rw-   0        0        0     3792 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt
--rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt
--rw-rw-rw-   0        0        0     3792 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt
--rw-rw-rw-   0        0        0     3792 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt
--rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt
--rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt
--rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt
--rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt
--rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 03:44:54.783383 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/station_polars/
--rw-rw-rw-   0        0        0     6152 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar
--rwxrwxrwx   0        0        0  1176521 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/prop_database/xrotor.exe
--rw-rw-rw-   0        0        0    53871 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.4/propeller_design_tools/propeller.py
--rw-rw-rw-   0        0        0    17617 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.4/propeller_design_tools/radialstation.py
--rw-rw-rw-   0        0        0     1674 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/science_spinbox_class.py
--rw-rw-rw-   0        0        0     4111 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.4/propeller_design_tools/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:44:55.175137 propeller_design_tools-0.4.4/propeller_design_tools/supporting_files/
--rw-rw-rw-   0        0        0     1358 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/supporting_files/crosshair_cursor.png
--rw-rw-rw-   0        0        0    10192 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/supporting_files/gunshot1.wav
--rw-rw-rw-   0        0        0    18704 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/supporting_files/gunshot2.wav
--rw-rw-rw-   0        0        0    23984 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/supporting_files/gunshot3.wav
--rw-rw-rw-   0        0        0    24784 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/supporting_files/gunshot4.wav
--rw-rw-rw-   0        0        0      236 2023-06-18 03:29:40.000000 propeller_design_tools-0.4.4/propeller_design_tools/supporting_files/user-settings.txt
--rw-rw-rw-   0        0        0     5857 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.4/propeller_design_tools/user_interface.py
--rw-rw-rw-   0        0        0     2839 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.4/propeller_design_tools/user_io.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:44:53.535362 propeller_design_tools-0.4.4/propeller_design_tools.egg-info/
--rw-rw-rw-   0        0        0    51157 2023-06-19 03:44:53.000000 propeller_design_tools-0.4.4/propeller_design_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    14434 2023-06-19 03:44:53.000000 propeller_design_tools-0.4.4/propeller_design_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 03:44:53.000000 propeller_design_tools-0.4.4/propeller_design_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2023-06-19 03:44:53.000000 propeller_design_tools-0.4.4/propeller_design_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-19 03:44:53.000000 propeller_design_tools-0.4.4/propeller_design_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1866 2023-06-18 05:52:56.000000 propeller_design_tools-0.4.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-19 03:44:55.175137 propeller_design_tools-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-06-18 02:25:12.000000 propeller_design_tools-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:00.438835 propeller_design_tools-0.4.5/
+-rw-rw-rw-   0        0        0    35801 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/LICENSE
+-rw-rw-rw-   0        0        0     1403 2023-06-19 04:50:38.000000 propeller_design_tools-0.4.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    54565 2023-06-19 06:52:00.434830 propeller_design_tools-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0    12013 2023-06-19 06:03:12.000000 propeller_design_tools-0.4.5/README.md
+-rw-rw-rw-   0        0        0     2551 2023-06-19 06:31:29.000000 propeller_design_tools-0.4.5/TODO.md
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:00.150805 propeller_design_tools-0.4.5/propeller_design_tools/
+-rw-rw-rw-   0        0        0      479 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.5/propeller_design_tools/__init__.py
+-rw-rw-rw-   0        0        0    28820 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.5/propeller_design_tools/airfoil.py
+-rw-rw-rw-   0        0        0     4871 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/custom_opengl_classes.py
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:00.185936 propeller_design_tools-0.4.5/propeller_design_tools/foil_database/
+-rw-rw-rw-   0        0        0     1132 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/foil_database/arad13.dat
+-rw-rw-rw-   0        0        0     2730 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/foil_database/clarky.dat
+-rw-rw-rw-   0        0        0     1520 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/foil_database/e855.dat
+-rw-rw-rw-   0        0        0     2778 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/foil_database/hs1606.dat
+-rw-rw-rw-   0        0        0     2768 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/foil_database/mrc-16.dat
+-rwxrwxrwx   0        0        0  1002125 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/foil_database/xfoil.exe
+-rw-rw-rw-   0        0        0    18378 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.5/propeller_design_tools/foil_ui_classes.py
+-rw-rw-rw-   0        0        0    50416 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.5/propeller_design_tools/funcs.py
+-rw-rw-rw-   0        0        0    17861 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.5/propeller_design_tools/helper_ui_classes.py
+-rw-rw-rw-   0        0        0    16315 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.5/propeller_design_tools/helper_ui_subclasses.py
+-rw-rw-rw-   0        0        0      401 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.5/propeller_design_tools/opt_ui_classes.py
+-rw-rw-rw-   0        0        0    11040 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.5/propeller_design_tools/optimizations.py
+-rw-rw-rw-   0        0        0    15622 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_analysis_ui_classes.py
+-rw-rw-rw-   0        0        0    37027 2023-06-19 04:50:38.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_creation_ui_classes.py
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:00.190501 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:00.195436 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/
+-rw-rw-rw-   0        0        0    25993 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta
+-rw-rw-rw-   0        0        0     8599 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop
+-rw-rw-rw-   0        0        0     6239 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:00.425759 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/
+-rw-rw-rw-   0        0        0     3813 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt
+-rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt
+-rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt
+-rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt
+-rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt
+-rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt
+-rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt
+-rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt
+-rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt
+-rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt
+-rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt
+-rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt
+-rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt
+-rw-rw-rw-   0        0        0     3807 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt
+-rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt
+-rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt
+-rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt
+-rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt
+-rw-rw-rw-   0        0        0     3808 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt
+-rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt
+-rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:00.425759 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/station_polars/
+-rw-rw-rw-   0        0        0     4595 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:00.201000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/
+-rw-rw-rw-   0        0        0    13191 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta
+-rw-rw-rw-   0        0        0     4923 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop
+-rw-rw-rw-   0        0        0     3593 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:00.270600 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt
+-rw-rw-rw-   0        0        0     2064 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt
+-rw-rw-rw-   0        0        0     2064 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt
+-rw-rw-rw-   0        0        0     2064 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt
+-rw-rw-rw-   0        0        0     2064 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt
+-rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt
+-rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt
+-rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt
+-rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt
+-rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt
+-rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt
+-rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:00.274634 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/station_polars/
+-rw-rw-rw-   0        0        0     5160 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:00.274634 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/
+-rw-rw-rw-   0        0        0    13630 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta
+-rw-rw-rw-   0        0        0     4875 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop
+-rw-rw-rw-   0        0        0     3593 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:00.350626 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/
+-rw-rw-rw-   0        0        0     3771 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt
+-rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt
+-rw-rw-rw-   0        0        0     3765 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt
+-rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt
+-rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt
+-rw-rw-rw-   0        0        0     3768 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt
+-rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt
+-rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt
+-rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt
+-rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt
+-rw-rw-rw-   0        0        0     3770 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt
+-rw-rw-rw-   0        0        0     3771 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt
+-rw-rw-rw-   0        0        0     3771 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt
+-rw-rw-rw-   0        0        0     3774 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt
+-rw-rw-rw-   0        0        0     3775 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt
+-rw-rw-rw-   0        0        0     3777 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt
+-rw-rw-rw-   0        0        0     3778 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt
+-rw-rw-rw-   0        0        0     3781 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt
+-rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt
+-rw-rw-rw-   0        0        0     3784 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt
+-rw-rw-rw-   0        0        0     3795 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt
+-rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt
+-rw-rw-rw-   0        0        0     3795 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt
+-rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt
+-rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt
+-rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt
+-rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt
+-rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt
+-rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt
+-rw-rw-rw-   0        0        0     3768 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt
+-rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt
+-rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt
+-rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt
+-rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt
+-rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt
+-rw-rw-rw-   0        0        0     3792 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt
+-rw-rw-rw-   0        0        0     3792 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt
+-rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt
+-rw-rw-rw-   0        0        0     3792 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt
+-rw-rw-rw-   0        0        0     3792 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt
+-rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt
+-rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:00.353666 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/station_polars/
+-rw-rw-rw-   0        0        0     6152 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar
+-rwxrwxrwx   0        0        0  1176521 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/prop_database/xrotor.exe
+-rw-rw-rw-   0        0        0    53871 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.5/propeller_design_tools/propeller.py
+-rw-rw-rw-   0        0        0    17617 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.5/propeller_design_tools/radialstation.py
+-rw-rw-rw-   0        0        0     1674 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/science_spinbox_class.py
+-rw-rw-rw-   0        0        0     4111 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.5/propeller_design_tools/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:00.434830 propeller_design_tools-0.4.5/propeller_design_tools/supporting_files/
+-rw-rw-rw-   0        0        0     1358 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/supporting_files/crosshair_cursor.png
+-rw-rw-rw-   0        0        0    10192 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/supporting_files/gunshot1.wav
+-rw-rw-rw-   0        0        0    18704 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/supporting_files/gunshot2.wav
+-rw-rw-rw-   0        0        0    23984 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/supporting_files/gunshot3.wav
+-rw-rw-rw-   0        0        0    24784 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/supporting_files/gunshot4.wav
+-rw-rw-rw-   0        0        0      236 2023-06-18 03:29:40.000000 propeller_design_tools-0.4.5/propeller_design_tools/supporting_files/user-settings.txt
+-rw-rw-rw-   0        0        0     5857 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.5/propeller_design_tools/user_interface.py
+-rw-rw-rw-   0        0        0     2839 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.5/propeller_design_tools/user_io.py
+drwxrwxrwx   0        0        0        0 2023-06-19 06:52:00.174763 propeller_design_tools-0.4.5/propeller_design_tools.egg-info/
+-rw-rw-rw-   0        0        0    54565 2023-06-19 06:52:00.000000 propeller_design_tools-0.4.5/propeller_design_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    14434 2023-06-19 06:52:00.000000 propeller_design_tools-0.4.5/propeller_design_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 06:52:00.000000 propeller_design_tools-0.4.5/propeller_design_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2023-06-19 06:52:00.000000 propeller_design_tools-0.4.5/propeller_design_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-19 06:52:00.000000 propeller_design_tools-0.4.5/propeller_design_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1934 2023-06-19 06:03:12.000000 propeller_design_tools-0.4.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 06:52:00.438835 propeller_design_tools-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-06-18 02:25:12.000000 propeller_design_tools-0.4.5/setup.py
```

### Comparing `propeller_design_tools-0.4.4/LICENSE` & `propeller_design_tools-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/MANIFEST.in` & `propeller_design_tools-0.4.5/MANIFEST.in`

 * *Files 0% similar despite different names*

```diff
@@ -20,9 +20,7 @@
 include propeller_design_tools/prop_database/MyPropeller3/blade_profiles/*.txt
 include propeller_design_tools/prop_database/MyPropeller3/station_polars/*.polar
 include propeller_design_tools/prop_database/MyPropeller3/*.meta
 include propeller_design_tools/prop_database/MyPropeller3/*.xrop
 include propeller_design_tools/prop_database/MyPropeller3/*.xrr
 
 include propeller_design_tools/prop_database/*.exe
-
-include *.md
```

### Comparing `propeller_design_tools-0.4.4/PKG-INFO` & `propeller_design_tools-0.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propeller_design_tools
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python 3.7 package that provides exactly what it sounds like by automating usage of MIT professor Mark Drela's GNU-licensed CLI-utilities XFOIL and XROTOR.
 Author-email: Jacob Bronson <bronsoneering@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -677,208 +677,243 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Project-URL: Homepage, https://github.com/helloDestroyerOfWorlds/propeller_design_tools.git
 Project-URL: Documentation, https://github.com/helloDestroyerOfWorlds/propeller_design_tools.git
 Project-URL: Repository, https://github.com/helloDestroyerOfWorlds/propeller_design_tools.git
 Project-URL: Changelog, https://github.com/helloDestroyerOfWorlds/propeller_design_tools.git
-Keywords: propeller,design,tools,computational,fluid,dynamics,CFD,STL,prop,rotor,xrotor,xfoil,MIT,Drela,Youngren
+Keywords: propeller,design,tools,computational,fluid,dynamics,CFD,STL,prop,rotor,xrotor,xfoil,MIT,Drela,Youngren,engineering,aero,dynamic,aerodynamic,hydrodynamic
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: stl_saving
 Provides-Extra: gui
 License-File: LICENSE
 
 propeller_design_tools (PDT)
 ============================
 ---
-**Work in progress / incomplete documentation**
+**Work in progress / incomplete documentation (all current documentation is below, as well as a step-by-step typical 
+usage/workflow scenario)**
 
-Note: The graphical user interface for this should be functional for Linux users as well very soon!!!
-
-Eventually I do plan to create better docs, but for now it's just what you see below and the source code itself.
+Note: The graphical user interface for this should be functional for Linux now as well!
 
 ---
 
 Description
 ===========
-Python 3.7 package that provides exactly what it sounds 
-like by automating usage of the GPL-licensed 
+Python 3.7 package that provides exactly what it sounds like by automating usage of the GPL-licensed 
 CLI-utilities XFOIL and XROTOR.
 
 Both utilities are published by professor Mark Drela (MIT).
-- XFOIL: for arbitrary 2D airfoil analysis
-- XROTOR: for arbitrary propeller design schemes
+- XFOIL: for arbitrary 2D airfoil analysis and design
+- XROTOR: for arbitrary propeller design schemes and analysis
+
+XFOIL and XROTOR Executables
+-------------------------------------------
+In order to utilize any PDT functionality that depends on
+running XFOIL, the "xfoil.exe" executable file needs to be
+in the user-set "airfoil_database" location. *Current pip
+installations include the xfoil.exe file in the foil_database,
+there should theoretically be no need to download it manually,
+even if the user changes the foil_database location.*
+
+[XFOIL executable and docs](https://web.mit.edu/drela/Public/web/xfoil/)
+
+Likewise, in order to utilize any PDT functionality that
+depends on running XROTOR, the "xrotor.exe" executable file
+needs to be in the user-set "propeller_database" location.
+*Current pip installations include the xrotor.exe file in the
+default prop_database, there should theoretically be no need to
+download it manually, even if the user changes the prop_database
+location.*
+
+[CROTOR executable and docs](http://www.esotec.org/sw/crotor.html#download)
+*(this is actually a link to "CROTOR", which I find is
+the easiest way to obtain a windows-executable of XROTOR)*
+
+[actual XROTOR docs](https://web.mit.edu/drela/Public/web/xrotor/xrotor_doc.txt)
+
+Both XFOIL and XROTOR contain much, much more utility than PDT currently has integrated. They are part of an incredible
+set of aerodynamic (or hydrodynamic) modeling command-line-interface (CLI) utilities from MIT. The ones that I 
+personally know of include:
+1. XFOIL - for arbitrary 2D airfoil analysis and design
+2. XROTOR - for arbitrary propeller design schemes and analysis
+3. AVL - for arbitrary lifting planform analysis
+4. QPROP - another CLI utility for propeller design and analysis
+5. QMIL - for arbitrary windmill designs (and more)
+
+Combined, the above represents an amazing fluid-dynamics modeling capability that is completely free, and fast. While 
+it's unlikely they will ever get as accurate as true computational-fluid-dynamics (CFD) software, they still offer 
+great value for being free, and are several orders of magnitude faster than true CFD software. Personally, I have found
+them to be completely sufficient tools for all stages of engineering design, but then again I have only ever worked in 
+prototyping engineering.
+
+Troubleshooting PDT Errors / Crashes (GUI and/or Scripting)
+===========================================================
+So I just quit my job as a systems engineer to become a software developer, so hopefully this package starts to get 
+more frequent updates and support from me. If you encounter what you think is an error coming from this code, I would
+love to know about it, please submit an issue to: 
+[link to Github issues](https://github.com/helloDestroyerOfWorlds/propeller_design_tools/issues)
+and I will likely see it quickly and will at least answer you, if not just fix it and push the update. Please only do 
+this though once you are sure the error is coming from the PDT code.
+
+If you think you have discovered a legitimate issue, before submitting it please also read through the list below to 
+see if any of the listed things could fix your error.
+
+1. XFOIL or XROTOR executables: Errors might be coming from XFOIL or XROTOR in actuality rather than this source code 
+   - Currently PDT implements these as executables installed when pip installing this package
+   - This means if you are having pip install errors and are on Linux it might be caused by that, actually, if you are 
+     having any errors, even in the GUI, and you are on Linux it might be caused by me not understanding until now much 
+     about Linux. If this is the case, and you think you know what is causing the error, please feel free to reach out 
+     to me via the issues link above.
+   - Additionally, I just implemented a fix to automatically install all required dependencies when pip installing this 
+     package. This should fix many issues for Linux users, if not all the current ones. Note that if you want to use the
+     GUI, read the next point.
+   - Still submit an issue using the link above if this is the case -> in theory I can detect most of these
+2. Did not install GUI version: To enable the ability to use the graphical-user-interface (GUI) you must:
+`pip install propeller_design_tools[gui]` - or - `pip install --upgrade propeller_design_tools[gui]`
+3. You're asking for an "impossible" propeller: XROTOR will error in this case.  
+   - Impossible in terms of the pure physics of what you're asking for (asking for too much thrust / power essentially)
+   - PDT has no way to know if your propeller is impossible, so I'm not sure how I could ever wrap this error in an 
+     appropriate python error wrapper even.
+   - I highly recommend to use only the "constant" blade cl distribution target option
+     - I have not had time yet to test any of the other options much
+     - Other options are disabled in the GUI until I can test them fully
+     - Other options in the future will be a "linear" option as well as "file" option (which essentially allows the user 
+       to define an arbitrary, discreet function for the blade Cl distribution).
+   - It is also highly recommended to use only the 'grad' or 'pot' solver options until you know you have the code at 
+     least generating an output without failing. 
+     - I would only then recommend moving on to using the 'vrtx' solver. This solver is (in my opinion) the superior of 
+       the 3 options. Though it takes longest to solve by far, it seems to be the only one that reliably produces 
+       reasonable chord lengths near the hub. I think the 'vrtx' solver is somewhat less stable than the other two as 
+       well, so if you think you're having errors with PDT try to switch solvers.
+4. You're asking for XFOIL to analyze your airfoil at too low or too high of an angle-of-attack (AoA)
+   - I have attempted to remove the need for the user to enter AoA, but my algorithm for this is far from perfect.
+   - If you think this is your error, please submit it via issue link above.
+5. You're trying to open the STL file generated by PDT in SolidWorks: this is a known issue currently being worked on.
+   - I've no idea why this happens, it seems to be a purely SolidWorks issue, the STL file seems to open just fine in
+     everything else I have tried.
+   - Try opening the file and re-saving it (I suggest MS Paint, I think the new version can save STLs).
+   - Try opening the file and re-saving it after having very slightly changed it.
+   - If you encounter this error but think you have figured it out or have useful information about it please submit an
+     issue via the link above.
 
-IMPORTANT NOTE: to potentially aid in realizing errors are coming from XFOIL or XROTOR rather than this source code ->
-currently this source code implements these as executables installed when pip installing this package -> this means if
-you are having pip install errors and are on Linux it might be caused by that.  Actually, if you are having any errors,
-even in the GUI, and you are on Linux it might be caused by me not understanding until now much about Linux.  If this 
-is the case and you think you know what is causing the error, please feel free to reach out to me to let me know.
-
-CONTINUED: additionally, very soon I will be implementing a fix to automatically install all dependencies, which should
-fix many issues for Linux users, if not all of the current ones.  I also HIGHLY RECOMMEND to use only the "constant" 
-blade cl distribution target option for the first time you ever use this code, and then only venture into other options
-once you are familiar with the code more and can explain to me even what exactly Mark Drela means by this parameter.  I
-think it's just his way of saying the parameter that controls what you want each target section's operating AoA to be,
-which in all honestly I have personally found to not really affect the outputs all that much with the exception
-(obviously) of what each section's chord length will end up being.  It doesn't seem to impact overall realized efficiency
-of the design very much (< ~5-10 percent in all my experiences).
-
-For this same exact reason, it is also HIGHLY RECOMMENDED to use only the 'grad' or 'pot' solver options until you know
-you have the code at least generating an output without failing.  My personal favorite solver is the 'vrtx' option, 
-but XROTOR seems to be much less stable and take much, much longer to arrive at solutions when using 'vrtx'.  However,
-the 'vrtx' option is the only one that seems to produce relatively reasonable chord lengths near the hub.
 Thank you all that is my TED talk.
 
 Purpose
 =======
-PDT seeks to provide the user a set of python3 utilities
-that can be used for arbitrary scripting efforts to automate
-usage of both XFOIL and XROTOR while implementing its own 
-unique python3.7-native algorithms to maintain local
-input files, meta files, databases, and results files and
-weave everything together for the user in a simple,
-meaningful way to aid in the initial / investigatory 
-stage of well-behaved propeller designs.
+PDT seeks to provide the user a set of python3 utilities that can be used for arbitrary scripting efforts to automate
+usage of both XFOIL and XROTOR while implementing its own unique python3-native algorithms to maintain local
+input files, meta files, databases, and results files and weave everything together for the user in a simple,
+meaningful way to aid in the initial / investigatory stage of well-behaved propeller designs (free-flow and non-ducted
+assumptions).
 
 Getting Started
 ===============
 Installation
 ------------
-`pip install propdes`
+`pip install propeller_design_tools` - or - `pip install propeller_design_tools[gui]`
+
+Update
+------
+`pip install --upgrade propeller_design_tools` - or - `pip install --upgrade propeller_design_tools[gui]`
 
 General Operation
 -----------------
 `import propeller_design_tools as pdt`
 
-PDT operates on two different "database" directories, defined
-by the user with:
+PDT operates on two different "database" directories, defined by the user with:
 
-    pdt.set_airfoil_database(path: str)
-    pdt.set_propeller_database(path: str)
+`pdt.set_airfoil_database(path: str)`
+and
+`pdt.set_propeller_database(path: str)`
 
-**The user must set these two directories at the top 
-of every script right after the imports**
+**The user must set these two directories at the top of every script right after the imports**
 
-*The airfoil directory will be used to store any foil / 
-XFOIL- related support files, and the propeller directory
-will be used similarly to store any propeller / XROTOR - 
-related support files.*
-
-Pre-Requisite: XFOIL and XROTOR Executables
--------------------------------------------
-(soon this section will be obsolete as I plan to implement a pure-python
-version of both XFOIL and XROTOR in the source code)
-
-In order to utilize any PDT functionality that depends on 
-running XFOIL, the "xfoil.exe" executable file needs to be
-in the user-set "airfoil_database" location. *Current pip 
-installations include the xfoil.exe file in the foil_database,
-there should theoretically be no need to download it manually.*
-
-[XFOIL executable and docs](https://web.mit.edu/drela/Public/web/xfoil/)
-
-Likewise, in order to utilize any PDT functionality that
-depends on running XROTOR, the "xrotor.exe" executable file
-needs to be in the user-set "propeller_database" location.
-*Current pip installations include the xrotor.exe file in the 
-default prop_database, there should theoretically be no need to 
-download it manually.*
-
-[CROTOR executable and docs](http://www.esotec.org/sw/crotor.html#download)
-*(this is actually a link to "CROTOR", which I find is
-the easiest way to obtain a windows-executable of XROTOR)*
-
-[actual XROTOR docs](https://web.mit.edu/drela/Public/web/xrotor/xrotor_doc.txt)
+*The airfoil directory will be used to store any foil / XFOIL-related support files, and the propeller directory
+will be used similarly to store any propeller / XROTOR-related support files.*
 
 Example Scripts / Workflow
 --------------------------
-At a high-level, the current concept for PDT workflow is as 
-follows (after obtaining the required executables and pip-installing 
-the PDT package):
+At a high-level, the current concept for the PDT workflow is as follows (after pip-installing the PDT package):
 
 0. Try out the (currently extremely buggy and incomplete) user interface!
 [example0_user_interface.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example0_user_interface.py
    )
  
+   ![why_dont_my_image_links_work](https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/ex0-1.png)
+
    ![ex0-1](./tests/ex0-1.png)
    ![ex0-2](./tests/ex0-2.png)
    ![ex0-3](./tests/ex0-3.png)
 
-2. Obtain normalized airfoil coordinate files from
+
+1. Obtain normalized airfoil coordinate files from
 [UIUC Database](https://m-selig.ae.illinois.edu/ads/coord_database.html)
--> save these files into the "airfoil_database" directory
+and save these files into the "airfoil_database" directory (GUI users can just use the built-in tool to download)
 
 
-2. Use PDT to run XFOIL across ranges of Reynolds Numbers in order to
-populate database data for the desired foil sections -> see 
+2. Use PDT to run XFOIL across ranges of Reynolds Numbers in order to populate database data for the desired foil 
+sections -> see 
 [example1_airfoil_analysis.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example1_airfoil_analysis.py
    )
 
    ![ex1-1](./tests/ex1-1.png)
    ![ex1-2](./tests/ex1-2.png)
 
 
-3. Once the required 2D airfoil data is generated, PDT can then be used
-to automatically generate all the required 2D foil definition parameters
-required by XROTOR (these "station parameters" are essentially what 
-allow XROTOR to model the performance of well-behaved, arbitrarily-lofted 
-blade geometries) -> see
+3. Once the required 2D airfoil data is generated, PDT can then be used to automatically generate all the required 2D 
+   foil definition parameters required by XROTOR (these "station parameters" are essentially what allow XROTOR to model 
+   the performance of well-behaved, arbitrarily-lofted blade geometries) -> see
 [example2_radialstation_creation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example2_radialstation_creation.py
    )
 
    ![ex2-1](./tests/ex2-1.png)
    
-   But this step is also automated & displayed by PDT when the user uses
-the builtin PDT propeller creation function -> see
+**But this step is also automated & displayed by PDT when the using the builtin PDT propeller creation function (or the 
+GUI)** -> see
 [example3_prop_creation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example3_prop_creation.py
    )
 
    ![ex3-1](./tests/ex3-1.png)
 
-   NOTE: It is highly recommended to first run XROTOR using either the 'grad' 
-or the 'pot' vortex formulation in order to get your design "tweaked in" -> 
-these are much faster than the (more accurate) 'vrtx' formulation, which you 
+NOTE: It is highly recommended to first run XROTOR using either the 'grad' or the 'pot' vortex formulation in order to 
+get your design "tweaked in" -> these are much faster than the (more accurate) 'vrtx' formulation, which you 
 can then move on to.
 
    ![ex3-2](./tests/ex3-2.png)
 
 
-4. PDT's Propeller() object instances can generate 3D geometry files 
-including profle xyz coordinate listings, and .stl 3D geometry files -> see
+4. PDT's `Propeller()` object instances can generate 3D geometry files including profile xyz coordinate listings and 
+   .stl 3D geometry files -> see
 [example4_stl_generation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example4_stl_generation.py
    )
 
    ![ex4-1](./tests/ex4-1.png)
 
-Note: It is known that currently there is an issue with these .stl files opening in SolidWorks -> try converting them
-using anything (first idea is MS Paint, I think the new version can save STL files as well).  As far as I can tell this 
-is only an issue for SolidWorks users on Windows, these files open and display fine in every other application.
 
-5. Analyze a given Propeller() instance across a sweep of operating points -> see 
+5. Analyze a given `Propeller()` instance across a sweep of operating points -> see 
 [example5_prop_analysis.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example5_prop_analysis.py
    )
 
    ![ex5-1](./tests/ex5-1.png)
 
 
-6. **WIP** Prop optimization (grid-search style generic optimizer for "optimal"
-prop design generation by means of maximizing or minimizing a given output / 
-calculated metric based on outputs, optionally taking into account different
-propeller operating points via the ability to define the propeller's "duty-cycle"
--> coming soon! This should elimiate the user's need to even input a value for the
-desired blade cl distribution altogether.)
+6. **WIP** Prop optimization 
+   - Will be a grid-search style generic optimizer for "optimal" prop design generation by means of minimizing overall 
+     energy usage. 
+   - Optionally takes into account different propeller operating points via the ability to define the propeller's 
+     "duty-cycle"
+     - This feature is coming soon!
```

### Comparing `propeller_design_tools-0.4.4/README.md` & `propeller_design_tools-0.4.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,186 +1,222 @@
 propeller_design_tools (PDT)
 ============================
 ---
-**Work in progress / incomplete documentation**
+**Work in progress / incomplete documentation (all current documentation is below, as well as a step-by-step typical 
+usage/workflow scenario)**
 
-Note: The graphical user interface for this should be functional for Linux users as well very soon!!!
-
-Eventually I do plan to create better docs, but for now it's just what you see below and the source code itself.
+Note: The graphical user interface for this should be functional for Linux now as well!
 
 ---
 
 Description
 ===========
-Python 3.7 package that provides exactly what it sounds 
-like by automating usage of the GPL-licensed 
+Python 3.7 package that provides exactly what it sounds like by automating usage of the GPL-licensed 
 CLI-utilities XFOIL and XROTOR.
 
 Both utilities are published by professor Mark Drela (MIT).
-- XFOIL: for arbitrary 2D airfoil analysis
-- XROTOR: for arbitrary propeller design schemes
+- XFOIL: for arbitrary 2D airfoil analysis and design
+- XROTOR: for arbitrary propeller design schemes and analysis
+
+XFOIL and XROTOR Executables
+-------------------------------------------
+In order to utilize any PDT functionality that depends on
+running XFOIL, the "xfoil.exe" executable file needs to be
+in the user-set "airfoil_database" location. *Current pip
+installations include the xfoil.exe file in the foil_database,
+there should theoretically be no need to download it manually,
+even if the user changes the foil_database location.*
+
+[XFOIL executable and docs](https://web.mit.edu/drela/Public/web/xfoil/)
+
+Likewise, in order to utilize any PDT functionality that
+depends on running XROTOR, the "xrotor.exe" executable file
+needs to be in the user-set "propeller_database" location.
+*Current pip installations include the xrotor.exe file in the
+default prop_database, there should theoretically be no need to
+download it manually, even if the user changes the prop_database
+location.*
+
+[CROTOR executable and docs](http://www.esotec.org/sw/crotor.html#download)
+*(this is actually a link to "CROTOR", which I find is
+the easiest way to obtain a windows-executable of XROTOR)*
+
+[actual XROTOR docs](https://web.mit.edu/drela/Public/web/xrotor/xrotor_doc.txt)
+
+Both XFOIL and XROTOR contain much, much more utility than PDT currently has integrated. They are part of an incredible
+set of aerodynamic (or hydrodynamic) modeling command-line-interface (CLI) utilities from MIT. The ones that I 
+personally know of include:
+1. XFOIL - for arbitrary 2D airfoil analysis and design
+2. XROTOR - for arbitrary propeller design schemes and analysis
+3. AVL - for arbitrary lifting planform analysis
+4. QPROP - another CLI utility for propeller design and analysis
+5. QMIL - for arbitrary windmill designs (and more)
+
+Combined, the above represents an amazing fluid-dynamics modeling capability that is completely free, and fast. While 
+it's unlikely they will ever get as accurate as true computational-fluid-dynamics (CFD) software, they still offer 
+great value for being free, and are several orders of magnitude faster than true CFD software. Personally, I have found
+them to be completely sufficient tools for all stages of engineering design, but then again I have only ever worked in 
+prototyping engineering.
+
+Troubleshooting PDT Errors / Crashes (GUI and/or Scripting)
+===========================================================
+So I just quit my job as a systems engineer to become a software developer, so hopefully this package starts to get 
+more frequent updates and support from me. If you encounter what you think is an error coming from this code, I would
+love to know about it, please submit an issue to: 
+[link to Github issues](https://github.com/helloDestroyerOfWorlds/propeller_design_tools/issues)
+and I will likely see it quickly and will at least answer you, if not just fix it and push the update. Please only do 
+this though once you are sure the error is coming from the PDT code.
+
+If you think you have discovered a legitimate issue, before submitting it please also read through the list below to 
+see if any of the listed things could fix your error.
+
+1. XFOIL or XROTOR executables: Errors might be coming from XFOIL or XROTOR in actuality rather than this source code 
+   - Currently PDT implements these as executables installed when pip installing this package
+   - This means if you are having pip install errors and are on Linux it might be caused by that, actually, if you are 
+     having any errors, even in the GUI, and you are on Linux it might be caused by me not understanding until now much 
+     about Linux. If this is the case, and you think you know what is causing the error, please feel free to reach out 
+     to me via the issues link above.
+   - Additionally, I just implemented a fix to automatically install all required dependencies when pip installing this 
+     package. This should fix many issues for Linux users, if not all the current ones. Note that if you want to use the
+     GUI, read the next point.
+   - Still submit an issue using the link above if this is the case -> in theory I can detect most of these
+2. Did not install GUI version: To enable the ability to use the graphical-user-interface (GUI) you must:
+`pip install propeller_design_tools[gui]` - or - `pip install --upgrade propeller_design_tools[gui]`
+3. You're asking for an "impossible" propeller: XROTOR will error in this case.  
+   - Impossible in terms of the pure physics of what you're asking for (asking for too much thrust / power essentially)
+   - PDT has no way to know if your propeller is impossible, so I'm not sure how I could ever wrap this error in an 
+     appropriate python error wrapper even.
+   - I highly recommend to use only the "constant" blade cl distribution target option
+     - I have not had time yet to test any of the other options much
+     - Other options are disabled in the GUI until I can test them fully
+     - Other options in the future will be a "linear" option as well as "file" option (which essentially allows the user 
+       to define an arbitrary, discreet function for the blade Cl distribution).
+   - It is also highly recommended to use only the 'grad' or 'pot' solver options until you know you have the code at 
+     least generating an output without failing. 
+     - I would only then recommend moving on to using the 'vrtx' solver. This solver is (in my opinion) the superior of 
+       the 3 options. Though it takes longest to solve by far, it seems to be the only one that reliably produces 
+       reasonable chord lengths near the hub. I think the 'vrtx' solver is somewhat less stable than the other two as 
+       well, so if you think you're having errors with PDT try to switch solvers.
+4. You're asking for XFOIL to analyze your airfoil at too low or too high of an angle-of-attack (AoA)
+   - I have attempted to remove the need for the user to enter AoA, but my algorithm for this is far from perfect.
+   - If you think this is your error, please submit it via issue link above.
+5. You're trying to open the STL file generated by PDT in SolidWorks: this is a known issue currently being worked on.
+   - I've no idea why this happens, it seems to be a purely SolidWorks issue, the STL file seems to open just fine in
+     everything else I have tried.
+   - Try opening the file and re-saving it (I suggest MS Paint, I think the new version can save STLs).
+   - Try opening the file and re-saving it after having very slightly changed it.
+   - If you encounter this error but think you have figured it out or have useful information about it please submit an
+     issue via the link above.
 
-IMPORTANT NOTE: to potentially aid in realizing errors are coming from XFOIL or XROTOR rather than this source code ->
-currently this source code implements these as executables installed when pip installing this package -> this means if
-you are having pip install errors and are on Linux it might be caused by that.  Actually, if you are having any errors,
-even in the GUI, and you are on Linux it might be caused by me not understanding until now much about Linux.  If this 
-is the case and you think you know what is causing the error, please feel free to reach out to me to let me know.
-
-CONTINUED: additionally, very soon I will be implementing a fix to automatically install all dependencies, which should
-fix many issues for Linux users, if not all of the current ones.  I also HIGHLY RECOMMEND to use only the "constant" 
-blade cl distribution target option for the first time you ever use this code, and then only venture into other options
-once you are familiar with the code more and can explain to me even what exactly Mark Drela means by this parameter.  I
-think it's just his way of saying the parameter that controls what you want each target section's operating AoA to be,
-which in all honestly I have personally found to not really affect the outputs all that much with the exception
-(obviously) of what each section's chord length will end up being.  It doesn't seem to impact overall realized efficiency
-of the design very much (< ~5-10 percent in all my experiences).
-
-For this same exact reason, it is also HIGHLY RECOMMENDED to use only the 'grad' or 'pot' solver options until you know
-you have the code at least generating an output without failing.  My personal favorite solver is the 'vrtx' option, 
-but XROTOR seems to be much less stable and take much, much longer to arrive at solutions when using 'vrtx'.  However,
-the 'vrtx' option is the only one that seems to produce relatively reasonable chord lengths near the hub.
 Thank you all that is my TED talk.
 
 Purpose
 =======
-PDT seeks to provide the user a set of python3 utilities
-that can be used for arbitrary scripting efforts to automate
-usage of both XFOIL and XROTOR while implementing its own 
-unique python3.7-native algorithms to maintain local
-input files, meta files, databases, and results files and
-weave everything together for the user in a simple,
-meaningful way to aid in the initial / investigatory 
-stage of well-behaved propeller designs.
+PDT seeks to provide the user a set of python3 utilities that can be used for arbitrary scripting efforts to automate
+usage of both XFOIL and XROTOR while implementing its own unique python3-native algorithms to maintain local
+input files, meta files, databases, and results files and weave everything together for the user in a simple,
+meaningful way to aid in the initial / investigatory stage of well-behaved propeller designs (free-flow and non-ducted
+assumptions).
 
 Getting Started
 ===============
 Installation
 ------------
-`pip install propdes`
+`pip install propeller_design_tools` - or - `pip install propeller_design_tools[gui]`
+
+Update
+------
+`pip install --upgrade propeller_design_tools` - or - `pip install --upgrade propeller_design_tools[gui]`
 
 General Operation
 -----------------
 `import propeller_design_tools as pdt`
 
-PDT operates on two different "database" directories, defined
-by the user with:
+PDT operates on two different "database" directories, defined by the user with:
 
-    pdt.set_airfoil_database(path: str)
-    pdt.set_propeller_database(path: str)
+`pdt.set_airfoil_database(path: str)`
+and
+`pdt.set_propeller_database(path: str)`
 
-**The user must set these two directories at the top 
-of every script right after the imports**
+**The user must set these two directories at the top of every script right after the imports**
 
-*The airfoil directory will be used to store any foil / 
-XFOIL- related support files, and the propeller directory
-will be used similarly to store any propeller / XROTOR - 
-related support files.*
-
-Pre-Requisite: XFOIL and XROTOR Executables
--------------------------------------------
-(soon this section will be obsolete as I plan to implement a pure-python
-version of both XFOIL and XROTOR in the source code)
-
-In order to utilize any PDT functionality that depends on 
-running XFOIL, the "xfoil.exe" executable file needs to be
-in the user-set "airfoil_database" location. *Current pip 
-installations include the xfoil.exe file in the foil_database,
-there should theoretically be no need to download it manually.*
-
-[XFOIL executable and docs](https://web.mit.edu/drela/Public/web/xfoil/)
-
-Likewise, in order to utilize any PDT functionality that
-depends on running XROTOR, the "xrotor.exe" executable file
-needs to be in the user-set "propeller_database" location.
-*Current pip installations include the xrotor.exe file in the 
-default prop_database, there should theoretically be no need to 
-download it manually.*
-
-[CROTOR executable and docs](http://www.esotec.org/sw/crotor.html#download)
-*(this is actually a link to "CROTOR", which I find is
-the easiest way to obtain a windows-executable of XROTOR)*
-
-[actual XROTOR docs](https://web.mit.edu/drela/Public/web/xrotor/xrotor_doc.txt)
+*The airfoil directory will be used to store any foil / XFOIL-related support files, and the propeller directory
+will be used similarly to store any propeller / XROTOR-related support files.*
 
 Example Scripts / Workflow
 --------------------------
-At a high-level, the current concept for PDT workflow is as 
-follows (after obtaining the required executables and pip-installing 
-the PDT package):
+At a high-level, the current concept for the PDT workflow is as follows (after pip-installing the PDT package):
 
 0. Try out the (currently extremely buggy and incomplete) user interface!
 [example0_user_interface.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example0_user_interface.py
    )
  
+   ![why_dont_my_image_links_work](https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/ex0-1.png)
+
    ![ex0-1](./tests/ex0-1.png)
    ![ex0-2](./tests/ex0-2.png)
    ![ex0-3](./tests/ex0-3.png)
 
-2. Obtain normalized airfoil coordinate files from
+
+1. Obtain normalized airfoil coordinate files from
 [UIUC Database](https://m-selig.ae.illinois.edu/ads/coord_database.html)
--> save these files into the "airfoil_database" directory
+and save these files into the "airfoil_database" directory (GUI users can just use the built-in tool to download)
 
 
-2. Use PDT to run XFOIL across ranges of Reynolds Numbers in order to
-populate database data for the desired foil sections -> see 
+2. Use PDT to run XFOIL across ranges of Reynolds Numbers in order to populate database data for the desired foil 
+sections -> see 
 [example1_airfoil_analysis.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example1_airfoil_analysis.py
    )
 
    ![ex1-1](./tests/ex1-1.png)
    ![ex1-2](./tests/ex1-2.png)
 
 
-3. Once the required 2D airfoil data is generated, PDT can then be used
-to automatically generate all the required 2D foil definition parameters
-required by XROTOR (these "station parameters" are essentially what 
-allow XROTOR to model the performance of well-behaved, arbitrarily-lofted 
-blade geometries) -> see
+3. Once the required 2D airfoil data is generated, PDT can then be used to automatically generate all the required 2D 
+   foil definition parameters required by XROTOR (these "station parameters" are essentially what allow XROTOR to model 
+   the performance of well-behaved, arbitrarily-lofted blade geometries) -> see
 [example2_radialstation_creation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example2_radialstation_creation.py
    )
 
    ![ex2-1](./tests/ex2-1.png)
    
-   But this step is also automated & displayed by PDT when the user uses
-the builtin PDT propeller creation function -> see
+**But this step is also automated & displayed by PDT when the using the builtin PDT propeller creation function (or the 
+GUI)** -> see
 [example3_prop_creation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example3_prop_creation.py
    )
 
    ![ex3-1](./tests/ex3-1.png)
 
-   NOTE: It is highly recommended to first run XROTOR using either the 'grad' 
-or the 'pot' vortex formulation in order to get your design "tweaked in" -> 
-these are much faster than the (more accurate) 'vrtx' formulation, which you 
+NOTE: It is highly recommended to first run XROTOR using either the 'grad' or the 'pot' vortex formulation in order to 
+get your design "tweaked in" -> these are much faster than the (more accurate) 'vrtx' formulation, which you 
 can then move on to.
 
    ![ex3-2](./tests/ex3-2.png)
 
 
-4. PDT's Propeller() object instances can generate 3D geometry files 
-including profle xyz coordinate listings, and .stl 3D geometry files -> see
+4. PDT's `Propeller()` object instances can generate 3D geometry files including profile xyz coordinate listings and 
+   .stl 3D geometry files -> see
 [example4_stl_generation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example4_stl_generation.py
    )
 
    ![ex4-1](./tests/ex4-1.png)
 
-Note: It is known that currently there is an issue with these .stl files opening in SolidWorks -> try converting them
-using anything (first idea is MS Paint, I think the new version can save STL files as well).  As far as I can tell this 
-is only an issue for SolidWorks users on Windows, these files open and display fine in every other application.
 
-5. Analyze a given Propeller() instance across a sweep of operating points -> see 
+5. Analyze a given `Propeller()` instance across a sweep of operating points -> see 
 [example5_prop_analysis.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example5_prop_analysis.py
    )
 
    ![ex5-1](./tests/ex5-1.png)
 
 
-6. **WIP** Prop optimization (grid-search style generic optimizer for "optimal"
-prop design generation by means of maximizing or minimizing a given output / 
-calculated metric based on outputs, optionally taking into account different
-propeller operating points via the ability to define the propeller's "duty-cycle"
--> coming soon! This should elimiate the user's need to even input a value for the
-desired blade cl distribution altogether.)
+6. **WIP** Prop optimization 
+   - Will be a grid-search style generic optimizer for "optimal" prop design generation by means of minimizing overall 
+     energy usage. 
+   - Optionally takes into account different propeller operating points via the ability to define the propeller's 
+     "duty-cycle"
+     - This feature is coming soon!
```

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/airfoil.py` & `propeller_design_tools-0.4.5/propeller_design_tools/airfoil.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/custom_opengl_classes.py` & `propeller_design_tools-0.4.5/propeller_design_tools/custom_opengl_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/foil_database/arad13.dat` & `propeller_design_tools-0.4.5/propeller_design_tools/foil_database/arad13.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/foil_database/clarky.dat` & `propeller_design_tools-0.4.5/propeller_design_tools/foil_database/clarky.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/foil_database/e855.dat` & `propeller_design_tools-0.4.5/propeller_design_tools/foil_database/e855.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/foil_database/hs1606.dat` & `propeller_design_tools-0.4.5/propeller_design_tools/foil_database/hs1606.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/foil_database/mrc-16.dat` & `propeller_design_tools-0.4.5/propeller_design_tools/foil_database/mrc-16.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/foil_database/xfoil.exe` & `propeller_design_tools-0.4.5/propeller_design_tools/foil_database/xfoil.exe`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/foil_ui_classes.py` & `propeller_design_tools-0.4.5/propeller_design_tools/foil_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/funcs.py` & `propeller_design_tools-0.4.5/propeller_design_tools/funcs.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/helper_ui_classes.py` & `propeller_design_tools-0.4.5/propeller_design_tools/helper_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/helper_ui_subclasses.py` & `propeller_design_tools-0.4.5/propeller_design_tools/helper_ui_subclasses.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/optimizations.py` & `propeller_design_tools-0.4.5/propeller_design_tools/optimizations.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_analysis_ui_classes.py` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_analysis_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_creation_ui_classes.py` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_creation_ui_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,16 @@
         self.design_power_sb.setSpecialValueText('None')
         self.design_power_sb.setMaximum(np.inf)
         self.design_power_sb.valueChanged.connect(self.des_power_sb_changed)
         form_lay2a.addRow(PDT_Label('Power:', font_size=12), self.design_power_sb)
 
         # center / right form layout
         self.design_cl_le = PDT_LineEdit(font_size=12, width=80)
-        form_lay2c.addRow(PDT_Label('C_l (const or root, tip):', font_size=12), self.design_cl_le)
+        self.design_cl_le.setText('0.1')
+        form_lay2c.addRow(PDT_Label('C_l (constant):', font_size=12), self.design_cl_le)
 
         # atmo props, vorform, station params
         self.atmo_props_widg = AtmoPropsInputWidget()
         form_lay2c.addRow(PDT_Label('Atmosphere\nProperties->', font_size=12), self.atmo_props_widg)
         self.station_params_widg = StationParamsWidget()
         form_lay2c.addRow(PDT_Label('Control\nStations->', font_size=12), self.station_params_widg)
```

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/prop_database/xrotor.exe` & `propeller_design_tools-0.4.5/propeller_design_tools/prop_database/xrotor.exe`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/propeller.py` & `propeller_design_tools-0.4.5/propeller_design_tools/propeller.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/radialstation.py` & `propeller_design_tools-0.4.5/propeller_design_tools/radialstation.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/science_spinbox_class.py` & `propeller_design_tools-0.4.5/propeller_design_tools/science_spinbox_class.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/settings.py` & `propeller_design_tools-0.4.5/propeller_design_tools/settings.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/supporting_files/crosshair_cursor.png` & `propeller_design_tools-0.4.5/propeller_design_tools/supporting_files/crosshair_cursor.png`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/supporting_files/gunshot1.wav` & `propeller_design_tools-0.4.5/propeller_design_tools/supporting_files/gunshot1.wav`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/supporting_files/gunshot2.wav` & `propeller_design_tools-0.4.5/propeller_design_tools/supporting_files/gunshot2.wav`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/supporting_files/gunshot3.wav` & `propeller_design_tools-0.4.5/propeller_design_tools/supporting_files/gunshot3.wav`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/supporting_files/gunshot4.wav` & `propeller_design_tools-0.4.5/propeller_design_tools/supporting_files/gunshot4.wav`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/user_interface.py` & `propeller_design_tools-0.4.5/propeller_design_tools/user_interface.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools/user_io.py` & `propeller_design_tools-0.4.5/propeller_design_tools/user_io.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools.egg-info/PKG-INFO` & `propeller_design_tools-0.4.5/propeller_design_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propeller-design-tools
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python 3.7 package that provides exactly what it sounds like by automating usage of MIT professor Mark Drela's GNU-licensed CLI-utilities XFOIL and XROTOR.
 Author-email: Jacob Bronson <bronsoneering@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -677,208 +677,243 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Project-URL: Homepage, https://github.com/helloDestroyerOfWorlds/propeller_design_tools.git
 Project-URL: Documentation, https://github.com/helloDestroyerOfWorlds/propeller_design_tools.git
 Project-URL: Repository, https://github.com/helloDestroyerOfWorlds/propeller_design_tools.git
 Project-URL: Changelog, https://github.com/helloDestroyerOfWorlds/propeller_design_tools.git
-Keywords: propeller,design,tools,computational,fluid,dynamics,CFD,STL,prop,rotor,xrotor,xfoil,MIT,Drela,Youngren
+Keywords: propeller,design,tools,computational,fluid,dynamics,CFD,STL,prop,rotor,xrotor,xfoil,MIT,Drela,Youngren,engineering,aero,dynamic,aerodynamic,hydrodynamic
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: stl_saving
 Provides-Extra: gui
 License-File: LICENSE
 
 propeller_design_tools (PDT)
 ============================
 ---
-**Work in progress / incomplete documentation**
+**Work in progress / incomplete documentation (all current documentation is below, as well as a step-by-step typical 
+usage/workflow scenario)**
 
-Note: The graphical user interface for this should be functional for Linux users as well very soon!!!
-
-Eventually I do plan to create better docs, but for now it's just what you see below and the source code itself.
+Note: The graphical user interface for this should be functional for Linux now as well!
 
 ---
 
 Description
 ===========
-Python 3.7 package that provides exactly what it sounds 
-like by automating usage of the GPL-licensed 
+Python 3.7 package that provides exactly what it sounds like by automating usage of the GPL-licensed 
 CLI-utilities XFOIL and XROTOR.
 
 Both utilities are published by professor Mark Drela (MIT).
-- XFOIL: for arbitrary 2D airfoil analysis
-- XROTOR: for arbitrary propeller design schemes
+- XFOIL: for arbitrary 2D airfoil analysis and design
+- XROTOR: for arbitrary propeller design schemes and analysis
+
+XFOIL and XROTOR Executables
+-------------------------------------------
+In order to utilize any PDT functionality that depends on
+running XFOIL, the "xfoil.exe" executable file needs to be
+in the user-set "airfoil_database" location. *Current pip
+installations include the xfoil.exe file in the foil_database,
+there should theoretically be no need to download it manually,
+even if the user changes the foil_database location.*
+
+[XFOIL executable and docs](https://web.mit.edu/drela/Public/web/xfoil/)
+
+Likewise, in order to utilize any PDT functionality that
+depends on running XROTOR, the "xrotor.exe" executable file
+needs to be in the user-set "propeller_database" location.
+*Current pip installations include the xrotor.exe file in the
+default prop_database, there should theoretically be no need to
+download it manually, even if the user changes the prop_database
+location.*
+
+[CROTOR executable and docs](http://www.esotec.org/sw/crotor.html#download)
+*(this is actually a link to "CROTOR", which I find is
+the easiest way to obtain a windows-executable of XROTOR)*
+
+[actual XROTOR docs](https://web.mit.edu/drela/Public/web/xrotor/xrotor_doc.txt)
+
+Both XFOIL and XROTOR contain much, much more utility than PDT currently has integrated. They are part of an incredible
+set of aerodynamic (or hydrodynamic) modeling command-line-interface (CLI) utilities from MIT. The ones that I 
+personally know of include:
+1. XFOIL - for arbitrary 2D airfoil analysis and design
+2. XROTOR - for arbitrary propeller design schemes and analysis
+3. AVL - for arbitrary lifting planform analysis
+4. QPROP - another CLI utility for propeller design and analysis
+5. QMIL - for arbitrary windmill designs (and more)
+
+Combined, the above represents an amazing fluid-dynamics modeling capability that is completely free, and fast. While 
+it's unlikely they will ever get as accurate as true computational-fluid-dynamics (CFD) software, they still offer 
+great value for being free, and are several orders of magnitude faster than true CFD software. Personally, I have found
+them to be completely sufficient tools for all stages of engineering design, but then again I have only ever worked in 
+prototyping engineering.
+
+Troubleshooting PDT Errors / Crashes (GUI and/or Scripting)
+===========================================================
+So I just quit my job as a systems engineer to become a software developer, so hopefully this package starts to get 
+more frequent updates and support from me. If you encounter what you think is an error coming from this code, I would
+love to know about it, please submit an issue to: 
+[link to Github issues](https://github.com/helloDestroyerOfWorlds/propeller_design_tools/issues)
+and I will likely see it quickly and will at least answer you, if not just fix it and push the update. Please only do 
+this though once you are sure the error is coming from the PDT code.
+
+If you think you have discovered a legitimate issue, before submitting it please also read through the list below to 
+see if any of the listed things could fix your error.
+
+1. XFOIL or XROTOR executables: Errors might be coming from XFOIL or XROTOR in actuality rather than this source code 
+   - Currently PDT implements these as executables installed when pip installing this package
+   - This means if you are having pip install errors and are on Linux it might be caused by that, actually, if you are 
+     having any errors, even in the GUI, and you are on Linux it might be caused by me not understanding until now much 
+     about Linux. If this is the case, and you think you know what is causing the error, please feel free to reach out 
+     to me via the issues link above.
+   - Additionally, I just implemented a fix to automatically install all required dependencies when pip installing this 
+     package. This should fix many issues for Linux users, if not all the current ones. Note that if you want to use the
+     GUI, read the next point.
+   - Still submit an issue using the link above if this is the case -> in theory I can detect most of these
+2. Did not install GUI version: To enable the ability to use the graphical-user-interface (GUI) you must:
+`pip install propeller_design_tools[gui]` - or - `pip install --upgrade propeller_design_tools[gui]`
+3. You're asking for an "impossible" propeller: XROTOR will error in this case.  
+   - Impossible in terms of the pure physics of what you're asking for (asking for too much thrust / power essentially)
+   - PDT has no way to know if your propeller is impossible, so I'm not sure how I could ever wrap this error in an 
+     appropriate python error wrapper even.
+   - I highly recommend to use only the "constant" blade cl distribution target option
+     - I have not had time yet to test any of the other options much
+     - Other options are disabled in the GUI until I can test them fully
+     - Other options in the future will be a "linear" option as well as "file" option (which essentially allows the user 
+       to define an arbitrary, discreet function for the blade Cl distribution).
+   - It is also highly recommended to use only the 'grad' or 'pot' solver options until you know you have the code at 
+     least generating an output without failing. 
+     - I would only then recommend moving on to using the 'vrtx' solver. This solver is (in my opinion) the superior of 
+       the 3 options. Though it takes longest to solve by far, it seems to be the only one that reliably produces 
+       reasonable chord lengths near the hub. I think the 'vrtx' solver is somewhat less stable than the other two as 
+       well, so if you think you're having errors with PDT try to switch solvers.
+4. You're asking for XFOIL to analyze your airfoil at too low or too high of an angle-of-attack (AoA)
+   - I have attempted to remove the need for the user to enter AoA, but my algorithm for this is far from perfect.
+   - If you think this is your error, please submit it via issue link above.
+5. You're trying to open the STL file generated by PDT in SolidWorks: this is a known issue currently being worked on.
+   - I've no idea why this happens, it seems to be a purely SolidWorks issue, the STL file seems to open just fine in
+     everything else I have tried.
+   - Try opening the file and re-saving it (I suggest MS Paint, I think the new version can save STLs).
+   - Try opening the file and re-saving it after having very slightly changed it.
+   - If you encounter this error but think you have figured it out or have useful information about it please submit an
+     issue via the link above.
 
-IMPORTANT NOTE: to potentially aid in realizing errors are coming from XFOIL or XROTOR rather than this source code ->
-currently this source code implements these as executables installed when pip installing this package -> this means if
-you are having pip install errors and are on Linux it might be caused by that.  Actually, if you are having any errors,
-even in the GUI, and you are on Linux it might be caused by me not understanding until now much about Linux.  If this 
-is the case and you think you know what is causing the error, please feel free to reach out to me to let me know.
-
-CONTINUED: additionally, very soon I will be implementing a fix to automatically install all dependencies, which should
-fix many issues for Linux users, if not all of the current ones.  I also HIGHLY RECOMMEND to use only the "constant" 
-blade cl distribution target option for the first time you ever use this code, and then only venture into other options
-once you are familiar with the code more and can explain to me even what exactly Mark Drela means by this parameter.  I
-think it's just his way of saying the parameter that controls what you want each target section's operating AoA to be,
-which in all honestly I have personally found to not really affect the outputs all that much with the exception
-(obviously) of what each section's chord length will end up being.  It doesn't seem to impact overall realized efficiency
-of the design very much (< ~5-10 percent in all my experiences).
-
-For this same exact reason, it is also HIGHLY RECOMMENDED to use only the 'grad' or 'pot' solver options until you know
-you have the code at least generating an output without failing.  My personal favorite solver is the 'vrtx' option, 
-but XROTOR seems to be much less stable and take much, much longer to arrive at solutions when using 'vrtx'.  However,
-the 'vrtx' option is the only one that seems to produce relatively reasonable chord lengths near the hub.
 Thank you all that is my TED talk.
 
 Purpose
 =======
-PDT seeks to provide the user a set of python3 utilities
-that can be used for arbitrary scripting efforts to automate
-usage of both XFOIL and XROTOR while implementing its own 
-unique python3.7-native algorithms to maintain local
-input files, meta files, databases, and results files and
-weave everything together for the user in a simple,
-meaningful way to aid in the initial / investigatory 
-stage of well-behaved propeller designs.
+PDT seeks to provide the user a set of python3 utilities that can be used for arbitrary scripting efforts to automate
+usage of both XFOIL and XROTOR while implementing its own unique python3-native algorithms to maintain local
+input files, meta files, databases, and results files and weave everything together for the user in a simple,
+meaningful way to aid in the initial / investigatory stage of well-behaved propeller designs (free-flow and non-ducted
+assumptions).
 
 Getting Started
 ===============
 Installation
 ------------
-`pip install propdes`
+`pip install propeller_design_tools` - or - `pip install propeller_design_tools[gui]`
+
+Update
+------
+`pip install --upgrade propeller_design_tools` - or - `pip install --upgrade propeller_design_tools[gui]`
 
 General Operation
 -----------------
 `import propeller_design_tools as pdt`
 
-PDT operates on two different "database" directories, defined
-by the user with:
+PDT operates on two different "database" directories, defined by the user with:
 
-    pdt.set_airfoil_database(path: str)
-    pdt.set_propeller_database(path: str)
+`pdt.set_airfoil_database(path: str)`
+and
+`pdt.set_propeller_database(path: str)`
 
-**The user must set these two directories at the top 
-of every script right after the imports**
+**The user must set these two directories at the top of every script right after the imports**
 
-*The airfoil directory will be used to store any foil / 
-XFOIL- related support files, and the propeller directory
-will be used similarly to store any propeller / XROTOR - 
-related support files.*
-
-Pre-Requisite: XFOIL and XROTOR Executables
--------------------------------------------
-(soon this section will be obsolete as I plan to implement a pure-python
-version of both XFOIL and XROTOR in the source code)
-
-In order to utilize any PDT functionality that depends on 
-running XFOIL, the "xfoil.exe" executable file needs to be
-in the user-set "airfoil_database" location. *Current pip 
-installations include the xfoil.exe file in the foil_database,
-there should theoretically be no need to download it manually.*
-
-[XFOIL executable and docs](https://web.mit.edu/drela/Public/web/xfoil/)
-
-Likewise, in order to utilize any PDT functionality that
-depends on running XROTOR, the "xrotor.exe" executable file
-needs to be in the user-set "propeller_database" location.
-*Current pip installations include the xrotor.exe file in the 
-default prop_database, there should theoretically be no need to 
-download it manually.*
-
-[CROTOR executable and docs](http://www.esotec.org/sw/crotor.html#download)
-*(this is actually a link to "CROTOR", which I find is
-the easiest way to obtain a windows-executable of XROTOR)*
-
-[actual XROTOR docs](https://web.mit.edu/drela/Public/web/xrotor/xrotor_doc.txt)
+*The airfoil directory will be used to store any foil / XFOIL-related support files, and the propeller directory
+will be used similarly to store any propeller / XROTOR-related support files.*
 
 Example Scripts / Workflow
 --------------------------
-At a high-level, the current concept for PDT workflow is as 
-follows (after obtaining the required executables and pip-installing 
-the PDT package):
+At a high-level, the current concept for the PDT workflow is as follows (after pip-installing the PDT package):
 
 0. Try out the (currently extremely buggy and incomplete) user interface!
 [example0_user_interface.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example0_user_interface.py
    )
  
+   ![why_dont_my_image_links_work](https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/ex0-1.png)
+
    ![ex0-1](./tests/ex0-1.png)
    ![ex0-2](./tests/ex0-2.png)
    ![ex0-3](./tests/ex0-3.png)
 
-2. Obtain normalized airfoil coordinate files from
+
+1. Obtain normalized airfoil coordinate files from
 [UIUC Database](https://m-selig.ae.illinois.edu/ads/coord_database.html)
--> save these files into the "airfoil_database" directory
+and save these files into the "airfoil_database" directory (GUI users can just use the built-in tool to download)
 
 
-2. Use PDT to run XFOIL across ranges of Reynolds Numbers in order to
-populate database data for the desired foil sections -> see 
+2. Use PDT to run XFOIL across ranges of Reynolds Numbers in order to populate database data for the desired foil 
+sections -> see 
 [example1_airfoil_analysis.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example1_airfoil_analysis.py
    )
 
    ![ex1-1](./tests/ex1-1.png)
    ![ex1-2](./tests/ex1-2.png)
 
 
-3. Once the required 2D airfoil data is generated, PDT can then be used
-to automatically generate all the required 2D foil definition parameters
-required by XROTOR (these "station parameters" are essentially what 
-allow XROTOR to model the performance of well-behaved, arbitrarily-lofted 
-blade geometries) -> see
+3. Once the required 2D airfoil data is generated, PDT can then be used to automatically generate all the required 2D 
+   foil definition parameters required by XROTOR (these "station parameters" are essentially what allow XROTOR to model 
+   the performance of well-behaved, arbitrarily-lofted blade geometries) -> see
 [example2_radialstation_creation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example2_radialstation_creation.py
    )
 
    ![ex2-1](./tests/ex2-1.png)
    
-   But this step is also automated & displayed by PDT when the user uses
-the builtin PDT propeller creation function -> see
+**But this step is also automated & displayed by PDT when the using the builtin PDT propeller creation function (or the 
+GUI)** -> see
 [example3_prop_creation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example3_prop_creation.py
    )
 
    ![ex3-1](./tests/ex3-1.png)
 
-   NOTE: It is highly recommended to first run XROTOR using either the 'grad' 
-or the 'pot' vortex formulation in order to get your design "tweaked in" -> 
-these are much faster than the (more accurate) 'vrtx' formulation, which you 
+NOTE: It is highly recommended to first run XROTOR using either the 'grad' or the 'pot' vortex formulation in order to 
+get your design "tweaked in" -> these are much faster than the (more accurate) 'vrtx' formulation, which you 
 can then move on to.
 
    ![ex3-2](./tests/ex3-2.png)
 
 
-4. PDT's Propeller() object instances can generate 3D geometry files 
-including profle xyz coordinate listings, and .stl 3D geometry files -> see
+4. PDT's `Propeller()` object instances can generate 3D geometry files including profile xyz coordinate listings and 
+   .stl 3D geometry files -> see
 [example4_stl_generation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example4_stl_generation.py
    )
 
    ![ex4-1](./tests/ex4-1.png)
 
-Note: It is known that currently there is an issue with these .stl files opening in SolidWorks -> try converting them
-using anything (first idea is MS Paint, I think the new version can save STL files as well).  As far as I can tell this 
-is only an issue for SolidWorks users on Windows, these files open and display fine in every other application.
 
-5. Analyze a given Propeller() instance across a sweep of operating points -> see 
+5. Analyze a given `Propeller()` instance across a sweep of operating points -> see 
 [example5_prop_analysis.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example5_prop_analysis.py
    )
 
    ![ex5-1](./tests/ex5-1.png)
 
 
-6. **WIP** Prop optimization (grid-search style generic optimizer for "optimal"
-prop design generation by means of maximizing or minimizing a given output / 
-calculated metric based on outputs, optionally taking into account different
-propeller operating points via the ability to define the propeller's "duty-cycle"
--> coming soon! This should elimiate the user's need to even input a value for the
-desired blade cl distribution altogether.)
+6. **WIP** Prop optimization 
+   - Will be a grid-search style generic optimizer for "optimal" prop design generation by means of minimizing overall 
+     energy usage. 
+   - Optionally takes into account different propeller operating points via the ability to define the propeller's 
+     "duty-cycle"
+     - This feature is coming soon!
```

### Comparing `propeller_design_tools-0.4.4/propeller_design_tools.egg-info/SOURCES.txt` & `propeller_design_tools-0.4.5/propeller_design_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.4/pyproject.toml` & `propeller_design_tools-0.4.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [build-system]
 requires = ["setuptools>=67.8.0", "wheel>=0.40.0"]  # build requirements (don't include build or twine)
 build-backend = "setuptools.build_meta"
 
 
 [project]
-version = "0.4.4"
+version = "0.4.5"
 name = "propeller_design_tools"
 authors = [{name = "Jacob Bronson", email = "bronsoneering@gmail.com"}]
 description = "Python 3.7 package that provides exactly what it sounds like by automating usage of MIT professor Mark Drela's GNU-licensed CLI-utilities XFOIL and XROTOR."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ['propeller', 'design', 'tools', 'computational', 'fluid', 'dynamics', 'CFD', 'STL', 'prop', 'rotor',
-            'xrotor', 'xfoil', 'MIT', 'Drela', 'Youngren']
+            'xrotor', 'xfoil', 'MIT', 'Drela', 'Youngren', 'engineering', 'aero', 'dynamic', 'aerodynamic',
+            'hydrodynamic']
 license = {file = "LICENSE"}
 
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
@@ -27,19 +28,19 @@
 
 dependencies = [
     "numpy>=1.21.2",
     "matplotlib>=3.4.3",
     "scipy>=1.7.1",
     "pyqtgraph>=0.12.4",
     "pyopengl>=3.1.6",
+    "numpy-stl>=2.16.3",
 ]
 
 
 [project.optional-dependencies]
-stl_saving = ["numpy-stl>=2.16.3"]
 gui = ["PyQt5>=5.15.9"]
 
 
 [project.urls]
 Homepage = "https://github.com/helloDestroyerOfWorlds/propeller_design_tools.git"
 Documentation = "https://github.com/helloDestroyerOfWorlds/propeller_design_tools.git"
 Repository = "https://github.com/helloDestroyerOfWorlds/propeller_design_tools.git"
```

