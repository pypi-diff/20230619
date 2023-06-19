# Comparing `tmp/gwdetchar-2.1.0.tar.gz` & `tmp/gwdetchar-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdetchar-2.1.0.tar", last modified: Sat Jun 17 00:03:06 2023, max compression
+gzip compressed data, was "gwdetchar-2.1.1.tar", last modified: Mon Jun 19 18:13:48 2023, max compression
```

## Comparing `gwdetchar-2.1.0.tar` & `gwdetchar-2.1.1.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.672925 gwdetchar-2.1.0/
--rw-r--r--   0 egoetz     (501) staff       (20)      184 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/.codecov.yml
--rw-r--r--   0 egoetz     (501) staff       (20)      134 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/.flake8
--rw-r--r--   0 egoetz     (501) staff       (20)       35 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/.gitattributes
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.567351 gwdetchar-2.1.0/.github/
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.582700 gwdetchar-2.1.0/.github/workflows/
--rw-r--r--   0 egoetz     (501) staff       (20)     2885 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/.github/workflows/build.yml
--rw-r--r--   0 egoetz     (501) staff       (20)     1334 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/.github/workflows/docs.yml
--rw-r--r--   0 egoetz     (501) staff       (20)     1084 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/.github/workflows/lint.yml
--rw-r--r--   0 egoetz     (501) staff       (20)      617 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/.gitignore
--rw-r--r--   0 egoetz     (501) staff       (20)      577 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/.readthedocs.yml
--rw-r--r--   0 egoetz     (501) staff       (20)     2638 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/CONTRIBUTING.md
--rw-r--r--   0 egoetz     (501) staff       (20)    35147 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/LICENSE
--rw-r--r--   0 egoetz     (501) staff       (20)       69 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/MANIFEST.in
--rw-r--r--   0 egoetz     (501) staff       (20)     3726 2023-06-17 00:03:06.672402 gwdetchar-2.1.0/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2328 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/README.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.583376 gwdetchar-2.1.0/ci/
--rw-r--r--   0 egoetz     (501) staff       (20)     1135 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/ci/test-cli.sh
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.585552 gwdetchar-2.1.0/docs/
--rw-r--r--   0 egoetz     (501) staff       (20)     6857 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/docs/Makefile
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.568003 gwdetchar-2.1.0/docs/_static/
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.586437 gwdetchar-2.1.0/docs/_static/css/
--rw-r--r--   0 egoetz     (501) staff       (20)     4997 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/docs/_static/css/custom.css
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.587096 gwdetchar-2.1.0/docs/api/
--rw-r--r--   0 egoetz     (501) staff       (20)       54 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/docs/api/index.rst
--rw-r--r--   0 egoetz     (501) staff       (20)    10994 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/docs/conf.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.587750 gwdetchar-2.1.0/docs/conlog/
--rw-r--r--   0 egoetz     (501) staff       (20)      964 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/docs/conlog/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.588637 gwdetchar-2.1.0/docs/daq/
--rw-r--r--   0 egoetz     (501) staff       (20)     1807 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/docs/daq/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.589270 gwdetchar-2.1.0/docs/data/
--rw-r--r--   0 egoetz     (501) staff       (20)      863 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/docs/data/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.589989 gwdetchar-2.1.0/docs/html/
--rw-r--r--   0 egoetz     (501) staff       (20)     1488 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/docs/html/index.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     2968 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/docs/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.590628 gwdetchar-2.1.0/docs/lasso/
--rw-r--r--   0 egoetz     (501) staff       (20)     1439 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/docs/lasso/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.591228 gwdetchar-2.1.0/docs/nagios/
--rw-r--r--   0 egoetz     (501) staff       (20)      941 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/docs/nagios/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.591877 gwdetchar-2.1.0/docs/omega/
--rw-r--r--   0 egoetz     (501) staff       (20)     3035 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/docs/omega/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.592499 gwdetchar-2.1.0/docs/saturation/
--rw-r--r--   0 egoetz     (501) staff       (20)     1638 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/docs/saturation/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.593367 gwdetchar-2.1.0/docs/scattering/
--rw-r--r--   0 egoetz     (501) staff       (20)     2926 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/docs/scattering/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.604874 gwdetchar-2.1.0/gwdetchar/
--rw-r--r--   0 egoetz     (501) staff       (20)     1408 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/gwdetchar/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)      160 2023-06-17 00:03:06.000000 gwdetchar-2.1.0/gwdetchar/_version.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3732 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/cds.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4738 2023-05-16 23:56:26.000000 gwdetchar-2.1.0/gwdetchar/cli.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2773 2023-04-25 15:49:41.000000 gwdetchar-2.1.0/gwdetchar/condor.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2703 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/conftest.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7363 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/conlog.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2997 2023-05-17 00:05:55.000000 gwdetchar-2.1.0/gwdetchar/const.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7440 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/daq.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.612968 gwdetchar-2.1.0/gwdetchar/io/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/io/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7522 2023-06-17 00:02:41.000000 gwdetchar-2.1.0/gwdetchar/io/datafind.py
--rw-r--r--   0 egoetz     (501) staff       (20)    41413 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/gwdetchar/io/html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3749 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/io/ligolw.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.616185 gwdetchar-2.1.0/gwdetchar/io/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      827 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/io/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4834 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/io/tests/test_datafind.py
--rw-r--r--   0 egoetz     (501) staff       (20)    24146 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/gwdetchar/io/tests/test_html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2455 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/io/tests/test_ligolw.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.621633 gwdetchar-2.1.0/gwdetchar/lasso/
--rw-r--r--   0 egoetz     (501) staff       (20)     1063 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/lasso/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    35568 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/gwdetchar/lasso/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6652 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/lasso/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    20595 2022-10-03 17:36:21.000000 gwdetchar-2.1.0/gwdetchar/lasso/old.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4946 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/lasso/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.629730 gwdetchar-2.1.0/gwdetchar/lasso/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/lasso/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3984 2023-04-27 00:53:55.000000 gwdetchar-2.1.0/gwdetchar/lasso/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1549 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/lasso/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2142 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/lasso/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6744 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/mct.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.638209 gwdetchar-2.1.0/gwdetchar/nagios/
--rw-r--r--   0 egoetz     (501) staff       (20)      887 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/nagios/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2959 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/nagios/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2166 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/nagios/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.639984 gwdetchar-2.1.0/gwdetchar/nagios/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/nagios/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2131 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/nagios/tests/test_main.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.651116 gwdetchar-2.1.0/gwdetchar/omega/
--rw-r--r--   0 egoetz     (501) staff       (20)     1188 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13880 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    12682 2023-05-16 23:56:26.000000 gwdetchar-2.1.0/gwdetchar/omega/batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)    15875 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/config.py
--rw-r--r--   0 egoetz     (501) staff       (20)    10365 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    20699 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8871 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.655049 gwdetchar-2.1.0/gwdetchar/omega/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3689 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/tests/test_batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6970 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/tests/test_config.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5493 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13502 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/gwdetchar/omega/tests/test_html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     9824 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2702 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)    17732 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/overflow.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2244 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.657251 gwdetchar-2.1.0/gwdetchar/saturation/
--rw-r--r--   0 egoetz     (501) staff       (20)     1039 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/saturation/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13870 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/saturation/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7654 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/saturation/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.658443 gwdetchar-2.1.0/gwdetchar/saturation/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/saturation/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3510 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/saturation/tests/test_saturation.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.661821 gwdetchar-2.1.0/gwdetchar/scattering/
--rw-r--r--   0 egoetz     (501) staff       (20)     1983 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/scattering/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    32277 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/scattering/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6413 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/scattering/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5282 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/scattering/plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8523 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/scattering/simple.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.665006 gwdetchar-2.1.0/gwdetchar/scattering/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/scattering/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2238 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/scattering/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5520 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/scattering/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1831 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/scattering/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3156 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/scattering/tests/test_simple.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.671489 gwdetchar-2.1.0/gwdetchar/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3276 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/tests/test_cds.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3181 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/tests/test_cli.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1918 2023-04-25 15:49:41.000000 gwdetchar-2.1.0/gwdetchar/tests/test_condor.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4819 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/tests/test_conlog.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1928 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/tests/test_const.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3306 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/tests/test_daq.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2077 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2831 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/tests/test_utils.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4531 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/utils.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.608977 gwdetchar-2.1.0/gwdetchar.egg-info/
--rw-r--r--   0 egoetz     (501) staff       (20)     3726 2023-06-17 00:03:06.000000 gwdetchar-2.1.0/gwdetchar.egg-info/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2832 2023-06-17 00:03:06.000000 gwdetchar-2.1.0/gwdetchar.egg-info/SOURCES.txt
--rw-r--r--   0 egoetz     (501) staff       (20)        1 2023-06-17 00:03:06.000000 gwdetchar-2.1.0/gwdetchar.egg-info/dependency_links.txt
--rw-r--r--   0 egoetz     (501) staff       (20)      591 2023-06-17 00:03:06.000000 gwdetchar-2.1.0/gwdetchar.egg-info/entry_points.txt
--rw-r--r--   0 egoetz     (501) staff       (20)      353 2023-06-17 00:03:06.000000 gwdetchar-2.1.0/gwdetchar.egg-info/requires.txt
--rw-r--r--   0 egoetz     (501) staff       (20)       10 2023-06-17 00:03:06.000000 gwdetchar-2.1.0/gwdetchar.egg-info/top_level.txt
--rw-r--r--   0 egoetz     (501) staff       (20)     3462 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/pyproject.toml
--rw-r--r--   0 egoetz     (501) staff       (20)       38 2023-06-17 00:03:06.673062 gwdetchar-2.1.0/setup.cfg
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.480367 gwdetchar-2.1.1/
+-rw-r--r--   0 egoetz     (501) staff       (20)      184 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/.codecov.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      134 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/.flake8
+-rw-r--r--   0 egoetz     (501) staff       (20)       35 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/.gitattributes
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.401522 gwdetchar-2.1.1/.github/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.416593 gwdetchar-2.1.1/.github/workflows/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2885 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/.github/workflows/build.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)     1334 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/.github/workflows/docs.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)     1084 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/.github/workflows/lint.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      617 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/.gitignore
+-rw-r--r--   0 egoetz     (501) staff       (20)      577 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/.readthedocs.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)     2638 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/CONTRIBUTING.md
+-rw-r--r--   0 egoetz     (501) staff       (20)    35147 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/LICENSE
+-rw-r--r--   0 egoetz     (501) staff       (20)       69 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/MANIFEST.in
+-rw-r--r--   0 egoetz     (501) staff       (20)     3726 2023-06-19 18:13:48.479852 gwdetchar-2.1.1/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2328 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/README.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.417203 gwdetchar-2.1.1/ci/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1135 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/ci/test-cli.sh
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.419003 gwdetchar-2.1.1/docs/
+-rw-r--r--   0 egoetz     (501) staff       (20)     6857 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/docs/Makefile
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.402153 gwdetchar-2.1.1/docs/_static/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.419826 gwdetchar-2.1.1/docs/_static/css/
+-rw-r--r--   0 egoetz     (501) staff       (20)     4997 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/docs/_static/css/custom.css
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.420299 gwdetchar-2.1.1/docs/api/
+-rw-r--r--   0 egoetz     (501) staff       (20)       54 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/docs/api/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)    10994 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/docs/conf.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.420707 gwdetchar-2.1.1/docs/conlog/
+-rw-r--r--   0 egoetz     (501) staff       (20)      964 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/docs/conlog/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.421671 gwdetchar-2.1.1/docs/daq/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1807 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/docs/daq/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.422276 gwdetchar-2.1.1/docs/data/
+-rw-r--r--   0 egoetz     (501) staff       (20)      863 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/docs/data/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.422862 gwdetchar-2.1.1/docs/html/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1488 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/docs/html/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     2968 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/docs/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.423373 gwdetchar-2.1.1/docs/lasso/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1439 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/docs/lasso/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.424052 gwdetchar-2.1.1/docs/nagios/
+-rw-r--r--   0 egoetz     (501) staff       (20)      941 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/docs/nagios/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.424814 gwdetchar-2.1.1/docs/omega/
+-rw-r--r--   0 egoetz     (501) staff       (20)     3035 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/docs/omega/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.425524 gwdetchar-2.1.1/docs/saturation/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1638 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/docs/saturation/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.426276 gwdetchar-2.1.1/docs/scattering/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2926 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/docs/scattering/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.436457 gwdetchar-2.1.1/gwdetchar/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1408 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/gwdetchar/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)      160 2023-06-19 18:13:48.000000 gwdetchar-2.1.1/gwdetchar/_version.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3732 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/cds.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4738 2023-05-16 23:56:26.000000 gwdetchar-2.1.1/gwdetchar/cli.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2773 2023-04-25 15:49:41.000000 gwdetchar-2.1.1/gwdetchar/condor.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2703 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/conftest.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7363 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/conlog.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2997 2023-05-17 00:05:55.000000 gwdetchar-2.1.1/gwdetchar/const.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7440 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/daq.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.440990 gwdetchar-2.1.1/gwdetchar/io/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/io/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7584 2023-06-19 18:12:55.000000 gwdetchar-2.1.1/gwdetchar/io/datafind.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    41413 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/gwdetchar/io/html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3764 2023-06-19 18:12:55.000000 gwdetchar-2.1.1/gwdetchar/io/ligolw.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.443060 gwdetchar-2.1.1/gwdetchar/io/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      827 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/io/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4834 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/io/tests/test_datafind.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    24146 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/gwdetchar/io/tests/test_html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2451 2023-06-19 18:12:55.000000 gwdetchar-2.1.1/gwdetchar/io/tests/test_ligolw.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.447783 gwdetchar-2.1.1/gwdetchar/lasso/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1063 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/lasso/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    35568 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/gwdetchar/lasso/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6652 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/lasso/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20595 2022-10-03 17:36:21.000000 gwdetchar-2.1.1/gwdetchar/lasso/old.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4946 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/lasso/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.450190 gwdetchar-2.1.1/gwdetchar/lasso/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/lasso/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3984 2023-04-27 00:53:55.000000 gwdetchar-2.1.1/gwdetchar/lasso/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1549 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/lasso/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2142 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/lasso/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6744 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/mct.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.451375 gwdetchar-2.1.1/gwdetchar/nagios/
+-rw-r--r--   0 egoetz     (501) staff       (20)      887 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/nagios/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2959 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/nagios/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2166 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/nagios/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.452159 gwdetchar-2.1.1/gwdetchar/nagios/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/nagios/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2131 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/nagios/tests/test_main.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.456175 gwdetchar-2.1.1/gwdetchar/omega/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1188 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    13880 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    12682 2023-05-16 23:56:26.000000 gwdetchar-2.1.1/gwdetchar/omega/batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    15875 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/config.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10365 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20699 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8871 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.460717 gwdetchar-2.1.1/gwdetchar/omega/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3689 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/tests/test_batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6970 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/tests/test_config.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5493 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    13502 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/gwdetchar/omega/tests/test_html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     9824 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2702 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    17732 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/overflow.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2244 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.463657 gwdetchar-2.1.1/gwdetchar/saturation/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1039 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/saturation/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    13870 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/saturation/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7654 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/saturation/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.465177 gwdetchar-2.1.1/gwdetchar/saturation/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/saturation/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3510 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/saturation/tests/test_saturation.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.468893 gwdetchar-2.1.1/gwdetchar/scattering/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1983 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/scattering/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    32277 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/scattering/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6413 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/scattering/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5282 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/scattering/plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8523 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/scattering/simple.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.472746 gwdetchar-2.1.1/gwdetchar/scattering/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/scattering/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2238 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/scattering/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5520 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/scattering/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1831 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/scattering/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3156 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/scattering/tests/test_simple.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.478957 gwdetchar-2.1.1/gwdetchar/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3276 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/tests/test_cds.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3181 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/tests/test_cli.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1918 2023-04-25 15:49:41.000000 gwdetchar-2.1.1/gwdetchar/tests/test_condor.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4819 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/tests/test_conlog.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1928 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/tests/test_const.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3306 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/tests/test_daq.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2077 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2831 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/tests/test_utils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4531 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/utils.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.439235 gwdetchar-2.1.1/gwdetchar.egg-info/
+-rw-r--r--   0 egoetz     (501) staff       (20)     3726 2023-06-19 18:13:48.000000 gwdetchar-2.1.1/gwdetchar.egg-info/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2832 2023-06-19 18:13:48.000000 gwdetchar-2.1.1/gwdetchar.egg-info/SOURCES.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)        1 2023-06-19 18:13:48.000000 gwdetchar-2.1.1/gwdetchar.egg-info/dependency_links.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      591 2023-06-19 18:13:48.000000 gwdetchar-2.1.1/gwdetchar.egg-info/entry_points.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      348 2023-06-19 18:13:48.000000 gwdetchar-2.1.1/gwdetchar.egg-info/requires.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)       10 2023-06-19 18:13:48.000000 gwdetchar-2.1.1/gwdetchar.egg-info/top_level.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)     3457 2023-06-19 18:12:55.000000 gwdetchar-2.1.1/pyproject.toml
+-rw-r--r--   0 egoetz     (501) staff       (20)       38 2023-06-19 18:13:48.480508 gwdetchar-2.1.1/setup.cfg
```

### Comparing `gwdetchar-2.1.0/.github/workflows/build.yml` & `gwdetchar-2.1.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/.github/workflows/docs.yml` & `gwdetchar-2.1.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/.github/workflows/lint.yml` & `gwdetchar-2.1.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/.gitignore` & `gwdetchar-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/.readthedocs.yml` & `gwdetchar-2.1.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/CONTRIBUTING.md` & `gwdetchar-2.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/LICENSE` & `gwdetchar-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/PKG-INFO` & `gwdetchar-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdetchar
-Version: 2.1.0
+Version: 2.1.1
 Summary: A python package for gravitational-wave detector characterisation
 Author-email: Alex Urban <alex.urban@ligo.org>, Duncan Macleod <duncan.macleod@ligo.org>
 Maintainer-email: Evan Goetz <evan.goetz@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://gwdetchar.readthedocs.io
 Project-URL: Source Code, https://github.com/gwdetchar/gwdetchar
 Project-URL: Bug Tracker, https://github.com/gwdetchar/gwdetchar/issues
```

### Comparing `gwdetchar-2.1.0/README.rst` & `gwdetchar-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/ci/test-cli.sh` & `gwdetchar-2.1.1/ci/test-cli.sh`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/docs/Makefile` & `gwdetchar-2.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/docs/_static/css/custom.css` & `gwdetchar-2.1.1/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/docs/conf.py` & `gwdetchar-2.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/docs/conlog/index.rst` & `gwdetchar-2.1.1/docs/conlog/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/docs/daq/index.rst` & `gwdetchar-2.1.1/docs/daq/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/docs/data/index.rst` & `gwdetchar-2.1.1/docs/data/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/docs/html/index.rst` & `gwdetchar-2.1.1/docs/html/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/docs/index.rst` & `gwdetchar-2.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/docs/lasso/index.rst` & `gwdetchar-2.1.1/docs/lasso/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/docs/nagios/index.rst` & `gwdetchar-2.1.1/docs/nagios/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/docs/omega/index.rst` & `gwdetchar-2.1.1/docs/omega/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/docs/saturation/index.rst` & `gwdetchar-2.1.1/docs/saturation/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/docs/scattering/index.rst` & `gwdetchar-2.1.1/docs/scattering/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/__init__.py` & `gwdetchar-2.1.1/gwdetchar/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/cds.py` & `gwdetchar-2.1.1/gwdetchar/cds.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/cli.py` & `gwdetchar-2.1.1/gwdetchar/cli.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/condor.py` & `gwdetchar-2.1.1/gwdetchar/condor.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/conftest.py` & `gwdetchar-2.1.1/gwdetchar/conftest.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/conlog.py` & `gwdetchar-2.1.1/gwdetchar/conlog.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/const.py` & `gwdetchar-2.1.1/gwdetchar/const.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/daq.py` & `gwdetchar-2.1.1/gwdetchar/daq.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/io/__init__.py` & `gwdetchar-2.1.1/gwdetchar/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/io/datafind.py` & `gwdetchar-2.1.1/gwdetchar/io/datafind.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,14 +183,16 @@
     """
     # get TimeSeries class
     if isinstance(channel, (list, tuple)):
         series_class = TimeSeriesDict
     else:
         series_class = TimeSeries
 
+    pad = kwargs.pop('pad', None)
+
     if frametype is not None:
         try:  # locate frame files
             ifo = re.search('[A-Z]1', frametype).group(0)
             obs = ifo[0]
             on_gaps = kwargs.get('on_gaps', 'error')
             source = io_datafind.find_urls(obs, frametype, start, end,
                                            on_gaps=on_gaps, **kwargs)
@@ -201,20 +203,20 @@
             pass
     if source and (isinstance(source, list) and
                    isinstance(channel, (list, tuple))):
         channel = remove_missing_channels(channel, source)
     if source:  # read from frame files
         return series_class.read(
             source, channel, start=start, end=end, nproc=nproc,
-            verbose=verbose, **kwargs)
+            verbose=verbose, pad=pad, **kwargs)
 
     # read single channel from NDS
     if not isinstance(channel, (list, tuple)):
         return series_class.get(
-            channel, start, end, verbose=verbose, **kwargs)
+            channel, start, end, verbose=verbose, pad=pad, **kwargs)
 
     # if all else fails, process channels in groups of 60
     data = series_class()
     for group in [channel[i:i + 60] for i in range(0, len(channel), 60)]:
         data.append(series_class.get(
-            group, start, end, verbose=verbose, **kwargs))
+            group, start, end, verbose=verbose, pad=pad, **kwargs))
     return data
```

### Comparing `gwdetchar-2.1.0/gwdetchar/io/html.py` & `gwdetchar-2.1.1/gwdetchar/io/html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/io/ligolw.py` & `gwdetchar-2.1.1/gwdetchar/io/ligolw.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,43 +15,48 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with GW DetChar.  If not, see <http://www.gnu.org/licenses/>.
 
 """Utilties for LIGO_LW XML I/O
 """
 
+from ligo.lw import (
+    ligolw,
+    table,
+)
 try:
-    from glue.ligolw import (ligolw, table, lsctables)
-except ImportError as exc:
-    exc.args = ("{!s}, please install lscsoft-glue to "
-                "handle LIGO_LW files".format(exc),)
+    from ligo.lw import lsctables
+except ModuleNotFoundError as exc:
+    exc.msg = (
+        f"{exc.msg}, please install python-lal / python3-lal / lalsuite "
+        "to handle LIGO_LW files"
+    )
+    exc.args = (exc.msg,)
     raise
 
 from gwpy.segments import (Segment, DataQualityFlag, DataQualityDict)
 
-LIGOTimeGPS = lsctables.LIGOTimeGPS
-
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
 
 def new_table(tab, *args, **kwargs):
-    """Create a new `~glue.ligolw.Table`
+    """Create a new `~ligo.lw.table.Table`
 
-    This is just a convenience wrapper around `~glue.ligolw.lsctables.New`
+    This is just a convenience wrapper around `~ligo.lw.lsctables.New`
 
     Parameters
     ----------
     tab : `type`, `str`
-        `~glue.ligolw.Table` subclass, or name of table to create
+        `~ligo.lw.table.Table` subclass, or name of table to create
     *args, **kwargs
-        other parameters are passed directly to `~glue.ligolw.lsctables.New`
+        other parameters are passed directly to `~ligo.lw.lsctables.New`
 
     Returns
     -------
-    table : `~glue.ligolw.Table`
+    table : `~ligo.lw.table.Table`
         a newly-created table with the relevant attributes and structure
     """
     if isinstance(tab, str):
         tab = lsctables.TableByName[table.Table.TableName(tab)]
     return lsctables.New(tab, *args, **kwargs)
 
 
@@ -62,33 +67,33 @@
     table = new_table('sngl_burst', columns=list(columns))
     get_next_id = table.get_next_id
     RowType = table.RowType
     append = table.append
     for t in times:
         row = RowType()
         row.event_id = get_next_id()
-        row.set_peak(LIGOTimeGPS(t))
+        row.peak = t
         for key, val in params.items():
             setattr(row, key, val)
         append(row)
     return table
 
 
 def sngl_burst_from_segments(segs, **params):
     """Create a `SnglBurstTable from a `~ligo.segments.segmentlist`
     """
     table = new_table('sngl_burst', columns=params.keys())
-    next_id = table.next_id
+    get_next_id = table.get_next_id
     RowType = table.RowType
     append = table.append
     for seg in segs:
         row = RowType()
-        row.event_id = next_id()
-        row.set_period(seg)
-        row.set_peak(LIGOTimeGPS(seg[0] + abs(seg)/2.))
+        row.event_id = get_next_id()
+        row.peak = seg[0] + abs(seg) / 2.
+        row.period = seg
         for key, val in params.items():
             setattr(row, key, val)
         append(row)
     return table
 
 
 def segments_from_sngl_burst(table, padding, known=None):
@@ -96,15 +101,15 @@
 
     This method creates a `~gwpy.segments.DataQualityFlag` for each unique
     channel found in the given table by padding the peak time by the given
     amount on each side
     """
     out = DataQualityDict()
     for row in table:
-        t = row.get_peak()
+        t = row.peak
         seg = Segment(t-padding, t+padding)
         try:
             out[row.channel].active.append(seg)
         except KeyError:
             out[row.channel] = DataQualityFlag(row.channel, known=known,
                                                active=[seg])
     return out
```

### Comparing `gwdetchar-2.1.0/gwdetchar/io/tests/__init__.py` & `gwdetchar-2.1.1/gwdetchar/io/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/io/tests/test_datafind.py` & `gwdetchar-2.1.1/gwdetchar/io/tests/test_datafind.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/io/tests/test_html.py` & `gwdetchar-2.1.1/gwdetchar/io/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/io/tests/test_ligolw.py` & `gwdetchar-2.1.1/gwdetchar/io/tests/test_ligolw.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 
 import numpy
 from numpy.testing import (assert_array_equal, assert_allclose)
 
 from gwpy.segments import (Segment, SegmentList)
 from gwpy.testing.utils import assert_segmentlist_equal
 
-lsctables = pytest.importorskip("glue.ligolw.lsctables")
+lsctables = pytest.importorskip("ligo.lw.lsctables")
 ligolw = pytest.importorskip("gwdetchar.io.ligolw")
 
 
 def test_new_table():
     tab = ligolw.new_table('sngl_burst')
     assert isinstance(tab, lsctables.SnglBurstTable)
-    assert sorted(tab.columnnames) == sorted(
+    assert sorted(tab.columnnamesreal) == sorted(
         lsctables.SnglBurstTable.validcolumns.keys())
 
     cols = ['peak_time', 'peak_time_ns', 'snr']
     tab = ligolw.new_table(lsctables.SnglBurstTable, columns=cols)
     assert tab.columnnames == cols
 
 
@@ -59,12 +59,12 @@
     segs = ligolw.segments_from_sngl_burst(tab, 1)
     assert_segmentlist_equal(segs['test'].active, SegmentList([
         Segment(0, 2), Segment(3, 5), Segment(6, 8), Segment(9, 11),
     ]))
 
 
 def test_table_to_document():
-    from glue.ligolw.ligolw import Document
+    from ligo.lw.ligolw import Document
     tab = ligolw.new_table('sngl_burst')
     xmldoc = ligolw.table_to_document(tab)
     assert isinstance(xmldoc, Document)
     assert xmldoc.childNodes[-1].childNodes[0] is tab
```

### Comparing `gwdetchar-2.1.0/gwdetchar/lasso/__init__.py` & `gwdetchar-2.1.1/gwdetchar/lasso/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/lasso/__main__.py` & `gwdetchar-2.1.1/gwdetchar/lasso/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/lasso/core.py` & `gwdetchar-2.1.1/gwdetchar/lasso/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/lasso/old.py` & `gwdetchar-2.1.1/gwdetchar/lasso/old.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/lasso/plot.py` & `gwdetchar-2.1.1/gwdetchar/lasso/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/lasso/tests/__init__.py` & `gwdetchar-2.1.1/gwdetchar/lasso/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/lasso/tests/test_core.py` & `gwdetchar-2.1.1/gwdetchar/lasso/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/lasso/tests/test_main.py` & `gwdetchar-2.1.1/gwdetchar/lasso/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/lasso/tests/test_plot.py` & `gwdetchar-2.1.1/gwdetchar/lasso/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/mct.py` & `gwdetchar-2.1.1/gwdetchar/mct.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/nagios/__init__.py` & `gwdetchar-2.1.1/gwdetchar/nagios/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/nagios/__main__.py` & `gwdetchar-2.1.1/gwdetchar/nagios/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/nagios/core.py` & `gwdetchar-2.1.1/gwdetchar/nagios/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/nagios/tests/__init__.py` & `gwdetchar-2.1.1/gwdetchar/nagios/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/nagios/tests/test_main.py` & `gwdetchar-2.1.1/gwdetchar/nagios/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/omega/__init__.py` & `gwdetchar-2.1.1/gwdetchar/omega/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/omega/__main__.py` & `gwdetchar-2.1.1/gwdetchar/omega/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/omega/batch.py` & `gwdetchar-2.1.1/gwdetchar/omega/batch.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/omega/config.py` & `gwdetchar-2.1.1/gwdetchar/omega/config.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/omega/core.py` & `gwdetchar-2.1.1/gwdetchar/omega/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/omega/html.py` & `gwdetchar-2.1.1/gwdetchar/omega/html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/omega/plot.py` & `gwdetchar-2.1.1/gwdetchar/omega/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/omega/tests/__init__.py` & `gwdetchar-2.1.1/gwdetchar/omega/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/omega/tests/test_batch.py` & `gwdetchar-2.1.1/gwdetchar/omega/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/omega/tests/test_config.py` & `gwdetchar-2.1.1/gwdetchar/omega/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/omega/tests/test_core.py` & `gwdetchar-2.1.1/gwdetchar/omega/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/omega/tests/test_html.py` & `gwdetchar-2.1.1/gwdetchar/omega/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/omega/tests/test_main.py` & `gwdetchar-2.1.1/gwdetchar/omega/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/omega/tests/test_plot.py` & `gwdetchar-2.1.1/gwdetchar/omega/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/overflow.py` & `gwdetchar-2.1.1/gwdetchar/overflow.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/plot.py` & `gwdetchar-2.1.1/gwdetchar/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/saturation/__init__.py` & `gwdetchar-2.1.1/gwdetchar/saturation/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/saturation/__main__.py` & `gwdetchar-2.1.1/gwdetchar/saturation/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/saturation/core.py` & `gwdetchar-2.1.1/gwdetchar/saturation/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/saturation/tests/__init__.py` & `gwdetchar-2.1.1/gwdetchar/saturation/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/saturation/tests/test_saturation.py` & `gwdetchar-2.1.1/gwdetchar/saturation/tests/test_saturation.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/scattering/__init__.py` & `gwdetchar-2.1.1/gwdetchar/scattering/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/scattering/__main__.py` & `gwdetchar-2.1.1/gwdetchar/scattering/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/scattering/core.py` & `gwdetchar-2.1.1/gwdetchar/scattering/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/scattering/plot.py` & `gwdetchar-2.1.1/gwdetchar/scattering/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/scattering/simple.py` & `gwdetchar-2.1.1/gwdetchar/scattering/simple.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/scattering/tests/__init__.py` & `gwdetchar-2.1.1/gwdetchar/scattering/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/scattering/tests/test_core.py` & `gwdetchar-2.1.1/gwdetchar/scattering/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/scattering/tests/test_main.py` & `gwdetchar-2.1.1/gwdetchar/scattering/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/scattering/tests/test_plot.py` & `gwdetchar-2.1.1/gwdetchar/scattering/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/scattering/tests/test_simple.py` & `gwdetchar-2.1.1/gwdetchar/scattering/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/tests/__init__.py` & `gwdetchar-2.1.1/gwdetchar/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/tests/test_cds.py` & `gwdetchar-2.1.1/gwdetchar/tests/test_cds.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/tests/test_cli.py` & `gwdetchar-2.1.1/gwdetchar/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/tests/test_condor.py` & `gwdetchar-2.1.1/gwdetchar/tests/test_condor.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/tests/test_conlog.py` & `gwdetchar-2.1.1/gwdetchar/tests/test_conlog.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/tests/test_const.py` & `gwdetchar-2.1.1/gwdetchar/tests/test_const.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/tests/test_daq.py` & `gwdetchar-2.1.1/gwdetchar/tests/test_daq.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/tests/test_plot.py` & `gwdetchar-2.1.1/gwdetchar/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/tests/test_utils.py` & `gwdetchar-2.1.1/gwdetchar/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar/utils.py` & `gwdetchar-2.1.1/gwdetchar/utils.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar.egg-info/PKG-INFO` & `gwdetchar-2.1.1/gwdetchar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdetchar
-Version: 2.1.0
+Version: 2.1.1
 Summary: A python package for gravitational-wave detector characterisation
 Author-email: Alex Urban <alex.urban@ligo.org>, Duncan Macleod <duncan.macleod@ligo.org>
 Maintainer-email: Evan Goetz <evan.goetz@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://gwdetchar.readthedocs.io
 Project-URL: Source Code, https://github.com/gwdetchar/gwdetchar
 Project-URL: Bug Tracker, https://github.com/gwdetchar/gwdetchar/issues
```

### Comparing `gwdetchar-2.1.0/gwdetchar.egg-info/SOURCES.txt` & `gwdetchar-2.1.1/gwdetchar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/gwdetchar.egg-info/entry_points.txt` & `gwdetchar-2.1.1/gwdetchar.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.0/pyproject.toml` & `gwdetchar-2.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -41,22 +41,22 @@
   "beautifulsoup4",
   "coloredlogs",
   "gwdatafind",
   "gwpy >=3.0.0",
   "gwtrigfind",
   "lalsuite",
   "ligo-segments",
-  "lscsoft-glue >=2.0.0",
   "lxml",
   "MarkupPy >=1.14",
   "matplotlib >=3.1.0",
   "numpy >=1.16",
   "pandas",
   "pycondor",
   "pygments >=2.7.3",
+  "python-ligo-lw",
   "pytz",
   "scikit-learn",
   "scipy >=1.2.0",
 ]
 
 dynamic = ["version"]
 
@@ -128,8 +128,8 @@
 report_level = "SEVERE"
 ignore_languages = [
   "bash",
 ]
 ignore_directives = [
   "autosummary",
   "command-output",
-]
+]
```

