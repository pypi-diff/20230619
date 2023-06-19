# Comparing `tmp/pycdfpp-0.4.3.tar.gz` & `tmp/pycdfpp-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycdfpp-0.4.3.tar", last modified: Mon Jun 19 20:07:42 2023, max compression
+gzip compressed data, was "pycdfpp-0.4.4.tar", last modified: Mon Jun 19 21:50:39 2023, max compression
```

## Comparing `pycdfpp-0.4.3.tar` & `pycdfpp-0.4.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-rw-rw-   0        0        0      210 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.bumpversion.cfg
--rw-rw-rw-   0        0        0     2965 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.cirrus.yml
--rw-rw-rw-   0        0        0      639 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.clang-format
--rw-rw-rw-   0        0        0     1636 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.github/workflows/pythonpublish-linux.yml
--rw-rw-rw-   0        0        0     1298 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.github/workflows/pythonpublish-osx.yml
--rw-rw-rw-   0        0        0     1284 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.github/workflows/pythonpublish-win.yml
--rw-rw-rw-   0        0        0      768 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.github/workflows/tests-linux.yml
--rw-rw-rw-   0        0        0      794 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.github/workflows/tests-osx.yml
--rw-rw-rw-   0        0        0     1145 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.github/workflows/tests-windows.yml
--rw-rw-rw-   0        0        0     1276 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.github/workflows/tests-with-coverage.yml
--rw-rw-rw-   0        0        0      141 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.gitignore
--rw-rw-rw-   0        0        0      388 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.gitpod.Dockerfile
--rw-rw-rw-   0        0        0      283 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.gitpod.yml
--rw-rw-rw-   0        0        0      321 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/.theia/settings.json
--rw-rw-rw-   0        0        0     1585 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/COPYING
--rw-rw-rw-   0        0        0     6690 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/README.md
--rw-rw-rw-   0        0        0      184 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/environment.yml
--rw-rw-rw-   0        0        0     1077 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/examples/basic_cpp/main.cpp
--rw-rw-rw-   0        0        0   551791 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/examples/notebooks/Demo.ipynb
--rw-rw-rw-   0        0        0     3855 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/attribute.hpp
--rw-rw-rw-   0        0        0     8976 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-data.hpp
--rw-rw-rw-   0        0        0     1839 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-debug.hpp
--rw-rw-rw-   0        0        0     4980 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-endianness.hpp
--rw-rw-rw-   0        0        0     8224 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-enums.hpp
--rw-rw-rw-   0        0        0     2049 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-file.hpp
--rw-rw-rw-   0        0        0     1600 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-helpers.hpp
--rw-rw-rw-   0        0        0     3380 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-attribute.hpp
--rw-rw-rw-   0        0        0     9593 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-buffers.hpp
--rw-rw-rw-   0        0        0     7658 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-common.hpp
--rw-rw-rw-   0        0        0    29307 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-desc-records.hpp
--rw-rw-rw-   0        0        0     1957 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-rle.hpp
--rw-rw-rw-   0        0        0    12155 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-variable.hpp
--rw-rw-rw-   0        0        0     7435 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-zlib.hpp
--rw-rw-rw-   0        0        0     7742 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io.hpp
--rw-rw-rw-   0        0        0     6848 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-majority-swap.hpp
--rw-rw-rw-   0        0        0     8734 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf-repr.hpp
--rw-rw-rw-   0        0        0     1351 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/cdf.hpp
--rw-rw-rw-   0        0        0     1453 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/chrono/cdf-chrono-constants.hpp
--rw-rw-rw-   0        0        0     4532 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/chrono/cdf-chrono.hpp
--rw-rw-rw-   0        0        0     5839 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/chrono/cdf-leap-seconds.h
--rw-rw-rw-   0        0        0     3633 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/include/cdfpp/variable.hpp
--rw-rw-rw-   0        0        0     7154 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/meson.build
--rw-rw-rw-   0        0        0      219 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/meson_options.txt
--rw-rw-rw-   0        0        0     8668 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/notebooks/Leap_seconds.ipynb
--rw-rw-rw-   0        0        0     2683 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/notebooks/chrono_test_table_gen.ipynb
--rw-rw-rw-   0        0        0      922 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/pyproject.toml
--rw-rw-rw-   0        0        0     1387 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/scripts/build_wheel.py
--rw-rw-rw-   0        0        0     1253 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/scripts/version.py
--rw-rw-rw-   0        0        0      443 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/subprojects/catch2.wrap
--rw-rw-rw-   0        0        0      458 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/subprojects/fmt.wrap
--rw-rw-rw-   0        0        0      463 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/subprojects/hedley.wrap
--rw-rw-rw-   0        0        0      629 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/subprojects/pybind11.wrap
--rw-rw-rw-   0        0        0      461 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/subprojects/zlib.wrap
--rw-rw-rw-   0        0        0     2171 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/chrono/main.cpp
--rw-rw-rw-   0        0        0   127282 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/chrono/test_values.hpp
--rw-rw-rw-   0        0        0      561 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/endianness/main.cpp
--rw-rw-rw-   0        0        0     1438 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/majority/main.cpp
--rw-rw-rw-   0        0        0     1000 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/manual_load/main.cpp
--rw-rw-rw-   0        0        0     9079 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/python_wrapper/test.py
--rw-rw-rw-   0        0        0     5721 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/python_wrapper/test_corpus.py
--rw-rw-rw-   0        0        0      479 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/python_wrapper_cpp/main.cpp
--rw-rw-rw-   0        0        0   113172 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/resources/a_cdf.cdf
--rw-rw-rw-   0        0        0    41097 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/resources/a_cdf_with_compressed_vars.cdf
--rw-rw-rw-   0        0        0   113172 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/resources/a_col_major_cdf.cdf
--rw-rw-rw-   0        0        0     4936 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/resources/a_compressed_cdf.cdf
--rw-rw-rw-   0        0        0     4936 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/resources/a_rle_compressed_cdf.cdf
--rw-rw-rw-   0        0        0     4444 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/resources/make_cdf.py
--rw-rw-rw-   0        0        0       21 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/resources/not_a_cdf.cdf
--rw-rw-rw-   0        0        0   117066 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/resources/testutf8.cdf
--rw-rw-rw-   0        0        0    55597 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/resources/wi_l2-30min_sms-stics-afm-magnetosphere_00000000_v01.cdf
--rw-rw-rw-   0        0        0    20148 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/simple_open/main.cpp
--rw-rw-rw-   0        0        0     2073 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/tests/zlib/main.cpp
--rw-rw-rw-   0        0        0        7 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/version.txt
--rw-rw-rw-   0        0        0     8879 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/wrapper/buffers.hpp
--rw-rw-rw-   0        0        0     7608 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/wrapper/chrono.hpp
--rw-rw-rw-   0        0        0    10735 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/wrapper/pycdfpp.cpp
--rw-r--r--   0        0        0     9108 1970-01-01 00:00:00.000000 pycdfpp-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0      210 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/.bumpversion.cfg
+-rw-rw-rw-   0        0        0     2965 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/.cirrus.yml
+-rw-rw-rw-   0        0        0      639 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/.clang-format
+-rw-rw-rw-   0        0        0     1644 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/.github/workflows/pythonpublish-linux.yml
+-rw-rw-rw-   0        0        0     1306 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/.github/workflows/pythonpublish-osx.yml
+-rw-rw-rw-   0        0        0     1292 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/.github/workflows/pythonpublish-win.yml
+-rw-rw-rw-   0        0        0      776 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/.github/workflows/tests-linux.yml
+-rw-rw-rw-   0        0        0      802 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/.github/workflows/tests-osx.yml
+-rw-rw-rw-   0        0        0     1153 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/.github/workflows/tests-windows.yml
+-rw-rw-rw-   0        0        0     1284 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/.github/workflows/tests-with-coverage.yml
+-rw-rw-rw-   0        0        0      141 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/.gitignore
+-rw-rw-rw-   0        0        0      388 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/.gitpod.Dockerfile
+-rw-rw-rw-   0        0        0      283 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/.gitpod.yml
+-rw-rw-rw-   0        0        0      321 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/.theia/settings.json
+-rw-rw-rw-   0        0        0     1585 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/COPYING
+-rw-rw-rw-   0        0        0     6690 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/README.md
+-rw-rw-rw-   0        0        0      184 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/environment.yml
+-rw-rw-rw-   0        0        0     1077 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/examples/basic_cpp/main.cpp
+-rw-rw-rw-   0        0        0   551791 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/examples/notebooks/Demo.ipynb
+-rw-rw-rw-   0        0        0     3855 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/attribute.hpp
+-rw-rw-rw-   0        0        0     8976 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/cdf-data.hpp
+-rw-rw-rw-   0        0        0     1839 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/cdf-debug.hpp
+-rw-rw-rw-   0        0        0     4980 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/cdf-endianness.hpp
+-rw-rw-rw-   0        0        0     8224 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/cdf-enums.hpp
+-rw-rw-rw-   0        0        0     2049 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/cdf-file.hpp
+-rw-rw-rw-   0        0        0     1600 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/cdf-helpers.hpp
+-rw-rw-rw-   0        0        0     3380 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/cdf-io/cdf-io-attribute.hpp
+-rw-rw-rw-   0        0        0     9593 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/cdf-io/cdf-io-buffers.hpp
+-rw-rw-rw-   0        0        0     7658 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/cdf-io/cdf-io-common.hpp
+-rw-rw-rw-   0        0        0    29307 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/cdf-io/cdf-io-desc-records.hpp
+-rw-rw-rw-   0        0        0     1957 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/cdf-io/cdf-io-rle.hpp
+-rw-rw-rw-   0        0        0    12155 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/cdf-io/cdf-io-variable.hpp
+-rw-rw-rw-   0        0        0     7435 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/cdf-io/cdf-io-zlib.hpp
+-rw-rw-rw-   0        0        0     7742 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/cdf-io/cdf-io.hpp
+-rw-rw-rw-   0        0        0     6848 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/cdf-majority-swap.hpp
+-rw-rw-rw-   0        0        0     8734 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/cdf-repr.hpp
+-rw-rw-rw-   0        0        0     1351 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/cdf.hpp
+-rw-rw-rw-   0        0        0     1453 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/chrono/cdf-chrono-constants.hpp
+-rw-rw-rw-   0        0        0     4532 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/chrono/cdf-chrono.hpp
+-rw-rw-rw-   0        0        0     5839 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/chrono/cdf-leap-seconds.h
+-rw-rw-rw-   0        0        0     3633 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/include/cdfpp/variable.hpp
+-rw-rw-rw-   0        0        0     7154 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/meson.build
+-rw-rw-rw-   0        0        0      219 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/meson_options.txt
+-rw-rw-rw-   0        0        0     8668 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/notebooks/Leap_seconds.ipynb
+-rw-rw-rw-   0        0        0     2683 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/notebooks/chrono_test_table_gen.ipynb
+-rw-rw-rw-   0        0        0      930 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1387 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/scripts/build_wheel.py
+-rw-rw-rw-   0        0        0     1253 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/scripts/version.py
+-rw-rw-rw-   0        0        0      443 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/subprojects/catch2.wrap
+-rw-rw-rw-   0        0        0      458 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/subprojects/fmt.wrap
+-rw-rw-rw-   0        0        0      463 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/subprojects/hedley.wrap
+-rw-rw-rw-   0        0        0      629 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/subprojects/pybind11.wrap
+-rw-rw-rw-   0        0        0      461 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/subprojects/zlib.wrap
+-rw-rw-rw-   0        0        0     2171 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/tests/chrono/main.cpp
+-rw-rw-rw-   0        0        0   127282 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/tests/chrono/test_values.hpp
+-rw-rw-rw-   0        0        0      561 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/tests/endianness/main.cpp
+-rw-rw-rw-   0        0        0     1438 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/tests/majority/main.cpp
+-rw-rw-rw-   0        0        0     1000 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/tests/manual_load/main.cpp
+-rw-rw-rw-   0        0        0     9079 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/tests/python_wrapper/test.py
+-rw-rw-rw-   0        0        0     5721 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/tests/python_wrapper/test_corpus.py
+-rw-rw-rw-   0        0        0      479 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/tests/python_wrapper_cpp/main.cpp
+-rw-rw-rw-   0        0        0   113172 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/tests/resources/a_cdf.cdf
+-rw-rw-rw-   0        0        0    41097 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/tests/resources/a_cdf_with_compressed_vars.cdf
+-rw-rw-rw-   0        0        0   113172 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/tests/resources/a_col_major_cdf.cdf
+-rw-rw-rw-   0        0        0     4936 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/tests/resources/a_compressed_cdf.cdf
+-rw-rw-rw-   0        0        0     4936 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/tests/resources/a_rle_compressed_cdf.cdf
+-rw-rw-rw-   0        0        0     4444 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/tests/resources/make_cdf.py
+-rw-rw-rw-   0        0        0       21 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/tests/resources/not_a_cdf.cdf
+-rw-rw-rw-   0        0        0   117066 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/tests/resources/testutf8.cdf
+-rw-rw-rw-   0        0        0    55597 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/tests/resources/wi_l2-30min_sms-stics-afm-magnetosphere_00000000_v01.cdf
+-rw-rw-rw-   0        0        0    20148 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/tests/simple_open/main.cpp
+-rw-rw-rw-   0        0        0     2073 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/tests/zlib/main.cpp
+-rw-rw-rw-   0        0        0        7 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/version.txt
+-rw-rw-rw-   0        0        0     8879 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/wrapper/buffers.hpp
+-rw-rw-rw-   0        0        0     7608 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/wrapper/chrono.hpp
+-rw-rw-rw-   0        0        0    10735 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/wrapper/pycdfpp.cpp
+-rw-r--r--   0        0        0     9108 1970-01-01 00:00:00.000000 pycdfpp-0.4.4/PKG-INFO
```

### Comparing `pycdfpp-0.4.3/.cirrus.yml` & `pycdfpp-0.4.4/.cirrus.yml`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/.clang-format` & `pycdfpp-0.4.4/.clang-format`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/.github/workflows/pythonpublish-linux.yml` & `pycdfpp-0.4.4/.github/workflows/pythonpublish-linux.yml`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             echo "/opt/python/${{ matrix.python-version }}/bin" >> $GITHUB_PATH
       - uses: actions/checkout@v3
         with:
           submodules: true
       - name: Build for Python ${{ matrix.python-version }}
         run: |
             git config --global --add safe.directory '*'
-            pip install --upgrade "meson" "ninja" "numpy" "meson-python" "build" "wheel" "twine" "auditwheel"
+            pip install --upgrade "meson" "ninja" "numpy" "meson-python==0.12.1" "build" "wheel" "twine" "auditwheel"
             python scripts/build_wheel.py
       - name: Make wheels universal
         run: for wheel in $(ls dist/*.whl); do auditwheel repair $wheel; done
       - name: Save packages as artifacts
         uses: actions/upload-artifact@v3
         with:
           name: pycdfpp-linux-${{ matrix.python-version }}
```

### Comparing `pycdfpp-0.4.3/.github/workflows/pythonpublish-osx.yml` & `pycdfpp-0.4.4/.github/workflows/pythonpublish-osx.yml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
       - uses: actions/checkout@v3
       - name: Build python wheel
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           architecture: x64
       - run: |
-          pip install --upgrade twine build ninja meson numpy wheel meson-python
+          pip install --upgrade twine build ninja meson numpy wheel meson-python==0.12.1
           CC=gcc-11 CXX=g++-11 python scripts/build_wheel.py
       - name: Save packages as artifacts
         uses: actions/upload-artifact@v3
         with:
           name: pycdfpp-MacOs-${{ matrix.python-version }}
           path: dist/*
       - name: Publish on PyPi
```

### Comparing `pycdfpp-0.4.3/.github/workflows/pythonpublish-win.yml` & `pycdfpp-0.4.4/.github/workflows/pythonpublish-win.yml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
       - uses: actions/checkout@v3
       - name: Build python wheel
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           architecture: x64
       - run: |
-          pip install --upgrade twine build ninja wheel meson numpy meson-python
+          pip install --upgrade twine build ninja wheel meson numpy meson-python==0.12.1
           python scripts/build_wheel.py
       - name: Save packages as artifacts
         uses: actions/upload-artifact@v3
         with:
           name: pycdfpp-windows-${{ matrix.python-version }}
           path: dist/*
       - name: Publish on PyPi
```

### Comparing `pycdfpp-0.4.3/.github/workflows/tests-linux.yml` & `pycdfpp-0.4.4/.github/workflows/tests-osx.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-name: Linux test matrix
+name: MacOs test matrix
 
 on: [push]
 
 jobs:
   build:
-    name: Linux test matrix
-    runs-on: ubuntu-latest
+    name: MacOs test matrix
+    runs-on: macos-latest
     continue-on-error: false
     strategy:
       fail-fast: false
       matrix:
         python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
     steps:
       - uses: actions/checkout@v3
       - name: Build python wheel
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           architecture: x64
       - name: build
         run: |
-          pip install --upgrade meson ninja numpy meson-python build wheel
-          meson -Dbuildtype=release -Dwith_tests=true . build
+          pip install --upgrade meson ninja numpy meson-python==0.12.1 build wheel twine
+          CC=gcc-11 CXX=g++-11 meson -Dbuildtype=release -Dwith_tests=true . build
           ninja --verbose -C build
       - name: run tests
         run: |
           ninja test -C build
```

### Comparing `pycdfpp-0.4.3/.github/workflows/tests-osx.yml` & `pycdfpp-0.4.4/.github/workflows/tests-linux.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-name: MacOs test matrix
+name: Linux test matrix
 
 on: [push]
 
 jobs:
   build:
-    name: MacOs test matrix
-    runs-on: macos-latest
+    name: Linux test matrix
+    runs-on: ubuntu-latest
     continue-on-error: false
     strategy:
       fail-fast: false
       matrix:
         python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
     steps:
       - uses: actions/checkout@v3
       - name: Build python wheel
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           architecture: x64
       - name: build
         run: |
-          pip install --upgrade meson ninja numpy meson-python build wheel twine
-          CC=gcc-11 CXX=g++-11 meson -Dbuildtype=release -Dwith_tests=true . build
+          pip install --upgrade meson ninja numpy meson-python==0.12.1 build wheel
+          meson -Dbuildtype=release -Dwith_tests=true . build
           ninja --verbose -C build
       - name: run tests
         run: |
           ninja test -C build
```

### Comparing `pycdfpp-0.4.3/.github/workflows/tests-windows.yml` & `pycdfpp-0.4.4/.github/workflows/tests-windows.yml`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 #        run: Remove-Item -Path "C:\Strawberry" -Force -Recurse
 #      - name: install missing zlib
 #            run: |
 #              choco uninstall -y -f mingw
 #              choco install -y mingw --version=8.1.0
       - name: build (Windows)
         run: |
-          pip install --upgrade meson ninja numpy meson-python build wheel twine
+          pip install --upgrade meson ninja numpy meson-python==0.12.1 build wheel twine
           meson -Dbuildtype=release -Dwith_tests=true . build
           ninja --verbose -C build
       - name: run tests
         run: |
           ninja test -C build
```

### Comparing `pycdfpp-0.4.3/.github/workflows/tests-with-coverage.yml` & `pycdfpp-0.4.4/.github/workflows/tests-with-coverage.yml`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
       - uses: actions/checkout@v3
         with:
           submodules: true
       - name: Install dependencies
         run: |
           sudo apt update
           sudo apt install -y python3-pip lcov g++
-          pip install --upgrade meson ninja numpy meson-python build wheel
+          pip install --upgrade meson ninja numpy meson-python==0.12.1 build wheel
       - name: Configure with meson
         run: meson -Db_coverage=true -Dwith_tests=true . build
       - name: Build (meson)
         run: ninja -C build
       - name: Run tests (meson)
         run: ninja test -C build
       - name: Generate Coverage repport
```

### Comparing `pycdfpp-0.4.3/COPYING` & `pycdfpp-0.4.4/COPYING`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/README.md` & `pycdfpp-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/examples/basic_cpp/main.cpp` & `pycdfpp-0.4.4/examples/basic_cpp/main.cpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/examples/notebooks/Demo.ipynb` & `pycdfpp-0.4.4/examples/notebooks/Demo.ipynb`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/attribute.hpp` & `pycdfpp-0.4.4/include/cdfpp/attribute.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/cdf-data.hpp` & `pycdfpp-0.4.4/include/cdfpp/cdf-data.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/cdf-debug.hpp` & `pycdfpp-0.4.4/include/cdfpp/cdf-debug.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/cdf-endianness.hpp` & `pycdfpp-0.4.4/include/cdfpp/cdf-endianness.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/cdf-enums.hpp` & `pycdfpp-0.4.4/include/cdfpp/cdf-enums.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/cdf-file.hpp` & `pycdfpp-0.4.4/include/cdfpp/cdf-file.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/cdf-helpers.hpp` & `pycdfpp-0.4.4/include/cdfpp/cdf-helpers.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-attribute.hpp` & `pycdfpp-0.4.4/include/cdfpp/cdf-io/cdf-io-attribute.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-buffers.hpp` & `pycdfpp-0.4.4/include/cdfpp/cdf-io/cdf-io-buffers.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-common.hpp` & `pycdfpp-0.4.4/include/cdfpp/cdf-io/cdf-io-common.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-desc-records.hpp` & `pycdfpp-0.4.4/include/cdfpp/cdf-io/cdf-io-desc-records.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-rle.hpp` & `pycdfpp-0.4.4/include/cdfpp/cdf-io/cdf-io-rle.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-variable.hpp` & `pycdfpp-0.4.4/include/cdfpp/cdf-io/cdf-io-variable.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io-zlib.hpp` & `pycdfpp-0.4.4/include/cdfpp/cdf-io/cdf-io-zlib.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/cdf-io/cdf-io.hpp` & `pycdfpp-0.4.4/include/cdfpp/cdf-io/cdf-io.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/cdf-majority-swap.hpp` & `pycdfpp-0.4.4/include/cdfpp/cdf-majority-swap.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/cdf-repr.hpp` & `pycdfpp-0.4.4/include/cdfpp/cdf-repr.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/cdf.hpp` & `pycdfpp-0.4.4/include/cdfpp/cdf.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/chrono/cdf-chrono-constants.hpp` & `pycdfpp-0.4.4/include/cdfpp/chrono/cdf-chrono-constants.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/chrono/cdf-chrono.hpp` & `pycdfpp-0.4.4/include/cdfpp/chrono/cdf-chrono.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/chrono/cdf-leap-seconds.h` & `pycdfpp-0.4.4/include/cdfpp/chrono/cdf-leap-seconds.h`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/include/cdfpp/variable.hpp` & `pycdfpp-0.4.4/include/cdfpp/variable.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/meson.build` & `pycdfpp-0.4.4/meson.build`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/notebooks/Leap_seconds.ipynb` & `pycdfpp-0.4.4/notebooks/Leap_seconds.ipynb`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/notebooks/chrono_test_table_gen.ipynb` & `pycdfpp-0.4.4/notebooks/chrono_test_table_gen.ipynb`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/pyproject.toml` & `pycdfpp-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
 build-backend = 'mesonpy'
-requires = ['meson-python', 'numpy']
+requires = ['meson-python==0.12.1', 'numpy']
 
 [project]
 name = "pycdfpp"
 description="A modern C++ header only cdf library"
 authors = [{name="Alexis Jeandet", email="alexis.jeandet@member.fsf.org"}]
 summary = "A simple to use CDF files reader"
 requires-python=">=3.7"
```

### Comparing `pycdfpp-0.4.3/scripts/build_wheel.py` & `pycdfpp-0.4.4/scripts/build_wheel.py`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/scripts/version.py` & `pycdfpp-0.4.4/scripts/version.py`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/subprojects/pybind11.wrap` & `pycdfpp-0.4.4/subprojects/pybind11.wrap`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/tests/chrono/main.cpp` & `pycdfpp-0.4.4/tests/chrono/main.cpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/tests/chrono/test_values.hpp` & `pycdfpp-0.4.4/tests/chrono/test_values.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/tests/endianness/main.cpp` & `pycdfpp-0.4.4/tests/endianness/main.cpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/tests/majority/main.cpp` & `pycdfpp-0.4.4/tests/majority/main.cpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/tests/manual_load/main.cpp` & `pycdfpp-0.4.4/tests/manual_load/main.cpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/tests/python_wrapper/test.py` & `pycdfpp-0.4.4/tests/python_wrapper/test.py`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/tests/python_wrapper/test_corpus.py` & `pycdfpp-0.4.4/tests/python_wrapper/test_corpus.py`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/tests/resources/a_cdf.cdf` & `pycdfpp-0.4.4/tests/resources/a_cdf.cdf`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/tests/resources/a_cdf_with_compressed_vars.cdf` & `pycdfpp-0.4.4/tests/resources/a_cdf_with_compressed_vars.cdf`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/tests/resources/a_col_major_cdf.cdf` & `pycdfpp-0.4.4/tests/resources/a_col_major_cdf.cdf`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/tests/resources/a_compressed_cdf.cdf` & `pycdfpp-0.4.4/tests/resources/a_compressed_cdf.cdf`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/tests/resources/a_rle_compressed_cdf.cdf` & `pycdfpp-0.4.4/tests/resources/a_rle_compressed_cdf.cdf`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/tests/resources/make_cdf.py` & `pycdfpp-0.4.4/tests/resources/make_cdf.py`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/tests/resources/testutf8.cdf` & `pycdfpp-0.4.4/tests/resources/testutf8.cdf`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/tests/resources/wi_l2-30min_sms-stics-afm-magnetosphere_00000000_v01.cdf` & `pycdfpp-0.4.4/tests/resources/wi_l2-30min_sms-stics-afm-magnetosphere_00000000_v01.cdf`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/tests/simple_open/main.cpp` & `pycdfpp-0.4.4/tests/simple_open/main.cpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/tests/zlib/main.cpp` & `pycdfpp-0.4.4/tests/zlib/main.cpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/wrapper/buffers.hpp` & `pycdfpp-0.4.4/wrapper/buffers.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/wrapper/chrono.hpp` & `pycdfpp-0.4.4/wrapper/chrono.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/wrapper/pycdfpp.cpp` & `pycdfpp-0.4.4/wrapper/pycdfpp.cpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.3/PKG-INFO` & `pycdfpp-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycdfpp
-Version: 0.4.3
+Version: 0.4.4
 Summary: A modern C++ header only cdf library
 Home-page: https://github.com/SciQLop/CDFpp
 Author-Email: Alexis Jeandet <alexis.jeandet@member.fsf.org>
 License: GNU GENERAL PUBLIC LICENSE
                               Version 3, 29 June 2007
         
             An easy to use ISTP loader package.
```

