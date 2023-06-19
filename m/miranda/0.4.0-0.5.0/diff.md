# Comparing `tmp/miranda-0.4.0.tar.gz` & `tmp/miranda-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miranda-0.4.0.tar", last modified: Thu Mar 30 15:35:25 2023, max compression
+gzip compressed data, was "miranda-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `miranda-0.4.0.tar` & `miranda-0.5.0.tar`

### file list

```diff
@@ -1,103 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:25.754883 miranda-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-30 15:35:16.000000 miranda-0.4.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-03-30 15:35:16.000000 miranda-0.4.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11380 2023-03-30 15:35:16.000000 miranda-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-30 15:35:16.000000 miranda-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-03-30 15:35:25.754883 miranda-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-03-30 15:35:16.000000 miranda-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:25.746883 miranda-0.4.0/miranda/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:25.746883 miranda-0.4.0/miranda/archive/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/archive/_groupings.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/archive/_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:25.750883 miranda-0.4.0/miranda/convert/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/_data_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/_data_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/_reconstruction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:25.750883 miranda-0.4.0/miranda/convert/data/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/data/cmip_ouranos_attrs.json
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/data/deh_cf_attrs.json
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/data/eccc_cf_attrs.json
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/data/eccc_rdrs_cf_attrs.json
--rw-r--r--   0 runner    (1001) docker     (123)    21890 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/data/ecmwf_cf_attrs.json
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/data/ets_grnch_cf_attrs.json
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/data/hq_cf_attrs.json
--rw-r--r--   0 runner    (1001) docker     (123)    13592 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/data/melcc_cf_attrs.json
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/data/nasa_cf_attrs.json
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/data/rvt_raven_attrs.json
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/data/usask_cf_attrs.json
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/deh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/eccc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/eccc_rdrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/ecmwf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/hq.py
--rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/melcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/convert/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:25.750883 miranda-0.4.0/miranda/decode/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/decode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29755 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/decode/_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/decode/_time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:25.750883 miranda-0.4.0/miranda/eccc/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/eccc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/eccc/_homogenized.py
--rw-r--r--   0 runner    (1001) docker     (123)    35248 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/eccc/_raw.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10686 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/eccc/_summaries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/eccc/_support_rvt.py
--rw-r--r--   0 runner    (1001) docker     (123)    34334 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/eccc/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:25.754883 miranda-0.4.0/miranda/eccc/data/
--rw-r--r--   0 runner    (1001) docker     (123)    35391 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/eccc/data/ahccd_gen2_precipitation.csv
--rw-r--r--   0 runner    (1001) docker     (123)    50143 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/eccc/data/ahccd_gen3_temperature.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/eccc/eccc_homogenized_cf_attrs.json
--rw-r--r--   0 runner    (1001) docker     (123)    25849 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/eccc/eccc_obs_cf_attrs.json
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/eccc/eccc_obs_summary_cf_attrs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:25.754883 miranda-0.4.0/miranda/ecmwf/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/ecmwf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14213 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/ecmwf/_era5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/ecmwf/_tigge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:25.754883 miranda-0.4.0/miranda/gis/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/gis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/gis/_domains.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:25.754883 miranda-0.4.0/miranda/io/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/io/_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/io/_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/io/_rechunk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:25.754883 miranda-0.4.0/miranda/io/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/io/data/chunk_configurations.json
--rw-r--r--   0 runner    (1001) docker     (123)     8214 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:25.754883 miranda-0.4.0/miranda/ncar/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/ncar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/ncar/_aws_cordex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:25.754883 miranda-0.4.0/miranda/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/remote/archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/remote/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/remote/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/remote/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:25.754883 miranda-0.4.0/miranda/structure/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15826 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/structure/_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:25.754883 miranda-0.4.0/miranda/structure/data/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/structure/data/ouranos_schema.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    11795 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-03-30 15:35:16.000000 miranda-0.4.0/miranda/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:25.746883 miranda-0.4.0/miranda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-03-30 15:35:25.000000 miranda-0.4.0/miranda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-03-30 15:35:25.000000 miranda-0.4.0/miranda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 15:35:25.000000 miranda-0.4.0/miranda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 15:35:25.000000 miranda-0.4.0/miranda.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-30 15:35:25.000000 miranda-0.4.0/miranda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-30 15:35:25.000000 miranda-0.4.0/miranda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-30 15:35:16.000000 miranda-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-30 15:35:16.000000 miranda-0.4.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-30 15:35:16.000000 miranda-0.4.0/requirements_remote.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-30 15:35:25.754883 miranda-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-03-30 15:35:16.000000 miranda-0.4.0/setup.py
+-rw-r--r--   0        0        0      667 2023-06-19 15:19:39.732955 miranda-0.5.0/AUTHORS.rst
+-rw-r--r--   0        0        0     3344 2023-06-19 15:19:39.732955 miranda-0.5.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     5112 2023-06-19 15:19:39.732955 miranda-0.5.0/HISTORY.rst
+-rw-r--r--   0        0        0    11380 2023-06-19 15:19:39.732955 miranda-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1806 2023-06-19 15:19:39.732955 miranda-0.5.0/Makefile
+-rw-r--r--   0        0        0     3589 2023-06-19 15:19:39.732955 miranda-0.5.0/README.rst
+-rw-r--r--   0        0        0     6778 2023-06-19 15:19:39.732955 miranda-0.5.0/docs/Makefile
+-rw-r--r--   0        0        0    11485 2023-06-19 15:19:39.732955 miranda-0.5.0/docs/_static/images/miranda-logo-small.png
+-rw-r--r--   0        0        0    16857 2023-06-19 15:19:39.732955 miranda-0.5.0/docs/_static/images/miranda-logo.png
+-rw-r--r--   0        0        0       28 2023-06-19 15:19:39.732955 miranda-0.5.0/docs/authors.rst
+-rw-r--r--   0        0        0     9928 2023-06-19 15:19:39.732955 miranda-0.5.0/docs/conf.py
+-rw-r--r--   0        0        0       33 2023-06-19 15:19:39.732955 miranda-0.5.0/docs/contributing.rst
+-rw-r--r--   0        0        0       28 2023-06-19 15:19:39.732955 miranda-0.5.0/docs/history.rst
+-rw-r--r--   0        0        0      646 2023-06-19 15:19:39.732955 miranda-0.5.0/docs/index.rst
+-rw-r--r--   0        0        0     1755 2023-06-19 15:19:39.732955 miranda-0.5.0/docs/installation.rst
+-rw-r--r--   0        0        0       63 2023-06-19 15:19:39.732955 miranda-0.5.0/docs/license.rst
+-rw-r--r--   0        0        0     6467 2023-06-19 15:19:39.732955 miranda-0.5.0/docs/make.bat
+-rw-r--r--   0        0        0       66 2023-06-19 15:19:39.732955 miranda-0.5.0/docs/usage.rst
+-rw-r--r--   0        0        0      669 2023-06-19 15:19:39.732955 miranda-0.5.0/environment.yml
+-rw-r--r--   0        0        0      933 2023-06-19 15:19:39.732955 miranda-0.5.0/miranda/__init__.py
+-rw-r--r--   0        0        0      110 2023-06-19 15:19:39.732955 miranda-0.5.0/miranda/archive/__init__.py
+-rw-r--r--   0        0        0     4754 2023-06-19 15:19:39.732955 miranda-0.5.0/miranda/archive/_groupings.py
+-rw-r--r--   0        0        0     1172 2023-06-19 15:19:39.732955 miranda-0.5.0/miranda/archive/_selection.py
+-rw-r--r--   0        0        0      243 2023-06-19 15:19:39.732955 miranda-0.5.0/miranda/convert/__init__.py
+-rw-r--r--   0        0        0     3789 2023-06-19 15:19:39.732955 miranda-0.5.0/miranda/convert/_aggregation.py
+-rw-r--r--   0        0        0    35149 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/_data_corrections.py
+-rw-r--r--   0        0        0     9728 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/_data_definitions.py
+-rw-r--r--   0        0        0    10517 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/_reconstruction.py
+-rw-r--r--   0        0        0      727 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/data/cmip_ouranos_attrs.json
+-rw-r--r--   0        0        0      542 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/data/deh_cf_attrs.json
+-rw-r--r--   0        0        0      835 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/data/eccc_cf_attrs.json
+-rw-r--r--   0        0        0     2852 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/data/eccc_rdrs_cf_attrs.json
+-rw-r--r--   0        0        0    23179 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/data/ecmwf_cf_attrs.json
+-rw-r--r--   0        0        0     4463 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/data/emdna_cf_attrs.json
+-rw-r--r--   0        0        0      920 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/data/espo-g6-e5l_attrs.json
+-rw-r--r--   0        0        0      918 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/data/espo-g6-r2_attrs.json
+-rw-r--r--   0        0        0     2828 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/data/ets_grnch_cf_attrs.json
+-rw-r--r--   0        0        0     3705 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/data/hq_cf_attrs.json
+-rw-r--r--   0        0        0    13592 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/data/melcc_cf_attrs.json
+-rw-r--r--   0        0        0     4333 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/data/nasa_cf_attrs.json
+-rw-r--r--   0        0        0      521 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/data/nex-gddp-cmip6_attrs.json
+-rw-r--r--   0        0        0      615 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/data/rvt_raven_attrs.json
+-rw-r--r--   0        0        0     3003 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/data/usask_cf_attrs.json
+-rw-r--r--   0        0        0     3936 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/deh.py
+-rw-r--r--   0        0        0     2239 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/eccc.py
+-rw-r--r--   0        0        0     7070 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/eccc_rdrs.py
+-rw-r--r--   0        0        0     2346 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/ecmwf.py
+-rw-r--r--   0        0        0     5339 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/hq.py
+-rw-r--r--   0        0        0    21154 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/melcc.py
+-rw-r--r--   0        0        0     4989 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/convert/utils.py
+-rw-r--r--   0        0        0     3958 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/cv.py
+-rw-r--r--   0        0        0     4411 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/data.py
+-rw-r--r--   0        0        0       81 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/decode/__init__.py
+-rw-r--r--   0        0        0    33955 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/decode/_decoder.py
+-rw-r--r--   0        0        0     2223 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/decode/_time.py
+-rw-r--r--   0        0        0      185 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/eccc/__init__.py
+-rw-r--r--   0        0        0     9672 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/eccc/_homogenized.py
+-rw-r--r--   0        0        0    35058 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/eccc/_raw.py
+-rwxr-xr-x   0        0        0    10898 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/eccc/_summaries.py
+-rw-r--r--   0        0        0     2549 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/eccc/_support_rvt.py
+-rw-r--r--   0        0        0    34323 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/eccc/_utils.py
+-rw-r--r--   0        0        0    35391 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/eccc/data/ahccd_gen2_precipitation.csv
+-rw-r--r--   0        0        0    50143 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/eccc/data/ahccd_gen3_temperature.csv
+-rw-r--r--   0        0        0     4165 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/eccc/eccc_homogenized_cf_attrs.json
+-rw-r--r--   0        0        0    25849 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/eccc/eccc_obs_cf_attrs.json
+-rw-r--r--   0        0        0     5792 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/eccc/eccc_obs_summary_cf_attrs.json
+-rw-r--r--   0        0        0      108 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/ecmwf/__init__.py
+-rw-r--r--   0        0        0    14198 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/ecmwf/_era5.py
+-rw-r--r--   0        0        0     5142 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/ecmwf/_tigge.py
+-rw-r--r--   0        0        0       89 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/gis/__init__.py
+-rw-r--r--   0        0        0     4209 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/gis/_domains.py
+-rw-r--r--   0        0        0      152 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/io/__init__.py
+-rw-r--r--   0        0        0     3195 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/io/_input.py
+-rw-r--r--   0        0        0    11213 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/io/_output.py
+-rw-r--r--   0        0        0     9541 2023-06-19 15:19:39.736955 miranda-0.5.0/miranda/io/_rechunk.py
+-rw-r--r--   0        0        0     1238 2023-06-19 15:19:39.740955 miranda-0.5.0/miranda/io/data/ouranos_chunk_config.json
+-rw-r--r--   0        0        0      682 2023-06-19 15:19:39.740955 miranda-0.5.0/miranda/io/data/ouranos_name_config.json
+-rw-r--r--   0        0        0    10230 2023-06-19 15:19:39.740955 miranda-0.5.0/miranda/io/utils.py
+-rw-r--r--   0        0        0       90 2023-06-19 15:19:39.740955 miranda-0.5.0/miranda/ncar/__init__.py
+-rw-r--r--   0        0        0     7354 2023-06-19 15:19:39.740955 miranda-0.5.0/miranda/ncar/_aws_cordex.py
+-rw-r--r--   0        0        0      156 2023-06-19 15:19:39.740955 miranda-0.5.0/miranda/remote/__init__.py
+-rw-r--r--   0        0        0     5710 2023-06-19 15:19:39.740955 miranda-0.5.0/miranda/remote/archiver.py
+-rw-r--r--   0        0        0     2746 2023-06-19 15:19:39.740955 miranda-0.5.0/miranda/remote/connect.py
+-rw-r--r--   0        0        0     4835 2023-06-19 15:19:39.740955 miranda-0.5.0/miranda/remote/ops.py
+-rw-r--r--   0        0        0     6952 2023-06-19 15:19:39.740955 miranda-0.5.0/miranda/remote/remove.py
+-rw-r--r--   0        0        0     1749 2023-06-19 15:19:39.740955 miranda-0.5.0/miranda/scripting.py
+-rw-r--r--   0        0        0    10545 2023-06-19 15:19:39.740955 miranda-0.5.0/miranda/storage.py
+-rw-r--r--   0        0        0       91 2023-06-19 15:19:39.740955 miranda-0.5.0/miranda/structure/__init__.py
+-rw-r--r--   0        0        0    15870 2023-06-19 15:19:39.740955 miranda-0.5.0/miranda/structure/_structure.py
+-rw-r--r--   0        0        0      963 2023-06-19 15:19:39.740955 miranda-0.5.0/miranda/structure/data/ouranos_schema.yml
+-rw-r--r--   0        0        0     5282 2023-06-19 15:19:39.740955 miranda-0.5.0/miranda/units.py
+-rw-r--r--   0        0        0    11905 2023-06-19 15:19:39.740955 miranda-0.5.0/miranda/utils.py
+-rw-r--r--   0        0        0     5410 2023-06-19 15:19:39.740955 miranda-0.5.0/miranda/validators.py
+-rw-r--r--   0        0        0     3074 2023-06-19 15:19:39.740955 miranda-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       96 2023-06-19 15:19:39.740955 miranda-0.5.0/requirements_remote.txt
+-rw-r--r--   0        0        0     1086 2023-06-19 15:19:39.740955 miranda-0.5.0/setup.cfg
+-rw-r--r--   0        0        0      669 2023-06-19 15:19:39.740955 miranda-0.5.0/templates/aws_cordex_download.py
+-rw-r--r--   0        0        0      399 2023-06-19 15:19:39.740955 miranda-0.5.0/templates/convert_reanalysis.py
+-rw-r--r--   0        0        0      870 2023-06-19 15:19:39.740955 miranda-0.5.0/templates/eccc_ahccd_conversion.py
+-rw-r--r--   0        0        0     1471 2023-06-19 15:19:39.740955 miranda-0.5.0/templates/eccc_raw_daily_conversion.py
+-rw-r--r--   0        0        0     1674 2023-06-19 15:19:39.740955 miranda-0.5.0/templates/eccc_raw_hourly_conversion.py
+-rw-r--r--   0        0        0     1810 2023-06-19 15:19:39.740955 miranda-0.5.0/templates/eccc_rdrs_processing.py
+-rw-r--r--   0        0        0      287 2023-06-19 15:19:39.740955 miranda-0.5.0/templates/eccc_summary_daily_conversion.py
+-rw-r--r--   0        0        0     1301 2023-06-19 15:19:39.740955 miranda-0.5.0/templates/ecmwf_download.py
+-rw-r--r--   0        0        0     1948 2023-06-19 15:19:39.740955 miranda-0.5.0/templates/emdna_processing.py
+-rw-r--r--   0        0        0      552 2023-06-19 15:19:39.740955 miranda-0.5.0/templates/era5-land_reanalysis_processing.py
+-rw-r--r--   0        0        0     2217 2023-06-19 15:19:39.740955 miranda-0.5.0/templates/espo-g6.py
+-rw-r--r--   0        0        0      828 2023-06-19 15:19:39.740955 miranda-0.5.0/templates/nasa_nex-gddp-cmip6_processing.py
+-rw-r--r--   0        0        0     1171 2023-06-19 15:19:39.740955 miranda-0.5.0/templates/rechunk_reanalysis.py
+-rw-r--r--   0        0        0      454 2023-06-19 15:19:39.740955 miranda-0.5.0/templates/restructure_datasets.py
+-rw-r--r--   0        0        0      282 2023-06-19 15:19:39.740955 miranda-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0   588724 2023-06-19 15:19:39.744955 miranda-0.5.0/tests/data/cmip5/tmax.cur.nc
+-rw-r--r--   0        0        0   734820 2023-06-19 15:19:39.748955 miranda-0.5.0/tests/data/cmip5/tmax.fut.nc
+-rw-r--r--   0        0        0   587204 2023-06-19 15:19:39.752956 miranda-0.5.0/tests/data/cmip5/tmax.obs.nc
+-rw-r--r--   0        0        0     1345 2023-06-19 15:19:39.752956 miranda-0.5.0/tests/test_connect.py
+-rwxr-xr-x   0        0        0     1490 2023-06-19 15:19:39.752956 miranda-0.5.0/tests/test_miranda.py
+-rw-r--r--   0        0        0     3543 2023-06-19 15:19:39.752956 miranda-0.5.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1134 2023-06-19 15:19:39.752956 miranda-0.5.0/tox.ini
+-rw-r--r--   0        0        0     6585 1970-01-01 00:00:00.000000 miranda-0.5.0/PKG-INFO
```

### Comparing `miranda-0.4.0/AUTHORS.rst` & `miranda-0.5.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `miranda-0.4.0/HISTORY.rst` & `miranda-0.5.0/HISTORY.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,34 @@
 .. :changelog:
 
 =======
 History
 =======
 
+v0.5.0 (2023-06-19)
+-------------------
+Contributors to this version: Juliette Lavoie (:user: `juliettelavoie`), Trevor James Smith (:user:`Zeitsperre`).
+
+New features
+^^^^^^^^^^^^
+* Added support for collecting and converting `ptype` ECMWF ERA5 variable.
+* A new ``"_frequency": true`` toggle for returning the output frequency of converted data.
+* Added a new JSON template for NEX-GDDP-CMIP6 datasets.
+* `miranda` is now `PEP 517 <https://peps.python.org/pep-0517/>`_ and `PEP 621 <https://peps.python.org/pep-0621/>`_ compliant, using the `flit <https://flit.pypa.io/en/stable/>`_ backend.
+
+Internal changes
+^^^^^^^^^^^^^^^^
+* Various fixes to existing docstrings.
+* Time frequency checks are more resilient when converting Monthly time-step data.
+* Masking and regridding of datasets when running ``convert_dataset`` is now optional or automatic.
+* Updated templates to newest API.
+* Created a `gis` recipe for exclusively installing GIS libraries.
+* Removed many unneeded dependencies, cleaned up Makefile.
+* All public-facing functions now contain at least a minimal docstring for documentation generation.
+
 v0.4.0 (2023-03-30)
 -------------------
 Contributors to this version: Trevor James Smith (:user:`Zeitsperre`), Pascal Bourgault (:user:`aulemahal`), Travis Logan (:user:`tlogan2000`).
 
 New features
 ^^^^^^^^^^^^
 * Improvements have been made to the development documentation; Project URLs, ReadTheDocs theming, and other quality of life changes.
```

### Comparing `miranda-0.4.0/LICENSE` & `miranda-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `miranda-0.4.0/README.rst` & `miranda-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `miranda-0.4.0/miranda/__init__.py` & `miranda-0.5.0/miranda/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
+from __future__ import annotations
 
 __author__ = "Trevor James Smith"
 __email__ = "smith.trevorj@ouranos.ca"
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 
-from . import (  # convert,
+from . import (
     archive,
     convert,
     cv,
     decode,
     io,
     scripting,
     structure,
```

### Comparing `miranda-0.4.0/miranda/archive/_groupings.py` & `miranda-0.5.0/miranda/archive/_groupings.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from __future__ import annotations
+
 import logging
 import re
 from logging.config import dictConfig
 from pathlib import Path
 from types import GeneratorType
-from typing import Dict, List, Union
+from typing import Dict, List
 
 from miranda.scripting import LOGGING_CONFIG
 from miranda.storage import report_file_size
 
 dictConfig(LOGGING_CONFIG)
 Nested_List = List[List[Path]]
 PathDict = Dict[str, List[Path]]
@@ -20,29 +22,29 @@
     "group_by_length",
     "group_by_size",
     "group_by_subdirectories",
 ]
 
 
 def group_by_length(
-    files: Union[GeneratorType, List[Union[str, Path]]],
+    files: GeneratorType | list[str | Path],
     size: int = 10,
     sort: bool = False,
-) -> List[List[Path]]:
+) -> list[list[Path]]:
     """Group files by an arbitrary number of file entries.
 
     Parameters
     ----------
-    files: Union[GeneratorType, List[Union[str, Path]]]
+    files: GeneratorType or list of str or pathlib.Path
     size: int
     sort: bool
 
     Returns
     -------
-    List[List[Path]]
+    list[list[pathlib.Path]]
     """
     logging.info(f"Creating groups of {size} files")
     if sort:
         files = [Path(f) for f in files]
         files.sort()
     grouped_list = list()
     group = list()
@@ -57,25 +59,25 @@
     else:
         grouped_list.append(group.copy())
     logging.info(f"Divided files into {len(grouped_list)} groups.")
     return grouped_list
 
 
 def group_by_deciphered_date(
-    files: Union[GeneratorType, List[Union[str, Path]]]
-) -> Dict[str, List[Path]]:
+    files: GeneratorType | list[str | Path],
+) -> dict[str, list[Path]]:
     """Find a common date and groups files based on year and month.
 
     Parameters
     ----------
-    files: Union[GeneratorType, List[Union[str, Path]]]
+    files: GeneratorType or list of str or pathlib.Path
 
     Returns
     -------
-    Dict[str, List[Path]]
+    dict[str, list[pathlib.Path]]
     """
     logging.warning("This function doesn't work well with multi-thread processing!")
     logging.info("Creating files from deciphered dates.")
 
     year_month_day = re.compile(
         r"(?P<year>\d{4})-?(?P<month>\d{2})-?(?P<day>\d{2})?.*\.(?P<suffix>nc|zarr)$"
     )
@@ -109,28 +111,27 @@
         )
     else:
         logging.info("No matches for dates found. Grouping aborted.")
     return dict(data=files)
 
 
 def group_by_size(
-    files: Union[GeneratorType, List[Union[str, Path]]], size: int = 10 * GiB
-) -> List[List[Path]]:
+    files: GeneratorType | list[str | Path], size: int = 10 * GiB
+) -> list[list[Path]]:
     """Group files up until a desired size and save it as a grouping within a list.
 
     Parameters
     ----------
-    files: Union[GeneratorType, List[Union[str, Path]]]
-    size: int
+    files : GeneratorType or list of str or pathlib.Path
+    size : int
 
     Returns
     -------
-    List[List[Path]]
+    list[list[pathlib.Path]]
     """
-
     logging.info(
         f"Creating groups of files based on size not exceeding: {report_file_size(size)}."
     )
 
     files = [Path(f) for f in files]
     files.sort()
     grouped_list = list()
@@ -148,27 +149,26 @@
         logging.info("The final group is empty. Skipping this set...")
     else:
         grouped_list.append(group.copy())
     return grouped_list
 
 
 def group_by_subdirectories(
-    files: Union[GeneratorType, List[Union[str, Path]]], within: Union[str, Path] = None
-) -> Dict[str, List[Path]]:
-    """
-    This function will group files based on the parent folder that they are located within.
+    files: GeneratorType | list[str | Path], within: str | Path = None
+) -> dict[str, list[Path]]:
+    """Group files based on the parent folder that they are located within.
 
     Parameters
     ----------
-    files: Union[GeneratorType, List[Union[str, Path]]]
-    within: Union[str, Path]
+    files : GeneratorType or list of str or pathlib.Path
+    within : str or pathlib.Path
 
     Returns
     -------
-    Dict[str, List[Path]]
+    dict[str, list[pathlib.Path]]
     """
     if not within:
         within = Path.cwd()
 
     files = [Path(f) for f in files]
     files.sort()
     groups = dict()
```

### Comparing `miranda-0.4.0/miranda/archive/_selection.py` & `miranda-0.5.0/miranda/archive/_selection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,53 @@
+from __future__ import annotations
+
 import logging
-from datetime import date
+from datetime import datetime
 from logging import config
 from pathlib import Path
-from typing import List, Union
 
 from miranda.io import find_filepaths
 from miranda.io.utils import creation_date
 from miranda.scripting import LOGGING_CONFIG
 
 __all__ = ["select_by_date_modified"]
 
 logging.config.dictConfig(LOGGING_CONFIG)
 
 
 def select_by_date_modified(
-    source: Union[Path, str],
-    year: int,
-    month: int,
-    day: int,
-    pattern: str = None,
-    datetime: date = None,
-) -> List:
-    """
+    source: str | Path,
+    year: int | None,
+    month: int | None,
+    day: int | None,
+    *,
+    suffixes: str = "nc",
+    date: datetime,
+) -> list[Path]:
+    """Select files by the date on which they were last modified.
 
     Parameters
     ----------
-    source
-    year
-    month
-    day
-    pattern
-    datetime
+    source : str or Path
+    year : int
+    month : int
+    day : int
+    suffixes : str
+    date : datetime.date
 
     Returns
     -------
-
+    list of Path
     """
+    if date:
+        date_selected = date
+    else:
+        date_selected = datetime(year, month, day)
 
-    date_selected = date(year, month, day) or datetime
-
-    files = find_filepaths(source, file_suffixes=pattern)
+    files = find_filepaths(source, file_suffixes=suffixes)
 
     selected_files = list()
     for file in files:
         if creation_date(file) == date_selected:
             logging.info(f"Selecting {file}.")
             selected_files.append(file)
```

### Comparing `miranda-0.4.0/miranda/convert/_aggregation.py` & `miranda-0.5.0/miranda/convert/_aggregation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+"""Aggregation module."""
+from __future__ import annotations
+
 import logging.config
-from typing import Dict, Set
 
 import xarray as xr
-import xclim.core.options
 from xclim.indices import tas
 
 from miranda.scripting import LOGGING_CONFIG
 from miranda.units import get_time_frequency
 
 logging.config.dictConfig(LOGGING_CONFIG)
 
@@ -16,15 +17,26 @@
 _resampling_keys = dict()
 _resampling_keys["hour"] = "H"
 _resampling_keys["day"] = "D"
 _resampling_keys["month"] = "M"
 _resampling_keys["year"] = "A"
 
 
-def aggregations_possible(ds: xr.Dataset, freq: str = "day") -> Dict[str, Set[str]]:
+def aggregations_possible(ds: xr.Dataset, freq: str = "day") -> dict[str, set[str]]:
+    """Determine which aggregations are possible based on variables within a dataset.
+
+    Parameters
+    ----------
+    ds : xarray.Dataset
+    freq : str
+
+    Returns
+    -------
+    dict[str, set[str]]
+    """
     logging.info("Determining potential upscaled climate variables.")
 
     offset, meaning = get_time_frequency(ds, minimum_continuous_period="1h")
 
     aggregation_legend = dict()
     for v in ["tas", "tdps"]:
         if freq == meaning:
@@ -55,15 +67,26 @@
             "swe",
         ]:
             aggregation_legend[variable] = {"mean"}
 
     return aggregation_legend
 
 
-def aggregate(ds, freq: str = "day") -> Dict[str, xr.Dataset]:
+def aggregate(ds: xr.Dataset, freq: str = "day") -> dict[str, xr.Dataset]:
+    """
+
+    Parameters
+    ----------
+    ds : xarray.Dataset
+    freq : str
+
+    Returns
+    -------
+    dict[str, xarray.Dataset]
+    """
     mappings = aggregations_possible(ds)
 
     try:
         xarray_agg = _resampling_keys[freq]
     except KeyError:
         xarray_agg = freq
```

### Comparing `miranda-0.4.0/miranda/convert/_data_corrections.py` & `miranda-0.5.0/miranda/convert/_data_corrections.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+from __future__ import annotations
+
 import datetime
 import json
 import logging.config
 import os
+import warnings
+from collections.abc import Iterator, Sequence
 from functools import partial
 from pathlib import Path
-from typing import Callable, Dict, Iterator, List, Optional, Sequence, Union
+from typing import Any, Callable
 
 import numpy as np
 import xarray as xr
 import xclim.core.units
-from clisops.core.subset import subset_bbox
 from xarray.coding import times
 from xclim.core import units
 from xclim.core.calendar import parse_offset
 
 from miranda import __version__ as __miranda_version__
 from miranda.gis import subset_domain
 from miranda.scripting import LOGGING_CONFIG
@@ -32,16 +35,26 @@
     "load_json_data_mappings",
     "metadata_conversion",
     "threshold_mask",
     "variable_conversion",
 ]
 
 
-def load_json_data_mappings(project: str) -> dict:
-    data_folder = Path(__file__).parent / "data"
+def load_json_data_mappings(project: str) -> dict[str, Any]:
+    """Load JSON mappings for supported dataset conversions.
+
+    Parameters
+    ----------
+    project : str
+
+    Returns
+    -------
+    dict[str, Any]
+    """
+    data_folder = Path(__file__).resolve().parent / "data"
 
     if project.startswith("era5"):
         metadata_definition = json.load(open(data_folder / "ecmwf_cf_attrs.json"))
     elif project in ["rdrs-v21"]:
         metadata_definition = json.load(open(data_folder / "eccc_rdrs_cf_attrs.json"))
     elif project in ["agcfsr", "agmerra2"]:  # This should handle the AG versions:
         metadata_definition = json.load(open(data_folder / "nasa_cf_attrs.json"))
@@ -53,14 +66,22 @@
         raise NotImplementedError()
     elif project == "wfdei-gem-capa":
         metadata_definition = json.load(open(data_folder / "usask_cf_attrs.json"))
     elif project.startswith("melcc"):
         metadata_definition = json.load(open(data_folder / "melcc_cf_attrs.json"))
     elif project.startswith("ec"):
         metadata_definition = json.load(open(data_folder / "eccc_cf_attrs.json"))
+    elif project in ["NEX-GDDP-CMIP6"]:
+        metadata_definition = json.load(open(data_folder / "nex-gddp-cmip6_attrs.json"))
+    elif project in ["ESPO-G6-R2"]:
+        metadata_definition = json.load(open(data_folder / "espo-g6-r2_attrs.json"))
+    elif project in ["ESPO-G6-E5L"]:
+        metadata_definition = json.load(open(data_folder / "espo-g6-e5l_attrs.json"))
+    elif project in ["EMDNA"]:
+        metadata_definition = json.load(open(data_folder / "emdna_cf_attrs.json"))
     else:
         raise NotImplementedError()
 
     return metadata_definition
 
 
 def _get_section_entry_key(meta, entry, var, key, project):
@@ -77,17 +98,15 @@
 
 def _iter_entry_key(ds, meta, entry, key, project):
     for vv in set(ds.data_vars).intersection(meta[entry]):
         val = _get_section_entry_key(meta, entry, vv, key, project)
         yield vv, val
 
 
-def _simple_fix_dims(
-    d: Union[xr.Dataset, xr.DataArray]
-) -> Union[xr.Dataset, xr.DataArray]:
+def _simple_fix_dims(d: xr.Dataset | xr.DataArray) -> xr.Dataset | xr.DataArray:
     """Adjust dimensions found in a file so that it can be used for regridding purposes."""
     if "lon" not in d.dims or "lat" not in d.dims:
         dim_rename = dict()
         for dim in d.dims:
             if str(dim).lower().startswith("lon"):
                 dim_rename[str(dim)] = "lon"
             if str(dim).lower().startswith("lat"):
@@ -101,83 +120,97 @@
     if "time" in d.dims:
         d = d.isel(time=0, drop=True)
 
     return d
 
 
 def conservative_regrid(
-    ds: Union[xr.DataArray, xr.Dataset], ref_grid: Union[xr.DataArray, xr.Dataset]
-) -> Union[xr.DataArray, xr.Dataset]:
+    ds: xr.DataArray | xr.Dataset, ref_grid: xr.DataArray | xr.Dataset
+) -> xr.DataArray | xr.Dataset:
     """Perform a conservative_normed regridding"""
     try:
-        import xesmf as xe
+        import xesmf as xe  # noqa
     except ModuleNotFoundError:
         raise ModuleNotFoundError(
             "This function requires the `xesmf` library which is not installed. "
             "Regridding step will be skipped."
         )
 
     ref_grid = _simple_fix_dims(ref_grid)
     method = "conservative_normed"
 
+    logging.info(
+        f"Performing regridding and masking with `xesmf` using method: {method}."
+    )
+
     regridder = xe.Regridder(ds, ref_grid, method, periodic=False)
     ds = regridder(ds)
 
     ds.attrs["history"] = (
         f"{datetime.datetime.now()}:"
         f"Regridded dataset using xesmf with method: {method}. "
         f"{ds.attrs.get('history')}".strip()
     )
     return ds
 
 
 def threshold_mask(
-    ds: Union[xr.Dataset, xr.DataArray],
+    ds: xr.Dataset | xr.DataArray,
     *,
-    mask: Union[xr.Dataset, xr.DataArray],
-    mask_cutoff: Union[float, bool] = False,
-) -> Union[xr.Dataset, xr.DataArray]:
+    mask: xr.Dataset | xr.DataArray,
+    mask_cutoff: float | bool = False,
+) -> xr.Dataset | xr.DataArray:
     """Land-Sea mask operations.
 
     Parameters
     ----------
-    ds : Union[xr.Dataset, str, os.PathLike]
-    mask : Union[xr.Dataset, xr.DataArray]
+    ds : xr.Dataset or str or os.PathLike
+    mask : xr.Dataset or xr.DataArray
     mask_cutoff : float or bool
 
     Returns
     -------
-    Union[xr.Dataset, xr.DataArray]
+    xr.Dataset or xr.DataArray
     """
     mask = _simple_fix_dims(mask)
 
     if isinstance(mask, xr.Dataset):
         if len(mask.data_vars) == 1:
-            mask_variable = list(mask.data_vars)[0].name
+            mask_variable = list(mask.data_vars)[0]
             mask = mask[mask_variable]
         else:
             raise ValueError(
                 "More than one data variable found in land-sea mask. Supply a DataArray instead."
             )
     else:
         mask_variable = mask.name
 
-    log_msg = f"Masking dataset with {mask_variable}."
-    if mask_cutoff:
-        log_msg = f"{log_msg.strip('.')} at `{mask_cutoff}` cutoff value."
-    logging.info(log_msg)
+    try:
+        from clisops.core import subset_bbox  # noqa
+
+        log_msg = f"Masking dataset with {mask_variable}."
+        if mask_cutoff:
+            log_msg = f"{log_msg.strip('.')} at `{mask_cutoff}` cutoff value."
+        logging.info(log_msg)
 
-    lon_bounds = np.array([ds.lon.min(), ds.lon.max()])
-    lat_bounds = np.array([ds.lat.min(), ds.lat.max()])
+        lon_bounds = np.array([ds.lon.min(), ds.lon.max()])
+        lat_bounds = np.array([ds.lat.min(), ds.lat.max()])
 
-    mask_subset = subset_bbox(
-        mask,
-        lon_bnds=lon_bounds,
-        lat_bnds=lat_bounds,
-    ).load()
+        mask_subset = subset_bbox(
+            mask,
+            lon_bnds=lon_bounds,
+            lat_bnds=lat_bounds,
+        ).load()
+    except ModuleNotFoundError:
+        log_msg = (
+            "This function requires the `clisops` library which is not installed. "
+            "subsetting step will be skipped."
+        )
+        warnings.warn(log_msg)
+        mask_subset = mask.load()
 
     if mask_subset.dtype == bool:
         if mask_cutoff:
             logging.warning("Mask value cutoff set for boolean mask. Ignoring.")
         mask_subset = mask_subset.where(mask)
     else:
         mask_subset = mask_subset.where(mask >= mask_cutoff)
@@ -225,27 +258,51 @@
     )
     d.attrs.update(dict(history=history))
 
     return d
 
 
 def correct_var_names(d: xr.Dataset, split: str = "_", location: int = 0) -> xr.Dataset:
+    """
+
+    Parameters
+    ----------
+    d : xarray.Dataset
+    split : str
+    location : int
+
+    Returns
+    -------
+    xarray.Dataset
+    """
     filename = d.encoding["source"]
     new_name = Path(filename).stem.split(split)[location]
     old_name = list(d.data_vars.keys())[0]
 
     prev_history = d.attrs.get("history", "")
     history = f"Variable renamed in preprocessing step ({old_name}: {new_name}). {prev_history}"
     d.attrs.update(dict(history=history))
 
     return d.rename({old_name: new_name})
 
 
-def preprocessing_corrections(ds: xr.Dataset, *, project: str) -> xr.Dataset:
-    def _preprocess_correct(d: xr.Dataset, *, ops: List[partial]) -> xr.Dataset:
+def preprocessing_corrections(ds: xr.Dataset, project: str) -> xr.Dataset:
+    """Corrections function dispatcher to ensure minimal dataset validity on open.
+
+    Parameters
+    ----------
+    ds : xarray.Dataset
+    project : str
+
+    Returns
+    -------
+    xarray.Dataset
+    """
+
+    def _preprocess_correct(d: xr.Dataset, *, ops: list[partial]) -> xr.Dataset:
         for correction in ops:
             d = correction(d)
         return d
 
     correction_fields = load_json_data_mappings(project).get("_preprocess")
     if correction_fields:
         preprocess_ops = []
@@ -260,30 +317,30 @@
                 )
         if preprocess_ops:
             corrector = partial(_preprocess_correct, ops=preprocess_ops)
             return corrector(ds)
     return ds
 
 
-def _correct_units_names(d: xr.Dataset, p: str, m: Dict) -> xr.Dataset:
+def _correct_units_names(d: xr.Dataset, p: str, m: dict) -> xr.Dataset:
     key = "_corrected_units"
     for var, val in _iter_entry_key(d, m, "variables", key, p):
         if val:
             d[var].attrs["units"] = val
 
     # FIXME: This is no longer relevant. Performed under dimension conversion step.
     val_time = _get_section_entry_key(m, "variables", "time", key, p)
     if val_time:
         d["time"].attrs["units"] = val_time
 
     return d
 
 
 # for de-accumulation or conversion to flux
-def _transform(d: xr.Dataset, p: str, m: Dict) -> xr.Dataset:
+def _transform(d: xr.Dataset, p: str, m: dict) -> xr.Dataset:
     key = "_transformation"
     d_out = xr.Dataset(coords=d.coords, attrs=d.attrs)
     converted = []
     offset, offset_meaning = None, None
 
     time_freq = dict()
     expected_period = _get_section_entry_key(
@@ -312,14 +369,15 @@
                         getattr(d[vv].time.dt, offset_meaning) == offset[0],
                         out.broadcast_like(d[vv]),
                     )
                     out = units.amount2rate(out, out_units=m["variables"][vv]["units"])
                     d_out[vv] = out
                 converted.append(vv)
             elif trans == "amount2rate":
+                # NOTE: This treatment is no longer needed in xclim v0.43.0+ but is kept for backwards compatibility
                 # frequency-based totals to time-based flux
                 logging.info(
                     f"Performing amount-to-rate units conversion for variable `{vv}`."
                 )
                 with xr.set_options(keep_attrs=True):
                     out = units.amount2rate(
                         d[vv],
@@ -368,15 +426,15 @@
     # Copy unconverted variables
     for vv in d.data_vars:
         if vv not in converted:
             d_out[vv] = d[vv]
     return d_out
 
 
-def _offset_time(d: xr.Dataset, p: str, m: Dict) -> xr.Dataset:
+def _offset_time(d: xr.Dataset, p: str, m: dict) -> xr.Dataset:
     key = "_offset_time"
     d_out = xr.Dataset(coords=d.coords, attrs=d.attrs)
     converted = []
     offset, offset_meaning = None, None
 
     time_freq = dict()
     expected_period = _get_section_entry_key(
@@ -417,15 +475,15 @@
     # Copy unconverted variables
     for vv in d.data_vars:
         if vv not in converted:
             d_out[vv] = d[vv]
     return d_out
 
 
-def _invert_sign(d: xr.Dataset, p: str, m: Dict) -> xr.Dataset:
+def _invert_sign(d: xr.Dataset, p: str, m: dict) -> xr.Dataset:
     key = "_invert_sign"
     d_out = xr.Dataset(coords=d.coords, attrs=d.attrs)
     converted = []
     for vv, inv_sign in _iter_entry_key(d, m, "variables", key, p):
         if inv_sign:
             logging.info(f"Inverting sign for `{vv}` (switching direction of values).")
             with xr.set_options(keep_attrs=True):
@@ -445,32 +503,32 @@
     for vv in d.data_vars:
         if vv not in converted:
             d_out[vv] = d[vv]
     return d_out
 
 
 # For converting variable units to standard workflow units
-def _units_cf_conversion(d: xr.Dataset, m: Dict) -> xr.Dataset:
+def _units_cf_conversion(d: xr.Dataset, m: dict) -> xr.Dataset:
     if "time" in m["dimensions"].keys():
         if m["dimensions"]["time"].get("units"):
             d["time"]["units"] = m["dimensions"]["time"]["units"]
 
     for vv, unit in _iter_entry_key(d, m, "variables", "units", None):
         if unit:
             with xr.set_options(keep_attrs=True):
-                d[vv] = units.convert_units_to(d[vv], unit)
+                d[vv] = units.convert_units_to(d[vv], unit, context="hydro")
             prev_history = d.attrs.get("history", "")
             history = f"Converted variable `{vv}` to CF-compliant units (`{unit}`). {prev_history}"
             d.attrs.update(dict(history=history))
 
     return d
 
 
 # For clipping variable values to an established maximum/minimum
-def _clip_values(d: xr.Dataset, p: str, m: Dict) -> xr.Dataset:
+def _clip_values(d: xr.Dataset, p: str, m: dict) -> xr.Dataset:
     key = "_clip_values"
     d_out = xr.Dataset(coords=d.coords, attrs=d.attrs)
     converted = []
     for vv in d.data_vars:
         if vv in m["variables"].keys():
             clip_values = _get_section_entry_key(m, "variables", vv, key, p)
             if clip_values:
@@ -510,15 +568,15 @@
     for vv in d.data_vars:
         if vv not in converted:
             d_out[vv] = d[vv]
 
     return d_out
 
 
-def _ensure_correct_time(d: xr.Dataset, p: str, m: Dict) -> xr.Dataset:
+def _ensure_correct_time(d: xr.Dataset, p: str, m: dict) -> xr.Dataset:
     key = "_ensure_correct_time"
     strict_time = "_strict_time"
 
     if "time" not in m["dimensions"].keys():
         logging.warning(f"No time corrections listed for project `{p}`. Continuing...")
         return d
 
@@ -528,17 +586,14 @@
             f"{' ,'.join([str(v) for v in d.variables.keys()])}. "
             "Continuing..."
         )
         return d
 
     if key in m["dimensions"]["time"].keys():
         freq_found = xr.infer_freq(d.time)
-        if freq_found in ["M", "A"]:
-            freq_found = f"{freq_found}S"
-
         if strict_time in m["dimensions"]["time"].keys():
             if not freq_found:
                 msg = (
                     "Time frequency could not be found. There may be missing timesteps."
                 )
                 if m["dimensions"]["time"].get(strict_time):
                     raise ValueError(msg)
@@ -560,38 +615,54 @@
         else:
             logging.warning("No expected times set for family of projects.")
             return d
 
         if freq_found not in correct_times:
             error_msg = (
                 f"Time frequency {freq_found} not among allowed frequencies: "
-                f"{' ,'.join(correct_times)}"
+                f"{', '.join(correct_times) if isinstance(correct_times, list) else correct_times}"
             )
             if isinstance(correct_time_entry, dict):
                 error_msg = f"{error_msg} for project `{p}`."
             else:
                 error_msg = f"{error_msg}."
             raise ValueError(error_msg)
 
         logging.info(f"Resampling dataset with time frequency: {freq_found}.")
-        d_out = d.assign_coords(
-            time=d.time.resample(time=freq_found).mean(dim="time").time
-        )
+        with xr.set_options(keep_attrs=True):
+            d_out = d.assign_coords(
+                time=d.time.resample(time=freq_found).mean(dim="time").time
+            )
+            d_out.time.attrs.update(d.time.attrs)
 
         prev_history = d.attrs.get("history", "")
         history = f"Resampled time with `freq={freq_found}`. {prev_history}"
         d_out.attrs.update(dict(history=history))
         return d_out
 
     return d
 
 
 # For renaming and reordering lat and lon dims
 def dims_conversion(d: xr.Dataset, p: str, m: dict) -> xr.Dataset:
-    # Rename dimensions to CF to their equivalents
+    """Rename dimensions to CF to their equivalents.
+
+    Parameters
+    ----------
+    d : xarray.Dataset
+        Dataset with dimensions to be updated.
+    p : str
+        Dataset project name.
+    m : dict
+        Metadata definition dictionary for project and variable(s).
+
+    Returns
+    -------
+    xarray.Dataset
+    """
     rename_dims = dict()
     for dim in d.dims:
         if dim in m["dimensions"].keys():
             cf_name = _get_section_entry_key(
                 m, "dimensions", dim, "_cf_dimension_name", p
             )
             if cf_name:
@@ -621,27 +692,44 @@
 
     # Add dimension original name and update attrs
     dim_descriptions = m["dimensions"]
     for dim in m["dimensions"].keys():
         cf_name = dim_descriptions[dim].get("_cf_dimension_name")
         if cf_name is not None and cf_name in d.dims:
             d[cf_name].attrs.update(dict(original_variable=dim))
-            for field in dim_descriptions[dim].keys():
-                if not field.startswith("_"):
-                    d[cf_name].attrs.update({field: dim_descriptions[dim][field]})
+        else:
+            # variable name already follows CF standards
+            cf_name = dim
+        for field in dim_descriptions[dim].keys():
+            if not field.startswith("_"):
+                d[cf_name].attrs.update({field: dim_descriptions[dim][field]})
 
     prev_history = d.attrs.get("history", "")
     history = f"Transposed and renamed dimensions. {prev_history}"
     d.attrs.update(dict(history=history))
 
     return d
 
 
 def variable_conversion(d: xr.Dataset, p: str, m: dict) -> xr.Dataset:
-    # Add variable metadata and remove nonstandard entries
+    """Add variable metadata and remove nonstandard entries.
+
+    Parameters
+    ----------
+    d : xarray.Dataset
+        Dataset with variable(s) to be updated.
+    p : str
+        Dataset project name.
+    m : dict
+        Metadata definition dictionary for project and variable(s).
+
+    Returns
+    -------
+    xarray.Dataset
+    """
     var_descriptions = m["variables"]
     var_correction_fields = [
         "_clip_values",
         "_corrected_units",
         "_invert_sign",
         "_offset_time",
         "_transformation",
@@ -661,15 +749,15 @@
             d = d.rename({orig_var_name: cf_name})
             d[cf_name].attrs.update(dict(original_variable=orig_var_name))
             del d[cf_name].attrs["_cf_variable_name"]
 
     return d
 
 
-def metadata_conversion(d: xr.Dataset, p: str, m: Dict) -> xr.Dataset:
+def metadata_conversion(d: xr.Dataset, p: str, m: dict) -> xr.Dataset:
     """Update xarray dataset and data_vars with project-specific metadata fields.
 
     Parameters
     ----------
     d : xarray.Dataset
         Dataset with metadata to be updated.
     p : str
@@ -679,43 +767,82 @@
 
     Returns
     -------
     xarray.Dataset
     """
     logging.info("Converting metadata to CF-like conventions.")
 
+    header = m["Header"]
+
     # Static handling of version global attributes
-    miranda_version = m["Header"].get("_miranda_version")
+    miranda_version = header.get("_miranda_version")
     if miranda_version:
         if isinstance(miranda_version, bool):
-            m["Header"]["miranda_version"] = __miranda_version__
+            header["miranda_version"] = __miranda_version__
         elif isinstance(miranda_version, dict):
             if p in miranda_version.keys():
-                m["Header"]["miranda_version"] = __miranda_version__
+                header["miranda_version"] = __miranda_version__
+        else:
+            logging.warning(
+                f"`_miranda_version` not set for project `{p}`. Not appending."
+            )
+    if "_miranda_version" in header:
+        del header["_miranda_version"]
+
+    frequency = m["Header"].get("_frequency")
+    if frequency:
+        if isinstance(frequency, bool):
+            _, m["Header"]["frequency"] = get_time_frequency(d)
+        elif isinstance(frequency, dict):
+            if p in frequency.keys():
+                m["Header"]["frequency"] = get_time_frequency(d)
         else:
-            logging.warning("`__miranda_version__` not set for project. Not appending.")
-    if "_miranda_version" in m["Header"]:
-        del m["Header"]["_miranda_version"]
+            logging.warning("`frequency` not set for project. Not appending.")
+    if "_frequency" in m["Header"]:
+        del m["Header"]["_frequency"]
 
     # Conditional handling of global attributes based on project name
-    for field in [f for f in m["Header"] if f.startswith("_")]:
-        if p in m["Header"][field]:
-            if field == "_remove_attrs":
-                for ff in m["Header"][field][p]:
-                    del d.attrs[ff]
+    for field in [f for f in header if f.startswith("_")]:
+        if isinstance(header[field], list):
+            if p in header[field]:
+                attr_treatment = header[field][p]
             else:
-                m["Header"][field[1:]] = m["Header"][field][p]
-        elif field[1:] in m["Header"]:
-            pass
+                logging.warning(
+                    f"Attribute handling (`{field}`) not set for project `{p}`. Continuing..."
+                )
+                continue
+        elif isinstance(header[field], dict):
+            attr_treatment = header[field]
         else:
-            raise AttributeError(f"`{field[1:]}` not found for project dataset.")
-        del m["Header"][field]
+            raise AttributeError(
+                "Attribute handling configuration seems to not be properly configured. Verify JSON."
+            )
+
+        if field == "_map_attrs":
+            for attribute, mapping in attr_treatment.items():
+                header[mapping] = d.attrs[attribute]
+                del d.attrs[attribute]
+        elif field == "_remove_attrs":
+            for ff in attr_treatment:
+                del d.attrs[ff]
+        elif isinstance(attr_treatment, str):
+            if field[1:] in d.attrs:
+                logging.warning(
+                    f"Overwriting `{field[1:]}` based on JSON configuration."
+                )
+            header[field[1:]] = attr_treatment
+        else:
+            raise AttributeError(
+                f"Attribute treatment `{field}` is not properly configured. Verify JSON."
+            )
+
+        del header[field]
 
     # Add global attributes
-    d.attrs.update(m["Header"])
+    d.attrs.update(header)
     d.attrs.update(dict(project=p))
 
     # Date-based versioning
     if not d.attrs.get("version"):
         d.attrs.update(dict(version=f"v{VERSION}"))
 
     prev_history = d.attrs.get("history", "")
@@ -753,70 +880,74 @@
         f"{ds.attrs.get('history')}".strip()
     )
 
     return ds
 
 
 def dataset_conversion(
-    input_files: Union[
-        str,
-        os.PathLike,
-        Sequence[Union[str, os.PathLike]],
-        Iterator[os.PathLike],
-        xr.Dataset,
-    ],
+    input_files: (
+        str
+        | os.PathLike
+        | Sequence[str | os.PathLike]
+        | Iterator[os.PathLike]
+        | xr.Dataset
+    ),
     project: str,
-    domain: Optional[str] = None,
-    mask: Optional[Union[xr.Dataset, xr.DataArray]] = None,
-    mask_cutoff: float = 0.5,
+    domain: str | None = None,
+    mask: xr.Dataset | xr.DataArray | None = None,
+    mask_cutoff: float | bool = False,
+    regrid: bool = False,
     add_version_hashes: bool = True,
-    preprocess: Optional[Union[Callable, str]] = "auto",
+    preprocess: Callable | str | None = "auto",
     **xr_kwargs,
-) -> Union[xr.Dataset, xr.DataArray]:
+) -> xr.Dataset | xr.DataArray:
     """Convert an existing Xarray-compatible dataset to another format with variable corrections applied.
 
     Parameters
     ----------
     input_files : str or os.PathLike or Sequence[str or os.PathLike] or Iterator[os.PathLike] or xr.Dataset
         Files or objects to be converted.
         If sent a list or GeneratorType, will open with :py:func:`xarray.open_mfdataset` and concatenate files.
     project : {"cordex", "cmip5", "cmip6", "ets-grnch", "isimip-ft", "pcic-candcs-u6", "converted"}
         Project name for decoding/handling purposes.
     domain: {"global", "nam", "can", "qc", "mtl"}, optional
         Domain to perform subsetting for. Default: None.
     mask : Optional[Union[xr.Dataset, xr.DataArray]]
         DataArray or single data_variable dataset containing mask.
-    mask_cutoff : float
-        If land_sea_mask supplied, the threshold above which to mask with land_sea_mask. Default: 0.5.
+    mask_cutoff : float or bool
+        If land_sea_mask supplied, the threshold above which to mask with land_sea_mask. Default: False.
+    regrid : bool
+        Performing regridding with xesmf. Default: False.
     add_version_hashes : bool
         If True, version name and sha256sum of source file(s) will be added as a field among the global attributes.
     preprocess : callable or str, optional
         Preprocessing functions to perform over each Dataset.
         Default: "auto" - Run preprocessing fixes based on supplied fields from metadata definition.
         Callable - Runs function over Dataset (single) or supplied to `preprocess` (multifile dataset).
     **xr_kwargs
         Arguments passed directly to xarray.
 
     Returns
     -------
     xr.Dataset or xr.DataArray
     """
-    if not isinstance(input_files, xr.Dataset):
+    if isinstance(input_files, xr.Dataset):
+        ds = input_files
+    else:
         if isinstance(input_files, (str, os.PathLike)):
             if Path(input_files).is_dir():
                 files = []
                 files.extend([f for f in Path(input_files).glob("*.nc")])
                 files.extend([f for f in Path(input_files).glob("*.zarr")])
             else:
                 files = [Path(input_files)]
         elif isinstance(input_files, (Sequence, Iterator)):
             files = [Path(f) for f in input_files]
         else:
             files = input_files
-
         version_hashes = dict()
         if add_version_hashes:
             for file in files:
                 version_hashes[file.name] = find_version_hash(file)
 
         preprocess_kwargs = dict()
         if preprocess:
@@ -829,29 +960,23 @@
 
         if len(files) == 1:
             ds = xr.open_dataset(files[0], **xr_kwargs)
             for _, process in preprocess_kwargs.items():
                 ds = process(ds)
         else:
             ds = xr.open_mfdataset(files, **xr_kwargs, **preprocess_kwargs)
-
         if version_hashes:
             ds.attrs.update(dict(original_files=str(version_hashes)))
-    else:
-        ds = input_files
 
     ds = dataset_corrections(ds, project)
 
     if domain:
         ds = subset_domain(ds, domain)
 
     if isinstance(mask, (str, Path)):
         mask = xr.open_dataset(mask)
     if isinstance(mask, (xr.Dataset, xr.DataArray)):
-        # TODO: This should only be triggered by differences in lat, lon grid.
-        # logging.info(
-        #     "Mask supplied. Performing conservative-normed regridding and masking."
-        # )
-        # mask = conservative_regrid(mask, ds)
+        if regrid:
+            mask = conservative_regrid(ds, mask)
         ds = threshold_mask(ds, mask=mask, mask_cutoff=mask_cutoff)
 
     return ds
```

### Comparing `miranda-0.4.0/miranda/convert/_data_definitions.py` & `miranda-0.5.0/miranda/convert/_data_definitions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,34 @@
+from __future__ import annotations
+
 import datetime
 import json
 import logging.config
 import os
 from pathlib import Path
-from typing import Dict, List, Optional, Union
 
 from miranda.scripting import LOGGING_CONFIG
 from miranda.storage import report_file_size
 
 logging.config.dictConfig(LOGGING_CONFIG)
 
 __all__ = [
     "era5_variables",
     "eccc_rdrs_variables",
     "gather_agcfsr",
     "gather_agmerra",
     "gather_ecmwf",
     "gather_grnch",
+    "gather_nex",
     "gather_nrcan_gridded_obs",
     "gather_raw_rdrs_by_years",
     "gather_rdrs",
     "gather_sc_earth",
     "gather_wfdei_gem_capa",
+    "gather_emdna",
     "nasa_ag_variables",
     "nrcan_variables",
     "project_institutes",
     "sc_earth_variables",
     "wfdei_gem_capa_variables",
     "xarray_frequencies_to_cmip6like",
 ]
@@ -72,17 +75,17 @@
     "era5-single-levels-monthly-means": "ecmwf",
     "era5-single-levels-monthly-means-preliminary-back-extension": "ecmwf",
     "era5-single-levels-preliminary-back-extension": "ecmwf",
     "merra2": "nasa",
     "nrcan-gridded-10km": "nrcan",
     "wfdei-gem-capa": "usask",
     "rdrs-v21": "eccc",
+    "NEX-GDDP-CMIP6": "nasa",
 }
 
-
 # Manually map xarray frequencies to CMIP6/CMIP5 controlled vocabulary.
 # see: https://github.com/ES-DOC/pyessv-archive
 xarray_frequencies_to_cmip6like = {
     "H": "hr",
     "D": "day",
     "W": "sem",
     "M": "mon",
@@ -90,101 +93,100 @@
     "A": "yr",
     "Y": "yr",
 }
 
 
 def _gather(
     name: str,
-    variables: List[str],
-    source: Union[str, os.PathLike],
+    variables: list[str],
+    source: str | os.PathLike,
     glob_pattern: str,
-    suffix: Optional[str] = None,
-    recursive: Optional[bool] = False,
-) -> Dict[str, List[Path]]:
+    suffix: str | None = None,
+    recursive: bool | None = False,
+) -> dict[str, list[Path]]:
     source = Path(source).expanduser()
     logging.info(f"Gathering {name} files from: {source.as_posix()}")
     in_files = list()
     for variable in variables:
         if suffix:
             pattern = glob_pattern.format(variable=variable, name=name, suffix=suffix)
         else:
-            pattern = glob_pattern.format(variable)
+            pattern = glob_pattern.format(variable=variable)
         if recursive:
             in_files.extend(list(sorted(source.rglob(pattern))))
         else:
             in_files.extend(list(sorted(source.glob(pattern))))
     logging.info(
         f"Found {len(in_files)} files, totalling {report_file_size(in_files)}."
     )
     return {name: in_files}
 
 
 def gather_ecmwf(
     project: str,
-    path: Union[str, os.PathLike],
+    path: str | os.PathLike,
     back_extension: bool = False,
     monthly_means: bool = False,
-) -> Dict[str, List[Path]]:
+) -> dict[str, list[Path]]:
     """
 
     Parameters
     ----------
     project : {"era5-single-levels", "era5-pressure-levels", "era5-land"}
     path : str or os.PathLike
     back_extension : bool
     monthly_means : bool
 
     Returns
     -------
-    dict(str, list[pathlib.Path])
+    dict[str, list[pathlib.Path]]
     """
-    # ERA5-Single-Levels source data
     name = (
         f"{project}"
         f"{'-monthly-means' if monthly_means else ''}"
         f"{'-preliminary-back-extension' if back_extension else ''}"
     )
     glob_pattern = "".join(["{variable}", f"_*_{name}_*.nc"])
 
     return _gather(name, era5_variables, source=path, glob_pattern=glob_pattern)
 
 
-def gather_agmerra(path: Union[str, os.PathLike]) -> Dict[str, List[Path]]:
+def gather_agmerra(path: str | os.PathLike) -> dict[str, list[Path]]:
     """Gather agMERRA source data.
 
     Parameters
     ----------
     path : str or os.PathLike
 
     Returns
     -------
-    dict(str, list[pathlib.Path])
+    dict[str, list[pathlib.Path]]
     """
     return _gather(
         "merra", nasa_ag_variables, source=path, glob_pattern="AgMERRA_*_{variable}.nc4"
     )
 
 
-def gather_agcfsr(path: Union[str, os.PathLike]) -> Dict[str, List[Path]]:
+def gather_agcfsr(path: str | os.PathLike) -> dict[str, list[Path]]:
     """Gather agCFSR source data.
 
     Parameters
     ----------
     path : str or os.PathLike
 
     Returns
     -------
-    dict(str, list[pathlib.Path])
+    dict[str, list[pathlib.Path]]
     """
     return _gather(
         "cfsr", nasa_ag_variables, source=path, glob_pattern="AgCFSR_*_{variable}.nc4"
     )
 
 
-def gather_nrcan_gridded_obs(path: Union[str, os.PathLike]) -> Dict[str, List[Path]]:
+def gather_nrcan_gridded_obs(path: str | os.PathLike) -> dict[str, list[Path]]:
     """Gather NRCan Gridded Observations source data.
 
     Parameters
     ----------
     path : str or os.PathLike
 
     Returns
@@ -192,67 +194,68 @@
     dict(str, list[pathlib.Path])
     """
     return _gather(
         "nrcan", nrcan_variables, source=path, glob_pattern="*{variable}_*.nc"
     )
 
 
-def gather_wfdei_gem_capa(path: Union[str, os.PathLike]) -> Dict[str, List[Path]]:
+def gather_wfdei_gem_capa(path: str | os.PathLike) -> dict[str, list[Path]]:
     """Gather WFDEI-GEM-CaPa source data.
 
     Parameters
     ----------
     path : str or os.PathLike
 
     Returns
     -------
-    dict(str, list[pathlib.Path])
+    dict[str, list[pathlib.Path]]
     """
     return _gather(
         "wfdei-gem-capa",
         wfdei_gem_capa_variables,
         source=path,
         glob_pattern="{variable}_*.nc",
     )
 
 
-def gather_sc_earth(path: Union[str, os.PathLike]) -> Dict[str, List[Path]]:
+def gather_sc_earth(path: str | os.PathLike) -> dict[str, list[Path]]:
     """Gather SC-Earth source data
 
     Parameters
     ----------
     path : str or os.PathLike
 
     Returns
     -------
-    dict(str, list[pathlib.Path])
+    dict[str, list[pathlib.Path]]
     """
     return _gather(
         "sc-earth",
         sc_earth_variables,
         source=path,
         glob_pattern="SC-Earth_{variable}_*.nc",
     )
 
 
 def gather_rdrs(
-    name: str, path: Union[str, os.PathLike], suffix: str, key: str
-) -> Dict[str, Dict[str, List[Path]]]:
+    name: str, path: str | os.PathLike, suffix: str, key: str
+) -> dict[str, dict[str, list[Path]]]:
     """Gather RDRS processed source data.
 
     Parameters
     ----------
     name : str
     path : str or os.PathLike
     suffix : str
-    key : str  one of 'raw' or 'cf' indicating which variable name dictionary to search for
+    key : {"raw", "cf"}
+        Indicating which variable name dictionary to search for.
 
     Returns
     -------
-    dict(str, list[pathlib.Path])
+    dict[str, list[pathlib.Path]]
     """
     if isinstance(path, str):
         path = Path(path).expanduser()
 
     files = dict({name: dict()})
     for vv in eccc_rdrs_variables[key]:
         tmp = _gather(
@@ -264,44 +267,111 @@
             recursive=True,
         )
         files[name][vv] = tmp[name]
     return files
 
 
 def gather_raw_rdrs_by_years(
-    path: Union[str, os.PathLike]
-) -> Dict[str, Dict[str, List[Path]]]:
+    path: str | os.PathLike,
+) -> dict[str, dict[str, list[Path]]]:
     """Gather raw RDRS files for preprocessing.
 
     Parameters
     ----------
     path: str or os.PathLike
 
     Returns
     -------
-    dict(str, dict(str, list[Path])) or None
+    dict[str, dict[str, list[pathlib.Path]]
     """
     # Time stamps starts at noon and flow into subsequent months
     # Need full year plus previous december in order to easily produce complete hourly frequency monthly files
     path = Path(path)
     year_sets = dict()
     for year in range(1950, datetime.datetime.now().year + 1):
         files = sorted(list(path.glob(f"{year - 1}12*.nc")))
         if files:
             files = [files[-1]]
         files.extend(sorted(list(path.glob(f"{year}*.nc"))))
         year_sets[str(year)] = files
     return {"rdrs-v21": year_sets}
 
 
-def gather_grnch(path: Union[str, os.PathLike]) -> Dict[str, List[Path]]:
+def gather_grnch(path: str | os.PathLike) -> dict[str, list[Path]]:
+    """Gather raw ETS-GRNCH files for preprocessing.
+
+    Parameters
+    ----------
+    path: str or os.PathLike
+
+    Returns
+    -------
+    dict(str, dict(str, list[Path])) or None
+    """
     # GRNCH-ETS source data
     source_grnch = Path(path)
     logging.info(f"Gathering GRNCH from: {source_grnch.as_posix()}")
     in_files_grnch = list()
     for v in grnch_variables:
         for yyyy in range(1970, 2020):
             in_files_grnch.extend(list(source_grnch.rglob(f"{v}_{yyyy}.nc")))
     logging.info(
         f"Found {len(in_files_grnch)} files, totalling {report_file_size(in_files_grnch)}."
     )
     return dict(cfsr=sorted(in_files_grnch))
+
+
+def gather_nex(
+    path: str | os.PathLike,
+) -> dict[str, list[Path]]:
+    """Gather raw NEX files for preprocessing.
+
+    Put all files that should be contained in one dataset in one entry of the dictionary.
+
+    Parameters
+    ----------
+    path : str or os.PathLike
+
+    Returns
+    -------
+    dict[str, list[pathlib.Path]]
+    """
+    source = Path(path)
+    datasets = source.glob("*/*/*/*/*/*/*/*/*/")
+
+    out_dict = dict()
+    # separate files by datasets
+    for dataset in datasets:
+        in_files = list()
+        in_files.extend(list(sorted(dataset.glob("*.nc"))))
+        out_dict[str(dataset)] = in_files
+    return out_dict
+
+
+def gather_emdna(
+    path: str | os.PathLike,
+) -> dict[str, list[Path]]:
+    """Gather raw EMDNA files for preprocessing.
+
+    Put all files with the same member together.
+
+    Parameters
+    ----------
+    path : str or os.PathLike
+
+    Returns
+    -------
+    dict[str, list[pathlib.Path]]
+    """
+    source = Path(path)
+    member_dict = {}
+    # 100 members
+    members = [f"{i:03d}" for i in range(1, 101)]
+    for member in members:
+        member_dict[member] = list(
+            sorted(source.glob(f"EMDNA_estimate/*/EMDNA_*.{member}.nc4"))
+        )
+
+    # OI
+    member_dict["OI"] = list(sorted(source.glob("OI_estimate/*.nc4")))
+
+    return member_dict
```

### Comparing `miranda-0.4.0/miranda/convert/_reconstruction.py` & `miranda-0.5.0/miranda/convert/_reconstruction.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from __future__ import annotations
+
 import logging.config
 import os
+from collections.abc import Sequence
 from pathlib import Path
-from typing import Dict, List, Optional, Sequence, Union
 
 import dask.config
 import xarray as xr
-from clisops.core import subset
 from dask import compute
 from dask.diagnostics import ProgressBar
 from xclim.core import calendar
 
 from miranda.gis import subset_domain
 from miranda.io.utils import delayed_write, get_chunks_on_disk
 from miranda.scripting import LOGGING_CONFIG
@@ -32,34 +33,34 @@
 def _drop_those_time_bnds(dataset: xr.Dataset) -> xr.Dataset:
     if "time_bnds" in dataset.variables:
         return dataset.drop_vars(["time_bnds"])
     return dataset
 
 
 def reanalysis_processing(
-    data: Dict[str, List[Union[str, os.PathLike]]],
-    output_folder: Union[str, os.PathLike],
+    data: dict[str, list[str | os.PathLike]],
+    output_folder: str | os.PathLike,
     variables: Sequence[str],
-    aggregate: Union[str, bool] = False,
-    domains: Union[str, List[str]] = "_DEFAULT",
-    start: Optional[str] = None,
-    end: Optional[str] = None,
-    target_chunks: Optional[dict] = None,
+    aggregate: str | bool = False,
+    domains: str | list[str] = "_DEFAULT",
+    start: str | None = None,
+    end: str | None = None,
+    target_chunks: dict | None = None,
     output_format: str = "netcdf",
     overwrite: bool = False,
     engine: str = "h5netcdf",
     n_workers: int = 4,
     **dask_kwargs,
 ) -> None:
     """
 
     Parameters
     ----------
-    data: Dict[str, List[str]]
-    output_folder: Union[str, os.PathLike]
+    data: dict[str, list[str]]
+    output_folder: str or os.PathLike
     variables: Sequence[str]
     aggregate: {"day", None}
     domains: {"QC", "CAN", "AMNO", "NAM", "GLOBAL"}
     start: str, optional
     end: str, optional
     target_chunks: dict, optional
     output_format: {"netcdf", "zarr"}
@@ -148,18 +149,16 @@
                             preprocess=_drop_those_time_bnds,
                             parallel=True,
                         )
 
                         # Subsetting operations
                         if domain.lower() in ["global", "not-specified"]:
                             if start or end:
-                                ds = subset.subset_time(
-                                    xr.open_mfdataset(multi_files, **xr_kwargs),
-                                    start_date=start,
-                                    end_date=end,
+                                ds = xr.open_mfdataset(multi_files, **xr_kwargs).sel(
+                                    time=slice(start, end)
                                 )
                             else:
                                 ds = xr.open_mfdataset(multi_files, **xr_kwargs)
                         else:
                             ds = subset_domain(
                                 xr.open_mfdataset(multi_files, **xr_kwargs),
                                 domain,
```

### Comparing `miranda-0.4.0/miranda/convert/data/cmip_ouranos_attrs.json` & `miranda-0.5.0/miranda/convert/data/cmip_ouranos_attrs.json`

 * *Files identical despite different names*

### Comparing `miranda-0.4.0/miranda/convert/data/deh_cf_attrs.json` & `miranda-0.5.0/miranda/convert/data/deh_cf_attrs.json`

 * *Files identical despite different names*

### Comparing `miranda-0.4.0/miranda/convert/data/eccc_cf_attrs.json` & `miranda-0.5.0/miranda/convert/data/eccc_cf_attrs.json`

 * *Files identical despite different names*

### Comparing `miranda-0.4.0/miranda/convert/data/eccc_rdrs_cf_attrs.json` & `miranda-0.5.0/miranda/convert/data/eccc_rdrs_cf_attrs.json`

 * *Files identical despite different names*

### Comparing `miranda-0.4.0/miranda/convert/data/ecmwf_cf_attrs.json` & `miranda-0.5.0/miranda/convert/data/ecmwf_cf_attrs.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.977518315018315%*

 * *Differences: {"'Header'": "{'_frequency': True}",*

 * * "'dimensions'": "{'latitude': {'_precision': {'era5-land-monthly-means': 4}}, 'longitude': "*

 * *                 "{'_precision': {'era5-land-monthly-means': 4}}, 'time': {'_ensure_correct_time': "*

 * *                 "{'era5-land-monthly-means': 'MS', 'era5-pressure-levels-monthly-means': 'MS', "*

 * *                 "'era5-pressure-levels-monthly-means-preliminary-back-extension': 'MS', "*

 * *                 "'era5-single-levels-monthly-means': 'MS', "*

 * *                 "'era5-singl […]*

```diff
@@ -9,14 +9,15 @@
             "era5-pressure-levels-monthly-means-preliminary-back-extension": "https://doi.org/10.24381/cds.6860a573",
             "era5-pressure-levels-preliminary-back-extension": "https://doi.org/10.24381/cds.bd0915c6",
             "era5-single-levels": "https://doi.org/10.24381/cds.adbb2d47",
             "era5-single-levels-monthly-means": "https://doi.org/10.24381/cds.f17050d7",
             "era5-single-levels-monthly-means-preliminary-back-extension": "https://doi.org/10.24381/cds.f17050d7",
             "era5-single-levels-preliminary-back-extension": "https://doi.org/10.24381/cds.adbb2d47"
         },
+        "_frequency": true,
         "_miranda_version": true,
         "_source": {
             "era5-land": "ERA5-Land",
             "era5-land-monthly-means": "ERA5-Land",
             "era5-pressure-levels": "ERA5",
             "era5-pressure-levels-monthly-means": "ERA5",
             "era5-pressure-levels-monthly-means-preliminary-back-extension": "ERA5-preliminary",
@@ -36,38 +37,40 @@
         "table_id": "ECMWF",
         "type": "reconstruction"
     },
     "dimensions": {
         "latitude": {
             "_cf_dimension_name": "lat",
             "_precision": {
-                "era5-land": 4
+                "era5-land": 4,
+                "era5-land-monthly-means": 4
             },
             "axis": "Y",
             "standard_name": "latitude"
         },
         "longitude": {
             "_cf_dimension_name": "lon",
             "_precision": {
-                "era5-land": 4
+                "era5-land": 4,
+                "era5-land-monthly-means": 4
             },
             "axis": "X",
             "standard_name": "longitude"
         },
         "time": {
             "_ensure_correct_time": {
                 "era5-land": "1H",
-                "era5-land-monthly-means": "1M",
+                "era5-land-monthly-means": "MS",
                 "era5-pressure-levels": "1H",
-                "era5-pressure-levels-monthly-means": "1M",
-                "era5-pressure-levels-monthly-means-preliminary-back-extension": "1M",
+                "era5-pressure-levels-monthly-means": "MS",
+                "era5-pressure-levels-monthly-means-preliminary-back-extension": "MS",
                 "era5-pressure-levels-preliminary-back-extension": "1H",
                 "era5-single-levels": "1H",
-                "era5-single-levels-monthly-means": "1M",
-                "era5-single-levels-monthly-means-preliminary-back-extension": "1M",
+                "era5-single-levels-monthly-means": "MS",
+                "era5-single-levels-monthly-means-preliminary-back-extension": "MS",
                 "era5-single-levels-preliminary-back-extension": "1H"
             },
             "_strict_time": false,
             "axis": "T",
             "long_name": "time",
             "standard_name": "time"
         }
@@ -118,14 +121,25 @@
             "cell_methods": "time: mean (interval: 1 hour)",
             "description": "Total potential evaporation thickness converted to mass flux using a water density of 1000 kg/m\u00b3.",
             "long_name": "Potential evapotranspiration",
             "original_long_name": "Potential evaporation",
             "standard_name": "water_evapotranspiration_flux",
             "units": "kg m-2 s-1"
         },
+        "ptype": {
+            "_cf_variable_name": "prtype",
+            "_invert_sign": false,
+            "_offset_time": false,
+            "_transformation": false,
+            "cell_methods": "time: point",
+            "description": "This parameter describes the type of precipitation at the surface, at the specified time. A precipitation type is assigned wherever there is a non-zero value of precipitation. In the ECMWF Integrated Forecasting System (IFS) there are only two predicted precipitation variables: rain and snow. Precipitation type is derived from these two predicted variables in combination with atmospheric conditions, such as temperature. Values of precipitation type defined in the IFS: 0: No precipitation, 1: Rain, 3: Freezing rain (i.e. supercooled raindrops which freeze on contact with the ground and other surfaces), 5: Snow, 6: Wet snow (i.e. snow particles which are starting to melt); 7: Mixture of rain and snow, 8: Ice pellets. These precipitation types are consistent with WMO Code Table 4.201. Other types in this WMO table are not defined in the IFS.",
+            "long_name": "Precipitation type",
+            "standard_name": "predominant_precipitation_type_at_surface",
+            "units": "1"
+        },
         "q": {
             "_cf_variable_name": "hus",
             "_corrected_units": 1,
             "_invert_sign": false,
             "_offset_time": false,
             "_transformation": false,
             "cell_methods": "time: point",
```

### Comparing `miranda-0.4.0/miranda/convert/data/ets_grnch_cf_attrs.json` & `miranda-0.5.0/miranda/convert/data/ets_grnch_cf_attrs.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'Header'": "{'_frequency': True, delete: ['frequency']}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "Header": {
         "Conventions": "CF-1.9",
+        "_frequency": true,
         "_miranda_version": true,
         "contact": "Dr. Annie Poulin (annie.poulin@etsmtl.ca)",
         "creation_date": "2022-07-16T11:22:42Z",
-        "frequency": "day",
         "institution": "ETS",
         "institution_name": "\u00c9cole de Technologie Sup\u00e9rieure (ETS), Hydrology, Climate and Climate Change Laboratory (HC3)",
         "license": "Creative Commons Attribution 4.0 International (CC-BY 4.0)",
         "license_type": "OSI approved",
         "license_url": "https://creativecommons.org/licenses/by/4.0",
         "processing_level": "raw",
         "project": "Info-CRUE",
```

### Comparing `miranda-0.4.0/miranda/convert/data/hq_cf_attrs.json` & `miranda-0.5.0/miranda/convert/data/hq_cf_attrs.json`

 * *Files identical despite different names*

### Comparing `miranda-0.4.0/miranda/convert/data/melcc_cf_attrs.json` & `miranda-0.5.0/miranda/convert/data/melcc_cf_attrs.json`

 * *Files identical despite different names*

### Comparing `miranda-0.4.0/miranda/convert/data/nasa_cf_attrs.json` & `miranda-0.5.0/miranda/convert/data/nasa_cf_attrs.json`

 * *Files identical despite different names*

### Comparing `miranda-0.4.0/miranda/convert/data/rvt_raven_attrs.json` & `miranda-0.5.0/miranda/convert/data/rvt_raven_attrs.json`

 * *Files identical despite different names*

### Comparing `miranda-0.4.0/miranda/convert/data/usask_cf_attrs.json` & `miranda-0.5.0/miranda/convert/data/usask_cf_attrs.json`

 * *Files identical despite different names*

### Comparing `miranda-0.4.0/miranda/convert/deh.py` & `miranda-0.5.0/miranda/convert/deh.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+"""DEH Hydrograph Conversion module."""
+from __future__ import annotations
+
 import json
 import logging.config
 import os
 import re
 from pathlib import Path
-from typing import Optional, Tuple, Union
 
 import pandas as pd
 import xarray as xr
 from xclim.core.units import units as u
 
 from miranda.scripting import LOGGING_CONFIG
 
@@ -26,17 +28,16 @@
     "Bassin versant: ": "bv",
     "Coordonnées: (NAD83) ": "coords",
 }
 
 data_header_pattern = "Station Date Débit (m³/s) Remarque\n"
 
 
-def extract_daily(path: Union[os.PathLike, str]) -> Tuple[dict, pd.DataFrame]:
+def extract_daily(path: os.PathLike | str) -> tuple[dict, pd.DataFrame]:
     """Extract data and metadata from DEH (MELCC) stream flow file."""
-
     with open(path, encoding="latin1") as fh:
         txt = fh.read()
         txt = re.sub(" +", " ", txt)
         meta, data = txt.split(data_header_pattern)
 
     m = dict()
     for key in meta_patterns:
@@ -115,11 +116,11 @@
         "source"
     ] = "Hydrometric data <https://www.cehq.gouv.qc.ca/hydrometrie/historique_donnees/index.asp>"
     ds.attrs["redistribution"] = "Redistribution policy unknown. For internal use only."
 
     return ds
 
 
-def open_txt(path: Union[str, Path], cf_table: Optional[dict] = cmor) -> xr.Dataset:
+def open_txt(path: str | Path, cf_table: dict | None = cmor) -> xr.Dataset:
     """Extract daily HQ meteorological data and convert to xr.DataArray with CF-Convention attributes."""
     meta, data = extract_daily(path)
     return to_cf(meta, data, cf_table)
```

### Comparing `miranda-0.4.0/miranda/convert/eccc.py` & `miranda-0.5.0/miranda/convert/eccc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Convert ECCC data
+"""Environment and Climate Change Canada Data Conversion module."""
 from __future__ import annotations
 
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import xarray as xr
```

### Comparing `miranda-0.4.0/miranda/convert/eccc_rdrs.py` & `miranda-0.5.0/miranda/convert/eccc_rdrs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+"""Environment and Climate Change Canada RDRS conversion tools."""
+from __future__ import annotations
+
 import logging.config
 import os
 from pathlib import Path
-from typing import List, Optional, Set, Union
 
 import xarray as xr
 from numpy import unique
 
 from miranda.io import fetch_chunk_config, write_dataset_dict
 from miranda.scripting import LOGGING_CONFIG
 from miranda.units import get_time_frequency
@@ -19,74 +21,73 @@
 
 __all__ = ["convert_rdrs", "rdrs_to_daily"]
 
 
 # FIXME: Can we use `name_output_file` instead? We already have a better version of this function.
 
 
-def _get_drop_vars(
-    file: Union[str, os.PathLike], *, keep_vars: Union[List[str], Set[str]]
-):
+def _get_drop_vars(file: str | os.PathLike, *, keep_vars: list[str] | set[str]):
     drop_vars = list(xr.open_dataset(file).data_vars)
     return list(set(drop_vars) - set(keep_vars))
 
 
 def convert_rdrs(
     project: str,
-    input_folder: Union[str, os.PathLike],
-    output_folder: Union[str, os.PathLike],
+    input_folder: str | os.PathLike,
+    output_folder: str | os.PathLike,
     output_format: str = "zarr",
-    working_folder: Optional[Union[str, os.PathLike]] = None,
+    working_folder: str | os.PathLike | None = None,
     overwrite: bool = False,
     **dask_kwargs,
-):
-    """
+) -> None:
+    r"""
 
     Parameters
     ----------
-    project
-    input_folder
-    output_folder
-    output_format
-    working_folder
-    overwrite
-    dask_kwargs
+    project : str
+    input_folder : str or os.PathLike
+    output_folder : str or os.PathLike
+    output_format : {"netcdf", "zarr"}
+    working_folder : str or os.PathLike, optional
+    overwrite : bool
+    \*\*dask_kwargs
 
     Returns
     -------
-
+    None
     """
     # TODO: This setup configuration is near-universally portable. Should we consider applying it to all conversions?
     var_attrs = load_json_data_mappings(project=project)["variables"]
     freq_dict = dict(h="hr", d="day")
 
     if isinstance(input_folder, str):
         input_folder = Path(input_folder).expanduser()
     if isinstance(output_folder, str):
         output_folder = Path(output_folder).expanduser()
     if isinstance(working_folder, str):
         working_folder = Path(working_folder).expanduser()
 
     # FIXME: Do we want to collect everything? Maybe return a dictionary with years and associated files?
 
+    out_freq = None
     gathered = gather_raw_rdrs_by_years(input_folder)
     for year, ncfiles in gathered[project].items():
         ds_allvars = None
         if len(ncfiles) >= 28:
             for nc in ncfiles:
                 ds1 = xr.open_dataset(nc, chunks="auto")
-                if ds_allvars is None:
+                if ds_allvars is None and out_freq is None:
                     ds_allvars = ds1
-                    outfreq, meaning = get_time_frequency(ds1)
-                    outfreq = (
-                        f"{outfreq[0]}{freq_dict[outfreq[1]]}"
+                    out_freq, meaning = get_time_frequency(ds1)
+                    out_freq = (
+                        f"{out_freq[0]}{freq_dict[out_freq[1]]}"
                         if meaning == "hour"
-                        else freq_dict[outfreq[1]]
+                        else freq_dict[out_freq[1]]
                     )
-                    ds_allvars.attrs["frequency"] = outfreq
+                    ds_allvars.attrs["frequency"] = out_freq
                 else:
                     ds_allvars = xr.concat(
                         [ds_allvars, ds1], data_vars="minimal", dim="time"
                     )
             ds_allvars = ds_allvars.sel(time=f"{year}")
             # This is the heart of the conversion utility; We could apply this to multiple projects.
             for month in unique(ds_allvars.time.dt.month):
@@ -99,58 +100,60 @@
                     ds_out = ds_out.assign_coords(rotated_pole=ds_out["rotated_pole"])
                     ds_corr = dataset_conversion(
                         ds_out,
                         project=project,
                         add_version_hashes=False,
                         overwrite=overwrite,
                     )
-                    chunks = fetch_chunk_config(project=project, freq=outfreq)
+                    chunks = fetch_chunk_config(
+                        priority="time", freq=out_freq, dims=ds_corr.dims
+                    )
                     chunks["time"] = len(ds_corr.time)
                     write_dataset_dict(
                         {var_attrs[var_attr]["_cf_variable_name"]: ds_corr},
-                        output_folder=output_folder.joinpath(outfreq),
+                        output_folder=output_folder.joinpath(out_freq),
                         temp_folder=working_folder,
                         output_format=output_format,
                         overwrite=False,
                         chunks=chunks,
                         **dask_kwargs,
                     )
 
 
 # FIXME: This looks mostly like code to stage writing out files. Should it be moved to an IO module?
 def rdrs_to_daily(
     project: str,
-    input_folder: Union[str, os.PathLike],
-    output_folder: Union[str, os.PathLike],
-    working_folder: Optional[Union[str, os.PathLike]] = None,
+    input_folder: str | os.PathLike,
+    output_folder: str | os.PathLike,
+    working_folder: str | os.PathLike | None = None,
     overwrite: bool = False,
     output_format: str = "zarr",
-    year_start: Optional[int] = None,
-    year_end: Optional[int] = None,
-    process_variables: Optional[list] = None,
+    year_start: int | None = None,
+    year_end: int | None = None,
+    process_variables: list[str] | None = None,
     **dask_kwargs,
-):
-    """
+) -> None:
+    r"""Write out RDRS files to daily-timestep files.
 
     Parameters
     ----------
-    project
-    input_folder
-    output_folder
-    working_folder
-    overwrite
-    output_format
-    year_start
-    year_end
-    process_variables
-    dask_kwargs
+    project : str
+    input_folder : str or os.PathLike
+    output_folder : str or os.PathLike
+    working_folder : str or os.PathLike
+    overwrite : bool
+    output_format : {"netcdf", "zarr"}
+    year_start : int, optional
+    year_end : int, optional
+    process_variables : list of str, optional
+    \*\*dask_kwargs
 
     Returns
     -------
-
+    None
     """
     if isinstance(input_folder, str):
         input_folder = Path(input_folder).expanduser()
     if isinstance(output_folder, str):
         output_folder = Path(output_folder).expanduser()  # noqa
     if isinstance(working_folder, str):
         working_folder = Path(working_folder).expanduser()
```

### Comparing `miranda-0.4.0/miranda/convert/ecmwf.py` & `miranda-0.5.0/miranda/convert/ecmwf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
+"""ECMWF TIGGE Conversion module."""
+from __future__ import annotations
+
 import itertools as it
 import logging.config
 import multiprocessing
 import os
 import shutil
 import tempfile
 from pathlib import Path
-from typing import Optional
 
 import xarray
 from dask.diagnostics import ProgressBar
 
 from miranda.scripting import LOGGING_CONFIG
 
 logging.config.dictConfig(LOGGING_CONFIG)
 
 __all__ = ["tigge_convert"]
 
 
 def tigge_convert(
-    source: Optional[os.PathLike] = None,
-    target: Optional[os.PathLike] = None,
+    source: os.PathLike | None = None,
+    target: os.PathLike | None = None,
     processes: int = 8,
 ) -> None:
     """Convert grib2 file to netCDF format.
 
     Parameters
     ----------
     source : os.PathLike, optional
```

### Comparing `miranda-0.4.0/miranda/convert/hq.py` & `miranda-0.5.0/miranda/convert/hq.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+"""Hydro Quebec Weather Station Data Conversion module."""
+from __future__ import annotations
+
 import csv
 import datetime as dt
 import json
 import logging.config
 import re
 from pathlib import Path
-from typing import Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 from xclim.core.units import units as u
 from xclim.core.units import units2pint
 
@@ -59,15 +61,15 @@
     "Qualite": lambda x: int(x.split("-")[0]),
     "Statut": lambda x: int(x.split("-")[0]),
     "unité": lambda x: cf_units.get(x, x),
     "pas": lambda x: cf_frequency.get(x, x),
 }
 
 
-def guess_variable(meta, cf_table: Optional[dict]) -> Tuple[str, Optional[str]]:
+def guess_variable(meta, cf_table: dict | None) -> tuple[str, str | None]:
     """Return the corresponding CMOR variable."""
     if cf_table is None:
         cf_table = cmor
 
     v = meta["variable"]
 
     corr = {
@@ -103,17 +105,16 @@
     "Fin du pas journalier": "day",
     "Instantanée du pas horaire": "1h",
     "Fin du pas horaire": "1h",
 }
 cf_attrs_names = {"x": "lon", "y": "lat", "z": "elevation", "nom": "site"}
 
 
-def extract_daily(path) -> Tuple[dict, pd.DataFrame]:
+def extract_daily(path) -> tuple[dict, pd.DataFrame]:
     """Extract data and metadata from HQ meteo file."""
-
     with open(path, encoding="latin1") as fh:
         txt = fh.read()
         meta, data = re.split(data_header_pattern, txt, maxsplit=2)
 
     sections = iter(re.split(section_patterns, meta)[1:])
 
     m = dict()
@@ -141,19 +142,16 @@
         infer_datetime_format=True,
         decimal=",",
     )
 
     return m, d
 
 
-def to_cf(
-    meta: dict, data: pd.DataFrame, cf_table: Optional[dict] = None
-) -> xr.DataArray:
+def to_cf(meta: dict, data: pd.DataFrame, cf_table: dict | None = None) -> xr.DataArray:
     """Return CF-compliant metadata."""
-
     if cf_table is None:
         cf_table = dict()
 
     # Convert meta values
     m = dict()
     for key, val in meta.items():
         m[key] = converters.get(key, lambda q: q)(val)
@@ -177,11 +175,11 @@
     coords["time"] = data.index.values
     cf_corrected = xr.DataArray(
         data=x, dims="time", coords=coords, name=name, attrs=attrs
     )
     return cf_corrected
 
 
-def open_csv(path: Union[str, Path], cf_table: Optional[dict] = cmor) -> xr.DataArray:
+def open_csv(path: str | Path, cf_table: dict | None = cmor) -> xr.DataArray:
     """Extract daily HQ meteo data and convert to xr.DataArray with CF-Convention attributes."""
     meta, data = extract_daily(path)
     return to_cf(meta, data, cf_table)
```

### Comparing `miranda-0.4.0/miranda/convert/melcc.py` & `miranda-0.5.0/miranda/convert/melcc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+"""MELCC (Québec) Weather Stations data conversion module."""
 from __future__ import annotations
 
 import datetime as dt
 import logging.config
+import os
 import re
 import warnings
 from argparse import ArgumentParser
+from collections.abc import Sequence
 from io import StringIO
 from pathlib import Path
 from subprocess import run
-from typing import Sequence
+from typing import Any
 
 import numpy as np
 import pandas as pd
+import xarray
 import xarray as xr
 from xclim.core.formatting import update_history
 from xclim.core.units import convert_units_to, pint_multiply, str2pint
 
 from miranda import __version__
 from miranda.scripting import LOGGING_CONFIG
 
@@ -48,16 +52,26 @@
     "convert_mdb",
     "convert_snow_table",
     "concat",
     "convert_melcc_obs",
 ]
 
 
-def parse_var_code(vcode):
-    match = re.match(r"([^\d]*)(\d*)([abcfhqz])", vcode)
+def parse_var_code(vcode: str) -> dict[str, Any]:
+    """Parse variable code to generate metadata
+
+    Parameters
+    ----------
+    vcode: str
+
+    Returns
+    -------
+    dict[str, Any]
+    """
+    match = re.match(r"(\D*)(\d*)([abcfhqz])", vcode)
     if match is None:
         raise ValueError(f"Failed to parse variable {vcode}.")
     short_code, instrument, freq = match.groups()
     melcc_code = vcode[:2].upper() + vcode[2:-1].lower() + vcode[-1].upper()
     short_code = short_code[:2].upper() + short_code[2:].lower()
     return {
         "freq": frequencies[freq][0],
@@ -65,27 +79,38 @@
         # PI has different meanings, it's not just a different instrument.
         "var_name": short_code if short_code != "PI" else melcc_code[:-1],
         "instrument": np.int32(instrument),
         "melcc_code": melcc_code,
     }
 
 
-def list_tables(dbfile):
-    """List the tables of a MDB file."""
-    res = run(["mdb-tables", dbfile], capture_output=True, encoding="utf-8")
+def list_tables(db_file):
+    """List the tables of an MDB file."""
+    res = run(["mdb-tables", db_file], capture_output=True, encoding="utf-8")
     if res.returncode != 0:
         raise ValueError(
-            f"Calling mdb-tables on {dbfile} failed with code {res.returncode}: {res.stderr}"
+            f"Calling mdb-tables on {db_file} failed with code {res.returncode}: {res.stderr}"
         )
     return res.stdout.lower().strip().split()
 
 
-def read_table(dbfile, table):
+def read_table(db_file: str | os.PathLike, tab: str | os.PathLike) -> xarray.Dataset:
+    """Read a MySQL table into an xarray object.
+
+    Parameters
+    ----------
+    db_file: str or os.PathLike
+    tab : str or os.PathLike
+
+    Returns
+    -------
+    xarray.Dataset
+    """
     res = run(
-        ["mdb-export", "-T", "%Y-%m-%dT%H:%M:%S", dbfile, table.upper()],
+        ["mdb-export", "-T", "%Y-%m-%dT%H:%M:%S", db_file, tab.upper()],
         capture_output=True,
         encoding="utf-8",
         check=True,
     )
     df = (
         pd.read_csv(
             StringIO(res.stdout),
@@ -103,23 +128,33 @@
         )
         .drop(columns=["STATUT_APPROBATION"])  # I don't know what this is...
         .set_index(["station", "time"])
     )
     NaT = df.index.get_level_values("time").isnull().sum()
     if NaT > 0:
         logger.warning(
-            f"{NaT} values dropped because of unparsable timestamps (probably data from before 1900)."
+            f"{NaT} values dropped because of unparseable timestamps (probably data from before 1900)."
         )
         df = df[df.index.get_level_values("time").notnull()]
     return df[~df.index.duplicated()].to_xarray()
 
 
-def read_stations(dbfile):
+def read_stations(db_file: str | os.PathLike) -> pd.DataFrame:
+    """Read station file using mdbtools.
+
+    Parameters
+    ----------
+    db_file: str or os.PathLike
+
+    Returns
+    -------
+    pandas.DataFrame
+    """
     res = run(
-        ["mdb-export", "-T", "%Y-%m-%dT%H:%M:%S", dbfile, "STATIONs"],
+        ["mdb-export", "-T", "%Y-%m-%dT%H:%M:%S", db_file, "STATIONs"],
         capture_output=True,
         encoding="utf-8",
         check=True,
     )
     df = pd.read_csv(
         StringIO(res.stdout),
         parse_dates=["Date_Ouverture", "Date_Fermeture"],
@@ -150,15 +185,25 @@
     da["station_name"] = da["station_name"].astype(str)
     da["station_type"] = da["station_type"].astype(str)
     da.station_opening.attrs.update(description="Date of station creation.")
     da.station_closing.attrs.update(description="Date of station closure.")
     return da.isel(station=~da.indexes["station"].duplicated())
 
 
-def read_definitions(dbfile):
+def read_definitions(dbfile: str):
+    """Read variable definition file using mdbtools.
+
+    Parameters
+    ----------
+    dbfile: str
+
+    Returns
+    -------
+    pandas.DataFrame
+    """
     res = run(
         ["mdb-export", dbfile, "DDs"],
         capture_output=True,
         encoding="utf-8",
         check=True,
     )
     definitions = (
@@ -182,49 +227,63 @@
 
 def convert_mdb(
     database: str | Path,
     stations: xr.Dataset,
     definitions: xr.Dataset,
     output: str | Path,
     overwrite: bool = True,
-):
-    outs = {}
+) -> dict[tuple[str, str], Path]:
+    """Convert microsoft databases of MELCC observation data to xarray objects.
+
+    Parameters
+    ----------
+    database: str or Path
+    stations
+    definitions
+    output
+    overwrite
+
+    Returns
+    -------
+    dict[tuple[str, str], Path]
+    """
+    outs = dict()
     tables = list_tables(database)
-    for table in tables:
-        if table.startswith("gdb") or table.startswith("~"):
+    for tab in tables:
+        if table.startswith("gdb") or tab.startswith("~"):
             continue
-        logger.info(f"Parsing {database}:{table}.")
-        meta = parse_var_code(table)
+        logger.info(f"Parsing {database}:{tab}.")
+        meta = parse_var_code(tab)
         code = meta["melcc_code"]
         existing = list(output.glob(f"*_{code}_MELCC_{meta['freq']}_*.nc"))
         if existing and not overwrite:
             if len(existing) > 1:
                 raise ValueError(f"Found more than one existing file for table {code}!")
             file = existing[0]
             vname = file.stem.split(code)[0][:-1]
             logger.info(f"File already exists {file}, skipping.")
             outs[(vname, code)] = file
             continue
-        raw = read_table(database, table)
+        raw = read_table(database, tab)
         if np.prod(list(raw.dims.values())) == 0:
             # If any dimension is 0.
             logger.warning("The table is empty.")
             continue
         vv = meta.pop("var_name")
 
-        raw = raw.rename({table: vv, f"{table}_flag": f"{vv}_flag"})
+        raw = raw.rename({tab: vv, f"{tab}_flag": f"{vv}_flag"})
         raw.attrs["frequency"] = meta.pop("freq")
         raw[vv].attrs.update(**meta)
 
-        if table.lower() not in definitions.index:
+        if tab.lower() not in definitions.index:
             warnings.warn(
                 f"The {code} variable wasn't defined in the definition table."
             )
         else:
-            dd = definitions.loc[table]
+            dd = definitions.loc[tab]
             raw[vv].attrs.update(**dd)
 
         raw[f"{vv}_flag"] = raw[f"{vv}_flag"].fillna(0).astype(np.int32)
         raw[f"{vv}_flag"].attrs.update(
             standard_name="status_flag",
             flag_values=np.array([0, 1, 3, 5, 7], dtype="int32"),
             flag_meanings="nodata good estimated forced trace",
@@ -246,29 +305,42 @@
 
         ds = dataset_corrections(raw, "melcc-obs")
         new_var_name = list(
             filter(lambda k: not k.endswith("_flag"), ds.data_vars.keys())
         )[0]
         ds.attrs[
             "history"
-        ] = f"[{dt.datetime.now():%Y-%m-%d %H:%M:%S}] Conversion from {database.name}:{table} to netCDF."
+        ] = f"[{dt.datetime.now():%Y-%m-%d %H:%M:%S}] Conversion from {database.name}:{tab} to netCDF."
         date = "-".join(ds.indexes["time"][[0, -1]].strftime("%Y%m"))
         outs[(new_var_name, code)] = (
             output / f"{new_var_name}_{code}_MELCC_{raw.attrs['frequency']}_{date}.nc"
         )
         ds.to_netcdf(outs[(new_var_name, code)])
     return outs
 
 
 def convert_melcc_obs(
     metafile: str | Path,
     folder: str | Path,
     output: str | Path | None = None,
     overwrite: bool = True,
-):
+) -> dict[tuple[str, str], Path]:
+    """Convert MELCC observation data to xarray data objects, returning paths.
+
+    Parameters
+    ----------
+    metafile: str or Path
+    folder: str or Path
+    output: str or Path, optional
+    overwrite: bool
+
+    Returns
+    -------
+    dict[str, Path]
+    """
     output = Path(output or ".")
 
     stations = read_stations(metafile)
     definitions = read_definitions(metafile)
 
     logger.info("Parsing databases.")
     folder = Path(folder)
@@ -276,15 +348,27 @@
     for database in folder.glob("*.mdb"):
         outs.update(convert_mdb(database, stations, definitions, output, overwrite))
     return outs
 
 
 def concat(
     files: Sequence[str | Path], output_folder: str | Path, overwrite: bool = True
-):
+) -> Path:
+    """Concatenate converted weather station files.
+
+    Parameters
+    ----------
+    files: sequence of str or Path
+    output_folder: str or Path
+    overwrite: bool
+
+    Returns
+    -------
+    Path
+    """
     *vv, _, melcc, freq, _ = Path(files[0]).stem.split("_")
     vv = "_".join(vv)
     logger.info(f"Concatening variables from {len(files)} files ({vv}).")
     # Magic one-liner to parse all date_start and date_end entries from the file names.
     dates_start, dates_end = list(
         zip(*[map(int, Path(file).stem.split("_")[-1].split("-")) for file in files])
     )
@@ -292,15 +376,15 @@
         Path(output_folder)
         / f"{vv}_{melcc}_{freq}_{min(dates_start):06d}-{max(dates_end):06d}.nc"
     )
     if outpath.is_file() and not overwrite:
         logger.info(f"Already done in {outpath}. Skipping.")
         return outpath
 
-    dss = {}
+    dss = dict()
     for i, file in enumerate(files):
         ds = xr.open_dataset(file, chunks={"time": 1000})
         for crd in ds.coords.values():
             crd.load()
         if list(sorted(ds.data_vars.keys())) != [vv, f"{vv}_flag"]:
             raise ValueError(
                 f"Unexpected variables in {file}. Got {ds.data_vars.keys()}, expected {vv} and {vv}_flag."
@@ -489,15 +573,16 @@
         ds[[vv, f"{vv}_flag"]].to_netcdf(
             output / f"{vv}_{ds[vv].melcc_code}_MELCC_2sem_{date}.nc"
         )
 
 
 if __name__ == "__main__":
     argparser = ArgumentParser(
-        description="Convert MS Access data to netCDF. Requires mdbtools to be installed. By default, a single netCDF is created for each data table."
+        description="Convert MS Access data to netCDF. Requires mdbtools to be installed. "
+        "By default, a single netCDF is created for each data table."
     )
     argparser.add_argument(
         "-v", "--verbose", help="Increase verbosity of the script.", action="store_true"
     )
     argparser.add_argument(
         "-c",
         "--concat",
@@ -525,24 +610,24 @@
         "folder", help="Path to a folder including many *.mdb files to convert."
     )
     args = argparser.parse_args()
 
     if args.verbose:
         logging.basicConfig(level=logging.DEBUG)
 
-    outs = convert_melcc_obs(
+    outputs = convert_melcc_obs(
         args.metafile,
         args.folder,
         output=args.raw_output or args.output,
         overwrite=not args.skip_existing,
     )
 
     if args.concat:
         new_vars = {}
-        for (new_var, table), path in outs.items():
+        for (new_var, table), path in outputs.items():
             new_vars.setdefault(new_var, []).append(path)
 
-        for new_var, files in new_vars.items():
+        for new_var, fichiers in new_vars.items():
             try:
-                concat(files, args.output, overwrite=not args.skip_existing)
+                concat(fichiers, args.output, overwrite=not args.skip_existing)
             except Exception as err:
                 logger.error(err)
```

### Comparing `miranda-0.4.0/miranda/convert/utils.py` & `miranda-0.5.0/miranda/convert/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,33 @@
+"""Conversion Utilities submodule."""
+from __future__ import annotations
+
 import hashlib
 import logging.config
 import os
 import re
 from pathlib import Path
-from typing import Dict, Union
 
 import cftime
 import pandas as pd
 from pandas._libs import NaTType  # noqa
 
 from miranda.scripting import LOGGING_CONFIG
 
 logging.config.dictConfig(LOGGING_CONFIG)
 
 __all__ = ["find_version_hash", "date_parser"]
 
 
-def find_version_hash(file: Union[os.PathLike, str]) -> Dict:
-    """
+def find_version_hash(file: os.PathLike | str) -> dict:
+    """Check for an existing version hash file and, if one cannot be found, generate one from file.
 
     Parameters
     ----------
-    file : Path or str
+    file : str or os.PathLike
 
     Returns
     -------
     dict
     """
 
     def _get_hash(f):
@@ -64,15 +66,15 @@
 
 def date_parser(
     date: str,
     *,
     end_of_period: bool = False,
     output_type: str = "str",
     strftime_format: str = "%Y-%m-%d",
-) -> Union[str, pd.Timestamp, NaTType]:
+) -> str | pd.Timestamp | NaTType:
     """Parses datetime objects from a string representation of a date or both a start and end date.
 
     Parameters
     ----------
     date : str
         Date to be converted.
     end_of_period : bool
@@ -87,15 +89,14 @@
     pd.Timestamp or str or pd.NaT
         Parsed date.
 
     Notes
     -----
     Adapted from code written by Gabriel Rondeau-Genesse (@RondeauG)
     """
-
     # Formats, ordered depending on string length
     formats = {
         4: ["%Y"],
         6: ["%Y%m"],
         7: ["%Y-%m"],
         8: ["%Y%m%d"],
         10: ["%Y%m%d%H", "%Y-%m-%d"],
```

### Comparing `miranda-0.4.0/miranda/cv.py` & `miranda-0.5.0/miranda/cv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""Controlled Vocabulary module."""
+from __future__ import annotations
+
 import warnings
 
 from miranda.utils import HiddenPrints
 
 with HiddenPrints():
     try:
         import pyessv
```

### Comparing `miranda-0.4.0/miranda/data.py` & `miranda-0.5.0/miranda/data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,35 @@
+"""Database Management module."""
+from __future__ import annotations
+
 import logging.config
 import os
 from pathlib import Path
 from types import GeneratorType
-from typing import List, Optional, Tuple, Union
 
-from .io._input import find_filepaths
+from .io import find_filepaths
 from .scripting import LOGGING_CONFIG
 from .units import GiB
 from .validators import url_validate
 
 logging.config.dictConfig(LOGGING_CONFIG)
 
 __all__ = ["DataBase"]
 
 
 class DataBase:
-    """ """
+    """Database management class."""
 
     def __init__(
         self,
         source,
         *,
-        destination: Optional[Union[Path, str]] = None,
-        common_path: Optional[Union[Path, str]] = None,
-        file_pattern: Union[str, List[str]] = "*.nc",
+        destination: Path | str | None = None,
+        common_path: Path | str | None = None,
+        file_pattern: str | list[str] = "*.nc",
         project_name: str = None,
         recursive: bool = True,
     ):
         self._source = Path(source)
 
         if destination is not None:
             self._destination = Path(destination)
@@ -39,15 +41,15 @@
             self.project_name = self._destination.stem
 
         if not file_pattern:
             self.file_suffixes = ["*"]
 
         elif isinstance(file_pattern, str):
             self.file_suffixes = [file_pattern]
-        elif isinstance(file_pattern, (GeneratorType, List)):
+        elif isinstance(file_pattern, (GeneratorType, list)):
             self.file_suffixes = file_pattern
 
         if not recursive:
             self.recursive = False
         else:
             self.recursive = True
 
@@ -56,41 +58,48 @@
 
         self._files = self._scrape(source)
         self._is_server = False
 
         self.successful_transfers = int(0)
 
     def __repr__(self):
+        """Repl function."""
         return "<{}.{} object at {}>".format(
             self.__class__.__module__, self.__class__.__name__, hex(id(self))
         )
 
     def __str__(self):
+        """String function."""
         prepr = "[%s]" % ", ".join([f'{k}: "{v}"' for k, v in self.__dict__.items()])
         return f"{self.__class__.__name__}({prepr})"
 
     def __getitem__(self, key):
+        """Getter."""
         return self.__dict__[key]
 
     def __setitem__(self, key, value):
+        """Setter."""
         self.__dict__[key] = value
 
     def __delitem__(self, key):
+        """Delete item."""
         del self.__dict__[key]
 
     def __contains__(self, key):
+        """Contains function."""
         return key in self.__dict__
 
     def __len__(self):
+        """Length."""
         return len(self._files)
 
-    def _scrape(self, source) -> List[Path]:
+    def _scrape(self, source) -> list[Path]:
         if source is None:
             raise ValueError("No source provided.")
-        if isinstance(source, (GeneratorType, List, Tuple, str, Path)):
+        if isinstance(source, (GeneratorType, list, tuple, str, Path)):
             files = find_filepaths(source, **self._as_dict())
             common_path = os.path.commonpath(files)
             self._files = files
             self._common_path = common_path
             return files
         raise ValueError("Source must be an iterable of strings or Paths.")
 
@@ -98,47 +107,60 @@
         return {
             key: value
             for key, value in self.__dict__.items()
             if not key.startswith("_") and not callable(key)
         }
 
     def items(self):
+        """Show items."""
         return self._as_dict().items()
 
     def keys(self):
+        """Show keys."""
         return self._as_dict().keys()
 
     def values(self):
+        """Show values."""
         return self._as_dict().values()
 
     def group_by(
         self,
         *,
-        common_path: Union[Path, str] = None,
+        common_path: Path | str = None,
         subdirectories: bool = True,
         dates: bool = True,
         size: int = 10 * GiB,
     ):
+        """Grouping meta-function.
+
+        Notes
+        -----
+        Not yet implemented.
+
+        """
         # use_grouping = True
         #
         # if subdirectories:
         #     file_groups = group_by_subdirectories(self._files, within=common_path)
         #
         # else:
         #     file_groups = defaultdict(lambda: list())
         #     for f in self._files:
         #         file_groups["."].append(f)
         pass
 
-    def target(self, target: Union[Path, str]):
+    def target(self, target: Path | str):
+        """Target directory or server address."""
         self._destination = target
         self._is_server = self._url_validate(target=target)
 
     @staticmethod
     def _url_validate(target):
         return url_validate(target=target)
 
     def archive(self):
+        """Not yet implemented."""
         pass
 
     def transfer(self):
+        """Not yet implemented."""
         pass
```

### Comparing `miranda-0.4.0/miranda/decode/_decoder.py` & `miranda-0.5.0/miranda/decode/_decoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from __future__ import annotations
+
 import logging
 import multiprocessing as mp
 import os
 import re
 import warnings
 from functools import partial
 from logging import config
 from os import PathLike
 from pathlib import Path
 from types import GeneratorType
-from typing import Dict, List, Optional, Union
 
 import netCDF4 as nc  # noqa
 import pandas as pd
 import schema
 import xarray as xr
 import zarr
 from pandas._libs.tslibs import NaTType  # noqa
@@ -22,26 +23,26 @@
 from miranda.scripting import LOGGING_CONFIG
 from miranda.units import get_time_frequency
 
 from ._time import TIME_UNITS_TO_FREQUENCY, TIME_UNITS_TO_TIMEDELTA, DecoderError
 
 if VALIDATION_ENABLED:
     from miranda.cv import INSTITUTIONS, PROJECT_MODELS
-    from miranda.validators import FACETS_SCHEMA
+    from miranda.validators import FACETS_SCHEMA  # noqa
 
 
 config.dictConfig(LOGGING_CONFIG)
 
 __all__ = [
     "Decoder",
     "guess_project",
 ]
 
 
-def guess_project(file: Union[os.PathLike, str]) -> str:
+def guess_project(file: os.PathLike | str) -> str:
     """Guess the name of the project
 
     Parameters
     ----------
     file : str or os.PathLike
 
     Returns
@@ -62,25 +63,25 @@
 
 
 class Decoder:
     project = None
     guess = False
     _file_facets = dict()
 
-    def __init__(self, project: Optional[str]):
+    def __init__(self, project: str | None):
         self.project = project
 
     @staticmethod
     def _decoder(
-        d: Dict,
+        d: dict,
         fail_early: bool,
         proj: str,
         guess: bool,
         lock: mp.Lock,
-        file: Union[str, Path],
+        file: str | Path,
     ) -> None:
         if proj is None:
             if guess:
                 try:
                     proj = guess_project(file)
                 except DecoderError:
                     print(
@@ -113,69 +114,71 @@
             print(f"Unable to read data from {Path(file)}. Ensure pathname is correct.")
             raise
         except schema.SchemaError as e:
             print(f"Decoded facets from {Path(file).name} are not valid: {e}")
 
     def decode(
         self,
-        files: Union[os.PathLike, str, List[Union[str, os.PathLike]], GeneratorType],
-        chunks: Optional[int] = None,
+        files: os.PathLike | str | list[str | os.PathLike] | GeneratorType,
+        chunks: int | None = None,
         raise_error: bool = False,
     ) -> None:
         """Decode facets from file or list of files.
 
         Parameters
         ----------
-        files: Union[str, Path, List[Union[str, Path]]]
-        chunks: int, optional
-        raise_error: bool
+        files : str or Path or list of str or Path or generator
+        chunks : int, optional
+            The chunk size used when processing files. Not to be confused with xarray chunks for dimensions.
+        raise_error : bool
         """
         if isinstance(files, (str, os.PathLike)):
             files = [files]
 
-        if chunks is None:
-            if isinstance(files, list):
-                if len(files) >= 10:
-                    chunk_size = 10
-                else:
-                    chunk_size = len(files)
-            else:
+        if chunks is None and isinstance(files, list):
+            if len(files) >= 10:
                 chunk_size = 10
+            elif 1 <= len(files) < 10:
+                chunk_size = len(files)
+            else:
+                raise ValueError("No file entries found.")
+        elif isinstance(files, GeneratorType):
+            chunk_size = 10
         else:
             chunk_size = chunks
 
         if self.project is None:
             warnings.warn(
                 "The decoder 'project' is not set; Decoding step will be much slower."
             )
         else:
             logging.info(f"Deciphering metadata with project = '{self.project}'")
 
-        manager = mp.Manager()
-        _file_facets = manager.dict()
-        lock = manager.Lock()
-        func = partial(
-            self._decoder, _file_facets, raise_error, self.project, self.guess, lock
-        )
+        with mp.Manager() as manager:
+            _file_facets = manager.dict()
+            lock = manager.Lock()
+            func = partial(
+                self._decoder, _file_facets, raise_error, self.project, self.guess, lock
+            )
 
-        with mp.Pool() as pool:
-            pool.imap(func, files, chunksize=chunk_size)
-            pool.close()
-            pool.join()
+            with mp.Pool() as pool:
+                pool.imap(func, files, chunksize=chunk_size)
+                pool.close()
+                pool.join()
 
-        self._file_facets.update(_file_facets)
+            self._file_facets.update(_file_facets)
 
     def facets_table(self):
         raise NotImplementedError()
 
-    def file_facets(self) -> Dict[os.PathLike, Dict]:
+    def file_facets(self) -> dict[os.PathLike, dict]:
         return self._file_facets
 
     @classmethod
-    def _from_dataset(cls, file: Union[Path, str]) -> (str, str, Dict):
+    def _from_dataset(cls, file: Path | str) -> (str, str, dict):
         file_name = Path(file).stem
 
         try:
             variable_name = cls._decode_primary_variable(file)
         except DecoderError:
             logging.error(f"Unable to open dataset: {file.name}")
             raise
@@ -239,15 +242,15 @@
             else:
                 raise NotImplementedError()
         except ValueError:
             raise DecoderError()
 
     @staticmethod
     def _decode_hour_of_day_info(
-        file: Union[PathLike, str],
+        file: PathLike | str,
     ) -> dict:
         """
 
         Parameters
         ----------
         file : Path or str
 
@@ -278,25 +281,25 @@
             return dict()
 
         else:
             raise NotImplementedError()
 
     @staticmethod
     def _decode_time_info(
-        file: Optional[Union[PathLike, str, List[str]]] = None,
-        data: Optional[Dict] = None,
-        term: Optional[str] = None,
+        file: PathLike | str | list[str] | None = None,
+        data: dict | None = None,
+        term: str | None = None,
         *,
         field: str = None,
-    ) -> Union[str, NaTType]:
+    ) -> str | NaTType:
         """
 
         Parameters
         ----------
-        file : Union[os.PathLike, str], optional
+        file : os.PathLike or str, optional
         data : dict, optional
         term : str
         field : {"timedelta", "frequency"}
 
         Returns
         -------
         str or NaTType
@@ -446,20 +449,20 @@
                     "Time frequency found in dataset on analysis was not found in filename. "
                     f"Basing fields on `{found_freq}`."
                 )
                 return time_dictionary[found_freq]
         raise DecoderError(f"Time frequency indiscernible for file `{file}`.")
 
     @staticmethod
-    def _decode_version(file: Union[PathLike, str], data: Dict) -> dict:
+    def _decode_version(file: PathLike | str, data: dict) -> dict:
         """
 
         Parameters
         ----------
-        file: Union[os.PathLike, str]
+        file: os.PathLike or str
         data: dict
 
         Returns
         -------
         dict
         """
         version_info = dict()
@@ -480,15 +483,15 @@
                         version_info["sha256sum"] = sig.open().read()
                         break
                 else:
                     version_info["version"] = "vNotFound"
         return version_info
 
     @classmethod
-    def decode_converted(cls, file: Union[PathLike, str]) -> dict:
+    def decode_converted(cls, file: PathLike | str) -> dict:
         facets = dict()
         try:
             variable, date, data = cls._from_dataset(file=file)
         except DecoderError:
             return facets
 
         facets.update(data)
@@ -522,27 +525,27 @@
             facets["date_end"] = date_parser(date, end_of_period=True)
         except DecoderError:
             pass
 
         return facets
 
     @staticmethod
-    def decode_eccc_obs(self, file: Union[PathLike, str]) -> Dict:
+    def decode_eccc_obs(self, file: PathLike | str) -> dict:
         raise NotImplementedError()
 
     @staticmethod
-    def decode_ahccd_obs(self, file: Union[PathLike, str]) -> Dict:
+    def decode_ahccd_obs(self, file: PathLike | str) -> dict:
         raise NotImplementedError()
 
     @staticmethod
-    def decode_melcc_obs(self, file: Union[PathLike, str]) -> Dict:
+    def decode_melcc_obs(self, file: PathLike | str) -> dict:
         raise NotImplementedError()
 
     @classmethod
-    def decode_pcic_candcs_u6(cls, file: Union[PathLike, str]) -> dict:
+    def decode_pcic_candcs_u6(cls, file: PathLike | str) -> dict:
         if "Derived" in Path(file).parents:
             raise NotImplementedError("Derived CanDCS-U6 variables are not supported.")
 
         facets = dict()
         try:
             variable, date, data = cls._from_dataset(file=file)
         except DecoderError:
@@ -585,15 +588,15 @@
             facets["date_end"] = date_parser(date, end_of_period=True)
         except DecoderError:
             pass
 
         return facets
 
     @classmethod
-    def decode_cmip6(cls, file: Union[PathLike, str]) -> dict:
+    def decode_cmip6(cls, file: PathLike | str) -> dict:
         facets = dict()
         try:
             variable, date, data = cls._from_dataset(file=file)
         except DecoderError:
             return facets
 
         facets["activity"] = data["activity_id"]
@@ -624,15 +627,15 @@
             facets["date_end"] = date_parser(date, end_of_period=True)
         except DecoderError:
             pass
 
         return facets
 
     @classmethod
-    def decode_cmip5(cls, file: Union[PathLike, str]) -> dict:
+    def decode_cmip5(cls, file: PathLike | str) -> dict:
         facets = dict()
         try:
             variable, date, data = cls._from_dataset(file=file)
         except DecoderError:
             return facets
 
         facets["activity"] = "CMIP"
@@ -662,15 +665,15 @@
             facets["date_end"] = date_parser(date, end_of_period=True)
         except DecoderError:
             pass
 
         return facets
 
     @classmethod
-    def decode_cordex(cls, file: Union[PathLike, str]) -> dict:
+    def decode_cordex(cls, file: PathLike | str) -> dict:
         facets = dict()
         try:
             variable, date, data = cls._from_dataset(file=file)
         except DecoderError:
             return dict()
 
         # FIXME: What to do about our internal data that breaks all established conventions?
@@ -796,15 +799,15 @@
                 raise KeyError()
         except KeyError:
             facets["member"] = data["driving_model_ensemble_member"].strip()
 
         return facets
 
     @classmethod
-    def decode_isimip_ft(cls, file: Union[PathLike, str]) -> dict:
+    def decode_isimip_ft(cls, file: PathLike | str) -> dict:
         facets = dict()
         try:
             variable, date, data = cls._from_dataset(file=file)
         except DecoderError:
             return facets
 
         facets["activity"] = "ISIMIP"
@@ -831,9 +834,129 @@
             facets["timedelta"] = cls._decode_time_info(
                 term=facets["frequency"], field="timedelta"
             )
             facets["date_start"] = date_parser(date)
             facets["date_end"] = date_parser(date, end_of_period=True)
         except DecoderError:
             pass
+
+        return facets
+
+    @classmethod
+    def decode_nex_gddp_cmip6(cls, file: PathLike | str) -> dict:
+        facets = dict()
+        try:
+            variable, date, data = cls._from_dataset(file=file)
+        except DecoderError:
+            return facets
+
+        facets["experiment"] = data["scenario"]
+        facets["activity"] = (
+            "CMIP" if facets["experiment"] == "historical" else "ScenarioMIP"
+        )
+        facets["institution"] = data["cmip6_institution_id"]
+        facets["member"] = data["variant_label"]
+        facets["processing_level"] = "biasadjusted"
+        facets["bias_adjust_project"] = "NEX-GDDP-CMIP6"
+        facets["bias_adjust_institution"] = "NASA"
+        facets["mip_era"] = "CMIP6"
+        facets["source"] = data["cmip6_source_id"]
+        facets["type"] = "simulation"
+        facets["variable"] = variable
+        facets.update(cls._decode_version(data=data, file=file))
+        facets.update(cls._decode_hour_of_day_info(file=file))
+
+        try:
+            facets["frequency"] = cls._decode_time_info(
+                data=data, file=file, field="frequency"
+            )
+            facets["timedelta"] = cls._decode_time_info(
+                term=facets["frequency"], field="timedelta"
+            )
+            facets["date_start"] = date_parser(date)
+            facets["date_end"] = date_parser(date, end_of_period=True)
+        except DecoderError:
+            pass
+
+        return facets
+
+    @classmethod
+    def decode_espo_g6_r2(cls, file: PathLike | str) -> dict:
+        facets = dict()
+        try:
+            variable, date, data = cls._from_dataset(file=file)
+        except DecoderError:
+            return facets
+
+        facets["bias_adjust_project"] = "ESPO-G6-R2"
+        facets["processing_level"] = "biasadjusted"
+        facets["version"] = "1.0.0"
+        facets["domain"] = "NAM"
+        for f in [
+            "experiment",
+            "activity",
+            "institution",
+            "member",
+            "bias_adjust_institution",
+            "mip_era",
+            "source",
+            "type",
+        ]:
+            facets[f] = data[f"cat:{f}"]
+        facets["variable"] = variable
+        # facets.update(cls._decode_version(data=data, file=file))
+        facets.update(cls._decode_hour_of_day_info(file=file))
+
+        try:
+            facets["frequency"] = cls._decode_time_info(
+                data=data, file=file, field="frequency"
+            )
+            facets["timedelta"] = cls._decode_time_info(
+                term=facets["frequency"], field="timedelta"
+            )
+            facets["date_start"] = date_parser(date)
+            facets["date_end"] = date_parser(date, end_of_period=True)
+        except DecoderError:
+            pass
+
+        return facets
+
+    @classmethod
+    def decode_espo_g6_e5l(cls, file: PathLike | str) -> dict:
+        facets = dict()
+        try:
+            variable, date, data = cls._from_dataset(file=file)
+        except DecoderError:
+            return facets
+
+        facets["bias_adjust_project"] = "ESPO-G6-E5L"
+        facets["processing_level"] = "biasadjusted"
+        facets["version"] = "1.0.0"
+        facets["domain"] = "NAM"
+        for f in [
+            "experiment",
+            "activity",
+            "institution",
+            "member",
+            "bias_adjust_institution",
+            "mip_era",
+            "source",
+            "type",
+        ]:
+            facets[f] = data[f"cat:{f}"]
+        facets["variable"] = variable
+        # facets.update(cls._decode_version(data=data, file=file))
+        facets.update(cls._decode_hour_of_day_info(file=file))
+
+        try:
+            facets["frequency"] = cls._decode_time_info(
+                data=data, file=file, field="frequency"
+            )
+            facets["timedelta"] = cls._decode_time_info(
+                term=facets["frequency"], field="timedelta"
+            )
+            facets["date_start"] = date_parser(date)
+            facets["date_end"] = date_parser(date, end_of_period=True)
+        except DecoderError:
+            pass
 
         return facets
```

### Comparing `miranda-0.4.0/miranda/decode/_time.py` & `miranda-0.5.0/miranda/decode/_time.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 from logging import config
 
 from pandas._libs.tslibs import NaTType  # noqa
 
 from miranda.scripting import LOGGING_CONFIG
```

### Comparing `miranda-0.4.0/miranda/eccc/_homogenized.py` & `miranda-0.5.0/miranda/eccc/_homogenized.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,49 @@
+"""Adjusted and Homogenized Canadian Clime Data module."""
+from __future__ import annotations
+
 import calendar
 import logging.config
 from pathlib import Path
-from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 from dask.diagnostics import ProgressBar
 
 from miranda.scripting import LOGGING_CONFIG
 
 from ._utils import cf_ahccd_metadata
 
 logging.config.dictConfig(LOGGING_CONFIG)
-
 logger = logging.Logger("miranda")
 
 __all__ = ["convert_ahccd", "convert_ahccd_fwf_files"]
 
 
 def convert_ahccd(
-    data_source: Union[str, Path],
-    output_dir: Union[str, Path],
+    data_source: str | Path,
+    output_dir: str | Path,
     variable: str,
-    generation: Optional[int] = None,
-):
-    output_dir = Path(output_dir).expanduser().joinpath(variable)
+    generation: int | None = None,
+) -> None:
+    """Convert Adjusted and Homogenized Canadian Climate Dataset files.
+
+    Parameters
+    ----------
+    data_source: str or Path
+    output_dir: str or Path
+    variable: str
+    generation: int, optional
+
+    Returns
+    -------
+    None
+    """
+    output_dir = Path(output_dir).resolve().joinpath(variable)
     output_dir.mkdir(parents=True, exist_ok=True)
 
     code = dict(tasmax="dx", tasmin="dn", tas="dm", pr="dt", prsn="ds", prlp="dr").get(
         variable
     )
     var, col_names, col_spaces, header_row, global_attrs = cf_ahccd_metadata(
         code, generation
@@ -38,15 +52,15 @@
     if generation == 3 and code in {"dx", "dn", "dm"}:
         meta = "ahccd_gen3_temperature.csv"
     elif generation == 2 and code in {"dt", "ds", "dr"}:
         meta = "ahccd_gen2_precipitation.csv"
 
     else:
         raise NotImplementedError(f"Code '{code} for generation {gen}.")
-    metadata_source = Path(__file__).parent.joinpath("data").joinpath(meta)
+    metadata_source = Path(__file__).resolve().parent.joinpath("data").joinpath(meta)
 
     if "tas" in variable:
         metadata = pd.read_csv(metadata_source, header=2)
         metadata.columns = col_names.keys()
         cols_specs = col_spaces
 
     elif "pr" in variable:
@@ -75,15 +89,15 @@
 
             if len(metadata_st) == 1:
                 ds_out = convert_ahccd_fwf_files(
                     ff, metadata_st, variable, generation, cols_specs, var
                 )
                 ds_out.attrs = global_attrs
 
-                ds_out.to_netcdf(outfile)
+                ds_out.to_netcdf(outfile, engine="h5netcdf")
             else:
                 logger.warning(
                     f"metadata info for station {ff.name} not found : skipping"
                 )
 
     # merge individual stations to single .nc file
     # variable
@@ -122,31 +136,48 @@
 
             for clean_name, orig_name in col_names.items():
                 if clean_name in ["lat", "long"]:
                     continue
                 ds_ahccd[clean_name].attrs["long_name"] = orig_name
 
             outfile.parent.mkdir(parents=True, exist_ok=True)
-            ds_ahccd.to_netcdf(outfile, format="NETCDF4_CLASSIC", mode="w")
+            ds_ahccd.to_netcdf(
+                outfile, engine="h5netcdf", format="NETCDF4_CLASSIC", mode="w"
+            )
 
             del ds_ahccd
     for nc in outfile.parent.glob("*.nc"):
         logger.info(nc)
         ds = xr.open_dataset(nc)
         logger.info(ds)
 
 
 def convert_ahccd_fwf_files(
-    ff,
-    metadata,
-    variable,
+    ff: Path | str,
+    metadata: pd.DataFrame,
+    variable: str,
     generation: int = None,
-    cols_specs: Optional[List[Tuple[int, int]]] = None,
-    attrs: Optional[dict] = None,
+    cols_specs: list[tuple[int, int]] | None = None,
+    attrs: dict | None = None,
 ) -> xr.Dataset:
+    """Convert AHCCD fixed-width files.
+
+    Parameters
+    ----------
+    ff: str or Path
+    metadata: pandas.DataFrame
+    variable: str
+    generation
+    cols_specs
+    attrs
+
+    Returns
+    -------
+    xarray.Dataset
+    """
     code = dict(tasmax="dx", tasmin="dn", tas="dm", pr="dt", prsn="ds", prlp="dr").get(
         variable
     )
 
     if attrs is None:
         attrs, _, _, _, _ = cf_ahccd_metadata(code, generation)
     if cols_specs is None:
```

### Comparing `miranda-0.4.0/miranda/eccc/_raw.py` & `miranda-0.5.0/miranda/eccc/_raw.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 #
 # 2) on scan les fichiers sources annuels en cherchant une variable et on sauve
 # ce qu'on trouve dans des fichiers netcdf. On applique aussi les flags
 # et on fait les changements d'unites
 #
 # obtenu via http://climate.weather.gc.ca/index_e.html en cliquant sur 'about the data'
 #######################################################################
+from __future__ import annotations
+
 import contextlib
 import functools
 import logging
 import multiprocessing as mp
 import os
 import re
 import sys
 import tempfile
 import time
 from calendar import monthrange
 from datetime import datetime as dt
 from logging import config
 from pathlib import Path
-from typing import List, Optional, Set, Union
 from urllib.error import HTTPError
 
 import dask.dataframe as dd
 import numpy as np
 import pandas as pd
 import xarray as xr
 from dask.diagnostics import ProgressBar
@@ -49,15 +50,15 @@
     "convert_flat_files",
     "merge_converted_variables",
 ]
 
 TABLE_DATE = dt.now().strftime("%d %B %Y")
 
 
-def load_station_metadata(meta: Union[str, os.PathLike]) -> xr.Dataset:
+def load_station_metadata(meta: str | os.PathLike) -> xr.Dataset:
     if meta:
         df_inv = pd.read_csv(meta, header=0)
     else:
         try:
             import geopandas as gpd
 
             station_metadata_url = "https://api.weather.gc.ca/collections/climate-stations/items?f=json&limit=15000000"
@@ -83,22 +84,22 @@
         )
     return ds.sel(time=~ds.get_index("time").duplicated())
 
 
 def _convert_station_file(
     fichier: Path,
     output_path: Path,
-    errored_files: List[Path],
+    errored_files: list[Path],
     mode: str,
     add_offset: float,
-    column_dtypes: List[str],
-    column_names: List[str],
+    column_dtypes: list[str],
+    column_names: list[str],
     long_name: str,
-    missing_flags: Set[str],
-    missing_values: Set[str],
+    missing_flags: set[str],
+    missing_values: set[str],
     nc_name: str,
     raw_units: str,
     units: str,
     scale_factor: float,
     standard_name: str,
     variable_code: str,
     **kwargs,
@@ -382,17 +383,17 @@
         if os.listdir(temp_folder):
             for temporary_file in Path(temp_folder).glob("*"):
                 if temporary_file in data_files:
                     temporary_file.unlink()
 
 
 def convert_flat_files(
-    source_files: Union[str, os.PathLike],
-    output_folder: Union[str, os.PathLike, List[Union[str, int]]],
-    variables: Union[str, int, List[Union[str, int]]],
+    source_files: str | os.PathLike,
+    output_folder: str | os.PathLike | list[str | int],
+    variables: str | int | list[str | int],
     mode: str = "hourly",
     n_workers: int = 4,
 ) -> None:
     """
 
     Parameters
     ----------
@@ -473,38 +474,38 @@
                 "Some files failed to be properly parsed:\n", ", ".join(errored_files)
             )
 
     logging.warning(f"Process completed in {time.time() - func_time:.2f} seconds")
 
 
 def aggregate_stations(
-    source_files: Optional[Union[str, os.PathLike]] = None,
-    output_folder: Optional[Union[str, os.PathLike]] = None,
+    source_files: str | os.PathLike | None = None,
+    output_folder: str | os.PathLike | None = None,
     time_step: str = None,
-    variables: Optional[Union[str, int, List[Union[str, int]]]] = None,
+    variables: str | int | list[str | int] | None = None,
     include_flags: bool = True,
-    groupings: Optional[int] = None,
-    mf_dataset_freq: Optional[str] = None,
-    temp_directory: Optional[Union[str, os.PathLike]] = None,
+    groupings: int | None = None,
+    mf_dataset_freq: str | None = None,
+    temp_directory: str | os.PathLike | None = None,
     n_workers: int = 1,
 ) -> None:
     """
 
     Parameters
     ----------
-    source_files: Union[str, Path]
-    output_folder: Union[str, Path]
-    variables: Optional[Union[str, int, List[Union[str, int]]]]
+    source_files: str or Path
+    output_folder: str or Path
+    variables: str or int or list of str or int, optional
     time_step: {"hourly", "daily"}
     include_flags: bool
     groupings: int
       The number of files in each group used for converting to multi-file Datasets.
-    mf_dataset_freq: Optional[str]
+    mf_dataset_freq: str, optional
       Resampling frequency for creating output multi-file Datasets. E.g. 'YS': 1 year per file, '5YS': 5 years per file.
-    temp_directory: Optional[Union[str, Path]]
+    temp_directory: str or Path, optional
       Use another temporary directory location in case default location is not spacious enough.
     n_workers: int
 
     Returns
     -------
     None
     """
@@ -684,27 +685,27 @@
 
 def _export_agg_nc(args):
     dataset, path = args
     comp = dict(zlib=True, complevel=5)
     encoding = {var: comp for var in dataset.data_vars}
     dataset.load().to_netcdf(
         path,
-        engine="netcdf4",
+        engine="h5netcdf",
         format="NETCDF4_CLASSIC",
         encoding=encoding,
     )
     dataset.close()
     del dataset
 
 
 def _tmp_zarr(
     iterable: int,
-    nc: List[Union[str, os.PathLike]],
-    tempdir: Union[str, os.PathLike],
-    group: Optional[int] = None,
+    nc: list[str | os.PathLike],
+    tempdir: str | os.PathLike,
+    group: int | None = None,
 ) -> None:
     logging.info(
         f"Processing batch of files {iterable + 1}"
         f"{' of ' + str(group) if group is not None else ''}."
     )
     station_file_codes = [Path(x).name.split("_")[0] for x in nc]
 
@@ -733,17 +734,17 @@
         )
     del ds
 
 
 def _combine_years(
     station_folder: str,
     varia: str,
-    out_folder: Union[str, os.PathLike],
-    meta_file: Union[str, os.PathLike],
-    rejected: List[str],
+    out_folder: str | os.PathLike,
+    meta_file: str | os.PathLike,
+    rejected: list[str],
     _verbose: bool = False,
 ) -> None:
     nc_files = sorted(list(Path(station_folder).glob("*.nc")))
     if len(nc_files):
         logging.info(
             f"Found {len(nc_files)} files for station code {Path(station_folder).name}."
         )
@@ -844,45 +845,44 @@
         logging.info(f"Merging to {outfile.name}")
         comp = dict(zlib=True, complevel=5)
         encoding = {data_var: comp for data_var in ds.data_vars}
         encoding["time"] = dict(dtype="single")
         with ProgressBar():
             ds.to_netcdf(
                 outfile,
-                engine="netcdf4",
-                format="NETCDF4",
+                engine="h5netcdf",
+                format="NETCDF4_CLASSIC",
                 encoding=encoding,
             )
     else:
         logging.info(f"Files exist for {outfile.name}. Continuing...")
 
 
 def merge_converted_variables(
-    source_files: Union[str, os.PathLike],
-    output_folder: Union[str, os.PathLike],
-    variables: Optional[Union[str, int, List[Union[str, int]]]] = None,
-    station_metadata: Optional[Union[str, os.PathLike]] = None,
+    source_files: str | os.PathLike,
+    output_folder: str | os.PathLike,
+    variables: str | int | list[str | int] | None = None,
+    station_metadata: str | os.PathLike | None = None,
     overwrite: bool = False,
     n_workers: int = 1,
 ) -> None:
     """
 
     Parameters
     ----------
-    source_files: Union[str, Path]
-    output_folder: Union[str, Path]
-    variables: Optional[Union[str, int, List[Union[str, int]]]]
-    station_metadata: Optional[Union[str, Path]]
+    source_files: str, Path
+    output_folder: str, Path
+    variables: str or int or list of str or int, optional
+    station_metadata: str or Path, optional
     overwrite: bool
     n_workers: int
 
     Returns
     -------
     None
-
     """
     meta = load_station_metadata(station_metadata)
     metadata_file = Path(tempfile.NamedTemporaryFile(suffix=".nc", delete=False).name)
     meta.to_netcdf(metadata_file)
 
     if isinstance(source_files, str):
         source_files = Path(source_files)
```

### Comparing `miranda-0.4.0/miranda/eccc/_summaries.py` & `miranda-0.5.0/miranda/eccc/_summaries.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 # then appends the data within a pandas Dataframe
 #
 # dly_to_netcdf takes that Dataframe and exports it to a netCDF. When possible,
 # the variables are converted to be compatible with CF-Convention. For example,
 # "Max Temp (°C)" is renamed "tasmax" and converted to °K.
 #
 #####################################################################
+from __future__ import annotations
+
 import json
 import logging
 from collections import defaultdict
+from collections.abc import Generator
 from logging import config
 from pathlib import Path
-from typing import Generator, List, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 
 from miranda.scripting import LOGGING_CONFIG
 
@@ -30,52 +32,55 @@
 eccc_metadata = json.load(
     open(Path(__file__).parent / "eccc_obs_summary_cf_attrs.json")
 )["variable_entry"]
 
 
 # Searches a location for the station data, then calls the needed scripts to read and assembles the data using pandas
 def extract_daily_summaries(
-    path_station: Union[Path, str], rm_flags: bool = False, file_suffix: str = ".csv"
+    path_station: Path | str, rm_flags: bool = False, file_suffix: str = ".csv"
 ) -> dict:
-    """
+    """Extract daily climate summaries from ECCC CSV files.
 
     Parameters
     ----------
-    path_station : Union[Path, str]
-      PathLike or str to the station's folder containing the csv files.
+    path_station : str or Path
+        PathLike or str to the station's folder containing the csv files.
     rm_flags : bool
-      Removes the 'Flag' and 'Quality' columns of the ECCC files.
+        Removes the 'Flag' and 'Quality' columns of the ECCC files.
     file_suffix : str
-      File suffixes used by the tabular data. Default: ".csv".
+        File suffixes used by the tabular data. Default: ".csv".
+
     Returns
     -------
     dict
-      dict containing the station metadata, as well as the data stored within a pandas Dataframe.
+        dict containing the station metadata, as well as the data stored within a pandas Dataframe.
     """
-
     # Find the CSV files
     if "*" not in file_suffix:
         file_suffix = f"*{file_suffix}"
     station_files = Path(path_station).rglob(file_suffix)
 
     # extract the .csv data
     stations = _read_multiple_daily_summaries(station_files, rm_flags=rm_flags)
 
     return stations
 
 
-# Uses xarray to transform the 'station' from find_and_extract_dly into a CF-Convention netCDF file
-def daily_summaries_to_netcdf(station: dict, path_output: Union[Path, str]) -> None:
-    """
+#
+def daily_summaries_to_netcdf(station: dict, path_output: Path | str) -> None:
+    """Convert daily climate summaries to NetCDF files.
+
+    Uses xarray to transform the 'station' from find_and_extract_dly into a CF-Convention netCDF file
 
     Parameters
     ----------
     station : dict
-      dict created by using find_and_extract_dly
-    path_output: Union[Path, str]
+        dict created by using find_and_extract_dly
+    path_output: str or Path
+        Output path.
 
     Returns
     -------
     None
     """
     # first, transform the Date/Time to a 'days since' format
     time = station["data"]["Date/Time"] - np.array(
@@ -178,33 +183,36 @@
 
 
 ##########################################
 # BELOW THIS POINT ARE UTILITY SCRIPTS
 ##########################################
 
 
-# This calls _read_single_eccc_dly and appends the data in a single Dict
+# This
 def _read_multiple_daily_summaries(
-    files: Union[List[Union[str, Path]], Generator[Path, None, None]],
+    files: list[str | Path] | Generator[Path, None, None],
     rm_flags: bool = False,
 ) -> dict:
     """
 
+    Notes
+    -----
+    This calls `_read_single_eccc_dly` and appends the data in a single Dict.
+
     Parameters
     ----------
-    files : List[Union[str, Path]]
-      A list of all the files to append.
+    files : list of str or Path, or Generator[Path]
+        A list of all the files to append.
     rm_flags : bool
-      Removes all the 'Flag' and 'Quality' columns of the ECCC files. Default: False.
+        Removes all the 'Flag' and 'Quality' columns of the ECCC files. Default: False.
 
     Returns
     -------
     dict
     """
-
     # Extract the data for each files
     all_stations = dict()
     station_data = list()
 
     file_list = [Path(f) for f in files]
     file_list.sort()
 
@@ -218,51 +226,58 @@
             station = pd.read_csv(summary)
             station_data.append(station)
 
         station_summary_full = pd.DataFrame(
             station_data
         )  # FIXME: Find the way to combine list of dataframes into one
 
-        # datafull = datafull.append(data, ignore_index=True)
-
         # change the Date/Time column to a datetime64 type
         station_summary_full["Date/Time"] = pd.to_datetime(
             station_summary_full["Date/Time"]
         )
 
         # if wanted, remove the quality and flag columns
-        # if rm_flags:
-        #     index_quality = [
-        #         i for i, s in enumerate(datafull.columns.values) if "Quality" in s
-        #     ]
-        #     datafull = datafull.drop(datafull.columns.values[index_quality], axis="columns")
-        #     index_flag = [i for i, s in enumerate(datafull.columns.values) if "Flag" in s]
-        #     datafull = datafull.drop(datafull.columns.values[index_flag], axis="columns")
+        if rm_flags:
+            index_quality = [
+                i
+                for i, s in enumerate(station_summary_full.columns.values)
+                if "Quality" in s
+            ]
+            station_summary_full = station_summary_full.drop(
+                station_summary_full.columns.values[index_quality], axis="columns"
+            )
+            index_flag = [
+                i
+                for i, s in enumerate(station_summary_full.columns.values)
+                if "Flag" in s
+            ]
+            station_summary_full = station_summary_full.drop(
+                station_summary_full.columns.values[index_flag], axis="columns"
+            )
 
         # combine everything in a single Dict
-        # station = station_meta
         all_stations[station_code] = station_summary_full
 
     return all_stations
 
 
-# This is the script that actually reads the CSV files.
-# The metadata are saved in a Dict, while the data is returned as a pandas Dataframe.
-# FIXME: Climate Services Canada has changed the way they store metadata -- No longer in CSV heading
-# FIXME: Mohammad feel free to remove this
-def _read_single_daily_summaries(file: Union[Path, str]) -> Tuple[dict, pd.DataFrame]:
-    """
+def _read_single_daily_summaries(file: str | Path) -> tuple[dict, pd.DataFrame]:
+    """Read station summary information from CSV header.
+
+    Notes
+    -----
+    Climate Services Canada has changed the way they store metadata and no longer store this infor in the CSV heading.
 
     Parameters
     ----------
-    file : Union[Path, str]
+    file : str or Path
 
     Returns
     -------
-    Tuple[dict, pd.DataFrame]
+    tuple[dict, pd.DataFrame]
     """
     # Read the whole file
     with open(file, encoding="utf-8-sig") as fi:
         lines = fi.readlines()
 
     # Find each element in the header
     search_header = [0] * 9
```

### Comparing `miranda-0.4.0/miranda/eccc/_support_rvt.py` & `miranda-0.5.0/miranda/eccc/_support_rvt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,41 @@
+from __future__ import annotations
+
 import datetime
 import re
 import urllib
 from pathlib import Path
-from typing import Optional, Union
 
 import pandas as pd
 
 "https://api.weather.gc.ca/collections/climate-daily/items?datetime=1840-03-01%2000:00:00/2021-06-02%2000:00:00&STN_ID=10761&f=json&limit=1500000&startindex=0"
 
 # TODO: Investigate the API definition: https://api.weather.gc.ca/collections/climate-hourly
 
 
 # FIXME: This function is a WIP - requires work.
 def gather_eccc_stations(
     timestep: str,
-    start_date: Optional[Union[datetime.datetime, str]] = None,
-    end_date: Optional[Union[datetime.datetime, str]] = None,
-    climate_id: Optional[str] = None,
+    start_date: datetime.datetime | str | None = None,
+    end_date: datetime.datetime | str | None = None,
+    climate_id: str | None = None,
 ) -> pd.DataFrame:
+    """Collect ECCC station data from the Environment and Climate Change Canada API.
+
+    Parameters
+    ----------
+    timestep : str
+    start_date : datetime.datetime or str, optional
+    end_date : datetime.datetime or str, optional
+    climate_id : str, optional
+
+    Returns
+    -------
+    pandas.DataFrame
+    """
     if timestep.lower() in ["hourly", "daily"]:
         base_url = f"https://api.weather.gc.ca/collections/climate-{timestep}/"
     else:
         raise ValueError(timestep)
 
     dates = [start_date, end_date]
     for i, date in enumerate(dates):
```

### Comparing `miranda-0.4.0/miranda/eccc/_utils.py` & `miranda-0.5.0/miranda/eccc/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
+from __future__ import annotations
+
 import logging.config
+from collections.abc import Mapping
 from datetime import datetime as dt
-from typing import Dict, List, Mapping, Tuple, Union
 
 from miranda.scripting import LOGGING_CONFIG
 
 __all__ = ["cf_station_metadata", "cf_ahccd_metadata"]
 
 logging.config.dictConfig(LOGGING_CONFIG)
 
 
-def cf_station_metadata(
-    variable_code: Union[int, str]
-) -> Mapping[str, Union[int, float, str]]:
+def cf_station_metadata(variable_code: int | str) -> Mapping[str, int | float | str]:
     """
 
     Parameters
     ----------
-    variable_code: Union[int, str]
+    variable_code: int or  str
 
     Returns
     -------
     dict
     """
     ec_hourly_variables = {
         "001": {
@@ -836,25 +836,25 @@
         logging.error(f"Hourly variable `{code}` not supported.")
         raise
     return variable
 
 
 def cf_ahccd_metadata(
     code: str, gen: int
-) -> (Mapping[str, Union[int, float, str]], Dict, List[Tuple[int, int]], int):
+) -> (dict[str, int | float | str], dict, list[tuple[int, int]], int):
     """
 
     Parameters
     ----------
     code: {"dx", "dn", "dm", "dt", "ds", "dr"}
     gen: {1, 2, 3}
 
     Returns
     -------
-    Mapping[str, Union[str, float]], Dict, List[Tuple[int, int]], int
+    dict[str, int or str or float], dict, list[tuple[int, int]], int
     """
     generation = {1: "First", 2: "Second", 3: "Third"}.get(gen)
 
     ec_ahccd_attrs = dict(
         dx=dict(
             variable="tasmax",
             units="degC",
```

### Comparing `miranda-0.4.0/miranda/eccc/data/ahccd_gen2_precipitation.csv` & `miranda-0.5.0/miranda/eccc/data/ahccd_gen2_precipitation.csv`

 * *Files identical despite different names*

### Comparing `miranda-0.4.0/miranda/eccc/data/ahccd_gen3_temperature.csv` & `miranda-0.5.0/miranda/eccc/data/ahccd_gen3_temperature.csv`

 * *Files identical despite different names*

### Comparing `miranda-0.4.0/miranda/eccc/eccc_homogenized_cf_attrs.json` & `miranda-0.5.0/miranda/eccc/eccc_homogenized_cf_attrs.json`

 * *Files identical despite different names*

### Comparing `miranda-0.4.0/miranda/eccc/eccc_obs_cf_attrs.json` & `miranda-0.5.0/miranda/eccc/eccc_obs_cf_attrs.json`

 * *Files identical despite different names*

### Comparing `miranda-0.4.0/miranda/eccc/eccc_obs_summary_cf_attrs.json` & `miranda-0.5.0/miranda/eccc/eccc_obs_summary_cf_attrs.json`

 * *Files identical despite different names*

### Comparing `miranda-0.4.0/miranda/ecmwf/_era5.py` & `miranda-0.5.0/miranda/ecmwf/_era5.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,30 @@
+from __future__ import annotations
+
 import datetime
 import functools
 import logging.config
 import multiprocessing
 import os
 import re
 import shutil
 import warnings
+from collections.abc import Sequence
 from datetime import datetime as dt
 from pathlib import Path
-from typing import Any, List, Mapping, Optional, Sequence, Tuple, Union
+from typing import Any
 
 import xarray as xr
 
 try:
     from cdsapi import Client  # noqa
 except ModuleNotFoundError:
     warnings.warn(
         "ERA5 downloading capabilities requires additional dependencies. "
-        "Please install them with `pip install miranda[full]`."
+        "Please install them with `pip install miranda[remote]`."
     )
 
 from miranda.gis import subsetting_domains
 from miranda.scripting import LOGGING_CONFIG
 from miranda.units import get_time_frequency
 
 logging.config.dictConfig(LOGGING_CONFIG)
@@ -41,27 +44,27 @@
     "era5-single-levels-monthly-means",
     "era5-single-levels-preliminary-back-extension",
     "era5-single-levels-monthly-means-preliminary-back-extension",
 ]
 
 
 def request_era5(
-    projects: Union[str, List[str]],
+    projects: str | list[str],
     *,
-    variables: Optional[Union[str, Sequence[str]]] = None,
+    variables: str | Sequence[str] | None = None,
     domain: str = "AMNO",
-    pressure_levels: Optional[List[int]] = None,
+    pressure_levels: list[int] | None = None,
     separate_pressure_levels: bool = True,
-    output_folder: Optional[Union[str, os.PathLike]] = None,
-    year_start: Optional[Union[str, int]] = None,
-    year_end: Optional[Union[str, int]] = None,
+    output_folder: str | os.PathLike | None = None,
+    year_start: str | int | None = None,
+    year_end: str | int | None = None,
     dry_run: bool = False,
     processes: int = 10,
-    url: Optional[str] = None,
-    key: Optional[str] = None,
+    url: str | None = None,
+    key: str | None = None,
 ) -> None:
     """Request ERA5/ERA5-Land from Copernicus Data Store in NetCDF4 format.
 
     Parameters
     ----------
     projects : str or List[str]
         Allowed keys: {"era5-land", "era5-land-monthly-means", "era5-single-levels", "era5-single-levels-monthly-means",
@@ -122,15 +125,15 @@
     )
 
     era5_single_levels = variable_reference[
         "era5-land", "era5-land-monthly-means"
     ].copy()
     del era5_single_levels["sde"]  # sde is not available for era5
     era5_single_levels.update(
-        msl="mean_sea_level_pressure", sd="snow_depth"
+        msl="mean_sea_level_pressure", sd="snow_depth", ptype="precipitation_type"
     )  # note difference in name vs era5-land cf_variable == snw"
     variable_reference[
         "era5-single-levels",
         "era5-single-levels-monthly-means",
         "era5-single-levels-preliminary-back-extension",
         "era5-single-levels-monthly-means-preliminary-back-extension",
     ] = era5_single_levels
@@ -164,15 +167,15 @@
         project_names[project] = f"reanalysis-{project}"
 
     for project_name, request_code in project_names.items():
         if year_start is None:
             if "preliminary-back-extension" in project_name or project_name.startswith(
                 "era5-land"
             ):
-                project_year_start = 1950
+                project_year_start = 1940
             else:
                 project_year_start = 1959
         else:
             project_year_start = year_start
 
         if year_end is None:
             if "preliminary-back-extension" in project_name:
@@ -265,27 +268,27 @@
 
         proc.map(func, yearmonth)
         proc.close()
         proc.join()
 
 
 def _request_direct_era(
-    variables: Mapping[str, str],
+    variables: dict[str, str],
     project: str,
     domain: str,
-    pressure_levels: Optional[List[str]],
+    pressure_levels: list[str] | None,
     separate_pressure_level_requests: bool,
     product: str,
     dry_run: bool,
-    client: Optional[Any],
-    yearmonth: Tuple[int, str],
+    client: Any | None,
+    yearmonth: tuple[int, str],
 ):
     """Launch formatted request."""
 
-    def __request(nc_name: str, p: str, rq_kwargs: Mapping[str, str], c: Any):
+    def __request(nc_name: str, p: str, rq_kwargs: dict[str, str], c: Any):
         if Path(nc_name).exists():
             logging.info(f"Dataset {nc_name} already exists. Continuing...")
             return
 
         if not dry_run:
             c.retrieve(
                 p,
@@ -348,15 +351,15 @@
         netcdf_name = (
             f"{var}_{timestep}_ecmwf_{'-'.join(project.split('-')[1:])}"
             f"_{product.replace('_', '-')}_{domain.upper()}_{year_month}.nc"
         )
         __request(netcdf_name, project, request_kwargs, client)
 
 
-def rename_era5_files(path: Union[os.PathLike, str]) -> None:
+def rename_era5_files(path: os.PathLike | str) -> None:
     """Rename badly named ERA5 files.
 
     Notes
     -----
     Requires that the proper ERA5 project name is in the filename, separated by underscores.
     Assumes that the data
```

### Comparing `miranda-0.4.0/miranda/ecmwf/_tigge.py` & `miranda-0.5.0/miranda/ecmwf/_tigge.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,45 @@
+from __future__ import annotations
+
 import functools
 import logging.config
 import multiprocessing
 import os
 from datetime import datetime as dt
 from datetime import timedelta as td
 from pathlib import Path
-from typing import List, Optional
 
 from miranda.scripting import LOGGING_CONFIG
 
 logging.config.dictConfig(LOGGING_CONFIG)
 
 __all__ = ["request_tigge"]
 
 
 def request_tigge(
-    variables: List[str],
-    providers: Optional[List[str]] = None,
+    variables: list[str],
+    providers: list[str] | None = None,
     *,
     forecast_type: str = "pf",
-    times: Optional[List[str]] = None,
-    dates: Optional[List[str]] = None,
-    date_start: Optional[str] = None,
-    date_end: Optional[str] = None,
-    output_folder: Optional[os.PathLike] = None,
+    times: list[str] | None = None,
+    dates: list[str] | None = None,
+    date_start: str | None = None,
+    date_end: str | None = None,
+    output_folder: os.PathLike | None = None,
     processes: int = 4,
 ) -> None:
     """Request tigge data from ECMWF in grib format.
 
     Parameters
     ----------
-    variables : List[str]
-    providers : List[str], optional
+    variables : list of str
+    providers : ist of str, optional
     forecast_type: {"pf", "cf"}
-    times : List[str], optional
-    dates : List[str]. optional
+    times : list of str, optional
+    dates : list of str. optional
     date_start : str, optional
     date_end : str, optional
     output_folder : os.PathLike, optional
     processes : int
 
     Returns
     -------
@@ -47,24 +48,24 @@
 
     def _request_direct_tigge(
         variable_name: str,
         variable_code: str,
         time: str,
         fc_type: str,
         provider: str,
-        nums: Optional[int],
+        nums: int | None,
         date: str,
     ):
         """Launch formatted request."""
         try:
             from ecmwfapi import ECMWFDataServer
         except ModuleNotFoundError:
             raise ModuleNotFoundError(
                 f"{_request_direct_tigge.__name__} requires additional dependencies. "
-                "Please install them with `pip install miranda[full]`."
+                "Please install them with `pip install miranda[remote]`."
             )
 
         number_range = ""
         if nums:
             number_range = "/".join([str(n) for n in range(1, nums + 1)])
         output_name = (
             f"{variable_name}_{provider}_{'-'.join(time.split('/'))}_tigge_reanalysis_6h_"
```

### Comparing `miranda-0.4.0/miranda/gis/_domains.py` & `miranda-0.5.0/miranda/gis/_domains.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,63 @@
-import logging
+from __future__ import annotations
+
 import logging.config
-from pathlib import Path
-from typing import List, Optional, Tuple, Union
 
-import fiona
-import geojson
 import numpy as np
-import regionmask
 import xarray as xr
-from clisops.core.subset import subset_bbox
-from pyproj.crs import CRS
 
 from miranda.scripting import LOGGING_CONFIG
 
 logging.config.dictConfig(LOGGING_CONFIG)
 
 
 __all__ = ["subset_domain", "subsetting_domains", "add_ar6_regions"]
 
+_gis_import_error_message = (
+    "`{}` requires installation of the miranda GIS libraries. These can be installed using the"
+    " `pip install miranda[gis]` recipe or via Anaconda (`conda env update -n miranda-env -f environment.yml`)"
+    " from the miranda repository source files."
+)
+
 
 def subset_domain(
-    ds: Union[xr.Dataset, xr.DataArray], domain: str, **kwargs
-) -> Union[xr.Dataset, xr.DataArray]:
+    ds: xr.Dataset | xr.DataArray, domain: str, **kwargs
+) -> xr.Dataset | xr.DataArray:
+    r"""Subset an xarray object according to a specific domain.
+
+    Notes
+    -----
+    Requires installation of GIS libraries.
+
+    Parameters
+    ----------
+    ds: xarray.Dataset or xarray.DataArray
+    domain: str
+    \*\*kwargs
+
+    Returns
+    -------
+    xarray.Dataset or xarray.DataArray
+    """
+    try:
+        from clisops.core.subset import subset_bbox  # noqa
+    except ModuleNotFoundError:
+        msg = _gis_import_error_message.format(subset_domain.__name__)
+        raise ModuleNotFoundError(msg)
+
     region = subsetting_domains(domain)
     lon_values = np.array([region[1], region[3]])
     lat_values = np.array([region[0], region[2]])
 
     ds = subset_bbox(ds, lon_bnds=lon_values, lat_bnds=lat_values, **kwargs)
 
     return ds
 
 
-def subsetting_domains(domain: str) -> List:
+def subsetting_domains(domain: str) -> list:
     """Provides the bounding box coordinates for specific domains.
 
     Parameters
     ----------
     domain : {"global", "nam", "can", "qc", "mtl"}
 
     Returns
@@ -58,59 +80,70 @@
     if region is not None:
         return region
 
     raise NotImplementedError(domain)
 
 
 # FIXME: This approach will not work with Fiona 1.9+
-def _read_geometries(
-    shape: Union[str, Path], crs: Optional[Union[str, int, dict]] = None
-) -> Tuple[List[geojson.geometry.Geometry], CRS]:
-    """
-    A decorator to perform a check to verify a geometry is valid.
-    Returns the function with geom set to the shapely Shape object.
-    """
-    try:
-        if shape is None:
-            raise ValueError
-    except (KeyError, ValueError):
-        logging.exception("No shape provided.")
-        raise
-
-    geom = list()
-    geometry_types = list()
-    try:
-        with fiona.open(shape) as fio:
-            logging.info("Vector read OK.")
-            if crs:
-                shape_crs = CRS.from_user_input(crs)
-            else:
-                shape_crs = CRS(fio.crs or 4326)
-            for i, feat in enumerate(fio):
-                g = geojson.GeoJSON(feat)
-                geom.append(g["geometry"])
-                geometry_types.append(g["geometry"]["type"])
-    except fiona.errors.DriverError:
-        logging.exception("Unable to read shape.")
-        raise
-
-    if len(geom) > 0:
-        logging.info(f"Shapes found are: {', '.join(set(geometry_types))}.")
-        return geom, shape_crs
-    raise RuntimeError("No geometries found.")
+# def _read_geometries(
+#     shape: Union[str, Path], crs: Optional[Union[str, int, dict]] = None
+# ) -> Tuple[List[geojson.geometry.Geometry], Any]:
+#     """Perform a check to verify a geometry is valid.
+#
+#     Returns the function with geom set to the shapely Shape object.
+#     """
+#     try:
+#         from pyproj import CRS
+#     except ModuleNotFoundError:
+#         msg = gis_import_error_message.format(add_ar6_regions.__name__)
+#         raise ModuleNotFoundError(msg)
+#
+#     try:
+#         if shape is None:
+#             raise ValueError
+#     except (KeyError, ValueError):
+#         logging.exception("No shape provided.")
+#         raise
+#
+#     geom = list()
+#     geometry_types = list()
+#     try:
+#         with fiona.open(shape) as fio:
+#             logging.info("Vector read OK.")
+#             if crs:
+#                 shape_crs = CRS.from_user_input(crs)
+#             else:
+#                 shape_crs = CRS(fio.crs or 4326)
+#             for i, feat in enumerate(fio):
+#                 g = geojson.GeoJSON(feat)
+#                 geom.append(g["geometry"])
+#                 geometry_types.append(g["geometry"]["type"])
+#     except fiona.errors.DriverError:
+#         logging.exception("Unable to read shape.")
+#         raise
+#
+#     if len(geom) > 0:
+#         logging.info(f"Shapes found are: {', '.join(set(geometry_types))}.")
+#         return geom, shape_crs
+#     raise RuntimeError("No geometries found.")
 
 
 def add_ar6_regions(ds: xr.Dataset) -> xr.Dataset:
     """Add the IPCC AR6 Regions to dataset.
 
     Parameters
     ----------
     ds : xarray.Dataset
 
     Returns
     -------
     xarray.Dataset
     """
+    try:
+        import regionmask  # noqa
+    except ImportError:
+        msg = _gis_import_error_message.format(add_ar6_regions.__name__)
+        raise ImportError(msg)
 
     mask = regionmask.defined_regions.ar6.all.mask(ds.lon, ds.lat)
     ds = ds.assign_coords(region=mask)
     return ds
```

### Comparing `miranda-0.4.0/miranda/io/_input.py` & `miranda-0.5.0/miranda/io/_input.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from __future__ import annotations
+
 import logging.config
 import os
 from pathlib import Path
 from types import GeneratorType
-from typing import List, Optional, Union
 
 import netCDF4 as nc  # noqa
 
 from miranda.scripting import LOGGING_CONFIG
 
 logging.config.dictConfig(LOGGING_CONFIG)
 
@@ -15,37 +16,36 @@
     "discover_data",
     "find_filepaths",
 ]
 
 
 # FIXME: How are these two functions different?
 def discover_data(
-    input_files: Union[str, os.PathLike, List[Union[str, os.PathLike]], GeneratorType],
+    input_files: str | os.PathLike | list[str | os.PathLike] | GeneratorType,
     suffix: str = "nc",
     recurse: bool = True,
-) -> Union[List[Path], GeneratorType]:
+) -> list[Path] | GeneratorType:
     """Discover data.
 
     Parameters
     ----------
-    input_files: str or Path or List[Union[str, Path]] or GeneratorType
-      Path or string to a file, a folder, or a generator of paths.
-    suffix: str
-      File-ending suffix to search for. Default: "nc".
-    recurse: bool
-      Whether to recurse through folders or not. Default: True.
+    input_files : str, pathlib.Path, list of str or Path, or GeneratorType
+        Path or string to a file, a folder, or a generator of paths.
+    suffix : str
+        File-ending suffix to search for. Default: "nc".
+    recurse : bool
+        Whether to recurse through folders or not. Default: True.
 
     Returns
     -------
-    list or generator of Path
+    list of pathlib.Path or GeneratorType of pathlib.Path
 
     Warnings
     --------
     Recursion through ".zarr" files is explicitly disabled. Recursive globs and generators will not be expanded/sorted.
-
     """
     if isinstance(input_files, (Path, str)):
         input_files = Path(input_files)
         if input_files.is_dir():
             if suffix.endswith("zarr") or not recurse:
                 input_files = sorted(list(input_files.glob(f"*.{suffix}")))
             else:
@@ -64,32 +64,31 @@
         pass
     else:
         raise NotImplementedError(f"input_files: {type(input_files)}")
     return input_files
 
 
 def find_filepaths(
-    source: Union[Path, str, GeneratorType, List[Union[Path, str]]],
+    source: str | Path | GeneratorType | list[Path | str],
     recursive: bool = True,
-    file_suffixes: Optional[Union[str, List[str]]] = None,
+    file_suffixes: str | list[str] | None = None,
     **_,
-) -> List[Path]:
+) -> list[Path]:
     """Find all available filepaths at a given source.
 
     Parameters
     ----------
-    source : Union[Path, str, GeneratorType, List[Union[Path, str]]]
+    source : str, Path, GeneratorType, or list[str or Path]
     recursive : bool
-    file_suffixes: List[str]
+    file_suffixes: str or list of str, optional
 
     Returns
     -------
-    List[Path]
+    list of pathlib.Path
     """
-
     if file_suffixes is None:
         file_suffixes = ["*", ".*"]
     elif isinstance(file_suffixes, str):
         file_suffixes = [file_suffixes]
 
     found = list()
     if isinstance(source, (Path, str)):
```

### Comparing `miranda-0.4.0/miranda/io/_output.py` & `miranda-0.5.0/miranda/io/_output.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,53 @@
+"""IO Output Operations module."""
+from __future__ import annotations
+
 import logging.config
 import os
 import shutil
 import time
+from collections.abc import Sequence
 from pathlib import Path
-from typing import Dict, Optional, Sequence, Union
 
 import dask
 import xarray as xr
 from dask.distributed import Client
 
 from miranda.convert.utils import date_parser
 from miranda.scripting import LOGGING_CONFIG
 
 from ._input import discover_data
-from ._rechunk import fetch_chunk_config, translate_time_chunk
+from ._rechunk import fetch_chunk_config, prepare_chunks_for_ds, translate_time_chunk
 from .utils import delayed_write, get_global_attrs, name_output_file, sort_variables
 
 logging.config.dictConfig(LOGGING_CONFIG)
 
 
 __all__ = [
     "write_dataset",
     "write_dataset_dict",
     "concat_rechunk_zarr",
     "merge_rechunk_zarrs",
 ]
 
 
 def write_dataset(
-    ds: Union[xr.DataArray, xr.Dataset],
-    project: str,
-    output_path: Union[str, os.PathLike],
+    ds: xr.DataArray | xr.Dataset,
+    output_path: str | os.PathLike,
     output_format: str,
-    chunks: Optional[dict] = None,
+    chunks: dict | None = None,
     overwrite: bool = False,
     compute: bool = True,
-):
-    """
+) -> dict[str, Path]:
+    """Write xarray object to NetCDf or Zarr with appropriate chunking regime.
 
     Parameters
     ----------
     ds : xr.DataArray or xr.Dataset
-
-    project : {"cordex", "cmip5", "cmip6", "ets-grnch", "isimip-ft", "pcic-candcs-u6", "converted"}
-        Project name for decoding/handling purposes.
+        Dataset or DatArray.
     output_path : str or os.PathLike
         Output folder path.
     output_format: {"netcdf", "zarr"}
         Output data container type.
     chunks : dict, optional
         Chunking layout to be written to new files. If None, chunking will be left to the relevant backend engine.
     overwrite : bool
@@ -55,68 +55,89 @@
     compute : bool
         If True, files will be converted with each call to file conversion.
         If False, will return a dask.Delayed object that can be computed later.
         Default: True.
 
     Returns
     -------
-
+    dict[str, Path]
     """
     if isinstance(output_path, str):
         output_path = Path(output_path)
 
-    outfile = name_output_file(ds, project, output_format)
+    outfile = name_output_file(ds, output_format)
     outfile_path = output_path.joinpath(outfile)
 
     if overwrite and outfile_path.exists():
         logging.warning(f"Removing existing {output_format} files for {outfile}.")
         if outfile_path.is_dir():
             shutil.rmtree(outfile_path)
         if outfile_path.is_file():
             outfile_path.unlink()
 
+    if chunks is None and "frequency" in ds.attrs:
+        freq = ds.attrs["frequency"]  # TOD0: check that this is really there
+        chunks = fetch_chunk_config(priority="time", freq=freq, dims=ds.dims)
+
     logging.info(f"Writing {outfile}.")
     write_object = delayed_write(
         ds,
         outfile_path,
         output_format,
         overwrite,
-        target_chunks=chunks,
+        target_chunks=prepare_chunks_for_ds(ds, chunks),
     )
     if compute:
         write_object.compute()
         return dict(path=outfile_path)
     return dict(path=outfile_path, object=write_object)
 
 
 def write_dataset_dict(
-    dataset_dict: Dict[str, xr.Dataset],
-    output_folder: Union[str, os.PathLike],
-    temp_folder: Union[str, os.PathLike],
+    dataset_dict: dict[str, xr.Dataset | None],
+    output_folder: str | os.PathLike,
+    temp_folder: str | os.PathLike,
+    *,
     output_format: str = "zarr",
     overwrite: bool = False,
-    chunks: Dict[str, int] = None,
+    chunks: dict[str, int],
     **dask_kwargs,
 ):
+    r"""Write dataset from Miranda-formatted dataset.
+
+    Parameters
+    ----------
+    dataset_dict : dict[str, xr.Dataset or None]
+    output_folder : str or os.PathLike
+    temp_folder : str or os.PathLike
+    output_format : {"netcdf", "zarr"}
+    overwrite : bool
+    chunks : dict[str, int]
+    \*\*dask_kwargs
+
+    Returns
+    -------
+    None
+    """
     if isinstance(output_folder, str):
         output_folder = Path(output_folder).expanduser()
     if isinstance(temp_folder, str):
         temp_folder = Path(temp_folder).expanduser()
 
     if temp_folder:
         if temp_folder.exists():
             shutil.rmtree(temp_folder)
         temp_folder.mkdir(parents=True)
 
     for variable, ds in dataset_dict.items():
         if ds is None:
             continue
 
-        outfile = name_output_file(ds, ds.attrs["project"], output_format)
-        outpath = output_folder.joinpath(variable, outfile)
+        outfile = name_output_file(ds, output_format)
+        outpath = output_folder.joinpath(str(variable), outfile)
         if not outpath.exists() or overwrite:
             outpath.parent.mkdir(parents=True, exist_ok=True)
             if outpath.exists():
                 shutil.rmtree(outfile)
 
             tmp_path = None
             if temp_folder:
@@ -138,35 +159,33 @@
             logging.warning(
                 f"{outpath.as_posix()} exists and overwrite is False. Continuing..."
             )
 
 
 # FIXME: concat_rechunk and merge_rechunk could be collapsed into each other
 def concat_rechunk_zarr(
-    project: str,
     freq: str,
-    input_folder: Union[str, os.PathLike],
-    output_folder: Union[str, os.PathLike],
+    input_folder: str | os.PathLike,
+    output_folder: str | os.PathLike,
     overwrite: bool = False,
     **dask_kwargs,
-):
-    """
+) -> None:
+    r"""Concatenate and rechunk zarr files.
 
     Parameters
     ----------
-    project
-    freq
-    input_folder
-    output_folder
-    overwrite
-    dask_kwargs
+    freq : str
+    input_folder : str or os.PathLike
+    output_folder : str or os.PathLike
+    overwrite : bool
+    \*\*dask_kwargs
 
     Returns
     -------
-
+    None
     """
     if isinstance(input_folder, str):
         input_folder = Path(input_folder).expanduser()
     if isinstance(output_folder, str):
         output_folder = Path(output_folder).expanduser()
 
     list_zarr = sorted(list(input_folder.glob("*.zarr")))
@@ -175,95 +194,103 @@
     start_year = date_parser(
         list_zarr[0].stem.split("_")[-1], output_type="datetime"
     ).year
     end_year = date_parser(
         list_zarr[-1].stem.split("_")[-1], output_type="datetime"
     ).year
 
-    outzarr = f"{out_stem}_{start_year}_{end_year}.zarr"
-    outzarr = output_folder.joinpath(outzarr)
+    out_zarr = output_folder.joinpath(f"{out_stem}_{start_year}_{end_year}.zarr")
 
-    if not outzarr.exists() or overwrite:
-        chunks = fetch_chunk_config(project=project, freq=freq, priority="time")
+    if not out_zarr.exists() or overwrite:
         # maketemp files 1 zarr per 4 years
         years = [y for y in range(int(start_year), int(end_year) + 1)]
         years = [years[x : x + 4] for x in range(0, len(years), 4)]
+        tmp_folder = out_zarr.parent.joinpath("tmp")
+        tmp_folder.mkdir(exist_ok=True)
+        chunks = dict()
         for year in years:
             list_zarr1 = sorted(
                 [
-                    zarrfile
-                    for zarrfile in list_zarr
-                    if int(zarrfile.stem.split("_")[-1].split("-")[0][0:4]) in year
+                    zarr_file
+                    for zarr_file in list_zarr
+                    if int(zarr_file.stem.split("_")[-1].split("-")[0][0:4]) in year
                 ]
             )
             # assert len(list_zarr1) / len(year) == 12
             ds = xr.open_mfdataset(list_zarr1, parallel=True, engine="zarr")
-            chunks = translate_time_chunk(
-                chunks=chunks, calendar=ds.time.dt.calendar, timesize=len(ds.time)
+            if not chunks:
+                chunk_config = fetch_chunk_config(
+                    priority="time", freq=freq, dims=ds.dims
+                )
+                chunks.update(
+                    translate_time_chunk(
+                        chunks=chunk_config,
+                        calendar=ds.time.dt.calendar,
+                        timesize=len(ds.time),
+                    )
+                )
+            tmp_zarr = tmp_folder.joinpath(
+                f"{out_zarr.stem.split(f'_{start_year}_')[0]}_{year[0]}-{year[-1]}.zarr",
             )
-            tmpzarr = outzarr.parent.joinpath(
-                "tmp",
-                f"{outzarr.stem.split(f'_{start_year}_')[0]}_{year[0]}-{year[-1]}.zarr",
-            )
-            tmpzarr.parent.mkdir(exist_ok=True, parents=True)
-            logging.info(f"Writing year {year} to {tmpzarr.as_posix()}.")
+            tmp_zarr.parent.mkdir(exist_ok=True, parents=True)
+            logging.info(f"Writing year {year} to {tmp_zarr.as_posix()}.")
 
             job = delayed_write(
                 ds=ds,
-                outfile=tmpzarr,
+                outfile=tmp_zarr,
                 output_format="zarr",
                 target_chunks=chunks,
                 overwrite=True,
             )  # kwargs=zarr_kwargs)
             # FIXME: Client is only needed for computation. Should be elsewhere.
             with Client(**dask_kwargs):
                 dask.compute(job)
 
         # get tmp zarrs
-        list_zarr = sorted(list(tmpzarr.parent.glob("*zarr")))
+        list_zarr = sorted(list(tmp_folder.glob("*zarr")))
         ds = xr.open_mfdataset(list_zarr, engine="zarr")
         # FIXME: Client is only needed for computation. Should be elsewhere.
         job = delayed_write(
             ds=ds,
-            outfile=outzarr,
+            outfile=out_zarr,
             output_format="zarr",
             target_chunks=chunks,
             overwrite=overwrite,
         )  # kwargs=zarr_kwargs)
         with Client(**dask_kwargs):
             dask.compute(job)
-        shutil.rmtree(tmpzarr.parent)
+        shutil.rmtree(tmp_folder)
 
 
 def merge_rechunk_zarrs(
-    input_folder: Union[str, os.PathLike],
-    output_folder: Union[str, os.PathLike],
-    project: Optional[str] = None,
-    target_chunks: Optional[Dict[str, int]] = None,
-    variables: Optional[Sequence[str]] = None,
-    freq: Optional[str] = None,
+    input_folder: str | os.PathLike,
+    output_folder: str | os.PathLike,
+    project: str | None = None,
+    target_chunks: dict[str, int] | None = None,
+    variables: Sequence[str] | None = None,
+    freq: str | None = None,
     suffix: str = "zarr",
     overwrite: bool = False,
-):
-    """
+) -> None:
+    """Merge and rechunk zarr files.
 
     Parameters
     ----------
-    input_folder
-    output_folder
-    project
-    target_chunks
-    variables
-    freq
-    suffix
-    overwrite
+    input_folder : str or os.PathLike
+    output_folder : str or os.PathLike
+    project : str, optional
+    target_chunks : dict[str, int], optional
+    variables : Sequence of str, optional
+    freq : str, optional
+    suffix : {"nc", "zarr"}
+    overwrite : bool
 
     Returns
     -------
-
+    None
     """
     chunk_defaults = {
         # Four months of hours
         "1hr": {"time": 2922},
         # Four years of days
         "day": {"time": 365 * 4 + 1},
     }
@@ -300,15 +327,15 @@
     start = time.perf_counter()
 
     for variable, files in variable_sorted.items():
         start_var = time.perf_counter()
 
         ds = xr.open_mfdataset(files_found, parallel=True, engine="zarr")
 
-        merged_zarr = name_output_file(ds, project, output_format="zarr")
+        merged_zarr = name_output_file(ds, output_format="zarr")
         out_zarr = output_folder.joinpath(merged_zarr)
 
         if overwrite:
             if out_zarr.is_dir():
                 logging.warning(f"Removing existing zarr files for {out_zarr.name}.")
                 shutil.rmtree(out_zarr)
         else:
```

### Comparing `miranda-0.4.0/miranda/io/_rechunk.py` & `miranda-0.5.0/miranda/io/_rechunk.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,71 @@
+from __future__ import annotations
+
 import json
 import logging.config
 import os
 import shutil
 import time
+from collections.abc import Hashable, Sequence
 from pathlib import Path
-from typing import Dict, Optional, Sequence, Union
 
 import xarray as xr
+from xarray.core.utils import Frozen
 
-from miranda.convert import project_institutes
 from miranda.scripting import LOGGING_CONFIG
 
 from ._input import discover_data
 from .utils import delayed_write, get_global_attrs, get_time_attrs, sort_variables
 
 logging.config.dictConfig(LOGGING_CONFIG)
 
 
-__all__ = ["fetch_chunk_config", "rechunk_files", "translate_time_chunk"]
+__all__ = [
+    "fetch_chunk_config",
+    "prepare_chunks_for_ds",
+    "rechunk_files",
+    "translate_time_chunk",
+]
 
 _data_folder = Path(__file__).parent / "data"
-chunk_configurations = json.load(open(_data_folder / "chunk_configurations.json"))
+chunk_configurations = json.load(open(_data_folder / "ouranos_chunk_config.json"))
+
+
+def prepare_chunks_for_ds(
+    ds: xr.Dataset, chunks: dict[str, str | int]
+) -> dict[str, int]:
+    """Prepare the chunks to be used to write Dataset.
+
+    This includes translating the time chunks, making sure chunks are not too small, and removing -1.
+
+    Parameters
+    ----------
+    ds : xr.Dataset
+        Dataset that we want to write with the chunks.
+    chunks : dict
+        Desired chunks in human-readable format (with "4 years" and -1).
+
+    Returns
+    -------
+    dict
+        Chunks in a format that is ready to be used to write to disk.
+    """
+    # check if any of the chunks are strings and need to be translated
+    if any(isinstance(x, str) for x in chunks.values()):
+        calendar, size = get_time_attrs(ds)
+        chunks = translate_time_chunk(chunks, calendar, size)
+
+    # replace -1 that netcdf can't handle and cut chunks that are too big for the dim
+    for dim, c in chunks.copy().items():
+        length = ds.dims[dim]
+        if c == -1 or c > length:
+            logging.info(f"Chunk was changed from {c} to {length} for dimension {dim}.")
+            chunks[dim] = length
+
+    return chunks
 
 
 # Shamelessly stolen and modified from xscen
 def translate_time_chunk(chunks: dict, calendar: str, timesize: int) -> dict:
     """Translate chunk specification for time into a number.
 
     Notes
@@ -44,57 +85,57 @@
                 chunks[k] = int(Nt)
             elif v == -1:
                 chunks[k] = timesize
     return chunks
 
 
 def fetch_chunk_config(
-    project: str, freq: str, priority: str = "files"
-) -> Dict[str, int]:
+    priority: str,
+    freq: str,
+    dims: Sequence[str] | dict[str, int] | Frozen | tuple[Hashable],
+    default_config: dict = chunk_configurations,
+) -> dict[str, int]:
     """
 
     Parameters
     ----------
-    project : str, optional
-        Supported projects. Used for determining chunk dictionary.
-    freq: {"1hr", "day", "month"}
-        The chunking regime for
     priority : {"time", "files"}
         Specifies whether the chunking regime should prioritize file granularity ("files") or time series ("time").
+    freq : {"1hr", "day", "month"}
+        The time frequency of the input data.
+    dims : sequence of str
+        The dimension names that will be used for chunking.
+    default_config : dict
+        The dictionary to use for determining the chunking configuration.
 
     Returns
     -------
-
+    dict[str, int]
     """
-    institute = project_institutes[project]
-    entry = chunk_configurations[institute.upper()]
+    if isinstance(dims, (dict, Frozen)):
+        dims = {k for k in dims.keys()}
 
-    # TODO: Currently no explicit handling for multi-level data
-    if project in entry["projects"]:
-        return entry["time"][freq]
-        # if priority in entry[project]:
-        #     if freq in entry[priority]:
-        #         try:
-        #             return entry[priority][freq]
-        #         except KeyError:
-        #             raise KeyError(
-        #                 f"Chunks at frequency `{freq}` not found for project `{project}`."
-        #             )
-        # raise KeyError(f"Priority regime `{priority}` not found.")
-    raise KeyError(f"Project `{project}` not found.")
+    if priority in default_config:
+        if freq in default_config[priority]:
+            for config in default_config[priority][freq].keys():
+                if set(default_config[priority][freq][config]).issubset(dims):
+                    return default_config[priority][freq][config]
+            raise KeyError(f"Chunk dimensions `{dims}` configuration not found.")
+        raise KeyError(f"Frequency `{freq}` configuration not found.")
+    raise KeyError(f"Priority regime `{priority}` configuration not found.")
 
 
 def rechunk_files(
-    input_folder: Union[str, os.PathLike],
-    output_folder: Union[str, os.PathLike],
-    project: Optional[str] = None,
-    time_step: Optional[str] = None,
+    input_folder: str | os.PathLike,
+    output_folder: str | os.PathLike,
+    project: str | None = None,
+    time_step: str | None = None,
     chunking_priority: str = "auto",
-    target_chunks: Optional[Dict[str, int]] = None,
-    variables: Optional[Sequence[str]] = None,
+    target_chunks: dict[str, int] | None = None,
+    variables: Sequence[str] | None = None,
     suffix: str = "nc",
     output_format: str = "netcdf",
     overwrite: bool = False,
 ) -> None:
     """Rechunks dataset for better loading/reading performance.
 
     Warnings
@@ -187,15 +228,15 @@
                 else:
                     logging.info(f"Files exist: {file.name}")
                     continue
 
             ds = xr.open_dataset(file, chunks={"time": -1})
 
             if target_chunks is None:
-                chunk_config = fetch_chunk_config(project, time_step, chunking_priority)
+                chunk_config = fetch_chunk_config(chunking_priority, time_step, ds.dims)
                 calendar, size = get_time_attrs(ds)
                 target_chunks = translate_time_chunk(chunk_config, calendar, size)
 
             try:
                 delayed_write(
                     ds,
                     out,
```

### Comparing `miranda-0.4.0/miranda/io/data/chunk_configurations.json` & `miranda-0.5.0/miranda/io/data/ouranos_chunk_config.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('files', OrderedDict([('1hr', OrderedDict([('default', "*

 * *            "OrderedDict([('lat', 250), ('lon', 250), ('time', 168)])), ('rotated', "*

 * *            "OrderedDict([('rlat', 250), ('rlon', 250), ('time', 168)]))])), ('day', "*

 * *            "OrderedDict([('default', OrderedDict([('lat', 125), ('lon', 125), ('time', '1 "*

 * *            "year')])), ('rotated', OrderedDict([('rlat', 125), ('rlon', 125), ('time', '1 "*

 * *            "year')]))])), ('month', OrderedDict([('default', Ordered […]*

```diff
@@ -1,84 +1,78 @@
 {
-    "ECCC": {
-        "files": {
-            "1hr": {
+    "files": {
+        "1hr": {
+            "default": {
+                "lat": 250,
+                "lon": 250,
+                "time": 168
+            },
+            "rotated": {
                 "rlat": 250,
                 "rlon": 250,
                 "time": 168
+            }
+        },
+        "day": {
+            "default": {
+                "lat": 125,
+                "lon": 125,
+                "time": "1 year"
             },
-            "day": {
+            "rotated": {
                 "rlat": 125,
                 "rlon": 125,
                 "time": "1 year"
-            },
-            "month": {
-                "rlat": 500,
-                "rlon": 500,
-                "time": 120
             }
         },
-        "projects": [
-            "rdrs-v21"
-        ],
-        "time": {
-            "1hr": {
-                "rlat": 50,
-                "rlon": 50,
-                "time": 1440
-            },
-            "day": {
-                "rlat": 50,
-                "rlon": 50,
-                "time": "4 years"
-            },
-            "month": {
-                "rlat": 250,
-                "rlon": 250,
-                "time": 240
-            }
-        }
-    },
-    "ECMWF": {
-        "files": {
-            "1hr": {
-                "lat": 250,
-                "lon": 250,
-                "time": 168
-            },
-            "day": {
-                "latitude": 125,
-                "longitude": 125,
-                "time": "1 year"
+        "month": {
+            "default": {
+                "lat": 500,
+                "lon": 500,
+                "time": 120
             },
-            "month": {
+            "rotated": {
                 "rlat": 500,
                 "rlon": 500,
                 "time": 120
             }
-        },
-        "projects": [
-            "era5-single-levels",
-            "era5-single-levels-preliminary-back-extension",
-            "era5-land",
-            "era5-pressure-levels",
-            "era5-pressure-levels-preliminary-back-extension"
-        ],
-        "time": {
-            "1hr": {
+        }
+    },
+    "time": {
+        "1hr": {
+            "default": {
                 "lat": 50,
                 "lon": 50,
                 "time": 1440
             },
-            "day": {
+            "rotated": {
+                "rlat": 50,
+                "rlon": 50,
+                "time": 1440
+            }
+        },
+        "day": {
+            "default": {
                 "lat": 50,
                 "lon": 50,
                 "time": "4 years"
             },
-            "month": {
+            "rotated": {
+                "rlat": 50,
+                "rlon": 50,
+                "time": "4 years"
+            }
+        },
+        "month": {
+            "default": {
                 "lat": 250,
                 "lon": 250,
                 "time": 240
+            },
+            "rotated": {
+                "rlat": 250,
+                "rlon": 250,
+                "time": 240
             }
         }
     }
 }
```

### Comparing `miranda-0.4.0/miranda/io/utils.py` & `miranda-0.5.0/miranda/io/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+"""IO Utilities module."""
+from __future__ import annotations
+
+import json
 import logging.config
 import os
+from collections.abc import Sequence
 from datetime import date
 from pathlib import Path
-from typing import Dict, List, Optional, Sequence, Union
 
 import dask
 import netCDF4 as nc  # noqa
 import xarray as xr
 import zarr
 
 from miranda.scripting import LOGGING_CONFIG
@@ -20,43 +24,45 @@
     "get_chunks_on_disk",
     "get_global_attrs",
     "get_time_attrs",
     "name_output_file",
     "sort_variables",
 ]
 
+_data_folder = Path(__file__).parent / "data"
+name_configurations = json.load(open(_data_folder / "ouranos_name_config.json"))
+
 
 def name_output_file(
-    ds_or_dict: Union[xr.Dataset, Dict[str, str]], project: str, output_format: str
+    ds_or_dict: xr.Dataset | dict[str, str], output_format: str
 ) -> str:
     """Name an output file based on facets within a Dataset or a dictionary.
 
     Parameters
     ----------
     ds_or_dict : xr.Dataset or dict
-    project: str
+        A miranda-converted Dataset or a dictionary containing the appropriate facets.
     output_format : {"netcdf", "zarr"}
-        Suffix to be used for filename
+        Output filetype to be used for generating filename suffix.
 
     Returns
     -------
     str
 
     Notes
     -----
-    If using a dictionary, the following must be keys: "variable", "frequency", "institution", "time_start", "time_end".
-
+    If using a dictionary, the following keys must be set:
+    * "variable", "frequency", "institution", "time_start", "time_end".
     """
     if output_format.lower() not in {"netcdf", "zarr"}:
         raise NotImplementedError(f"Format: {output_format}.")
     else:
         suffix = dict(netcdf="nc", zarr="zarr")[output_format]
 
     facets = dict()
-    facets["project"] = project
     facets["suffix"] = suffix
 
     if isinstance(ds_or_dict, xr.Dataset):
         if len(ds_or_dict.data_vars) == 1:
             facets["variable"] = list(ds_or_dict.data_vars.keys())[0]
         elif (
             len(ds_or_dict.data_vars) == 2
@@ -65,52 +71,100 @@
             facets["variable"] = [
                 v for v in ds_or_dict.data_vars if v != "rotated_pole"
             ][0]
         else:
             raise NotImplementedError(
                 f"Too many `data_vars` in Dataset: {' ,'.join(ds_or_dict.data_vars.keys())}."
             )
-        facets["frequency"] = ds_or_dict.attrs.get("frequency")
-        facets["institution"] = ds_or_dict.attrs.get("institution")
+        for f in [
+            "bias_adjust_project",
+            "domain",
+            "frequency",
+            "institution",
+            "source",
+            "experiment",
+            "member",
+            "processing_level",
+            "project",
+            "type",
+            "mip_era",
+            "activity",
+        ]:
+            facets[f] = ds_or_dict.attrs.get(f)
+
+        if facets["frequency"] in ["1hr", "day"]:
+            date_format = "%Y%m%d"
+        elif facets["frequency"] == "month":
+            date_format = "%Y%m"
+        elif facets["frequency"] == "year":
+            date_format = "%Y"
+        else:
+            raise KeyError("`frequency` not found.")
+
         facets["time_start"], facets["time_end"] = (
-            ds_or_dict.time.isel(time=[0, -1]).dt.strftime("%Y%m%d").values
+            ds_or_dict.time.isel(time=[0, -1]).dt.strftime(date_format).values
         )
+        facets["year_start"], facets["year_end"] = ds_or_dict.time.isel(
+            time=[0, -1]
+        ).dt.year.values
     elif isinstance(ds_or_dict, dict):
-        facets["variable"] = ds_or_dict.get("variable")
-        facets["frequency"] = ds_or_dict.get("variable")
-        facets["institution"] = ds_or_dict.get("variable")
-        facets["time_start"] = ds_or_dict.get("variable")
-        facets["time_end"] = ds_or_dict.get("variable")
+        for f in [
+            "bias_adjust_project",
+            "domain",
+            "frequency",
+            "institution",
+            "processing_level",
+            "project",
+            "type",
+            "time",
+            "time_end",
+            "time_start",
+            "variable",
+        ]:
+            facets[f] = ds_or_dict.get(f)
     else:
         raise NotImplementedError("Must be a Dataset or dictionary.")
 
+    if {"time_start", "time_end"}.issubset(facets) and "time" not in facets:
+        if facets["time_start"] == facets["time_end"]:
+            facets["time"] = "-".join([facets["time_start"], facets["time_end"]])
+        else:
+            facets["time"] = facets["time_start"]
+
+    str_name = "{variable}_{frequency}_{institution}_{project}_{time}.{suffix}"
+    # Get the string for the name
+    if facets["type"] in name_configurations.keys():
+        if facets["project"] in name_configurations[facets["type"]].keys():
+            str_name = name_configurations[facets["type"]][facets["project"]]
+
     missing = []
     for k, v in facets.items():
-        if v is None:
+        if (
+            v is None and k in str_name
+        ):  # only missing if the facets is needed in the name
             missing.append(k)
     if missing:
         raise ValueError(f"The following facets were not found: {' ,'.join(missing)}.")
 
-    return "{variable}_{frequency}_{institution}_{project}_{time_start}-{time_end}.{suffix}".format(
-        **facets
-    )
+    # fill in string with facets
+    return str_name.format(**facets)
 
 
 def delayed_write(
     ds: xr.Dataset,
-    outfile: Union[str, os.PathLike],
+    outfile: str | os.PathLike,
     output_format: str,
     overwrite: bool,
-    target_chunks: Optional[dict] = None,
+    target_chunks: dict | None = None,
 ) -> dask.delayed:
-    """
+    """Stage a Dataset writing job using `dask.delayed` objects.
 
     Parameters
     ----------
-    ds : Union[xr.Dataset, str, os.PathLike]
+    ds : xr.Dataset
     outfile : str or os.PathLike
     target_chunks : dict
     output_format : {"netcdf", "zarr"}
     overwrite : bool
 
     Returns
     -------
@@ -152,29 +206,31 @@
     except KeyError:
         logging.error("Unable to encode chunks. Verify dataset.")
         raise
 
     return getattr(ds, f"to_{output_format}")(outfile, **kwargs)
 
 
-def get_time_attrs(file_or_dataset: Union[str, os.PathLike, xr.Dataset]) -> (str, int):
+def get_time_attrs(file_or_dataset: str | os.PathLike | xr.Dataset) -> (str, int):
+    """Determine attributes related to time dimensions."""
     if isinstance(file_or_dataset, (str, Path)):
         ds = xr.open_dataset(Path(file_or_dataset).expanduser())
     else:
         ds = file_or_dataset
 
     calendar = ds.time.dt.calendar
     time = len(ds.time)
 
     return calendar, time
 
 
 def get_global_attrs(
-    file_or_dataset: Union[str, os.PathLike, xr.Dataset]
-) -> Dict[str, Union[str, int]]:
+    file_or_dataset: str | os.PathLike | xr.Dataset,
+) -> dict[str, str | int]:
+    """Collect global attributes from NetCDF, Zarr, or Dataset object."""
     if isinstance(file_or_dataset, (str, Path)):
         file = Path(file_or_dataset).expanduser()
     elif isinstance(file_or_dataset, xr.Dataset):
         file = file_or_dataset
     else:
         raise NotImplementedError(f"Type: `{type(file_or_dataset)}`.")
 
@@ -190,16 +246,27 @@
     else:
         data = file.attrs
 
     return data
 
 
 def sort_variables(
-    files: List[Path], variables: Sequence[str]
-) -> Dict[str, List[Path]]:
+    files: list[Path], variables: Sequence[str]
+) -> dict[str, list[Path]]:
+    """Sort all variables within supplied files for treatment.
+
+    Parameters
+    ----------
+    files: list of Path
+    variables: sequence of str
+
+    Returns
+    -------
+    dict[str, list[Path]]
+    """
     variable_sorted = dict()
     if variables:
         logging.info("Sorting variables into groups. This could take some time.")
         for variable in variables:
             var_group = []
             for file in files:
                 if file.name.startswith(variable):
@@ -210,16 +277,16 @@
             variable_sorted[variable] = sorted(var_group)
     else:
         variable_sorted["all_variables"] = files
 
     return variable_sorted
 
 
-def get_chunks_on_disk(file: Union[os.PathLike, str]) -> dict:
-    """
+def get_chunks_on_disk(file: os.PathLike | str) -> dict:
+    """Determine the chunks on disk for a given NetCDF or Zarr file.
 
     Parameters
     ----------
     file : str or os.PathLike
         File to be examined. Supports NetCDF and Zarr.
 
     Returns
@@ -242,26 +309,26 @@
                 if v[1]:
                     chunks[v[0]] = v[1]
     else:
         raise NotImplementedError(f"File type: {file.suffix}.")
     return chunks
 
 
-def creation_date(path_to_file: Union[Path, str]) -> Union[float, date]:
-    """Try to get the date that a file was created, falling back to when it was last modified if that isn't possible.
+def creation_date(path_to_file: str | os.PathLike) -> float | date:
+    """Return the date that a file was created, falling back to when it was last modified if unable to determine.
 
     See https://stackoverflow.com/a/39501288/1709587 for explanation.
 
     Parameters
     ----------
-    path_to_file: Union[Path, str]
+    path_to_file : str or os.PathLike
 
     Returns
     -------
-    Union[float, date]
+    float or date
     """
     if os.name == "nt":
         return Path(path_to_file).stat().st_ctime
 
     stat = Path(path_to_file).stat()
     try:
         return date.fromtimestamp(stat.st_ctime)
```

### Comparing `miranda-0.4.0/miranda/ncar/_aws_cordex.py` & `miranda-0.5.0/miranda/ncar/_aws_cordex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+from __future__ import annotations
+
 import ast
 import functools
 import json
 import logging.config
 import warnings
 from json.decoder import JSONDecodeError
 from pathlib import Path
-from typing import Dict, List, Optional, Union
 
 import schema
 import xarray as xr
-from clisops.core import subset_bbox
 from dask.diagnostics import ProgressBar
 from xclim.core import calendar as xcal  # noqa
 
 from miranda.gis import subsetting_domains
 from miranda.scripting import LOGGING_CONFIG
 
 logging.config.dictConfig(LOGGING_CONFIG)
@@ -22,15 +22,15 @@
     import intake  # noqa
     import intake_esm  # noqa
     import numcodecs  # noqa
     import s3fs  # noqa
 except ImportError:
     warnings.warn(
         f"{__name__} functions require additional dependencies. "
-        "Please install them with `pip install miranda[full]`."
+        "Please install them with `pip install miranda[remote]`."
     )
 
 
 __all__ = [
     "cordex_aws_calendar_correction",
     "cordex_aws_download",
 ]
@@ -66,15 +66,15 @@
         schema.Optional("bias_correction"): schema.Or(
             ["raw", "mbcn-Daymet", "mbcn-gridMET"]
         ),
     }
 )
 
 
-def cordex_aws_calendar_correction(ds) -> Optional[xr.Dataset]:
+def cordex_aws_calendar_correction(ds) -> xr.Dataset | None:
     """AWS-stored CORDEX datasets are all on the same standard calendar, this converts
     the data back to the original calendar, removing added NaNs.
 
     Credit: Pascal Bourgault (@aulemahal)
     """
     orig_calendar = ds.attrs.get("original_calendar", "standard")
 
@@ -90,23 +90,35 @@
                 raise ValueError("Conversion of dataset to 360_day calendar failed.")
             ds["time"] = time
 
     return ds
 
 
 def cordex_aws_download(
-    target_folder: Union[str, Path],
+    target_folder: str | Path,
     *,
-    search: Dict[str, Union[str, List[str]]],
+    search: dict[str, str | list[str]],
     correct_times: bool = False,
-    domain: Optional[str] = None,
+    domain: str | None = None,
 ):
-    def _subset_preprocess(d: xr.Dataset, dom: List[float]) -> xr.Dataset:
-        n, w, s, e = subsetting_domains(dom)
-        return subset_bbox(d, lon_bnds=[w, e], lat_bnds=[s, n])
+    """Download CORDEX interpolated grid for North America from Amazon S3."""
+
+    def _subset_preprocess(d: xr.Dataset, dom: list[float]) -> xr.Dataset:
+        try:
+            from clisops.core import subset_bbox
+
+            n, w, s, e = subsetting_domains(dom)
+            return subset_bbox(d, lon_bnds=[w, e], lat_bnds=[s, n])
+        except ModuleNotFoundError:
+            log_msg = (
+                "This function requires the `clisops` library which is not installed. "
+                "Domain subsetting step will be skipped."
+            )
+            warnings.warn(log_msg)
+            return d
 
     schema.Schema(_allowed_args).validate(search)
 
     # Define the catalog description file location.
     catalog_url = (
         "https://ncar-na-cordex.s3-us-west-2.amazonaws.com/catalogs/aws-na-cordex.json"
     )
@@ -202,8 +214,10 @@
                     logging.warning(
                         f"All files currently exist for {scen} and {member.name}. Continuing..."
                     )
                     continue
 
                 logging.info(f"Final count of files: {len(datasets)}")
 
-                xr.save_mfdataset(datasets, paths, format="NETCDF4_CLASSIC")
+                xr.save_mfdataset(
+                    datasets, paths, engine="h5netcdf", format="NETCDF4_CLASSIC"
+                )
```

### Comparing `miranda-0.4.0/miranda/remote/archiver.py` & `miranda-0.5.0/miranda/remote/archiver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import logging
+"""Archive Module."""
+from __future__ import annotations
+
 import logging.config
 from collections import defaultdict
 from pathlib import Path
-from typing import List, Union
 
 from miranda.archive import (
     group_by_deciphered_date,
     group_by_size,
     group_by_subdirectories,
 )
 from miranda.io import find_filepaths
@@ -19,17 +20,17 @@
 
 logging.config.dictConfig(LOGGING_CONFIG)
 
 __all__ = ["archive_database"]
 
 
 def archive_database(
-    source: Union[Path, str, List],
-    common_path: Union[Path, str],
-    destination: Union[Path, str],
+    source: Path | str | list,
+    common_path: Path | str,
+    destination: Path | str,
     file_suffixes: str = ".nc",
     server: str = None,
     username: str = None,
     project_name: str = None,
     overwrite: bool = False,
     compression: bool = False,
     recursive: bool = False,
```

### Comparing `miranda-0.4.0/miranda/remote/connect.py` & `miranda-0.5.0/miranda/remote/connect.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,40 @@
+"""Remote Connection Operations module."""
+from __future__ import annotations
+
 import logging.config
 import warnings
 from getpass import getpass
 from pathlib import Path
-from typing import Union
 
 from miranda.scripting import LOGGING_CONFIG
 
 try:
     import fabric  # noqa
     from paramiko import SSHClient  # noqa
     from scp import SCPClient  # noqa
 except ImportError:
     warnings.warn(
         f"{__name__} functions require additional dependencies."
-        f"Please install them with `pip install miranda[full]`."
+        f"Please install them with `pip install miranda[remote]`."
     )
 
 
 logging.config.dictConfig(LOGGING_CONFIG)
 
 __all__ = ["Connection"]
 
 
 class Connection:
+    """Connection contextualise class."""
+
     def __init__(
         self,
-        username: Union[str, Path] = None,
-        host: Union[str, Path] = None,
+        username: str | Path = None,
+        host: str | Path = None,
         protocol: str = "sftp",
         *args,
         **kwargs,
     ):
         self.user = username or input("Enter username: ")
         self.host = host or input("Enter host URL: ")
         self._args = list(*args)
@@ -39,27 +43,35 @@
 
         if protocol.lower() in ["sftp", "scp"]:
             self.protocol = protocol.lower()
         else:
             raise ValueError('Protocol must be "sftp" or "scp".')
 
     def update(self, **kwargs):
+        """Update connection keyword arguments.
+
+        Warnings
+        --------
+        Credentials are not encrypted.
+        """
         self._kwargs = kwargs
 
     def __call__(self, **kwargs):
+        """Update keyword arguments on call."""
         self.update(**kwargs)
         return self
 
     def __str__(self):
         return f"Connection to {self.host} as {self.user}"
 
     def __repr__(self):
         return f"<{self.__class__.__module__}.{self.__class__.__name__} object at {hex(id(self))}>"
 
     def connect(self, **kwargs):
+        """Connect to a remote server with credential prompts."""
         try:
             keywords = (
                 dict(**kwargs)
                 or dict(**self._kwargs)
                 or dict(password=getpass("Enter password: "))
             )
             if self.protocol == "sftp":
```

### Comparing `miranda-0.4.0/miranda/remote/ops.py` & `miranda-0.5.0/miranda/remote/ops.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,49 @@
+"""Remote Operations module."""
 from __future__ import annotations
 
-import logging
 import logging.config
 import os
 import tarfile
 import tempfile
 import time
 import warnings
 from pathlib import Path
-from typing import List, Union
 
 import miranda.remote
 from miranda.scripting import LOGGING_CONFIG
 
 try:
     import fabric  # noqa
     from paramiko import SFTPClient, SSHClient, SSHException  # noqa
     from scp import SCPClient, SCPException  # noqa
 except ImportError:
     warnings.warn(
-        f"{__name__} functions require additional dependencies. Please install them with `pip install miranda[full]`."
+        f"{__name__} functions require additional dependencies. Please install them with `pip install miranda[remote]`."
     )
 
 
 logging.config.dictConfig(LOGGING_CONFIG)
 __all__ = ["create_archive", "create_remote_directory", "transfer_file"]
 
 
 def create_remote_directory(
     directory: str | os.PathLike,
     transport: SSHClient | fabric.Connection | miranda.remote.Connection,
 ) -> None:
-    """
-    This calls a "mkdir -p" function to create a folder structure over SFTP/SSH and waits
-    for confirmation before continuing
+    """Call "mkdir -p" function to create a folder structure over SFTP/SSH and wait for confirmation before continuing.
 
     Parameters
     ----------
-    directory : Union[str, os.PathLike]
-    transport : Union[SSHClient, fabric.Connection, Connection]
+    directory :  str or os.PathLike
+    transport : SSHClient or fabric.Connection or miranda.remote.Connection
 
     Returns
     -------
     None
-
     """
     if isinstance(directory, str):
         directory = Path(directory)
     logging.info(f"Creating remote path: {directory}")
 
     ownership = "0775"
     command = f"mkdir -p -m {ownership} '{directory.as_posix()}'"
@@ -68,34 +64,34 @@
 
 def create_archive(
     source_files: list[str | os.PathLike],
     destination: str | os.PathLike,
     transport: SCPClient
     | SFTPClient
     | fabric.Connection
-    | miranda.remote.Connection = None,
+    | miranda.remote.Connection
+    | None = None,
     delete: bool = True,
     compression: bool = False,
     recursive: bool = True,
 ) -> None:
-    """
+    """Create an archive from source files and transfer to another location (remote or local).
 
     Parameters
     ----------
-    source_files : List[Union[str, os.PathLike]]
-    destination : Union[str, os.PathLike]
-    transport : Union[SCPClient, SFTPClient, fabric.Connection, Connection]
+    source_files : list of str or os.PathLike
+    destination : str or os.PathLike
+    transport : SCPClient or SFTPClient or fabric.Connection or miranda.remote.Connection, optional
     delete : bool
     compression : bool
     recursive : bool
 
     Returns
     -------
     None
-
     """
     if compression:
         write = "w:gz"
     elif not compression:
         write = "w"
     else:
         raise ValueError(f"Compression: {compression}")
@@ -117,30 +113,29 @@
 
 def transfer_file(
     source_file: str | os.PathLike,
     destination_file: str | os.PathLike,
     transport: SCPClient
     | SFTPClient
     | fabric.Connection
-    | miranda.remote.Connection = None,
+    | miranda.remote.Connection
+    | None = None,
 ) -> bool:
-    """
+    """Transfer file from one location (remote or local) to another.
 
     Parameters
     ----------
-    source_file : Union[str, os.PathLike]
-    destination_file : Union[str, os.PathLike]
-    transport : Union[SCPClient, SFTPClient, fabric.Connection, Connection]
+    source_file : str or os.PathLike
+    destination_file : str or os.PathLike
+    transport : SCPClient or SFTPClient or fabric.Connection or miranda.remote.Connection, optional
 
     Returns
     -------
     bool
-
     """
-
     source_file = Path(source_file)
     destination_file = Path(destination_file)
 
     if transport:
         try:
             logging.info(f"Beginning transfer of {source_file}")
             transport.put(str(source_file), str(destination_file))
```

### Comparing `miranda-0.4.0/miranda/remote/remove.py` & `miranda-0.5.0/miranda/remote/remove.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,93 @@
+"""Remote File Removal Operations module."""
+from __future__ import annotations
+
 import logging.config
 import warnings
 from datetime import date
 from getpass import getpass
 from pathlib import Path
 from types import GeneratorType
-from typing import List, Optional, Union
 
 from miranda.io.utils import creation_date
 from miranda.scripting import LOGGING_CONFIG
 from miranda.storage import report_file_size
 
 logging.config.dictConfig(LOGGING_CONFIG)
 
 try:
     import fabric  # noqa
 except ImportError:
     warnings.warn(
         f"{__name__} functions require additional dependencies. "
-        "Please install them with `pip install miranda[full]`."
+        "Please install them with `pip install miranda[remote]`."
     )
 
 
 __all__ = [
     "delete_by_date",
     "delete_by_variable",
     "delete_duplicates",
     "file_emptier",
 ]
 
 
-def file_emptier(*, file_list: Union[List[Union[str, Path]], GeneratorType]) -> None:
-    """
-    Provided a list of file paths, will open and overwrite them in order to delete data while preserving the file name.
+def file_emptier(*, file_list: list[str | Path] | GeneratorType) -> None:
+    """Open and overwrite a list of file paths in order to delete data while preserving the file name.
 
     Parameters
     ----------
-    file_list: List[Union[str, Path]]
-      List of files to be overwritten
+    file_list : list of str or Path, or GeneratorType
+        List of files to be overwritten
 
     Returns
     -------
     None
     """
-
-    file_list = [Path(f) for f in file_list]
-    file_list.sort()
+    file_list = sorted([Path(f) for f in file_list])
 
     logging.info(
         f"Found {len(file_list)} files totalling {report_file_size(file_list)}."
     )
 
     for file in file_list:
         logging.warning(f"Overwriting {file}")
         open(file, "w").close()
 
 
 def delete_by_date(
     *,
-    source: Union[str, Path],
-    year: Optional[int] = None,
-    month: Optional[int] = None,
-    day: Optional[int] = None,
-    pattern: Optional[str] = None,
-    server: Optional[Union[str, Path]] = None,
-    user: Optional[str] = None,
-    password: Optional[str] = None,
-    date_object: Optional[date] = None,
+    source: str | Path,
+    year: int | None = None,
+    month: int | None = None,
+    day: int | None = None,
+    pattern: str | None = None,
+    server: str | Path | None = None,
+    user: str | None = None,
+    password: str | None = None,
+    date_object: date | None = None,
 ) -> None:
-    """
+    """Remove a selection of files based on a given date of last modification.
 
     Parameters
     ----------
-    source: Union[str, Path]
-    year: Optional[int]
-    month: Optional[int]
-    day: Optional[int]
-    pattern: Optional[str]
-    server: Optional[Union[str, Path]]
-    user: Optional[str]
-    password: Optional[str]
-    date_object: Optional[date]
+    source: str or Path
+    year: int, optional
+    month: int, optional
+    day: int, optional
+    pattern: str, optional
+    server: str or Path, optional
+    user: str, optional
+    password: str, optional
+    date_object: date, optional
 
     Returns
     -------
     None
     """
-
     user = user or input("Username:")
     password = password or getpass("Password:")
 
     if year and month and day:
         date_selected = date(year, month, day)
     elif date_object:
         date_selected = date_object
@@ -132,39 +130,38 @@
         context.close()
 
     return
 
 
 def delete_duplicates(
     *,
-    source: Union[str, Path],
-    target: Union[str, Path],
-    server: Optional[Union[str, Path]],
+    source: str | Path,
+    target: str | Path,
+    server: str | Path | None = None,
     user: str = None,
     password: str = None,
     pattern: str = None,
     delete_target_duplicates: bool = False,
 ) -> None:
     """
 
     Parameters
     ----------
-    source : Union[str, Path]
-    target : Union[str, Path]
-    server : Optional[Union[str, Path]]
+    source : str or Path
+    target : str or Path
+    server : str or Path, optional
     user: str
     password : str
     pattern: str
     delete_target_duplicates : bool
 
     Returns
     -------
     None
     """
-
     user = user or input("Username:")
     password = password or getpass("Password:")
     glob_pattern = pattern or "*.nc"
 
     connection = fabric.Connection(
         host=server, user=user, connect_kwargs=dict(password=password)
     )
@@ -198,41 +195,41 @@
         f"Removed { deleted_files} files totalling {report_file_size(freed_space)}."
     )
     return
 
 
 def delete_by_variable(
     *,
-    target: Union[str, Path, List[Union[str, Path]], GeneratorType] = None,
-    variables: List[str] = None,
-    server: Optional[str or Path],
-    user: Optional[str] = None,
-    password: Optional[str] = None,
-    file_suffix: Optional[str] = None,
+    target: str | Path | list[str | Path] | GeneratorType = None,
+    variables: list[str],
+    server: str | Path | None = None,
+    user: str | None = None,
+    password: str | None = None,
+    file_suffix: str | None = None,
     delete: bool = False,
 ) -> None:
-    """
+    """Delete according to variable name.
+
     Given target location(s), a list of variables and a server address, perform a glob search
-     and delete file names starting with the variables identified
+    and delete file names starting with the variables identified
 
     Parameters
     ----------
-    target : Union[str, Path, List[Union[str, Path]], GeneratorType]
-    variables : List[str]
-    server :Optional[Union[str, Path]]
-    user : Optional[str]
-    password : Optional[str]
-    file_suffix : Optional[str]
+    target : str, Path, list of str or Path, or GeneratorType]
+    variables : list of str
+    server : str or Path, optional
+    user : str, optional
+    password : str, optional
+    file_suffix : str, optional
     delete : bool
 
     Returns
     -------
     None
     """
-
     user = user or input("Username:")
     password = password or getpass("Password:")
 
     connection = fabric.Connection(
         host=server, user=user, connect_kwargs=dict(password=password)
     )
```

### Comparing `miranda-0.4.0/miranda/scripting.py` & `miranda-0.5.0/miranda/scripting.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+"""Scripting Helpers module."""
+from __future__ import annotations
+
 import pathlib
 import sys
 from datetime import datetime as dt
 
-MiB = int(pow(2, 20))
-
 _CONSOLE_FORMAT = "%(asctime)s [%(levelname)s] %(name)s: %(message)s"
 _LOGFILE_FORMAT = "%(asctime)s: [%(levelname)s]: %(filename)s(%(funcName)s:%(lineno)s) >>> %(message)s"
 
 __all__ = ["LOGGING_CONFIG"]
 
 LOGGING_CONFIG = {
     "version": 1,
@@ -17,31 +18,27 @@
         "logfile": {"format": _LOGFILE_FORMAT},
     },
     "handlers": {
         "default": {
             "level": "INFO",
             "formatter": "standard",
             "class": "logging.StreamHandler",
-            "stream": "ext://sys.stdout",  # Default is stderr
+            "stream": sys.stdout,
         },
         "rotated_file": {
             "class": "logging.handlers.RotatingFileHandler",
             "formatter": "logfile",
-            "filename": "{}_{}.log".format(
-                dt.now().strftime("%Y%m%d"), pathlib.Path(sys.argv[0]).stem
-            ),
-            "maxBytes": 2 * MiB,
+            "filename": f"{dt.now().strftime('%Y%m%d')}_{pathlib.Path(sys.argv[0]).stem}.log",
+            "maxBytes": 2 * 1024 * 1024,  # 2 MB
             "backupCount": 10,
         },
         "standard_file": {
             "class": "logging.FileHandler",
             "formatter": "logfile",
-            "filename": "{}_{}.log".format(
-                dt.now().strftime("%Y%m%d"), pathlib.Path(sys.argv[0]).stem
-            ),
+            "filename": f"{dt.now().strftime('%Y%m%d')}_{pathlib.Path(sys.argv[0]).stem}.log",
         },
     },
     "loggers": {
         "": {  # root logger
             "handlers": ["default", "standard_file"],
             "level": "INFO",
             "propagate": False,
```

### Comparing `miranda-0.4.0/miranda/storage.py` & `miranda-0.5.0/miranda/storage.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 
 Functions:
 
  * :func:`total_size` - get total size of a list of files.
  * :func:`size_division` - divide files based on number and size restrictions.
 
 """
+from __future__ import annotations
+
 import logging
 import logging.config
 import os
 import subprocess
 from functools import reduce
 from pathlib import Path
 from types import GeneratorType
-from typing import Dict, List, Union
 
 from .scripting import LOGGING_CONFIG
 
 logging.config.dictConfig(LOGGING_CONFIG)
 
 
 __all__ = [
@@ -37,14 +38,16 @@
     "report_file_size",
     "size_division",
     "size_evaluation",
 ]
 
 
 class DiskSpaceError(Exception):
+    """DiskSpaceError Exception."""
+
     pass
 
 
 class FileMeta:
     """File path and size."""
 
     django = {
@@ -60,15 +63,14 @@
         path : str
             full path of the file.
         size : int
             size of file in bytes (default: will obtain from os.path.getsize
             if file exists, set to 0 otherwise).
 
         """
-
         # Make sure we have the full path of the file
         self.path = Path(path).absolute()
 
         # Get size of file if it is not specified
         if (-1 == size) and self.path.exists():
             try:
                 self.size = self.path.stat().st_size
@@ -103,15 +105,14 @@
             space currently used on the medium (default: will obtain from
             system call to 'df').
         free_space : int
             space available on the medium (default: will obtain from system
             call to 'df').
 
         """
-
         # Make sure we have the full base path
         self.base_path = Path(base_path).absolute()
 
         # Get attributes from 'df' function if they are not specified
         if not self.base_path.is_dir():
             raise DiskSpaceError(f"Cannot analyze {self.base_path}.")
         if not Path("/bin/df").exists():
@@ -141,28 +142,27 @@
                 self.free_space = int(df_output_split[3]) * 1000
             except Exception as e:
                 raise DiskSpaceError("/bin/df output not as expected.") from e
         else:
             self.free_space = free_space
 
 
-def size_evaluation(file_list: List[Union[str, FileMeta, Path]]) -> int:
+def size_evaluation(file_list: list[str | FileMeta | Path]) -> int:
     """Total size of files.
 
     Parameters
     ----------
-    file_list : Union[str, Path, FileMeta]
+    file_list : list of str or Path or FileMeta
 
     Returns
     -------
     int
       total size of files in bytes.
 
     """
-
     if file_list:
         size = 0
         for file_to_add in file_list:
             # If file paths are given, convert to FileMeta objects first
             if not isinstance(file_to_add, FileMeta):
                 try:
                     file_to_add = FileMeta(file_to_add)
@@ -171,41 +171,40 @@
             size += file_to_add.size
         return size
     else:
         return 0
 
 
 def size_division(
-    files_to_divide: Union[List, FileMeta, Path],
+    files_to_divide: list | FileMeta | Path,
     size_limit: int = 0,
     file_limit: int = 0,
     check_name_repetition: bool = False,
     preserve_order: bool = False,
-) -> List[list]:
+) -> list[list]:
     """Divide files according to size and number limits.
 
     Parameters
     ----------
-    files_to_divide : Union[List, FileMeta, Path]
+    files_to_divide : list of str or Path, FileMeta, Path
+        Files to be sorted.
     size_limit : int
-      Size limit of divisions in bytes. Default: 0 (no limit).
+        Size limit of divisions in bytes. Default: 0 (no limit).
     file_limit : int
-      Number of files limit of divisions. Default: 0 (no limit).
+        Number of files limit of divisions. Default: 0 (no limit).
     check_name_repetition : bool
-      Flag to prevent file name repetitions. Default: False.
+        Flag to prevent file name repetitions. Default: False.
     preserve_order : bool
-      Flag to force files to be restored in the order they are given. Default: False.
+        Flag to force files to be restored in the order they are given. Default: False.
 
     Returns
     -------
-    List[list]
-      list of divisions (each division is a list of FileMeta objects).
-
+    list[list]
+        list of divisions (each division is a list of FileMeta objects).
     """
-
     divisions = list()
     for file_divide in files_to_divide:
         # If file paths are given, convert to FileMeta objects first
         if not isinstance(file_divide, FileMeta):
             try:
                 file_divide = FileMeta(file_divide)
             except DiskSpaceError:
@@ -236,28 +235,28 @@
                 break
         else:
             divisions.append([file_divide])
     return divisions
 
 
 def file_size(
-    file_path_or_bytes_or_dict: Union[
-        Path,
-        str,
-        int,
-        List[Union[str, Path]],
-        GeneratorType,
-        Dict[str, Union[Path, List[Path]]],
-    ]
+    file_path_or_bytes_or_dict: (
+        Path
+        | str
+        | int
+        | list[str | Path]
+        | GeneratorType
+        | dict[str, Path | list[Path]]
+    )
 ) -> int:
-    """
+    """Return size of object in bytes.
 
     Parameters
     ----------
-    file_path_or_bytes_or_dict : Union[Path, str, int, List[Union[str, Path]], GeneratorType, Dict[str, Union[Path, List[Path]]]]
+    file_path_or_bytes_or_dict : Path or str or int, list of str or Path, GeneratorType, or dict[str, Path or list of Path]
 
     Returns
     -------
     int
     """
     try:
         if isinstance(file_path_or_bytes_or_dict, int):
@@ -298,30 +297,41 @@
         )
         raise
 
     return total
 
 
 def report_file_size(
-    file_path_or_bytes_or_dict: Union[
-        Path, str, int, List[Union[str, Path]], Dict[str, Union[Path, List[Path]]]
-    ],
+    file_path_or_bytes_or_dict: (
+        Path
+        | str
+        | int
+        | list[str | Path]
+        | GeneratorType
+        | dict[str, Path | list[Path]]
+    ),
     use_binary: bool = True,
     significant_digits: int = 2,
 ) -> str:
-    """
+    """Report file size in a human-readable format.
+
     This function will parse the contents of a list or generator of files and return the
     size in bytes of a file or a list of files in pretty formatted text.
+
+    Parameters
+    ----------
+    file_path_or_bytes_or_dict : Path or str or int, list of str or Path, GeneratorType, or dict[str, Path or list of Path]
+    use_binary : bool
+    significant_digits : int
+
     """
     _CONVERSIONS = ["B", "k{}B", "M{}B", "G{}B", "T{}B", "P{}B", "E{}B", "Z{}B", "Y{}B"]
 
     def _size_formatter(i: int, binary: bool = True, precision: int = 2) -> str:
-        """
-        This function will format byte size into an appropriate nomenclature for prettier printing.
-        """
+        """Format byte size into an appropriate nomenclature for prettier printing."""
         import math
 
         base = 1024 if binary else 1000
         if i == 0:
             return "0 B"
         multiple = math.trunc(math.log2(i) / math.log2(base))
         value = i / math.pow(base, multiple)
```

### Comparing `miranda-0.4.0/miranda/structure/_structure.py` & `miranda-0.5.0/miranda/structure/_structure.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
+from __future__ import annotations
+
 import hashlib
 import logging.config
 import multiprocessing
 import os
 import shutil
-import sys
 from functools import partial
 from pathlib import Path
 from types import GeneratorType
-from typing import Dict, List, Optional, Union
 
 import yaml
 from schema import SchemaError
 
 from miranda.cv import VALIDATION_ENABLED
 from miranda.decode import Decoder, DecoderError, guess_project
 from miranda.io import discover_data
@@ -74,18 +74,18 @@
 
     else:
         print(f"Writing sha256sum file `{Path(out_file).name}` exists. Continuing...")
 
 
 def generate_hash_metadata(
     in_file: os.PathLike,
-    version: Optional[str] = None,
-    hash_file: Optional[os.PathLike] = None,
+    version: str | None = None,
+    hash_file: os.PathLike | None = None,
     verify: bool = False,
-) -> Dict[str, List[str]]:
+) -> dict[str, list[str]]:
     hashversion = dict()
 
     if version is None:
         version = "vNotFound"
 
     if not Path(hash_file).exists():
         hash_sha256_writer = hashlib.sha256()
@@ -109,20 +109,34 @@
 
         hashversion[Path(in_file).name] = [version, calculated_sha256sum]
 
     return hashversion
 
 
 def create_version_hash_files(
-    input_files: Optional[
-        Union[str, os.PathLike, List[Union[str, os.PathLike]], GeneratorType]
-    ] = None,
-    facet_dict: Optional[Dict] = None,
+    input_files: str
+    | os.PathLike
+    | list[str | os.PathLike]
+    | GeneratorType
+    | None = None,
+    facet_dict: dict | None = None,
     verify_hash: bool = False,
 ) -> None:
+    """Create version hashes based on files or a facets dictionary.
+
+    Parameters
+    ----------
+    input_files : str, os.PathLike, list of str or os.PathLike, or GeneratorType
+    facet_dict : dict, optional
+    verify_hash : bool
+
+    Returns
+    -------
+    None
+    """
     if not facet_dict and not input_files:
         raise ValueError("Facets dictionary or sequence of filepaths required.")
 
     if input_files:
         if isinstance(input_files, os.PathLike):
             input_files = [input_files]
         for f in input_files:
@@ -149,16 +163,16 @@
             zip(version_hash_paths.keys(), version_hash_paths.values()),
         )
         pool.close()
         pool.join()
 
 
 def _structure_datasets(
-    in_file: Union[str, os.PathLike],
-    out_path: Union[str, os.PathLike],
+    in_file: str | os.PathLike,
+    out_path: str | os.PathLike,
     method: str,
     dry_run: bool = False,
 ):
     if isinstance(in_file, str):
         in_file = Path(in_file)
 
     if method.lower() in ["move", "copy"]:
@@ -166,27 +180,22 @@
         output_file = Path(out_path).joinpath(in_file.name)
         try:
             if not dry_run:
                 method_mod = ""
                 if in_file.is_dir() and method.lower() == "copy":
                     method_mod = "tree"
 
-                if sys.version_info < (3, 9):
-                    getattr(shutil, f"{method}{method_mod}")(
-                        str(in_file), str(output_file)
-                    )
-                else:
-                    getattr(shutil, f"{method}{method_mod}")(in_file, output_file)
+                getattr(shutil, f"{method}{method_mod}")(in_file, output_file)
             print(f"{meth} {in_file.name} to {output_file}.")
         except FileExistsError:
             print(f"{in_file.name} already exists at location. Continuing...")
 
 
 def parse_schema(
-    facets: dict, schema: Union[str, os.PathLike, dict], top_folder: str = "datasets"
+    facets: dict, schema: str | os.PathLike | dict, top_folder: str = "datasets"
 ) -> list:
     """Parse the schema from a YAML schema configuration and construct path using a dictionary of facets.
 
     Parameters
     ----------
     facets : dict
     schema : str or os.PathLike or dict
@@ -268,19 +277,19 @@
     tree.extend(_parse_structure(branch, facets))
 
     return tree
 
 
 def build_path_from_schema(
     facets: dict,
-    output_folder: Union[str, os.PathLike],
-    schema: Optional[Union[str, os.PathLike, dict]] = None,
+    output_folder: str | os.PathLike,
+    schema: str | os.PathLike | dict | None = None,
     top_folder: str = "datasets",
     validate: bool = True,
-) -> Optional[Path]:
+) -> Path | None:
     """Build a filepath based on a valid data schema.
 
     Parameters
     ----------
     facets : dict
         Facets for a given dataset.
     output_folder : str or os.PathLike
@@ -292,15 +301,14 @@
     validate: bool
         Run facets-validation checks over given file. Default: True.
 
     Returns
     -------
     Path or None
     """
-
     if schema is None:
         schema = Path(__file__).parent.joinpath("data").joinpath("ouranos_schema.yml")
 
     tree = parse_schema(facets, schema, top_folder)
     branch = tree[0]
 
     if validate and VALIDATION_ENABLED:
@@ -327,33 +335,34 @@
     for facet in tree:
         # Remove spaces in folder paths
         file_location.append(str(facets[facet]).replace(" ", "-"))
     return Path(output_folder).joinpath("/".join(file_location))
 
 
 def structure_datasets(
-    input_files: Union[str, os.PathLike, List[Union[str, os.PathLike]], GeneratorType],
-    output_folder: Union[str, os.PathLike],
+    input_files: str | os.PathLike | list[str | os.PathLike] | GeneratorType,
+    output_folder: str | os.PathLike,
     *,
-    project: Optional[str] = None,
+    project: str | None = None,
     guess: bool = True,
     dry_run: bool = False,
     method: str = "copy",
     make_dirs: bool = False,
     set_version_hashes: bool = False,
     verify_hashes: bool = False,
     suffix: str = "nc",
-) -> Dict[Path, Path]:
+) -> dict[Path, Path]:
     """
 
     Parameters
     ----------
-    input_files : str or Path or list of str or Path or GeneratorType
+    input_files : str, Path, list of str or Path, or GeneratorType
+        Files to be sorted.
     output_folder : str or Path
-
+        The desired location for the folder-tree.
     project : {"cordex", "cmip5", "cmip6", "isimip-ft", "pcic-candcs-u6", "converted"}, optional
         Project used to parse the facets of all supplied datasets.
         If not supplied, will attempt parsing with all available data categories for each file (slow)
         unless `guess` is True.
     guess : bool
         If project not supplied, suggest to decoder that activity is the same for all input_files. Default: True.
     dry_run : bool
@@ -368,15 +377,15 @@
         Ensure that any existing she256sum files correspond with companion file. Raise on error. Default: False.
     suffix : {"nc", "zarr"}
         If "zarr", will perform a 'glob' with provided pattern.
         Otherwise, will perform an 'rglob' (recursive) operation.
 
     Returns
     -------
-    Dict[Path, Path]
+    dict[Path, Path]
     """
     input_files = discover_data(input_files, suffix)
     if guess and project is None:
         # Examine the first file from a list or generator
         for f in input_files:
             project = guess_project(f)
             decoder = Decoder(project)
```

### Comparing `miranda-0.4.0/miranda/structure/data/ouranos_schema.yml` & `miranda-0.5.0/miranda/structure/data/ouranos_schema.yml`

 * *Files 18% similar despite different names*

```diff
@@ -23,14 +23,16 @@
   - option: type
     value: reconstruction
     structure:
       - type
       - institution
       - source
       - domain
+      - option: member
+        is_true: member
       - frequency
       - variable
   - option: type
     value: simulation
     structure:
       - type
       - processing_level
```

### Comparing `miranda-0.4.0/miranda/units.py` & `miranda-0.5.0/miranda/units.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,53 @@
+"""Special Time Units-Handling submodule."""
+from __future__ import annotations
+
 import logging
-from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 from xclim.core.calendar import parse_offset
 
 KiB = int(pow(2, 10))
 MiB = int(pow(2, 20))
 GiB = int(pow(2, 30))
 
 
 def get_time_frequency(
     d: xr.Dataset,
-    expected_period: Optional[str] = None,
+    expected_period: str | None = None,
     minimum_continuous_period: str = "1M",
-) -> Tuple[List[Union[int, str]], str]:
+) -> tuple[list[int | str], str]:
     """Try to understand the Dataset frequency.
 
     If it can't be inferred with :py:func:`xarray.infer_freq` it tries to:
     - look for a "freq" attrs in the global or time variable attributes.
     - infer monthly frequency if all time steps are between 27 and 32 days
 
     In the event that an `expected_period` is supplied, special handling will be called allowing for determining data
     that may be internally discontinuous (e.g. discontinuous overall, but continuous for `minimum_continuous_period`).
     This is provided for instances where input data in a multifile dataset is sparse.
 
     Parameters
     ----------
     d : xr.Dataset
+        An xarray.Dataset.
     expected_period : str
-        An xarray-compatible time period (e.g. "1H", "1D", "7D", "1M", "1A")
+        An xarray-compatible time period (e.g. "1H", "1D", "7D", "1M", "1A").
         The time period expected of the input dataset.
         The "1M" period is specially-handled.
     minimum_continuous_period : str
-        An xarray-compatible time period (e.g. "1H", "1D", "7D", "1M", "1A")
+        An xarray-compatible time period (e.g. "1H", "1D", "7D", "1M", "1A").
         The minimum expected granular period that data should have continuous values for.
         The "1M" period is specially-handled.
 
     Returns
     -------
-    offset : List[Union[int, str]]
+    offset : list of int or str
         The offset a list of (multiplier, base)
     offset_meaning : str
         The offset meaning (single word)
 
     """
     if expected_period is not None:
         if not [expected_period.endswith(end) for end in ["H", "D", "M", "A"]]:
```

### Comparing `miranda-0.4.0/miranda/utils.py` & `miranda-0.5.0/miranda/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+"""Miscellaneous Helper Utilities module."""
+from __future__ import annotations
+
 import gzip
 import logging.config
 import os
 import re
 import sys
 import tarfile
 import tempfile
 import warnings
 import zipfile
+from collections.abc import Iterable, Sequence
 from contextlib import contextmanager
 from io import StringIO
 from pathlib import Path
-from typing import Dict, Iterable, List, Optional, Sequence, TextIO, Union
+from typing import TextIO
 
 from .scripting import LOGGING_CONFIG
 
 logging.config.dictConfig(LOGGING_CONFIG)
 
 __all__ = [
     "HiddenPrints",
@@ -30,17 +34,22 @@
 ISO_8601 = (
     r"^(-?(?:[1-9][0-9]*)?[0-9]{4})-(1[0-2]|0[1-9])-(3[01]|0[1-9]|[12][0-9])"
     r"T(2[0-3]|[01][0-9]):([0-5][0-9]):([0-5][0-9])(\.[0-9]+)?(Z|[+-](?:2[0-3]|[01][0-9]):[0-5][0-9])?$"
 )
 
 
 class HiddenPrints:
-    # Solution from https://stackoverflow.com/a/45669280/7322852
-    # Credit to Alexander C (https://stackoverflow.com/users/2039471/alexander-c)
-    # CC-BY-SA 4.0 (https://creativecommons.org/licenses/by-sa/4.0/)
+    """Special context manager for hiding print statements.
+
+    Notes
+    -----
+    Solution from https://stackoverflow.com/a/45669280/7322852
+    Credit to Alexander C (https://stackoverflow.com/users/2039471/alexander-c)
+    CC-BY-SA 4.0 (https://creativecommons.org/licenses/by-sa/4.0/)-
+    """
 
     def __enter__(self):
         self._original_stdout = sys.stdout
         sys.stdout = open(os.devnull, "w")
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         sys.stdout.close()
@@ -64,28 +73,27 @@
         except StopIteration:
             if chunk:
                 yield chunk
             break
 
 
 @contextmanager
-def working_directory(directory: Union[str, Path]) -> None:
+def working_directory(directory: str | Path) -> None:
     """Change the working directory within a context object.
 
     This function momentarily changes the working directory within the context and reverts to the file working directory
     when the code block it is acting upon exits
 
     Parameters
     ----------
-    directory: Union[str, Path]
+    directory : str or pathlib.Path
 
     Returns
     -------
     None
-
     """
     owd = os.getcwd()
 
     if (2, 7) < sys.version_info < (3, 6):
         directory = str(directory)
 
     try:
@@ -114,32 +122,31 @@
     has_another_true = any(
         iterator
     )  # carry on consuming until another true value / exhausted
     return has_true and not has_another_true  # True if exactly one true found
 
 
 def generic_extract_archive(
-    resources: Union[str, Path, List[Union[bytes, str, Path]]],
-    output_dir: Optional[Union[str, Path]] = None,
-) -> List[Path]:
+    resources: str | Path | list[bytes | str | Path],
+    output_dir: str | Path | None = None,
+) -> list[Path]:
     """Extract archives (tar/zip) to a working directory.
 
     Parameters
     ----------
-    resources : Union[str, Path, List[Union[bytes, str, Path]]]
+    resources : str or Path or list of bytes or str or Path
         list of archive files (if netCDF files are in list, they are passed and returned as well in the return).
-    output_dir : Optional[Union[str, Path]]
+    output_dir : str or Path, optional
         string or Path to a working location (default: temporary folder).
 
     Returns
     -------
     list
         List of original or of extracted files
     """
-
     archive_types = [".gz", ".tar", ".zip", ".7z"]
     output_dir = output_dir or tempfile.gettempdir()
 
     if not isinstance(resources, list):
         resources = [resources]
 
     files = list()
@@ -188,43 +195,42 @@
     return files
 
 
 ########################################################################################
 
 
 def list_paths_with_elements(
-    base_paths: Union[str, List[str]], elements: List[str]
-) -> List[Dict]:
+    base_paths: str | list[str], elements: list[str]
+) -> list[dict]:
     """List a given path structure.
 
     Parameters
     ----------
-    base_paths : List[str]
-        list of paths from which to start the search.
-    elements : List[str]
-        ordered list of the expected elements.
+    base_paths : list of str
+        List of paths from which to start the search.
+    elements : list of str
+        Ordered list of the expected elements.
 
     Returns
     -------
-    List[Dict]
+    list of dict
         The keys are 'path' and each of the members of the given elements, the path is the absolute path.
 
     Notes
     -----
     Suppose you have the following structure: /base_path/{color}/{shape}
     The resulting list would look like::
 
          [{'path':/base_path/red/square, 'color':'red', 'shape':'square'},
          {'path':/base_path/red/circle, 'color':'red', 'shape':'circle'},
          {'path':/base_path/blue/triangle, 'color':'blue', 'shape':'triangle'},
          ...]
 
     Obviously, 'path' should not be in the input list of elements.
     """
-
     # Make sure the base_paths input is a list of absolute path
     paths = list()
     if not hasattr(base_paths, "__iter__"):
         paths.append(base_paths)
     paths = map(os.path.abspath, base_paths)
     # If elements list is empty, return empty list (end of recursion).
     if not elements:
@@ -250,16 +256,16 @@
         elif len(elements) == 1:
             for my_path, my_item in zip(next_base_paths, path_content):
                 paths_elements.append({"path": my_path, elements[0]: my_item})
     return paths_elements
 
 
 def publish_release_notes(
-    style: str = "md", file: Optional[Union[os.PathLike, StringIO, TextIO]] = None
-) -> Optional[str]:
+    style: str = "md", file: os.PathLike | StringIO | TextIO | None = None
+) -> str | None:
     """Format release history in Markdown or ReStructuredText.
 
     Parameters
     ----------
     style : {"rst", "md"}
         Use ReStructuredText formatting or Markdown. Default: Markdown.
     file : {os.PathLike, StringIO, TextIO}, optional
@@ -325,26 +331,26 @@
     if not file:
         return history
     if isinstance(file, (Path, os.PathLike)):
         file = Path(file).open("w")
     print(history, file=file)
 
 
-def read_privileges(location: Union[Path, str], strict: bool = False) -> bool:
+def read_privileges(location: str | Path, strict: bool = False) -> bool:
     """Determine whether a user has read privileges to a specific file.
 
     Parameters
     ----------
-    location: Union[Path, str]
+    location: str or Path
     strict: bool
 
     Returns
     -------
     bool
-      Whether the current user shell has read privileges
+        Whether the current user shell has read privileges
     """
     msg = ""
     try:
         if Path(location).exists():
             if os.access(location, os.R_OK):
                 msg = f"{location} is read OK!"
                 logging.info(msg)
```

### Comparing `miranda-0.4.0/miranda/validators.py` & `miranda-0.5.0/miranda/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""Data Validation module."""
+from __future__ import annotations
+
 import re
 import typing
 
 import pandas as pd
 from pandas._libs.tslibs import NaTType  # noqa
 from schema import Literal, Optional, Or, Regex, Schema
 
@@ -142,15 +145,15 @@
         {
             data_type: GRIDDED_SCHEMA
             for data_type in ["forecast", "gridded-obs", "reconstruction"]
         }
     )
 
 
-def url_validate(target: str) -> typing.Optional[typing.Match[str]]:
+def url_validate(target: str) -> typing.Match[str] | None:
     """Validate whether a supplied URL is reliably written.
 
     Parameters
     ----------
     target : str
 
     References
```

### Comparing `miranda-0.4.0/setup.cfg` & `miranda-0.5.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 [bumpversion]
-current_version = 0.4.0
+current_version = 0.5.0
 commit = True
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+).(?P<patch>\d+)(\-(?P<release>[a-z]+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}
 	{major}.{minor}.{patch}
 
 [bumpversion:part:release]
 optional_value = gamma
 values = 
 	beta
 	gamma
 
-[bumpversion:file:setup.py]
-search = VERSION = "{current_version}"
-replace = VERSION = "{new_version}"
-
 [bumpversion:file:miranda/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
 [flake8]
 exclude = 
 	.git,
@@ -36,21 +32,14 @@
 	E266
 	E501
 	F401
 	F403
 	W503
 	W504
 
-[coverage:run]
-relative_files = True
-
-[isort]
-profile = black
-py_version = 37
-
 [aliases]
 test = pytest
 
 [tool:pytest]
 addopts = 
 	--verbose
 	--color=yes
@@ -65,13 +54,26 @@
 	line-too-long,
 	protected-access,
 	too-few-public-methods,
 	too-many-arguments,
 
 [pydocstyle]
 convention = numpy
-match = ((?!test_).)*\.py
-
-[egg_info]
-tag_build = 
-tag_date = 0
-
+add-ignore = 
+	D105,
+	D205,
+	D400,
+	D401,
+	D403
+match = ((?!(test_|conf)).)*\.py
+
+[pycodestyle]
+count = False
+exclude = tests
+ignore = 
+	E203,
+	E226,
+	E402,
+	E501,
+	W503
+max-line-length = 120
+statistics = True
```

