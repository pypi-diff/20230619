# Comparing `tmp/cdflib-1.0.4.tar.gz` & `tmp/cdflib-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdflib-1.0.4.tar", last modified: Tue Jun  6 16:35:05 2023, max compression
+gzip compressed data, was "cdflib-1.0.5.tar", last modified: Mon Jun 19 08:00:11 2023, max compression
```

## Comparing `cdflib-1.0.4.tar` & `cdflib-1.0.5.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.214663 cdflib-1.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.210664 cdflib-1.0.4/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-06 16:34:50.000000 cdflib-1.0.4/.circleci/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-06 16:34:50.000000 cdflib-1.0.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.206665 cdflib-1.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.210664 cdflib-1.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-06 16:34:50.000000 cdflib-1.0.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-06 16:34:50.000000 cdflib-1.0.4/.github/workflows/pypi-build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-06 16:34:50.000000 cdflib-1.0.4/.github/workflows/python-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-06 16:34:50.000000 cdflib-1.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-06 16:34:50.000000 cdflib-1.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-06 16:34:50.000000 cdflib-1.0.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-06 16:34:50.000000 cdflib-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-06 16:34:50.000000 cdflib-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-06 16:35:05.214663 cdflib-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-06 16:34:50.000000 cdflib-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.210664 cdflib-1.0.4/archive/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-06 16:34:50.000000 cdflib-1.0.4/archive/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-06-06 16:34:50.000000 cdflib-1.0.4/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.210664 cdflib-1.0.4/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 16:34:50.000000 cdflib-1.0.4/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-06 16:34:50.000000 cdflib-1.0.4/benchmarks/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.210664 cdflib-1.0.4/cdflib/
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/CDFLeapSeconds.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 16:35:05.000000 cdflib-1.0.4/cdflib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    84171 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/cdfread.py
--rw-r--r--   0 runner    (1001) docker     (123)   104416 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/cdfwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)    65531 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/epochs_astropy.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.210664 cdflib-1.0.4/cdflib/xarray/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38117 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/xarray/cdf_to_xarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    32580 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/xarray/xarray_to_cdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.210664 cdflib-1.0.4/cdflib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-06 16:35:05.000000 cdflib-1.0.4/cdflib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-06 16:35:05.000000 cdflib-1.0.4/cdflib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 16:35:05.000000 cdflib-1.0.4/cdflib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-06 16:35:05.000000 cdflib-1.0.4/cdflib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 16:35:05.000000 cdflib-1.0.4/cdflib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 16:34:50.000000 cdflib-1.0.4/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.210664 cdflib-1.0.4/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.214663 cdflib-1.0.4/doc/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/modules/cdfepoch.rst
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/modules/cdfread.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/modules/cdfwrite.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/modules/dataclasses.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/modules/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/modules/xarray.rst
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-06 16:34:50.000000 cdflib-1.0.4/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-06 16:34:50.000000 cdflib-1.0.4/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-06 16:34:50.000000 cdflib-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-06 16:35:05.214663 cdflib-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.214663 cdflib-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-06 16:34:50.000000 cdflib-1.0.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-06 16:34:50.000000 cdflib-1.0.4/tests/test_astropy_epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-06 16:34:50.000000 cdflib-1.0.4/tests/test_cdfread.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-06 16:34:50.000000 cdflib-1.0.4/tests/test_cdfread_rle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16228 2023-06-06 16:34:50.000000 cdflib-1.0.4/tests/test_cdfwrite.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9647 2023-06-06 16:34:50.000000 cdflib-1.0.4/tests/test_epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17241 2023-06-06 16:34:50.000000 cdflib-1.0.4/tests/test_xarray_reader_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.214663 cdflib-1.0.4/tests/testfiles/
--rw-r--r--   0 runner    (1001) docker     (123)   125566 2023-06-06 16:34:50.000000 cdflib-1.0.4/tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf
--rw-r--r--   0 runner    (1001) docker     (123)    67164 2023-06-06 16:34:50.000000 cdflib-1.0.4/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf
--rw-r--r--   0 runner    (1001) docker     (123)    70003 2023-06-06 16:34:50.000000 cdflib-1.0.4/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-06 16:34:50.000000 cdflib-1.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.726974 cdflib-1.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.706974 cdflib-1.0.5/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-19 07:59:50.000000 cdflib-1.0.5/.circleci/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-19 07:59:50.000000 cdflib-1.0.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.702974 cdflib-1.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.706974 cdflib-1.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-19 07:59:50.000000 cdflib-1.0.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-19 07:59:50.000000 cdflib-1.0.5/.github/workflows/pypi-build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-19 07:59:50.000000 cdflib-1.0.5/.github/workflows/python-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-19 07:59:50.000000 cdflib-1.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-19 07:59:50.000000 cdflib-1.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-19 07:59:50.000000 cdflib-1.0.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 07:59:50.000000 cdflib-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-19 07:59:50.000000 cdflib-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-19 08:00:11.726974 cdflib-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-19 07:59:50.000000 cdflib-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.706974 cdflib-1.0.5/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-19 07:59:50.000000 cdflib-1.0.5/archive/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-06-19 07:59:50.000000 cdflib-1.0.5/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.710974 cdflib-1.0.5/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:59:50.000000 cdflib-1.0.5/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-19 07:59:50.000000 cdflib-1.0.5/benchmarks/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.714974 cdflib-1.0.5/cdflib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/CDFLeapSeconds.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 08:00:11.000000 cdflib-1.0.5/cdflib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84143 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/cdfread.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104416 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/cdfwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65533 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/epochs_astropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.714974 cdflib-1.0.5/cdflib/xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38117 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/xarray/cdf_to_xarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32580 2023-06-19 07:59:50.000000 cdflib-1.0.5/cdflib/xarray/xarray_to_cdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.714974 cdflib-1.0.5/cdflib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-19 08:00:11.000000 cdflib-1.0.5/cdflib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-19 08:00:11.000000 cdflib-1.0.5/cdflib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:00:11.000000 cdflib-1.0.5/cdflib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-19 08:00:11.000000 cdflib-1.0.5/cdflib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 08:00:11.000000 cdflib-1.0.5/cdflib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 07:59:50.000000 cdflib-1.0.5/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.718974 cdflib-1.0.5/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.718974 cdflib-1.0.5/doc/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/modules/cdfepoch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/modules/cdfread.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/modules/cdfwrite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/modules/dataclasses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/modules/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-19 07:59:50.000000 cdflib-1.0.5/doc/modules/xarray.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-19 07:59:50.000000 cdflib-1.0.5/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-19 07:59:50.000000 cdflib-1.0.5/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-19 07:59:50.000000 cdflib-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-19 08:00:11.726974 cdflib-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.722974 cdflib-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-19 07:59:50.000000 cdflib-1.0.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-19 07:59:50.000000 cdflib-1.0.5/tests/test_astropy_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-19 07:59:50.000000 cdflib-1.0.5/tests/test_cdfread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-19 07:59:50.000000 cdflib-1.0.5/tests/test_cdfread_rle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16228 2023-06-19 07:59:50.000000 cdflib-1.0.5/tests/test_cdfwrite.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9647 2023-06-19 07:59:50.000000 cdflib-1.0.5/tests/test_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17241 2023-06-19 07:59:50.000000 cdflib-1.0.5/tests/test_xarray_reader_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:00:11.722974 cdflib-1.0.5/tests/testfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)   125566 2023-06-19 07:59:50.000000 cdflib-1.0.5/tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf
+-rw-r--r--   0 runner    (1001) docker     (123)    67164 2023-06-19 07:59:50.000000 cdflib-1.0.5/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf
+-rw-r--r--   0 runner    (1001) docker     (123)    70003 2023-06-19 07:59:50.000000 cdflib-1.0.5/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-19 07:59:50.000000 cdflib-1.0.5/tox.ini
```

### Comparing `cdflib-1.0.4/.circleci/config.yml` & `cdflib-1.0.5/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/.github/workflows/ci.yml` & `cdflib-1.0.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/.github/workflows/pypi-build.yaml` & `cdflib-1.0.5/.github/workflows/pypi-build.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/.pre-commit-config.yaml` & `cdflib-1.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/.readthedocs.yml` & `cdflib-1.0.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/LICENSE` & `cdflib-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/PKG-INFO` & `cdflib-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdflib
-Version: 1.0.4
+Version: 1.0.5
 Summary: A python CDF reader toolkit
 Home-page: https://github.com/MAVENSDC/cdflib
 Author: MAVEN SDC
 Author-email: mavensdc@lasp.colorado.edu
 Keywords: CDF,maven,lasp,PDS,GSFC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cdflib-1.0.4/README.md` & `cdflib-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/asv.conf.json` & `cdflib-1.0.5/asv.conf.json`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/benchmarks/benchmarks.py` & `cdflib-1.0.5/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/cdflib/CDFLeapSeconds.txt` & `cdflib-1.0.5/cdflib/CDFLeapSeconds.txt`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/cdflib/cdfread.py` & `cdflib-1.0.5/cdflib/cdfread.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         return self
 
     def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
         return
 
     def cdf_info(self) -> CDFInfo:
         """
-        Returns a dictionary that shows the basic CDF information.
+        Returns basic CDF information.
 
         Returns
         -------
         CDFInfo
         """
         varnames = self._get_varnames()
         return CDFInfo(
```

### Comparing `cdflib-1.0.4/cdflib/cdfwrite.py` & `cdflib-1.0.5/cdflib/cdfwrite.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/cdflib/dataclasses.py` & `cdflib-1.0.5/cdflib/dataclasses.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/cdflib/epochs.py` & `cdflib-1.0.5/cdflib/epochs.py`

 * *Files 0% similar despite different names*

```diff
@@ -634,15 +634,15 @@
                 else:
                     nanoSecSinceJ2000 = int(nanoSecSinceJ2000 - CDFepoch.T12hinNanoSecs)
                     nanoSecSinceJ2000 = int(nanoSecSinceJ2000 + t2)
                     nanoSecSinceJ2000 = int(nanoSecSinceJ2000 + CDFepoch.dTinNanoSecs)
 
             nanoSecSinceJ2000s.append(int(nanoSecSinceJ2000))
 
-        return np.array(nanoSecSinceJ2000s)
+        return np.squeeze(nanoSecSinceJ2000s)
 
     @staticmethod
     def _LeapSecondsfromYMD(year: int, month: int, day: int) -> float:
         j = -1
         m = 12 * year + month
         for i, _ in reversed(list(enumerate(CDFepoch.LTS))):
             n = 12 * CDFepoch.LTS[i][0] + CDFepoch.LTS[i][1]
```

### Comparing `cdflib-1.0.4/cdflib/epochs_astropy.py` & `cdflib-1.0.5/cdflib/epochs_astropy.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/cdflib/s3.py` & `cdflib-1.0.5/cdflib/s3.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/cdflib/xarray/cdf_to_xarray.py` & `cdflib-1.0.5/cdflib/xarray/cdf_to_xarray.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/cdflib/xarray/xarray_to_cdf.py` & `cdflib-1.0.5/cdflib/xarray/xarray_to_cdf.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/cdflib.egg-info/PKG-INFO` & `cdflib-1.0.5/cdflib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdflib
-Version: 1.0.4
+Version: 1.0.5
 Summary: A python CDF reader toolkit
 Home-page: https://github.com/MAVENSDC/cdflib
 Author: MAVEN SDC
 Author-email: mavensdc@lasp.colorado.edu
 Keywords: CDF,maven,lasp,PDS,GSFC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cdflib-1.0.4/cdflib.egg-info/SOURCES.txt` & `cdflib-1.0.5/cdflib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/doc/Makefile` & `cdflib-1.0.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/doc/changelog.rst` & `cdflib-1.0.5/doc/changelog.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =========
 Changelog
 =========
 
+1.0.5
+=====
+- Fixed the output of :meth:`cdflib.epochs.CDFepoch.compute_tt2000` to
+  be squeezed if a single input is given.
+- Fixed warnings with numpy 1.25.
+
 1.0.4
 =====
 - Fixed issue where multi-dimensional variables were dropped when converting to xarray.
 - Replaced all print and warning statements with a logger, ``cdflib.logging.logger``.
 
 1.0.3
 =====
```

### Comparing `cdflib-1.0.4/doc/conf.py` & `cdflib-1.0.5/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/doc/index.rst` & `cdflib-1.0.5/doc/index.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/doc/make.bat` & `cdflib-1.0.5/doc/make.bat`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/doc/modules/cdfepoch.rst` & `cdflib-1.0.5/doc/modules/cdfepoch.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/doc/modules/cdfread.rst` & `cdflib-1.0.5/doc/modules/cdfread.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/doc/modules/cdfwrite.rst` & `cdflib-1.0.5/doc/modules/cdfwrite.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/meta.yaml` & `cdflib-1.0.5/meta.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/mypy.ini` & `cdflib-1.0.5/mypy.ini`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/setup.cfg` & `cdflib-1.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/tests/test_astropy_epochs.py` & `cdflib-1.0.5/tests/test_astropy_epochs.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/tests/test_cdfread.py` & `cdflib-1.0.5/tests/test_cdfread.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/tests/test_cdfwrite.py` & `cdflib-1.0.5/tests/test_cdfwrite.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/tests/test_epochs.py` & `cdflib-1.0.5/tests/test_epochs.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/tests/test_xarray_reader_writer.py` & `cdflib-1.0.5/tests/test_xarray_reader_writer.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf` & `cdflib-1.0.5/tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf` & `cdflib-1.0.5/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.4/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf` & `cdflib-1.0.5/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf`

 * *Files identical despite different names*

