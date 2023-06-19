# Comparing `tmp/funding-service-design-utils-2.0.5.tar.gz` & `tmp/funding-service-design-utils-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funding-service-design-utils-2.0.5.tar", last modified: Fri Jun  9 16:22:45 2023, max compression
+gzip compressed data, was "funding-service-design-utils-2.0.6.tar", last modified: Mon Jun 19 06:05:58 2023, max compression
```

## Comparing `funding-service-design-utils-2.0.5.tar` & `funding-service-design-utils-2.0.6.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:45.490394 funding-service-design-utils-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-06-09 16:22:45.490394 funding-service-design-utils-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:45.482394 funding-service-design-utils-2.0.5/fsd_test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_test_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:45.482394 funding-service-design-utils-2.0.5/fsd_test_utils/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_test_utils/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_test_utils/fixtures/db_fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:45.482394 funding-service-design-utils-2.0.5/fsd_test_utils/test_config/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_test_utils/test_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_test_utils/test_config/useful_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:45.482394 funding-service-design-utils-2.0.5/fsd_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:45.482394 funding-service-design-utils-2.0.5/fsd_utils/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/authentication/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/authentication/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/authentication/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/authentication/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:45.482394 funding-service-design-utils-2.0.5/fsd_utils/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/config/commonconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/config/configclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/config/notify_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:45.482394 funding-service-design-utils-2.0.5/fsd_utils/gunicorn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/gunicorn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:45.486394 funding-service-design-utils-2.0.5/fsd_utils/gunicorn/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/gunicorn/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/gunicorn/config/devtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/gunicorn/config/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:45.486394 funding-service-design-utils-2.0.5/fsd_utils/healthchecks/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/healthchecks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/healthchecks/checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/healthchecks/healthcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:45.486394 funding-service-design-utils-2.0.5/fsd_utils/locale_selector/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/locale_selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/locale_selector/get_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/locale_selector/set_lang.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:45.486394 funding-service-design-utils-2.0.5/fsd_utils/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:45.486394 funding-service-design-utils-2.0.5/fsd_utils/sentry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/sentry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/sentry/init_sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:45.486394 funding-service-design-utils-2.0.5/fsd_utils/simple_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/simple_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/simple_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/simple_utils/date_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:45.486394 funding-service-design-utils-2.0.5/fsd_utils/toggles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/toggles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/fsd_utils/toggles/toggles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:45.486394 funding-service-design-utils-2.0.5/funding_service_design_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-06-09 16:22:45.000000 funding-service-design-utils-2.0.5/funding_service_design_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-09 16:22:45.000000 funding-service-design-utils-2.0.5/funding_service_design_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:22:45.000000 funding-service-design-utils-2.0.5/funding_service_design_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-09 16:22:45.000000 funding-service-design-utils-2.0.5/funding_service_design_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-09 16:22:45.000000 funding-service-design-utils-2.0.5/funding_service_design_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 16:22:45.490394 funding-service-design-utils-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:45.490394 funding-service-design-utils-2.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/tests/test_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/tests/test_get_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/tests/test_healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-09 16:22:34.000000 funding-service-design-utils-2.0.5/tests/test_set_lang.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:58.432068 funding-service-design-utils-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-06-19 06:05:58.432068 funding-service-design-utils-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:58.428068 funding-service-design-utils-2.0.6/fsd_test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_test_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:58.428068 funding-service-design-utils-2.0.6/fsd_test_utils/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_test_utils/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_test_utils/fixtures/db_fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:58.428068 funding-service-design-utils-2.0.6/fsd_test_utils/test_config/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_test_utils/test_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_test_utils/test_config/useful_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:58.428068 funding-service-design-utils-2.0.6/fsd_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:58.428068 funding-service-design-utils-2.0.6/fsd_utils/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/authentication/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/authentication/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/authentication/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/authentication/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:58.428068 funding-service-design-utils-2.0.6/fsd_utils/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/config/commonconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/config/configclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/config/notify_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:58.428068 funding-service-design-utils-2.0.6/fsd_utils/gunicorn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/gunicorn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:58.428068 funding-service-design-utils-2.0.6/fsd_utils/gunicorn/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/gunicorn/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/gunicorn/config/devtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/gunicorn/config/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:58.432068 funding-service-design-utils-2.0.6/fsd_utils/healthchecks/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/healthchecks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/healthchecks/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/healthchecks/healthcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:58.432068 funding-service-design-utils-2.0.6/fsd_utils/locale_selector/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/locale_selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/locale_selector/get_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/locale_selector/set_lang.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:58.432068 funding-service-design-utils-2.0.6/fsd_utils/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:58.432068 funding-service-design-utils-2.0.6/fsd_utils/sentry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/sentry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/sentry/init_sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:58.432068 funding-service-design-utils-2.0.6/fsd_utils/simple_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/simple_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/simple_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/simple_utils/date_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:58.432068 funding-service-design-utils-2.0.6/fsd_utils/toggles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/toggles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/fsd_utils/toggles/toggles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:58.432068 funding-service-design-utils-2.0.6/funding_service_design_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-06-19 06:05:58.000000 funding-service-design-utils-2.0.6/funding_service_design_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-19 06:05:58.000000 funding-service-design-utils-2.0.6/funding_service_design_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 06:05:58.000000 funding-service-design-utils-2.0.6/funding_service_design_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-19 06:05:58.000000 funding-service-design-utils-2.0.6/funding_service_design_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-19 06:05:58.000000 funding-service-design-utils-2.0.6/funding_service_design_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 06:05:58.432068 funding-service-design-utils-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:58.432068 funding-service-design-utils-2.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/tests/test_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/tests/test_get_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/tests/test_healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-19 06:05:44.000000 funding-service-design-utils-2.0.6/tests/test_set_lang.py
```

### Comparing `funding-service-design-utils-2.0.5/LICENSE` & `funding-service-design-utils-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/PKG-INFO` & `funding-service-design-utils-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funding-service-design-utils
-Version: 2.0.5
+Version: 2.0.6
 Summary: Utilities used by the DLUHC Funding Service Design Team
 Author-email: DLUHC <FundingServiceDesignTeam@levellingup.gov.uk>
 License: MIT License
         
         Copyright (c) 2022 Crown Copyright (Department for Levelling Up, Housing and Communities)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `funding-service-design-utils-2.0.5/README.md` & `funding-service-design-utils-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/fsd_test_utils/fixtures/db_fixtures.py` & `funding-service-design-utils-2.0.6/fsd_test_utils/fixtures/db_fixtures.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/fsd_utils/__init__.py` & `funding-service-design-utils-2.0.6/fsd_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/fsd_utils/authentication/config.py` & `funding-service-design-utils-2.0.6/fsd_utils/authentication/config.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/fsd_utils/authentication/decorators.py` & `funding-service-design-utils-2.0.6/fsd_utils/authentication/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,20 +98,18 @@
     if f is None:
         return lambda f: login_required(
             f=f, roles_required=roles_required, return_app=return_app
         )
 
     @wraps(f)
     def _wrapper(*args, **kwargs):
-        if (
-            current_app.config.get("FLASK_ENV") == "development"
-            and current_app.config.get("DEBUG_USER_ROLE")
-            and current_app.config.get("DEBUG_USER")
-        ):
-            g.account_id = "dev-account-id"
+        if current_app.config.get(
+            "FLASK_ENV"
+        ) == "development" and current_app.config.get("DEBUG_USER_ON"):
+            g.account_id = current_app.config.get("DEBUG_USER_ACCOUNT_ID")
             g.user = User(**current_app.config.get("DEBUG_USER"))
         else:
             token_payload = _check_access_token(return_app=return_app)
             g.account_id = token_payload.get("accountId")
             g.user = User.set_with_token(token_payload)
 
         g.logout_url = _build_logout_url(return_app)
```

### Comparing `funding-service-design-utils-2.0.5/fsd_utils/authentication/models.py` & `funding-service-design-utils-2.0.6/fsd_utils/authentication/models.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/fsd_utils/authentication/utils.py` & `funding-service-design-utils-2.0.6/fsd_utils/authentication/utils.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/fsd_utils/config/commonconfig.py` & `funding-service-design-utils-2.0.6/fsd_utils/config/commonconfig.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/fsd_utils/config/configclass.py` & `funding-service-design-utils-2.0.6/fsd_utils/config/configclass.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/fsd_utils/config/notify_constants.py` & `funding-service-design-utils-2.0.6/fsd_utils/config/notify_constants.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/fsd_utils/gunicorn/config/devtest.py` & `funding-service-design-utils-2.0.6/fsd_utils/gunicorn/config/devtest.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/fsd_utils/gunicorn/config/local.py` & `funding-service-design-utils-2.0.6/fsd_utils/gunicorn/config/local.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/fsd_utils/healthchecks/checkers.py` & `funding-service-design-utils-2.0.6/fsd_utils/healthchecks/checkers.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/fsd_utils/healthchecks/healthcheck.py` & `funding-service-design-utils-2.0.6/fsd_utils/healthchecks/healthcheck.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/fsd_utils/locale_selector/get_lang.py` & `funding-service-design-utils-2.0.6/fsd_utils/locale_selector/get_lang.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/fsd_utils/locale_selector/set_lang.py` & `funding-service-design-utils-2.0.6/fsd_utils/locale_selector/set_lang.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/fsd_utils/logging/logging.py` & `funding-service-design-utils-2.0.6/fsd_utils/logging/logging.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/fsd_utils/sentry/init_sentry.py` & `funding-service-design-utils-2.0.6/fsd_utils/sentry/init_sentry.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/fsd_utils/simple_utils/date_utils.py` & `funding-service-design-utils-2.0.6/fsd_utils/simple_utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/fsd_utils/toggles/toggles.py` & `funding-service-design-utils-2.0.6/fsd_utils/toggles/toggles.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/funding_service_design_utils.egg-info/PKG-INFO` & `funding-service-design-utils-2.0.6/funding_service_design_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funding-service-design-utils
-Version: 2.0.5
+Version: 2.0.6
 Summary: Utilities used by the DLUHC Funding Service Design Team
 Author-email: DLUHC <FundingServiceDesignTeam@levellingup.gov.uk>
 License: MIT License
         
         Copyright (c) 2022 Crown Copyright (Department for Levelling Up, Housing and Communities)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `funding-service-design-utils-2.0.5/funding_service_design_utils.egg-info/SOURCES.txt` & `funding-service-design-utils-2.0.6/funding_service_design_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/pyproject.toml` & `funding-service-design-utils-2.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "funding-service-design-utils"
-version = "2.0.5"
+version = "2.0.6"
 authors = [
   { name="DLUHC", email="FundingServiceDesignTeam@levellingup.gov.uk" },
 ]
 description = "Utilities used by the DLUHC Funding Service Design Team"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10,<4.0"
```

### Comparing `funding-service-design-utils-2.0.5/tests/conftest.py` & `funding-service-design-utils-2.0.6/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
             rsa256_public_key = public_key_file.read()
 
         app_context.app.config.update(
             {
                 "FSD_LANG_COOKIE_NAME": "language",
                 "COOKIE_DOMAIN": None,
                 "FLASK_ENV": "development",
+                "DEBUG_USER_ON": True,
                 "DEBUG_USER_ROLE": "ADMIN",
                 "DEBUG_USER": {
                     "full_name": "Development User",
                     "email": "dev@example.com",
                     "roles": ["ADMIN", "TEST"],
                     "highest_role": "ADMIN",
                 },
```

### Comparing `funding-service-design-utils-2.0.5/tests/test_authentication.py` & `funding-service-design-utils-2.0.6/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/tests/test_checkers.py` & `funding-service-design-utils-2.0.6/tests/test_checkers.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/tests/test_data_utils.py` & `funding-service-design-utils-2.0.6/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/tests/test_get_lang.py` & `funding-service-design-utils-2.0.6/tests/test_get_lang.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/tests/test_healthcheck.py` & `funding-service-design-utils-2.0.6/tests/test_healthcheck.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.5/tests/test_set_lang.py` & `funding-service-design-utils-2.0.6/tests/test_set_lang.py`

 * *Files identical despite different names*

