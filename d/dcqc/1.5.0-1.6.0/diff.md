# Comparing `tmp/dcqc-1.5.0.tar.gz` & `tmp/dcqc-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcqc-1.5.0.tar", last modified: Wed Jun 14 16:34:35 2023, max compression
+gzip compressed data, was "dcqc-1.6.0.tar", last modified: Mon Jun 19 21:07:28 2023, max compression
```

## Comparing `dcqc-1.5.0.tar` & `dcqc-1.6.0.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:34:35.594009 dcqc-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-14 16:33:37.000000 dcqc-1.5.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:34:35.582008 dcqc-1.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:34:35.586009 dcqc-1.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-14 16:33:37.000000 dcqc-1.5.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-14 16:33:37.000000 dcqc-1.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 16:33:37.000000 dcqc-1.5.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-14 16:33:37.000000 dcqc-1.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-14 16:33:37.000000 dcqc-1.5.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-14 16:33:37.000000 dcqc-1.5.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-14 16:33:37.000000 dcqc-1.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-06-14 16:33:37.000000 dcqc-1.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 16:33:37.000000 dcqc-1.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-14 16:34:35.594009 dcqc-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-14 16:33:37.000000 dcqc-1.5.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)   102584 2023-06-14 16:33:37.000000 dcqc-1.5.0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-14 16:33:37.000000 dcqc-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:34:35.586009 dcqc-1.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-14 16:33:37.000000 dcqc-1.5.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:34:35.586009 dcqc-1.5.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-14 16:33:37.000000 dcqc-1.5.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 16:33:37.000000 dcqc-1.5.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-14 16:33:37.000000 dcqc-1.5.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-06-14 16:33:37.000000 dcqc-1.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-14 16:33:37.000000 dcqc-1.5.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-14 16:33:37.000000 dcqc-1.5.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-14 16:33:37.000000 dcqc-1.5.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-14 16:33:37.000000 dcqc-1.5.0/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-14 16:33:37.000000 dcqc-1.5.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-14 16:33:37.000000 dcqc-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-14 16:34:35.598009 dcqc-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-14 16:33:37.000000 dcqc-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:34:35.586009 dcqc-1.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:34:35.590009 dcqc-1.5.0/src/dcqc/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12514 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:34:35.590009 dcqc-1.5.0/src/dcqc/suites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/suites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/suites/suite_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/suites/suites.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:34:35.590009 dcqc-1.5.0/src/dcqc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/tests/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/tests/bioformats_info_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/tests/file_extension_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/tests/grep_date_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/tests/json_load_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/tests/jsonld_load_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/tests/libtiff_info_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/tests/md5_checksum_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/tests/ome_xml_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/tests/paired_fastq_parity_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/tests/tiff_tag_306_date_time_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/updaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/dcqc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:34:35.590009 dcqc-1.5.0/src/dcqc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-14 16:34:35.000000 dcqc-1.5.0/src/dcqc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-14 16:34:35.000000 dcqc-1.5.0/src/dcqc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:34:35.000000 dcqc-1.5.0/src/dcqc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-14 16:34:35.000000 dcqc-1.5.0/src/dcqc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:34:35.000000 dcqc-1.5.0/src/dcqc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-14 16:34:35.000000 dcqc-1.5.0/src/dcqc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 16:34:35.000000 dcqc-1.5.0/src/dcqc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:34:35.590009 dcqc-1.5.0/src/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-14 16:33:37.000000 dcqc-1.5.0/src/docker/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:34:35.594009 dcqc-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:34:35.594009 dcqc-1.5.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    76770 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/circuit.tif
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/empty_input.csv
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/example.bam
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/example.fastq
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/example.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/example.jsonld
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/example.tsv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/fastq1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/fastq2.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/file.json
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/files.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)     2085 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/input.csv
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/small.csv
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/suite.json
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/suites.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:34:35.594009 dcqc-1.5.0/tests/data/suites_files/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/suites_files/suites_1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/suites_files/suites_2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/suites_files/suites_3.json
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/target.json
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/test.computed.json
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/test.external.json
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/test.internal.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/test_contains_word_date.txt
--rw-r--r--   0 runner    (1001) docker     (123)   262517 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/test_image_dirty_datetime.tif
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/test_input.csv
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/test_output.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/tests.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:34:35.594009 dcqc-1.5.0/tests/data/tiffinfo/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/tiffinfo/exit_code.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/tiffinfo/std_err.txt
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/data/tiffinfo/std_out.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/test_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/test_suites.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/test_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/test_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-14 16:33:37.000000 dcqc-1.5.0/tests/test_updaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-14 16:33:37.000000 dcqc-1.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:07:28.426689 dcqc-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-19 21:06:34.000000 dcqc-1.6.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:07:28.414689 dcqc-1.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:07:28.414689 dcqc-1.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-19 21:06:34.000000 dcqc-1.6.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-19 21:06:34.000000 dcqc-1.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-19 21:06:34.000000 dcqc-1.6.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-19 21:06:34.000000 dcqc-1.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-19 21:06:34.000000 dcqc-1.6.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-19 21:06:34.000000 dcqc-1.6.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-19 21:06:34.000000 dcqc-1.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-06-19 21:06:34.000000 dcqc-1.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 21:06:34.000000 dcqc-1.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-19 21:07:28.426689 dcqc-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-19 21:06:34.000000 dcqc-1.6.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)   102584 2023-06-19 21:06:34.000000 dcqc-1.6.0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-19 21:06:34.000000 dcqc-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:07:28.418689 dcqc-1.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-19 21:06:34.000000 dcqc-1.6.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:07:28.418689 dcqc-1.6.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 21:06:34.000000 dcqc-1.6.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 21:06:34.000000 dcqc-1.6.0/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-19 21:06:34.000000 dcqc-1.6.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-06-19 21:06:34.000000 dcqc-1.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-19 21:06:34.000000 dcqc-1.6.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-19 21:06:34.000000 dcqc-1.6.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-19 21:06:34.000000 dcqc-1.6.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-19 21:06:34.000000 dcqc-1.6.0/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-19 21:06:34.000000 dcqc-1.6.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-19 21:06:34.000000 dcqc-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-19 21:07:28.426689 dcqc-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-19 21:06:34.000000 dcqc-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:07:28.414689 dcqc-1.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:07:28.418689 dcqc-1.6.0/src/dcqc/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12514 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:07:28.418689 dcqc-1.6.0/src/dcqc/suites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/suites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/suites/suite_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/suites/suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:07:28.418689 dcqc-1.6.0/src/dcqc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/tests/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/tests/bioformats_info_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/tests/file_extension_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/tests/grep_date_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/tests/json_load_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/tests/jsonld_load_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/tests/libtiff_info_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/tests/md5_checksum_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/tests/ome_xml_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/tests/paired_fastq_parity_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/tests/tiff_tag_306_date_time_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/updaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/dcqc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:07:28.418689 dcqc-1.6.0/src/dcqc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-19 21:07:28.000000 dcqc-1.6.0/src/dcqc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-19 21:07:28.000000 dcqc-1.6.0/src/dcqc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 21:07:28.000000 dcqc-1.6.0/src/dcqc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-19 21:07:28.000000 dcqc-1.6.0/src/dcqc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 21:07:28.000000 dcqc-1.6.0/src/dcqc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-19 21:07:28.000000 dcqc-1.6.0/src/dcqc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 21:07:28.000000 dcqc-1.6.0/src/dcqc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:07:28.418689 dcqc-1.6.0/src/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-19 21:06:34.000000 dcqc-1.6.0/src/docker/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:07:28.422689 dcqc-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:07:28.422689 dcqc-1.6.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    76770 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/circuit.tif
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/empty_input.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/example.bam
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/example.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/example.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/example.jsonld
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/example.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/fastq1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/fastq2.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/file.json
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/files.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2085 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/input.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/small.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/suite.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/suites.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:07:28.422689 dcqc-1.6.0/tests/data/suites_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/suites_files/suites_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/suites_files/suites_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/suites_files/suites_3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/target.json
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/test.computed.json
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/test.external.json
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/test.internal.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/test_contains_word_date.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   262517 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/test_image_dirty_datetime.tif
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/test_input.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/test_output.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/tests.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:07:28.426689 dcqc-1.6.0/tests/data/tiffinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/tiffinfo/exit_code.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/tiffinfo/std_err.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/data/tiffinfo/std_out.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/test_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/test_suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/test_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/test_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-19 21:06:34.000000 dcqc-1.6.0/tests/test_updaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-19 21:06:34.000000 dcqc-1.6.0/tox.ini
```

### Comparing `dcqc-1.5.0/.coveragerc` & `dcqc-1.6.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/.github/workflows/ci.yml` & `dcqc-1.6.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/.gitignore` & `dcqc-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/.pre-commit-config.yaml` & `dcqc-1.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/CONTRIBUTING.md` & `dcqc-1.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/LICENSE.txt` & `dcqc-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/PKG-INFO` & `dcqc-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcqc
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python package for performing quality control (QC) for data coordination (DC)
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Bruno Grande
 Author-email: bruno.grande@sagebase.org
 License: Apache-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `dcqc-1.5.0/Pipfile.lock` & `dcqc-1.6.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/README.md` & `dcqc-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/docs/Makefile` & `dcqc-1.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/docs/conf.py` & `dcqc-1.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/docs/index.md` & `dcqc-1.6.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/pyproject.toml` & `dcqc-1.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/setup.cfg` & `dcqc-1.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/setup.py` & `dcqc-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/src/dcqc/__init__.py` & `dcqc-1.6.0/src/dcqc/__init__.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/src/dcqc/file.py` & `dcqc-1.6.0/src/dcqc/file.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/src/dcqc/main.py` & `dcqc-1.6.0/src/dcqc/main.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/src/dcqc/mixins.py` & `dcqc-1.6.0/src/dcqc/mixins.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/src/dcqc/parsers.py` & `dcqc-1.6.0/src/dcqc/parsers.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/src/dcqc/reports.py` & `dcqc-1.6.0/src/dcqc/reports.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/src/dcqc/suites/suite_abc.py` & `dcqc-1.6.0/src/dcqc/suites/suite_abc.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/src/dcqc/suites/suites.py` & `dcqc-1.6.0/src/dcqc/suites/suites.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/src/dcqc/target.py` & `dcqc-1.6.0/src/dcqc/target.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/src/dcqc/tests/__init__.py` & `dcqc-1.6.0/src/dcqc/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/src/dcqc/tests/base_test.py` & `dcqc-1.6.0/src/dcqc/tests/base_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -149,14 +149,15 @@
         command_args = shlex.split(command)
         dictionary["command_args"] = command_args
         process = cls(**dictionary)
         return process
 
 
 class ExternalTestMixin(BaseTest):
+    pass_code: ClassVar[str]
     # Class attributes
     is_external_test = True
 
     # Class constants
     STDOUT_PATH: ClassVar[Path]
     STDOUT_PATH = Path("std_out.txt")
     STDERR_PATH: ClassVar[Path]
@@ -191,20 +192,35 @@
                 raise FileNotFoundError(message)
         return outputs
 
     def _interpret_process_outputs(self, outputs: dict[str, Path]) -> TestStatus:
         """Interpret the process output files to yield a test status."""
         exit_code = outputs["exit_code"].read_text()
         exit_code = exit_code.strip()
-        if exit_code == "0":
+        if exit_code == self.pass_code:
             status = TestStatus.PASS
         else:
             status = TestStatus.FAIL
         return status
 
+    # TODO: make changes to this package or the nextflow
+    # workflow so that file mounting is handled cleaner
+    @staticmethod
+    def _short_string_path(path: Path, substring: str) -> str:
+        # chech if substring is in path
+        if substring not in path.as_posix():
+            raise ValueError(f"{substring} not in {path}")
+        # get index where staged folder is
+        index = next(i for i, item in enumerate(path.parts) if substring in item)
+        # shorten path starting from staged folder
+        short_path = Path(*path.parts[index:])
+        # wrap path string in quotes
+        quote_path = str(short_path)
+        return f"'{quote_path}'"
+
     # TODO: Include process in serialized test dictionary
     # def to_dict(self):
     #     dictionary = super(ExternalTestMixin, self).to_dict()
     #     process = self.generate_process()
     #     dictionary["process"] = process.to_dict()
     #     return dictionary
```

### Comparing `dcqc-1.5.0/src/dcqc/tests/bioformats_info_test.py` & `dcqc-1.6.0/src/dcqc/tests/bioformats_info_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/src/dcqc/tests/file_extension_test.py` & `dcqc-1.6.0/src/dcqc/tests/file_extension_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/src/dcqc/tests/grep_date_test.py` & `dcqc-1.6.0/src/dcqc/tests/grep_date_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from dcqc.target import SingleTarget
 from dcqc.tests.base_test import ExternalBaseTest, Process
 
 
 class GrepDateTest(ExternalBaseTest):
     tier = 4
+    pass_code = "1"
     target: SingleTarget
 
     def generate_process(self) -> Process:
         path = self.target.file.stage()
+        string_path = self._short_string_path(path, "dcqc-staged-")
+
         command_args = [
-            "!",  # negate exit status
             "grep",
             "-E",  # extended regular expression
             "-i",  # case insensitive
             "-a",  # treat input as text
             "-q",  # suppress output
             "'date|time'",  # match date or time
-            path,
+            string_path,
         ]
         process = Process(
             container="quay.io/biocontainers/coreutils:8.30--h14c3975_1000",
             command_args=command_args,
         )
         return process
```

### Comparing `dcqc-1.5.0/src/dcqc/tests/json_load_test.py` & `dcqc-1.6.0/src/dcqc/tests/json_load_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/src/dcqc/tests/jsonld_load_test.py` & `dcqc-1.6.0/src/dcqc/tests/jsonld_load_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/src/dcqc/tests/md5_checksum_test.py` & `dcqc-1.6.0/src/dcqc/tests/md5_checksum_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/src/dcqc/tests/ome_xml_schema_test.py` & `dcqc-1.6.0/src/dcqc/tests/ome_xml_schema_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/src/dcqc/tests/paired_fastq_parity_test.py` & `dcqc-1.6.0/src/dcqc/tests/paired_fastq_parity_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/src/dcqc/tests/tiff_tag_306_date_time_test.py` & `dcqc-1.6.0/src/dcqc/tests/tiff_tag_306_date_time_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from dcqc.target import SingleTarget
 from dcqc.tests.base_test import ExternalBaseTest, Process
 
 
 class TiffTag306DateTimeTest(ExternalBaseTest):
     tier = 4
+    pass_code = "1"
     target: SingleTarget
 
     def generate_process(self) -> Process:
         path = self.target.file.stage()
+        string_path = self._short_string_path(path, "dcqc-staged-")
+
         command_args = [
-            "!",  # negate exit status
             "tifftools",
             "dump",
-            path,
+            string_path,
             "|",
             "grep",  # pipe the output
             "-a",  # treat input as text
             "-q",  # suppress output
             "'DateTime 306 (0x132) ASCII'",  # match the DateTime 306 tag
         ]
         process = Process(
```

### Comparing `dcqc-1.5.0/src/dcqc/updaters.py` & `dcqc-1.6.0/src/dcqc/updaters.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/src/dcqc/utils.py` & `dcqc-1.6.0/src/dcqc/utils.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/src/dcqc.egg-info/PKG-INFO` & `dcqc-1.6.0/src/dcqc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcqc
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python package for performing quality control (QC) for data coordination (DC)
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Bruno Grande
 Author-email: bruno.grande@sagebase.org
 License: Apache-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `dcqc-1.5.0/src/dcqc.egg-info/SOURCES.txt` & `dcqc-1.6.0/src/dcqc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/tests/conftest.py` & `dcqc-1.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/tests/data/circuit.tif` & `dcqc-1.6.0/tests/data/circuit.tif`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/tests/data/example.jsonld` & `dcqc-1.6.0/tests/data/example.jsonld`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/tests/data/files.csv` & `dcqc-1.6.0/tests/data/files.csv`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/tests/data/generate.py` & `dcqc-1.6.0/tests/data/generate.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/tests/data/suite.json` & `dcqc-1.6.0/tests/data/suite.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/tests/data/suites.json` & `dcqc-1.6.0/tests/data/suites.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/tests/data/suites_files/suites_1.json` & `dcqc-1.6.0/tests/data/suites_files/suites_1.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/tests/data/suites_files/suites_2.json` & `dcqc-1.6.0/tests/data/suites_files/suites_2.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/tests/data/suites_files/suites_3.json` & `dcqc-1.6.0/tests/data/suites_files/suites_3.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/tests/data/test_image_dirty_datetime.tif` & `dcqc-1.6.0/tests/data/test_image_dirty_datetime.tif`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/tests/data/tests.json` & `dcqc-1.6.0/tests/data/tests.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/tests/test_acceptance.py` & `dcqc-1.6.0/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/tests/test_file.py` & `dcqc-1.6.0/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/tests/test_main.py` & `dcqc-1.6.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/tests/test_parsers.py` & `dcqc-1.6.0/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/tests/test_reports.py` & `dcqc-1.6.0/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/tests/test_suites.py` & `dcqc-1.6.0/tests/test_suites.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/tests/test_target.py` & `dcqc-1.6.0/tests/test_target.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/tests/test_tests.py` & `dcqc-1.6.0/tests/test_tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -86,31 +86,32 @@
             abc_index = mro.index(BaseTest)
             assert mixin_index < abc_index
 
 
 def test_that_the_libtiff_info_test_correctly_interprets_exit_code_0_and_1(
     test_files, mocker
 ):
+    # 0 is pass, 1 is fail
     tiff_file = test_files["tiff"]
     target = SingleTarget(tiff_file)
     with TemporaryDirectory() as tmp_dir:
         path_0 = Path(tmp_dir, "code_0.txt")
         path_1 = Path(tmp_dir, "code_1.txt")
         path_0.write_text("0")
         path_1.write_text("1")
-        good_outputs = {"std_out": path_1, "std_err": path_1, "exit_code": path_0}
-        bad_outputs = {"std_out": path_0, "std_err": path_0, "exit_code": path_1}
+        pass_outputs = {"std_out": path_1, "std_err": path_1, "exit_code": path_0}
+        fail_outputs = {"std_out": path_0, "std_err": path_0, "exit_code": path_1}
 
         test = tests.LibTiffInfoTest(target)
-        mocker.patch.object(test, "_find_process_outputs", return_value=good_outputs)
+        mocker.patch.object(test, "_find_process_outputs", return_value=pass_outputs)
         test_status = test.get_status()
         assert test_status == TestStatus.PASS
 
         test = tests.LibTiffInfoTest(target)
-        mocker.patch.object(test, "_find_process_outputs", return_value=bad_outputs)
+        mocker.patch.object(test, "_find_process_outputs", return_value=fail_outputs)
         test_status = test.get_status()
         assert test_status == TestStatus.FAIL
 
 
 def test_that_the_libtiff_info_test_command_is_produced(test_targets):
     target = test_targets["tiff"]
     test = tests.LibTiffInfoTest(target)
@@ -179,31 +180,32 @@
     process_from_dict = Process.from_dict(process_dict)
     assert process_dict == process_from_dict.to_dict()
 
 
 def test_that_the_grep_date_test_correctly_interprets_exit_code_0_and_1(
     test_files, mocker
 ):
+    # 1 is pass, 0 is fail
     tiff_file = test_files["tiff"]
     target = SingleTarget(tiff_file)
     with TemporaryDirectory() as tmp_dir:
         path_0 = Path(tmp_dir, "code_0.txt")
         path_1 = Path(tmp_dir, "code_1.txt")
         path_0.write_text("0")
         path_1.write_text("1")
-        good_outputs = {"std_out": path_1, "std_err": path_1, "exit_code": path_0}
-        bad_outputs = {"std_out": path_0, "std_err": path_0, "exit_code": path_1}
+        fail_outputs = {"std_out": path_1, "std_err": path_1, "exit_code": path_0}
+        pass_outputs = {"std_out": path_0, "std_err": path_0, "exit_code": path_1}
 
         test = tests.GrepDateTest(target)
-        mocker.patch.object(test, "_find_process_outputs", return_value=good_outputs)
+        mocker.patch.object(test, "_find_process_outputs", return_value=pass_outputs)
         test_status = test.get_status()
         assert test_status == TestStatus.PASS
 
-        test = tests.LibTiffInfoTest(target)
-        mocker.patch.object(test, "_find_process_outputs", return_value=bad_outputs)
+        test = tests.GrepDateTest(target)
+        mocker.patch.object(test, "_find_process_outputs", return_value=fail_outputs)
         test_status = test.get_status()
         assert test_status == TestStatus.FAIL
 
 
 def test_that_the_grep_date_test_command_is_produced(test_targets):
     target = test_targets["tiff"]
     test = tests.GrepDateTest(target)
@@ -217,31 +219,32 @@
     process = test.generate_process()
     assert "grep" in process.command
 
 
 def test_that_the_tifftag306datetimetest_correctly_interprets_exit_code_0_and_1(
     test_files, mocker
 ):
+    # 1 is pass, 0 is fail
     tiff_file = test_files["tiff"]
     target = SingleTarget(tiff_file)
     with TemporaryDirectory() as tmp_dir:
         path_0 = Path(tmp_dir, "code_0.txt")
         path_1 = Path(tmp_dir, "code_1.txt")
         path_0.write_text("0")
         path_1.write_text("1")
-        good_outputs = {"std_out": path_1, "std_err": path_1, "exit_code": path_0}
-        bad_outputs = {"std_out": path_0, "std_err": path_0, "exit_code": path_1}
+        fail_outputs = {"std_out": path_1, "std_err": path_1, "exit_code": path_0}
+        pass_outputs = {"std_out": path_0, "std_err": path_0, "exit_code": path_1}
 
         test = tests.TiffTag306DateTimeTest(target)
-        mocker.patch.object(test, "_find_process_outputs", return_value=good_outputs)
+        mocker.patch.object(test, "_find_process_outputs", return_value=pass_outputs)
         test_status = test.get_status()
         assert test_status == TestStatus.PASS
 
-        test = tests.LibTiffInfoTest(target)
-        mocker.patch.object(test, "_find_process_outputs", return_value=bad_outputs)
+        test = tests.TiffTag306DateTimeTest(target)
+        mocker.patch.object(test, "_find_process_outputs", return_value=fail_outputs)
         test_status = test.get_status()
         assert test_status == TestStatus.FAIL
 
 
 def test_that_paired_fastq_parity_test_correctly_passes_identical_fastq_files(
     test_files,
 ):
@@ -267,7 +270,22 @@
     test_files,
 ):
     fastq2 = test_files["fastq2"]
     target = PairedTarget([fastq2, fastq2])
     test = tests.PairedFastqParityTest(target)
     test_status = test.get_status()
     assert test_status == TestStatus.PASS
+
+
+def test_that_short_string_path_correctly_shortens_file_paths():
+    substring = "test-substring"
+    long_path = f"path/needs/to/be/shortened/{substring}/file.txt"
+    expected_short_path = f"'{substring}/file.txt'"
+    short_path = ExternalTestMixin._short_string_path(Path(long_path), substring)
+    assert short_path == expected_short_path
+
+
+def test_that_short_string_path_raises_valueerror_if_substring_not_in_path():
+    substring = "test-substring"
+    long_path = "path/needs/to/be/shortened/fail/file.txt"
+    with pytest.raises(ValueError):
+        ExternalTestMixin._short_string_path(Path(long_path), substring)
```

### Comparing `dcqc-1.5.0/tests/test_updaters.py` & `dcqc-1.6.0/tests/test_updaters.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.5.0/tox.ini` & `dcqc-1.6.0/tox.ini`

 * *Files identical despite different names*

