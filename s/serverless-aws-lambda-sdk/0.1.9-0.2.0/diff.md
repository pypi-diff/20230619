# Comparing `tmp/serverless-aws-lambda-sdk-0.1.9.tar.gz` & `tmp/serverless-aws-lambda-sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/console/console/python/packages/dist/.tmp-qkqvef4t/serverless-aws-lambda-sdk-0.1.9.tar", last modified: Mon Mar 20 13:46:39 2023, max compression
+gzip compressed data, was "/home/runner/work/console/console/python/packages/dist/.tmp-h60s0tzu/serverless-aws-lambda-sdk-0.2.0.tar", last modified: Mon Jun 19 16:00:57 2023, max compression
```

## Comparing `serverless-aws-lambda-sdk-0.1.9.tar` & `serverless-aws-lambda-sdk-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:46:39.000000 serverless-aws-lambda-sdk-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-03-20 13:46:39.000000 serverless-aws-lambda-sdk-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-20 13:46:19.000000 serverless-aws-lambda-sdk-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-03-20 13:46:19.000000 serverless-aws-lambda-sdk-0.1.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:46:39.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-03-20 13:46:19.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-20 13:46:19.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-20 13:46:19.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:46:39.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk/instrument/
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-03-20 13:46:19.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk/instrument/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:46:39.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk/instrument/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:46:19.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk/instrument/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:46:39.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk/internal_extension/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:46:19.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk/internal_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-03-20 13:46:19.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk/internal_extension/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      647 2023-03-20 13:46:19.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk/internal_extension/exec_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-03-20 13:46:19.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk/internal_extension/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:46:39.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk/trace_spans/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:46:19.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk/trace_spans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-03-20 13:46:19.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk/trace_spans/aws_lambda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:46:39.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-03-20 13:46:39.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-20 13:46:39.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 13:46:39.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-20 13:46:39.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-20 13:46:39.000000 serverless-aws-lambda-sdk-0.1.9/serverless_aws_lambda_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 13:46:39.000000 serverless-aws-lambda-sdk-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-20 13:46:19.000000 serverless-aws-lambda-sdk-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:46:39.000000 serverless-aws-lambda-sdk-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-03-20 13:46:19.000000 serverless-aws-lambda-sdk-0.1.9/tests/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-03-20 13:46:19.000000 serverless-aws-lambda-sdk-0.1.9/tests/test_instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-03-20 13:46:19.000000 serverless-aws-lambda-sdk-0.1.9/tests/test_internal_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-20 13:46:19.000000 serverless-aws-lambda-sdk-0.1.9/tests/test_internal_extension_exec_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-03-20 13:46:19.000000 serverless-aws-lambda-sdk-0.1.9/tests/test_internal_extension_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/
+-rw-r--r--   0 runner    (1001) docker     (123)    21378 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/api_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/dev_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/event_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/invocation_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/payload_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/response_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrument/lib/telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/instrumentation/aws_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/internal_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/internal_extension/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3063 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/internal_extension/exec_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/internal_extension/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/lib/instrumentation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/safe_stringify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/service_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/trace_spans/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/trace_spans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk/trace_spans/aws_lambda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/serverless_aws_lambda_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:00:57.000000 serverless-aws-lambda-sdk-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-19 16:00:34.000000 serverless-aws-lambda-sdk-0.2.0/tests/test_sdk.py
```

