# Comparing `tmp/pycdfpp-0.4.2.tar.gz` & `tmp/pycdfpp-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycdfpp-0.4.2.tar", last modified: Fri Aug 19 22:27:59 2022, max compression
+gzip compressed data, was "pycdfpp-0.4.3.tar", last modified: Mon Jun 19 20:07:42 2023, max compression
```

## Comparing `pycdfpp-0.4.2.tar` & `pycdfpp-0.4.3.tar`

### file list

```diff
@@ -1,76 +1,77 @@
--rw-r--r--   0        0        0      212 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/.bumpversion.cfg
--rw-r--r--   0        0        0     1570 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/.cirrus.yml
--rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/.clang-format
--rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/.github/workflows/pythonpublish-linux.yml
--rw-r--r--   0        0        0     1302 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/.github/workflows/pythonpublish-osx.yml
--rw-r--r--   0        0        0     1288 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/.github/workflows/pythonpublish-win.yml
--rw-r--r--   0        0        0      772 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/.github/workflows/tests-linux.yml
--rw-r--r--   0        0        0      798 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/.github/workflows/tests-osx.yml
--rw-r--r--   0        0        0     1149 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/.github/workflows/tests-windows.yml
--rw-r--r--   0        0        0     1276 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/.github/workflows/tests-with-coverage.yml
--rw-r--r--   0        0        0      141 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/.gitignore
--rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/.gitpod.Dockerfile
--rw-r--r--   0        0        0      283 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/.gitpod.yml
--rw-r--r--   0        0        0      321 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/.theia/settings.json
--rw-r--r--   0        0        0     1585 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/COPYING
--rw-r--r--   0        0        0     5848 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/README.md
--rw-r--r--   0        0        0      184 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/environment.yml
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/examples/basic_cpp/main.cpp
--rw-r--r--   0        0        0   551791 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/examples/notebooks/Demo.ipynb
--rw-r--r--   0        0        0     3855 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/include/cdfpp/attribute.hpp
--rw-r--r--   0        0        0     8976 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/include/cdfpp/cdf-data.hpp
--rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/include/cdfpp/cdf-debug.hpp
--rw-r--r--   0        0        0     4974 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/include/cdfpp/cdf-endianness.hpp
--rw-r--r--   0        0        0     8224 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/include/cdfpp/cdf-enums.hpp
--rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/include/cdfpp/cdf-file.hpp
--rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/include/cdfpp/cdf-helpers.hpp
--rw-r--r--   0        0        0     3380 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/include/cdfpp/cdf-io/cdf-io-attribute.hpp
--rw-r--r--   0        0        0     9593 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/include/cdfpp/cdf-io/cdf-io-buffers.hpp
--rw-r--r--   0        0        0     7397 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/include/cdfpp/cdf-io/cdf-io-common.hpp
--rw-r--r--   0        0        0    29307 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/include/cdfpp/cdf-io/cdf-io-desc-records.hpp
--rw-r--r--   0        0        0     1957 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/include/cdfpp/cdf-io/cdf-io-rle.hpp
--rw-r--r--   0        0        0    12155 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/include/cdfpp/cdf-io/cdf-io-variable.hpp
--rw-r--r--   0        0        0     7435 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/include/cdfpp/cdf-io/cdf-io-zlib.hpp
--rw-r--r--   0        0        0     7427 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/include/cdfpp/cdf-io/cdf-io.hpp
--rw-r--r--   0        0        0     6848 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/include/cdfpp/cdf-majority-swap.hpp
--rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/include/cdfpp/cdf.hpp
--rw-r--r--   0        0        0     1453 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/include/cdfpp/chrono/cdf-chrono-constants.hpp
--rw-r--r--   0        0        0     4532 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/include/cdfpp/chrono/cdf-chrono.hpp
--rw-r--r--   0        0        0     5839 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/include/cdfpp/chrono/cdf-leap-seconds.h
--rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/include/cdfpp/variable.hpp
--rw-r--r--   0        0        0     7016 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/meson.build
--rw-r--r--   0        0        0      219 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/meson_options.txt
--rw-r--r--   0        0        0     8668 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/notebooks/Leap_seconds.ipynb
--rw-r--r--   0        0        0     2683 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/notebooks/chrono_test_table_gen.ipynb
--rw-r--r--   0        0        0      922 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1387 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/scripts/build_wheel.py
--rw-r--r--   0        0        0     1253 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/scripts/version.py
--rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/subprojects/catch2.wrap
--rw-r--r--   0        0        0      416 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/subprojects/hedley.wrap
--rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/subprojects/pybind11.wrap
--rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/subprojects/zlib.wrap
--rw-r--r--   0        0        0     2149 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/tests/chrono/main.cpp
--rw-r--r--   0        0        0   127282 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/tests/chrono/test_values.hpp
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/tests/endianness/main.cpp
--rw-r--r--   0        0        0     1416 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/tests/majority/main.cpp
--rw-r--r--   0        0        0     1000 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/tests/manual_load/main.cpp
--rw-r--r--   0        0        0     8945 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/tests/python_wrapper/test.py
--rw-r--r--   0        0        0     5721 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/tests/python_wrapper/test_corpus.py
--rw-r--r--   0        0        0      479 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/tests/python_wrapper_cpp/main.cpp
--rw-r--r--   0        0        0   113172 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/tests/resources/a_cdf.cdf
--rw-r--r--   0        0        0    41097 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/tests/resources/a_cdf_with_compressed_vars.cdf
--rw-r--r--   0        0        0   113172 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/tests/resources/a_col_major_cdf.cdf
--rw-r--r--   0        0        0     4936 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/tests/resources/a_compressed_cdf.cdf
--rw-r--r--   0        0        0     4936 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/tests/resources/a_rle_compressed_cdf.cdf
--rw-r--r--   0        0        0     4444 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/tests/resources/make_cdf.py
--rw-r--r--   0        0        0       21 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/tests/resources/not_a_cdf.cdf
--rw-r--r--   0        0        0   117066 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/tests/resources/testutf8.cdf
--rw-r--r--   0        0        0    55597 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/tests/resources/wi_l2-30min_sms-stics-afm-magnetosphere_00000000_v01.cdf
--rw-r--r--   0        0        0    18070 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/tests/simple_open/main.cpp
--rw-r--r--   0        0        0     2051 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/tests/zlib/main.cpp
--rw-r--r--   0        0        0        7 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/version.txt
--rw-r--r--   0        0        0     8879 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/wrapper/buffers.hpp
--rw-r--r--   0        0        0     7608 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/wrapper/chrono.hpp
--rw-r--r--   0        0        0    10475 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/wrapper/pycdfpp.cpp
--rw-r--r--   0        0        0     8585 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/wrapper/repr.hpp
--rw-r--r--   0        0        0     8291 1970-01-01 00:00:00.000000 pycdfpp-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0      210 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.bumpversion.cfg
+-rw-rw-rw-   0        0        0     2965 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.cirrus.yml
+-rw-rw-rw-   0        0        0      639 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.clang-format
+-rw-rw-rw-   0        0        0     1636 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.github/workflows/pythonpublish-linux.yml
+-rw-rw-rw-   0        0        0     1298 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.github/workflows/pythonpublish-osx.yml
+-rw-rw-rw-   0        0        0     1284 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.github/workflows/pythonpublish-win.yml
+-rw-rw-rw-   0        0        0      768 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.github/workflows/tests-linux.yml
+-rw-rw-rw-   0        0        0      794 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.github/workflows/tests-osx.yml
+-rw-rw-rw-   0        0        0     1145 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.github/workflows/tests-windows.yml
+-rw-rw-rw-   0        0        0     1276 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.github/workflows/tests-with-coverage.yml
+-rw-rw-rw-   0        0        0      141 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.gitignore
+-rw-rw-rw-   0        0        0      388 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.gitpod.Dockerfile
+-rw-rw-rw-   0        0        0      283 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.gitpod.yml
+-rw-rw-rw-   0        0        0      321 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.theia/settings.json
+-rw-rw-rw-   0        0        0     1585 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/COPYING
+-rw-rw-rw-   0        0        0     6690 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/README.md
+-rw-rw-rw-   0        0        0      184 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/environment.yml
+-rw-rw-rw-   0        0        0     1077 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/examples/basic_cpp/main.cpp
+-rw-rw-rw-   0        0        0   551791 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/examples/notebooks/Demo.ipynb
+-rw-rw-rw-   0        0        0     3855 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/attribute.hpp
+-rw-rw-rw-   0        0        0     8976 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-data.hpp
+-rw-rw-rw-   0        0        0     1839 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-debug.hpp
+-rw-rw-rw-   0        0        0     4980 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-endianness.hpp
+-rw-rw-rw-   0        0        0     8224 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-enums.hpp
+-rw-rw-rw-   0        0        0     2049 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-file.hpp
+-rw-rw-rw-   0        0        0     1600 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-helpers.hpp
+-rw-rw-rw-   0        0        0     3380 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-attribute.hpp
+-rw-rw-rw-   0        0        0     9593 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-buffers.hpp
+-rw-rw-rw-   0        0        0     7658 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-common.hpp
+-rw-rw-rw-   0        0        0    29307 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-desc-records.hpp
+-rw-rw-rw-   0        0        0     1957 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-rle.hpp
+-rw-rw-rw-   0        0        0    12155 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-variable.hpp
+-rw-rw-rw-   0        0        0     7435 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-zlib.hpp
+-rw-rw-rw-   0        0        0     7742 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io.hpp
+-rw-rw-rw-   0        0        0     6848 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-majority-swap.hpp
+-rw-rw-rw-   0        0        0     8734 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-repr.hpp
+-rw-rw-rw-   0        0        0     1351 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf.hpp
+-rw-rw-rw-   0        0        0     1453 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/chrono/cdf-chrono-constants.hpp
+-rw-rw-rw-   0        0        0     4532 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/chrono/cdf-chrono.hpp
+-rw-rw-rw-   0        0        0     5839 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/chrono/cdf-leap-seconds.h
+-rw-rw-rw-   0        0        0     3633 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/variable.hpp
+-rw-rw-rw-   0        0        0     7154 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/meson.build
+-rw-rw-rw-   0        0        0      219 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/meson_options.txt
+-rw-rw-rw-   0        0        0     8668 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/notebooks/Leap_seconds.ipynb
+-rw-rw-rw-   0        0        0     2683 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/notebooks/chrono_test_table_gen.ipynb
+-rw-rw-rw-   0        0        0      922 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1387 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/scripts/build_wheel.py
+-rw-rw-rw-   0        0        0     1253 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/scripts/version.py
+-rw-rw-rw-   0        0        0      443 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/subprojects/catch2.wrap
+-rw-rw-rw-   0        0        0      458 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/subprojects/fmt.wrap
+-rw-rw-rw-   0        0        0      463 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/subprojects/hedley.wrap
+-rw-rw-rw-   0        0        0      629 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/subprojects/pybind11.wrap
+-rw-rw-rw-   0        0        0      461 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/subprojects/zlib.wrap
+-rw-rw-rw-   0        0        0     2171 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/chrono/main.cpp
+-rw-rw-rw-   0        0        0   127282 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/chrono/test_values.hpp
+-rw-rw-rw-   0        0        0      561 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/endianness/main.cpp
+-rw-rw-rw-   0        0        0     1438 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/majority/main.cpp
+-rw-rw-rw-   0        0        0     1000 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/manual_load/main.cpp
+-rw-rw-rw-   0        0        0     9079 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/python_wrapper/test.py
+-rw-rw-rw-   0        0        0     5721 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/python_wrapper/test_corpus.py
+-rw-rw-rw-   0        0        0      479 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/python_wrapper_cpp/main.cpp
+-rw-rw-rw-   0        0        0   113172 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/resources/a_cdf.cdf
+-rw-rw-rw-   0        0        0    41097 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/resources/a_cdf_with_compressed_vars.cdf
+-rw-rw-rw-   0        0        0   113172 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/resources/a_col_major_cdf.cdf
+-rw-rw-rw-   0        0        0     4936 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/resources/a_compressed_cdf.cdf
+-rw-rw-rw-   0        0        0     4936 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/resources/a_rle_compressed_cdf.cdf
+-rw-rw-rw-   0        0        0     4444 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/resources/make_cdf.py
+-rw-rw-rw-   0        0        0       21 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/resources/not_a_cdf.cdf
+-rw-rw-rw-   0        0        0   117066 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/resources/testutf8.cdf
+-rw-rw-rw-   0        0        0    55597 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/resources/wi_l2-30min_sms-stics-afm-magnetosphere_00000000_v01.cdf
+-rw-rw-rw-   0        0        0    20148 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/simple_open/main.cpp
+-rw-rw-rw-   0        0        0     2073 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/zlib/main.cpp
+-rw-rw-rw-   0        0        0        7 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/version.txt
+-rw-rw-rw-   0        0        0     8879 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/wrapper/buffers.hpp
+-rw-rw-rw-   0        0        0     7608 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/wrapper/chrono.hpp
+-rw-rw-rw-   0        0        0    10735 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/wrapper/pycdfpp.cpp
+-rw-r--r--   0        0        0     9108 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/PKG-INFO
```

### Comparing `pycdfpp-0.4.2/.clang-format` & `pycdfpp-0.4.3/.clang-format`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/.github/workflows/pythonpublish-linux.yml` & `pycdfpp-0.4.3/.github/workflows/pythonpublish-linux.yml`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/.github/workflows/pythonpublish-osx.yml` & `pycdfpp-0.4.3/.github/workflows/pythonpublish-osx.yml`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 jobs:
   build:
     runs-on: macos-10.15
     strategy:
       max-parallel: 4
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11-dev']
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
     name: Python ${{ matrix.python-version }}
     steps:
       - uses: actions/checkout@v3
       - name: Build python wheel
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `pycdfpp-0.4.2/.github/workflows/pythonpublish-win.yml` & `pycdfpp-0.4.3/.github/workflows/pythonpublish-win.yml`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 jobs:
   build:
     runs-on: windows-2019
     strategy:
       max-parallel: 4
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11-dev']
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
     name: Python ${{ matrix.python-version }}
     steps:
       - uses: actions/checkout@v3
       - name: Build python wheel
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `pycdfpp-0.4.2/.github/workflows/tests-linux.yml` & `pycdfpp-0.4.3/.github/workflows/tests-linux.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   build:
     name: Linux test matrix
     runs-on: ubuntu-latest
     continue-on-error: false
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11-dev']
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
     steps:
       - uses: actions/checkout@v3
       - name: Build python wheel
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           architecture: x64
```

### Comparing `pycdfpp-0.4.2/.github/workflows/tests-osx.yml` & `pycdfpp-0.4.3/.github/workflows/tests-osx.yml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   build:
     name: MacOs test matrix
     runs-on: macos-latest
     continue-on-error: false
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11-dev']
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
     steps:
       - uses: actions/checkout@v3
       - name: Build python wheel
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           architecture: x64
```

### Comparing `pycdfpp-0.4.2/.github/workflows/tests-windows.yml` & `pycdfpp-0.4.3/.github/workflows/tests-windows.yml`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     name: Windows test matrix
     # Stick to 2019 which ships with mingw 8.1.0 (chocolatey), since latest version misses zlib :/
     runs-on: windows-2019
     continue-on-error: false
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11-dev']
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
     steps:
       - uses: actions/checkout@v3
       - name: Build python wheel
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           architecture: x64
```

### Comparing `pycdfpp-0.4.2/.github/workflows/tests-with-coverage.yml` & `pycdfpp-0.4.3/.github/workflows/tests-with-coverage.yml`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/COPYING` & `pycdfpp-0.4.3/COPYING`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/README.md` & `pycdfpp-0.4.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,42 @@
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![CPP17](https://img.shields.io/badge/Language-C++17-blue.svg)]()
 [![PyPi](https://img.shields.io/pypi/v/pycdfpp.svg)](https://pypi.python.org/pypi/pycdfpp)
-[![Windows(x86_64) test matrix](https://github.com/SciQLop/CDFpp/actions/workflows/tests-windows.yml/badge.svg?branch=main)](https://github.com/SciQLop/CDFpp/actions/workflows/tests-windows.yml)
-[![Linux test matrix](https://github.com/SciQLop/CDFpp/actions/workflows/tests-linux.yml/badge.svg?branch=main)](https://github.com/SciQLop/CDFpp/actions/workflows/tests-linux.yml)
-[![MacOs(x86_64) test matrix](https://github.com/SciQLop/CDFpp/actions/workflows/tests-osx.yml/badge.svg?branch=main)](https://github.com/SciQLop/CDFpp/actions/workflows/tests-osx.yml)
-[![MacOs(ARM64) test matrix](https://api.cirrus-ci.com/github/SciQLop/CDFpp.svg)](https://cirrus-ci.com/github/SciQLop/CDFpp)
 [![Coverage](https://codecov.io/gh/SciQLop/CDFpp/coverage.svg?branch=main)](https://codecov.io/gh/SciQLop/CDFpp/branch/main)
 [![Discover on MyBinder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/SciQLop/CDFpp/main?labpath=examples/notebooks)
 
+# Python packages
+
+| Linux x86_64 | Windows x86_64  | MacOs x86_64  | MacOs ARM64  |
+| --- | --- | --- | --- |
+| [![linux_x86_64][1]][2] | [![windows_x86_64][3]][4] | [![macos_x86_64][5]][6] | [![macos_arm64][7]][8] |
+
+[1]: https://github.com/SciQLop/CDFpp/actions/workflows/pythonpublish-linux.yml/badge.svg
+[2]: https://github.com/SciQLop/CDFpp/actions/workflows/pythonpublish-linux.yml
+[3]: https://github.com/SciQLop/CDFpp/actions/workflows/pythonpublish-win.yml/badge.svg
+[4]: https://github.com/SciQLop/CDFpp/actions/workflows/pythonpublish-win.yml
+[5]: https://github.com/SciQLop/CDFpp/actions/workflows/pythonpublish-osx.yml/badge.svg
+[6]: https://github.com/SciQLop/CDFpp/actions/workflows/pythonpublish-osx.yml
+[7]: https://api.cirrus-ci.com/github/SciQLop/CDFpp.svg
+[8]: https://cirrus-ci.com/github/SciQLop/CDFpp
+
+
+# Unit Tests
+
+| Linux x86_64  | Windows x86_64 | MacOs x86_64  |
+| --- | --- | --- |
+| [![linux_x86_64][9]][10] | [![windows_x86_64][11]][12] | [![macos_x86_64][13]][14] |
+
+[9]: https://github.com/SciQLop/CDFpp/actions/workflows/tests-linux.yml/badge.svg?branch=main
+[10]: https://github.com/SciQLop/CDFpp/actions/workflows/tests-linux.yml
+[11]: https://github.com/SciQLop/CDFpp/actions/workflows/tests-windows.yml/badge.svg?branch=main
+[12]: https://github.com/SciQLop/CDFpp/actions/workflows/tests-windows.yml
+[13]: https://github.com/SciQLop/CDFpp/actions/workflows/tests-osx.yml/badge.svg?branch=main
+[14]: https://github.com/SciQLop/CDFpp/actions/workflows/tests-osx.yml
+
 
 # CDFpp (CDF++)
 A NASA's [CDF](https://cdf.gsfc.nasa.gov/) modern C++ library. 
 This is not a C++ wrapper but a full C++ implementation.
 Why? CDF files are still used for space physics missions but few implementations are available.
 The main one is NASA's C implementation available [here](https://cdf.gsfc.nasa.gov/) but it lacks multi-threads support, has an old C interface and has a license which isn't compatible with most Linux distributions policy.
 There are also Java and Python implementations which are not usable in C++.
```

### Comparing `pycdfpp-0.4.2/examples/basic_cpp/main.cpp` & `pycdfpp-0.4.3/examples/basic_cpp/main.cpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/examples/notebooks/Demo.ipynb` & `pycdfpp-0.4.3/examples/notebooks/Demo.ipynb`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/include/cdfpp/attribute.hpp` & `pycdfpp-0.4.3/include/cdfpp/attribute.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/include/cdfpp/cdf-data.hpp` & `pycdfpp-0.4.3/include/cdfpp/cdf-data.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/include/cdfpp/cdf-debug.hpp` & `pycdfpp-0.4.3/include/cdfpp/cdf-debug.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/include/cdfpp/cdf-endianness.hpp` & `pycdfpp-0.4.3/include/cdfpp/cdf-endianness.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 -- You should have received a copy of the GNU General Public License
 -- along with this program; if not, write to the Free Software
 -- Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307 USA
 -------------------------------------------------------------------------------*/
 /*-- Author : Alexis Jeandet
 -- Mail : alexis.jeandet@member.fsf.org
 ----------------------------------------------------------------------------*/
-#include "config.h"
+#include "cdfpp_config.h"
 #ifdef CDFpp_BIG_ENDIAN
 inline const bool host_is_big_endian = true;
 inline const bool host_is_little_endian = false;
 #else
 #ifdef CDFpp_LITTLE_ENDIAN
 inline const bool host_is_big_endian = false;
 inline const bool host_is_little_endian = true;
```

### Comparing `pycdfpp-0.4.2/include/cdfpp/cdf-enums.hpp` & `pycdfpp-0.4.3/include/cdfpp/cdf-enums.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/include/cdfpp/cdf-file.hpp` & `pycdfpp-0.4.3/include/cdfpp/cdf-file.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -17,25 +17,27 @@
 -- along with this program; if not, write to the Free Software
 -- Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307 USA
 -------------------------------------------------------------------------------*/
 /*-- Author : Alexis Jeandet
 -- Mail : alexis.jeandet@member.fsf.org
 ----------------------------------------------------------------------------*/
 #include "attribute.hpp"
+#include "cdf-enums.hpp"
+#include "cdf-io/cdf-io-common.hpp"
 #include "variable.hpp"
 #include <string>
-#include "cdf-enums.hpp"
 #include <unordered_map>
 
 
 namespace cdf
 {
 struct CDF
 {
     cdf_majority majority;
+    std::tuple<uint32_t,uint32_t,uint32_t> distribution_version;
     std::unordered_map<std::string, Variable> variables;
     std::unordered_map<std::string, Attribute> attributes;
     const Variable& operator[](const std::string& name) const { return variables.at(name); }
     Variable& operator[](const std::string& name) { return variables.at(name); }
 };
 
 void add_attribute(CDF& cdf_file, const std::string& name, Attribute::attr_data_t&& data)
```

### Comparing `pycdfpp-0.4.2/include/cdfpp/cdf-helpers.hpp` & `pycdfpp-0.4.3/include/cdfpp/cdf-helpers.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/include/cdfpp/cdf-io/cdf-io-attribute.hpp` & `pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-attribute.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/include/cdfpp/cdf-io/cdf-io-buffers.hpp` & `pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-buffers.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/include/cdfpp/cdf-io/cdf-io-common.hpp` & `pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-common.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -20,31 +20,37 @@
 /*-- Author : Alexis Jeandet
 -- Mail : alexis.jeandet@member.fsf.org
 ----------------------------------------------------------------------------*/
 #include "../attribute.hpp"
 #include "../cdf-endianness.hpp"
 #include "../cdf-majority-swap.hpp"
 #include "../variable.hpp"
+#include <assert.h>
 #include <functional>
 #include <tuple>
 #include <type_traits>
 #include <unordered_map>
 #include <vector>
-#include <assert.h>
 
 namespace cdf::io::common
 {
 using magic_numbers_t = std::pair<uint32_t, uint32_t>;
+using version_t = std::pair<uint8_t, uint8_t>;
+
+inline version_t cdf_version(const magic_numbers_t& magic)
+{
+    return { (magic.first >> 16) & 0xf, (magic.first >> 12) & 0xf };
+}
 
-bool is_v3x(const magic_numbers_t& magic)
+inline bool is_v3x(const magic_numbers_t& magic)
 {
-    return ((magic.first >> 12) & 0xff) >= 0x30;
+    return cdf_version(magic).first >= 3;
 }
 
-bool is_cdf(const magic_numbers_t& magic_numbers) noexcept
+inline bool is_cdf(const magic_numbers_t& magic_numbers) noexcept
 {
     return (((magic_numbers.first & 0xfff00000) == 0xCDF00000)
                && (magic_numbers.second == 0xCCCC0001 || magic_numbers.second == 0x0000FFFF))
         || (magic_numbers.first == 0x0000FFFF && magic_numbers.second == 0x0000FFFF);
 }
 
 template <typename context_t>
@@ -166,14 +172,15 @@
     value_type* operator->() { return &block; }
     value_type& operator*() { return block; }
 };
 
 struct cdf_repr
 {
     cdf_majority majority;
+    std::tuple<uint32_t, uint32_t, uint32_t> distribution_version;
     std::unordered_map<std::string, Variable> variables;
     std::unordered_map<std::string, Attribute> attributes;
     std::unordered_map<std::size_t, std::unordered_map<std::string, Attribute>> var_attributes;
 };
 
 void add_global_attribute(cdf_repr& repr, const std::string& name, Attribute::attr_data_t&& data)
 {
```

### Comparing `pycdfpp-0.4.2/include/cdfpp/cdf-io/cdf-io-desc-records.hpp` & `pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-desc-records.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/include/cdfpp/cdf-io/cdf-io-rle.hpp` & `pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-rle.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/include/cdfpp/cdf-io/cdf-io-variable.hpp` & `pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-variable.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/include/cdfpp/cdf-io/cdf-io-zlib.hpp` & `pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-zlib.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/include/cdfpp/cdf-io/cdf-io.hpp` & `pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -56,47 +56,53 @@
     {
         inline static constexpr bool v3 = is_v3_v<version_t>;
         using version_tag = version_t;
         common::magic_numbers_t magic;
         cdf_CDR_t<version_t, buffer_t> cdr;
         cdf_GDR_t<version_t, buffer_t> gdr;
         cdf_majority majority;
+        std::tuple<uint32_t, uint32_t, uint32_t> distribution_version;
+
         buffer_t& buffer;
         bool is_compressed;
         bool ok = false;
         cdf_headers_t(buffer_t& buffer, std::size_t CDRoffset = 8)
                 : cdr { buffer }, gdr { buffer }, buffer { buffer }
         {
             magic = get_magic(buffer);
             if (common::is_cdf(magic) && cdr.load(CDRoffset) && gdr.load(cdr.GDRoffset.value))
             {
                 ok = true;
                 majority = common::majority(cdr);
+                distribution_version = { cdr.Version, cdr.Release, cdr.Increment };
             }
         }
         inline cdf_encoding encoding() { return cdr.Encoding.value; }
     };
 
     CDF from_repr(common::cdf_repr&& repr)
     {
         CDF cdf;
         cdf.majority = repr.majority;
+        cdf.distribution_version = repr.distribution_version;
         cdf.attributes = std::move(repr.attributes);
         cdf.variables = std::move(repr.variables);
         return cdf;
     }
 
     template <bool iso_8859_1_to_utf8, typename cdf_headers_t>
     std::optional<CDF> impl_parse_cdf(cdf_headers_t& cdf_headers)
     {
         common::cdf_repr repr;
         repr.majority = cdf_headers.majority;
+        repr.distribution_version = { cdf_headers.distribution_version };
         if (!cdf_headers.ok)
             return std::nullopt;
-        if (!attribute::load_all<typename cdf_headers_t::version_tag, iso_8859_1_to_utf8>(cdf_headers, repr))
+        if (!attribute::load_all<typename cdf_headers_t::version_tag, iso_8859_1_to_utf8>(
+                cdf_headers, repr))
             return std::nullopt;
         if (!variable::load_all<typename cdf_headers_t::version_tag>(cdf_headers, repr))
             return std::nullopt;
         return from_repr(std::move(repr));
     }
 
     template <typename cdf_version_tag_t, bool iso_8859_1_to_utf8, typename buffer_t>
```

### Comparing `pycdfpp-0.4.2/include/cdfpp/cdf-majority-swap.hpp` & `pycdfpp-0.4.3/include/cdfpp/cdf-majority-swap.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/include/cdfpp/cdf.hpp` & `pycdfpp-0.4.3/include/cdfpp/cdf.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -20,12 +20,13 @@
 /*-- Author : Alexis Jeandet
 -- Mail : alexis.jeandet@member.fsf.org
 ----------------------------------------------------------------------------*/
 #include "attribute.hpp"
 #include "cdf-file.hpp"
 #include "cdf-io/cdf-io.hpp"
 #include "variable.hpp"
+#include "cdf-repr.hpp"
 #include <optional>
 
 namespace cdf
 {
 } // namespace cdf
```

### Comparing `pycdfpp-0.4.2/include/cdfpp/chrono/cdf-chrono-constants.hpp` & `pycdfpp-0.4.3/include/cdfpp/chrono/cdf-chrono-constants.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/include/cdfpp/chrono/cdf-chrono.hpp` & `pycdfpp-0.4.3/include/cdfpp/chrono/cdf-chrono.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/include/cdfpp/chrono/cdf-leap-seconds.h` & `pycdfpp-0.4.3/include/cdfpp/chrono/cdf-leap-seconds.h`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/include/cdfpp/variable.hpp` & `pycdfpp-0.4.3/include/cdfpp/variable.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/meson.build` & `pycdfpp-0.4.3/meson.build`

 * *Files 6% similar despite different names*

```diff
@@ -19,27 +19,29 @@
 conf_data = configuration_data()
 conf_data.set_quoted('CDFPP_VERSION', meson.project_version())
 if(target_machine.endian() == 'big')
     conf_data.set('CDFpp_BIG_ENDIAN', true)
 else
     conf_data.set('CDFpp_LITTLE_ENDIAN', true)
 endif
-configure_file(output : 'config.h',
+configure_file(output : 'cdfpp_config.h',
                install : true,
                install_dir : 'include/cdfpp',
                configuration : conf_data)
 
 cpp = meson.get_compiler('cpp')
 if('clang'==cpp.get_id())
     add_global_arguments('-fsized-deallocation', language : 'cpp')
 endif
 
 
-pybind11_dep = dependency('pybind11', required : true, fallback:['pybind11','pybind11_dep'])
-hedley_dep = dependency('hedley', main : true, fallback : ['hedley', 'hedley_dep'])
+pybind11_dep = dependency('pybind11')
+hedley_dep = dependency('hedley')
+fmt_dep = dependency('fmt')
+
 
 if build_machine.system() == 'windows'
     link_args = ['-static-libstdc++','-static-libgcc','-static']
     zlib_dep = meson.get_compiler('cpp').find_library('z', static: true, required:false)
     if not zlib_dep.found()
         zlib_dep = dependency('zlib', main : true, static: true)
     endif
@@ -61,29 +63,29 @@
     'include/cdfpp/attribute.hpp',
     'include/cdfpp/variable.hpp',
     'include/cdfpp/cdf.hpp',
     'include/cdfpp/cdf-helpers.hpp',
     'include/cdfpp/chrono/cdf-chrono.hpp',
     'include/cdfpp/chrono/cdf-chrono-constants.hpp',
     'include/cdfpp/chrono/cdf-leap-seconds.h',
+    'include/cdfpp/cdf-repr.hpp',
     'include/cdfpp/cdf-data.hpp',
     'include/cdfpp/cdf-debug.hpp',
     'include/cdfpp/cdf-endianness.hpp',
     'include/cdfpp/cdf-majority-swap.hpp',
     'include/cdfpp/cdf-enums.hpp',
     'include/cdfpp/cdf-file.hpp',
     'include/cdfpp/cdf-io/cdf-io.hpp',
     'include/cdfpp/cdf-io/cdf-io-attribute.hpp',
     'include/cdfpp/cdf-io/cdf-io-buffers.hpp',
     'include/cdfpp/cdf-io/cdf-io-common.hpp',
     'include/cdfpp/cdf-io/cdf-io-desc-records.hpp',
     'include/cdfpp/cdf-io/cdf-io-variable.hpp',
     'include/cdfpp/cdf-io/cdf-io-zlib.hpp',
     'include/cdfpp/cdf-io/cdf-io-rle.hpp',
-    'wrapper/repr.hpp',
     'wrapper/chrono.hpp',
     'wrapper/buffers.hpp'
 ]
 
 cdfpp_extra_files = [
     'pyproject.toml',
     'README.md',
@@ -106,28 +108,35 @@
     cdfpp_lib = static_library('CDFpp',
             include_directories: include_directories('include'),
             dependencies: [zlib_dep, hedley_dep],
             extra_files: [cdfpp_headers, cdfpp_extra_files]
             )
 endif
 
-cdfpp_dep = declare_dependency(include_directories: include_directories('include'),
+if meson.is_subproject()
+    cdfpp_dep_inc = include_directories(['include', meson.current_build_dir()])
+else
+    cdfpp_dep_inc = include_directories('include')
+endif
+
+cdfpp_dep = declare_dependency(include_directories: cdfpp_dep_inc,
                                 dependencies: [zlib_dep, hedley_dep])
 
 
 
 python3.extension_module('pycdfpp', 'wrapper/pycdfpp.cpp',
-                         dependencies: [cdfpp_dep, pybind11_dep,python3.dependency()],
+                         dependencies: [cdfpp_dep, fmt_dep, pybind11_dep,python3.dependency()],
                          link_args: link_args,
                          install: true
                         )
 install_headers(
 [
     'include/cdfpp/attribute.hpp',
     'include/cdfpp/variable.hpp',
+    'include/cdfpp/cdf-repr.hpp',
     'include/cdfpp/cdf.hpp',
     'include/cdfpp/cdf-helpers.hpp',
     'include/cdfpp/cdf-data.hpp',
     'include/cdfpp/cdf-debug.hpp',
     'include/cdfpp/cdf-endianness.hpp',
     'include/cdfpp/cdf-majority-swap.hpp',
     'include/cdfpp/cdf-enums.hpp',
@@ -158,15 +167,15 @@
 
     configure_file(output : 'tests_config.hpp',
       configuration : {
         'DATA_PATH' : '"' + meson.current_source_dir() / 'tests/resources' + '"'
       }
     )
 
-    catch_dep = dependency('catch2', main : true, fallback : ['catch2', 'catch2_dep'])
+    catch_dep = dependency('catch2-with-main', version:'>3.0.0', required : true)
 
 
     foreach test:['endianness','simple_open', 'zlib', 'majority', 'chrono']
         exe = executable('test-'+test,'tests/'+test+'/main.cpp',
                         dependencies:[catch_dep, cdfpp_dep],
                         install: false
                         )
```

### Comparing `pycdfpp-0.4.2/notebooks/Leap_seconds.ipynb` & `pycdfpp-0.4.3/notebooks/Leap_seconds.ipynb`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/notebooks/chrono_test_table_gen.ipynb` & `pycdfpp-0.4.3/notebooks/chrono_test_table_gen.ipynb`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/pyproject.toml` & `pycdfpp-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/scripts/build_wheel.py` & `pycdfpp-0.4.3/scripts/build_wheel.py`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/scripts/version.py` & `pycdfpp-0.4.3/scripts/version.py`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/tests/chrono/main.cpp` & `pycdfpp-0.4.3/tests/chrono/main.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #include <chrono>
 #include <ctime>
 
-#define CATCH_CONFIG_MAIN
-#if __has_include(<catch2/catch.hpp>)
-#include <catch2/catch.hpp>
+#if __has_include(<catch2/catch_all.hpp>)
+#include <catch2/catch_all.hpp>
+#include <catch2/catch_test_macros.hpp>
 #else
 #include <catch.hpp>
 #endif
 
 #include "cdfpp/chrono/cdf-chrono.hpp"
 #include "test_values.hpp"
```

### Comparing `pycdfpp-0.4.2/tests/chrono/test_values.hpp` & `pycdfpp-0.4.3/tests/chrono/test_values.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/tests/endianness/main.cpp` & `pycdfpp-0.4.3/tests/endianness/main.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-#define CATCH_CONFIG_MAIN
-#if __has_include(<catch2/catch.hpp>)
-#include <catch2/catch.hpp>
+#if __has_include(<catch2/catch_all.hpp>)
+#include <catch2/catch_all.hpp>
+#include <catch2/catch_test_macros.hpp>
 #else
 #include <catch.hpp>
 #endif
 #include "cdfpp/cdf-endianness.hpp"
 #include <cstdint>
```

### Comparing `pycdfpp-0.4.2/tests/majority/main.cpp` & `pycdfpp-0.4.3/tests/majority/main.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-#define CATCH_CONFIG_MAIN
-#if __has_include(<catch2/catch.hpp>)
-#include <catch2/catch.hpp>
+#if __has_include(<catch2/catch_all.hpp>)
+#include <catch2/catch_all.hpp>
+#include <catch2/catch_test_macros.hpp>
 #else
 #include <catch.hpp>
 #endif
 #include "cdfpp/cdf-majority-swap.hpp"
 #include "vector"
```

### Comparing `pycdfpp-0.4.2/tests/manual_load/main.cpp` & `pycdfpp-0.4.3/tests/manual_load/main.cpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/tests/python_wrapper/test.py` & `pycdfpp-0.4.3/tests/python_wrapper/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,18 @@
         self.cdfs = list(map(pycdfpp.load, files)) + list(map(lambda f: pycdfpp.load(load_bytes(f)), files))
         for cdf in self.cdfs:
             self.assertIsNotNone(cdf)
 
     def tearDown(self):
         pass
 
+    def test_cdflib_version(self):
+        for cdf in self.cdfs:
+            self.assertEqual(cdf.distribution_version, (3,8,0))
+
     def test_has_all_expected_vars(self):
         for cdf in self.cdfs:
             for name in variables:
                 self.assertTrue(name in cdf)
 
     def test_has_all_expected_attributes(self):
         for cdf in self.cdfs:
```

### Comparing `pycdfpp-0.4.2/tests/python_wrapper/test_corpus.py` & `pycdfpp-0.4.3/tests/python_wrapper/test_corpus.py`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/tests/resources/a_cdf.cdf` & `pycdfpp-0.4.3/tests/resources/a_cdf.cdf`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/tests/resources/a_cdf_with_compressed_vars.cdf` & `pycdfpp-0.4.3/tests/resources/a_cdf_with_compressed_vars.cdf`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/tests/resources/a_col_major_cdf.cdf` & `pycdfpp-0.4.3/tests/resources/a_col_major_cdf.cdf`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/tests/resources/a_compressed_cdf.cdf` & `pycdfpp-0.4.3/tests/resources/a_compressed_cdf.cdf`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/tests/resources/a_rle_compressed_cdf.cdf` & `pycdfpp-0.4.3/tests/resources/a_rle_compressed_cdf.cdf`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/tests/resources/make_cdf.py` & `pycdfpp-0.4.3/tests/resources/make_cdf.py`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/tests/resources/testutf8.cdf` & `pycdfpp-0.4.3/tests/resources/testutf8.cdf`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/tests/resources/wi_l2-30min_sms-stics-afm-magnetosphere_00000000_v01.cdf` & `pycdfpp-0.4.3/tests/resources/wi_l2-30min_sms-stics-afm-magnetosphere_00000000_v01.cdf`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/tests/simple_open/main.cpp` & `pycdfpp-0.4.3/tests/simple_open/main.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #include <algorithm>
 #include <cstdint>
 #include <optional>
 #include <string>
 #include <unordered_map>
 #include <vector>
+#include <tuple>
 
 
-#define CATCH_CONFIG_MAIN
-#if __has_include(<catch2/catch.hpp>)
-#include <catch2/catch.hpp>
+#if __has_include(<catch2/catch_all.hpp>)
+#include <catch2/catch_all.hpp>
+#include <catch2/catch_test_macros.hpp>
 #else
 #include <catch.hpp>
 #endif
 
 #include <chrono>
 
 
@@ -190,14 +191,18 @@
     auto pos = file.tellg();
     file.seekg(0, file.end);
     pos = file.tellg() - pos;
     file.seekg(0, file.beg);
     return static_cast<std::size_t>(pos);
 }
 
+#define CHECK_CDF_FILE(cd, expected_version, expected_majority)                                        \
+    REQUIRE(cd.distribution_version == expected_version);                                                       \
+    REQUIRE(cd.majority == expected_majority);
+
 
 #define CHECK_ATTRIBUTES(cd)                                                                       \
     REQUIRE(std::size(cd.attributes) == 8);                                                        \
     REQUIRE(has_attribute(cd, "attr"));                                                            \
     REQUIRE(compare_attribute_values(cd.attributes["attr"], "a cdf text attribute"));              \
     REQUIRE(has_attribute(cd, "attr_float"));                                                      \
     REQUIRE(compare_attribute_values(cd.attributes["attr_float"], std::vector { 1.f, 2.f, 3.f },   \
@@ -283,14 +288,19 @@
         WHEN("file exists and is a cdf file")
         {
             auto path = std::string(DATA_PATH) + "/a_cdf.cdf";
             REQUIRE(file_exists(path));
             auto cd_opt = cdf::io::load(path);
             REQUIRE(cd_opt != std::nullopt);
             auto cd = *cd_opt;
+            THEN("Version and majority are retrieved")
+            {
+                static constexpr auto version = std::tuple<uint32_t,uint32_t,uint32_t>{3,8,0};
+                CHECK_CDF_FILE(cd, version, cdf::cdf_majority::row);
+            }
             THEN("All expected attributes are loaded")
             {
                 CHECK_ATTRIBUTES(cd);
             }
             THEN("All expected variables are loaded")
             {
                 CHECK_VARIABLES(cd);
@@ -310,14 +320,19 @@
                     return data;
                 }
                 return {};
             }();
             auto cd_opt = cdf::io::load(data);
             REQUIRE(cd_opt != std::nullopt);
             auto cd = *cd_opt;
+            THEN("Version and majority are retrieved")
+            {
+                static constexpr auto version = std::tuple<uint32_t,uint32_t,uint32_t>{3,8,0};
+                CHECK_CDF_FILE(cd, version, cdf::cdf_majority::row);
+            }
             THEN("All expected attributes are loaded")
             {
                 CHECK_ATTRIBUTES(cd);
             }
             THEN("All expected variables are loaded")
             {
                 CHECK_VARIABLES(cd);
@@ -339,14 +354,19 @@
                 }
                 return std::make_tuple(static_cast<char*>(nullptr), std::size_t { 0UL });
             }();
             auto cd_opt = cdf::io::load(data, size);
             delete[] data;
             REQUIRE(cd_opt != std::nullopt);
             auto cd = *cd_opt;
+            THEN("Version and majority are retrieved")
+            {
+                static constexpr auto version = std::tuple<uint32_t,uint32_t,uint32_t>{3,8,0};
+                CHECK_CDF_FILE(cd, version, cdf::cdf_majority::row);
+            }
             THEN("All expected attributes are loaded")
             {
                 CHECK_ATTRIBUTES(cd);
             }
             THEN("All expected variables are loaded")
             {
                 CHECK_VARIABLES(cd);
@@ -355,14 +375,19 @@
         WHEN("file exists and is a compressed cdf file (GZIP)")
         {
             auto path = std::string(DATA_PATH) + "/a_compressed_cdf.cdf";
             REQUIRE(file_exists(path));
             auto cd_opt = cdf::io::load(path);
             REQUIRE(cd_opt != std::nullopt);
             auto cd = *cd_opt;
+            THEN("Version and majority are retrieved")
+            {
+                static constexpr auto version = std::tuple<uint32_t,uint32_t,uint32_t>{3,8,0};
+                CHECK_CDF_FILE(cd, version, cdf::cdf_majority::row);
+            }
             THEN("All expected attributes are loaded")
             {
                 CHECK_ATTRIBUTES(cd);
             }
             THEN("All expected variables are loaded")
             {
                 CHECK_VARIABLES(cd);
@@ -371,14 +396,19 @@
         WHEN("file exists and is a compressed cdf file (RLE)")
         {
             auto path = std::string(DATA_PATH) + "/a_rle_compressed_cdf.cdf";
             REQUIRE(file_exists(path));
             auto cd_opt = cdf::io::load(path);
             REQUIRE(cd_opt != std::nullopt);
             auto cd = *cd_opt;
+            THEN("Version and majority are retrieved")
+            {
+                static constexpr auto version = std::tuple<uint32_t,uint32_t,uint32_t>{3,8,0};
+                CHECK_CDF_FILE(cd, version, cdf::cdf_majority::row);
+            }
             THEN("All expected attributes are loaded")
             {
                 CHECK_ATTRIBUTES(cd);
             }
             THEN("All expected variables are loaded")
             {
                 CHECK_VARIABLES(cd);
@@ -387,14 +417,19 @@
         WHEN("file exists and is a cdf file with compressed variables")
         {
             auto path = std::string(DATA_PATH) + "/a_cdf_with_compressed_vars.cdf";
             REQUIRE(file_exists(path));
             auto cd_opt = cdf::io::load(path);
             REQUIRE(cd_opt != std::nullopt);
             auto cd = *cd_opt;
+            THEN("Version and majority are retrieved")
+            {
+                static constexpr auto version = std::tuple<uint32_t,uint32_t,uint32_t>{3,8,0};
+                CHECK_CDF_FILE(cd, version, cdf::cdf_majority::row);
+            }
             THEN("All expected attributes are loaded")
             {
                 CHECK_ATTRIBUTES(cd);
             }
             THEN("All expected variables are loaded")
             {
                 CHECK_VARIABLES(cd);
@@ -403,14 +438,19 @@
         WHEN("file exists and is a column major cdf file")
         {
             auto path = std::string(DATA_PATH) + "/a_col_major_cdf.cdf";
             REQUIRE(file_exists(path));
             auto cd_opt = cdf::io::load(path);
             REQUIRE(cd_opt != std::nullopt);
             auto cd = *cd_opt;
+            THEN("Version and majority are retrieved")
+            {
+                static constexpr auto version = std::tuple<uint32_t,uint32_t,uint32_t>{3,8,0};
+                CHECK_CDF_FILE(cd, version, cdf::cdf_majority::column);
+            }
             THEN("All expected attributes are loaded")
             {
                 CHECK_ATTRIBUTES(cd);
             }
             THEN("All expected variables are loaded")
             {
                 CHECK_VARIABLES(cd);
```

### Comparing `pycdfpp-0.4.2/tests/zlib/main.cpp` & `pycdfpp-0.4.3/tests/zlib/main.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-#define CATCH_CONFIG_MAIN
-#if __has_include(<catch2/catch.hpp>)
-#include <catch2/catch.hpp>
+#if __has_include(<catch2/catch_all.hpp>)
+#include <catch2/catch_all.hpp>
+#include <catch2/catch_test_macros.hpp>
 #else
 #include <catch.hpp>
 #endif
 #include "cdfpp/cdf-io/cdf-io-zlib.hpp"
 #include <algorithm>
 #include <cstdint>
 #include <random>
```

### Comparing `pycdfpp-0.4.2/wrapper/buffers.hpp` & `pycdfpp-0.4.3/wrapper/buffers.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/wrapper/chrono.hpp` & `pycdfpp-0.4.3/wrapper/chrono.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.2/wrapper/pycdfpp.cpp` & `pycdfpp-0.4.3/wrapper/pycdfpp.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 -- Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307 USA
 -------------------------------------------------------------------------------*/
 /*-- Author : Alexis Jeandet
 -- Mail : alexis.jeandet@member.fsf.org
 ----------------------------------------------------------------------------*/
 #include "buffers.hpp"
 #include "chrono.hpp"
-#include "repr.hpp"
 #include <cdfpp/cdf-data.hpp>
+#include <cdfpp/cdf-repr.hpp>
 #include <cdfpp/cdf.hpp>
 #include <cdfpp/chrono/cdf-chrono.hpp>
-#include <config.h>
+#include <cdfpp_config.h>
 using namespace cdf;
 
 #include <pybind11/chrono.h>
 #include <pybind11/iostream.h>
 #include <pybind11/numpy.h>
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
@@ -185,20 +185,23 @@
         .value("CDF_UINT4", CDF_Types::CDF_UINT4)
         .value("CDF_DOUBLE", CDF_Types::CDF_DOUBLE)
         .value("CDF_EPOCH16", CDF_Types::CDF_EPOCH16)
         .value("CDF_TIME_TT2000", CDF_Types::CDF_TIME_TT2000)
         .export_values();
 
     py::class_<CDF>(m, "CDF")
-        .def_readonly("attributes", &CDF::attributes, py::return_value_policy::reference)
+        .def_readonly("attributes", &CDF::attributes, py::return_value_policy::reference,
+            py::keep_alive<0, 1>())
         .def_property_readonly("majority", [](const CDF& cdf) { return cdf.majority; })
+        .def_property_readonly(
+            "distribution_version", [](const CDF& cdf) { return cdf.distribution_version; })
         .def("__repr__", __repr__<CDF>)
         .def(
             "__getitem__", [](CDF& cd, const std::string& key) -> Variable& { return cd[key]; },
-            py::return_value_policy::reference)
+            py::return_value_policy::reference_internal)
         .def("__contains__",
             [](const CDF& cd, std::string& key) { return cd.variables.count(key) > 0; })
         .def(
             "__iter__",
             [](const CDF& cd)
             { return py::make_key_iterator(std::begin(cd.variables), std::end(cd.variables)); },
             py::keep_alive<0, 1>())
@@ -208,34 +211,36 @@
             { return py::make_iterator(std::begin(cd.variables), std::end(cd.variables)); },
             py::keep_alive<0, 1>())
         .def("__len__", [](const CDF& cd) { return std::size(cd.variables); });
 
     py::class_<Attribute>(m, "Attribute")
         .def_property_readonly("name", [](Attribute& attr) { return attr.name; })
         .def("__repr__", __repr__<Attribute>)
-        .def("__getitem__",
+        .def(
+            "__getitem__",
             [](Attribute& att, std::size_t index) -> py_cdf_attr_data_t
             {
                 if (index >= att.size())
                     throw std::out_of_range(
                         "Trying to get an attribute value outside of its range");
                 return to_py_cdf_data(att[index]);
-            })
+            },
+            py::return_value_policy::reference_internal)
         .def("__len__", [](const Attribute& att) { return att.size(); });
 
     py::class_<Variable>(m, "Variable", py::buffer_protocol())
         .def("__repr__", __repr__<Variable>)
         .def_readonly("attributes", &Variable::attributes, py::return_value_policy::reference)
         .def_property_readonly("name", &Variable::name)
         .def_property_readonly("type", &Variable::type)
         .def_property_readonly("shape", &Variable::shape)
         .def_property_readonly("majority", &Variable::majority)
         .def_buffer([](Variable& var) -> py::buffer_info { return make_buffer(var); })
-        .def_property_readonly(
-            "values", make_values_view, py::return_value_policy::reference_internal);
+        .def_property_readonly("values", make_values_view,
+            py::return_value_policy::reference_internal);
 
     m.def(
         "load",
         [](py::bytes& buffer, bool iso_8859_1_to_utf8)
         {
             py::buffer_info info(py::buffer(buffer).request());
             return io::load(static_cast<char*>(info.ptr), static_cast<std::size_t>(info.size),
```

### Comparing `pycdfpp-0.4.2/wrapper/repr.hpp` & `pycdfpp-0.4.3/include/cdfpp/cdf-repr.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -20,32 +20,30 @@
 /*-- Author : Alexis Jeandet
 -- Mail : alexis.jeandet@member.fsf.org
 ----------------------------------------------------------------------------*/
 #include <cdfpp/cdf-data.hpp>
 #include <cdfpp/cdf.hpp>
 #include <cdfpp/chrono/cdf-chrono.hpp>
 #include <chrono>
+#include <fmt/core.h>
 #include <iomanip>
 #include <sstream>
 #include <string>
 using namespace cdf;
 
-#include <pybind11/numpy.h>
-#include <pybind11/pybind11.h>
-#include <pybind11/stl.h>
-
-namespace py = pybind11;
-
 inline std::ostream& operator<<(std::ostream& os, const cdf::data_t& data);
 
 template <typename collection_t>
 constexpr bool is_char_like_v
     = std::is_same_v<int8_t,
-          std::remove_cv_t<std::remove_reference_t<decltype(*std::cbegin(std::declval<
-              collection_t>()))>>> or std::is_same_v<uint8_t, std::remove_cv_t<std::remove_reference_t<decltype(*std::cbegin(std::declval<collection_t>()))>>>;
+          std::remove_cv_t<
+              std::remove_reference_t<decltype(*std::cbegin(std::declval<collection_t>()))>>>
+    or std::is_same_v<uint8_t,
+        std::remove_cv_t<
+            std::remove_reference_t<decltype(*std::cbegin(std::declval<collection_t>()))>>>;
 
 template <int widtw>
 std::ostream& fixed_width(std::ostream& os)
 {
     return os << std::setprecision(widtw) << std::setw(widtw) << std::setfill('0');
 };
 
@@ -225,15 +223,19 @@
     else
         os << "majority: row";
     return os;
 }
 
 inline std::ostream& operator<<(std::ostream& os, const cdf::CDF& cdf_file)
 {
-    os << "CDF:\n" << cdf_file.majority << "\n\nAttributes:\n";
+    os << "CDF:\n"
+       << fmt::format("version: {}.{}.{}\n", std::get<0>(cdf_file.distribution_version),
+              std::get<1>(cdf_file.distribution_version),
+              std::get<2>(cdf_file.distribution_version))
+       << cdf_file.majority << "\n\nAttributes:\n";
     std::for_each(std::cbegin(cdf_file.attributes), std::cend(cdf_file.attributes),
         [&os](const auto& item) { os << "\t" << item.second; });
     os << "\nVariables:\n";
     std::for_each(std::cbegin(cdf_file.variables), std::cend(cdf_file.variables),
         [&os](const auto& item) { os << "\t" << item.second; });
     os << std::endl;
```

### Comparing `pycdfpp-0.4.2/PKG-INFO` & `pycdfpp-0.4.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycdfpp
-Version: 0.4.2
+Version: 0.4.3
 Summary: A modern C++ header only cdf library
 Home-page: https://github.com/SciQLop/CDFpp
 Author-Email: Alexis Jeandet <alexis.jeandet@member.fsf.org>
 License: GNU GENERAL PUBLIC LICENSE
                               Version 3, 29 June 2007
         
             An easy to use ISTP loader package.
@@ -49,21 +49,46 @@
 Requires-Python: >=3.7
 Requires-Dist: numpy
 Description-Content-Type: text/markdown
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![CPP17](https://img.shields.io/badge/Language-C++17-blue.svg)]()
 [![PyPi](https://img.shields.io/pypi/v/pycdfpp.svg)](https://pypi.python.org/pypi/pycdfpp)
-[![Windows(x86_64) test matrix](https://github.com/SciQLop/CDFpp/actions/workflows/tests-windows.yml/badge.svg?branch=main)](https://github.com/SciQLop/CDFpp/actions/workflows/tests-windows.yml)
-[![Linux test matrix](https://github.com/SciQLop/CDFpp/actions/workflows/tests-linux.yml/badge.svg?branch=main)](https://github.com/SciQLop/CDFpp/actions/workflows/tests-linux.yml)
-[![MacOs(x86_64) test matrix](https://github.com/SciQLop/CDFpp/actions/workflows/tests-osx.yml/badge.svg?branch=main)](https://github.com/SciQLop/CDFpp/actions/workflows/tests-osx.yml)
-[![MacOs(ARM64) test matrix](https://api.cirrus-ci.com/github/SciQLop/CDFpp.svg)](https://cirrus-ci.com/github/SciQLop/CDFpp)
 [![Coverage](https://codecov.io/gh/SciQLop/CDFpp/coverage.svg?branch=main)](https://codecov.io/gh/SciQLop/CDFpp/branch/main)
 [![Discover on MyBinder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/SciQLop/CDFpp/main?labpath=examples/notebooks)
 
+# Python packages
+
+| Linux x86_64 | Windows x86_64  | MacOs x86_64  | MacOs ARM64  |
+| --- | --- | --- | --- |
+| [![linux_x86_64][1]][2] | [![windows_x86_64][3]][4] | [![macos_x86_64][5]][6] | [![macos_arm64][7]][8] |
+
+[1]: https://github.com/SciQLop/CDFpp/actions/workflows/pythonpublish-linux.yml/badge.svg
+[2]: https://github.com/SciQLop/CDFpp/actions/workflows/pythonpublish-linux.yml
+[3]: https://github.com/SciQLop/CDFpp/actions/workflows/pythonpublish-win.yml/badge.svg
+[4]: https://github.com/SciQLop/CDFpp/actions/workflows/pythonpublish-win.yml
+[5]: https://github.com/SciQLop/CDFpp/actions/workflows/pythonpublish-osx.yml/badge.svg
+[6]: https://github.com/SciQLop/CDFpp/actions/workflows/pythonpublish-osx.yml
+[7]: https://api.cirrus-ci.com/github/SciQLop/CDFpp.svg
+[8]: https://cirrus-ci.com/github/SciQLop/CDFpp
+
+
+# Unit Tests
+
+| Linux x86_64  | Windows x86_64 | MacOs x86_64  |
+| --- | --- | --- |
+| [![linux_x86_64][9]][10] | [![windows_x86_64][11]][12] | [![macos_x86_64][13]][14] |
+
+[9]: https://github.com/SciQLop/CDFpp/actions/workflows/tests-linux.yml/badge.svg?branch=main
+[10]: https://github.com/SciQLop/CDFpp/actions/workflows/tests-linux.yml
+[11]: https://github.com/SciQLop/CDFpp/actions/workflows/tests-windows.yml/badge.svg?branch=main
+[12]: https://github.com/SciQLop/CDFpp/actions/workflows/tests-windows.yml
+[13]: https://github.com/SciQLop/CDFpp/actions/workflows/tests-osx.yml/badge.svg?branch=main
+[14]: https://github.com/SciQLop/CDFpp/actions/workflows/tests-osx.yml
+
 
 # CDFpp (CDF++)
 A NASA's [CDF](https://cdf.gsfc.nasa.gov/) modern C++ library. 
 This is not a C++ wrapper but a full C++ implementation.
 Why? CDF files are still used for space physics missions but few implementations are available.
 The main one is NASA's C implementation available [here](https://cdf.gsfc.nasa.gov/) but it lacks multi-threads support, has an old C interface and has a license which isn't compatible with most Linux distributions policy.
 There are also Java and Python implementations which are not usable in C++.
```

