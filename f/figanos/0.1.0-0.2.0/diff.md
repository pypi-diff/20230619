# Comparing `tmp/figanos-0.1.0.tar.gz` & `tmp/figanos-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "figanos-0.1.0.tar", last modified: Fri Jun  9 19:54:02 2023, max compression
+gzip compressed data, was "figanos-0.2.0.tar", last modified: Mon Jun 19 19:02:56 2023, max compression
```

## Comparing `figanos-0.1.0.tar` & `figanos-0.2.0.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-06-09 19:54:02.681818 figanos-0.1.0/
--rw-r--r--   0 tjs       (1000) tjs       (1000)      519 2023-03-21 15:22:44.000000 figanos-0.1.0/AUTHORS.rst
--rw-r--r--   0 tjs       (1000) tjs       (1000)     7194 2023-06-09 19:24:09.000000 figanos-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 tjs       (1000) tjs       (1000)       89 2023-03-21 15:22:44.000000 figanos-0.1.0/HISTORY.rst
--rw-r--r--   0 tjs       (1000) tjs       (1000)      590 2023-03-20 18:25:30.000000 figanos-0.1.0/LICENSE
--rw-r--r--   0 tjs       (1000) tjs       (1000)      618 2023-06-09 19:24:09.000000 figanos-0.1.0/MANIFEST.in
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2286 2023-06-09 19:54:02.681818 figanos-0.1.0/PKG-INFO
--rw-r--r--   0 tjs       (1000) tjs       (1000)     1115 2023-06-09 19:24:09.000000 figanos-0.1.0/README.rst
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-06-09 19:54:02.669818 figanos-0.1.0/docs/
--rw-r--r--   0 tjs       (1000) tjs       (1000)      608 2023-06-09 19:24:09.000000 figanos-0.1.0/docs/Makefile
--rw-r--r--   0 tjs       (1000) tjs       (1000)       98 2023-06-09 19:24:09.000000 figanos-0.1.0/docs/api.rst
--rw-r--r--   0 tjs       (1000) tjs       (1000)       28 2023-03-20 18:25:30.000000 figanos-0.1.0/docs/authors.rst
--rwxr-xr-x   0 tjs       (1000) tjs       (1000)     5187 2023-06-09 19:24:09.000000 figanos-0.1.0/docs/conf.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)       33 2023-03-20 18:25:30.000000 figanos-0.1.0/docs/contributing.rst
--rw-r--r--   0 tjs       (1000) tjs       (1000)       28 2023-03-20 18:25:30.000000 figanos-0.1.0/docs/history.rst
--rw-r--r--   0 tjs       (1000) tjs       (1000)      370 2023-06-09 19:24:09.000000 figanos-0.1.0/docs/index.rst
--rw-r--r--   0 tjs       (1000) tjs       (1000)     1693 2023-06-09 19:24:09.000000 figanos-0.1.0/docs/installation.rst
--rw-r--r--   0 tjs       (1000) tjs       (1000)      769 2023-06-09 19:24:09.000000 figanos-0.1.0/docs/make.bat
--rw-r--r--   0 tjs       (1000) tjs       (1000)       27 2023-03-20 18:25:30.000000 figanos-0.1.0/docs/readme.rst
--rw-r--r--   0 tjs       (1000) tjs       (1000)      123 2023-06-09 19:24:09.000000 figanos-0.1.0/docs/usage.rst
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-06-09 19:54:02.670818 figanos-0.1.0/figanos/
--rw-r--r--   0 tjs       (1000) tjs       (1000)      188 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/__init__.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)      418 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/cli.py
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-06-09 19:54:02.672818 figanos-0.1.0/figanos/data/
--rw-r--r--   0 tjs       (1000) tjs       (1000)     1134 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/colors.json
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-06-09 19:54:02.673818 figanos-0.1.0/figanos/data/ipcc_colors/
--rw-r--r--   0 tjs       (1000) tjs       (1000)      118 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/README.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)     1924 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/categorical_colors.json
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-06-09 19:54:02.676818 figanos-0.1.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/
--rw-r--r--   0 tjs       (1000) tjs       (1000)       65 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/bright_cat.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)       61 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/chem_cat.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)       20 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/cmip_cat.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)       40 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/contrast_cat.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)       82 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/dark_cat.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)       66 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/gree-blue_cat.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)       39 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/rcp_cat.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)       52 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/red-yellow_cat.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)       75 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/spectrum_cat.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)       54 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/ssp_cat_1.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)       61 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/ssp_cat_2.txt
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-06-09 19:54:02.679818 figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2855 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/chem_div.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2878 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/chem_seq.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2795 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/cryo_div.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2722 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/cryo_seq.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2793 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/misc_div.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2851 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/misc_seq_1.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2866 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/misc_seq_2.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2684 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/misc_seq_3.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2821 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/prec_div.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2813 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/prec_seq.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2861 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/slev_div.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2838 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/slev_seq.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2852 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/temp_div.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2702 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/temp_seq.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2788 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/wind_div.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2644 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/wind_seq.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)      587 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/data/ipcc_colors/variable_groups.json
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-06-09 19:54:02.680818 figanos-0.1.0/figanos/matplotlib/
--rw-r--r--   0 tjs       (1000) tjs       (1000)      200 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/matplotlib/__init__.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)    64110 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/matplotlib/plot.py
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-06-09 19:54:02.681818 figanos-0.1.0/figanos/matplotlib/style/
--rw-r--r--   0 tjs       (1000) tjs       (1000)     1469 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/matplotlib/style/ouranos.mplstyle
--rw-r--r--   0 tjs       (1000) tjs       (1000)      442 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/matplotlib/style/paper.mplstyle
--rw-r--r--   0 tjs       (1000) tjs       (1000)      453 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/matplotlib/style/poster.mplstyle
--rw-r--r--   0 tjs       (1000) tjs       (1000)    33548 2023-06-09 19:24:09.000000 figanos-0.1.0/figanos/matplotlib/utils.py
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-06-09 19:54:02.672818 figanos-0.1.0/figanos.egg-info/
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2286 2023-06-09 19:54:02.000000 figanos-0.1.0/figanos.egg-info/PKG-INFO
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2820 2023-06-09 19:54:02.000000 figanos-0.1.0/figanos.egg-info/SOURCES.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)        1 2023-06-09 19:54:02.000000 figanos-0.1.0/figanos.egg-info/dependency_links.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)       45 2023-06-09 19:54:02.000000 figanos-0.1.0/figanos.egg-info/entry_points.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)        1 2023-06-09 19:52:19.000000 figanos-0.1.0/figanos.egg-info/not-zip-safe
--rw-r--r--   0 tjs       (1000) tjs       (1000)      501 2023-06-09 19:54:02.000000 figanos-0.1.0/figanos.egg-info/requires.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)        8 2023-06-09 19:54:02.000000 figanos-0.1.0/figanos.egg-info/top_level.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)      219 2023-06-07 18:49:01.000000 figanos-0.1.0/requirements_dev.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)      129 2023-06-09 19:24:09.000000 figanos-0.1.0/requirements_docs.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)     1018 2023-06-09 19:54:02.682818 figanos-0.1.0/setup.cfg
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2294 2023-06-09 19:24:09.000000 figanos-0.1.0/setup.py
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-06-09 19:54:02.681818 figanos-0.1.0/tests/
--rw-r--r--   0 tjs       (1000) tjs       (1000)      930 2023-06-09 19:24:09.000000 figanos-0.1.0/tests/test_figanos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:02:56.396637 figanos-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-19 19:02:53.000000 figanos-0.2.0/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-19 19:02:53.000000 figanos-0.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-06-19 19:02:53.000000 figanos-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-19 19:02:53.000000 figanos-0.2.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-19 19:02:53.000000 figanos-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 19:02:53.000000 figanos-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-19 19:02:56.396637 figanos-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-19 19:02:53.000000 figanos-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:02:56.384637 figanos-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-19 19:02:53.000000 figanos-0.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:02:56.376637 figanos-0.2.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:02:56.384637 figanos-0.2.0/docs/_static/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)    12758 2023-06-19 19:02:53.000000 figanos-0.2.0/docs/_static/_images/figanos_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-19 19:02:53.000000 figanos-0.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 19:02:53.000000 figanos-0.2.0/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5673 2023-06-19 19:02:53.000000 figanos-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-19 19:02:53.000000 figanos-0.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 19:02:53.000000 figanos-0.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-19 19:02:53.000000 figanos-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-19 19:02:53.000000 figanos-0.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-19 19:02:53.000000 figanos-0.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-19 19:02:53.000000 figanos-0.2.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:02:56.384637 figanos-0.2.0/figanos/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:02:56.388637 figanos-0.2.0/figanos/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/colors.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:02:56.388637 figanos-0.2.0/figanos/data/ipcc_colors/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/categorical_colors.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:02:56.392637 figanos-0.2.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/bright_cat.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/chem_cat.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/cmip_cat.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/contrast_cat.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/dark_cat.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/gree-blue_cat.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/rcp_cat.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/red-yellow_cat.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/spectrum_cat.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/ssp_cat_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/categorical_colors_rgb_0-255/ssp_cat_2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:02:56.396637 figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/chem_div.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/chem_seq.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/cryo_div.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/cryo_seq.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/misc_div.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/misc_seq_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/misc_seq_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/misc_seq_3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/prec_div.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/prec_seq.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/slev_div.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/slev_seq.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/temp_div.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/temp_seq.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/wind_div.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/wind_seq.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/data/ipcc_colors/variable_groups.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:02:56.396637 figanos-0.2.0/figanos/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64110 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/matplotlib/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:02:56.396637 figanos-0.2.0/figanos/matplotlib/style/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/matplotlib/style/ouranos.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/matplotlib/style/paper.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/matplotlib/style/poster.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)    33548 2023-06-19 19:02:53.000000 figanos-0.2.0/figanos/matplotlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:02:56.388637 figanos-0.2.0/figanos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-19 19:02:56.000000 figanos-0.2.0/figanos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-19 19:02:56.000000 figanos-0.2.0/figanos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:02:56.000000 figanos-0.2.0/figanos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 19:02:56.000000 figanos-0.2.0/figanos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:02:56.000000 figanos-0.2.0/figanos.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-19 19:02:56.000000 figanos-0.2.0/figanos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 19:02:56.000000 figanos-0.2.0/figanos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-19 19:02:53.000000 figanos-0.2.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-19 19:02:53.000000 figanos-0.2.0/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-19 19:02:56.396637 figanos-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-19 19:02:53.000000 figanos-0.2.0/setup.py
```

### Comparing `figanos-0.1.0/AUTHORS.rst` & `figanos-0.2.0/AUTHORS.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 =======
 Credits
 =======
 
 Development Lead
 ----------------
 
-* Sarah-Claude Bourdeau-Goulet <bourdeau-goulet.sarah-claude@ouranos.ca> `@sarahclaude <https://github.com/sarahclaude>`_
+* Sarah-Claude Bourdeau-Goulet <bourdeau-goulet.sarah-claude@ouranos.ca> `@Sarahclaude <https://github.com/Sarahclaude>`_
 
-Contributors
-------------
+Co-Developers
+-------------
 
 * Trevor James Smith <smith.trevorj@ouranos.ca> `@Zeitsperre <https://github.com/Zeitsperre>`_
 * Alexis Beaupré-Laperrière <Beaupre-Laperriere.Alexis@ouranos.ca> `@Beauprel <https://github.com/Beauprel>`_
 * Juliette Lavoie <lavoie.juliette@ouranos.ca> `@juliettelavoie <https://github.com/juliettelavoie>`_
```

### Comparing `figanos-0.1.0/CONTRIBUTING.rst` & `figanos-0.2.0/CONTRIBUTING.rst`

 * *Files 4% similar despite different names*

```diff
@@ -115,17 +115,15 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.rst.
-3. The pull request should work for Python 3.7, 3.8, 3.9, and 3.10. Check
-   https://github.com/Ouranosinc/figanos/pulls
-   and make sure that the tests pass for all supported Python versions.
+3. The pull request should work for all major supported Python versions (3.8, 3.9, 3.10, and 3.11).
 
 Tips
 ----
 
 To run a subset of tests::
 
 $ pytest tests.test_figanos
@@ -148,22 +146,23 @@
 When a new version has been minted (features have been successfully integrated test coverage and stability is adequate),
 maintainers should update the pip-installable package (wheel and source release) on PyPI as well as the binary on conda-forge.
 
 The simple approach
 ~~~~~~~~~~~~~~~~~~~
 
 The simplest approach to packaging for general support (pip wheels) requires the following packages installed:
+ * build
  * setuptools
- * wheel
  * twine
+ * wheel
 
 From the command line on your Linux distribution, simply run the following from the clone's main dev branch::
 
     # To build the packages (sources and wheel)
-    $ python setup.py sdist bdist_wheel
+    $ python -m build --sdist --wheel
 
     # To upload to PyPI
     $ twine upload dist/*
 
 The new version based off of the version checked out will now be available via `pip` (`$ pip install figanos`).
 
 Releasing on conda-forge
@@ -200,15 +199,15 @@
 
     $ sudo docker pull quay.io/pypa/manylinux_2_24_x86_64
 
 From the figanos source folder we can enter into the docker container, providing access to the `figanos` source files by linking them to the running image::
 
     $ sudo docker run --rm -ti -v $(pwd):/figanos -w /figanos quay.io/pypa/manylinux_2_24_x86_64 bash
 
-Finally, to build the wheel, we run it against the provided Python3.7 binary::
+Finally, to build the wheel, we run it against the provided Python3.8 binary::
 
-    $ /opt/python/cp37-cp37m/bin/python setup.py sdist bdist_wheel
+    $ /opt/python/cp38-cp38m/bin/python setup.py sdist bdist_wheel
 
 This will then place two files in `figanos/dist/` ("figanos-1.2.3-py3-none-any.whl" and "figanos-1.2.3.tar.gz").
 We can now leave our docker container (`$ exit`) and continue with uploading the files to PyPI::
 
     $ twine upload dist/*
```

### Comparing `figanos-0.1.0/LICENSE` & `figanos-0.2.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 Apache Software License 2.0
 
 Copyright (c) 2022, Trevor James Smith
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `figanos-0.1.0/MANIFEST.in` & `figanos-0.2.0/MANIFEST.in`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 include AUTHORS.rst
 include CONTRIBUTING.rst
 include HISTORY.rst
 include LICENSE
 include README.rst
+include .zenodo.json
 include requirements_dev.txt
 include requirements_docs.txt
 
 recursive-include figanos *.json *.mplstyle *.py *.txt
 recursive-include docs *.rst conf.py Makefile make.bat *.jpg *.png *.gif
 recursive-include data *.json *.txt
```

### Comparing `figanos-0.1.0/PKG-INFO` & `figanos-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,79 @@
 Metadata-Version: 2.1
 Name: figanos
-Version: 0.1.0
+Version: 0.2.0
 Summary: Outils pour produire des graphiques informatifs sur les impacts des changements climatiques.
 Author: Sarah-Claude Bourdeau-Goulet
 Author-email: bourdeau-goulet.sarah-claude@ouranos.ca
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/Ouranosinc/figanos
 Project-URL: Issue tracker, https://github.com/Ouranosinc/figanos/issues
 Project-URL: About Ouranos, https://www.ouranos.ca/en/
 Keywords: figanos
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS.rst
 
-==========
+=======
 figanos
-==========
+=======
 
 
 .. image:: https://img.shields.io/pypi/v/figanos.svg
         :target: https://pypi.python.org/pypi/figanos
+        :alt: PyPI
 
-.. image:: https://img.shields.io/travis/Zeitsperre/figanos.svg
-        :target: https://travis-ci.com/Zeitsperre/figanos
+.. image:: https://github.com/Ouranosinc/figanos/actions/workflows/main.yml/badge.svg
+        :target: https://github.com/Ouranosinc/figanos/actions
+        :alt: Build Status
 
 .. image:: https://readthedocs.org/projects/figanos/badge/?version=latest
         :target: https://figanos.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
+.. image:: https://img.shields.io/pypi/l/figanos
+        :target: https://github.com/Ouranosinc/figanos/blob/main/LICENSE
+        :alt: License
+
+Figanos: Tool to create FIGures in the OurANOS style
 
-Outils pour produire des graphiques informatifs sur les impacts des changements climatiques.
 
 Pour nous partager vos codes à ajouter dans figanos, s.v.p créer un issue sur le repo github avec une description de la fonction et
 le code de celle-ci.
 
 
 * Free software: Apache Software License 2.0
 * Documentation: https://figanos.readthedocs.io.
 
 
 Features
 --------
 
-* TODO
+* timeseries(): Creates time series as line plots.
+* gridmap(): Plots gridded georeferenced data on a map.
+* scattermap(): Make a scatter plot of georeferenced data on a map.
+* gdfmap(): Plots geometries (through a GeoDataFrame) on a map.
+* stripes(): Create climate stripe diagrams.
+* violin(): Create seaborn violin plots with extra options.
+* heatmap(): Create seaborn heatmaps with extra options.
+* taylordiagram(): Create Taylor diagram.
+
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `Ouranosinc/cookiecutter-pypackage`_ project template.
 
-.. _Cookiecutter: https://github.com/audreyfeldroy/cookiecutter-pypackage
+.. _Cookiecutter: https://github.com/cookiecutter/cookiecutter
 .. _`Ouranosinc/cookiecutter-pypackage`: https://github.com/Ouranosinc/cookiecutter-pypackage
-
-
-=======
-History
-=======
-
-0.1.0 (unreleased)
-------------------
-
-* First release on PyPI.
```

### Comparing `figanos-0.1.0/README.rst` & `figanos-0.2.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,52 @@
-==========
+=======
 figanos
-==========
+=======
 
 
 .. image:: https://img.shields.io/pypi/v/figanos.svg
         :target: https://pypi.python.org/pypi/figanos
+        :alt: PyPI
 
-.. image:: https://img.shields.io/travis/Zeitsperre/figanos.svg
-        :target: https://travis-ci.com/Zeitsperre/figanos
+.. image:: https://github.com/Ouranosinc/figanos/actions/workflows/main.yml/badge.svg
+        :target: https://github.com/Ouranosinc/figanos/actions
+        :alt: Build Status
 
 .. image:: https://readthedocs.org/projects/figanos/badge/?version=latest
         :target: https://figanos.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
+.. image:: https://img.shields.io/pypi/l/figanos
+        :target: https://github.com/Ouranosinc/figanos/blob/main/LICENSE
+        :alt: License
+
+Figanos: Tool to create FIGures in the OurANOS style
 
-Outils pour produire des graphiques informatifs sur les impacts des changements climatiques.
 
 Pour nous partager vos codes à ajouter dans figanos, s.v.p créer un issue sur le repo github avec une description de la fonction et
 le code de celle-ci.
 
 
 * Free software: Apache Software License 2.0
 * Documentation: https://figanos.readthedocs.io.
 
 
 Features
 --------
 
-* TODO
+* timeseries(): Creates time series as line plots.
+* gridmap(): Plots gridded georeferenced data on a map.
+* scattermap(): Make a scatter plot of georeferenced data on a map.
+* gdfmap(): Plots geometries (through a GeoDataFrame) on a map.
+* stripes(): Create climate stripe diagrams.
+* violin(): Create seaborn violin plots with extra options.
+* heatmap(): Create seaborn heatmaps with extra options.
+* taylordiagram(): Create Taylor diagram.
+
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `Ouranosinc/cookiecutter-pypackage`_ project template.
 
-.. _Cookiecutter: https://github.com/audreyfeldroy/cookiecutter-pypackage
+.. _Cookiecutter: https://github.com/cookiecutter/cookiecutter
 .. _`Ouranosinc/cookiecutter-pypackage`: https://github.com/Ouranosinc/cookiecutter-pypackage
```

### Comparing `figanos-0.1.0/docs/Makefile` & `figanos-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/docs/conf.py` & `figanos-0.2.0/docs/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,24 +29,42 @@
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode', 'nbsphinx']
+extensions = [
+    'sphinx.ext.autodoc',
+    'sphinx.ext.autosectionlabel',
+    'sphinx.ext.extlinks',
+    'sphinx.ext.viewcode',
+    'sphinx.ext.todo',
+    'nbsphinx',
+    'sphinx_codeautolink',
+    'sphinx_copybutton'
+]
+
+autosectionlabel_prefix_document = True
+autosectionlabel_maxdepth = 2
 
 # To ensure that underlined fields (e.g. `_field`) are shown in the docs.
 autodoc_default_options = {
     "members": True,
     "undoc-members": True,
     "private-members": False,
     "special-members": False,
 }
 
+extlinks = {
+    "issue": ("https://github.com/Ouranosinc/figanos/issues/%s", "GH/%s"),
+    "pull": ("https://github.com/Ouranosinc/figanos/pull/%s", "PR/%s"),
+    "user": ("https://github.com/%s", "@%s"),
+}
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
@@ -89,16 +107,17 @@
 
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'alabaster'
+html_theme = 'sphinx_book_theme'
 
+html_logo = "_static/_images/figanos_logo.png"
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
```

### Comparing `figanos-0.1.0/docs/make.bat` & `figanos-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos/data/colors.json` & `figanos-0.2.0/figanos/data/colors.json`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos/data/ipcc_colors/categorical_colors.json` & `figanos-0.2.0/figanos/data/ipcc_colors/categorical_colors.json`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/chem_div.txt` & `figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/chem_div.txt`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/chem_seq.txt` & `figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/chem_seq.txt`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/cryo_div.txt` & `figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/cryo_div.txt`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/cryo_seq.txt` & `figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/cryo_seq.txt`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/misc_div.txt` & `figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/misc_div.txt`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/misc_seq_1.txt` & `figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/misc_seq_1.txt`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/misc_seq_2.txt` & `figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/misc_seq_2.txt`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/misc_seq_3.txt` & `figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/misc_seq_3.txt`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/prec_div.txt` & `figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/prec_div.txt`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/prec_seq.txt` & `figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/prec_seq.txt`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/slev_div.txt` & `figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/slev_div.txt`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/slev_seq.txt` & `figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/slev_seq.txt`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/temp_div.txt` & `figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/temp_div.txt`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/temp_seq.txt` & `figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/temp_seq.txt`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/wind_div.txt` & `figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/wind_div.txt`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/wind_seq.txt` & `figanos-0.2.0/figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/wind_seq.txt`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos/data/ipcc_colors/variable_groups.json` & `figanos-0.2.0/figanos/data/ipcc_colors/variable_groups.json`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos/matplotlib/plot.py` & `figanos-0.2.0/figanos/matplotlib/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -628,16 +628,15 @@
     features: list[str] | dict[str, dict[str, Any]] | None = None,
     cmap: str | matplotlib.colors.Colormap | None = None,
     levels: int | list[int | float] | None = None,
     divergent: bool | int | float = False,
     cbar: bool = True,
     frame: bool = False,
 ) -> matplotlib.axes.Axes:
-    """
-    Create a map plot from geometries.
+    """Create a map plot from geometries.
 
     Parameters
     ----------
     df : geopandas.GeoDataFrame
         Dataframe containing the geometries and the data to plot. Must have a column named 'geometry'.
     df_col : str
         Name of the column of 'df' containing the data to plot using the colorscale.
@@ -1247,15 +1246,16 @@
     levels: int | None = None,
     divergent: bool | int | float = False,
     cbar_kw: dict[str, Any] | None = None,
     legend_kw: dict[str, Any] | None = None,
     show_time: bool | str | int | tuple[float, float] = False,
     frame: bool = False,
 ) -> matplotlib.axes.Axes:
-    """Make a scatter plot of georeferenced data on a map.
+    """
+    Make a scatter plot of georeferenced data on a map.
 
     Parameters
     ----------
     data : dict, DataArray or Dataset
         Input data do plot. If dictionary, must have only one entry.
         If a Dataset with multiple variables, the first one will be plotted against the colormap.
     ax : matplotlib axis, optional
```

### Comparing `figanos-0.1.0/figanos/matplotlib/style/ouranos.mplstyle` & `figanos-0.2.0/figanos/matplotlib/style/ouranos.mplstyle`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos/matplotlib/utils.py` & `figanos-0.2.0/figanos/matplotlib/utils.py`

 * *Files identical despite different names*

### Comparing `figanos-0.1.0/figanos.egg-info/PKG-INFO` & `figanos-0.2.0/figanos.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,79 @@
 Metadata-Version: 2.1
 Name: figanos
-Version: 0.1.0
+Version: 0.2.0
 Summary: Outils pour produire des graphiques informatifs sur les impacts des changements climatiques.
 Author: Sarah-Claude Bourdeau-Goulet
 Author-email: bourdeau-goulet.sarah-claude@ouranos.ca
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/Ouranosinc/figanos
 Project-URL: Issue tracker, https://github.com/Ouranosinc/figanos/issues
 Project-URL: About Ouranos, https://www.ouranos.ca/en/
 Keywords: figanos
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS.rst
 
-==========
+=======
 figanos
-==========
+=======
 
 
 .. image:: https://img.shields.io/pypi/v/figanos.svg
         :target: https://pypi.python.org/pypi/figanos
+        :alt: PyPI
 
-.. image:: https://img.shields.io/travis/Zeitsperre/figanos.svg
-        :target: https://travis-ci.com/Zeitsperre/figanos
+.. image:: https://github.com/Ouranosinc/figanos/actions/workflows/main.yml/badge.svg
+        :target: https://github.com/Ouranosinc/figanos/actions
+        :alt: Build Status
 
 .. image:: https://readthedocs.org/projects/figanos/badge/?version=latest
         :target: https://figanos.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
+.. image:: https://img.shields.io/pypi/l/figanos
+        :target: https://github.com/Ouranosinc/figanos/blob/main/LICENSE
+        :alt: License
+
+Figanos: Tool to create FIGures in the OurANOS style
 
-Outils pour produire des graphiques informatifs sur les impacts des changements climatiques.
 
 Pour nous partager vos codes à ajouter dans figanos, s.v.p créer un issue sur le repo github avec une description de la fonction et
 le code de celle-ci.
 
 
 * Free software: Apache Software License 2.0
 * Documentation: https://figanos.readthedocs.io.
 
 
 Features
 --------
 
-* TODO
+* timeseries(): Creates time series as line plots.
+* gridmap(): Plots gridded georeferenced data on a map.
+* scattermap(): Make a scatter plot of georeferenced data on a map.
+* gdfmap(): Plots geometries (through a GeoDataFrame) on a map.
+* stripes(): Create climate stripe diagrams.
+* violin(): Create seaborn violin plots with extra options.
+* heatmap(): Create seaborn heatmaps with extra options.
+* taylordiagram(): Create Taylor diagram.
+
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `Ouranosinc/cookiecutter-pypackage`_ project template.
 
-.. _Cookiecutter: https://github.com/audreyfeldroy/cookiecutter-pypackage
+.. _Cookiecutter: https://github.com/cookiecutter/cookiecutter
 .. _`Ouranosinc/cookiecutter-pypackage`: https://github.com/Ouranosinc/cookiecutter-pypackage
-
-
-=======
-History
-=======
-
-0.1.0 (unreleased)
-------------------
-
-* First release on PyPI.
```

### Comparing `figanos-0.1.0/figanos.egg-info/SOURCES.txt` & `figanos-0.2.0/figanos.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.zenodo.json
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
 requirements_dev.txt
@@ -13,16 +14,16 @@
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
-docs/readme.rst
 docs/usage.rst
+docs/_static/_images/figanos_logo.png
 figanos/__init__.py
 figanos/cli.py
 figanos.egg-info/PKG-INFO
 figanos.egg-info/SOURCES.txt
 figanos.egg-info/dependency_links.txt
 figanos.egg-info/entry_points.txt
 figanos.egg-info/not-zip-safe
@@ -60,9 +61,8 @@
 figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/wind_div.txt
 figanos/data/ipcc_colors/continuous_colormaps_rgb_0-255/wind_seq.txt
 figanos/matplotlib/__init__.py
 figanos/matplotlib/plot.py
 figanos/matplotlib/utils.py
 figanos/matplotlib/style/ouranos.mplstyle
 figanos/matplotlib/style/paper.mplstyle
-figanos/matplotlib/style/poster.mplstyle
-tests/test_figanos.py
+figanos/matplotlib/style/poster.mplstyle
```

### Comparing `figanos-0.1.0/setup.cfg` & `figanos-0.2.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 [bumpversion]
-current_version = 0.1.0
+current_version = 0.2.0
 commit = True
-tag = True
+tag = False
 
 [bumpversion:file:setup.py]
-search = version='{current_version}'
-replace = version='{new_version}'
+search = version="{current_version}"
+replace = version="{new_version}"
 
 [bumpversion:file:figanos/__init__.py]
-search = __version__ = '{current_version}'
-replace = __version__ = '{new_version}'
+search = __version__ = "{current_version}"
+replace = __version__ = "{new_version}"
+
+[bumpversion:file:tests/test_figanos.py]
+search = __version__ = "{current_version}"
+replace = __version__ = "{new_version}"
 
 [bumpversion:file:.cruft.json]
 search = "version": "{current_version}",
 replace = "version": "{new_version}",
 
 [aliases]
 test = pytest
 
 [tool:pytest]
 collect_ignore = ['setup.py']
-addopts = --verbose
+addopts = 
+	--verbose
 filterwarnings = 
 	ignore::UserWarning
 
 [flake8]
 exclude = 
 	.git,
 	docs,
@@ -57,19 +62,21 @@
 	py:mod,
 	py:obj,
 	py:ref,
 	ref
 
 [coverage:run]
 relative_files = True
+omit = */tests/*.py
 
 [isort]
 profile = black
+py_version = 38
 
 [pydocstyle]
 convention = numpy
-match = (?!test_).*\.py
+match = ((?!test_|conf).)*\.py
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `figanos-0.1.0/setup.py` & `figanos-0.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 """The setup script."""
 
 from setuptools import find_packages, setup
 
 with open("README.rst") as readme_file:
     readme = readme_file.read()
 
-with open("HISTORY.rst") as history_file:
-    history = history_file.read()
-
 requirements = [
     "cartopy",
     "click>=8.0",
     "dask",
     "geopandas",
     "geoviews",
     "h5py",
@@ -24,14 +21,15 @@
     "notebook",
     "numpy",
     "pandas",
     "xarray",
     "xclim>=0.38",
     "pyyaml",
     "zarr",
+    "seaborn",
 ]
 
 test_requirements = ["pytest>=3"]
 
 docs_requirements = [
     dependency for dependency in open("requirements_docs.txt").readlines()
 ]
@@ -39,35 +37,35 @@
 dev_requirements = [
     dependency for dependency in open("requirements_dev.txt").readlines()
 ]
 
 setup(
     author="Sarah-Claude Bourdeau-Goulet",
     author_email="bourdeau-goulet.sarah-claude@ouranos.ca",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     description="Outils pour produire des graphiques informatifs sur les impacts des changements climatiques.",
     entry_points={
         "console_scripts": [
             "figanos=figanos.cli:main",
         ],
     },
     install_requires=requirements,
     license="Apache Software License 2.0",
-    long_description=readme + "\n\n" + history,
+    long_description=readme,
     long_description_content_type="text/x-rst",
     include_package_data=True,
     keywords="figanos",
     name="figanos",
     packages=find_packages(include=["figanos", "figanos.*"]),
     test_suite="tests",
     tests_require=test_requirements,
@@ -76,10 +74,10 @@
         "dev": dev_requirements,
     },
     project_urls={
         "Source": "https://github.com/Ouranosinc/figanos",
         "Issue tracker": "https://github.com/Ouranosinc/figanos/issues",
         "About Ouranos": "https://www.ouranos.ca/en/",
     },
-    version="0.1.0",
+    version="0.2.0",
     zip_safe=False,
 )
```

