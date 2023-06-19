# Comparing `tmp/scprep-1.2.2.tar.gz` & `tmp/scprep-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/scprep/scprep/dist/.tmp-wa7u3mh4/scprep-1.2.2.tar", last modified: Wed Feb  1 15:30:47 2023, max compression
+gzip compressed data, was "scprep-1.2.3.tar", last modified: Mon Jun 19 18:17:58 2023, max compression
```

## Comparing `scprep-1.2.2.tar` & `scprep-1.2.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 15:30:47.000000 scprep-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (116)     1058 2023-02-01 15:30:33.000000 scprep-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     5639 2023-02-01 15:30:47.000000 scprep-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4425 2023-02-01 15:30:33.000000 scprep-1.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 15:30:47.000000 scprep-1.2.2/scprep/
--rw-r--r--   0 runner    (1001) docker     (116)      334 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4133 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/_lazyload.py
--rw-r--r--   0 runner    (1001) docker     (116)      511 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/_patch.py
--rw-r--r--   0 runner    (1001) docker     (116)    14699 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 15:30:47.000000 scprep-1.2.2/scprep/io/
--rw-r--r--   0 runner    (1001) docker     (116)      262 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4898 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (116)     3865 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/io/download.py
--rw-r--r--   0 runner    (1001) docker     (116)    12706 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/io/fcs.py
--rw-r--r--   0 runner    (1001) docker     (116)     4535 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/io/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (116)     3663 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/io/mtx.py
--rw-r--r--   0 runner    (1001) docker     (116)    13489 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/io/tenx.py
--rw-r--r--   0 runner    (1001) docker     (116)     5392 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/io/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     5158 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/measure.py
--rw-r--r--   0 runner    (1001) docker     (116)     5149 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 15:30:47.000000 scprep-1.2.2/scprep/plot/
--rw-r--r--   0 runner    (1001) docker     (116)      431 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3821 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/plot/colors.py
--rw-r--r--   0 runner    (1001) docker     (116)    14048 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/plot/histogram.py
--rw-r--r--   0 runner    (1001) docker     (116)     9646 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/plot/jitter.py
--rw-r--r--   0 runner    (1001) docker     (116)    11120 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/plot/marker.py
--rw-r--r--   0 runner    (1001) docker     (116)    46265 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/plot/scatter.py
--rw-r--r--   0 runner    (1001) docker     (116)     2846 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/plot/scree.py
--rw-r--r--   0 runner    (1001) docker     (116)    12287 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/plot/tools.py
--rw-r--r--   0 runner    (1001) docker     (116)     5288 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/plot/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     2920 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/plot/variable_genes.py
--rw-r--r--   0 runner    (1001) docker     (116)    11578 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 15:30:47.000000 scprep-1.2.2/scprep/run/
--rw-r--r--   0 runner    (1001) docker     (116)      222 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3754 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/run/conversion.py
--rw-r--r--   0 runner    (1001) docker     (116)    11481 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/run/dyngen.py
--rw-r--r--   0 runner    (1001) docker     (116)    10132 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/run/r_function.py
--rw-r--r--   0 runner    (1001) docker     (116)    11564 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/run/slingshot.py
--rw-r--r--   0 runner    (1001) docker     (116)    13635 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/run/splatter.py
--rw-r--r--   0 runner    (1001) docker     (116)     3639 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/sanitize.py
--rw-r--r--   0 runner    (1001) docker     (116)    22769 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/select.py
--rw-r--r--   0 runner    (1001) docker     (116)    26107 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/stats.py
--rw-r--r--   0 runner    (1001) docker     (116)     3752 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/transform.py
--rw-r--r--   0 runner    (1001) docker     (116)    31098 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)       22 2023-02-01 15:30:33.000000 scprep-1.2.2/scprep/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 15:30:47.000000 scprep-1.2.2/scprep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5639 2023-02-01 15:30:47.000000 scprep-1.2.2/scprep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1239 2023-02-01 15:30:47.000000 scprep-1.2.2/scprep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-01 15:30:47.000000 scprep-1.2.2/scprep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      390 2023-02-01 15:30:47.000000 scprep-1.2.2/scprep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2023-02-01 15:30:47.000000 scprep-1.2.2/scprep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      380 2023-02-01 15:30:47.000000 scprep-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2381 2023-02-01 15:30:33.000000 scprep-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 15:30:47.000000 scprep-1.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (116)    15855 2023-02-01 15:30:33.000000 scprep-1.2.2/test/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (116)     2154 2023-02-01 15:30:33.000000 scprep-1.2.2/test/test_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (116)    29008 2023-02-01 15:30:33.000000 scprep-1.2.2/test/test_io.py
--rw-r--r--   0 runner    (1001) docker     (116)     1180 2023-02-01 15:30:33.000000 scprep-1.2.2/test/test_lazyload.py
--rw-r--r--   0 runner    (1001) docker     (116)     3070 2023-02-01 15:30:33.000000 scprep-1.2.2/test/test_measure.py
--rw-r--r--   0 runner    (1001) docker     (116)     5436 2023-02-01 15:30:33.000000 scprep-1.2.2/test/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (116)      499 2023-02-01 15:30:33.000000 scprep-1.2.2/test/test_patch.py
--rw-r--r--   0 runner    (1001) docker     (116)    58725 2023-02-01 15:30:33.000000 scprep-1.2.2/test/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (116)     6955 2023-02-01 15:30:33.000000 scprep-1.2.2/test/test_reduce.py
--rw-r--r--   0 runner    (1001) docker     (116)    26733 2023-02-01 15:30:33.000000 scprep-1.2.2/test/test_run.py
--rw-r--r--   0 runner    (1001) docker     (116)     6052 2023-02-01 15:30:33.000000 scprep-1.2.2/test/test_sanitize.py
--rw-r--r--   0 runner    (1001) docker     (116)    23006 2023-02-01 15:30:33.000000 scprep-1.2.2/test/test_select.py
--rw-r--r--   0 runner    (1001) docker     (116)    14206 2023-02-01 15:30:33.000000 scprep-1.2.2/test/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (116)     4301 2023-02-01 15:30:33.000000 scprep-1.2.2/test/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (116)    21289 2023-02-01 15:30:33.000000 scprep-1.2.2/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:17:58.124339 scprep-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-19 18:17:42.000000 scprep-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-06-19 18:17:58.124339 scprep-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-06-19 18:17:42.000000 scprep-1.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:17:58.108339 scprep-1.2.3/scprep/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/_lazyload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:17:58.116339 scprep-1.2.3/scprep/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/io/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12706 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/io/fcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/io/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/io/mtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13489 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/io/tenx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:17:58.116339 scprep-1.2.3/scprep/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/plot/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/plot/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/plot/jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/plot/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46265 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/plot/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/plot/scree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12287 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/plot/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/plot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/plot/variable_genes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:17:58.120339 scprep-1.2.3/scprep/run/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/run/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/run/dyngen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/run/r_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/run/slingshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/run/splatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22769 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26107 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31201 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 18:17:42.000000 scprep-1.2.3/scprep/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:17:58.112339 scprep-1.2.3/scprep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-06-19 18:17:58.000000 scprep-1.2.3/scprep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-19 18:17:58.000000 scprep-1.2.3/scprep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 18:17:58.000000 scprep-1.2.3/scprep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-19 18:17:58.000000 scprep-1.2.3/scprep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 18:17:58.000000 scprep-1.2.3/scprep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-19 18:17:58.128339 scprep-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-19 18:17:42.000000 scprep-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:17:58.124339 scprep-1.2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    15855 2023-06-19 18:17:42.000000 scprep-1.2.3/test/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-19 18:17:42.000000 scprep-1.2.3/test/test_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29008 2023-06-19 18:17:42.000000 scprep-1.2.3/test/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-19 18:17:42.000000 scprep-1.2.3/test/test_lazyload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-19 18:17:42.000000 scprep-1.2.3/test/test_measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-06-19 18:17:42.000000 scprep-1.2.3/test/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-19 18:17:42.000000 scprep-1.2.3/test/test_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58725 2023-06-19 18:17:42.000000 scprep-1.2.3/test/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-06-19 18:17:42.000000 scprep-1.2.3/test/test_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26733 2023-06-19 18:17:42.000000 scprep-1.2.3/test/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-06-19 18:17:42.000000 scprep-1.2.3/test/test_sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23006 2023-06-19 18:17:42.000000 scprep-1.2.3/test/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-06-19 18:17:42.000000 scprep-1.2.3/test/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-19 18:17:42.000000 scprep-1.2.3/test/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21264 2023-06-19 18:17:42.000000 scprep-1.2.3/test/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scprep-1.2.2/LICENSE` & `scprep-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/PKG-INFO` & `scprep-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scprep
-Version: 1.2.2
+Version: 1.2.3
 Summary: scprep
 Home-page: https://github.com/KrishnaswamyLab/scprep
-Download-URL: https://github.com/KrishnaswamyLab/scprep/archive/v1.2.2.tar.gz
+Download-URL: https://github.com/KrishnaswamyLab/scprep/archive/v1.2.3.tar.gz
 Author: Scott Gigante, Daniel Burkhardt and Jay Stanley, Yale University
 Author-email: krishnaswamylab@gmail.com
 License: GNU General Public License Version 3
 Keywords: big-data,computational-biology
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Jupyter
```

### Comparing `scprep-1.2.2/README.rst` & `scprep-1.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/_lazyload.py` & `scprep-1.2.3/scprep/_lazyload.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/filter.py` & `scprep-1.2.3/scprep/filter.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/io/csv.py` & `scprep-1.2.3/scprep/io/csv.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/io/download.py` & `scprep-1.2.3/scprep/io/download.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/io/fcs.py` & `scprep-1.2.3/scprep/io/fcs.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/io/hdf5.py` & `scprep-1.2.3/scprep/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/io/mtx.py` & `scprep-1.2.3/scprep/io/mtx.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/io/tenx.py` & `scprep-1.2.3/scprep/io/tenx.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/io/utils.py` & `scprep-1.2.3/scprep/io/utils.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/measure.py` & `scprep-1.2.3/scprep/measure.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/normalize.py` & `scprep-1.2.3/scprep/normalize.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/plot/colors.py` & `scprep-1.2.3/scprep/plot/colors.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/plot/histogram.py` & `scprep-1.2.3/scprep/plot/histogram.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/plot/jitter.py` & `scprep-1.2.3/scprep/plot/jitter.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/plot/marker.py` & `scprep-1.2.3/scprep/plot/marker.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/plot/scatter.py` & `scprep-1.2.3/scprep/plot/scatter.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/plot/scree.py` & `scprep-1.2.3/scprep/plot/scree.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/plot/tools.py` & `scprep-1.2.3/scprep/plot/tools.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/plot/utils.py` & `scprep-1.2.3/scprep/plot/utils.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/plot/variable_genes.py` & `scprep-1.2.3/scprep/plot/variable_genes.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/reduce.py` & `scprep-1.2.3/scprep/reduce.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/run/conversion.py` & `scprep-1.2.3/scprep/run/conversion.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/run/dyngen.py` & `scprep-1.2.3/scprep/run/dyngen.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/run/r_function.py` & `scprep-1.2.3/scprep/run/r_function.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/run/slingshot.py` & `scprep-1.2.3/scprep/run/slingshot.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/run/splatter.py` & `scprep-1.2.3/scprep/run/splatter.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/sanitize.py` & `scprep-1.2.3/scprep/sanitize.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 from . import utils
 
 import numpy as np
 import pandas as pd
 import warnings
 
 
-def check_numeric(data, dtype="float", copy=None, suppress_errors=False):
+def check_numeric(data, dtype="float", copy=None, suppress_errors=False, default_fill_value=0.0):
     """Check a matrix contains only numeric data.
 
     Parameters
     ----------
     data : array-like, shape=[n_samples, n_features]
         Input data
     dtype : str or `np.dtype`, optional (default: 'float')
         Data type to which to coerce the data
     copy : bool or None, optional (default: None)
         Copy the data before coercion. If None, default to
         False for all datatypes except pandas.SparseDataFrame
     suppress_errors : bool, optional (default: False)
         Suppress errors from non-numeric data
+    default_fill_value : float
+        If sparse, the default fill value
 
     Returns
     -------
     data : array-like, shape=[n_samples, n_features]
         Output data as numeric type
 
     Raises
     ------
     TypeError : if `data` cannot be coerced to `dtype`
     """
     if copy is None:
         copy = utils.is_SparseDataFrame(data)
     try:
+        if utils.is_sparse_dataframe(data) and not isinstance(dtype, pd.SparseDtype):
+            dtype = pd.SparseDtype(dtype, fill_value=default_fill_value)
         return data.astype(dtype, copy=copy)
     except TypeError as e:
         if utils.is_SparseDataFrame(data):
             if not copy:
                 raise TypeError(
                     "pd.SparseDataFrame does not support "
                     "copy=False. Please use copy=True."
```

### Comparing `scprep-1.2.2/scprep/select.py` & `scprep-1.2.3/scprep/select.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/stats.py` & `scprep-1.2.3/scprep/stats.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/transform.py` & `scprep-1.2.3/scprep/transform.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/scprep/utils.py` & `scprep-1.2.3/scprep/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,15 +323,19 @@
             return True
         except AttributeError:
             pass
     return False
 
 
 def dataframe_to_sparse(x, fill_value=0.0):
-    return x.astype(pd.SparseDtype(float, fill_value=fill_value))
+    x = pd.DataFrame.sparse.from_spmatrix(
+        sparse.coo_matrix(x.values), index=x.index, columns=x.columns
+    )
+    x.sparse.fill_value = fill_value
+    return x
 
 
 def SparseDataFrame(X, columns=None, index=None, default_fill_value=0.0):
     if sparse.issparse(X):
         X = pd.DataFrame.sparse.from_spmatrix(X)
         X.sparse.fill_value = default_fill_value
     else:
```

### Comparing `scprep-1.2.2/scprep.egg-info/PKG-INFO` & `scprep-1.2.3/scprep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scprep
-Version: 1.2.2
+Version: 1.2.3
 Summary: scprep
 Home-page: https://github.com/KrishnaswamyLab/scprep
-Download-URL: https://github.com/KrishnaswamyLab/scprep/archive/v1.2.2.tar.gz
+Download-URL: https://github.com/KrishnaswamyLab/scprep/archive/v1.2.3.tar.gz
 Author: Scott Gigante, Daniel Burkhardt and Jay Stanley, Yale University
 Author-email: krishnaswamylab@gmail.com
 License: GNU General Public License Version 3
 Keywords: big-data,computational-biology
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Jupyter
```

### Comparing `scprep-1.2.2/scprep.egg-info/SOURCES.txt` & `scprep-1.2.3/scprep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/setup.py` & `scprep-1.2.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,25 @@
 import os
 
 install_requires = [
     "numpy>=1.12.0",
     "scipy>=0.18.1",
     "scikit-learn>=0.19.1",
     "decorator>=4.3.0",
-    "pandas>=0.25,<1.4",
+    "pandas>=0.25,<2.1",
     "packaging",
 ]
 
-optional_requires = ["fcsparser", "tables", "h5py", "anndata", "anndata2ri>=1.0.6"]
+optional_requires = [
+    "fcsparser<0.2.5",
+    "tables",
+    "h5py",
+    "anndata",
+    "anndata2ri>=1.0.6",
+]
 
 test_requires = [
     "nose",
     "nose2",
     "coverage",
     "coveralls",
     "parameterized",
```

### Comparing `scprep-1.2.2/test/test_filter.py` & `scprep-1.2.3/test/test_filter.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/test/test_hdf5.py` & `scprep-1.2.3/test/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/test/test_io.py` & `scprep-1.2.3/test/test_io.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/test/test_lazyload.py` & `scprep-1.2.3/test/test_lazyload.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/test/test_measure.py` & `scprep-1.2.3/test/test_measure.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/test/test_normalize.py` & `scprep-1.2.3/test/test_normalize.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/test/test_plot.py` & `scprep-1.2.3/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/test/test_reduce.py` & `scprep-1.2.3/test/test_reduce.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/test/test_run.py` & `scprep-1.2.3/test/test_run.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/test/test_sanitize.py` & `scprep-1.2.3/test/test_sanitize.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/test/test_select.py` & `scprep-1.2.3/test/test_select.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/test/test_stats.py` & `scprep-1.2.3/test/test_stats.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/test/test_transform.py` & `scprep-1.2.3/test/test_transform.py`

 * *Files identical despite different names*

### Comparing `scprep-1.2.2/test/test_utils.py` & `scprep-1.2.3/test/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     Y2, sample_labels = scprep.utils.combine_batches(
         [X, scprep.select.select_rows(X, idx=np.arange(X.shape[0] // 2))],
         batch_labels=[0, 1],
         append_to_cell_names=True,
     )
     assert np.all(Y.index == np.array([i[:-2] for i in Y2.index]))
     assert np.all(
-        np.core.defchararray.add("_", sample_labels.astype(str))
+        "_" + sample_labels.astype(str)
         == np.array([i[-2:] for i in Y2.index], dtype=str)
     )
     assert np.all(sample_labels.index == Y2.index)
     assert sample_labels.name == "sample_labels"
 
     def transform(X):
         return scprep.utils.combine_batches(
```

