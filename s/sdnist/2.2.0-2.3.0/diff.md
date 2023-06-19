# Comparing `tmp/sdnist-2.2.0.tar.gz` & `tmp/sdnist-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sdnist-2.2.0.tar", last modified: Fri Apr 14 14:39:51 2023, max compression
+gzip compressed data, was "dist/sdnist-2.3.0.tar", last modified: Mon Jun 19 16:58:54 2023, max compression
```

## Comparing `sdnist-2.2.0.tar` & `sdnist-2.3.0.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.451905 sdnist-2.2.0/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      138 2023-04-14 14:39:17.000000 sdnist-2.2.0/MANIFEST.in
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    21578 2023-04-14 14:39:51.451439 sdnist-2.2.0/PKG-INFO
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    18552 2023-04-14 14:39:17.000000 sdnist-2.2.0/README.md
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.404439 sdnist-2.2.0/sdnist/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     4118 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/__init__.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      213 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/__main__.py
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.412891 sdnist-2.2.0/sdnist/challenge/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/challenge/__init__.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1344 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/challenge/baseline.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     7883 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/challenge/submission.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      528 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/challenge/subsample.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    11568 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/load.py
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.428201 sdnist-2.2.0/sdnist/metrics/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/__init__.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     2218 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/apparent_match_dist.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      276 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/graph_edge_map.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     3518 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/hoc.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    17892 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/inconsistency.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    11971 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/kmarg_old.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     6501 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/kmarginal.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     8088 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/pca.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1554 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/pearson_correlation.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     3778 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/propensity.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     8519 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/regression.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1561 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/unique_exact_matches.py
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.429112 sdnist-2.2.0/sdnist/preprocess/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/preprocess/__init__.py
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.434190 sdnist-2.2.0/sdnist/report/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      296 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/__init__.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     5788 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/__main__.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      103 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/common.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      628 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/config.json
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.437475 sdnist-2.2.0/sdnist/report/dataset/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    14752 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/dataset/__init__.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     4967 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/dataset/binning.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1350 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/dataset/transform.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     4643 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/dataset/validate.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     3377 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/generate.py
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.442121 sdnist-2.2.0/sdnist/report/plots/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      418 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/plots/__init__.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     3208 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/plots/apparent_match_dist.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     3403 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/plots/correlation.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     4404 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/plots/grid.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1763 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/plots/pearson_correlation.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     2377 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/plots/propensity.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    13782 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/plots/univariate.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     7599 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/report_data.py
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.394607 sdnist-2.2.0/sdnist/report/resources/
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.442902 sdnist-2.2.0/sdnist/report/resources/templates/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    15672 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/resources/templates/main.jinja2
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.444773 sdnist-2.2.0/sdnist/report/score/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/score/__init__.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     7026 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/score/paragraphs.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     5884 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/score/privacy.py
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.448541 sdnist-2.2.0/sdnist/report/score/utility/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    29763 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/score/utility/__init__.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     4875 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/score/utility/inconsistency.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     8868 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/score/utility/linear_regression.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     7394 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/score/utility/pca.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      905 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/server.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1376 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/schema.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1034 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/strs.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     9992 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/utils.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)       22 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/version.py
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.449389 sdnist-2.2.0/sdnist/visualizer_resources/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     6936 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/visualizer_resources/report2.jinja2
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.408798 sdnist-2.2.0/sdnist.egg-info/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    21578 2023-04-14 14:39:51.000000 sdnist-2.2.0/sdnist.egg-info/PKG-INFO
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1733 2023-04-14 14:39:51.000000 sdnist-2.2.0/sdnist.egg-info/SOURCES.txt
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)        1 2023-04-14 14:39:51.000000 sdnist-2.2.0/sdnist.egg-info/dependency_links.txt
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      170 2023-04-14 14:39:51.000000 sdnist-2.2.0/sdnist.egg-info/requires.txt
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)        7 2023-04-14 14:39:51.000000 sdnist-2.2.0/sdnist.egg-info/top_level.txt
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)       38 2023-04-14 14:39:51.452098 sdnist-2.2.0/setup.cfg
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1584 2023-04-14 14:39:17.000000 sdnist-2.2.0/setup.py
+drwxr-xr-x   0 gsh3     (65125)    36684        0 2023-06-19 16:58:54.417552 sdnist-2.3.0/
+-rw-r--r--   0 gsh3     (65125)    36684     1830 2023-06-19 16:58:12.000000 sdnist-2.3.0/LICENSE
+-rw-r--r--   0 gsh3     (65125)    36684      138 2023-06-19 16:58:14.000000 sdnist-2.3.0/MANIFEST.in
+-rw-r--r--   0 gsh3     (65125)    36684    18337 2023-06-19 16:58:54.417042 sdnist-2.3.0/PKG-INFO
+-rw-r--r--   0 gsh3     (65125)    36684    17840 2023-06-19 16:58:14.000000 sdnist-2.3.0/README.md
+drwxr-xr-x   0 gsh3     (65125)    36684        0 2023-06-19 16:58:54.374721 sdnist-2.3.0/sdnist/
+-rw-r--r--   0 gsh3     (65125)    36684     4118 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/__init__.py
+-rw-r--r--   0 gsh3     (65125)    36684      213 2023-06-19 16:58:14.000000 sdnist-2.3.0/sdnist/__main__.py
+drwxr-xr-x   0 gsh3     (65125)    36684        0 2023-06-19 16:58:54.382257 sdnist-2.3.0/sdnist/challenge/
+-rw-------   0 gsh3     (65125)    36684        0 2023-06-19 16:58:14.000000 sdnist-2.3.0/sdnist/challenge/__init__.py
+-rw-r--r--   0 gsh3     (65125)    36684     1344 2023-06-19 16:58:14.000000 sdnist-2.3.0/sdnist/challenge/baseline.py
+-rw-r--r--   0 gsh3     (65125)    36684     7883 2023-06-19 16:58:14.000000 sdnist-2.3.0/sdnist/challenge/submission.py
+-rw-r--r--   0 gsh3     (65125)    36684      528 2023-06-19 16:58:14.000000 sdnist-2.3.0/sdnist/challenge/subsample.py
+-rw-r--r--   0 gsh3     (65125)    36684    11568 2023-06-19 16:58:14.000000 sdnist-2.3.0/sdnist/load.py
+drwxr-xr-x   0 gsh3     (65125)    36684        0 2023-06-19 16:58:54.391760 sdnist-2.3.0/sdnist/metrics/
+-rw-------   0 gsh3     (65125)    36684        0 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/metrics/__init__.py
+-rw-r--r--   0 gsh3     (65125)    36684     2218 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/metrics/apparent_match_dist.py
+-rw-r--r--   0 gsh3     (65125)    36684      276 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/metrics/graph_edge_map.py
+-rw-r--r--   0 gsh3     (65125)    36684     3518 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/metrics/hoc.py
+-rw-r--r--   0 gsh3     (65125)    36684    17919 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/metrics/inconsistency.py
+-rw-r--r--   0 gsh3     (65125)    36684    11971 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/metrics/kmarg_old.py
+-rw-r--r--   0 gsh3     (65125)    36684     6501 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/metrics/kmarginal.py
+-rw-r--r--   0 gsh3     (65125)    36684     8319 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/metrics/pca.py
+-rw-r--r--   0 gsh3     (65125)    36684     1554 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/metrics/pearson_correlation.py
+-rw-r--r--   0 gsh3     (65125)    36684     3778 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/metrics/propensity.py
+-rw-r--r--   0 gsh3     (65125)    36684     8613 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/metrics/regression.py
+-rw-r--r--   0 gsh3     (65125)    36684     1502 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/metrics/unique_exact_matches.py
+drwxr-xr-x   0 gsh3     (65125)    36684        0 2023-06-19 16:58:54.392553 sdnist-2.3.0/sdnist/preprocess/
+-rw-------   0 gsh3     (65125)    36684        0 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/preprocess/__init__.py
+drwxr-xr-x   0 gsh3     (65125)    36684        0 2023-06-19 16:58:54.397950 sdnist-2.3.0/sdnist/report/
+-rw-r--r--   0 gsh3     (65125)    36684      296 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/report/__init__.py
+-rw-r--r--   0 gsh3     (65125)    36684     5793 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/report/__main__.py
+-rw-r--r--   0 gsh3     (65125)    36684      103 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/report/common.py
+-rw-r--r--   0 gsh3     (65125)    36684      628 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/report/config.json
+drwxr-xr-x   0 gsh3     (65125)    36684        0 2023-06-19 16:58:54.401915 sdnist-2.3.0/sdnist/report/dataset/
+-rw-r--r--   0 gsh3     (65125)    36684    15237 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/report/dataset/__init__.py
+-rw-r--r--   0 gsh3     (65125)    36684     4968 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/report/dataset/binning.py
+-rw-r--r--   0 gsh3     (65125)    36684     1350 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/report/dataset/transform.py
+-rw-r--r--   0 gsh3     (65125)    36684     4644 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/report/dataset/validate.py
+-rw-r--r--   0 gsh3     (65125)    36684     3471 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/report/generate.py
+drwxr-xr-x   0 gsh3     (65125)    36684        0 2023-06-19 16:58:54.409224 sdnist-2.3.0/sdnist/report/plots/
+-rw-r--r--   0 gsh3     (65125)    36684      418 2023-06-19 16:58:14.000000 sdnist-2.3.0/sdnist/report/plots/__init__.py
+-rw-r--r--   0 gsh3     (65125)    36684     3208 2023-06-19 16:58:14.000000 sdnist-2.3.0/sdnist/report/plots/apparent_match_dist.py
+-rw-r--r--   0 gsh3     (65125)    36684     3403 2023-06-19 16:58:14.000000 sdnist-2.3.0/sdnist/report/plots/correlation.py
+-rw-r--r--   0 gsh3     (65125)    36684     4404 2023-06-19 16:58:14.000000 sdnist-2.3.0/sdnist/report/plots/grid.py
+-rw-r--r--   0 gsh3     (65125)    36684     1866 2023-06-19 16:58:14.000000 sdnist-2.3.0/sdnist/report/plots/pearson_correlation.py
+-rw-r--r--   0 gsh3     (65125)    36684     2626 2023-06-19 16:58:14.000000 sdnist-2.3.0/sdnist/report/plots/propensity.py
+-rw-r--r--   0 gsh3     (65125)    36684    13909 2023-06-19 16:58:14.000000 sdnist-2.3.0/sdnist/report/plots/univariate.py
+-rw-r--r--   0 gsh3     (65125)    36684     8183 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/report/report_data.py
+drwxr-xr-x   0 gsh3     (65125)    36684        0 2023-06-19 16:58:54.365810 sdnist-2.3.0/sdnist/report/resources/
+drwxr-xr-x   0 gsh3     (65125)    36684        0 2023-06-19 16:58:54.410058 sdnist-2.3.0/sdnist/report/resources/templates/
+-rw-r--r--   0 gsh3     (65125)    36684    16416 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/report/resources/templates/main.jinja2
+drwxr-xr-x   0 gsh3     (65125)    36684        0 2023-06-19 16:58:54.412534 sdnist-2.3.0/sdnist/report/score/
+-rw-------   0 gsh3     (65125)    36684        0 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/report/score/__init__.py
+-rw-r--r--   0 gsh3     (65125)    36684     9725 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/report/score/paragraphs.py
+-rw-r--r--   0 gsh3     (65125)    36684     6443 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/report/score/privacy.py
+drwxr-xr-x   0 gsh3     (65125)    36684        0 2023-06-19 16:58:54.415362 sdnist-2.3.0/sdnist/report/score/utility/
+-rw-r--r--   0 gsh3     (65125)    36684    29923 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/report/score/utility/__init__.py
+-rw-r--r--   0 gsh3     (65125)    36684     6038 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/report/score/utility/inconsistency.py
+-rw-r--r--   0 gsh3     (65125)    36684     8868 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/report/score/utility/linear_regression.py
+-rw-r--r--   0 gsh3     (65125)    36684     7383 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/report/score/utility/pca.py
+-rw-r--r--   0 gsh3     (65125)    36684      905 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/report/server.py
+-rw-r--r--   0 gsh3     (65125)    36684     1376 2023-06-19 16:58:14.000000 sdnist-2.3.0/sdnist/schema.py
+-rw-r--r--   0 gsh3     (65125)    36684     1034 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/strs.py
+-rw-r--r--   0 gsh3     (65125)    36684     9992 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/utils.py
+-rw-r--r--   0 gsh3     (65125)    36684       22 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/version.py
+drwxr-xr-x   0 gsh3     (65125)    36684        0 2023-06-19 16:58:54.416198 sdnist-2.3.0/sdnist/visualizer_resources/
+-rw-r--r--   0 gsh3     (65125)    36684     6936 2023-06-19 16:58:12.000000 sdnist-2.3.0/sdnist/visualizer_resources/report2.jinja2
+drwxr-xr-x   0 gsh3     (65125)    36684        0 2023-06-19 16:58:54.378935 sdnist-2.3.0/sdnist.egg-info/
+-rw-r--r--   0 gsh3     (65125)    36684    18337 2023-06-19 16:58:53.000000 sdnist-2.3.0/sdnist.egg-info/PKG-INFO
+-rw-r--r--   0 gsh3     (65125)    36684     1741 2023-06-19 16:58:53.000000 sdnist-2.3.0/sdnist.egg-info/SOURCES.txt
+-rw-r--r--   0 gsh3     (65125)    36684        1 2023-06-19 16:58:53.000000 sdnist-2.3.0/sdnist.egg-info/dependency_links.txt
+-rw-r--r--   0 gsh3     (65125)    36684      170 2023-06-19 16:58:53.000000 sdnist-2.3.0/sdnist.egg-info/requires.txt
+-rw-r--r--   0 gsh3     (65125)    36684        7 2023-06-19 16:58:53.000000 sdnist-2.3.0/sdnist.egg-info/top_level.txt
+-rw-r--r--   0 gsh3     (65125)    36684       38 2023-06-19 16:58:54.417745 sdnist-2.3.0/setup.cfg
+-rw-r--r--   0 gsh3     (65125)    36684     1584 2023-06-19 16:58:14.000000 sdnist-2.3.0/setup.py
```

### Comparing `sdnist-2.2.0/PKG-INFO` & `sdnist-2.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,328 +1,292 @@
-Metadata-Version: 2.1
-Name: sdnist
-Version: 2.2.0
-Summary: SDNist: Deidentified Data Report Generator
-Home-page: https://github.com/usnistgov/SDNist
-Author: National Institute of Standards and Technology
-Author-email: gary.howarth@nist.gov
-License: UNKNOWN
-Description: # SDNist v2.2: Deidentified Data Report Tool
-        
-        ## [SDNist is the offical software package for engaging in the NIST Collaborative Research Cycle](https://pages.nist.gov/privacy_collaborative_research_cycle)
-        
-        Welcome! SDNist is a python package that provides benchmark data and evaluation metrics for deidentified data generators. This version of SDNist supports using the [NIST Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/tree/main/nist%20diverse%20communities%20data%20excerpts), a geographically partioned, limited feature data set.
-        
-        The deidentified data report evaluates utility and privacy of a given deidentified dataset and generates a summary quality report with performance of a deidentified dataset enumerated and illustrated for each utility and privacy metric.
-        
-        [Preview sample reports produced by the tool here.](https://github.com/usnistgov/SDNist/tree/main/sdnist/report/sample-reports)
-        
-        This tool is being actively developed. Please (raise an Issue)[https://github.com/usnistgov/SDNist/issues]  if you catch a bug or would like have feature suggestions. 
-        
-        
-        ### Project Team  
-        **Karan Bhagat**, *Knexus Research* - Developer *sdnist.report* package  
-        
-        **Christine Task**, *Knexus Research* - Project technical lead
-        
-        **Gary Howarth**, *NIST* - Project PI [gary.howarth@nist.gov](mailto:gary.howarth@nist.gov)
-        
-        ### Reporting Issues
-        Help us improve the package and this guide by reporting issues [here](https://github.com/usnistgov/SDNist/issues).
-        
-        ### Temporal Map Challenge Environment
-        
-        SDNist v2.0 and above does not support the Temporal Map Challenge environment.
-        
-        To run the testing environment from the [*NIST PSCR Differential Privacy Temporal Map Challenge*](https://www.nist.gov/ctl/pscr/open-innovation-prize-challenges/past-prize-challenges/2020-differential-privacy-temporal) for the Chicago Taxi data sprint or the American Community Survey sprint, please go to the the [Temporal Map Challenge assets repository](https://github.com/usnistgov/Differential-Privacy-Temporal-Map-Challenge-assets).
-        
-        
-        Setting Up the SDNIST Report Tool
-        ------------------------
-        
-        ### Brief Setup Instructions
-        
-        SDNist requires Python version 3.7 or greater. If you have installed a previous version of the SDNist library, we recommend uninstalling or installing v2.2 in a virtual environment. v2.2 can be installed via [Release 2.2](https://github.com/usnistgov/SDNist/releases/tag/v2.2.0). The NIST Diverse Community Exceprt data will download on the fly.
-        ```
-        pip install sdnist
-        ```
-        
-        ### Detailed Setup Instructions
-        
-        1. The SDNist Report Tool is a part of the sdnist Python library that can be installed on a user’s MAC OS, Windows, or Linux machine.
-        
-        
-        2. The sdnist library requires Python version 3.7 or greater to be installed on the user's machine. Check whether an installation exists on the machine by executing the following command in your terminal on Mac/Linux or powershell on Windows:
-           ```
-            c:\\> python -V
-           ```
-            If Python is already installed, the above command should return the currently installed version. If Python is not found or the version is below 3.7, then you can download Python from the [Python website](https://www.python.org/downloads/).
-        
-        
-        3.  Create a local directory/folder on the machine to set up the SDNist library. This guide assumes the local directory to be sdnist-project; an example of a complete file path is c:\\sdnist-project:
-            ```
-            c:\\sdnist-project>     
-            ```
-        
-        4.  Download the sdnist installable wheel (sdnist-2.2.0-py3-none-any.whl) from the Github: [Release 2.2](https://github.com/usnistgov/SDNist/releases/download/v2.2.0/sdnist-2.2.0-py3-none-any.whl).
-        
-        
-        5.  Move the downloaded sdnist-2.2.0-py3-none-any.whl file to the sdnist-project directory.
-        
-        
-        6.  Using the terminal on Mac/Linux or powershell on Windows, navigate to the sdnist-project directory.
-        
-        
-        7.  In the already-opened terminal or powershell window, execute the following command to create a new Python environment. The sdnist library will be installed in this newly created Python environment:
-        
-            ```
-            c:\\sdnist-project> python -m venv venv
-            ```
-        
-        8. The new Python environment will be created in the sdnist-project directory, and the files of the environment should be in the venv directory. To check whether a new Python environment was created successfully, use the following command to list all directories in the sdnist-project directory, and make sure the venv directory exists.
-        
-            **MAC OS/Linux:**
-            ```
-            sdnist-project> ls
-            ```
-            **Windows:**
-            ```
-            c:\\sdnist-project> dir
-            ```
-        
-        9. Now activate the Python environment and install the sdnist library into it.
-        
-            **MAC OS/Linux:**
-            ```
-            sdnist-project> . venv/bin/activate
-            ```
-            The python virtual environment should now be activated. You should see environment name (**venv** in this case) appended to the terminal prompt as below:  
-            ```
-            (venv) sdnist-project>
-            ```
-        
-            **Windows:**
-            ```
-            c:\\sdnist-project> . venv/Scripts/activate
-            ```
-            The python virtual environment should now be activated. You should see environment name (**venv** in this case) appended to the command/powershell prompt as below:  
-            ```
-            (venv) c:\\sdnist-project>
-            ```
-        
-            On Windows, a few users may encounter the following error if their machines are new (executing scripts is disabled by default on some Windows machines):
-            ```
-            C:\\sdnist-project\\venv\\Scripts\\Activate.ps1 cannot be loaded because running scripts is disabled on this system.
-            ```
-            Run the following command to let Windows execute scripts:
-            ```
-            Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope LocalMachine
-            ```
-        
-        
-        10. Per step 5 above, the sdnist-2.2.0-py3-none-any.whl file should already be present in the sdnist-project directory. Check whether that is true by listing the files in the sdnist-project directory.
-        
-              **MAC OS/Linux:**
-               ```
-               (venv) sdnist-project> ls
-               ```
-              **Windows:**
-               ```
-               (venv) c:\\sdnist-project> dir
-               ```
-               The sdnist-2.2.0-py3-none-any.whl file should be in the list printed by the above command; otherwise, follow steps 4 and 5 again to download the .whl file.
-        
-        
-        11. Install sdnist Python library:
-               ```
-               (venv) c:\\sdnist-project> pip install sdnist-2.2.0-py3-none-any.whl
-               ```
-        
-        
-        12. Installation is successful if executing the following command outputs a help menu for the sdnist.report package:
-               ```
-               (venv) c:\\sdnist-project> python -m sdnist.report -h
-               ```
-               Output:
-               ```
-                usage: __main__.py [-h] [--labels LABELS] [--data-root DATA_ROOT]
-                                   PATH_DEIDENTIFIED_DATASET TARGET_DATASET_NAME
-                
-                positional arguments:
-                  PATH_DEIDENTIFIED_DATASET
-                                        Location of deidentified dataset (csv or parquet
-                                        file).
-                  TARGET_DATASET_NAME   Select name of the target dataset that was used to
-                                        generated given deidentified dataset.
-                
-                options:
-                  -h, --help            show this help message and exit
-                  --labels LABELS       This argument is used to add meta-data to help
-                                        identify which deidentified data was was evaluated in
-                                        the report. The argument can be a string that is a
-                                        plain text label for the file, or it can be a file
-                                        path to a json file containing [label, value] pairs.
-                                        This labels will be included in the printed report.
-                  --data-root DATA_ROOT
-                                        Path of the directory to be used as the root for the
-                                        target datasets.
-                
-                Choices for Target Dataset Name:
-                  [DATASET NAME]        [FILENAME]
-                  MA                    ma2019
-                  TX                    tx2019
-                  NATIONAL              national2019
-               ```
-        
-        
-        13. These instructions install sdnist into a virtual environment. The virtual environment must be activated (step 9) each time a new terminal window is used with sdnist.
-        
-        
-        Generate Data Quality Report
-        ---------------------------
-        
-        1.  The sdnist.report package requires a path to the deidentified dataset file and the name of the target dataset from which the deidentified dataset file will be created. Following is the command line usage of the sdnist.report package:
-              ```
-              python -m sdnist.report PATH_DEINDETIFIED_DATASET TARGET_DATSET_NAME
-              ```
-        
-              The above command is just an example usage signature of the package. Steps 3 through 5 show the actual commands to run the tool, where the parameter PATH_DEIDENTIFIED_DATASET is replaced with the path of the deidentified dataset file on the your machine, and the parameter TARGET_DATASET_NAME is replaced with one of the bundled dataset names (MA, TX, or NATIONAL).
-        
-              A deidentified dataset file can be anywhere on your machine. You only need the path of the file to pass it as an argument to the sdnist.report package. For illustration purposes, this guide assumes an example deidentified dataset file named syn_tx.csv is generated from the bundled dataset file named TX that is present in the sdnist-project directory. You can also use the bundled toy deidentified datasets for generating some toy evaluation reports using the sdnist.report package by following steps 5 and 6 in the next section, Setup Data for SDNIST Report Tool.
-        
-             The sdnist.report packages come bundled with three target datasets: MA, TX, and NATIONAL. If these datasets are not available locally, the package will download them automatically when you run any one of the commands in steps 3 through 5 for the first time. In case of any trouble while downloading the datasets, please refer to the next section, Setup Data for SDNIST Report Tool.
-        
-        
-        2.  If you have closed the terminal or the powershell window that was used for the tool setup, open a new one, and after navigating the to sdnist-project directory, run the activate script as explained in step 9 of the Setup SDNIST Report Tool section.
-        
-        
-        3.  Use the following command to generate a data quality report for the example deidentified dataset (syn_tx.csv) that is generated using the bundled dataset TX:
-              ```
-              (venv) c:\\sdnist-project> python -m sdnist.report syn_tx.csv TX
-              ```
-              At the completion of the process initiated by the above command, an .html report will open in the default web browser on your machine. Likewise, .html report files will be available in the reports directory created automatically in the sdnist-project directory.
-        
-        
-        4.  Use the following command to generate a data quality report for the example deidentified dataset (syn_ma.csv) that is generated using the bundled dataset MA:
-              ```
-              (venv) c:\\sdnist-project> python -m sdnist.report syn_ma.csv MA
-              ```
-        
-        
-        5.  Use the following command to generate a data quality report for the example deidentified dataset (syn_national.csv) that is generated using the bundled dataset NATIONAL:
-              ```
-              (venv) c:\\sdnist-project> python -m sdnist.report syn_national.csv NATIONAL
-              ```
-        6.  Starting from version 2.1, SDNist allow users to add labels for the deidentified dataset used to generate report:
-            * To add single string label to the report, use command line option **--labels** followed by a string as given in the following example command:
-              ```
-              (venv) c:\\sdnist-project> python -m sdnist.report syn_national.csv NATIONAL --labels used_epsilon_1
-              ```
-              This is how the string label *used_epsilon_1* will appear in the report:
-              ![string label in report](readme_resource/string_label.png)
-            * To add multiple string labels to the report, use command line option **--labels** followed by a path to the json file containing labels:
-              ```
-              (venv) c:\\sdnist-project> python -m sdnist.report syn_national.csv NATIONAL --labels example_labels.json
-              ```
-              Where example_labels.json can be:
-              ```
-                {
-                  "epsilon": "1",
-                  "delta": "10^-5",
-                  "created on": "March 3, 2023",
-                  "deidentification method": "example_method"
-                }
-              ```
-              This is how the *example_labels.json* will appear in the report:
-             ![multiple labels in report](readme_resource/multiple_labels.png)
-        7.  The following are all the parameters offered by the sdnist.report package:
-        
-             - **PATH_DEIDENTIFIED_DATASET**: The absolute or relative path to the deidentified dataset .csv or parquet file. If the provided path is relative, it should be relative to the current working directory. This guide assumes the current working directory is sdnist-project.
-             - **TARGET_DATASET_NAME**: This should be the name of one of the datasets bundled with the sdnist.report package. It is the name of the dataset from which the input deidentified dataset is generated, and it can be one of the following:
-               - MA
-               - TX
-               - NATIONAL
-        
-             - **--data-root**: The absolute or relative path to the directory containing the bundled dataset, or the directory where the bundled dataset should be downloaded to if it is not available locally. The default directory is set to **diverse_community_excerpts_data**.
-             - **--labels**: This argument is used to add meta-data to help identify which deidentified data was was evaluated in the report.  The argument can be a string that is a plain text label for the file, or it can be a file path to a json file containing label, value pairs. 
-        
-        Setup Data for SDNIST Report Tool
-        ---------------------------------
-        
-        1.  The sdnist.report package comes with built-in datasets. The package will automatically download the datasets from Github if they are not already available locally on your machine. You should see following message on your terminal or powershell window when the datasets are downloaded by the sdnist.report package:
-              ```
-              (venv) c:\\sdnist-project> python -m sdnist.report syn_tx.csv TX
-        
-              Downloading all SDNist datasets from:  
-              https://github.com/usnistgov/SDNist/releases/download/v2.2.0/diverse_communities_data_excerpts.zip ...  
-              ...5%, 47352 KB, 8265 KB/s, 5 seconds elapsed
-              ```
-        
-              Follow the next subsection, Download Data Manually, if the sdnist.report package is unable to download the datasets.
-        
-        
-        2. All the datasets required by the sdnist.report package are installed into the sdnist _toy _data directory, which should be now present inside the sdnist-project directory. sdnist _toy _data is also a data root directory. You can use some other directory as a data root by providing the –data-root argument to the sdnist.report package. If you provide a –data-root argument with a path, the sdnist.report package will look for datasets in the data root directory you have specified, and the package will download it if it is not present in the data root.
-        
-        
-        3. The sdnist.report package also needs a deidentified dataset that it can evaluate against its original counterpart. Since the sdnist.report package comes bundled with the datasets, the deidentified dataset should be generated using the bundled datasets.
-        
-           You can download a copy of the datasets from Github [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/tree/main/nist%20diverse%20communities%20data%20excerpts). This copy is similar to the one bundled with the sdnist.report package, but it contains more documentation and a description of the datasets.
-        
-        
-        4. You can download the toy deidentified datasets from Github [Sdnist Toy Deidentified Dataset](https://github.com/usnistgov/SDNist/releases/download/v2.1.1/toy_deidentified_data.zip). Unzip the downloaded file, and move the unzipped toy_deidentified_dataset directory to the sdnist-project directory.
-        
-        
-        5. Each toy deidentified dataset file is generated using the [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.2.0/diverse_communities_excerpts_data.zip). The syn_ma.csv, syn_tx.csv, and syn_national.csv deidentified dataset files are created from target datasets MA (ma2019.csv), TX (tx2019.csv), and NATIONAL(national2019.csv), respectively. You can use one of the toy deidentified dataset files for testing whether the sdnist.report package is installed correctly on your system.
-        
-        
-        6. Use the following commands for generating reports if you are using a toy deidentified dataset file:
-        
-           For evaluating the Massachusetts dataset:
-           ```
-           (venv) c:\\sdnist-project> python -m sdnist.report toy_deidentified_data/syn_ma.csv MA
-           ```
-        
-           For evaluating the Texas dataset:
-           ```
-           (venv) c:\\sdnist-project> python -m sdnist.report toy_deidentified_data/syn_tx.csv TX
-           ```
-        
-           For evaluating the national dataset:
-           ```
-           (venv) c:\\sdnist-project> python -m sdnist.report toy_deidentified_data/syn_national.csv NATIONAL
-           ```
-        
-        7.  A deidentified dataset can be a .csv or a parquet file, and the path of this file is required
-        by the sdnist.report package to generate a data quality report.
-        
-        
-        Download Data Manually
-        ----------------------
-        
-        1.  If the sdnist.report package is not able to download the datasets, you can download them from Github [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.2.0/diverse_communities_data_excerpts.zip).
-        3.  Unzip the **diverse_community_excerpts_data.zip** file and move the unzipped **diverse_community_excerpts_data** directory to the **sdnist-project** directory.
-        4.  Delete the **diverse_community_excerpts_data.zip** file once the data is successfully extracted from the zip.
-        
-        Citing SDNist Deidentified Data Report Tool
-        -------------------------------------------
-        
-        If you publish work that utilizes the SDNist Deidentified Data Tool, please cite the software. Citation recommendation:  
-        > Task C., Bhagat K., and Howarth G.S. (2023), SDNist v2: Deidentified Data Report Tool, 
-        > National Institute of Standards and Technology, 
-        > https://doi.org/10.18434/mds2-2943    
-        (NOTE: DOI is not yet active, but should be by 1 APR 2023).
-        
-        Credits 
-        ----------
-        
-        - [Christine Task](mailto:christine.task@knexusresearch.com) - Project technical lead - christine.task@knexusresearch.com
-        - [Karan Bhagat](https://github.com/kbtriangulum) - Contributor
-        - [David Lee](https://www.linkedin.com/in/david-lee-13872922/) - Documentation
-        - [Gary Howarth](https://www.nist.gov/people/gary-howarth) - Project PI - gary.howarth@nist.gov
-        
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: Public Domain
-Classifier: Intended Audience :: Science/Research
-Description-Content-Type: text/markdown
+# SDNist v2.3: Deidentified Data Report Tool
+
+## [SDNist is the offical software package for engaging in the NIST Collaborative Research Cycle](https://pages.nist.gov/privacy_collaborative_research_cycle)
+
+Welcome! SDNist is a python package that provides benchmark data and evaluation metrics for deidentified data generators. This version of SDNist supports using the [NIST Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/tree/main/nist%20diverse%20communities%20data%20excerpts), a geographically partioned, limited feature data set.
+
+The deidentified data report evaluates utility and privacy of a given deidentified dataset and generates a summary quality report with performance of a deidentified dataset enumerated and illustrated for each utility and privacy metric.
+
+[Preview sample reports produced by the tool here.](https://github.com/usnistgov/SDNist/tree/main/sdnist/report/sample-reports)
+
+This tool is being actively developed. Please (raise an Issue)[https://github.com/usnistgov/SDNist/issues]  if you catch a bug or would like have feature suggestions. 
+
+
+### Project Team  
+**Karan Bhagat**, *Knexus Research* - Developer *sdnist.report* package  
+
+**Christine Task**, *Knexus Research* - Project technical lead
+
+**Gary Howarth**, *NIST* - Project PI [gary.howarth@nist.gov](mailto:gary.howarth@nist.gov)
+
+### Acknowledgements
+
+SDNist v2 grew from [SDNist v1](https://github.com/usnistgov/Differential-Privacy-Temporal-Map-Challenge-assets), developed in partnership with Saurus Technologies under CRADA CN-21-0143.
+
+### Reporting Issues
+Help us improve the package and this guide by reporting issues [here](https://github.com/usnistgov/SDNist/issues).
+
+### Temporal Map Challenge Environment
+
+SDNist v2.0 and above does not support the Temporal Map Challenge environment.
+
+To run the testing environment from the [*NIST PSCR Differential Privacy Temporal Map Challenge*](https://www.nist.gov/ctl/pscr/open-innovation-prize-challenges/past-prize-challenges/2020-differential-privacy-temporal) for the Chicago Taxi data sprint or the American Community Survey sprint, please go to the the [Temporal Map Challenge assets repository](https://github.com/usnistgov/Differential-Privacy-Temporal-Map-Challenge-assets).
+
+
+Setting Up the SDNIST Report Tool
+------------------------
+
+### Brief Setup Instructions
+
+SDNist requires Python version 3.7 or greater. If you have installed a previous version of the SDNist library, we recommend installing v2.3 in a virtual environment. v2.3 can be installed via [Release 2.3](https://github.com/usnistgov/SDNist/releases/tag/v2.3.0) or via the Pypi server: `pip install sdnist` or, if you already have a version installed, `pip install --upgrade sdnist`.
+
+The NIST Diverse Community Exceprt data will download on the fly.
+
+
+
+### Detailed Setup Instructions Using Pypi
+
+1. The SDNist Report Tool is a part of the sdnist Python library that can be installed on a user’s MAC OS, Windows, or Linux machine.
+
+
+2. The sdnist library requires Python version 3.7 or greater to be installed on the user's machine. Check whether an installation exists on the machine by executing the following command in your terminal on Mac/Linux or powershell on Windows:
+   ```
+    c:\\> python -V
+   ```
+    If Python is already installed, the above command should return the currently installed version. If Python is not found or the version is below 3.7, then you can download Python from the [Python website](https://www.python.org/downloads/).
+
+
+3.  Create a local directory/folder on the machine to set up the SDNist library. This guide assumes the local directory to be sdnist-project; an example of a complete file path is c:\\sdnist-project:
+    ```
+    c:\\sdnist-project>     
+    ```
+
+
+4. In the already-opened terminal or powershell window, execute the following command to create a new Python environment. The sdnist library will be installed in this newly created Python environment:
+
+    ```
+    c:\\sdnist-project> python -m venv venv
+    ```
+
+5. The new Python environment will be created in the sdnist-project directory, and the files of the environment should be in the venv directory. To check whether a new Python environment was created successfully, use the following command to list all directories in the sdnist-project directory, and make sure the venv directory exists.
+
+    **MAC OS/Linux:**
+    ```
+    sdnist-project> ls
+    ```
+    **Windows:**
+    ```
+    c:\\sdnist-project> dir
+    ```
+
+6. Now activate the Python environment and install the sdnist library into it.
+
+    **MAC OS/Linux:**
+    ```
+    sdnist-project> . venv/bin/activate
+    ```
+    The python virtual environment should now be activated. You should see environment name (**venv** in this case) appended to the terminal prompt as below:  
+    ```
+    (venv) sdnist-project>
+    ```
+
+    **Windows:**
+    ```
+    c:\\sdnist-project> . venv/Scripts/activate
+    ```
+    The python virtual environment should now be activated. You should see environment name (**venv** in this case) appended to the command/powershell prompt as below:  
+    ```
+    (venv) c:\\sdnist-project>
+    ```
+
+    On Windows, a few users may encounter the following error if their machines are new (executing scripts is disabled by default on some Windows machines):
+    ```
+    C:\\sdnist-project\\venv\\Scripts\\Activate.ps1 cannot be loaded because running scripts is disabled on this system.
+    ```
+    Run the following command to let Windows execute scripts:
+    ```
+    Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope LocalMachine
+    ```
+
+7. Install sdnist Python library:
+       ```
+       (venv) c:\\sdnist-project> pip install sdnist
+       ```
+
+8. Installation is successful if executing the following command outputs a help menu for the sdnist.report package:
+       ```
+       (venv) c:\\sdnist-project> python -m sdnist.report -h
+       ```
+       Output:
+       ```
+        usage: __main__.py [-h] [--labels LABELS] [--data-root DATA_ROOT]
+                           PATH_DEIDENTIFIED_DATASET TARGET_DATASET_NAME
+        
+        positional arguments:
+          PATH_DEIDENTIFIED_DATASET
+                                Location of deidentified dataset (csv or parquet
+                                file).
+          TARGET_DATASET_NAME   Select name of the target dataset that was used to
+                                generated given deidentified dataset.
+        
+        options:
+          -h, --help            show this help message and exit
+          --labels LABELS       This argument is used to add meta-data to help
+                                identify which deidentified data was was evaluated in
+                                the report. The argument can be a string that is a
+                                plain text label for the file, or it can be a file
+                                path to a json file containing [label, value] pairs.
+                                This labels will be included in the printed report.
+          --data-root DATA_ROOT
+                                Path of the directory to be used as the root for the
+                                target datasets.
+        
+        Choices for Target Dataset Name:
+          [DATASET NAME]        [FILENAME]
+          MA                    ma2019
+          TX                    tx2019
+          NATIONAL              national2019
+       ```
+
+9. These instructions install sdnist into a virtual environment. The virtual environment must be activated (step 9) each time a new terminal window is used with sdnist.
+
+
+Generate Data Quality Report
+---------------------------
+
+1.  The sdnist.report package requires a path to the deidentified dataset file and the name of the target dataset from which the deidentified dataset file will be created. Following is the command line usage of the sdnist.report package:
+      ```
+      python -m sdnist.report PATH_DEINDETIFIED_DATASET TARGET_DATSET_NAME
+      ```
+
+      The above command is just an example usage signature of the package. Steps 3 through 5 show the actual commands to run the tool, where the parameter PATH_DEIDENTIFIED_DATASET is replaced with the path of the deidentified dataset file on the your machine, and the parameter TARGET_DATASET_NAME is replaced with one of the bundled dataset names (MA, TX, or NATIONAL).
+
+      A deidentified dataset file can be anywhere on your machine. You only need the path of the file to pass it as an argument to the sdnist.report package. For illustration purposes, this guide assumes an example deidentified dataset file named syn_tx.csv is generated from the bundled dataset file named TX that is present in the sdnist-project directory. You can also use the bundled toy deidentified datasets for generating some toy evaluation reports using the sdnist.report package by following steps 5 and 6 in the next section, Setup Data for SDNIST Report Tool.
+
+     The sdnist.report packages come bundled with three target datasets: MA, TX, and NATIONAL. If these datasets are not available locally, the package will download them automatically when you run any one of the commands in steps 3 through 5 for the first time. In case of any trouble while downloading the datasets, please refer to the next section, Setup Data for SDNIST Report Tool.
+
+
+2.  If you have closed the terminal or the powershell window that was used for the tool setup, open a new one, and after navigating the to sdnist-project directory, run the activate script as explained in step 9 of the Setup SDNIST Report Tool section.
+
+
+3.  Use the following command to generate a data quality report for the example deidentified dataset (syn_tx.csv) that is generated using the bundled dataset TX:
+      ```
+      (venv) c:\\sdnist-project> python -m sdnist.report syn_tx.csv TX
+      ```
+      At the completion of the process initiated by the above command, an .html report will open in the default web browser on your machine. Likewise, .html report files will be available in the reports directory created automatically in the sdnist-project directory.
+
+
+4.  Use the following command to generate a data quality report for the example deidentified dataset (syn_ma.csv) that is generated using the bundled dataset MA:
+      ```
+      (venv) c:\\sdnist-project> python -m sdnist.report syn_ma.csv MA
+      ```
+
+
+5.  Use the following command to generate a data quality report for the example deidentified dataset (syn_national.csv) that is generated using the bundled dataset NATIONAL:
+      ```
+      (venv) c:\\sdnist-project> python -m sdnist.report syn_national.csv NATIONAL
+      ```
+6.  Starting from version 2.1, SDNist allow users to add labels for the deidentified dataset used to generate report:
+    * To add single string label to the report, use command line option **--labels** followed by a string as given in the following example command:
+      ```
+      (venv) c:\\sdnist-project> python -m sdnist.report syn_national.csv NATIONAL --labels used_epsilon_1
+      ```
+      This is how the string label *used_epsilon_1* will appear in the report:
+      ![string label in report](readme_resource/string_label.png)
+    * To add multiple string labels to the report, use command line option **--labels** followed by a path to the json file containing labels:
+      ```
+      (venv) c:\\sdnist-project> python -m sdnist.report syn_national.csv NATIONAL --labels example_labels.json
+      ```
+      Where example_labels.json can be:
+      ```
+        {
+          "epsilon": "1",
+          "delta": "10^-5",
+          "created on": "March 3, 2023",
+          "deidentification method": "example_method"
+        }
+      ```
+      This is how the *example_labels.json* will appear in the report:
+     ![multiple labels in report](readme_resource/multiple_labels.png)
+7.  The following are all the parameters offered by the sdnist.report package:
+
+     - **PATH_DEIDENTIFIED_DATASET**: The absolute or relative path to the deidentified dataset .csv or parquet file. If the provided path is relative, it should be relative to the current working directory. This guide assumes the current working directory is sdnist-project.
+     - **TARGET_DATASET_NAME**: This should be the name of one of the datasets bundled with the sdnist.report package. It is the name of the dataset from which the input deidentified dataset is generated, and it can be one of the following:
+       - MA
+       - TX
+       - NATIONAL
+
+     - **--data-root**: The absolute or relative path to the directory containing the bundled dataset, or the directory where the bundled dataset should be downloaded to if it is not available locally. The default directory is set to **diverse_community_excerpts_data**.
+     - **--labels**: This argument is used to add meta-data to help identify which deidentified data was was evaluated in the report.  The argument can be a string that is a plain text label for the file, or it can be a file path to a json file containing label, value pairs. 
+
+Setup Data for SDNIST Report Tool
+---------------------------------
+
+1.  The sdnist.report package comes with built-in datasets. The package will automatically download the datasets from Github if they are not already available locally on your machine. You should see following message on your terminal or powershell window when the datasets are downloaded by the sdnist.report package:
+      ```
+      (venv) c:\\sdnist-project> python -m sdnist.report syn_tx.csv TX
+
+      Downloading all SDNist datasets from:  
+      https://github.com/usnistgov/SDNist/releases/download/v2.2.0/diverse_communities_data_excerpts.zip ...  
+      ...5%, 47352 KB, 8265 KB/s, 5 seconds elapsed
+      ```
+
+      Follow the next subsection, Download Data Manually, if the sdnist.report package is unable to download the datasets.
+
+
+2. All the datasets required by the sdnist.report package are installed into the sdnist \_toy \_data directory, which should be now present inside the sdnist-project directory. sdnist \_toy \_data is also a data root directory. You can use some other directory as a data root by providing the –data-root argument to the sdnist.report package. If you provide a –data-root argument with a path, the sdnist.report package will look for datasets in the data root directory you have specified, and the package will download it if it is not present in the data root.
+
+
+3. The sdnist.report package also needs a deidentified dataset that it can evaluate against its original counterpart. Since the sdnist.report package comes bundled with the datasets, the deidentified dataset should be generated using the bundled datasets.
+
+   You can download a copy of the datasets from Github [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/tree/main/nist%20diverse%20communities%20data%20excerpts). This copy is similar to the one bundled with the sdnist.report package, but it contains more documentation and a description of the datasets.
+
+
+4. You can download the toy deidentified datasets from Github [Sdnist Toy Deidentified Dataset](https://github.com/usnistgov/SDNist/releases/download/v2.1.1/toy_deidentified_data.zip). Unzip the downloaded file, and move the unzipped toy_deidentified_dataset directory to the sdnist-project directory.
+
+
+5. Each toy deidentified dataset file is generated using the [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.3.0/diverse_communities_data_excerpts.zip). The syn_ma.csv, syn_tx.csv, and syn_national.csv deidentified dataset files are created from target datasets MA (ma2019.csv), TX (tx2019.csv), and NATIONAL(national2019.csv), respectively. You can use one of the toy deidentified dataset files for testing whether the sdnist.report package is installed correctly on your system.
+
+
+6. Use the following commands for generating reports if you are using a toy deidentified dataset file:
+
+   For evaluating the Massachusetts dataset:
+   ```
+   (venv) c:\\sdnist-project> python -m sdnist.report toy_deidentified_data/syn_ma.csv MA
+   ```
+
+   For evaluating the Texas dataset:
+   ```
+   (venv) c:\\sdnist-project> python -m sdnist.report toy_deidentified_data/syn_tx.csv TX
+   ```
+
+   For evaluating the national dataset:
+   ```
+   (venv) c:\\sdnist-project> python -m sdnist.report toy_deidentified_data/syn_national.csv NATIONAL
+   ```
+
+7.  A deidentified dataset can be a .csv or a parquet file, and the path of this file is required
+by the sdnist.report package to generate a data quality report.
+
+
+Download Data Manually
+----------------------
+
+1.  If the sdnist.report package is not able to download the datasets, you can download them from Github [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.3.0/diverse_communities_data_excerpts.zip).
+3.  Unzip the **diverse_community_excerpts_data.zip** file and move the unzipped **diverse_community_excerpts_data** directory to the **sdnist-project** directory.
+4.  Delete the **diverse_community_excerpts_data.zip** file once the data is successfully extracted from the zip.
+
+Citing SDNist Deidentified Data Report Tool
+-------------------------------------------
+
+If you publish work that utilizes the SDNist Deidentified Data Tool, please cite the software. Citation recommendation:  
+> Task C., Bhagat K., and Howarth G.S. (2023), SDNist v2: Deidentified Data Report Tool, 
+> National Institute of Standards and Technology, 
+> https://doi.org/10.18434/mds2-2943.
+
+Credits 
+----------
+
+- [Christine Task](mailto:christine.task@knexusresearch.com) - Project technical lead - christine.task@knexusresearch.com
+- [Karan Bhagat](https://github.com/kbtriangulum) - Contributor
+- [David Lee](https://www.linkedin.com/in/david-lee-13872922/) - Documentation
+- [Gary Howarth](https://www.nist.gov/people/gary-howarth) - Project PI - gary.howarth@nist.gov
```

### Comparing `sdnist-2.2.0/README.md` & `sdnist-2.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,22 @@
-# SDNist v2.2: Deidentified Data Report Tool
+Metadata-Version: 2.1
+Name: sdnist
+Version: 2.3.0
+Summary: SDNist: Deidentified Data Report Generator
+Home-page: https://github.com/usnistgov/SDNist
+Author: National Institute of Standards and Technology
+Author-email: gary.howarth@nist.gov
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: Public Domain
+Classifier: Intended Audience :: Science/Research
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# SDNist v2.3: Deidentified Data Report Tool
 
 ## [SDNist is the offical software package for engaging in the NIST Collaborative Research Cycle](https://pages.nist.gov/privacy_collaborative_research_cycle)
 
 Welcome! SDNist is a python package that provides benchmark data and evaluation metrics for deidentified data generators. This version of SDNist supports using the [NIST Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/tree/main/nist%20diverse%20communities%20data%20excerpts), a geographically partioned, limited feature data set.
 
 The deidentified data report evaluates utility and privacy of a given deidentified dataset and generates a summary quality report with performance of a deidentified dataset enumerated and illustrated for each utility and privacy metric.
 
@@ -14,14 +28,18 @@
 ### Project Team  
 **Karan Bhagat**, *Knexus Research* - Developer *sdnist.report* package  
 
 **Christine Task**, *Knexus Research* - Project technical lead
 
 **Gary Howarth**, *NIST* - Project PI [gary.howarth@nist.gov](mailto:gary.howarth@nist.gov)
 
+### Acknowledgements
+
+SDNist v2 grew from [SDNist v1](https://github.com/usnistgov/Differential-Privacy-Temporal-Map-Challenge-assets), developed in partnership with Saurus Technologies under CRADA CN-21-0143.
+
 ### Reporting Issues
 Help us improve the package and this guide by reporting issues [here](https://github.com/usnistgov/SDNist/issues).
 
 ### Temporal Map Challenge Environment
 
 SDNist v2.0 and above does not support the Temporal Map Challenge environment.
 
@@ -29,20 +47,21 @@
 
 
 Setting Up the SDNIST Report Tool
 ------------------------
 
 ### Brief Setup Instructions
 
-SDNist requires Python version 3.7 or greater. If you have installed a previous version of the SDNist library, we recommend uninstalling or installing v2.2 in a virtual environment. v2.2 can be installed via [Release 2.2](https://github.com/usnistgov/SDNist/releases/tag/v2.2.0). The NIST Diverse Community Exceprt data will download on the fly.
-```
-pip install sdnist
-```
+SDNist requires Python version 3.7 or greater. If you have installed a previous version of the SDNist library, we recommend installing v2.3 in a virtual environment. v2.3 can be installed via [Release 2.3](https://github.com/usnistgov/SDNist/releases/tag/v2.3.0) or via the Pypi server: `pip install sdnist` or, if you already have a version installed, `pip install --upgrade sdnist`.
+
+The NIST Diverse Community Exceprt data will download on the fly.
+
+
 
-### Detailed Setup Instructions
+### Detailed Setup Instructions Using Pypi
 
 1. The SDNist Report Tool is a part of the sdnist Python library that can be installed on a user’s MAC OS, Windows, or Linux machine.
 
 
 2. The sdnist library requires Python version 3.7 or greater to be installed on the user's machine. Check whether an installation exists on the machine by executing the following command in your terminal on Mac/Linux or powershell on Windows:
    ```
     c:\\> python -V
@@ -51,41 +70,33 @@
 
 
 3.  Create a local directory/folder on the machine to set up the SDNist library. This guide assumes the local directory to be sdnist-project; an example of a complete file path is c:\\sdnist-project:
     ```
     c:\\sdnist-project>     
     ```
 
-4.  Download the sdnist installable wheel (sdnist-2.2.0-py3-none-any.whl) from the Github: [Release 2.2](https://github.com/usnistgov/SDNist/releases/download/v2.2.0/sdnist-2.2.0-py3-none-any.whl).
-
-
-5.  Move the downloaded sdnist-2.2.0-py3-none-any.whl file to the sdnist-project directory.
-
-
-6.  Using the terminal on Mac/Linux or powershell on Windows, navigate to the sdnist-project directory.
-
 
-7.  In the already-opened terminal or powershell window, execute the following command to create a new Python environment. The sdnist library will be installed in this newly created Python environment:
+4. In the already-opened terminal or powershell window, execute the following command to create a new Python environment. The sdnist library will be installed in this newly created Python environment:
 
     ```
     c:\\sdnist-project> python -m venv venv
     ```
 
-8. The new Python environment will be created in the sdnist-project directory, and the files of the environment should be in the venv directory. To check whether a new Python environment was created successfully, use the following command to list all directories in the sdnist-project directory, and make sure the venv directory exists.
+5. The new Python environment will be created in the sdnist-project directory, and the files of the environment should be in the venv directory. To check whether a new Python environment was created successfully, use the following command to list all directories in the sdnist-project directory, and make sure the venv directory exists.
 
     **MAC OS/Linux:**
     ```
     sdnist-project> ls
     ```
     **Windows:**
     ```
     c:\\sdnist-project> dir
     ```
 
-9. Now activate the Python environment and install the sdnist library into it.
+6. Now activate the Python environment and install the sdnist library into it.
 
     **MAC OS/Linux:**
     ```
     sdnist-project> . venv/bin/activate
     ```
     The python virtual environment should now be activated. You should see environment name (**venv** in this case) appended to the terminal prompt as below:  
     ```
@@ -106,35 +117,20 @@
     C:\\sdnist-project\\venv\\Scripts\\Activate.ps1 cannot be loaded because running scripts is disabled on this system.
     ```
     Run the following command to let Windows execute scripts:
     ```
     Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope LocalMachine
     ```
 
-
-10. Per step 5 above, the sdnist-2.2.0-py3-none-any.whl file should already be present in the sdnist-project directory. Check whether that is true by listing the files in the sdnist-project directory.
-
-      **MAC OS/Linux:**
-       ```
-       (venv) sdnist-project> ls
+7. Install sdnist Python library:
        ```
-      **Windows:**
+       (venv) c:\\sdnist-project> pip install sdnist
        ```
-       (venv) c:\\sdnist-project> dir
-       ```
-       The sdnist-2.2.0-py3-none-any.whl file should be in the list printed by the above command; otherwise, follow steps 4 and 5 again to download the .whl file.
-
 
-11. Install sdnist Python library:
-       ```
-       (venv) c:\\sdnist-project> pip install sdnist-2.2.0-py3-none-any.whl
-       ```
-
-
-12. Installation is successful if executing the following command outputs a help menu for the sdnist.report package:
+8. Installation is successful if executing the following command outputs a help menu for the sdnist.report package:
        ```
        (venv) c:\\sdnist-project> python -m sdnist.report -h
        ```
        Output:
        ```
         usage: __main__.py [-h] [--labels LABELS] [--data-root DATA_ROOT]
                            PATH_DEIDENTIFIED_DATASET TARGET_DATASET_NAME
@@ -161,16 +157,15 @@
         Choices for Target Dataset Name:
           [DATASET NAME]        [FILENAME]
           MA                    ma2019
           TX                    tx2019
           NATIONAL              national2019
        ```
 
-
-13. These instructions install sdnist into a virtual environment. The virtual environment must be activated (step 9) each time a new terminal window is used with sdnist.
+9. These instructions install sdnist into a virtual environment. The virtual environment must be activated (step 9) each time a new terminal window is used with sdnist.
 
 
 Generate Data Quality Report
 ---------------------------
 
 1.  The sdnist.report package requires a path to the deidentified dataset file and the name of the target dataset from which the deidentified dataset file will be created. Following is the command line usage of the sdnist.report package:
       ```
@@ -248,26 +243,26 @@
       https://github.com/usnistgov/SDNist/releases/download/v2.2.0/diverse_communities_data_excerpts.zip ...  
       ...5%, 47352 KB, 8265 KB/s, 5 seconds elapsed
       ```
 
       Follow the next subsection, Download Data Manually, if the sdnist.report package is unable to download the datasets.
 
 
-2. All the datasets required by the sdnist.report package are installed into the sdnist _toy _data directory, which should be now present inside the sdnist-project directory. sdnist _toy _data is also a data root directory. You can use some other directory as a data root by providing the –data-root argument to the sdnist.report package. If you provide a –data-root argument with a path, the sdnist.report package will look for datasets in the data root directory you have specified, and the package will download it if it is not present in the data root.
+2. All the datasets required by the sdnist.report package are installed into the sdnist \_toy \_data directory, which should be now present inside the sdnist-project directory. sdnist \_toy \_data is also a data root directory. You can use some other directory as a data root by providing the –data-root argument to the sdnist.report package. If you provide a –data-root argument with a path, the sdnist.report package will look for datasets in the data root directory you have specified, and the package will download it if it is not present in the data root.
 
 
 3. The sdnist.report package also needs a deidentified dataset that it can evaluate against its original counterpart. Since the sdnist.report package comes bundled with the datasets, the deidentified dataset should be generated using the bundled datasets.
 
    You can download a copy of the datasets from Github [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/tree/main/nist%20diverse%20communities%20data%20excerpts). This copy is similar to the one bundled with the sdnist.report package, but it contains more documentation and a description of the datasets.
 
 
 4. You can download the toy deidentified datasets from Github [Sdnist Toy Deidentified Dataset](https://github.com/usnistgov/SDNist/releases/download/v2.1.1/toy_deidentified_data.zip). Unzip the downloaded file, and move the unzipped toy_deidentified_dataset directory to the sdnist-project directory.
 
 
-5. Each toy deidentified dataset file is generated using the [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.2.0/diverse_communities_excerpts_data.zip). The syn_ma.csv, syn_tx.csv, and syn_national.csv deidentified dataset files are created from target datasets MA (ma2019.csv), TX (tx2019.csv), and NATIONAL(national2019.csv), respectively. You can use one of the toy deidentified dataset files for testing whether the sdnist.report package is installed correctly on your system.
+5. Each toy deidentified dataset file is generated using the [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.3.0/diverse_communities_data_excerpts.zip). The syn_ma.csv, syn_tx.csv, and syn_national.csv deidentified dataset files are created from target datasets MA (ma2019.csv), TX (tx2019.csv), and NATIONAL(national2019.csv), respectively. You can use one of the toy deidentified dataset files for testing whether the sdnist.report package is installed correctly on your system.
 
 
 6. Use the following commands for generating reports if you are using a toy deidentified dataset file:
 
    For evaluating the Massachusetts dataset:
    ```
    (venv) c:\\sdnist-project> python -m sdnist.report toy_deidentified_data/syn_ma.csv MA
@@ -286,28 +281,26 @@
 7.  A deidentified dataset can be a .csv or a parquet file, and the path of this file is required
 by the sdnist.report package to generate a data quality report.
 
 
 Download Data Manually
 ----------------------
 
-1.  If the sdnist.report package is not able to download the datasets, you can download them from Github [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.2.0/diverse_communities_data_excerpts.zip).
+1.  If the sdnist.report package is not able to download the datasets, you can download them from Github [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.3.0/diverse_communities_data_excerpts.zip).
 3.  Unzip the **diverse_community_excerpts_data.zip** file and move the unzipped **diverse_community_excerpts_data** directory to the **sdnist-project** directory.
 4.  Delete the **diverse_community_excerpts_data.zip** file once the data is successfully extracted from the zip.
 
 Citing SDNist Deidentified Data Report Tool
 -------------------------------------------
 
 If you publish work that utilizes the SDNist Deidentified Data Tool, please cite the software. Citation recommendation:  
 > Task C., Bhagat K., and Howarth G.S. (2023), SDNist v2: Deidentified Data Report Tool, 
 > National Institute of Standards and Technology, 
-> https://doi.org/10.18434/mds2-2943    
-(NOTE: DOI is not yet active, but should be by 1 APR 2023).
+> https://doi.org/10.18434/mds2-2943.
 
 Credits 
 ----------
 
 - [Christine Task](mailto:christine.task@knexusresearch.com) - Project technical lead - christine.task@knexusresearch.com
 - [Karan Bhagat](https://github.com/kbtriangulum) - Contributor
 - [David Lee](https://www.linkedin.com/in/david-lee-13872922/) - Documentation
 - [Gary Howarth](https://www.nist.gov/people/gary-howarth) - Project PI - gary.howarth@nist.gov
-
```

### Comparing `sdnist-2.2.0/sdnist/__init__.py` & `sdnist-2.3.0/sdnist/__init__.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.2.0/sdnist/challenge/baseline.py` & `sdnist-2.3.0/sdnist/challenge/baseline.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.2.0/sdnist/challenge/submission.py` & `sdnist-2.3.0/sdnist/challenge/submission.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.2.0/sdnist/challenge/subsample.py` & `sdnist-2.3.0/sdnist/challenge/subsample.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.2.0/sdnist/load.py` & `sdnist-2.3.0/sdnist/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
 
 def check_exists(root: Path, name: Path, download: bool, data_name: str = strs.DATA):
     root = root.expanduser()
     if not name.exists():
         print(f"{name} does not exist.")
         zip_path = Path(root.parent, 'data.zip')
-        version = "2.2.0"
+        version = "2.3.0"
 
         version_v = f"v{version}"
         sdnist_version = DEFAULT_DATASET
 
         download_link = f"https://github.com/usnistgov/SDNist/releases/download/{version_v}/{sdnist_version}.zip"
         if zip_path.exists() and error_opening_zip(zip_path):
             os.remove(zip_path)
```

### Comparing `sdnist-2.2.0/sdnist/metrics/apparent_match_dist.py` & `sdnist-2.3.0/sdnist/metrics/apparent_match_dist.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.2.0/sdnist/metrics/hoc.py` & `sdnist-2.3.0/sdnist/metrics/hoc.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.2.0/sdnist/metrics/inconsistency.py` & `sdnist-2.3.0/sdnist/metrics/inconsistency.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,15 +264,15 @@
                     ic_data[4] = row_path
                     self.report_data['age']['inconsistencies'].append(
                         {'inconsistency_name': ic_data[0],
                          'inconsistency_description': ic_data[1],
                          'inconsistency_features': ic_data[2],
                          'inconsistency_violations': int(ic_data[3].split(' ')[0]),
                          'inconsistent_data_indexes': ic_dict[i[NAME]],
-                         'inconsistent_record_example': relative_path(row_path)}
+                         'inconsistent_record_example': relative_path(row_path, level=3)}
                     )
 
         # ------- Compute work-based Inconsistencies------------
         ic_work = dict()
         work_violators = set()  # set of records that have at least one work ic
 
         age_path = Path(self.out_path, 'work')
@@ -294,15 +294,15 @@
                     ic_data[4] = row_path
                     self.report_data['age']['inconsistencies'].append(
                         {'inconsistency_name': ic_data[0],
                          'inconsistency_description': ic_data[1],
                          'inconsistency_features': ic_data[2],
                          'inconsistency_violations': int(ic_data[3].split(' ')[0]),
                          'inconsistent_data_indexes': ic_dict[i[NAME]],
-                         'inconsistent_record_example': relative_path(row_path)}
+                         'inconsistent_record_example': relative_path(row_path, level=3)}
                     )
 
         # ------- Compute housing-based Inconsistencies------------
         ic_house = dict()
         house_violators = set()  # set of records that have at least one house ic
 
         age_path = Path(self.out_path, 'work')
@@ -324,15 +324,15 @@
                     ic_data[4] = row_path
                     self.report_data['age']['inconsistencies'].append(
                         {'inconsistency_name': ic_data[0],
                          'inconsistency_description': ic_data[1],
                          'inconsistency_features': ic_data[2],
                          'inconsistency_violations': int(ic_data[3].split(' ')[0]),
                          'inconsistent_data_indexes': ic_dict[i[NAME]],
-                         'inconsistent_record_example': relative_path(row_path)}
+                         'inconsistent_record_example': relative_path(row_path, level=3)}
                     )
 
         # -------- Compute overall stats---------------------
         # set of records that have at least one ic of any type
         total_violators = age_violators.union(work_violators).union(house_violators)
 
         overall_stats = [['Age', len(age_violators), round((100 * len(age_violators)) / n, 1)],
```

### Comparing `sdnist-2.2.0/sdnist/metrics/kmarg_old.py` & `sdnist-2.3.0/sdnist/metrics/kmarg_old.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.2.0/sdnist/metrics/kmarginal.py` & `sdnist-2.3.0/sdnist/metrics/kmarginal.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.2.0/sdnist/metrics/pca.py` & `sdnist-2.3.0/sdnist/metrics/pca.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,29 +44,28 @@
         self.comp_df = None
 
     def compute_pca(self):
         cc = 5
         t_pca = PCA(n_components=cc)
 
         tdf_v = self.tar.values
-        sdf = self.syn.apply(lambda x: x - x.mean())
-        sdf_v = sdf.values
-
-        tdf_v = StandardScaler().fit_transform(tdf_v)
-        sdf_v = StandardScaler().fit_transform(sdf_v)
+        sdf_v = self.syn.values
+        scaler = StandardScaler().fit(tdf_v)
+        sdf_v = scaler.transform(sdf_v)
+        tdf_v = scaler.transform(tdf_v)
 
         t_pc = t_pca.fit_transform(tdf_v)
 
         t_ev = np.array(t_pca.components_)
         s_pc = np.matmul(sdf_v, t_ev.T)
 
         self.t_comp_data = []
         for i, comp in enumerate(t_pca.components_):
             qc = [[n, round(v, 2)] for n, v in zip(self.tar.columns.tolist(), comp)]
-            qc = sorted(qc, key=lambda x: x[1], reverse=True)
+            qc = sorted(qc, key=lambda x: abs(x[1]), reverse=True)
             qc = [f'{v[0]} ({v[1]})' for v in qc]
             self.t_comp_data.append({"Principal Component": f"PC-{i}",
                                      "Features Contribution: "
                                      "feature-name (contribution ratio)": ','.join(qc[:5])})
 
         self.comp_df = pd.DataFrame(t_pca.components_,
                                     columns=self.tar.columns,
@@ -84,15 +83,17 @@
 
         self.t_pdf_s = self.t_pdf.copy()
         self.s_pdf_s = self.s_pdf.copy()
 
         for c in self.t_pdf.columns:
             self.t_pdf_s[c] = min_max_scaling(self.t_pdf[c])
         for c in self.s_pdf.columns:
-            self.s_pdf_s[c] = min_max_scaling(self.s_pdf[c])
+            self.s_pdf_s[c] = min_max_scaling(self.s_pdf[c],
+                                              self.t_pdf[c].min(),
+                                              self.t_pdf[c].max())
 
     def plot(self, output_directory: Path) -> Dict[str, any]:
         s = time.time()
         plot_paths = dict()
         o_path = output_directory
         # individual component pair plot output path
         t_cp_o_path = Path(o_path, 'target_individual_components')
@@ -148,16 +149,21 @@
         # clear temporary data from report data
         remove_path(t_cp_o_path)
         remove_path(s_cp_o_path)
 
         return plot_paths
 
 
-def min_max_scaling(series):
-    return (series - series.min()) / (series.max() - series.min())
+def min_max_scaling(series, min_val=None, max_val=None):
+    if min_val is None:
+        min_val = series.min()
+    if max_val is None:
+        max_val = series.max()
+
+    return (series - min_val) / (max_val - min_val)
 
 
 def plot_all_components_pairs(title: str,
                               data: pd.DataFrame,
                               file_path: Path,
                               component_pairs_path: Path,
                               color='b',):
```

### Comparing `sdnist-2.2.0/sdnist/metrics/pearson_correlation.py` & `sdnist-2.3.0/sdnist/metrics/pearson_correlation.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.2.0/sdnist/metrics/propensity.py` & `sdnist-2.3.0/sdnist/metrics/propensity.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.2.0/sdnist/metrics/regression.py` & `sdnist-2.3.0/sdnist/metrics/regression.py`

 * *Files 5% similar despite different names*

```diff
@@ -212,17 +212,18 @@
         plt.suptitle('Comparison between ')
         plt.close()
 
         # --------- saves regression metric statistics to json report dictionary
         self.report_data = {
             "target_counts": relative_path(save_data_frame(self.tcm,
                                                            self.o_path,
-                                                           'target_counts')),
+                                                           'target_counts'), level=3),
             "target_deidentified_counts_difference": relative_path(save_data_frame(self.diff,
                                                                 self.o_path,
-                                                                "target_deidentified_counts_difference")),
-            "target_deidentified_difference_plot": relative_path(file_path),
+                                                                "target_deidentified_counts_difference"),
+                                                                   level=3),
+            "target_deidentified_difference_plot": relative_path(file_path, level=3),
             "target_regression_slope_and_intercept": (self.t_slope, self.t_intercept),
             "deidentified_regression_slope_and_intercept": (self.s_slope, self.s_intercept)
         }
 
         return [file_path]
```

### Comparing `sdnist-2.2.0/sdnist/metrics/unique_exact_matches.py` & `sdnist-2.3.0/sdnist/metrics/unique_exact_matches.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,41 +2,42 @@
 from pathlib import Path
 
 from sdnist.load import TestDatasetName
 
 from sdnist.report.dataset import Dataset
 import sdnist.utils as u
 
+
 def unique_exact_matches(target_data: pd.DataFrame, deidentified_data: pd.DataFrame):
     td, dd = target_data, deidentified_data
     cols = td.columns.tolist()
 
     # select rows that are unique in the target data
     u_td = td.loc[td.groupby(by=cols)[cols[0]].transform('count') == 1, :]
 
     # target unique records
     t_unique_records = u_td.shape[0]
     perc_t_unique_records = round(t_unique_records/td.shape[0] * 100, 2)
 
     # Keep only one copy of each duplicate row in the deidentified data
-    # and also save the count of each row in the deidentified data
-    dd= dd.drop_duplicates(subset=cols)
+    dd = dd.drop_duplicates(subset=cols)
 
     merged = u_td.merge(dd, how='inner', on=cols)
 
     # number of unique target records that exactly match in deidentified data
     t_rec_matched = merged.shape[0]
 
     # percent of unique target records that exactly match in deidentified data
-    perc_t_rec_matched = t_rec_matched/td.shape[0] * 100
+    perc_t_rec_matched = t_rec_matched/t_unique_records * 100
 
     perc_t_rec_matched = round(perc_t_rec_matched, 2)
 
     return t_rec_matched, perc_t_rec_matched, t_unique_records, perc_t_unique_records
 
+
 if __name__ == '__main__':
     THIS_DIR = Path(__file__).parent
     s_path = Path(THIS_DIR, '..', '..',
                   'toy_synthetic_data/syn/sdcmicro/k_ano_k_6.csv')
     log = u.SimpleLogger()
     dataset_name = TestDatasetName.national2019
     d = Dataset(s_path, log, dataset_name)
```

### Comparing `sdnist-2.2.0/sdnist/report/__main__.py` & `sdnist-2.3.0/sdnist/report/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,21 +15,22 @@
 from sdnist.load import TestDatasetName
 
 from sdnist.strs import *
 from sdnist.utils import *
 
 from sdnist.load import DEFAULT_DATASET
 
+
 def run(synthetic_filepath: Path,
         output_directory: Path = REPORTS_DIR,
         dataset_name: TestDatasetName = TestDatasetName.NONE,
         data_root: Path = Path(DEFAULT_DATASET),
         labels_dict: Optional[Dict] = None,
         download: bool = False,
-        test_mode: bool = False):
+        show_report: bool = True):
     outfile = Path(output_directory, 'report.json')
     ui_data = ReportUIData(output_directory=output_directory)
     report_data = ReportData(output_directory=output_directory)
     log = SimpleLogger()
     log.msg('SDNist: Deidentified Data Report Tool', level=0, timed=False)
     log.msg(f'Creating Evaluation Report for Deidentified Data at path: {synthetic_filepath}',
             level=1)
@@ -56,18 +57,19 @@
         report_data.save()
         log.end_msg()
     else:
         with open(outfile, 'r') as f:
             ui_data = json.load(f)
     log.end_msg()
     # Generate Report
-    generate(ui_data, output_directory, test_mode)
+    generate(ui_data, output_directory, show_report)
     log.msg(f'Reports available at path: {output_directory}', level=0, timed=False,
             msg_type='important')
 
+
 def setup():
     bundled_datasets = {"MA": TestDatasetName.ma2019,
                         "TX": TestDatasetName.tx2019,
                         "NATIONAL": TestDatasetName.national2019}
     parser = argparse.ArgumentParser()
     parser.register('action', 'none', NoAction)
     parser.add_argument("deidentified_dataset", type=argparse.FileType("r"),
```

### Comparing `sdnist-2.2.0/sdnist/report/config.json` & `sdnist-2.3.0/sdnist/report/config.json`

 * *Files identical despite different names*

### Comparing `sdnist-2.2.0/sdnist/report/dataset/__init__.py` & `sdnist-2.3.0/sdnist/report/dataset/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,38 +50,32 @@
     if 'k_marginal' in cnf and 'group_features' in cnf['k_marginal']:
         for f in cnf['k_marginal']['group_features'].copy():
             if f not in fl:
                 cnf['k_marginal']['group_features'].remove(f)
 
     return cnf
 
-def compute_feature_space(data_dict: Dict,
-                          features: List[str]):
-    # list of features and their value length
-    f_list = []
-    for f in features:
-        if "values" not in data_dict[f]:
-            vals = [0] * 269  # in case of INDP feature
-        else:
-            vals = data_dict[f]["values"]
-        if "min" in vals and f != 'AGEP':
-            continue
-        if f == 'AGEP':
-            f_list.append([f, 100])
-        else:
-            f_list.append([f, len(vals)])
 
-    f_df = pd.DataFrame(f_list, columns=['feature', 'len'])
-    f_df = f_df.sort_values(by='len')
+def feature_space_size(target_df: pd.DataFrame, data_dict: Dict):
+    size = 1
+
+    for col in target_df.columns:
+        if col in ['PINCP', 'POVPIP', 'WGTP', 'PWGTP', 'AGEP']:
+            size = size * 100
+        elif col in ['SEX', 'MSP', 'HISP', 'RAC1P', 'HOUSING_TYPE', 'OWN_RENT',
+                     'INDP_CAT', 'EDU', 'PINCP_DECILE', 'DVET', 'DREM', 'DPHY', 'DEYE',
+                     'DEAR']:
+            size = size * len(data_dict[col]['values'])
+        elif col in ['PUMA', 'DENSITY']:
+            size = size * len(target_df['PUMA'].unique())
+        elif col in ['NOC', 'NPF', 'INDP']:
+            size = size * len(target_df[col].unique())
 
-    # get product of all feature lengths
-    n_features = f_df['len'].astype(object).product()
+    return size
 
-    # return number of features and sorted list of features
-    return n_features
 
 @dataclass
 class Dataset:
     synthetic_filepath: Path
     log: u.SimpleLogger
     test: TestDatasetName = TestDatasetName.NONE
     data_root: Path = Path(DEFAULT_DATASET)
@@ -155,31 +149,37 @@
         self.synthetic_data = self.synthetic_data[common_columns]
 
         ind_features = [c for c in self.target_data.columns.tolist()
                         if c.startswith('IND_')]
         self.features = list(set(self.features).difference(set(ind_features)))
         self.features = list(set(self.features).intersection(list(common_columns)))
 
-        self.feature_space = compute_feature_space(self.data_dict, self.features)
-
         # raw subset data
         self.target_data = self.target_data[self.features]
         self.synthetic_data = self.synthetic_data[self.features]
 
+        self.feature_space = feature_space_size(self.target_data, self.data_dict)
+
         # validation and clean data
         self.c_synthetic_data, self.validation_log = \
             validate(self.synthetic_data, self.data_dict, self.features, self.log)
         self.c_target_data, _ = \
             validate(self.target_data, self.data_dict, self.features, self.log)
         self.features = self.c_synthetic_data.columns.tolist()
 
         # update data after validation and cleaning
         self.synthetic_data = self.synthetic_data[self.features]
         self.target_data = self.target_data[self.features]
 
+        # for f in self.target_data.columns:
+        #     if f not in ['PINCP', 'INDP', 'PWGTP', 'WGTP', 'POVPIP', 'DENSITY']:
+        #         print('T', f, self.target_data[f].unique().tolist())
+        #         print('S', f, self.synthetic_data[f].unique().tolist())
+        #         print()
+
         # sort columns in the data
         self.target_data = self.target_data.reindex(sorted(self.target_data.columns), axis=1)
         self.synthetic_data = self.synthetic_data.reindex(sorted(self.target_data.columns), axis=1)
         self.c_synthetic_data = self.c_synthetic_data.reindex(sorted(self.target_data.columns), axis=1)
         self.c_target_data = self.c_target_data.reindex(sorted(self.target_data.columns), axis=1)
         self.features = self.synthetic_data.columns.tolist()
 
@@ -295,21 +295,26 @@
 
     # create data dictionary appendix attachments
     dd_as = []
     for feat in dataset.data_dict.keys():
         f_desc = dataset.data_dict[feat]['description']
         feat_title = f'{feat}: {f_desc}'
         if 'link' in dataset.data_dict[feat] and feat == 'INDP':
-            data = f"<a href={dataset.data_dict[feat]['link']}>" \
+            data_1 = f"<a href={dataset.data_dict[feat]['link']}>" \
                    f"See codes in ACS data dictionary.</a> " \
                    f"Find codes by searching the string: {feat}, in " \
                    f"the ACS data dictionary"
             dd_as.append(Attachment(name=feat_title,
-                                    _data=data,
+                                    _data=data_1,
                                     _type=AttachmentType.String))
+            if "details" in dataset.data_dict[feat]:
+                data_2 = dataset.data_dict[feat]['details']
+                dd_as.append(Attachment(name=None,
+                                        _data=data_2,
+                                        _type=AttachmentType.String))
 
         elif 'values' in dataset.data_dict[feat]:
             f_name = feat_title
             if 'link' in dataset.data_dict[feat] and feat in ['WGTP', 'PWGTP']:
                 s_data = f"<a href={dataset.data_dict[feat]['link']}>" \
                        f"See description of weights.</a>"
                 dd_as.append(Attachment(name=f_name,
```

### Comparing `sdnist-2.2.0/sdnist/report/dataset/binning.py` & `sdnist-2.3.0/sdnist/report/dataset/binning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Dict, List
 import pandas as pd
 import numpy as np
 import math
 
+
 def percentile_rank_target(data: pd.DataFrame, features: List[str]):
     data = data.copy()
     for c in features:
         if c not in data.columns:
             continue
 
         if c == 'POVPIP':
```

### Comparing `sdnist-2.2.0/sdnist/report/dataset/transform.py` & `sdnist-2.3.0/sdnist/report/dataset/transform.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.2.0/sdnist/report/dataset/validate.py` & `sdnist-2.3.0/sdnist/report/dataset/validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Dict, Optional, List
 import pandas as pd
 
 from sdnist.utils import SimpleLogger
 
+
 def validate(synth_data: pd.DataFrame,
              data_dict: Dict,
              features: List[str],
              log: Optional[SimpleLogger] = None):
     """
     Removes all columns with the out of bound values.
     """
```

### Comparing `sdnist-2.2.0/sdnist/report/generate.py` & `sdnist-2.3.0/sdnist/report/generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,39 +75,44 @@
 #     page.loadFinished.connect(handle_load_finished)
 #     page.load(QtCore.QUrl.fromLocalFile(html))
 #     app.exec_()
 
 
 def generate(report_data: Dict[str, any],
              output_directory_path: Path,
-             test_mode: bool = False):
+             show_report: bool = True):
     out_dir = output_directory_path
     data = report_data
 
+    def debug(text):
+        print(text)
+        return ''
+
     env = Environment(loader=FileSystemLoader(Path(FILE_DIR, 'resources/templates')))
+    env.filters['debug'] = debug
     env.globals["enumerate"] = enumerate
 
     main_template = env.get_template('main.jinja2')
 
     out = main_template.render(data=data)
 
     out_path = Path(out_dir, 'report.html')
     out_pdf_path = Path(out_dir, 'report.pdf')
 
     with open(out_path, 'w') as f:
         f.write(out)
 
-    if not test_mode:
+    if show_report:
         webbrowser.open(f"file://{out_path}", new=True)
     # html_to_pdf(out_path, out_pdf_path)
 
 
 if __name__ == "__main__":
     h_p = Path(FILE_DIR, '../../reports/TX_ACS_EXCERPT_2019_08-02-2022T15.14.12/report.html')
     p_p = Path(FILE_DIR, '../../reports/TX_ACS_EXCERPT_2019_08-02-2022T15.14.12/report.pdf')
     p_o = Path(FILE_DIR, '../../reports/TX_ACS_EXCERPT_2019_08-02-2022T15.14.12/report0.pdf')
 
-    html_to_pdf_2(h_p, p_p)
+    # html_to_pdf_2(h_p, p_p)
```

### Comparing `sdnist-2.2.0/sdnist/report/plots/apparent_match_dist.py` & `sdnist-2.3.0/sdnist/report/plots/apparent_match_dist.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.2.0/sdnist/report/plots/correlation.py` & `sdnist-2.3.0/sdnist/report/plots/correlation.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.2.0/sdnist/report/plots/grid.py` & `sdnist-2.3.0/sdnist/report/plots/grid.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.2.0/sdnist/report/plots/pearson_correlation.py` & `sdnist-2.3.0/sdnist/report/plots/pearson_correlation.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,22 +20,23 @@
 
     def _setup(self):
         if not self.o_dir.exists():
             raise Exception(f'Path {self.o_dir} does not exist. Cannot save plots')
         if not self.o_path.exists():
             os.mkdir(self.o_path)
 
-    def save(self) -> List[Path]:
+    def save(self, path_level=2) -> List[Path]:
         file_path = Path(self.o_path, 'pearson_corr_diff.jpg')
 
         self.report_data = {
             "correlation_difference": relative_path(save_data_frame(self.cd,
                                                                     self.o_path,
-                                                                    'correlation_difference')),
-            "plot": relative_path(file_path)
+                                                                    'correlation_difference'),
+                                                     level=path_level),
+            "plot": relative_path(file_path, level=path_level)
         }
         cd = self.cd
         cd = cd.abs()
         fig = plt.figure(figsize=(6, 6), dpi=100)
         v_max = 0.15
         plt.imshow(cd, cmap='Blues', interpolation='none', vmin=0, vmax=v_max)
         im_ratio = cd.shape[0] / cd.shape[1]
```

### Comparing `sdnist-2.2.0/sdnist/report/plots/propensity.py` & `sdnist-2.3.0/sdnist/report/plots/propensity.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,21 @@
             os.mkdir(self.o_path)
 
     def save(self,
              filename: str = 'propensity_distribution',
              title: str = 'Distribution of data samples over 100 propensity bins') \
             -> List[Path]:
         file_path = Path(self.o_path, f'{filename}.jpg')
-        ax = self.p_dist.plot(title=title, xlabel="100 Propensity Bins", ylabel='Record Counts')
+        ax = self.p_dist.plot(title=title,
+                              xlabel="100 Propensity Bins",
+                              ylabel='Record Counts',
+                              color=['mediumblue', 'limegreen'],
+                              alpha=0.8,
+                              lw=2,
+                              figsize=(12, 6))
         fig = ax.get_figure()
         fig.savefig(file_path)
         self.report_data['plot'] = relative_path(file_path)
         return [file_path]
 
 
 class PropensityPairPlot:
```

### Comparing `sdnist-2.2.0/sdnist/report/plots/univariate.py` & `sdnist-2.3.0/sdnist/report/plots/univariate.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,21 +76,22 @@
         self.uni_counts = dict()  # univariate counts of target and synthetic data
 
     def _setup(self):
         if not self.o_dir.exists():
             raise Exception(f'Path {self.o_dir} does not exist. Cannot save plots')
         os.mkdir(self.out_path)
 
-    def report_data(self):
+    def report_data(self, level=2):
         return {"divergence": relative_path(save_data_frame(self.div_data,
                                                             self.out_path,
-                                                            'divergence')),
+                                                            'divergence'),
+                                            level=level),
                 "counts": self.uni_counts}
 
-    def save(self) -> Dict:
+    def save(self, level=2) -> Dict:
         if self.challenge == CENSUS:
             ignore_features = ['YEAR']
         elif self.challenge == TAXI:
             ignore_features = ['pickup_community_area', 'shift', 'company_id']
         else:
             raise Exception(f'Invalid Challenge Name: {self.challenge}. '
                             f'Unable to save univariate plots')
@@ -102,23 +103,25 @@
         # select 3 features with worst divergence
         # div_df = div_df.head(3)
 
         self.save_distribution_plot(self.dataset,
                                     self.syn,
                                     self.tar,
                                     div_df[FEATURE].tolist(),
-                                    self.out_path)
+                                    self.out_path,
+                                    level=level)
         return self.feat_data
 
     def save_distribution_plot(self,
                                dataset: Dataset,
                                synthetic: pd.DataFrame,
                                target: pd.DataFrame,
                                features: List,
-                               output_directory: Path):
+                               output_directory: Path,
+                               level=2):
         ds = dataset
         o_path = output_directory
         bar_width = 0.4
         saved_file_paths = []
         INDP = 'INDP'
         INDP_CAT = "INDP_CAT"
         o_tar = ds.target_data.loc[target.index]
@@ -134,34 +137,32 @@
                 # print(all_sectors)
                 for s in all_sectors:
                     if s == 'N':
                         continue
                     st_df = o_tar[o_tar[INDP_CAT].isin([s])].copy()
                     st_df.loc[:, f] = pd.to_numeric(st_df[f]).astype(int)
                     ss_df = o_syn[o_syn[INDP_CAT].isin([int(s)])]
-                    # print(s, type(s))
-                    # print(o_syn[INDP_CAT].unique().tolist())
+
                     unique_ind_codes = st_df[f].unique().tolist()
                     set(unique_ind_codes).update(set(ss_df[f].unique().tolist()))
                     unique_ind_codes = list(unique_ind_codes)
                     val_df = pd.DataFrame(unique_ind_codes, columns=[f])
+                    val_df[f] = val_df.astype(str)
 
                     t_counts_df = st_df.groupby(by=f)[f].size().reset_index(name='count_target')
                     s_counts_df = ss_df.groupby(by=f)[f].size().reset_index(name='count_deidentified')
-                    # print(s)
-                    # print(s_counts_df)
-                    # print(ss_df[f].unique().tolist())
-                    # print(ss_df.shape)
+                    t_counts_df[f] = t_counts_df[f].astype(str)
+                    s_counts_df[f] = s_counts_df[f].astype(str)
+
                     merged = pd.merge(left=val_df, right=t_counts_df, on=f, how='left')\
                         .fillna(0)
                     merged = pd.merge(left=merged, right=s_counts_df, on=f, how='left')\
                         .fillna(0)
                     div = l1(pk=merged['count_target'], qk=merged['count_deidentified'])
-                    # print(s)
-                    # print(merged[['count_target', 'count_deidentified']])
+
                     selected.append([merged, div, s])
                 selected = sorted(selected, key=lambda l: l[1], reverse=True)
 
                 for j, data in enumerate(selected):
                     merged = data[0]
                     div = data[1]
                     s = data[2]
@@ -188,16 +189,17 @@
                     plt.savefig(file_path, bbox_inches='tight')
 
                     plt.close()
                     self.uni_counts[f][f"Industry Category {s}"] = {
                         "divergence": div,
                         "counts": relative_path(save_data_frame(merged,
                                                 o_path,
-                                                f"Industry Category {s}")),
-                        "plot": relative_path(file_path)
+                                                f"Industry Category {s}"),
+                                                level=level),
+                        "plot": relative_path(file_path, level=level)
                     }
                     # if j < 2:
                     saved_file_paths.append(file_path)
 
                     self.feat_data[title] = {
                         "path": ''
                     }
@@ -221,16 +223,17 @@
                 c_vals = c_sort_merged['count_target'].head(2).values
                 c1, c2 = c_vals[0], c_vals[1]
 
 
                 self.uni_counts[f] = {
                     "counts": relative_path(save_data_frame(c_sort_merged.copy(),
                                                             o_path,
-                                                            f'{f}_counts')),
-                    "plot": relative_path(file_path)
+                                                            f'{f}_counts'),
+                                            level=level),
+                    "plot": relative_path(file_path, level)
                 }
 
                 if self.worst_univariates_to_display is None \
                         or i < self.worst_univariates_to_display:
                     self.feat_data[title] = dict()
                     if c1 >= c2*3 or f in ['PINCP']:
                         f_val = c_sort_merged.loc[0, f]
@@ -263,21 +266,22 @@
                             nv = min(mv)
                             updated_vals.append(nv)
                         else:
                             updated_vals.append(v)
                     vals = updated_vals
 
                 vals = [str(v) for v in vals]
+
                 if "-1" in vals:
                     idx = vals.index("-1")
                     vals[idx] = "N"
 
                 if f == 'PUMA':
                     f_val_dict = {i: v for i, v in enumerate(ds.schema[f]['values'])}
-                    vals = [f_val_dict[int(v)] for v in vals]
+                    vals = [f_val_dict[int(v)] if v != 'N' else 'N' for v in vals]
 
                 plt.gca().set_xticks(x_axis, vals)
                 plt.legend(loc='upper right')
                 plt.xticks(fontsize=8, rotation=45)
                 plt.tight_layout()
 
                 plt.title(title,
```

### Comparing `sdnist-2.2.0/sdnist/report/report_data.py` & `sdnist-2.3.0/sdnist/report/report_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import time
 from typing import List, Dict, Optional
 from dataclasses import dataclass, field
 from enum import Enum
 from pathlib import Path
 import datetime
 
 from sdnist.version import __version__
@@ -28,21 +29,27 @@
     WideTable = 'wide_table'
     ImageLinks = "image_links"
     ImageLinksHorizontal = "image_links_horizontal"
     String = 'string'
     ParaAndImage = 'para_and_image'
 
 
+
 @dataclass
 class Attachment:
     name: Optional[str]
     _data: any
+    group_id: int = -1
     _type: AttachmentType = field(default=AttachmentType.Table)
     dotted_break: bool = field(default=False)
 
+    def __post_init(self):
+        if self.group_id == -1:
+            self.group_id = int(time.time() * 100)
+
     @property
     def data(self) -> Dict[str, any]:
         d = self._data
         return {
             'name': self.name,
             'data': d,
             'type': self._type.value,
@@ -55,18 +62,24 @@
     metric_name: str
     score: Optional[float] = None
     attachment: List[Attachment] = field(default_factory=list)
     evaluation_type = None
 
     @property
     def data(self) -> Dict[str, any]:
+        attachments = dict()
+        for a in self.attachment:
+            if a.group_id in attachments:
+                attachments[a.group_id].append(a.data)
+            else:
+                attachments[a.group_id] = [a.data]
         d = {
             'metric_name': self.metric_name,
             'scores': self.score,
-            'attachments': [a.data for a in self.attachment]
+            'attachments': attachments
         }
         if self.score is None:
             del d['scores']
         return d
 
 
 class UtilityScorePacket(ScorePacket):
@@ -148,17 +161,20 @@
 class ReportUIData:
     output_directory: Path = REPORTS_DIR
     # dictionary containing description of datasets
     datasets: Dict[str, List[DataDescriptionPacket]] = field(default_factory=dict, init=False)
     feature_desc: Dict[str, any] = field(default_factory=dict, init=False)
     # list containing ScorePacket objects
     scores: List[ScorePacket] = field(default_factory=list, init=False)
+    key_val_pairs: Dict[str, any] = field(default_factory=dict, init=False)
 
     def add(self, score_packet: ScorePacket):
         self.scores.append(score_packet)
+    def add_key_val(self, key: str, val: any):
+        self.key_val_pairs[key] = val
 
     def add_data_description(self,
                              dataset_type: DatasetType,
                              data_description: DataDescriptionPacket):
         if dataset_type.value in self.datasets:
             self.datasets[dataset_type.value].append(data_description)
         else:
@@ -188,14 +204,16 @@
             d[strs.DATA_DESCRIPTION][k] = v.data
 
         d[EvaluationType.Utility.value] = []
         d[EvaluationType.Privacy.value] = []
         d['comparisons'] = []
         d['motivation'] = []
         d['observations'] = []
+        for k, v in self.key_val_pairs.items():
+            d[k] = v
 
         for s_pkt in self.scores:
             if s_pkt.evaluation_type == EvaluationType.Utility:
                 d[EvaluationType.Utility.value].append(s_pkt.data)
             elif s_pkt.evaluation_type == EvaluationType.Privacy:
                 d[EvaluationType.Privacy.value].append(s_pkt.data)
             elif s_pkt.evaluation_type == EvaluationType.Meta:
```

### Comparing `sdnist-2.2.0/sdnist/report/resources/templates/main.jinja2` & `sdnist-2.3.0/sdnist/report/resources/templates/main.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -380,66 +380,70 @@
 {% endmacro %}
 
 {% macro evaluation(data) %}
     {{ heading_2(data['metric_name']) }}
     {% if 'scores' in data %}
         <p>Score: {{ data['scores'] }}</p>
     {% endif %}
-    {% for i, a in enumerate(data['attachments']) %}
-        {% if a.type == 'image_links' and i > 0 %}
-            {% set style = 'attachment-div-break' %}
-        {% else %}
-            {% set style = 'attachment-div' %}
-        {% endif %}
+    {% for group, attachments in data['attachments'].items() %}
+        <div>
+            {% for i, a in enumerate(attachments) %}
+                {% if a.type == 'image_links' and i > 0 %}
+                    {% set style = 'attachment-div-break' %}
+                {% else %}
+                    {% set style = 'attachment-div' %}
+                {% endif %}
 
-        {% if a.dotted_break == True and i != data['attachments']|length - 1 %}
-            {% set dashed_line = 'dashed-line' %}
-        {% else %}
-            {% set dashed_line = '' %}
-        {% endif %}
+                {% if a.dotted_break == True and i != data['attachments']|length - 1 %}
+                    {% set dashed_line = 'dashed-line' %}
+                {% else %}
+                    {% set dashed_line = '' %}
+                {% endif %}
 
-        <div class="{{ style }} {{ dashed_line }}">
-            {% if a.name and a.name != '--no-brake--' %}
-                <br>
-                {{ heading_3(a.name) }}
-            {% elif a.name == None %}
-                <br>
-            {% endif %}
-            {% if a.type == "table" %}
-                {{ table(a.data) }}
-            {% elif a.type == "wide_table" %}
-                {{ wide_table(a.data) }}
-            {% elif a.type == "image_links" %}
-                {{ draw_images(a.data) }}
-            {% elif a.type == "image_links_horizontal" %}
-                {{ draw_images_horizontal(a.data) }}
-            {% elif a.type == "string" %}
-                {{ string_data(a.data) }}
-            {% elif a.type == "para_and_image" %}
-                <div class="float-container">
-                    <div class="float-child-left">
-                        {% for d in a.data['para'] %}
-                            {% if d[0] == 'heading' %}
-                                {{ string_data('h4' + d[1]) }}
-                            {%  elif d[0] == 'text' %}
-                                {{ string_data(d[1]) }}
-                            {% endif %}
-                        {% endfor %}
-                    </div>
-                    <div class="float-child-right">
-                        {{ draw_images(a.data['image']) }}
-                    </div>
+                <div class="{{ style }} {{ dashed_line }}">
+                    {% if a.name and a.name != '--no-brake--' %}
+                        <br>
+                        {{ heading_3(a.name) }}
+                    {% elif a.name == None %}
+                        <br>
+                    {% endif %}
+                    {% if a.type == "table" %}
+                        {{ table(a.data) }}
+                    {% elif a.type == "wide_table" %}
+                        {{ wide_table(a.data) }}
+                    {% elif a.type == "image_links" %}
+                        {{ draw_images(a.data) }}
+                    {% elif a.type == "image_links_horizontal" %}
+                        {{ draw_images_horizontal(a.data) }}
+                    {% elif a.type == "string" %}
+                        {{ string_data(a.data) }}
+                    {% elif a.type == "para_and_image" %}
+                        <div class="float-container">
+                            <div class="float-child-left">
+                                {% for d in a.data['para'] %}
+                                    {% if d[0] == 'heading' %}
+                                        {{ string_data('h4' + d[1]) }}
+                                    {%  elif d[0] == 'text' %}
+                                        {{ string_data(d[1]) }}
+                                    {% endif %}
+                                {% endfor %}
+                            </div>
+                            <div class="float-child-right">
+                                {{ draw_images(a.data['image']) }}
+                            </div>
+                        </div>
+                    {% endif %}
                 </div>
-            {% endif %}
+        {#        {% if a.dotted_break == True %}#}
+        {#            <div>#}
+        {#                <hr class="dashed-line">#}
+        {#            </div>#}
+        {#        {% endif %}#}
+            {% endfor %}
         </div>
-{#        {% if a.dotted_break == True %}#}
-{#            <div>#}
-{#                <hr class="dashed-line">#}
-{#            </div>#}
-{#        {% endif %}#}
     {% endfor %}
 {% endmacro %}
 
 
 <body>
     <div class="content-area">
         <div class="main-title">
@@ -484,16 +488,22 @@
                     {{ evaluation(item) }}
                 </div>
             {% endfor %}
         </div>
         <br>
         <div class="heading-2-div">
             {{ section_title('Privacy Evaluation') }}
-            {% for item in data['privacy'] %}
+            {% for i, item in enumerate(data['privacy']) %}
                 <div class="evaluation-div">
+                    {% if i > 0 %}
+                        <br>
+                        <br>
+                        <div class="section-separator-bar"></div>
+                        <br>
+                    {% endif %}
                     {{ evaluation(item) }}
                 </div>
             {% endfor %}
         </div>
         <br>
             <div class="heading-2-div">
             {{ section_title('Appendix') }}
```

#### html2text {}

```diff
@@ -52,19 +52,20 @@
 {% for i, part in enumerate(parts) %} {% if i%2 == 0 %} {{ part }} {% else %}
 {{ part }}  {% endif %} {% endfor %}
 {% else %}
 {{ data }}
 {% endif %} {% endmacro %} {% macro evaluation(data) %} {{ heading_2(data
 ['metric_name']) }} {% if 'scores' in data %}
 Score: {{ data['scores'] }}
-{% endif %} {% for i, a in enumerate(data['attachments']) %} {% if a.type ==
-'image_links' and i > 0 %} {% set style = 'attachment-div-break' %} {% else %}
-{% set style = 'attachment-div' %} {% endif %} {% if a.dotted_break == True and
-i != data['attachments']|length - 1 %} {% set dashed_line = 'dashed-line' %} {%
-else %} {% set dashed_line = '' %} {% endif %}
+{% endif %} {% for group, attachments in data['attachments'].items() %}
+{% for i, a in enumerate(attachments) %} {% if a.type == 'image_links' and i >
+0 %} {% set style = 'attachment-div-break' %} {% else %} {% set style =
+'attachment-div' %} {% endif %} {% if a.dotted_break == True and i != data
+['attachments']|length - 1 %} {% set dashed_line = 'dashed-line' %} {% else %}
+{% set dashed_line = '' %} {% endif %}
 {% if a.name and a.name != '--no-brake--' %}
 {{ heading_3(a.name) }} {% elif a.name == None %}
 {% endif %} {% if a.type == "table" %} {{ table(a.data) }} {% elif a.type ==
 "wide_table" %} {{ wide_table(a.data) }} {% elif a.type == "image_links" %} {
 { draw_images(a.data) }} {% elif a.type == "image_links_horizontal" %} {
 { draw_images_horizontal(a.data) }} {% elif a.type == "string" %} {
 { string_data(a.data) }} {% elif a.type == "para_and_image" %}
@@ -73,15 +74,16 @@
 endfor %}
 {{ draw_images(a.data['image']) }}
 {% endif %}
 {# {% if a.dotted_break == True %}#} {#
 #} {#
 ===============================================================================
 #} {#
-#} {# {% endif %}#} {% endfor %} {% endmacro %}
+#} {# {% endif %}#} {% endfor %}
+{% endfor %} {% endmacro %}
 ****** Data Evaluation Report ******
 
 Report created on: {{ data['Created on'] }}
 Created with SDNIST_v{{_data['version']_}}
 {{ section_title('Data Description') }} {% if 'synthetic' in data
 ['data_description'] %} {% for i, _ in enumerate(data['data_description']
 ['synthetic']) %} {% set ddict=data['data_description'] %} {{ data_description
@@ -95,15 +97,19 @@
 ['utility']) %}
 {% if i > 0 %}
 
 
 {% endif %} {{ evaluation(item) }}
 {% endfor %}
 
-{{ section_title('Privacy Evaluation') }} {% for item in data['privacy'] %}
-{{ evaluation(item) }}
+{{ section_title('Privacy Evaluation') }} {% for i, item in enumerate(data
+['privacy']) %}
+{% if i > 0 %}
+
+
+{% endif %} {{ evaluation(item) }}
 {% endfor %}
 
 {{ section_title('Appendix') }} {% for item in data['Appendix'] %}
 {{ evaluation(item) }}
 {% endfor %}
 {# a comment #}
```

### Comparing `sdnist-2.2.0/sdnist/report/score/paragraphs.py` & `sdnist-2.3.0/sdnist/report/score/paragraphs.py`

 * *Files 22% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                   "task, then the deidentified data must not be easy to distinguish from the target data. " \
                   "If the green line matches the blue line, then the deidentified data is high quality. " \
                   "Propensity based metrics have been developed by " \
                   "<a href='https://pennstate.pure.elsevier.com/en/publications/general-and-specific-utility-measures-for-synthetic-data'>" \
                   "Joshua Snoke and Gillian Raab</a> and <a href='https://www.researchgate.net/publication/323867757_STatistical_Election_to_Partition_Sequentially_STEPS_and_Its_Application_in_Differentially_Private_Release_and_Analysis_of_Youth_Voter_Registration_Data'>Claire Bowen</a>" \
                   ", all of whom have participated on the NIST Synthetic Data Challenges SME panels."
 
-k_marg_break_para = "In the metrics above we’ve considered all of the data together; " \
+k_marg_break_para = "In the metrics above we've considered all of the data together; " \
                     "however we know that algorithms may behave differently on different " \
                     "subgroups in the population. Below we look in more detail at deidentification " \
                     "performance just in the worst performing PUMA, based on k-marginal score."
 
 worst_k_marg_para = "Which are the worst performing PUMA?"
 
 rec_count_worst_para = "Did the deidentified versions of these PUMA have similar " \
@@ -74,11 +74,43 @@
                      "This distribution shows edit similarity between apparently matched pairs on how many of " \
                      "the 22 features does the deidentified record have the same value as the real record. " \
                      "If the distribution is centered near 100% that means these deidentified records largely " \
                      "mimic target records and are potentially leaking information about real individuals. " \
                      "If the distribution is centered below 50% that means the deidentified records are very " \
                      "different from the target records, and the apparent matches are not real matches."
 
-unique_exact_match_para = "This is a count of unique records in the target data that were exactly reproduced " \
-                          "in the deidentified data. Because these records were unique outliers in the " \
-                          "target data, and they still appear unchanged in the deidentified data, " \
-                          "they are potentially vulnerable to reidentification."
+unique_exact_match_para_1 = "Unique Exact Match (UEM) is a simple privacy metric that counts the " \
+                            "percentage of singleton records in the target that are also present in " \
+                            "the deidentified data; these uniquely identifiable individuals leaked " \
+                            "through the deidentification process."
+
+unique_exact_match_para_2 = "Below we also include an estimate of the feature space size. The feature " \
+                            "space is the set of all possible record values given the selected target " \
+                            "data and feature subset. For instance, if we had two features, Hat" \
+                            " [cap, bonnet] and Color [green, blue, purple], our feature space would " \
+                            "consist of 2 x 3 = 6 possible combinations (e.g. 'green cap', " \
+                            "'blue bonnet').  Note that feature spaces are based on the " \
+                            "feature set, not on what records actually exist in the data. " \
+                            "Purple bonnet is a possible combination in this feature space, " \
+                            "but it's likely no one in the hypothetical data owns a purple " \
+                            "bonnet (and the count of that record value would be 0)."
+
+unique_exact_match_para_3 = "As we add features to the feature set, we increase the size of the " \
+                            "feature space, but we don't change the actual number of records in " \
+                            "the data-- it's the same people, but now they're spread out more thinly " \
+                            "across a wider set of possible record values. Large feature spaces will " \
+                            "disperse populations very sparsely (most possible record values will have " \
+                            "count 0 or 1) and as a result the data will contain very many uniquely " \
+                            "identifiable records. Intuitively, once you know enough pieces of " \
+                            "information about someone, everyone becomes very distinct from everyone else. " \
+                            "This can pose a challenge for privacy. "
+
+unique_exact_match_para_4 = "The Target Data Properties below provides an estimate of the feature " \
+                            "space size (100 is used for continuous feature), " \
+                            "along with the portion of the records in the ground truth " \
+                            "target data that are unique (ie, they are the only person " \
+                            "with that record value, they have a count of 1). " \
+                            "The Deidentified Data Properties reports the percentage " \
+                            "of those uniquely identifiable individuals that are still " \
+                            "present in the deidentified data. " \
+                            "Because they are unique, real records, they are " \
+                            "potentially vulnerable to reidentification."
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -32,15 +32,15 @@
 deidentified data? " \ "If a classifier is trained to distinguish between the
 two data sets and it performs poorly on the " \ "task, then the deidentified
 data must not be easy to distinguish from the target data. " \ "If the green
 line matches the blue line, then the deidentified data is high quality. " \
 "Propensity based metrics have been developed by " \ ""_\_"Joshua_Snoke_and
 Gillian_Raab and Claire_Bowen" \ ", all of whom have participated on the NIST
 Synthetic Data Challenges SME panels." k_marg_break_para = "In the metrics
-above weâve considered all of the data together; " \ "however we know that
+above we've considered all of the data together; " \ "however we know that
 algorithms may behave differently on different " \ "subgroups in the
 population. Below we look in more detail at deidentification " \ "performance
 just in the worst performing PUMA, based on k-marginal score."
 worst_k_marg_para = "Which are the worst performing PUMA?" rec_count_worst_para
 = "Did the deidentified versions of these PUMA have similar " \ "population
 totals to the target versions? " univ_dist_worst_para = "Which features are
 performing the worst in each of these PUMA? " pear_corr_worst_para = "How are
@@ -61,12 +61,38 @@
 edit similarity between apparently matched pairs on how many of " \ "the 22
 features does the deidentified record have the same value as the real record. "
 \ "If the distribution is centered near 100% that means these deidentified
 records largely " \ "mimic target records and are potentially leaking
 information about real individuals. " \ "If the distribution is centered below
 50% that means the deidentified records are very " \ "different from the target
 records, and the apparent matches are not real matches."
-unique_exact_match_para = "This is a count of unique records in the target data
-that were exactly reproduced " \ "in the deidentified data. Because these
-records were unique outliers in the " \ "target data, and they still appear
-unchanged in the deidentified data, " \ "they are potentially vulnerable to
+unique_exact_match_para_1 = "Unique Exact Match (UEM) is a simple privacy
+metric that counts the " \ "percentage of singleton records in the target that
+are also present in " \ "the deidentified data; these uniquely identifiable
+individuals leaked " \ "through the deidentification process."
+unique_exact_match_para_2 = "Below we also include an estimate of the feature
+space size. The feature " \ "space is the set of all possible record values
+given the selected target " \ "data and feature subset. For instance, if we had
+two features, Hat" \ " [cap, bonnet] and Color [green, blue, purple], our
+feature space would " \ "consist of 2 x 3 = 6 possible combinations (e.g.
+'green cap', " \ "'blue bonnet'). Note that feature spaces are based on the " \
+"feature set, not on what records actually exist in the data. " \ "Purple
+bonnet is a possible combination in this feature space, " \ "but it's likely no
+one in the hypothetical data owns a purple " \ "bonnet (and the count of that
+record value would be 0)." unique_exact_match_para_3 = "As we add features to
+the feature set, we increase the size of the " \ "feature space, but we don't
+change the actual number of records in " \ "the data-- it's the same people,
+but now they're spread out more thinly " \ "across a wider set of possible
+record values. Large feature spaces will " \ "disperse populations very
+sparsely (most possible record values will have " \ "count 0 or 1) and as a
+result the data will contain very many uniquely " \ "identifiable records.
+Intuitively, once you know enough pieces of " \ "information about someone,
+everyone becomes very distinct from everyone else. " \ "This can pose a
+challenge for privacy. " unique_exact_match_para_4 = "The Target Data
+Properties below provides an estimate of the feature " \ "space size (100 is
+used for continuous feature), " \ "along with the portion of the records in the
+ground truth " \ "target data that are unique (ie, they are the only person " \
+"with that record value, they have a count of 1). " \ "The Deidentified Data
+Properties reports the percentage " \ "of those uniquely identifiable
+individuals that are still " \ "present in the deidentified data. " \ "Because
+they are unique, real records, they are " \ "potentially vulnerable to
 reidentification."
```

### Comparing `sdnist-2.2.0/sdnist/report/score/privacy.py` & `sdnist-2.3.0/sdnist/report/score/privacy.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,34 +18,44 @@
     rd = report_data
 
     log.msg('Unique Exact Matches', level=3)
     t_rec_matched, perc_t_rec_matched, \
         unique_target_records, perc_unique_target_records = \
         unique_exact_matches(ds.c_target_data, ds.c_synthetic_data)
     perc_t_rec_matched = perc_t_rec_matched
-    uem_para_a = Attachment(name=None,
-                            _data=unique_exact_match_para,
+    uem_para1_a = Attachment(name=None,
+                            _data=unique_exact_match_para_1,
+                            _type=AttachmentType.String)
+    uem_para2_a = Attachment(name=None,
+                            _data=unique_exact_match_para_2,
+                            _type=AttachmentType.String)
+    uem_para3_a = Attachment(name=None,
+                            _data=unique_exact_match_para_3,
+                            _type=AttachmentType.String)
+    uem_para4_a = Attachment(name=None,
+                            _data=unique_exact_match_para_4,
                             _type=AttachmentType.String)
 
+    feat_space_str = "{:0.3e}".format(ds.feature_space)
     target_matched_a = Attachment(name="Target Data Properties",
                                      _data=f"Feature space size (possible combinations): "
-                                           f"-Highlight-{f'{dataset.feature_space:,}'}-Highlight-<br>"
+                                           f"-Highlight-{feat_space_str}-Highlight-<br>"
                                            f"Number of unique records in Target Data: "
                                            f"-Highlight-{unique_target_records} "
                                            f"({perc_unique_target_records}%-Highlight-)",
                                      _type=AttachmentType.String)
     deid_matched_a = Attachment(name="Deidentified Data Properties",
                                      _data=f"Number of unique Target Data records exactly "
                                            f"matched in Deid. Data: "
                                            f"-Highlight-{t_rec_matched} "
                                            f"({perc_t_rec_matched}%)-Highlight-",
                                      _type=AttachmentType.String)
     r_ui_d.add(PrivacyScorePacket("Unique Exact Matches",
                               None,
-                              [uem_para_a,
+                              [uem_para1_a, uem_para2_a, uem_para3_a, uem_para4_a,
                                target_matched_a,
                                deid_matched_a]))
     rd.add('unique_exact_matches', {
         "records matched in target data": t_rec_matched,
         "percent records matched in target data": perc_t_rec_matched,
         "unique target records": unique_target_records,
         "percent unique target records": perc_unique_target_records,
```

### Comparing `sdnist-2.2.0/sdnist/report/score/utility/__init__.py` & `sdnist-2.3.0/sdnist/report/score/utility/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,20 +121,21 @@
 
     out_dir = Path(r_ui_d.output_directory, 'k_marginal_breakdown')
     if not out_dir.exists():
         os.mkdir(out_dir)
 
     up = UnivariatePlots(s, t,
                          ds, out_dir, ds.challenge, worst_univariates_to_display=3)
-    u_feature_data = up.save()
-    k_marg_break_rd[f'worst_{len(wpf)}_puma_univariate'] = up.report_data()
+    u_feature_data = up.save(level=3)
+    k_marg_break_rd[f'worst_{len(wpf)}_puma_univariate'] = up.report_data(level=3)
     k_marg_break_rd[f'worst_{len(wpf)}_puma_k_marginal_scores'] = \
         relative_path(save_data_frame(wsh,
                                       out_dir,
-                                      f'worst_{len(wpf)}_puma_k_marginal_scores'))
+                                      f'worst_{len(wpf)}_puma_k_marginal_scores'),
+                      level=2)
     u_as = []
     u_as.append(Attachment(name=None,
                            _data=f"h3Univariate Distribution of Worst "
                                  f"Performing Features in {len(wpf)} Worst Performing "
                                   + feature,
                            _type=AttachmentType.String))
     u_as.append(Attachment(name=None,
@@ -185,15 +186,15 @@
         u_as.append(a)
     corr_features = ds.config[strs.CORRELATION_FEATURES]
     corr_features = [f for f in ds.data_dict.keys() if f in corr_features]
     pcd = PearsonCorrelationDifference(t, s,
                                        corr_features)
     pcd.compute()
     pcp = PearsonCorrelationPlot(pcd.pp_corr_diff, out_dir)
-    pcp_saved_file_paths = pcp.save()
+    pcp_saved_file_paths = pcp.save(path_level=3)
     k_marg_break_rd['correlation_difference'] = {
         "pearson_correlation_difference": pcp.report_data
     }
 
     # rel_up_saved_file_paths = ["/".join(list(p.parts)[-3:])
     #                            for p in up_saved_file_paths]
     rel_pcp_saved_file_paths = ["/".join(list(p.parts)[-3:])
@@ -242,24 +243,25 @@
         # if remain_rows:
         #     rr_s = s.sample(n=remain_rows, replace=True)
         #     s = pd.concat([s, rr_s])
         return s
 
     # mapping of sub sample frac to k-marginal score of fraction
     ssample_score = dict()  # subsample scores dictionary
-    # find k-marginal of 10%, 20% ... 90% of sub-sample of target data
-    for i in range(1, 11):
+    # find k-marginal of 1%, 5%, 10%, 20% ... 90% of sub-sample of target data
+    sample_sizes = [1, 5] + [i*10 for i in range(1, 10)]
+    for i in sample_sizes:
         # using subsample of target data as synthetic data
-        s_sd = create_subsample(frac=i * 0.1)
+        s_sd = create_subsample(frac=i * 0.01)
         s_kmarg = k_marginal_cls(dataset.d_target_data,
                                  s_sd,
                                  group_features)
         s_kmarg.compute_score()
         s_score = int(s_kmarg.score)
-        ssample_score[i * 0.1] = s_score
+        ssample_score[i * 0.01] = s_score
 
     puma_scores = None
     if len(group_features):
         # subsample scores for each PUMA
         for i in range(5):
             s_sd = create_subsample(frac=4 * 0.1)
             s_kmarg = k_marginal_cls(dataset.d_target_data,
@@ -340,14 +342,15 @@
 
     sed_a = Attachment(name=None,
                        _data=sedf)
 
     # add k-marginal subsample and deidentified data scores to json report
     k_marg_synop_rd['subsample_error_comparison'] = \
         relative_path(save_data_frame(sedf_df, k_marg_synopsys_path, 'subsample_error_comparison'))
+    k_marg_synop_rd['sub_sampling_equivalent'] = int(min_frac * 100)
     k_marg_synop_rd['k_marginal_score'] = k_marginal_score
 
     report_data.add('k_marginal', {
         "k_marginal_synopsys": k_marg_synop_rd
     })
 
     # Create attachments for UI report
@@ -416,31 +419,28 @@
         ws_a = Attachment(name=None,
                           _data=worst_scores)
 
         # best score attachment
         bs_a = Attachment(name=f"{len(best_scores)} Best Performing " + '-'.join(group_features),
                           _data=best_scores)
 
-        report_data.add('k_marginal', {
-            "k_marginal_breakdown": k_marg_break_rd
-        })
-
+        report_data.add('worst_PUMA_breakdown', k_marg_break_rd)
         attachments.extend([as_para_a, as_a])
 
         metric_attachments = [k_marg_break_para_a, ws_para_a, ws_a]
 
         gp_a = grid_plot_attachment(group_features,
                                     group_scores,
                                     feature_values,
                                     ui_data.output_directory)
         if gp_a:
             metric_attachments.append(gp_a)
         metric_attachments.extend(worst_break_down)
 
-        kmarg_det_pkt = UtilityScorePacket('K-Marginal Score Breakdown',
+        kmarg_det_pkt = UtilityScorePacket('Worst Performing PUMAs Breakdown',
                                            None,
                                            metric_attachments)
 
     return kmarg_sum_pkt, kmarg_det_pkt
 
 
 def grid_plot_attachment(group_features: List[str],
@@ -605,18 +605,18 @@
     metric_name = s.NAME
 
     metric_score = int(s.score) if s.score > 100 else round(s.score, 3)
 
     p_dist_plot = PropensityDistribution(s.prob_dist, r_ui_d.output_directory)
     # pps = PropensityPairPlot(s.std_two_way_scores, rd.output_directory)
     #
-    prop_rep_data = {**s.report_data, **p_dist_plot.report_data}
-    rd.add('propensity mean square error', prop_rep_data)
 
     p_dist_paths = p_dist_plot.save()
+    prop_rep_data = {**s.report_data, **p_dist_plot.report_data}
+    rd.add('propensity mean square error', prop_rep_data)
     # pps_paths = pps.save('spmse',
     #                      'Two-Way Standardized Propensity Mean Square Error')
     rel_pd_path = ["/".join(list(p.parts)[-2:])
                     for p in p_dist_paths]
     # rel_pps_path = ["/".join(list(p.parts)[-2:])
     #                 for p in pps_paths]
```

### Comparing `sdnist-2.2.0/sdnist/report/score/utility/inconsistency.py` & `sdnist-2.3.0/sdnist/report/score/utility/inconsistency.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,14 +5,30 @@
 from sdnist.metrics.inconsistency import Inconsistencies
 from sdnist.report import Dataset
 from sdnist.report.report_data import \
     ReportData, ReportUIData, UtilityScorePacket, Attachment, AttachmentType
 
 from sdnist.utils import *
 
+ic_paragraphs = [
+    "In real world tabular data, it's common for record features to have "
+    "some deterministic, publicly known dependencies on each other: "
+    "knowing someone's AGEP= 3 necessarily tells you something about "
+    "their marital status, income and educational attainment. "
+    "Different deidentification methods may be better or worse at "
+    "automatically preserving these relationships. "
+    "When they fail (ex: producing toddlers with PhDs) we say "
+    "those records contain \"inconsistencies\". Our consistency "
+    "check metric below is not exhaustive, we don't catch everything "
+    "the way a production-grade system should, but this will give you "
+    "a sense of how consistency is preserved for age, work and household "
+    "features. Note that different deidentification approaches may do "
+    "better or worse with different types of inconsistencies."
+]
+
 
 class InconsistenciesReport:
     """
     Helper class for creating UI and json report data for the inconsistencies found
     in the deidentified data.
     """
 
@@ -38,14 +54,21 @@
         # initialize an instance of inconsistencies metric
         self.ic = Inconsistencies(self.s, o_path)
         self.ic.compute()  # compute inconsistencies in deidentified data
 
         # add inconsistencies stats and data to json report data
         self.rd.add('inconsistencies', self.ic.report_data)
 
+        # create report attachments
+        for p in ic_paragraphs:
+            para_a = Attachment(name=None,
+                                _data=p,
+                                _type=AttachmentType.String)
+            self.attachments.append(para_a)
+
         # --------- Add inconsistencies stats and dat to ui report data
         # UI attachment for summary of inconsistencies found in the deidentified data
         a_sum_h = Attachment(name='Summary',
                              _data={
                                  'table': self.ic.stats['summary'],
                                  'size': 60
                              },
```

### Comparing `sdnist-2.2.0/sdnist/report/score/utility/linear_regression.py` & `sdnist-2.3.0/sdnist/report/score/utility/linear_regression.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.2.0/sdnist/report/score/utility/pca.py` & `sdnist-2.3.0/sdnist/report/score/utility/pca.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,18 @@
            "<a href='https://en.wikipedia.org/wiki/Principal_component_analysis'>" \
            "Principle Component Analysis</a> " \
            "to find a way of representing the target data in a lower dimensional " \
            "space (in 5 dimensions rather than the full 22 " \
            "dimensions of the original feature space). Descriptions " \
            "of these new five dimensions (components) are " \
            "given in the components table; the components will change " \
-           "depending on which target data set you’re using. " \
+           "depending on which target data set you're using. " \
            "Five dimensions are better than 22, but we actually want to " \
            "get down to two dimensions so we can plot the data " \
-           "on simple (x,y) axes– the plots below show the data " \
+           "on simple (x,y) axes the plots below show the data " \
            "across each possible pair combination of our five components. " \
            "You can compare how the shapes change between the target data " \
            "and the deidentified data, and consider what that might mean in light " \
            "of the component definitions. This is a relatively new visualization " \
            "metric that was introduced by the " \
            "<a href='https://pages.nist.gov/HLG-MOS_Synthetic_Data_Test_Drive/submissions.html#ipums_international'>" \
            "IPUMS International team</a> " \
@@ -36,15 +36,15 @@
              "taken from the target data (listed in the table). Effectively, " \
              "we're looking at the data from the exact same angles in " \
              "both sets of plots so we can easily compare the target " \
              "data and the deidentified data with respect to those angles."
 
 pca_highlight_para = "The queries below explore the PCA metric results in more detail " \
                      "by zooming in on a single component-pair panel and highlighting " \
-                     "all individuals that satisfy a given constraint (such as MSP = “N”, " \
+                     "all individuals that satisfy a given constraint (such as MSP='N', " \
                      "individuals who are unmarried because they are children). " \
                      "If the deidentified data preserves the structure and feature " \
                      "correlations of the target data, the highlighted areas should have " \
                      "similar shape. "
 class PCAReport:
     def __init__(self,
                  dataset: Dataset,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sdnist-2.2.0/sdnist/report/server.py` & `sdnist-2.3.0/sdnist/report/server.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.2.0/sdnist/schema.py` & `sdnist-2.3.0/sdnist/schema.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.2.0/sdnist/strs.py` & `sdnist-2.3.0/sdnist/strs.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.2.0/sdnist/utils.py` & `sdnist-2.3.0/sdnist/utils.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.2.0/sdnist/visualizer_resources/report2.jinja2` & `sdnist-2.3.0/sdnist/visualizer_resources/report2.jinja2`

 * *Files identical despite different names*

### Comparing `sdnist-2.2.0/sdnist.egg-info/PKG-INFO` & `sdnist-2.3.0/sdnist.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,328 +1,306 @@
 Metadata-Version: 2.1
 Name: sdnist
-Version: 2.2.0
+Version: 2.3.0
 Summary: SDNist: Deidentified Data Report Generator
 Home-page: https://github.com/usnistgov/SDNist
 Author: National Institute of Standards and Technology
 Author-email: gary.howarth@nist.gov
-License: UNKNOWN
-Description: # SDNist v2.2: Deidentified Data Report Tool
-        
-        ## [SDNist is the offical software package for engaging in the NIST Collaborative Research Cycle](https://pages.nist.gov/privacy_collaborative_research_cycle)
-        
-        Welcome! SDNist is a python package that provides benchmark data and evaluation metrics for deidentified data generators. This version of SDNist supports using the [NIST Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/tree/main/nist%20diverse%20communities%20data%20excerpts), a geographically partioned, limited feature data set.
-        
-        The deidentified data report evaluates utility and privacy of a given deidentified dataset and generates a summary quality report with performance of a deidentified dataset enumerated and illustrated for each utility and privacy metric.
-        
-        [Preview sample reports produced by the tool here.](https://github.com/usnistgov/SDNist/tree/main/sdnist/report/sample-reports)
-        
-        This tool is being actively developed. Please (raise an Issue)[https://github.com/usnistgov/SDNist/issues]  if you catch a bug or would like have feature suggestions. 
-        
-        
-        ### Project Team  
-        **Karan Bhagat**, *Knexus Research* - Developer *sdnist.report* package  
-        
-        **Christine Task**, *Knexus Research* - Project technical lead
-        
-        **Gary Howarth**, *NIST* - Project PI [gary.howarth@nist.gov](mailto:gary.howarth@nist.gov)
-        
-        ### Reporting Issues
-        Help us improve the package and this guide by reporting issues [here](https://github.com/usnistgov/SDNist/issues).
-        
-        ### Temporal Map Challenge Environment
-        
-        SDNist v2.0 and above does not support the Temporal Map Challenge environment.
-        
-        To run the testing environment from the [*NIST PSCR Differential Privacy Temporal Map Challenge*](https://www.nist.gov/ctl/pscr/open-innovation-prize-challenges/past-prize-challenges/2020-differential-privacy-temporal) for the Chicago Taxi data sprint or the American Community Survey sprint, please go to the the [Temporal Map Challenge assets repository](https://github.com/usnistgov/Differential-Privacy-Temporal-Map-Challenge-assets).
-        
-        
-        Setting Up the SDNIST Report Tool
-        ------------------------
-        
-        ### Brief Setup Instructions
-        
-        SDNist requires Python version 3.7 or greater. If you have installed a previous version of the SDNist library, we recommend uninstalling or installing v2.2 in a virtual environment. v2.2 can be installed via [Release 2.2](https://github.com/usnistgov/SDNist/releases/tag/v2.2.0). The NIST Diverse Community Exceprt data will download on the fly.
-        ```
-        pip install sdnist
-        ```
-        
-        ### Detailed Setup Instructions
-        
-        1. The SDNist Report Tool is a part of the sdnist Python library that can be installed on a user’s MAC OS, Windows, or Linux machine.
-        
-        
-        2. The sdnist library requires Python version 3.7 or greater to be installed on the user's machine. Check whether an installation exists on the machine by executing the following command in your terminal on Mac/Linux or powershell on Windows:
-           ```
-            c:\\> python -V
-           ```
-            If Python is already installed, the above command should return the currently installed version. If Python is not found or the version is below 3.7, then you can download Python from the [Python website](https://www.python.org/downloads/).
-        
-        
-        3.  Create a local directory/folder on the machine to set up the SDNist library. This guide assumes the local directory to be sdnist-project; an example of a complete file path is c:\\sdnist-project:
-            ```
-            c:\\sdnist-project>     
-            ```
-        
-        4.  Download the sdnist installable wheel (sdnist-2.2.0-py3-none-any.whl) from the Github: [Release 2.2](https://github.com/usnistgov/SDNist/releases/download/v2.2.0/sdnist-2.2.0-py3-none-any.whl).
-        
-        
-        5.  Move the downloaded sdnist-2.2.0-py3-none-any.whl file to the sdnist-project directory.
-        
-        
-        6.  Using the terminal on Mac/Linux or powershell on Windows, navigate to the sdnist-project directory.
-        
-        
-        7.  In the already-opened terminal or powershell window, execute the following command to create a new Python environment. The sdnist library will be installed in this newly created Python environment:
-        
-            ```
-            c:\\sdnist-project> python -m venv venv
-            ```
-        
-        8. The new Python environment will be created in the sdnist-project directory, and the files of the environment should be in the venv directory. To check whether a new Python environment was created successfully, use the following command to list all directories in the sdnist-project directory, and make sure the venv directory exists.
-        
-            **MAC OS/Linux:**
-            ```
-            sdnist-project> ls
-            ```
-            **Windows:**
-            ```
-            c:\\sdnist-project> dir
-            ```
-        
-        9. Now activate the Python environment and install the sdnist library into it.
-        
-            **MAC OS/Linux:**
-            ```
-            sdnist-project> . venv/bin/activate
-            ```
-            The python virtual environment should now be activated. You should see environment name (**venv** in this case) appended to the terminal prompt as below:  
-            ```
-            (venv) sdnist-project>
-            ```
-        
-            **Windows:**
-            ```
-            c:\\sdnist-project> . venv/Scripts/activate
-            ```
-            The python virtual environment should now be activated. You should see environment name (**venv** in this case) appended to the command/powershell prompt as below:  
-            ```
-            (venv) c:\\sdnist-project>
-            ```
-        
-            On Windows, a few users may encounter the following error if their machines are new (executing scripts is disabled by default on some Windows machines):
-            ```
-            C:\\sdnist-project\\venv\\Scripts\\Activate.ps1 cannot be loaded because running scripts is disabled on this system.
-            ```
-            Run the following command to let Windows execute scripts:
-            ```
-            Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope LocalMachine
-            ```
-        
-        
-        10. Per step 5 above, the sdnist-2.2.0-py3-none-any.whl file should already be present in the sdnist-project directory. Check whether that is true by listing the files in the sdnist-project directory.
-        
-              **MAC OS/Linux:**
-               ```
-               (venv) sdnist-project> ls
-               ```
-              **Windows:**
-               ```
-               (venv) c:\\sdnist-project> dir
-               ```
-               The sdnist-2.2.0-py3-none-any.whl file should be in the list printed by the above command; otherwise, follow steps 4 and 5 again to download the .whl file.
-        
-        
-        11. Install sdnist Python library:
-               ```
-               (venv) c:\\sdnist-project> pip install sdnist-2.2.0-py3-none-any.whl
-               ```
-        
-        
-        12. Installation is successful if executing the following command outputs a help menu for the sdnist.report package:
-               ```
-               (venv) c:\\sdnist-project> python -m sdnist.report -h
-               ```
-               Output:
-               ```
-                usage: __main__.py [-h] [--labels LABELS] [--data-root DATA_ROOT]
-                                   PATH_DEIDENTIFIED_DATASET TARGET_DATASET_NAME
-                
-                positional arguments:
-                  PATH_DEIDENTIFIED_DATASET
-                                        Location of deidentified dataset (csv or parquet
-                                        file).
-                  TARGET_DATASET_NAME   Select name of the target dataset that was used to
-                                        generated given deidentified dataset.
-                
-                options:
-                  -h, --help            show this help message and exit
-                  --labels LABELS       This argument is used to add meta-data to help
-                                        identify which deidentified data was was evaluated in
-                                        the report. The argument can be a string that is a
-                                        plain text label for the file, or it can be a file
-                                        path to a json file containing [label, value] pairs.
-                                        This labels will be included in the printed report.
-                  --data-root DATA_ROOT
-                                        Path of the directory to be used as the root for the
-                                        target datasets.
-                
-                Choices for Target Dataset Name:
-                  [DATASET NAME]        [FILENAME]
-                  MA                    ma2019
-                  TX                    tx2019
-                  NATIONAL              national2019
-               ```
-        
-        
-        13. These instructions install sdnist into a virtual environment. The virtual environment must be activated (step 9) each time a new terminal window is used with sdnist.
-        
-        
-        Generate Data Quality Report
-        ---------------------------
-        
-        1.  The sdnist.report package requires a path to the deidentified dataset file and the name of the target dataset from which the deidentified dataset file will be created. Following is the command line usage of the sdnist.report package:
-              ```
-              python -m sdnist.report PATH_DEINDETIFIED_DATASET TARGET_DATSET_NAME
-              ```
-        
-              The above command is just an example usage signature of the package. Steps 3 through 5 show the actual commands to run the tool, where the parameter PATH_DEIDENTIFIED_DATASET is replaced with the path of the deidentified dataset file on the your machine, and the parameter TARGET_DATASET_NAME is replaced with one of the bundled dataset names (MA, TX, or NATIONAL).
-        
-              A deidentified dataset file can be anywhere on your machine. You only need the path of the file to pass it as an argument to the sdnist.report package. For illustration purposes, this guide assumes an example deidentified dataset file named syn_tx.csv is generated from the bundled dataset file named TX that is present in the sdnist-project directory. You can also use the bundled toy deidentified datasets for generating some toy evaluation reports using the sdnist.report package by following steps 5 and 6 in the next section, Setup Data for SDNIST Report Tool.
-        
-             The sdnist.report packages come bundled with three target datasets: MA, TX, and NATIONAL. If these datasets are not available locally, the package will download them automatically when you run any one of the commands in steps 3 through 5 for the first time. In case of any trouble while downloading the datasets, please refer to the next section, Setup Data for SDNIST Report Tool.
-        
-        
-        2.  If you have closed the terminal or the powershell window that was used for the tool setup, open a new one, and after navigating the to sdnist-project directory, run the activate script as explained in step 9 of the Setup SDNIST Report Tool section.
-        
-        
-        3.  Use the following command to generate a data quality report for the example deidentified dataset (syn_tx.csv) that is generated using the bundled dataset TX:
-              ```
-              (venv) c:\\sdnist-project> python -m sdnist.report syn_tx.csv TX
-              ```
-              At the completion of the process initiated by the above command, an .html report will open in the default web browser on your machine. Likewise, .html report files will be available in the reports directory created automatically in the sdnist-project directory.
-        
-        
-        4.  Use the following command to generate a data quality report for the example deidentified dataset (syn_ma.csv) that is generated using the bundled dataset MA:
-              ```
-              (venv) c:\\sdnist-project> python -m sdnist.report syn_ma.csv MA
-              ```
-        
-        
-        5.  Use the following command to generate a data quality report for the example deidentified dataset (syn_national.csv) that is generated using the bundled dataset NATIONAL:
-              ```
-              (venv) c:\\sdnist-project> python -m sdnist.report syn_national.csv NATIONAL
-              ```
-        6.  Starting from version 2.1, SDNist allow users to add labels for the deidentified dataset used to generate report:
-            * To add single string label to the report, use command line option **--labels** followed by a string as given in the following example command:
-              ```
-              (venv) c:\\sdnist-project> python -m sdnist.report syn_national.csv NATIONAL --labels used_epsilon_1
-              ```
-              This is how the string label *used_epsilon_1* will appear in the report:
-              ![string label in report](readme_resource/string_label.png)
-            * To add multiple string labels to the report, use command line option **--labels** followed by a path to the json file containing labels:
-              ```
-              (venv) c:\\sdnist-project> python -m sdnist.report syn_national.csv NATIONAL --labels example_labels.json
-              ```
-              Where example_labels.json can be:
-              ```
-                {
-                  "epsilon": "1",
-                  "delta": "10^-5",
-                  "created on": "March 3, 2023",
-                  "deidentification method": "example_method"
-                }
-              ```
-              This is how the *example_labels.json* will appear in the report:
-             ![multiple labels in report](readme_resource/multiple_labels.png)
-        7.  The following are all the parameters offered by the sdnist.report package:
-        
-             - **PATH_DEIDENTIFIED_DATASET**: The absolute or relative path to the deidentified dataset .csv or parquet file. If the provided path is relative, it should be relative to the current working directory. This guide assumes the current working directory is sdnist-project.
-             - **TARGET_DATASET_NAME**: This should be the name of one of the datasets bundled with the sdnist.report package. It is the name of the dataset from which the input deidentified dataset is generated, and it can be one of the following:
-               - MA
-               - TX
-               - NATIONAL
-        
-             - **--data-root**: The absolute or relative path to the directory containing the bundled dataset, or the directory where the bundled dataset should be downloaded to if it is not available locally. The default directory is set to **diverse_community_excerpts_data**.
-             - **--labels**: This argument is used to add meta-data to help identify which deidentified data was was evaluated in the report.  The argument can be a string that is a plain text label for the file, or it can be a file path to a json file containing label, value pairs. 
-        
-        Setup Data for SDNIST Report Tool
-        ---------------------------------
-        
-        1.  The sdnist.report package comes with built-in datasets. The package will automatically download the datasets from Github if they are not already available locally on your machine. You should see following message on your terminal or powershell window when the datasets are downloaded by the sdnist.report package:
-              ```
-              (venv) c:\\sdnist-project> python -m sdnist.report syn_tx.csv TX
-        
-              Downloading all SDNist datasets from:  
-              https://github.com/usnistgov/SDNist/releases/download/v2.2.0/diverse_communities_data_excerpts.zip ...  
-              ...5%, 47352 KB, 8265 KB/s, 5 seconds elapsed
-              ```
-        
-              Follow the next subsection, Download Data Manually, if the sdnist.report package is unable to download the datasets.
-        
-        
-        2. All the datasets required by the sdnist.report package are installed into the sdnist _toy _data directory, which should be now present inside the sdnist-project directory. sdnist _toy _data is also a data root directory. You can use some other directory as a data root by providing the –data-root argument to the sdnist.report package. If you provide a –data-root argument with a path, the sdnist.report package will look for datasets in the data root directory you have specified, and the package will download it if it is not present in the data root.
-        
-        
-        3. The sdnist.report package also needs a deidentified dataset that it can evaluate against its original counterpart. Since the sdnist.report package comes bundled with the datasets, the deidentified dataset should be generated using the bundled datasets.
-        
-           You can download a copy of the datasets from Github [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/tree/main/nist%20diverse%20communities%20data%20excerpts). This copy is similar to the one bundled with the sdnist.report package, but it contains more documentation and a description of the datasets.
-        
-        
-        4. You can download the toy deidentified datasets from Github [Sdnist Toy Deidentified Dataset](https://github.com/usnistgov/SDNist/releases/download/v2.1.1/toy_deidentified_data.zip). Unzip the downloaded file, and move the unzipped toy_deidentified_dataset directory to the sdnist-project directory.
-        
-        
-        5. Each toy deidentified dataset file is generated using the [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.2.0/diverse_communities_excerpts_data.zip). The syn_ma.csv, syn_tx.csv, and syn_national.csv deidentified dataset files are created from target datasets MA (ma2019.csv), TX (tx2019.csv), and NATIONAL(national2019.csv), respectively. You can use one of the toy deidentified dataset files for testing whether the sdnist.report package is installed correctly on your system.
-        
-        
-        6. Use the following commands for generating reports if you are using a toy deidentified dataset file:
-        
-           For evaluating the Massachusetts dataset:
-           ```
-           (venv) c:\\sdnist-project> python -m sdnist.report toy_deidentified_data/syn_ma.csv MA
-           ```
-        
-           For evaluating the Texas dataset:
-           ```
-           (venv) c:\\sdnist-project> python -m sdnist.report toy_deidentified_data/syn_tx.csv TX
-           ```
-        
-           For evaluating the national dataset:
-           ```
-           (venv) c:\\sdnist-project> python -m sdnist.report toy_deidentified_data/syn_national.csv NATIONAL
-           ```
-        
-        7.  A deidentified dataset can be a .csv or a parquet file, and the path of this file is required
-        by the sdnist.report package to generate a data quality report.
-        
-        
-        Download Data Manually
-        ----------------------
-        
-        1.  If the sdnist.report package is not able to download the datasets, you can download them from Github [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.2.0/diverse_communities_data_excerpts.zip).
-        3.  Unzip the **diverse_community_excerpts_data.zip** file and move the unzipped **diverse_community_excerpts_data** directory to the **sdnist-project** directory.
-        4.  Delete the **diverse_community_excerpts_data.zip** file once the data is successfully extracted from the zip.
-        
-        Citing SDNist Deidentified Data Report Tool
-        -------------------------------------------
-        
-        If you publish work that utilizes the SDNist Deidentified Data Tool, please cite the software. Citation recommendation:  
-        > Task C., Bhagat K., and Howarth G.S. (2023), SDNist v2: Deidentified Data Report Tool, 
-        > National Institute of Standards and Technology, 
-        > https://doi.org/10.18434/mds2-2943    
-        (NOTE: DOI is not yet active, but should be by 1 APR 2023).
-        
-        Credits 
-        ----------
-        
-        - [Christine Task](mailto:christine.task@knexusresearch.com) - Project technical lead - christine.task@knexusresearch.com
-        - [Karan Bhagat](https://github.com/kbtriangulum) - Contributor
-        - [David Lee](https://www.linkedin.com/in/david-lee-13872922/) - Documentation
-        - [Gary Howarth](https://www.nist.gov/people/gary-howarth) - Project PI - gary.howarth@nist.gov
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: Public Domain
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# SDNist v2.3: Deidentified Data Report Tool
+
+## [SDNist is the offical software package for engaging in the NIST Collaborative Research Cycle](https://pages.nist.gov/privacy_collaborative_research_cycle)
+
+Welcome! SDNist is a python package that provides benchmark data and evaluation metrics for deidentified data generators. This version of SDNist supports using the [NIST Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/tree/main/nist%20diverse%20communities%20data%20excerpts), a geographically partioned, limited feature data set.
+
+The deidentified data report evaluates utility and privacy of a given deidentified dataset and generates a summary quality report with performance of a deidentified dataset enumerated and illustrated for each utility and privacy metric.
+
+[Preview sample reports produced by the tool here.](https://github.com/usnistgov/SDNist/tree/main/sdnist/report/sample-reports)
+
+This tool is being actively developed. Please (raise an Issue)[https://github.com/usnistgov/SDNist/issues]  if you catch a bug or would like have feature suggestions. 
+
+
+### Project Team  
+**Karan Bhagat**, *Knexus Research* - Developer *sdnist.report* package  
+
+**Christine Task**, *Knexus Research* - Project technical lead
+
+**Gary Howarth**, *NIST* - Project PI [gary.howarth@nist.gov](mailto:gary.howarth@nist.gov)
+
+### Acknowledgements
+
+SDNist v2 grew from [SDNist v1](https://github.com/usnistgov/Differential-Privacy-Temporal-Map-Challenge-assets), developed in partnership with Saurus Technologies under CRADA CN-21-0143.
+
+### Reporting Issues
+Help us improve the package and this guide by reporting issues [here](https://github.com/usnistgov/SDNist/issues).
+
+### Temporal Map Challenge Environment
+
+SDNist v2.0 and above does not support the Temporal Map Challenge environment.
+
+To run the testing environment from the [*NIST PSCR Differential Privacy Temporal Map Challenge*](https://www.nist.gov/ctl/pscr/open-innovation-prize-challenges/past-prize-challenges/2020-differential-privacy-temporal) for the Chicago Taxi data sprint or the American Community Survey sprint, please go to the the [Temporal Map Challenge assets repository](https://github.com/usnistgov/Differential-Privacy-Temporal-Map-Challenge-assets).
+
+
+Setting Up the SDNIST Report Tool
+------------------------
+
+### Brief Setup Instructions
+
+SDNist requires Python version 3.7 or greater. If you have installed a previous version of the SDNist library, we recommend installing v2.3 in a virtual environment. v2.3 can be installed via [Release 2.3](https://github.com/usnistgov/SDNist/releases/tag/v2.3.0) or via the Pypi server: `pip install sdnist` or, if you already have a version installed, `pip install --upgrade sdnist`.
+
+The NIST Diverse Community Exceprt data will download on the fly.
+
+
+
+### Detailed Setup Instructions Using Pypi
+
+1. The SDNist Report Tool is a part of the sdnist Python library that can be installed on a user’s MAC OS, Windows, or Linux machine.
+
+
+2. The sdnist library requires Python version 3.7 or greater to be installed on the user's machine. Check whether an installation exists on the machine by executing the following command in your terminal on Mac/Linux or powershell on Windows:
+   ```
+    c:\\> python -V
+   ```
+    If Python is already installed, the above command should return the currently installed version. If Python is not found or the version is below 3.7, then you can download Python from the [Python website](https://www.python.org/downloads/).
+
+
+3.  Create a local directory/folder on the machine to set up the SDNist library. This guide assumes the local directory to be sdnist-project; an example of a complete file path is c:\\sdnist-project:
+    ```
+    c:\\sdnist-project>     
+    ```
+
+
+4. In the already-opened terminal or powershell window, execute the following command to create a new Python environment. The sdnist library will be installed in this newly created Python environment:
+
+    ```
+    c:\\sdnist-project> python -m venv venv
+    ```
+
+5. The new Python environment will be created in the sdnist-project directory, and the files of the environment should be in the venv directory. To check whether a new Python environment was created successfully, use the following command to list all directories in the sdnist-project directory, and make sure the venv directory exists.
+
+    **MAC OS/Linux:**
+    ```
+    sdnist-project> ls
+    ```
+    **Windows:**
+    ```
+    c:\\sdnist-project> dir
+    ```
+
+6. Now activate the Python environment and install the sdnist library into it.
+
+    **MAC OS/Linux:**
+    ```
+    sdnist-project> . venv/bin/activate
+    ```
+    The python virtual environment should now be activated. You should see environment name (**venv** in this case) appended to the terminal prompt as below:  
+    ```
+    (venv) sdnist-project>
+    ```
+
+    **Windows:**
+    ```
+    c:\\sdnist-project> . venv/Scripts/activate
+    ```
+    The python virtual environment should now be activated. You should see environment name (**venv** in this case) appended to the command/powershell prompt as below:  
+    ```
+    (venv) c:\\sdnist-project>
+    ```
+
+    On Windows, a few users may encounter the following error if their machines are new (executing scripts is disabled by default on some Windows machines):
+    ```
+    C:\\sdnist-project\\venv\\Scripts\\Activate.ps1 cannot be loaded because running scripts is disabled on this system.
+    ```
+    Run the following command to let Windows execute scripts:
+    ```
+    Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope LocalMachine
+    ```
+
+7. Install sdnist Python library:
+       ```
+       (venv) c:\\sdnist-project> pip install sdnist
+       ```
+
+8. Installation is successful if executing the following command outputs a help menu for the sdnist.report package:
+       ```
+       (venv) c:\\sdnist-project> python -m sdnist.report -h
+       ```
+       Output:
+       ```
+        usage: __main__.py [-h] [--labels LABELS] [--data-root DATA_ROOT]
+                           PATH_DEIDENTIFIED_DATASET TARGET_DATASET_NAME
+        
+        positional arguments:
+          PATH_DEIDENTIFIED_DATASET
+                                Location of deidentified dataset (csv or parquet
+                                file).
+          TARGET_DATASET_NAME   Select name of the target dataset that was used to
+                                generated given deidentified dataset.
+        
+        options:
+          -h, --help            show this help message and exit
+          --labels LABELS       This argument is used to add meta-data to help
+                                identify which deidentified data was was evaluated in
+                                the report. The argument can be a string that is a
+                                plain text label for the file, or it can be a file
+                                path to a json file containing [label, value] pairs.
+                                This labels will be included in the printed report.
+          --data-root DATA_ROOT
+                                Path of the directory to be used as the root for the
+                                target datasets.
+        
+        Choices for Target Dataset Name:
+          [DATASET NAME]        [FILENAME]
+          MA                    ma2019
+          TX                    tx2019
+          NATIONAL              national2019
+       ```
+
+9. These instructions install sdnist into a virtual environment. The virtual environment must be activated (step 9) each time a new terminal window is used with sdnist.
+
+
+Generate Data Quality Report
+---------------------------
+
+1.  The sdnist.report package requires a path to the deidentified dataset file and the name of the target dataset from which the deidentified dataset file will be created. Following is the command line usage of the sdnist.report package:
+      ```
+      python -m sdnist.report PATH_DEINDETIFIED_DATASET TARGET_DATSET_NAME
+      ```
+
+      The above command is just an example usage signature of the package. Steps 3 through 5 show the actual commands to run the tool, where the parameter PATH_DEIDENTIFIED_DATASET is replaced with the path of the deidentified dataset file on the your machine, and the parameter TARGET_DATASET_NAME is replaced with one of the bundled dataset names (MA, TX, or NATIONAL).
+
+      A deidentified dataset file can be anywhere on your machine. You only need the path of the file to pass it as an argument to the sdnist.report package. For illustration purposes, this guide assumes an example deidentified dataset file named syn_tx.csv is generated from the bundled dataset file named TX that is present in the sdnist-project directory. You can also use the bundled toy deidentified datasets for generating some toy evaluation reports using the sdnist.report package by following steps 5 and 6 in the next section, Setup Data for SDNIST Report Tool.
+
+     The sdnist.report packages come bundled with three target datasets: MA, TX, and NATIONAL. If these datasets are not available locally, the package will download them automatically when you run any one of the commands in steps 3 through 5 for the first time. In case of any trouble while downloading the datasets, please refer to the next section, Setup Data for SDNIST Report Tool.
+
+
+2.  If you have closed the terminal or the powershell window that was used for the tool setup, open a new one, and after navigating the to sdnist-project directory, run the activate script as explained in step 9 of the Setup SDNIST Report Tool section.
+
+
+3.  Use the following command to generate a data quality report for the example deidentified dataset (syn_tx.csv) that is generated using the bundled dataset TX:
+      ```
+      (venv) c:\\sdnist-project> python -m sdnist.report syn_tx.csv TX
+      ```
+      At the completion of the process initiated by the above command, an .html report will open in the default web browser on your machine. Likewise, .html report files will be available in the reports directory created automatically in the sdnist-project directory.
+
+
+4.  Use the following command to generate a data quality report for the example deidentified dataset (syn_ma.csv) that is generated using the bundled dataset MA:
+      ```
+      (venv) c:\\sdnist-project> python -m sdnist.report syn_ma.csv MA
+      ```
+
+
+5.  Use the following command to generate a data quality report for the example deidentified dataset (syn_national.csv) that is generated using the bundled dataset NATIONAL:
+      ```
+      (venv) c:\\sdnist-project> python -m sdnist.report syn_national.csv NATIONAL
+      ```
+6.  Starting from version 2.1, SDNist allow users to add labels for the deidentified dataset used to generate report:
+    * To add single string label to the report, use command line option **--labels** followed by a string as given in the following example command:
+      ```
+      (venv) c:\\sdnist-project> python -m sdnist.report syn_national.csv NATIONAL --labels used_epsilon_1
+      ```
+      This is how the string label *used_epsilon_1* will appear in the report:
+      ![string label in report](readme_resource/string_label.png)
+    * To add multiple string labels to the report, use command line option **--labels** followed by a path to the json file containing labels:
+      ```
+      (venv) c:\\sdnist-project> python -m sdnist.report syn_national.csv NATIONAL --labels example_labels.json
+      ```
+      Where example_labels.json can be:
+      ```
+        {
+          "epsilon": "1",
+          "delta": "10^-5",
+          "created on": "March 3, 2023",
+          "deidentification method": "example_method"
+        }
+      ```
+      This is how the *example_labels.json* will appear in the report:
+     ![multiple labels in report](readme_resource/multiple_labels.png)
+7.  The following are all the parameters offered by the sdnist.report package:
+
+     - **PATH_DEIDENTIFIED_DATASET**: The absolute or relative path to the deidentified dataset .csv or parquet file. If the provided path is relative, it should be relative to the current working directory. This guide assumes the current working directory is sdnist-project.
+     - **TARGET_DATASET_NAME**: This should be the name of one of the datasets bundled with the sdnist.report package. It is the name of the dataset from which the input deidentified dataset is generated, and it can be one of the following:
+       - MA
+       - TX
+       - NATIONAL
+
+     - **--data-root**: The absolute or relative path to the directory containing the bundled dataset, or the directory where the bundled dataset should be downloaded to if it is not available locally. The default directory is set to **diverse_community_excerpts_data**.
+     - **--labels**: This argument is used to add meta-data to help identify which deidentified data was was evaluated in the report.  The argument can be a string that is a plain text label for the file, or it can be a file path to a json file containing label, value pairs. 
+
+Setup Data for SDNIST Report Tool
+---------------------------------
+
+1.  The sdnist.report package comes with built-in datasets. The package will automatically download the datasets from Github if they are not already available locally on your machine. You should see following message on your terminal or powershell window when the datasets are downloaded by the sdnist.report package:
+      ```
+      (venv) c:\\sdnist-project> python -m sdnist.report syn_tx.csv TX
+
+      Downloading all SDNist datasets from:  
+      https://github.com/usnistgov/SDNist/releases/download/v2.2.0/diverse_communities_data_excerpts.zip ...  
+      ...5%, 47352 KB, 8265 KB/s, 5 seconds elapsed
+      ```
+
+      Follow the next subsection, Download Data Manually, if the sdnist.report package is unable to download the datasets.
+
+
+2. All the datasets required by the sdnist.report package are installed into the sdnist \_toy \_data directory, which should be now present inside the sdnist-project directory. sdnist \_toy \_data is also a data root directory. You can use some other directory as a data root by providing the –data-root argument to the sdnist.report package. If you provide a –data-root argument with a path, the sdnist.report package will look for datasets in the data root directory you have specified, and the package will download it if it is not present in the data root.
+
+
+3. The sdnist.report package also needs a deidentified dataset that it can evaluate against its original counterpart. Since the sdnist.report package comes bundled with the datasets, the deidentified dataset should be generated using the bundled datasets.
+
+   You can download a copy of the datasets from Github [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/tree/main/nist%20diverse%20communities%20data%20excerpts). This copy is similar to the one bundled with the sdnist.report package, but it contains more documentation and a description of the datasets.
+
+
+4. You can download the toy deidentified datasets from Github [Sdnist Toy Deidentified Dataset](https://github.com/usnistgov/SDNist/releases/download/v2.1.1/toy_deidentified_data.zip). Unzip the downloaded file, and move the unzipped toy_deidentified_dataset directory to the sdnist-project directory.
+
+
+5. Each toy deidentified dataset file is generated using the [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.3.0/diverse_communities_data_excerpts.zip). The syn_ma.csv, syn_tx.csv, and syn_national.csv deidentified dataset files are created from target datasets MA (ma2019.csv), TX (tx2019.csv), and NATIONAL(national2019.csv), respectively. You can use one of the toy deidentified dataset files for testing whether the sdnist.report package is installed correctly on your system.
+
+
+6. Use the following commands for generating reports if you are using a toy deidentified dataset file:
+
+   For evaluating the Massachusetts dataset:
+   ```
+   (venv) c:\\sdnist-project> python -m sdnist.report toy_deidentified_data/syn_ma.csv MA
+   ```
+
+   For evaluating the Texas dataset:
+   ```
+   (venv) c:\\sdnist-project> python -m sdnist.report toy_deidentified_data/syn_tx.csv TX
+   ```
+
+   For evaluating the national dataset:
+   ```
+   (venv) c:\\sdnist-project> python -m sdnist.report toy_deidentified_data/syn_national.csv NATIONAL
+   ```
+
+7.  A deidentified dataset can be a .csv or a parquet file, and the path of this file is required
+by the sdnist.report package to generate a data quality report.
+
+
+Download Data Manually
+----------------------
+
+1.  If the sdnist.report package is not able to download the datasets, you can download them from Github [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.3.0/diverse_communities_data_excerpts.zip).
+3.  Unzip the **diverse_community_excerpts_data.zip** file and move the unzipped **diverse_community_excerpts_data** directory to the **sdnist-project** directory.
+4.  Delete the **diverse_community_excerpts_data.zip** file once the data is successfully extracted from the zip.
+
+Citing SDNist Deidentified Data Report Tool
+-------------------------------------------
+
+If you publish work that utilizes the SDNist Deidentified Data Tool, please cite the software. Citation recommendation:  
+> Task C., Bhagat K., and Howarth G.S. (2023), SDNist v2: Deidentified Data Report Tool, 
+> National Institute of Standards and Technology, 
+> https://doi.org/10.18434/mds2-2943.
+
+Credits 
+----------
+
+- [Christine Task](mailto:christine.task@knexusresearch.com) - Project technical lead - christine.task@knexusresearch.com
+- [Karan Bhagat](https://github.com/kbtriangulum) - Contributor
+- [David Lee](https://www.linkedin.com/in/david-lee-13872922/) - Documentation
+- [Gary Howarth](https://www.nist.gov/people/gary-howarth) - Project PI - gary.howarth@nist.gov
```

### Comparing `sdnist-2.2.0/sdnist.egg-info/SOURCES.txt` & `sdnist-2.3.0/sdnist.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 sdnist/__init__.py
 sdnist/__main__.py
 sdnist/load.py
 sdnist/schema.py
```

### Comparing `sdnist-2.2.0/setup.py` & `sdnist-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     install_requires=[
         "jinja2==3.1.2",
         "loguru==0.7.0",
         "matplotlib==3.7.1",
         "numpy==1.24.2",
         "pandas==2.0.0",
         "pyarrow==11.0.0",
-        "requests==2.28.2",
+        "requests==2.31.0",
         "scikit-learn==1.2.2",
         "scipy==1.10.1",
         "tqdm==4.65.0",
         "colorama==0.4.6"
     ],
     classifiers=['Development Status :: 5 - Production/Stable',
                  'Programming Language :: Python :: 3.8',
```

