# Comparing `tmp/pyplotterlib-1.6.0.tar.gz` & `tmp/pyplotterlib-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplotterlib-1.6.0.tar", last modified: Thu Jun 15 19:21:22 2023, max compression
+gzip compressed data, was "pyplotterlib-1.7.0.tar", last modified: Mon Jun 19 19:32:28 2023, max compression
```

## Comparing `pyplotterlib-1.6.0.tar` & `pyplotterlib-1.7.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.692657 pyplotterlib-1.6.0/
--rw-rw-r--   0 richard   (1000) richard   (1000)     1066 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/LICENSE
--rw-rw-r--   0 richard   (1000) richard   (1000)     2054 2023-06-15 19:21:22.692657 pyplotterlib-1.6.0/PKG-INFO
--rw-rw-r--   0 richard   (1000) richard   (1000)      151 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/README.md
--rw-rw-r--   0 richard   (1000) richard   (1000)     1199 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/pyproject.toml
--rw-rw-r--   0 richard   (1000) richard   (1000)       38 2023-06-15 19:21:22.692657 pyplotterlib-1.6.0/setup.cfg
--rw-rw-r--   0 richard   (1000) richard   (1000)       50 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/setup.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/__init__.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib/core/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      570 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/json_transform.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1088 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/plot_command.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    11955 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/plot_options.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     5558 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/plotters.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib/core/serialization/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/serialization/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      510 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/serialization/json_io.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      175 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/serialization/register.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2617 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/serialization/registration_funct.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib/core/serialization/unit_tests/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/serialization/unit_tests/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2222 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/serialization/unit_tests/utest_create_from_json.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib/core/unit_tests/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/unit_tests/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    17393 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/unit_tests/utest_plot_options.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     5031 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/unit_tests/utest_plotters.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/__init__.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/read_serialization_test/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/read_serialization_test/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1276 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/read_serialization_test/helpers.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      570 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/shared.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/viz_diff/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/viz_diff/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1693 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/viz_diff/helpers.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib/standard/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     5823 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/annotations.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    40317 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/plot_commands.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    28022 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/plot_options.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      952 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/plotters.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    17613 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/bar_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    16907 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/box_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    15676 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/disc_heat_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     8696 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/histogram_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     4762 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/image_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     4309 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/line_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    23966 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/rect_multi_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     3002 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/shared.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     5339 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/shared_axis_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    18443 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/split_axis_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    23588 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/split_axis_plotter_creator.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.692657 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/unit_tests/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/unit_tests/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2079 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/unit_tests/utests_histogram_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1937 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/serialization.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.692657 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/__init__.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.692657 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1119 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_bar_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      888 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_histogram_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      951 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_image_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1269 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_line_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1049 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_rect_multi_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1093 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_shared_axis_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1289 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_creator.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1059 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1140 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/utests_plot_commands.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib.egg-info/
--rw-rw-r--   0 richard   (1000) richard   (1000)     2054 2023-06-15 19:21:22.000000 pyplotterlib-1.6.0/src/pyplotterlib.egg-info/PKG-INFO
--rw-rw-r--   0 richard   (1000) richard   (1000)     3047 2023-06-15 19:21:22.000000 pyplotterlib-1.6.0/src/pyplotterlib.egg-info/SOURCES.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)        1 2023-06-15 19:21:22.000000 pyplotterlib-1.6.0/src/pyplotterlib.egg-info/dependency_links.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)      180 2023-06-15 19:21:22.000000 pyplotterlib-1.6.0/src/pyplotterlib.egg-info/requires.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)       13 2023-06-15 19:21:22.000000 pyplotterlib-1.6.0/src/pyplotterlib.egg-info/top_level.txt
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-19 19:32:28.709144 pyplotterlib-1.7.0/
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1066 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/LICENSE
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2054 2023-06-19 19:32:28.709144 pyplotterlib-1.7.0/PKG-INFO
+-rw-rw-r--   0 richard   (1000) richard   (1000)      151 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/README.md
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1199 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/pyproject.toml
+-rw-rw-r--   0 richard   (1000) richard   (1000)       38 2023-06-19 19:32:28.709144 pyplotterlib-1.7.0/setup.cfg
+-rw-rw-r--   0 richard   (1000) richard   (1000)       50 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/setup.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-19 19:32:28.705145 pyplotterlib-1.7.0/src/
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-19 19:32:28.705145 pyplotterlib-1.7.0/src/pyplotterlib/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/__init__.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-19 19:32:28.705145 pyplotterlib-1.7.0/src/pyplotterlib/core/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/core/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      570 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/core/json_transform.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1088 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/core/plot_command.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    11955 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/core/plot_options.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     5558 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/core/plotters.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-19 19:32:28.705145 pyplotterlib-1.7.0/src/pyplotterlib/core/serialization/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/core/serialization/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      510 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/core/serialization/json_io.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      175 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/core/serialization/register.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2617 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/core/serialization/registration_funct.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-19 19:32:28.705145 pyplotterlib-1.7.0/src/pyplotterlib/core/serialization/unit_tests/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/core/serialization/unit_tests/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2222 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/core/serialization/unit_tests/utest_create_from_json.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-19 19:32:28.705145 pyplotterlib-1.7.0/src/pyplotterlib/core/unit_tests/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/core/unit_tests/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    17393 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/core/unit_tests/utest_plot_options.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     5031 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/core/unit_tests/utest_plotters.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-19 19:32:28.705145 pyplotterlib-1.7.0/src/pyplotterlib/reg_testing/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/reg_testing/__init__.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-19 19:32:28.705145 pyplotterlib-1.7.0/src/pyplotterlib/reg_testing/read_serialization_test/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/reg_testing/read_serialization_test/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1276 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/reg_testing/read_serialization_test/helpers.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      570 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/reg_testing/shared.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-19 19:32:28.705145 pyplotterlib-1.7.0/src/pyplotterlib/reg_testing/viz_diff/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/reg_testing/viz_diff/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1693 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/reg_testing/viz_diff/helpers.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-19 19:32:28.709144 pyplotterlib-1.7.0/src/pyplotterlib/standard/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     5823 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/annotations.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    45967 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/plot_commands.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    31967 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/plot_options.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      952 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/plotters.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-19 19:32:28.709144 pyplotterlib-1.7.0/src/pyplotterlib/standard/private/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/private/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    20103 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/private/bar_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    16907 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/private/box_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    15676 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/private/disc_heat_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     8696 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/private/histogram_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     4762 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/private/image_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     4692 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/private/line_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    23966 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/private/rect_multi_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     3002 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/private/shared.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     5339 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/private/shared_axis_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    18443 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/private/split_axis_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    23588 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/private/split_axis_plotter_creator.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-19 19:32:28.709144 pyplotterlib-1.7.0/src/pyplotterlib/standard/private/unit_tests/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/private/unit_tests/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2079 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/private/unit_tests/utests_histogram_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1937 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/serialization.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-19 19:32:28.709144 pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/__init__.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-19 19:32:28.709144 pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/serialization/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/serialization/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1119 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/serialization/utests_bar_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      888 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/serialization/utests_histogram_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      951 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/serialization/utests_image_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1269 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/serialization/utests_line_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1049 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/serialization/utests_rect_multi_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1093 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/serialization/utests_shared_axis_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1289 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_creator.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1059 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1140 2023-06-19 19:31:42.000000 pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/utests_plot_commands.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-19 19:32:28.705145 pyplotterlib-1.7.0/src/pyplotterlib.egg-info/
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2054 2023-06-19 19:32:28.000000 pyplotterlib-1.7.0/src/pyplotterlib.egg-info/PKG-INFO
+-rw-rw-r--   0 richard   (1000) richard   (1000)     3047 2023-06-19 19:32:28.000000 pyplotterlib-1.7.0/src/pyplotterlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)        1 2023-06-19 19:32:28.000000 pyplotterlib-1.7.0/src/pyplotterlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)      180 2023-06-19 19:32:28.000000 pyplotterlib-1.7.0/src/pyplotterlib.egg-info/requires.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)       13 2023-06-19 19:32:28.000000 pyplotterlib-1.7.0/src/pyplotterlib.egg-info/top_level.txt
```

### Comparing `pyplotterlib-1.6.0/LICENSE` & `pyplotterlib-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/PKG-INFO` & `pyplotterlib-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplotterlib
-Version: 1.6.0
+Version: 1.7.0
 Summary: A package used to create plots in python
 Author-email: Richard Fogarty <richard.m.fogarty@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 RFogarty1
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyplotterlib-1.6.0/pyproject.toml` & `pyplotterlib-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=60.9.3", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyplotterlib"
-version = "1.6.0"
+version = "1.7.0"
 description = "A package used to create plots in python"
 readme = "README.md"
 authors = [{ name = "Richard Fogarty", email = "richard.m.fogarty@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Framework :: Matplotlib",
     "License :: OSI Approved :: MIT License",
```

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/core/json_transform.py` & `pyplotterlib-1.7.0/src/pyplotterlib/core/json_transform.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/core/plot_command.py` & `pyplotterlib-1.7.0/src/pyplotterlib/core/plot_command.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/core/plot_options.py` & `pyplotterlib-1.7.0/src/pyplotterlib/core/plot_options.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/core/plotters.py` & `pyplotterlib-1.7.0/src/pyplotterlib/core/plotters.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/core/serialization/registration_funct.py` & `pyplotterlib-1.7.0/src/pyplotterlib/core/serialization/registration_funct.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/core/serialization/unit_tests/utest_create_from_json.py` & `pyplotterlib-1.7.0/src/pyplotterlib/core/serialization/unit_tests/utest_create_from_json.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/core/unit_tests/utest_plot_options.py` & `pyplotterlib-1.7.0/src/pyplotterlib/core/unit_tests/utest_plot_options.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/core/unit_tests/utest_plotters.py` & `pyplotterlib-1.7.0/src/pyplotterlib/core/unit_tests/utest_plotters.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/read_serialization_test/helpers.py` & `pyplotterlib-1.7.0/src/pyplotterlib/reg_testing/read_serialization_test/helpers.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/shared.py` & `pyplotterlib-1.7.0/src/pyplotterlib/reg_testing/shared.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/viz_diff/helpers.py` & `pyplotterlib-1.7.0/src/pyplotterlib/reg_testing/viz_diff/helpers.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/annotations.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/annotations.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/plot_commands.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/plot_commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -326,20 +326,75 @@
 		#Get the data; exit if none present
 		targVal = getattr(plotterInstance.opts, self._optName).value
 		if targVal is None:
 			return None
 		elif len(targVal)==0:
 			return None
 
+		#Look for any error bars present
+		_errorBarDefVal = [None for x in targVal]
+		errorBarsY = _getValueFromOptName(plotterInstance, "errorBarDataY", _errorBarDefVal)
+		errorBarsX = _getValueFromOptName(plotterInstance, "errorBarDataX", _errorBarDefVal)
+		errorBarMplHooks = _getValueFromOptName(plotterInstance, "errorBarLineMplHooks", _errorBarDefVal)
+
+		errorBarMplHooks = [hooks for hooks,unused in zip( it.cycle(errorBarMplHooks), targVal)]
+
 		#Plot the data; may want to return handles to scratch space later
-		for currData in targVal:
-			plt.plot( np.array(currData)[:,0], np.array(currData)[:,1] )
+		lineHandles = list()
+		errorLineHandles, errorCapHandles = list(), list()
+		capsizeVals = self._getCapsizeVals(plotterInstance)
+		for idx,(currData, xErrBars, yErrBars, hooks) in enumerate(it.zip_longest(targVal,errorBarsX,errorBarsY, errorBarMplHooks)):
+			xData, yData = np.array(currData)[:,0], np.array(currData)[:,1]
+			if (xErrBars is not None) or (yErrBars is not None):
+				_xBars, _yBars = [self._reshapeErrorBarData(bars) for bars in [xErrBars,yErrBars]]
+				hooks = dict() if hooks is None else hooks
+				if capsizeVals[idx] is not None:
+					hooks["capsize"] = capsizeVals[idx]
+				_allLines = plt.errorbar( xData, yData, yerr=_yBars, xerr=_xBars, **hooks ).lines
+				currLines = _allLines[0]
+				errorCapHandles.append(_allLines[1])
+				errorLineHandles.append(_allLines[2])
+			else:
+				currLines = plt.plot( xData, yData )[0]
+			lineHandles.append(currLines)
+
+		#Add plotted lines to scratch space
+		_setScratchSpaceDictKey(plotterInstance, "plotLineHandles", "value", lineHandles)
+		if len(errorLineHandles) > 0:
+			_setScratchSpaceDictKey(plotterInstance, "errorBars", "lineHandles", errorLineHandles)
+			_setScratchSpaceDictKey(plotterInstance, "errorBars", "capHandles", errorCapHandles)
 
 		return
 
+	def _reshapeErrorBarData(self, errorBarData):
+		if errorBarData is None:
+			return None
+
+		useData = np.array(errorBarData)
+
+		if useData.shape[-1] == 2:
+			return useData.transpose()
+		else:
+			return useData
+
+	def _getCapsizeVals(self, plotterInstance):
+		#Figure out how many vals we need to know
+		plotData = _getValueFromOptName(plotterInstance, self._optName, retIfNone=list())
+
+		#Figure out what capsizes to use
+		errorCapsizes = _getValueFromOptName(plotterInstance, "errorBarCapsize", retIfNone=None)
+		if errorCapsizes is None:
+			return [None for x in plotData]
+
+		useCapsizes = it.cycle(errorCapsizes)
+		outVals = [capsize for data,capsize in zip(plotData, useCapsizes)]
+
+		return outVals
+
+
 @serializationReg.registerForSerialization()
 class PlotHozAndVertLines(plotCommCoreHelp.PlotCommand):
 
 	def __init__(self):
 		self._name = "plot-hoz-and-vert-lines"
 		self._description = "Plots horizontal and vertical lines; generally should be AFTER the main plotting (and x/y limit setting)"
 
@@ -755,21 +810,65 @@
 		self._optName = "dataLabels"
 
 	def execute(self, plotterInstance):
 		targVal = getattr(plotterInstance.opts, self._optName).value
 		if targVal is None:
 			return None
 
-		plottedLineHandles = plt.gca().get_lines()
+		_defVal = list()
+		plottedLineHandles = _getScratchSpaceValueIfPresent(plotterInstance, "plotLineHandles", "value", retValIfNone=_defVal)
+
 		for lineHandle, dataLabel in zip(plottedLineHandles, targVal):
 			if dataLabel is not None:
 				lineHandle.set_label(dataLabel)
 
 
 @serializationReg.registerForSerialization()
+class SetLineErrorBarColors(plotCommCoreHelp.PlotCommand):
+
+	def __init__(self):
+		self._name = "setLineErrorBarColors"
+		self._description = "Sets the color of the error bars"
+
+	def execute(self, plotterInstance):
+		#Get error bar handles (exit if not present)
+		errorHandles = _getScratchSpaceValueIfPresent(plotterInstance, "errorBars", "lineHandles", retValIfNone=None)
+		errorCapHandles = _getScratchSpaceValueIfPresent(plotterInstance, "errorBars", "capHandles", retValIfNone=None)
+		if errorHandles is None:
+			return None
+
+		#Figure out what colors to use; if empty then exit without doing anything
+		colorCycle = self._getColorCycle(plotterInstance)
+		if colorCycle is None:
+			return None
+
+		useColors = it.cycle(colorCycle)
+
+		for capHandles,barHandles,color in zip(errorCapHandles,errorHandles,useColors):
+			[handle.set_color(color) for handle in barHandles]
+			[handle.set_color(color) for handle in capHandles]
+
+	def _getColorCycle(self, plotterInstance):
+		outCycles = None #The output variable
+
+		#Set default values to the data line colors if their present
+		useLineColors = _getValueFromOptName(plotterInstance, "errorBarColorsMatchLinesByDefault", retIfNone=False)
+		lineColors = _getValueFromOptName(plotterInstance, "lineColors", retIfNone=None)
+		if (lineColors is not None) and (useLineColors is True):
+			outCycles = lineColors
+
+		#TODO: Overwrite this with a more specific option if present
+		overwriteColors = _getValueFromOptName(plotterInstance, "errorBarColors", retIfNone=None)
+		if overwriteColors is not None:
+			outCycles = overwriteColors
+
+		return outCycles
+
+
+@serializationReg.registerForSerialization()
 class SetLegendFontSize(plotCommCoreHelp.PlotCommand):
 
 	def __init__(self):
 		self._name = "setLegendFontSize"
 		self._description = "Sets the font size to use in the legend"
 
 	def execute(self, plotterInstance):
@@ -833,29 +932,47 @@
 		try:
 			locStr = plotterInstance._scratchSpace["legendKwargDict"]["loc"] = targVal
 		except KeyError:
 			plotterInstance._scratchSpace["legendKwargDict"]["loc"] = targVal
 		else:
 			plotterInstance._scratchSpace["legendKwargDict"]["bbox_to_anchor"] = targVal
 
+#
+@serializationReg.registerForSerialization()
+class SetLegendHandlesToPlottedLinesDefault(plotCommCoreHelp.PlotCommand):
+
+	def __init__(self):
+		self._name = "setLegendHandlesToPlottedLines"
+		self._description = "If they are present in the scratch space, the legend handles are set to plotLineHandles; this is to avoid errorbars interfering with the legend"
+
+	def execute(self, plotterInstance):
+		lineHandles = _getScratchSpaceValueIfPresent(plotterInstance, "plotLineHandles", "value")
+		if lineHandles is None:
+			return None
+		_setScratchSpaceDictKey(plotterInstance, "legendKwargDict", "handles", lineHandles)
+		
+
 
 @serializationReg.registerForSerialization()
 class SetLineColors(plotCommCoreHelp.PlotCommand):
 
 	def __init__(self):
 		self._name = "setLineColors"
 		self._description = "Sets the line colors for lines currently plotted"
 		self._optName = "lineColors"
 
 	def execute(self, plotterInstance):
 		targVal = getattr(plotterInstance.opts, self._optName).value
 		if targVal is None:
 			return None
 
-		dataLines = plt.gca().get_lines()
+
+
+		_defVal = list()
+		dataLines = _getScratchSpaceValueIfPresent(plotterInstance, "plotLineHandles", "value", retValIfNone=_defVal)
 		colors = it.cycle(targVal)
 		for dataLine, color in zip(dataLines, colors):
 			dataLine.set_color(color)
 
 @serializationReg.registerForSerialization()
 class SetLineMarkerSizes(plotCommCoreHelp.PlotCommand):
 
@@ -865,15 +982,15 @@
 		self._optName = "lineMarkerSizes"
 
 	def execute(self, plotterInstance):
 		targVal = getattr(plotterInstance.opts, self._optName).value
 		if targVal is None:
 			return None
 
-		dataLines = plt.gca().get_lines()
+		dataLines = _getScratchSpaceValueIfPresent(plotterInstance, "plotLineHandles", "value", retValIfNone=list())
 		try:
 			iter(targVal)
 		except TypeError:
 			useVal = it.cycle([targVal])
 		else:
 			useVal = it.cycle(targVal)
 
@@ -890,15 +1007,15 @@
 		self._optName = "lineMarkerStyles"
 
 	def execute(self, plotterInstance):
 		targVal = getattr(plotterInstance.opts, self._optName).value
 		if targVal is None:
 			return None
 
-		dataLines = plt.gca().get_lines()
+		dataLines = _getScratchSpaceValueIfPresent(plotterInstance, "plotLineHandles", "value", retValIfNone=list())
 		markerStyles = it.cycle(targVal)
 		for dataLine, markerStyle in zip(dataLines, markerStyles):
 			dataLine.set_marker(markerStyle)
 
 @serializationReg.registerForSerialization()
 class SetLineStyles(plotCommCoreHelp.PlotCommand):
 
@@ -908,15 +1025,19 @@
 		self._optName = "lineStyles"
 
 	def execute(self, plotterInstance):
 		targVal = getattr(plotterInstance.opts, self._optName).value
 		if targVal is None:
 			return None
 
-		dataLines = plt.gca().get_lines()
+		#
+		_defLinesVal = list()
+		dataLines = _getScratchSpaceValueIfPresent(plotterInstance, "plotLineHandles", "value", retValIfNone=_defLinesVal)
+
+
 		lineStyles = it.cycle(targVal)
 		for dataLine, lineStyle in zip(dataLines, lineStyles):
 			dataLine.set_linestyle(lineStyle)
 
 
 @serializationReg.registerForSerialization()
 class SetTickLabelFontSize(plotCommCoreHelp.PlotCommand):
@@ -1206,15 +1327,23 @@
 	def execute(self, plotterInstance):
 		targVal = getattr(plotterInstance.opts, self._optName).value
 		if targVal is None:
 			return None
 
 		legendKwargDict = plotterInstance._scratchSpace["legendKwargDict"]
 
+		#Need to pass data line handles explicitly if present, otherwise error bars can interfere
+		_defLinesVal = list()
+		dataLines = _getScratchSpaceValueIfPresent(plotterInstance, "plotLineHandles", "value")
+
+
 		if targVal is True:
+#			if dataLines is not None:
+#				plt.legend(dataLines,**legendKwargDict)
+#			else:
 			plt.legend(**legendKwargDict)
 
 
 
 #Some shared helper functions
 def _getDefaultFontSizeFromPlotter(plotterInstance):
 	try:
@@ -1249,8 +1378,22 @@
 		useDict = dict()
 		plotterInstance._scratchSpace[dictName] = useDict
 
 	#
 	useDict[key] = value
 
 
+def _getScratchSpaceValueIfPresent(plotterInstance, dictName, key, retValIfNone=None):
+	#Check for dictionary, and get key if present
+	try:
+		useDict = plotterInstance._scratchSpace[dictName]
+	except KeyError:
+		return retValIfNone
+
+	#Check for key in dictionary + return it if present
+	try:
+		outVal = useDict[key]
+	except KeyError:
+		return retValIfNone
+
+	return outVal
```

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/plot_options.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/plot_options.py`

 * *Files 13% similar despite different names*

```diff
@@ -230,14 +230,102 @@
 	""" Set the data labels for the plot. Values should be a list of strings, with None for any data you want left with the default label. e.g. ["seriesA", None, "seriesC"] should mean only 1st and 3rd appear in the legend
 
 	"""
 	def __init__(self, name=None, value=None):
 		self.name = "dataLabels" if name is None else name
 		self.value = value
 
+
+@serializationReg.registerForSerialization()
+class ErrorBarCapsize(plotOptCore.FloatIterPlotOption):
+	""" Float-iter. Controls the size of caps on error bars. These are passed to the capsize argument in matplotlib.
+
+	Note: The number of entries doesnt have to match the number of data series. If you provide too few entries, they will simply cycle. E.g. errorBarCapsize=[2.5] will cause error bars for ALL series to have capsizes of 2.5
+	"""
+	def __init__(self, name=None, value=None):
+		self.name = "errorBarCapsize" if name is None else name
+		self.value = value
+
+
+@serializationReg.registerForSerialization()
+class ErrorBarColors(plotOptCore.StringIterPlotOption):
+	""" The colors to use for error bars. Allowed strings are the same as in matplotlib, meaning special color names or hex rgb codes are both fine. For Example ['red','green','orange'] is a valid value
+
+	Note: The number of colors doesnt have to match the number of data series. If you provide too few colors, they will simply cycle. For example if you set ['red','green'] then plotted data would be [red, green, red, green,.... etc]
+
+	"""
+	def __init__(self, name=None, value=None):
+		self.name = "errorBarColors" if name is None else name
+		self.value = value
+
+
+@serializationReg.registerForSerialization()
+class ErrorBarColorsMatchLinesByDefault(plotOptCore.BooleanPlotOption):
+	""" Boolean. If True, then error bar colors will match plotted line colors by default.
+
+	Note, that this behavior can be overwritten by other options (e.g. errorBarColors option)
+
+	"""
+	def __init__(self, name=None, value=None):
+		self.name = "errorBarColorsMatchLinesByDefault" if name is None else name
+		self.value = value
+
+@serializationReg.registerForSerialization()
+class ErrorBarDataX(plotOptCore.NumpyIterPlotOption):
+	""" Data for error bars for the x-direction. None will lead to no error bars being plotted; else an iterable should be passed with one value per data series:
+
+	1) None - to not plot any error bars
+	2) nx1 array: where values are symmetric for each data point in the relevant plotData series
+	3) nx2 array: where values are [lowerBar, upperBar] around the central values
+
+	Notes:
+		a) If N values are passed for N-1 data series, the last will be ignored
+		b) If N-1 values are passed for N data series, the last data series will be plotted without any error bars
+
+	"""
+	def __init__(self, name=None, value=None):
+		self.name = "errorBarDataX" if name is None else name
+		self.value = value
+
+
+@serializationReg.registerForSerialization()
+class ErrorBarDataY(plotOptCore.NumpyIterPlotOption):
+	""" Data for error bars for the y-direction. None will lead to no error bars being plotted; else an iterable should be passed with one value per data series:
+
+	1) None - to not plot any error bars
+	2) nx1 array: where values are symmetric for each data point in the relevant plotData series
+	3) nx2 array: where values are [lowerBar, upperBar] around the central values
+
+	Notes:
+		a) If N values are passed for N-1 data series, the last will be ignored
+		b) If N-1 values are passed for N data series, the last data series will be plotted without any error bars
+
+	"""
+	def __init__(self, name=None, value=None):
+		self.name = "errorBarDataY" if name is None else name
+		self.value = value
+
+@serializationReg.registerForSerialization()
+class ErrorBarLineMplHooks(plotOptCore.ObjectIterPlotOption):
+	""" Dicts that get passed as keywords to plt.errorbar (assuming errorBarData is present) when making line plots
+
+	See the matplotlib documentation for valid keys/vals:
+
+	https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.errorbar.html
+
+	Notes:
+		a) Need to pass an iterable of dicts.
+		b) If there are more series than dicts, then values will cycle. This means you can pass a len-1 list (e.g. [dict()]) to use the same options for all
+
+	"""
+	def __init__(self, name=None, value=None):
+		self.name = "errorBarLineMplHooks" if name is None else name
+		self.value = value
+
+
 @serializationReg.registerForSerialization()
 class FontSizeDefault(plotOptCore.IntPlotOption):
 	""" The default font size to use for a figure. None will fall back on matplotlib value.
 
 	Valid values are integers (e.g. 10-ish is standard)
 
 	"""
```

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/plotters.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/plotters.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/bar_plotter.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/private/bar_plotter.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,14 +91,17 @@
 	plotOptStdHelp.AxisColorX(),
 	plotOptStdHelp.AxisColorX_exclSpines(),
 	plotOptStdHelp.AxisColorY(),
 	plotOptStdHelp.AxisColorY_exclSpines(),
 	plotOptStdHelp.BarColors(),
 	plotOptStdHelp.BarOpacities(),
 	plotOptStdHelp.DataLabels(),
+	plotOptStdHelp.ErrorBarCapsize(),
+	plotOptStdHelp.ErrorBarColors(),
+	ErrorBarData(),
 	plotOptStdHelp.FontSizeDefault(),
 	plotOptStdHelp.GridLinesShow(value=False),
 	plotOptStdHelp.GridLinesShowX(),
 	plotOptStdHelp.GridLinesShowY(),
 	plotOptStdHelp.GridLinesStyle(),
 	plotOptStdHelp.GridLinesWidth(),
 	GroupLabels(),
@@ -155,14 +158,32 @@
 	"""
 	def __init__(self, name=None, value=None):
 		self.name = "barLabels" if name is None else name
 		self.value = value
 
 
 @serializationReg.registerForSerialization()
+class ErrorBarData(plotOptCoreHelp.NumpyIterPlotOption):
+	""" Data for error bars. None will lead to no error bars being plotted; else an iterable should be passed with one value per data series:
+
+	1) None - to not plot any error bars
+	2) nx1 array: where values are symmetric for each data point in the relevant plotData series
+	3) nx2 array: where values are [lowerBar, upperBar] around the central values
+
+	Notes:
+		a) If N values are passed for N-1 data series, the last will be ignored
+		b) If N-1 values are passed for N data series, the last data series will be plotted without any error bars
+
+	"""
+
+	def __init__(self, name=None, value=None):
+		self.name = "errorBarData" if name is None else name
+		self.value = value
+
+@serializationReg.registerForSerialization()
 class GroupLabels(plotOptStdHelp.GroupLabels):
 
 	"""String iter. Each is a label for a group of bars; if your only plotting one data series then this means 1 label per value input. 
 
 	E.g. If plotting years vs population this might be ["1970", "1980", "1990"]
 
 	"""
@@ -436,14 +457,17 @@
 		allCentres = plotterInstance._scratchSpace["centres"]
 		allBottoms = plotterInstance._scratchSpace["bottom_vals"]
 
 		#Figure out the bar widths
 		barWidth = plotterInstance.opts.widthBars.value
 		barWidth = 1.0 if barWidth is None else barWidth
 
+		#Figure out any options for plotting error bars - this includes doing things like reversing order
+		# and figuring out if error bars are along x or y
+		allErrorBars = self._getErrorBarOpts(plotterInstance)
 
 		#Optionally reverse the order the bars are plotted in
 		reverseIntraOrdering = getattr(plotterInstance.opts, "reverseIntraBarOrdering").value
 
 		#Plot the data; may want to return handles to scratch space later
 		outBars = list()
 		for idx,currData in enumerate(targVal):
@@ -454,25 +478,67 @@
 			else:
 				centres = allCentres[idx]
 				bottoms = allBottoms[idx]
 
 			useCentres = [centre for centre,val in zip(centres,currData) if val is not None]
 			useBottoms = [bottom for bottom,val in zip(bottoms,currData) if val is not None]
 			useData = [val for val in currData if val is not None]
+			useErrorBarOpts = allErrorBars[idx]
 
 			if plotHoz:
-				currBars = plt.barh( np.array(useCentres), np.array(useData), height=barWidth, left=np.array(useBottoms) )
+				currBars = plt.barh( np.array(useCentres), np.array(useData), height=barWidth, left=np.array(useBottoms), **useErrorBarOpts )
 			else:
-				currBars = plt.bar( np.array(useCentres), np.array(useData), width=barWidth, bottom=np.array(useBottoms) )
+				currBars = plt.bar( np.array(useCentres), np.array(useData), width=barWidth, bottom=np.array(useBottoms), **useErrorBarOpts )
 
 			outBars.append(currBars)
 
 		plotterInstance._scratchSpace["barHandles"] = outBars
 		return
 
+	def _getErrorBarOpts(self, plotterInstance):
+		#
+		barCentres = plotterInstance._scratchSpace["centres"]
+
+		#
+		errorBarData = plotCmdStdHelp._getValueFromOptName(plotterInstance, "errorBarData")
+		if errorBarData is None:
+			return [dict() for x in barCentres]
+
+		#Sort out the data if its present
+		outDicts = [dict() for x in barCentres]
+		dataKwarg = self._getErrorBarDirectionKey(plotterInstance)
+		for idx,data in enumerate(errorBarData):
+			if data is not None:
+				outDicts[idx][dataKwarg] = data
+
+		#If colors are present, use them cyclically
+		errorBarColors = plotCmdStdHelp._getValueFromOptName(plotterInstance, "errorBarColors")
+		if errorBarColors is not None:
+			useColors = it.cycle(errorBarColors)
+			for idx,(data,color) in enumerate( zip(errorBarData, useColors) ):
+				if color is not None:
+					outDicts[idx]["ecolor"] = color
+
+		#Set the capsizes if present
+		capsizeVals = plotCmdStdHelp._getValueFromOptName(plotterInstance, "errorBarCapsize")
+		if capsizeVals is not None:
+			useCapsizes = it.cycle(capsizeVals)
+			for idx,(data,capsize) in enumerate( zip(errorBarData,useCapsizes) ):
+				outDicts[idx]["capsize"] = capsize
+
+		return outDicts
+
+	def _getErrorBarDirectionKey(self, plotterInstance):
+		plotHoz = plotterInstance.opts.plotHorizontally.value
+		if plotHoz is True:
+			return "xerr"
+		else:
+			return "yerr"
+
+
 @serializationReg.registerForSerialization()
 class SetBarDataLabels(plotCmdStdHelp.SetBarDataLabels):
 	pass
 
 @serializationReg.registerForSerialization()
 class SetTickMinorValsOnOrOff(plotCommCoreHelp.PlotCommand):
```

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/box_plotter.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/private/box_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/disc_heat_plotter.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/private/disc_heat_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/histogram_plotter.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/private/histogram_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/image_plotter.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/private/image_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/line_plotter.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/private/line_plotter.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,21 +36,23 @@
 
 
 
 #Less indenting required this way
 def _createCommandsList():
 	outList = [
 	plotCmdStdHelp.CreateFigureIfNoAxHandle(),
+	plotCmdStdHelp.AddPlotterToOutput(),
 	plotCmdStdHelp.PlotDataAsLines(),
 	plotCmdStdHelp.GridLinesCreate(),
 	plotCmdStdHelp.SetDataLabels(),
 	plotCmdStdHelp.SetLineColors(),
 	plotCmdStdHelp.SetLineMarkerSizes(),
 	plotCmdStdHelp.SetLineMarkerStyles(),
 	plotCmdStdHelp.SetLineStyles(),
+	plotCmdStdHelp.SetLineErrorBarColors(),
 	plotCmdStdHelp.SetXLabelStr(),
 	plotCmdStdHelp.SetYLabelStr(),
 	plotCmdStdHelp.SetAxisScaleX(),
 	plotCmdStdHelp.SetAxisScaleY(),
 	plotCmdStdHelp.SetTickMarkerValues(),
 	plotCmdStdHelp.SetTickLabelValues(),
 	plotCmdStdHelp.SetTickLabelFontSize(),
@@ -65,14 +67,15 @@
 	plotCmdStdHelp.SetAxisColorY(),
 	plotCmdStdHelp.SetAxisBorderInvisible(),
 	plotCmdStdHelp.SetTitleStr(),
 	plotCmdStdHelp.SetLegendLocStr(),
 	plotCmdStdHelp.SetLegendFontSize(),
 	plotCmdStdHelp.SetLegendFractPosStart(),
 	plotCmdStdHelp.SetLegendNumberColumns(),
+	plotCmdStdHelp.SetLegendHandlesToPlottedLinesDefault(),
 	plotCmdStdHelp.PlotHozAndVertLines(),
 	plotCmdStdHelp.TurnLegendOnIfRequested(),
 	plotCmdStdHelp.DrawShadedAnnotationsGeneric(),
 	plotCmdStdHelp.DrawTextAnnotationsGeneric()
 	]
 
 	return outList
@@ -86,14 +89,20 @@
 	plotOptStdHelp.AxisColorX(),
 	plotOptStdHelp.AxisColorX_exclSpines(),
 	plotOptStdHelp.AxisColorY(),
 	plotOptStdHelp.AxisColorY_exclSpines(),
 	plotOptStdHelp.AxisScaleX(),
 	plotOptStdHelp.AxisScaleY(),
 	plotOptStdHelp.DataLabels(),
+	plotOptStdHelp.ErrorBarCapsize(),
+	plotOptStdHelp.ErrorBarColors(),
+	plotOptStdHelp.ErrorBarColorsMatchLinesByDefault(value=True),
+    plotOptStdHelp.ErrorBarDataX(),
+    plotOptStdHelp.ErrorBarDataY(),
+    plotOptStdHelp.ErrorBarLineMplHooks(),
 	plotOptStdHelp.FontSizeDefault(),
 	plotOptStdHelp.GridLinesShow(value=False),
 	plotOptStdHelp.GridLinesShowX(),
 	plotOptStdHelp.GridLinesShowY(),
 	plotOptStdHelp.GridLinesStyle(),
 	plotOptStdHelp.GridLinesWidth(),
 	plotOptStdHelp.LegendFractPosStart(),
```

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/rect_multi_plotter.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/private/rect_multi_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/shared.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/private/shared.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/shared_axis_plotter.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/private/shared_axis_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/split_axis_plotter.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/private/split_axis_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/split_axis_plotter_creator.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/private/split_axis_plotter_creator.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/unit_tests/utests_histogram_plotter.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/private/unit_tests/utests_histogram_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/serialization.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/serialization.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_bar_plotter.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/serialization/utests_bar_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_histogram_plotter.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/serialization/utests_histogram_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_image_plotter.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/serialization/utests_image_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_line_plotter.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/serialization/utests_line_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_rect_multi_plotter.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/serialization/utests_rect_multi_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_shared_axis_plotter.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/serialization/utests_shared_axis_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_creator.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_creator.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_plotter.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/utests_plot_commands.py` & `pyplotterlib-1.7.0/src/pyplotterlib/standard/unit_tests/utests_plot_commands.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib.egg-info/PKG-INFO` & `pyplotterlib-1.7.0/src/pyplotterlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplotterlib
-Version: 1.6.0
+Version: 1.7.0
 Summary: A package used to create plots in python
 Author-email: Richard Fogarty <richard.m.fogarty@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 RFogarty1
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyplotterlib-1.6.0/src/pyplotterlib.egg-info/SOURCES.txt` & `pyplotterlib-1.7.0/src/pyplotterlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

