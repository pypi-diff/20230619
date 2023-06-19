# Comparing `tmp/cca_zoo-2.0.2.tar.gz` & `tmp/cca_zoo-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cca_zoo-2.0.2.tar", last modified: Thu Jun 15 16:21:36 2023, max compression
+gzip compressed data, was "dist/cca_zoo-2.0.3.tar", last modified: Mon Jun 19 12:41:14 2023, max compression
```

## Comparing `cca_zoo-2.0.2.tar` & `cca_zoo-2.0.3.tar`

### file list

```diff
@@ -1,112 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/classical/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_gcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_grcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_altmaxvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_elasticnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_ey.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_gradkcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_incrementalpls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_pls_als.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_pmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_scca_admm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_scca_hsic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_scca_parkhomenko.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_scca_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_stochasticpls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_swcca.py
--rw-r--r--   0 runner    (1001) docker     (123)    12655 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_kcca.py
--rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_mcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_ncca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_partialcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_pcacca.py
--rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_pls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_prcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_tcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/data/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/data/deep.py
--rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/data/simulated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/deep/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_ey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_noi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_sdl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dgcca.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dtcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/deep/_generative/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_generative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_generative/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_generative/_dccae.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_generative/_dvcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_generative/_splitae.py
--rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/objectives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/model_selection/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/model_selection/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/model_selection/_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/probabilistic/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/probabilistic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/probabilistic/_probabilisticcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/test_deepmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/test_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/test_probabilistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/test_regularised.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/test_stochastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/test_unregularized.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/utils/check_values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/visualisation/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/visualisation/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-15 16:21:35.000000 cca_zoo-2.0.2/cca_zoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-15 16:21:35.000000 cca_zoo-2.0.2/cca_zoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:21:35.000000 cca_zoo-2.0.2/cca_zoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-15 16:21:35.000000 cca_zoo-2.0.2/cca_zoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 16:21:35.000000 cca_zoo-2.0.2/cca_zoo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/plot_dcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/plot_dcca_custom_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/plot_dcca_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/plot_dvcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/plot_hyperparameter_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/plot_kernel_cca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/plot_many_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/plot_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/plot_sparse_cca.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/plot_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-15 16:21:34.000000 cca_zoo-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/classical/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_gcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_grcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_altmaxvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13664 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_deflation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13828 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_elasticnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8614 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_ey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_gradkcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_incrementalpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_pls_als.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_pmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_scca_admm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_scca_hsic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_scca_parkhomenko.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_scca_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_stochasticpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_swcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12655 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_kcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_mcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_ncca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_partialcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_pcacca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_pls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_prcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_tcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/data/deep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/data/simulated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/deep/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_ey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_noi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_sdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dgcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dtcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/deep/_generative/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_generative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_generative/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_generative/_dccae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_generative/_dvcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_generative/_splitae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/objectives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/model_selection/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/model_selection/_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/probabilistic/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/probabilistic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/probabilistic/_probabilisticcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/test_deepmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/test_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/test_probabilistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/test_regularised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/test_stochastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/test_unregularized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/utils/check_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/visualisation/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/plot_dcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/plot_dcca_custom_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/plot_dcca_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/plot_dvcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/plot_hyperparameter_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/plot_kernel_cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/plot_many_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/plot_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/plot_sparse_cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/plot_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-19 12:41:13.000000 cca_zoo-2.0.3/setup.py
```

### Comparing `cca_zoo-2.0.2/PKG-INFO` & `cca_zoo-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cca_zoo
-Version: 2.0.2
+Version: 2.0.3
 Summary: Canonical Correlation Analysis Zoo: A collection of Regularized, Deep Learning based, Kernel, and Probabilistic methods in a scikit-learn style framework
 Home-page: https://github.com/jameschapman19/cca_zoo
 Author: jameschapman
 Author-email: james.chapman.19@ucl.ac.uk
 License: MIT
 Description: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5748062.svg)](https://doi.org/10.5281/zenodo.4382739)
         [![codecov](https://codecov.io/gh/jameschapman19/cca_zoo/branch/main/graph/badge.svg?token=JHG9VUB0L8)](https://codecov.io/gh/jameschapman19/cca_zoo)
```

### Comparing `cca_zoo-2.0.2/README.md` & `cca_zoo-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/__init__.py` & `cca_zoo-2.0.3/cca_zoo/classical/__init__.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_base.py` & `cca_zoo-2.0.3/cca_zoo/classical/_base.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_dummy.py` & `cca_zoo-2.0.3/cca_zoo/classical/_dummy.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_gcca.py` & `cca_zoo-2.0.3/cca_zoo/classical/_gcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_grcca.py` & `cca_zoo-2.0.3/cca_zoo/classical/_grcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_iterative/__init__.py` & `cca_zoo-2.0.3/cca_zoo/classical/_iterative/__init__.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_altmaxvar.py` & `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_altmaxvar.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_base.py` & `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-from abc import ABC, abstractmethod
-from typing import Iterable, List, Optional, Tuple, Union, Any
+from abc import abstractmethod
+from typing import Iterable, List, Optional, Union, Any
 
 import numpy as np
 import pytorch_lightning as pl
 import torch
 from pytorch_lightning.callbacks import Callback, EarlyStopping
-from torch import Tensor
 from torch.utils import data
 from torch.utils.data import DataLoader
-from tqdm import tqdm
 
 from cca_zoo.data.deep import NumpyDataset
 from cca_zoo.classical import MCCA, rCCA
 from cca_zoo.classical._base import BaseModel
 from cca_zoo.classical._dummy import DummyCCA
 
 # Default Trainer kwargs
@@ -188,75 +186,14 @@
             self.initialization, self.random_state, self.latent_dimensions
         )
         # Fit the initializer on the input views and get the weights as numpy arrays
         self.weights = initializer.fit(views).weights
         self.weights = [weights.astype(np.float32) for weights in self.weights]
 
 
-class BaseDeflation(BaseIterative, ABC):
-    def _fit(self, views: Iterable[np.ndarray]):
-        # if views is a tuple then convert to a list
-        if isinstance(views, tuple):
-            views = list(views)
-        # tqdm for each latent dimension
-        for k in tqdm(
-            range(self.latent_dimensions), desc="Latent Dimension", leave=False
-        ):
-            train_dataloader, val_dataloader = self.get_dataloader(views)
-            loop = self._get_module(weights=self.weights, k=k)
-            # make a trainer
-            trainer = pl.Trainer(
-                max_epochs=self.epochs, callbacks=self.callbacks, **self.trainer_kwargs
-            )
-            trainer.fit(loop, train_dataloader, val_dataloader)
-            # return the weights from the module. They will need to be changed from torch tensors to numpy arrays
-            weights = loop.weights
-            for i, (view, weight) in enumerate(zip(views, weights)):
-                self.weights[i][:, k] = weight
-                views[i] = self._deflate(view, weight)
-            # if loop has tracked the objective, return the objective
-            if hasattr(loop, "epoch_objective"):
-                self.objective = loop.epoch_objective
-        return self.weights
-
-    def _deflate(self, residual: np.ndarray, weights: np.ndarray) -> np.ndarray:
-        """Deflate view residual by CCA deflation.
-
-        Parameters
-        ----------
-        residual : np.ndarray
-            The current residual data matrix for a view
-        weights : np.ndarray
-            The current CCA weights for a view
-
-        Returns
-        -------
-        np.ndarray
-            The deflated residual data matrix for a view
-
-        Raises
-        ------
-        ValueError
-            If deflation method is not one of ["cca", "pls"]
-        """
-        # Compute the score vector for a view
-        score = residual @ weights
-
-        # Deflate the residual by different methods based on the deflation attribute
-        if self.deflation == "cca":
-            return residual - np.outer(score, score) @ residual / np.dot(score, score)
-        elif self.deflation == "pls":
-            return residual - np.outer(score, weights)
-        else:
-            raise ValueError(
-                f"Invalid deflation method: {self.deflation}. "
-                f"Must be one of ['cca', 'pls']."
-            )
-
-
 class BaseLoop(pl.LightningModule):
     def __init__(
         self,
         weights=None,
         k=None,
         automatic_optimization=False,
         tracking=False,
```

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_elasticnet.py` & `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_elasticnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import warnings
 from typing import Iterable, Union
 
 import numpy as np
 import torch
 from sklearn.linear_model import ElasticNet, Lasso, Ridge, SGDRegressor
 
-from cca_zoo.classical._iterative._base import BaseDeflation, BaseLoop
+from cca_zoo.classical._iterative._base import BaseLoop
+from cca_zoo.classical._iterative._deflation import BaseDeflation
 from cca_zoo.utils import _process_parameter
 
 
 class ElasticCCA(BaseDeflation):
     r"""
     A class used to fit an elastic CCA model for two or more views of data.
```

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_ey.py` & `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_ey.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     epochs : int, optional
         Number of epochs to use, by default 1
     learning_rate : float, optional
         Learning rate to use, by default 0.01
 
     References
     ----------
-    Chapman, James, Ana Lawry Aguila, and Lennie Wells. "A Generalized EigenGame with Extensions to Multiview Representation Learning." arXiv preprint arXiv:2211.11323 (2022).
+    Chapman, James, Ana Lawry Aguila, and Lennie Wells. "A GeneralizedDeflation EigenGame with Extensions to Multiview Representation Learning." arXiv preprint arXiv:2211.11323 (2022).
     """
 
     def __init__(
         self,
         latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
@@ -105,15 +105,15 @@
     epochs : int, optional
         Number of epochs to use, by default 1
     learning_rate : float, optional
         Learning rate to use, by default 0.01
 
     References
     ----------
-    Chapman, James, Ana Lawry Aguila, and Lennie Wells. "A Generalized EigenGame with Extensions to Multiview Representation Learning." arXiv preprint arXiv:2211.11323 (2022).
+    Chapman, James, Ana Lawry Aguila, and Lennie Wells. "A GeneralizedDeflation EigenGame with Extensions to Multiview Representation Learning." arXiv preprint arXiv:2211.11323 (2022).
     """
 
     def __init__(
         self,
         latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
```

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_gh.py` & `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_gh.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_gradkcca.py` & `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_gradkcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_incrementalpls.py` & `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_incrementalpls.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_pls_als.py` & `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_pls_als.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Union
 
 import numpy as np
 
 
-from cca_zoo.classical._iterative._base import BaseDeflation, BaseLoop
+from cca_zoo.classical._iterative._base import BaseLoop
+from cca_zoo.classical._iterative._deflation import BaseDeflation
 from cca_zoo.classical._pls import PLSMixin
 
 
 class PLS_ALS(BaseDeflation, PLSMixin):
     r"""
     A class used to fit a PLS model by alternating least squares (ALS).
```

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_pmd.py` & `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_pmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import itertools
 import warnings
 
 import numpy as np
 import torch
 
-from cca_zoo.classical._iterative._base import BaseDeflation, BaseLoop
+from cca_zoo.classical._iterative._base import BaseLoop
+from cca_zoo.classical._iterative._deflation import BaseDeflation
 from cca_zoo.classical._pls import PLSMixin
 from cca_zoo.classical._search import _delta_search
 from cca_zoo.utils import _check_converged_weights, _process_parameter
 
 
 class SCCA_PMD(BaseDeflation, PLSMixin):
     r"""
```

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_scca_admm.py` & `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_scca_admm.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_scca_hsic.py` & `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_scca_hsic.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_scca_parkhomenko.py` & `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_scca_parkhomenko.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Iterable, Union
 
 import numpy as np
 import pytorch_lightning as pl
 
-from cca_zoo.classical._iterative._base import BaseDeflation, BaseLoop
+from cca_zoo.classical._iterative._base import BaseLoop
+from cca_zoo.classical._iterative._deflation import BaseDeflation
 from cca_zoo.classical._search import _softthreshold
 from cca_zoo.utils import _process_parameter
 
 
 class SCCA_Parkhomenko(BaseDeflation):
     r"""
     A class used to fit a sparse CCA (penalized CCA) model for two or more views.
```

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_scca_span.py` & `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_scca_span.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_stochasticpls.py` & `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_stochasticpls.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_svd.py` & `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_svd.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_swcca.py` & `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_swcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_kcca.py` & `cca_zoo-2.0.3/cca_zoo/classical/_kcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_mcca.py` & `cca_zoo-2.0.3/cca_zoo/classical/_mcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_ncca.py` & `cca_zoo-2.0.3/cca_zoo/classical/_ncca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_partialcca.py` & `cca_zoo-2.0.3/cca_zoo/classical/_partialcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_pcacca.py` & `cca_zoo-2.0.3/cca_zoo/classical/_pcacca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_pls.py` & `cca_zoo-2.0.3/cca_zoo/classical/_pls.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,17 @@
         -------
         variance : numpy array of shape (n_views, latent_dimensions)
 
         """
         views = list(views)
         # Calculate total variance in each view by SVD
         n = views[0].shape[0]
-        if n < min(views[0].shape[1], views[1].shape[1]):
-            views = [reduce_dims(view) for view in views]
+        for i, view in enumerate(views):
+            if n < view.shape[1]:
+                views[i] = reduce_dims(view)
         variance = np.array(
             [np.sum(np.linalg.svd(view)[1] ** 2, keepdims=True) / n for view in views]
         )
         return variance
 
     def total_covariance_(self, views: Iterable[np.ndarray], **kwargs) -> float:
         """
@@ -75,17 +76,17 @@
         -------
         covariance : float
 
         """
         views = list(views)
         # Calculate total covariance by SVD
         n = views[0].shape[0]
-        # if n<p calculate views[0]@views[0].T@views[1]@views[1].T else calculate views[0].T@views[1]
-        if n < min(views[0].shape[1], views[1].shape[1]):
-            views = [reduce_dims(view) for view in views]
+        for i, view in enumerate(views):
+            if n < view.shape[1]:
+                views[i] = reduce_dims(view)
         covariance = np.sum(np.linalg.svd(views[0].T @ views[1])[1]) / (n - 1)
         return covariance
 
     def explained_variance_(self, views: Iterable[np.ndarray], **kwargs) -> np.ndarray:
         """
         Returns the total variance for each view
```

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_prcca.py` & `cca_zoo-2.0.3/cca_zoo/classical/_prcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_search.py` & `cca_zoo-2.0.3/cca_zoo/classical/_search.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/classical/_tcca.py` & `cca_zoo-2.0.3/cca_zoo/classical/_tcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/data/deep.py` & `cca_zoo-2.0.3/cca_zoo/data/deep.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/data/simulated.py` & `cca_zoo-2.0.3/cca_zoo/data/simulated.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/deep/__init__.py` & `cca_zoo-2.0.3/cca_zoo/deep/__init__.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/deep/_base.py` & `cca_zoo-2.0.3/cca_zoo/deep/_base.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca.py` & `cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py` & `cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_ey.py` & `cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_ey.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class DCCA_EY(DCCA):
     """
 
     References
     ----------
-    Chapman, James, Ana Lawry Aguila, and Lennie Wells. "A Generalized EigenGame with Extensions to Multiview Representation Learning." arXiv preprint arXiv:2211.11323 (2022).
+    Chapman, James, Ana Lawry Aguila, and Lennie Wells. "A GeneralizedDeflation EigenGame with Extensions to Multiview Representation Learning." arXiv preprint arXiv:2211.11323 (2022).
     """
 
     def __init__(self, latent_dimensions: int, encoders=None, r: float = 0, **kwargs):
         super().__init__(
             latent_dimensions=latent_dimensions, encoders=encoders, **kwargs
         )
         self.r = r
```

### Comparing `cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_gh.py` & `cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_gh.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_noi.py` & `cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_noi.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_sdl.py` & `cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_sdl.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_svd.py` & `cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_svd.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class DCCA_SVD(DCCA):
     """
 
     References
     ----------
-    Chapman, James, Ana Lawry Aguila, and Lennie Wells. "A Generalized EigenGame with Extensions to Multiview Representation Learning." arXiv preprint arXiv:2211.11323 (2022).
+    Chapman, James, Ana Lawry Aguila, and Lennie Wells. "A GeneralizedDeflation EigenGame with Extensions to Multiview Representation Learning." arXiv preprint arXiv:2211.11323 (2022).
     """
 
     def __init__(self, latent_dimensions: int, encoders=None, r: float = 0, **kwargs):
         super().__init__(
             latent_dimensions=latent_dimensions, encoders=encoders, **kwargs
         )
         self.r = r
```

### Comparing `cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dgcca.py` & `cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dgcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dtcca.py` & `cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dtcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/deep/_generative/_base.py` & `cca_zoo-2.0.3/cca_zoo/deep/_generative/_base.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/deep/_generative/_dccae.py` & `cca_zoo-2.0.3/cca_zoo/deep/_generative/_dccae.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/deep/_generative/_dvcca.py` & `cca_zoo-2.0.3/cca_zoo/deep/_generative/_dvcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/deep/_generative/_splitae.py` & `cca_zoo-2.0.3/cca_zoo/deep/_generative/_splitae.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/deep/architectures.py` & `cca_zoo-2.0.3/cca_zoo/deep/architectures.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/deep/metrics.py` & `cca_zoo-2.0.3/cca_zoo/deep/metrics.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/deep/objectives.py` & `cca_zoo-2.0.3/cca_zoo/deep/objectives.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/model_selection/_search.py` & `cca_zoo-2.0.3/cca_zoo/model_selection/_search.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/model_selection/_validation.py` & `cca_zoo-2.0.3/cca_zoo/model_selection/_validation.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/probabilistic/_probabilisticcca.py` & `cca_zoo-2.0.3/cca_zoo/probabilistic/_probabilisticcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/test/test_callbacks.py` & `cca_zoo-2.0.3/cca_zoo/test/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/test/test_data.py` & `cca_zoo-2.0.3/cca_zoo/test/test_data.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/test/test_deepmodels.py` & `cca_zoo-2.0.3/cca_zoo/test/test_deepmodels.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/test/test_kernel.py` & `cca_zoo-2.0.3/cca_zoo/test/test_kernel.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/test/test_probabilistic.py` & `cca_zoo-2.0.3/cca_zoo/test/test_probabilistic.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/test/test_regularised.py` & `cca_zoo-2.0.3/cca_zoo/test/test_regularised.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/test/test_stochastic.py` & `cca_zoo-2.0.3/cca_zoo/test/test_stochastic.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/test/test_unregularized.py` & `cca_zoo-2.0.3/cca_zoo/test/test_unregularized.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/test/test_utils.py` & `cca_zoo-2.0.3/cca_zoo/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/utils/check_values.py` & `cca_zoo-2.0.3/cca_zoo/utils/check_values.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo/visualisation/plotting.py` & `cca_zoo-2.0.3/cca_zoo/visualisation/plotting.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/cca_zoo.egg-info/PKG-INFO` & `cca_zoo-2.0.3/cca_zoo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cca-zoo
-Version: 2.0.2
+Version: 2.0.3
 Summary: Canonical Correlation Analysis Zoo: A collection of Regularized, Deep Learning based, Kernel, and Probabilistic methods in a scikit-learn style framework
 Home-page: https://github.com/jameschapman19/cca_zoo
 Author: jameschapman
 Author-email: james.chapman.19@ucl.ac.uk
 License: MIT
 Description: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5748062.svg)](https://doi.org/10.5281/zenodo.4382739)
         [![codecov](https://codecov.io/gh/jameschapman19/cca_zoo/branch/main/graph/badge.svg?token=JHG9VUB0L8)](https://codecov.io/gh/jameschapman19/cca_zoo)
```

### Comparing `cca_zoo-2.0.2/cca_zoo.egg-info/SOURCES.txt` & `cca_zoo-2.0.3/cca_zoo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 cca_zoo/classical/_pls.py
 cca_zoo/classical/_prcca.py
 cca_zoo/classical/_search.py
 cca_zoo/classical/_tcca.py
 cca_zoo/classical/_iterative/__init__.py
 cca_zoo/classical/_iterative/_altmaxvar.py
 cca_zoo/classical/_iterative/_base.py
+cca_zoo/classical/_iterative/_deflation.py
 cca_zoo/classical/_iterative/_elasticnet.py
 cca_zoo/classical/_iterative/_ey.py
 cca_zoo/classical/_iterative/_gh.py
 cca_zoo/classical/_iterative/_gradkcca.py
 cca_zoo/classical/_iterative/_incrementalpls.py
 cca_zoo/classical/_iterative/_pls_als.py
 cca_zoo/classical/_iterative/_pmd.py
```

### Comparing `cca_zoo-2.0.2/examples/__init__.py` & `cca_zoo-2.0.3/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/examples/plot_dcca.py` & `cca_zoo-2.0.3/examples/plot_dcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/examples/plot_dcca_custom_data.py` & `cca_zoo-2.0.3/examples/plot_dcca_custom_data.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/examples/plot_dcca_multi.py` & `cca_zoo-2.0.3/examples/plot_dcca_multi.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/examples/plot_dvcca.py` & `cca_zoo-2.0.3/examples/plot_dvcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/examples/plot_hyperparameter_selection.py` & `cca_zoo-2.0.3/examples/plot_hyperparameter_selection.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/examples/plot_kernel_cca.py` & `cca_zoo-2.0.3/examples/plot_kernel_cca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/examples/plot_many_views.py` & `cca_zoo-2.0.3/examples/plot_many_views.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/examples/plot_plotting.py` & `cca_zoo-2.0.3/examples/plot_plotting.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/examples/plot_sparse_cca.py` & `cca_zoo-2.0.3/examples/plot_sparse_cca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/examples/plot_validation.py` & `cca_zoo-2.0.3/examples/plot_validation.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.2/setup.py` & `cca_zoo-2.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "deep": ["torch", "torchvision", "pytorch-lightning"],
     "probabilistic": ["jax", "numpyro", "arviz"],
 }
 EXTRA_PACKAGES["all"] = EXTRA_PACKAGES["deep"] + EXTRA_PACKAGES["probabilistic"]
 
 setup(
     name="cca_zoo",
-    version="2.0.2",
+    version="2.0.3",
     include_package_data=True,
     keywords="cca",
     packages=find_packages(),
     url="https://github.com/jameschapman19/cca_zoo",
     license="MIT",
     author="jameschapman",
     description=(
```

