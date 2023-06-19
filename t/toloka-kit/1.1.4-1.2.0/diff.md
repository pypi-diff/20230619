# Comparing `tmp/toloka-kit-1.1.4.tar.gz` & `tmp/toloka-kit-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toloka-kit-1.1.4.tar", last modified: Fri Feb 24 10:28:35 2023, max compression
+gzip compressed data, was "toloka-kit-1.2.0.tar", last modified: Mon Jun 19 14:00:13 2023, max compression
```

## Comparing `toloka-kit-1.1.4.tar` & `toloka-kit-1.2.0.tar`

### file list

```diff
@@ -1,230 +1,229 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:28:35.445518 toloka-kit-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-02-24 10:28:35.445518 toloka-kit-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 10:28:35.445518 toloka-kit-1.1.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2510 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:28:35.417518 toloka-kit-1.1.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:28:35.417518 toloka-kit-1.1.4/src/async_client/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/async_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/async_client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/async_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   222399 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/async_client/client.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:28:35.417518 toloka-kit-1.1.4/src/autoquality/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/autoquality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/autoquality/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19610 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/autoquality/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/autoquality/optimizer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/autoquality/scoring.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/autoquality/scoring.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:28:35.429518 toloka-kit-1.1.4/src/client/
--rw-r--r--   0 runner    (1001) docker     (123)   163731 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   229801 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/_converter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15514 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/actions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/aggregation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/analytics_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/analytics_request.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:28:35.429518 toloka-kit-1.1.4/src/client/app/
--rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16768 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/app/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/assignment.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/attachment.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/batch_create_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/batch_create_results.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/clone_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/clone_results.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25265 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    33104 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/collectors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22331 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/conditions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/error_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/error_codes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    28730 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/filter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/message_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/message_thread.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/operation_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/operation_log.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    38784 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/owner.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:28:35.429518 toloka-kit-1.1.4/src/client/pool/
--rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22472 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/pool/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/pool/dynamic_overlap_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/pool/dynamic_overlap_config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/pool/dynamic_pricing_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/pool/dynamic_pricing_config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/pool/mixer_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/pool/mixer_config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/pool/speed_quality_balance_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/pool/speed_quality_balance_config.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:28:35.429518 toloka-kit-1.1.4/src/client/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/primitives/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14739 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/primitives/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/primitives/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/primitives/infinite_overlap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/primitives/infinite_overlap.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/primitives/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/primitives/operators.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/primitives/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/primitives/parameter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12734 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/primitives/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/primitives/retry.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:28:35.433518 toloka-kit-1.1.4/src/client/project/
--rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/field_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    17068 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/field_spec.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/localization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/localization.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/task_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/task_spec.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:28:35.433518 toloka-kit-1.1.4/src/client/project/template_builder/
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/template_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/template_builder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/template_builder/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/template_builder/actions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/template_builder/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/template_builder/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/template_builder/conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17950 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/template_builder/conditions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/template_builder/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/template_builder/data.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23859 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/template_builder/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    51953 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/template_builder/fields.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/template_builder/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19194 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/template_builder/helpers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/template_builder/layouts.py
--rw-r--r--   0 runner    (1001) docker     (123)    15389 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/template_builder/layouts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/template_builder/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    15738 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/template_builder/plugins.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19330 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/template_builder/view.py
--rw-r--r--   0 runner    (1001) docker     (123)    42359 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/template_builder/view.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/view_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/project/view_spec.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/quality_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/quality_control.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/requester.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    46903 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/search_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    86035 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/search_requests.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/search_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    19042 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/search_results.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/skill.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/solution.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    14884 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/task.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/task_distribution_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/task_distribution_function.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/task_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/task_suite.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/training.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/user.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/user_bonus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/user_bonus.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/user_restriction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/user_restriction.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/user_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/user_skill.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/webhook_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/client/webhook_subscription.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:28:35.437518 toloka-kit-1.1.4/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/metrics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/metrics/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/metrics/collector.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/metrics/jupyter_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/metrics/jupyter_dashboard.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19390 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/metrics/metrics.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22746 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/metrics/pool_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    15422 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/metrics/pool_metrics.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/metrics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:28:35.437518 toloka-kit-1.1.4/src/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/streaming/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/streaming/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17476 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/streaming/cursor.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/streaming/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/streaming/event.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/streaming/locker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/streaming/locker.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/streaming/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/streaming/observer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16206 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/streaming/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/streaming/pipeline.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/streaming/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/streaming/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/streaming/storage.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:28:35.441518 toloka-kit-1.1.4/src/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/util/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14591 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/util/_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/util/_codegen.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/util/_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/util/_docstrings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/util/_extendable_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/util/_extendable_enum.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/util/_managing_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/util/_managing_headers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/util/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/util/_typing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/util/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/util/async_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/util/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/util/stored.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/src/util/stored.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:28:35.441518 toloka-kit-1.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_aggregated_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_analytics_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15937 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_deep_clone_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13625 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_message_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_operation_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    32715 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)    29069 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    23006 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_task_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    23924 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    15977 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_user_bonus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_user_restriction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_user_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-02-24 10:28:05.000000 toloka-kit-1.1.4/tests/test_webhook_subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:28:35.441518 toloka-kit-1.1.4/toloka_kit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-02-24 10:28:35.000000 toloka-kit-1.1.4/toloka_kit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-02-24 10:28:35.000000 toloka-kit-1.1.4/toloka_kit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 10:28:35.000000 toloka-kit-1.1.4/toloka_kit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-02-24 10:28:35.000000 toloka-kit-1.1.4/toloka_kit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-24 10:28:35.000000 toloka-kit-1.1.4/toloka_kit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.195968 toloka-kit-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-19 13:59:36.000000 toloka-kit-1.2.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-19 13:59:36.000000 toloka-kit-1.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-19 13:59:36.000000 toloka-kit-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-19 13:59:36.000000 toloka-kit-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-06-19 14:00:13.195968 toloka-kit-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-06-19 13:59:36.000000 toloka-kit-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 14:00:13.195968 toloka-kit-1.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3038 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.131964 toloka-kit-1.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.131964 toloka-kit-1.2.0/src/async_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/async_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/async_client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/async_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   234034 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/async_client/client.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.135964 toloka-kit-1.2.0/src/autoquality/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/autoquality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/autoquality/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19610 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/autoquality/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/autoquality/optimizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/autoquality/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/autoquality/scoring.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.155965 toloka-kit-1.2.0/src/client/
+-rw-r--r--   0 runner    (1001) docker     (123)   174240 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   241349 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/_converter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15514 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/actions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/aggregation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/analytics_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/analytics_request.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.159965 toloka-kit-1.2.0/src/client/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    10400 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16900 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/app/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/assignment.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/attachment.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/batch_create_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/batch_create_results.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/clone_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/clone_results.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25265 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33104 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/collectors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22331 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/conditions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/error_codes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28730 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/filter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/message_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10895 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/message_thread.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/operation_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/operation_log.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38758 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/owner.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.159965 toloka-kit-1.2.0/src/client/pool/
+-rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22472 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/pool/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/pool/dynamic_overlap_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/pool/dynamic_overlap_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/pool/dynamic_pricing_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/pool/dynamic_pricing_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/pool/mixer_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/pool/mixer_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/pool/speed_quality_balance_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/pool/speed_quality_balance_config.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.163966 toloka-kit-1.2.0/src/client/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/adapters.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15884 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/infinite_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/infinite_overlap.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/operators.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/parameter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/retry.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.167966 toloka-kit-1.2.0/src/client/project/
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/field_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17068 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/field_spec.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/localization.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/task_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/task_spec.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.175966 toloka-kit-1.2.0/src/client/project/template_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/actions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/conditions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/data.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19962 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47185 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15852 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/helpers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13378 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/layouts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15278 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/plugins.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18995 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41485 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/view.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/view_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/view_spec.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/quality_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/quality_control.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/requester.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    46903 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/search_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86035 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/search_requests.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/search_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19042 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/search_results.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/skill.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/solution.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/task.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/task_distribution_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/task_distribution_function.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/task_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10033 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/task_suite.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/training.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/user.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/user_bonus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/user_bonus.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/user_restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/user_restriction.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/user_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/user_skill.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/webhook_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/webhook_subscription.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.179967 toloka-kit-1.2.0/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/collector.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14385 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/jupyter_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/jupyter_dashboard.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20330 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/metrics.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23397 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/pool_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16026 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/pool_metrics.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.183967 toloka-kit-1.2.0/src/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18175 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20538 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/cursor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/event.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/locker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/locker.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17204 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13113 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/observer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16466 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/pipeline.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/storage.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.187967 toloka-kit-1.2.0/src/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14689 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/_codegen.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/_docstrings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/_extendable_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/_extendable_enum.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/_managing_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/_managing_headers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/_typing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/async_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/stored.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/stored.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.195968 toloka-kit-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_aggregated_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_analytics_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15937 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_deep_clone_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13625 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_message_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_operation_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32761 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24016 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_user_restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_user_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_webhook_subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.195968 toloka-kit-1.2.0/toloka_kit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-06-19 14:00:13.000000 toloka-kit-1.2.0/toloka_kit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-19 14:00:13.000000 toloka-kit-1.2.0/toloka_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 14:00:13.000000 toloka-kit-1.2.0/toloka_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-19 14:00:13.000000 toloka-kit-1.2.0/toloka_kit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 14:00:13.000000 toloka-kit-1.2.0/toloka_kit.egg-info/top_level.txt
```

### Comparing `toloka-kit-1.1.4/CONTRIBUTING.md` & `toloka-kit-1.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/LICENSE` & `toloka-kit-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/PKG-INFO` & `toloka-kit-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toloka-kit
-Version: 1.1.4
+Version: 1.2.0
 Summary: Toloka API client
 Author: Vladimir Losev
 Author-email: losev@yandex-team.ru
 License: Apache 2.0
 Project-URL: Documentation, https://toloka.ai/en/docs/toloka-kit
 Project-URL: Source, https://github.com/Toloka/toloka-kit
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -44,32 +45,32 @@
 [![Coverage](https://codecov.io/gh/Toloka/toloka-kit/branch/main/graph/badge.svg)](https://codecov.io/gh/Toloka/toloka-kit)
 [![GitHub Tests](https://github.com/Toloka/toloka-kit/workflows/Tests/badge.svg?branch=main)](//github.com/Toloka/toloka-kit/actions?query=workflow:Tests)
 
 [Toloka website](https://toloka.ai/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) | [Documentation](https://toloka.ai/en/docs/toloka-kit/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) | [Issue tracker](https://github.com/Toloka/toloka-kit/issues)
 
 
 
-Toloka-Kit is a Python library for working with [Toloka API](https://toloka.ai/docs/api/concepts/about.html/?utm_source=github&utm_medium=site&utm_campaign=tolokakit). 
+Toloka-Kit is a Python library for working with [Toloka API](https://toloka.ai/docs/api/?utm_source=github&utm_medium=site&utm_campaign=tolokakit). 
 
 The API allows you to build scalable and fully automated human-in-the-loop ML pipelines, and integrate them into your processes. The toolkit makes integration easier. You can use it with Jupyter notebooks.
 
 * Support for all common Toloka use cases: creating projects, adding pools, uploading tasks, and so on.
 * Toloka entities are represented as Python classes. You can use them instead of accessing the API using JSON representations.
 * There’s no need to validate JSON files and work with them directly.
 * Support of both synchronous and asynchronous (via async/await) executions.
 * Streaming support: build complex pipelines which send and receive data in real time. For example, you can [pass data between two related projects](https://github.com/Toloka/toloka-kit/blob/main/examples/6.streaming_pipelines/streaming_pipelines.ipynb): one for data labeling, and another for its validation. 
 * [AutoQuality](https://medium.com/toloka/automating-crowdsourcing-quality-control-ad057baf00fd) feature which automatically finds the best fitting quality control rules for your project.
 
 ## Prerequisites
 
 Before you begin, make sure that:
 * You are using [Python](https://www.python.org/) v3.7 or higher.
-* You are [registered](https://toloka.ai/docs/guide/concepts/access.html/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) in Toloka as a requester.
-* You have [topped up](https://toloka.ai/docs/guide/concepts/refill.html/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) your Toloka account.
-* You have [set up an OAuth token](https://toloka.ai/docs/api/concepts/access.html/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) to access Toloka API.
+* You are [registered](https://toloka.ai/docs/guide/concepts/access/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) in Toloka as a requester.
+* You have [topped up](https://toloka.ai/docs/guide/concepts/refill/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) your Toloka account.
+* You have [set up an OAuth token](https://toloka.ai/docs/api/concepts/access/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) to access Toloka API.
 
 ## Get Started
 1. Install the Toloka-Kit package. Run the following command in the command shell:
 ```
 $ pip install toloka-kit
 ```
 For production environments, specify the exact package version. For the latest stable version, check the [project page at pypi.org](https://pypi.org/project/toloka-kit/).
@@ -106,20 +107,20 @@
 ```
 
 ## Usage examples
 [Toloka-kit usage examples](https://github.com/Toloka/toloka-kit/tree/main/examples#toloka-kit-usage-examples) - tutorials for specific data labeling tasks. They demonstrate how to work with Toloka API using Toloka-Kit.
 
 ## Documentation
 * [Toloka-Kit documentation](https://toloka.ai/en/docs/toloka-kit/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
-* [Toloka API reference](https://toloka.ai/docs/api/concepts/about.html/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
-* [Toloka web interface documentation](https://toloka.ai/docs/guide/concepts/overview.html/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
+* [Toloka API reference](https://toloka.ai/docs/api/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
+* [Toloka web interface documentation](https://toloka.ai/docs/guide/concepts/overview/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
 
 ## Support
 * To suggest a feature or report a bug, go to our [issues page](https://github.com/Toloka/toloka-kit/issues).
 * If you have any questions, feel free to ask our [Slack community](https://toloka.ai/community/?utm_source=github&utm_medium=site&utm_campaign=tolokakit).
 
 ## Contributing
 Feel free to contribute to toloka-kit. Right now, we need more [usage examples](https://github.com/Toloka/toloka-kit/tree/main/examples#need-more-examples).
 
 ## License
-© YANDEX LLC, 2020.
+© Copyright 2023 Toloka team authors.
 Licensed under the terms of the Apache License, Version 2.0. See [LICENSE](https://github.com/Toloka/toloka-kit/blob/main/LICENSE) for more details.
```

### Comparing `toloka-kit-1.1.4/README.md` & `toloka-kit-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 [![Coverage](https://codecov.io/gh/Toloka/toloka-kit/branch/main/graph/badge.svg)](https://codecov.io/gh/Toloka/toloka-kit)
 [![GitHub Tests](https://github.com/Toloka/toloka-kit/workflows/Tests/badge.svg?branch=main)](//github.com/Toloka/toloka-kit/actions?query=workflow:Tests)
 
 [Toloka website](https://toloka.ai/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) | [Documentation](https://toloka.ai/en/docs/toloka-kit/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) | [Issue tracker](https://github.com/Toloka/toloka-kit/issues)
 
 
 
-Toloka-Kit is a Python library for working with [Toloka API](https://toloka.ai/docs/api/concepts/about.html/?utm_source=github&utm_medium=site&utm_campaign=tolokakit). 
+Toloka-Kit is a Python library for working with [Toloka API](https://toloka.ai/docs/api/?utm_source=github&utm_medium=site&utm_campaign=tolokakit). 
 
 The API allows you to build scalable and fully automated human-in-the-loop ML pipelines, and integrate them into your processes. The toolkit makes integration easier. You can use it with Jupyter notebooks.
 
 * Support for all common Toloka use cases: creating projects, adding pools, uploading tasks, and so on.
 * Toloka entities are represented as Python classes. You can use them instead of accessing the API using JSON representations.
 * There’s no need to validate JSON files and work with them directly.
 * Support of both synchronous and asynchronous (via async/await) executions.
 * Streaming support: build complex pipelines which send and receive data in real time. For example, you can [pass data between two related projects](https://github.com/Toloka/toloka-kit/blob/main/examples/6.streaming_pipelines/streaming_pipelines.ipynb): one for data labeling, and another for its validation. 
 * [AutoQuality](https://medium.com/toloka/automating-crowdsourcing-quality-control-ad057baf00fd) feature which automatically finds the best fitting quality control rules for your project.
 
 ## Prerequisites
 
 Before you begin, make sure that:
 * You are using [Python](https://www.python.org/) v3.7 or higher.
-* You are [registered](https://toloka.ai/docs/guide/concepts/access.html/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) in Toloka as a requester.
-* You have [topped up](https://toloka.ai/docs/guide/concepts/refill.html/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) your Toloka account.
-* You have [set up an OAuth token](https://toloka.ai/docs/api/concepts/access.html/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) to access Toloka API.
+* You are [registered](https://toloka.ai/docs/guide/concepts/access/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) in Toloka as a requester.
+* You have [topped up](https://toloka.ai/docs/guide/concepts/refill/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) your Toloka account.
+* You have [set up an OAuth token](https://toloka.ai/docs/api/concepts/access/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) to access Toloka API.
 
 ## Get Started
 1. Install the Toloka-Kit package. Run the following command in the command shell:
 ```
 $ pip install toloka-kit
 ```
 For production environments, specify the exact package version. For the latest stable version, check the [project page at pypi.org](https://pypi.org/project/toloka-kit/).
@@ -70,20 +70,20 @@
 ```
 
 ## Usage examples
 [Toloka-kit usage examples](https://github.com/Toloka/toloka-kit/tree/main/examples#toloka-kit-usage-examples) - tutorials for specific data labeling tasks. They demonstrate how to work with Toloka API using Toloka-Kit.
 
 ## Documentation
 * [Toloka-Kit documentation](https://toloka.ai/en/docs/toloka-kit/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
-* [Toloka API reference](https://toloka.ai/docs/api/concepts/about.html/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
-* [Toloka web interface documentation](https://toloka.ai/docs/guide/concepts/overview.html/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
+* [Toloka API reference](https://toloka.ai/docs/api/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
+* [Toloka web interface documentation](https://toloka.ai/docs/guide/concepts/overview/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
 
 ## Support
 * To suggest a feature or report a bug, go to our [issues page](https://github.com/Toloka/toloka-kit/issues).
 * If you have any questions, feel free to ask our [Slack community](https://toloka.ai/community/?utm_source=github&utm_medium=site&utm_campaign=tolokakit).
 
 ## Contributing
 Feel free to contribute to toloka-kit. Right now, we need more [usage examples](https://github.com/Toloka/toloka-kit/tree/main/examples#need-more-examples).
 
 ## License
-© YANDEX LLC, 2020.
+© Copyright 2023 Toloka team authors.
 Licensed under the terms of the Apache License, Version 2.0. See [LICENSE](https://github.com/Toloka/toloka-kit/blob/main/LICENSE) for more details.
```

### Comparing `toloka-kit-1.1.4/setup.py` & `toloka-kit-1.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 # coding: utf8
 import os
+import sys
 
 from setuptools import setup, find_packages
 
 PREFIX = 'toloka'
 
 setup_py_dir = os.path.dirname(__file__)
 version_module_path = os.path.join(setup_py_dir, 'src', '__version__.py')
@@ -13,21 +14,43 @@
 
 with open(version_module_path) as f:
     exec(f.read(), about)
 
 with open('README.md') as f:
     readme = f.read()
 
+
+def get_ipython_with_version():
+    if sys.version_info < (3, 8):
+        return 'ipython < 8'
+    elif sys.version_info < (3, 9):
+        return 'ipython < 8.13'
+    return 'ipython'
+
+
 EXTRAS_REQUIRE = {
-    'dev': ['respx', 'aiohttp', 'pytest', 'pytest-lazy-fixture', 'pytest-asyncio'],
+    'dev': [
+        'aiohttp',
+        'data-science-types',
+        'flake8',
+        'mypy',
+        'pytest',
+        'pytest-asyncio',
+        'pytest-lazy-fixture',
+        'pytest-mock',
+        'pytest-timeout',
+        'respx',
+        'tox',
+        'types-urllib3',
+    ],
     'pandas': ['pandas'],
     'autoquality': ['crowd-kit >= 1.0.0'],
     's3': ['boto3 >= 1.4.7'],
     'zookeeper': ['kazoo >= 2.6.1'],
-    'jupyter-metrics': ['plotly', 'ipyplot', 'jupyter-dash'],
+    'jupyter-metrics': ['plotly', 'ipyplot', 'jupyter-dash', get_ipython_with_version()],
 }
 EXTRAS_REQUIRE['all'] = sum((deps for env, deps in EXTRAS_REQUIRE.items() if env != 'dev'), [])
 
 setup(
     name=about['__title__'],
     package_dir={PREFIX: 'src'},
     packages=['toloka', *(f'{PREFIX}.{package}' for package in find_packages('src'))],
@@ -37,20 +60,20 @@
     long_description_content_type='text/markdown',
     license=about['__license__'],
     author='Vladimir Losev',
     author_email='losev@yandex-team.ru',
     python_requires='>=3.7.0',
     install_requires=[
         'attrs >= 20.3.0',
-        'cattrs >= 1.1.1',
+        'cattrs >= 1.9',
         'cached-property; python_version < "3.8.0"',
         'filelock >= 3.2.0',
         'requests',
         'httpx',
-        'tenacity',
+        'tenacity >= 7.0.0',  # https://github.com/jd/tenacity/issues/139
         'typing-extensions',
         'urllib3 >= 1.26.0',
         'simplejson',
         'docstring-parser',
         'tqdm',
     ],
     extras_require=EXTRAS_REQUIRE,
@@ -67,13 +90,14 @@
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
         'Typing :: Typed',
     ],
 )
```

### Comparing `toloka-kit-1.1.4/src/async_client/client.pyi` & `toloka-kit-1.2.0/src/async_client/client.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -871,45 +871,44 @@
         ...
 
     async def add_message_thread_to_folders(
         self,
         message_thread_id: str,
         folders: typing.Union[typing.List[typing.Union[toloka.client.message_thread.Folder, str]], toloka.client.message_thread.MessageThreadFolders]
     ) -> toloka.client.message_thread.MessageThread:
-        """Adds a message chain to one or more folders ("unread", "important" etc.)
+        """Adds a message thread to folders.
 
         Args:
-            message_thread_id: ID of message chain.
-            folders: List of folders, where to move chain.
+            message_thread_id: The ID of the message thread.
+            folders: A list of folders where to add the thread.
 
         Returns:
-            MessageThread: Full object by ID with updated folders.
+            MessageThread: The updated message thread.
 
         Example:
             >>> toloka_client.add_message_thread_to_folders(message_thread_id='1', folders=['IMPORTANT'])
             ...
         """
         ...
 
     @typing.overload
     async def compose_message_thread(self, compose: toloka.client.message_thread.MessageThreadCompose) -> toloka.client.message_thread.MessageThread:
-        """Sends a message to a Toloker.
-
-        The sent message is added to a new message thread.
+        """Creates a message thread and sends the first thread message to Tolokers.
 
         Args:
-            compose: Message parameters.
+            compose: Parameters for creating the message thread.
 
         Returns:
-            MessageThread: New created thread.
+            MessageThread: The created message thread.
 
         Example:
-            If you want to thank Tolokers who have tried to complete your tasks, send them a nice message.
+            A message is sent to all Tolokers who have tried to complete your tasks.
+            The message is in english. Tolokers can't reply to your message.
 
-            >>> message_text = "Amazing job! We've just trained our first model with the data YOU prepared for us. Thank you!"
+            >>> message_text = "Amazing job! We've just trained our first model with the data you prepared for us. Thank you!"
             >>> toloka_client.compose_message_thread(
             >>>     recipients_select_type='ALL',
             >>>     topic={'EN': 'Thank you!'},
             >>>     text={'EN': message_text},
             >>>     answerable=False
             >>> )
             ...
@@ -923,28 +922,27 @@
         recipients_select_type: typing.Union[toloka.client.message_thread.RecipientsSelectType, str, None] = None,
         topic: typing.Optional[typing.Dict[str, str]] = None,
         text: typing.Optional[typing.Dict[str, str]] = None,
         answerable: typing.Optional[bool] = None,
         recipients_ids: typing.Optional[typing.List[str]] = None,
         recipients_filter: typing.Optional[toloka.client.filter.FilterCondition] = None
     ) -> toloka.client.message_thread.MessageThread:
-        """Sends a message to a Toloker.
-
-        The sent message is added to a new message thread.
+        """Creates a message thread and sends the first thread message to Tolokers.
 
         Args:
-            compose: Message parameters.
+            compose: Parameters for creating the message thread.
 
         Returns:
-            MessageThread: New created thread.
+            MessageThread: The created message thread.
 
         Example:
-            If you want to thank Tolokers who have tried to complete your tasks, send them a nice message.
+            A message is sent to all Tolokers who have tried to complete your tasks.
+            The message is in english. Tolokers can't reply to your message.
 
-            >>> message_text = "Amazing job! We've just trained our first model with the data YOU prepared for us. Thank you!"
+            >>> message_text = "Amazing job! We've just trained our first model with the data you prepared for us. Thank you!"
             >>> toloka_client.compose_message_thread(
             >>>     recipients_select_type='ALL',
             >>>     topic={'EN': 'Thank you!'},
             >>>     text={'EN': message_text},
             >>>     answerable=False
             >>> )
             ...
@@ -969,15 +967,15 @@
             sort: Sorting options. Default: `None`.
             limit: Returned message threads limit. The default limit is 50. The maximum allowed limit is 300.
 
         Returns:
             MessageThreadSearchResult: Found message threads and a flag showing whether there are more matching threads.
 
         Example:
-            Find all message threads in the Inbox folder.
+            Finding all message threads in the `INBOX` folder.
 
             >>> toloka_client.find_message_threads(folder='INBOX')
             ...
         """
         ...
 
     @typing.overload
@@ -1007,42 +1005,44 @@
             sort: Sorting options. Default: `None`.
             limit: Returned message threads limit. The default limit is 50. The maximum allowed limit is 300.
 
         Returns:
             MessageThreadSearchResult: Found message threads and a flag showing whether there are more matching threads.
 
         Example:
-            Find all message threads in the Inbox folder.
+            Finding all message threads in the `INBOX` folder.
 
             >>> toloka_client.find_message_threads(folder='INBOX')
             ...
         """
         ...
 
     async def reply_message_thread(
         self,
         message_thread_id: str,
         reply: toloka.client.message_thread.MessageThreadReply
     ) -> toloka.client.message_thread.MessageThread:
-        """Replies to a message in thread
+        """Sends a reply message in a thread.
 
         Args:
-            message_thread_id: In which thread to reply.
-            reply: Reply message.
+            message_thread_id: The ID of the thread.
+            reply: The reply message.
 
         Returns:
-            MessageThread: New created message.
+            MessageThread: The updated message thread.
 
         Example:
+            Sending a reply to all unread messages.
+
             >>> message_threads = toloka_client.get_message_threads(folder='UNREAD')
             >>> message_reply = {'EN': 'Thank you for your message! I will get back to you soon.'}
             >>> for thread in message_threads:
             >>>     toloka_client.reply_message_thread(
             >>>         message_thread_id=thread.id,
-            >>>         reply=toloka.message_thread.MessageThreadReply(text=message_reply)
+            >>>         reply=toloka.client.message_thread.MessageThreadReply(text=message_reply)
             >>>     )
             ...
         """
         ...
 
     @typing.overload
     def get_message_threads(
@@ -1108,22 +1108,22 @@
         ...
 
     async def remove_message_thread_from_folders(
         self,
         message_thread_id: str,
         folders: typing.Union[typing.List[typing.Union[toloka.client.message_thread.Folder, str]], toloka.client.message_thread.MessageThreadFolders]
     ) -> toloka.client.message_thread.MessageThread:
-        """Deletes a message chain from one or more folders ("unread", "important" etc.)
+        """Removes a message thread from folders.
 
         Args:
-            message_thread_id: ID of message chain.
-            folders:  List of folders, where from to remove chain.
+            message_thread_id: The ID of the message thread.
+            folders: A list of folders.
 
         Returns:
-            MessageThread: Full object by ID with updated folders.
+            MessageThread: The updated message thread.
 
         Example:
             >>> toloka_client.remove_message_thread_from_folders(message_thread_id='1', folders=['IMPORTANT'])
             ...
         """
         ...
 
@@ -2510,35 +2510,35 @@
 
         Example:
             >>> toloka_client.update_skill(skill_id=old_skill_id, skill=new_skill_object)
             ...
         """
         ...
 
-    async def get_analytics(self, stats: typing.List[toloka.client.analytics_request.AnalyticsRequest]) -> toloka.client.operations.Operation:
-        """Sends analytics queries, for example, to estimate the percentage of completed tasks in the pool
+    async def get_analytics(self, stats: typing.List[toloka.client.analytics_request.AnalyticsRequest]) -> toloka.client.operations.AnalyticsOperation:
+        """Sends analytics requests to Toloka.
 
-        Only pool analytics queries are available.
-        The values of different analytical metrics will be returned in the "details" field of the operation when it is
-        completed. See the example.
         You can request up to 10 metrics at a time.
 
+        The values of different analytical metrics are returned in the `details` field of the operation when it is completed.
+
         Args:
-            stats: Analytics queries list.
+            stats: A list of analytics requests.
 
         Returns:
-            operations.Operation: An operation that you can wait for to get the required statistics.
+            operations.AnalyticsOperation: An object to track the progress of the operation.
 
         Example:
-            How to get task completion percentage for one pool.
+            The example shows how get the percentage of completed tasks in the pool.
 
             >>> from toloka.client.analytics_request import CompletionPercentagePoolAnalytics
-            >>> operation = toloka_client.get_analytics([CompletionPercentagePoolAnalytics(subject_id=pool_id)])
+            >>> operation = toloka_client.get_analytics([CompletionPercentagePoolAnalytics(subject_id='1080020')])
             >>> operation = toloka_client.wait_operation(operation)
-            >>> print(operation.details['value'][0]['result']['value'])
+            >>> print(operation.details['value'][0])
+            >>> completed_task_percentage = operation.details['value'][0]['result']['value']
             ...
         """
         ...
 
     @typing.overload
     async def create_task(
         self,
@@ -2570,17 +2570,18 @@
         ...
 
     @typing.overload
     async def create_task(
         self,
         task: toloka.client.task.Task,
         *,
+        operation_id: typing.Optional[uuid.UUID] = ...,
+        async_mode: typing.Optional[bool] = True,
         allow_defaults: typing.Optional[bool] = None,
-        open_pool: typing.Optional[bool] = None,
-        operation_id: typing.Optional[uuid.UUID] = ...
+        open_pool: typing.Optional[bool] = None
     ) -> toloka.client.task.Task:
         """Creates a new task in Toloka.
 
         You can send a maximum of 100,000 requests of this kind per minute and a maximum of 2,000,000 requests per day.
 
         To create several tasks at once use the [create_tasks](toloka.client.TolokaClient.create_tasks.md) method.
 
@@ -2662,19 +2663,19 @@
         ...
 
     @typing.overload
     async def create_tasks(
         self,
         tasks: typing.List[toloka.client.task.Task],
         *,
+        operation_id: typing.Optional[uuid.UUID] = ...,
+        async_mode: typing.Optional[bool] = True,
         allow_defaults: typing.Optional[bool] = None,
         open_pool: typing.Optional[bool] = None,
-        operation_id: typing.Optional[uuid.UUID] = ...,
-        skip_invalid_items: typing.Optional[bool] = None,
-        async_mode: typing.Optional[bool] = True
+        skip_invalid_items: typing.Optional[bool] = None
     ) -> toloka.client.batch_create_results.TaskBatchCreateResult:
         """Creates several tasks in Toloka.
 
         You can add together general and control tasks.
         Tasks can be added to different pools.
         Note that pools must be configured before accepting new tasks. For example, [mixer configuration](toloka.client.pool.mixer_config.MixerConfig.md) must be set.
 
@@ -2756,19 +2757,19 @@
         ...
 
     @typing.overload
     async def create_tasks_async(
         self,
         tasks: typing.List[toloka.client.task.Task],
         *,
+        operation_id: typing.Optional[uuid.UUID] = ...,
+        async_mode: typing.Optional[bool] = True,
         allow_defaults: typing.Optional[bool] = None,
         open_pool: typing.Optional[bool] = None,
-        operation_id: typing.Optional[uuid.UUID] = ...,
-        skip_invalid_items: typing.Optional[bool] = None,
-        async_mode: typing.Optional[bool] = True
+        skip_invalid_items: typing.Optional[bool] = None
     ) -> toloka.client.operations.TasksCreateOperation:
         """Creates tasks in Toloka asynchronously.
 
         You can send a maximum of 100,000 requests of this kind per minute and a maximum of 2,000,000 requests per day.
 
         See also the [create_tasks](toloka.client.TolokaClient.create_tasks.md) method.
 
@@ -3077,18 +3078,17 @@
 
     @typing.overload
     async def create_task_suite(
         self,
         task_suite: toloka.client.task_suite.TaskSuite,
         *,
         operation_id: typing.Optional[uuid.UUID] = ...,
-        skip_invalid_items: typing.Optional[bool] = None,
+        async_mode: typing.Optional[bool] = True,
         allow_defaults: typing.Optional[bool] = None,
-        open_pool: typing.Optional[bool] = None,
-        async_mode: typing.Optional[bool] = True
+        open_pool: typing.Optional[bool] = None
     ) -> toloka.client.task_suite.TaskSuite:
         """Creates a task suite in Toloka.
 
         Usually, you don't need to create a task suite manually, because Toloka can group tasks into suites automatically.
 
         Use this method if you need to group specific tasks together or to set different parameters in different task suites.
 
@@ -3113,15 +3113,15 @@
         """
         ...
 
     @typing.overload
     async def create_task_suites(
         self,
         task_suites: typing.List[toloka.client.task_suite.TaskSuite],
-        parameters: typing.Optional[toloka.client.task_suite.TaskSuiteCreateRequestParameters] = None
+        parameters: typing.Optional[toloka.client.task_suite.TaskSuitesCreateRequestParameters] = None
     ) -> toloka.client.batch_create_results.TaskSuiteBatchCreateResult:
         """Creates several task suites in Toloka.
 
         Usually, you don't need to create a task suite manually, because Toloka can group tasks into suites automatically.
 
         Use this method if you need to group specific tasks together or to set different parameters in different task suites.
         Task suites can be created in different pools. You can create general and control tasks or task suites in different pools with a single method call.
@@ -3163,18 +3163,18 @@
 
     @typing.overload
     async def create_task_suites(
         self,
         task_suites: typing.List[toloka.client.task_suite.TaskSuite],
         *,
         operation_id: typing.Optional[uuid.UUID] = ...,
-        skip_invalid_items: typing.Optional[bool] = None,
+        async_mode: typing.Optional[bool] = True,
         allow_defaults: typing.Optional[bool] = None,
         open_pool: typing.Optional[bool] = None,
-        async_mode: typing.Optional[bool] = True
+        skip_invalid_items: typing.Optional[bool] = None
     ) -> toloka.client.batch_create_results.TaskSuiteBatchCreateResult:
         """Creates several task suites in Toloka.
 
         Usually, you don't need to create a task suite manually, because Toloka can group tasks into suites automatically.
 
         Use this method if you need to group specific tasks together or to set different parameters in different task suites.
         Task suites can be created in different pools. You can create general and control tasks or task suites in different pools with a single method call.
@@ -3214,15 +3214,15 @@
         """
         ...
 
     @typing.overload
     async def create_task_suites_async(
         self,
         task_suites: typing.List[toloka.client.task_suite.TaskSuite],
-        parameters: typing.Optional[toloka.client.task_suite.TaskSuiteCreateRequestParameters] = None
+        parameters: typing.Optional[toloka.client.task_suite.TaskSuitesCreateRequestParameters] = None
     ) -> toloka.client.operations.TaskSuiteCreateBatchOperation:
         """Creates several task suites in Toloka asynchronously.
 
         You can send a maximum of 100,000 requests of this kind per minute and 2,000,000 requests per day.
         It is recommended that you create no more than 10,000 task suites in a single request.
 
         See also the [create_task_suites](toloka.client.TolokaClient.create_task_suites.md) method.
@@ -3254,18 +3254,18 @@
 
     @typing.overload
     async def create_task_suites_async(
         self,
         task_suites: typing.List[toloka.client.task_suite.TaskSuite],
         *,
         operation_id: typing.Optional[uuid.UUID] = ...,
-        skip_invalid_items: typing.Optional[bool] = None,
+        async_mode: typing.Optional[bool] = True,
         allow_defaults: typing.Optional[bool] = None,
         open_pool: typing.Optional[bool] = None,
-        async_mode: typing.Optional[bool] = True
+        skip_invalid_items: typing.Optional[bool] = None
     ) -> toloka.client.operations.TaskSuiteCreateBatchOperation:
         """Creates several task suites in Toloka asynchronously.
 
         You can send a maximum of 100,000 requests of this kind per minute and 2,000,000 requests per day.
         It is recommended that you create no more than 10,000 task suites in a single request.
 
         See also the [create_task_suites](toloka.client.TolokaClient.create_task_suites.md) method.
@@ -3634,26 +3634,26 @@
         request: toloka.client.search_requests.OperationSearchRequest,
         batch_size: typing.Optional[int] = None
     ) -> toloka.util.async_utils.AsyncGenAdapter[toloka.client.operations.Operation, None]:
         """Finds all operations that match certain rules and returns them in an iterable object
 
         `get_operations` returns a generator. You can iterate over all found operations using the generator. Several requests to the Toloka server are possible while iterating.
 
-         If you need to sort operations use the [find_operations](toloka.client.TolokaClient.find_operations.md) method.
+        If you need to sort operations use the [find_operations](toloka.client.TolokaClient.find_operations.md) method.
+
+        Args:
+            request: Search criteria.
+            batch_size: Returned operations limit for each request. The default batch_size is 50. The maximum allowed batch_size is 500.
 
-         Args:
-             request: Search criteria.
-             batch_size: Returned operations limit for each request. The default batch_size is 50. The maximum allowed batch_size is 500.
-
-         Yields:
-             Operation: The next matching operations.
-
-         Example:
-             >>> bonuses = list(toloka_client.get_operations(submitted_lt='2021-06-01T00:00:00'))
-             ...
+        Yields:
+            Operation: The next matching operations.
+
+        Example:
+            >>> bonuses = list(toloka_client.get_operations(submitted_lt='2021-06-01T00:00:00'))
+            ...
         """
         ...
 
     @typing.overload
     def get_operations(
         self,
         type: typing.Optional[toloka.client.operations.OperationType] = None,
@@ -3672,26 +3672,26 @@
         finished_gte: typing.Optional[datetime.datetime] = None,
         batch_size: typing.Optional[int] = None
     ) -> toloka.util.async_utils.AsyncGenAdapter[toloka.client.operations.Operation, None]:
         """Finds all operations that match certain rules and returns them in an iterable object
 
         `get_operations` returns a generator. You can iterate over all found operations using the generator. Several requests to the Toloka server are possible while iterating.
 
-         If you need to sort operations use the [find_operations](toloka.client.TolokaClient.find_operations.md) method.
+        If you need to sort operations use the [find_operations](toloka.client.TolokaClient.find_operations.md) method.
+
+        Args:
+            request: Search criteria.
+            batch_size: Returned operations limit for each request. The default batch_size is 50. The maximum allowed batch_size is 500.
+
+        Yields:
+            Operation: The next matching operations.
 
-         Args:
-             request: Search criteria.
-             batch_size: Returned operations limit for each request. The default batch_size is 50. The maximum allowed batch_size is 500.
-
-         Yields:
-             Operation: The next matching operations.
-
-         Example:
-             >>> bonuses = list(toloka_client.get_operations(submitted_lt='2021-06-01T00:00:00'))
-             ...
+        Example:
+            >>> bonuses = list(toloka_client.get_operations(submitted_lt='2021-06-01T00:00:00'))
+            ...
         """
         ...
 
     async def get_operation_log(self, operation_id: str) -> typing.List[toloka.client.operation_log.OperationLogItem]:
         """Reads information about validation errors and which task (or task suites) were created
 
         You don't need to call this method if you use "create_tasks" for creating tasks ("create_task_suites" for task suites).
@@ -3752,15 +3752,15 @@
 
     @typing.overload
     async def create_user_bonus(
         self,
         user_bonus: toloka.client.user_bonus.UserBonus,
         *,
         operation_id: typing.Optional[uuid.UUID] = ...,
-        skip_invalid_items: typing.Optional[bool] = None
+        async_mode: typing.Optional[bool] = True
     ) -> toloka.client.user_bonus.UserBonus:
         """Issues payments directly to a Toloker.
 
         You can send a maximum of 10,000 requests of this kind per day.
 
         Args:
             user_bonus: To whom, how much to pay and for what.
@@ -3792,15 +3792,15 @@
         """
         ...
 
     @typing.overload
     async def create_user_bonuses(
         self,
         user_bonuses: typing.List[toloka.client.user_bonus.UserBonus],
-        parameters: typing.Optional[toloka.client.user_bonus.UserBonusCreateRequestParameters] = None
+        parameters: typing.Optional[toloka.client.user_bonus.UserBonusesCreateRequestParameters] = None
     ) -> toloka.client.batch_create_results.UserBonusBatchCreateResult:
         """Creates rewards for Tolokers.
 
         Right now it's safer to use asynchronous version: "create_user_bonuses_async"
         You can send a maximum of 10,000 requests of this kind per day.
 
         Args:
@@ -3848,14 +3848,15 @@
 
     @typing.overload
     async def create_user_bonuses(
         self,
         user_bonuses: typing.List[toloka.client.user_bonus.UserBonus],
         *,
         operation_id: typing.Optional[uuid.UUID] = ...,
+        async_mode: typing.Optional[bool] = True,
         skip_invalid_items: typing.Optional[bool] = None
     ) -> toloka.client.batch_create_results.UserBonusBatchCreateResult:
         """Creates rewards for Tolokers.
 
         Right now it's safer to use asynchronous version: "create_user_bonuses_async"
         You can send a maximum of 10,000 requests of this kind per day.
 
@@ -3902,15 +3903,15 @@
         """
         ...
 
     @typing.overload
     async def create_user_bonuses_async(
         self,
         user_bonuses: typing.List[toloka.client.user_bonus.UserBonus],
-        parameters: typing.Optional[toloka.client.user_bonus.UserBonusCreateRequestParameters] = None
+        parameters: typing.Optional[toloka.client.user_bonus.UserBonusesCreateRequestParameters] = None
     ) -> toloka.client.operations.UserBonusCreateBatchOperation:
         """Issues payments directly to Tolokers, asynchronously creates many `UserBonus` instances.
 
         You can send a maximum of 10,000 requests of this kind per day.
 
         Args:
             user_bonuses: To whom, how much to pay and for what.
@@ -3957,14 +3958,15 @@
 
     @typing.overload
     async def create_user_bonuses_async(
         self,
         user_bonuses: typing.List[toloka.client.user_bonus.UserBonus],
         *,
         operation_id: typing.Optional[uuid.UUID] = ...,
+        async_mode: typing.Optional[bool] = True,
         skip_invalid_items: typing.Optional[bool] = None
     ) -> toloka.client.operations.UserBonusCreateBatchOperation:
         """Issues payments directly to Tolokers, asynchronously creates many `UserBonus` instances.
 
         You can send a maximum of 10,000 requests of this kind per day.
 
         Args:
@@ -4095,26 +4097,26 @@
         request: toloka.client.search_requests.UserBonusSearchRequest,
         batch_size: typing.Optional[int] = None
     ) -> toloka.util.async_utils.AsyncGenAdapter[toloka.client.user_bonus.UserBonus, None]:
         """Finds all Tolokers' rewards that match certain rules and returns them in an iterable object
 
         `get_user_bonuses` returns a generator. You can iterate over all found Tolokers' rewards using the generator. Several requests to the Toloka server are possible while iterating.
 
-         If you need to sort rewards use the [find_user_bonuses](toloka.client.TolokaClient.find_user_bonuses.md) method.
+        If you need to sort rewards use the [find_user_bonuses](toloka.client.TolokaClient.find_user_bonuses.md) method.
 
-         Args:
-             request: Search criteria.
-             batch_size: Returned Tolokers' rewards limit for each request. The maximum allowed batch_size is 300.
-
-         Yields:
-             UserBonus: The next matching Toloker's reward.
-
-         Example:
-             >>> bonuses = list(toloka_client.get_user_bonuses(created_lt='2021-06-01T00:00:00'))
-             ...
+        Args:
+            request: Search criteria.
+            batch_size: Returned Tolokers' rewards limit for each request. The maximum allowed batch_size is 300.
+
+        Yields:
+            UserBonus: The next matching Toloker's reward.
+
+        Example:
+            >>> bonuses = list(toloka_client.get_user_bonuses(created_lt='2021-06-01T00:00:00'))
+            ...
         """
         ...
 
     @typing.overload
     def get_user_bonuses(
         self,
         user_id: typing.Optional[str] = None,
@@ -4130,26 +4132,26 @@
         created_gte: typing.Optional[datetime.datetime] = None,
         batch_size: typing.Optional[int] = None
     ) -> toloka.util.async_utils.AsyncGenAdapter[toloka.client.user_bonus.UserBonus, None]:
         """Finds all Tolokers' rewards that match certain rules and returns them in an iterable object
 
         `get_user_bonuses` returns a generator. You can iterate over all found Tolokers' rewards using the generator. Several requests to the Toloka server are possible while iterating.
 
-         If you need to sort rewards use the [find_user_bonuses](toloka.client.TolokaClient.find_user_bonuses.md) method.
+        If you need to sort rewards use the [find_user_bonuses](toloka.client.TolokaClient.find_user_bonuses.md) method.
 
-         Args:
-             request: Search criteria.
-             batch_size: Returned Tolokers' rewards limit for each request. The maximum allowed batch_size is 300.
-
-         Yields:
-             UserBonus: The next matching Toloker's reward.
-
-         Example:
-             >>> bonuses = list(toloka_client.get_user_bonuses(created_lt='2021-06-01T00:00:00'))
-             ...
+        Args:
+            request: Search criteria.
+            batch_size: Returned Tolokers' rewards limit for each request. The maximum allowed batch_size is 300.
+
+        Yields:
+            UserBonus: The next matching Toloker's reward.
+
+        Example:
+            >>> bonuses = list(toloka_client.get_user_bonuses(created_lt='2021-06-01T00:00:00'))
+            ...
         """
         ...
 
     @typing.overload
     async def find_user_restrictions(
         self,
         request: toloka.client.search_requests.UserRestrictionSearchRequest,
@@ -4565,25 +4567,24 @@
         Example:
             >>> toloka_client.delete_user_skill(user_skill_id='1')
             ...
         """
         ...
 
     async def upsert_webhook_subscriptions(self, subscriptions: typing.List[toloka.client.webhook_subscription.WebhookSubscription]) -> toloka.client.batch_create_results.WebhookSubscriptionBatchCreateResult:
-        """Creates (upsert) many webhook-subscriptions.
+        """Creates (upsert) webhook subscriptions.
 
         Args:
-            subscriptions: List of webhook-subscriptions, that will be created.
+            subscriptions: A list of webhook subscriptions to be created.
 
         Returns:
-            batch_create_results.WebhookSubscriptionBatchCreateResult: Result of subscriptions creation.
-                Contains created subscriptions in `items` and problems in "validation_errors".
+            batch_create_results.WebhookSubscriptionBatchCreateResult: The result of the operation.
 
         Raises:
-            ValidationApiError: If no subscriptions were created.
+            ValidationApiError: No subscriptions were created.
 
         Example:
             How to create several subscriptions.
 
             >>> created_result = toloka_client.upsert_webhook_subscriptions([
             >>>     {
             >>>         'webhook_url': 'https://awesome-requester.com/toloka-webhook',
@@ -4836,14 +4837,26 @@
     ) -> toloka.client.search_results.AppProjectSearchResult:
         """Finds App projects that match certain criteria.
 
         The number of returned projects is limited. To find remaining projects call `find_app_projects` with updated search criteria.
 
         To iterate over all matching projects you may use the [get_app_projects](toloka.client.TolokaClient.get_app_projects.md) method.
 
+        Example:
+            Searching active projects based on the App solution with the specified ID.
+
+            >>> search = toloka_client.find_app_projects(
+            >>>     app_id = '9lZaMl363jahzra1rrYq', status = 'READY')
+            >>> for app_project in search.content:
+            >>>     print(app_project.id, app_project.name)
+            >>>
+            >>> if search.has_more:
+            >>>     print('There are more App projects...')
+            ...
+
         Args:
             request: Search criteria.
             sort: The order and direction of sorting the results.
             limit: Returned projects limit. The maximum limit is 5000.
 
         Returns:
             AppProjectSearchResult: Found projects and a flag showing whether there are more matching projects exceeding the limit.
@@ -4876,14 +4889,26 @@
     ) -> toloka.client.search_results.AppProjectSearchResult:
         """Finds App projects that match certain criteria.
 
         The number of returned projects is limited. To find remaining projects call `find_app_projects` with updated search criteria.
 
         To iterate over all matching projects you may use the [get_app_projects](toloka.client.TolokaClient.get_app_projects.md) method.
 
+        Example:
+            Searching active projects based on the App solution with the specified ID.
+
+            >>> search = toloka_client.find_app_projects(
+            >>>     app_id = '9lZaMl363jahzra1rrYq', status = 'READY')
+            >>> for app_project in search.content:
+            >>>     print(app_project.id, app_project.name)
+            >>>
+            >>> if search.has_more:
+            >>>     print('There are more App projects...')
+            ...
+
         Args:
             request: Search criteria.
             sort: The order and direction of sorting the results.
             limit: Returned projects limit. The maximum limit is 5000.
 
         Returns:
             AppProjectSearchResult: Found projects and a flag showing whether there are more matching projects exceeding the limit.
@@ -4898,14 +4923,20 @@
     ) -> toloka.util.async_utils.AsyncGenAdapter[toloka.client.app.AppProject, None]:
         """Finds all App projects that match certain criteria.
 
         `get_app_projects` returns a generator. You can iterate over all found projects using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort App projects use the [find_app_projects](toloka.client.TolokaClient.find_app_projects.md) method.
 
+        Example:
+            >>> app_projects = toloka_client.get_app_projects(scope='MY')
+            >>> for app_project in app_projects:
+            >>>     print(app_project.id, app_project.status, app_project.name)
+            ...
+
         Args:
             request: Search criteria.
             batch_size: Returned projects limit for each request. The maximum batch_size is 5000.
 
         Yields:
             AppProject: The next matching App project.
         """
@@ -4936,63 +4967,121 @@
     ) -> toloka.util.async_utils.AsyncGenAdapter[toloka.client.app.AppProject, None]:
         """Finds all App projects that match certain criteria.
 
         `get_app_projects` returns a generator. You can iterate over all found projects using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort App projects use the [find_app_projects](toloka.client.TolokaClient.find_app_projects.md) method.
 
+        Example:
+            >>> app_projects = toloka_client.get_app_projects(scope='MY')
+            >>> for app_project in app_projects:
+            >>>     print(app_project.id, app_project.status, app_project.name)
+            ...
+
         Args:
             request: Search criteria.
             batch_size: Returned projects limit for each request. The maximum batch_size is 5000.
 
         Yields:
             AppProject: The next matching App project.
         """
         ...
 
     async def create_app_project(self, app_project: toloka.client.app.AppProject) -> toloka.client.app.AppProject:
         """Creates an App project in Toloka.
 
+        Example:
+            >>> app_project = toloka.AppProject(
+            >>>   app_id='9lZaMl363jahzra1rrYq',
+            >>>   name='Example project (product relevance)',
+            >>>   parameters={
+            >>>     "default_language": "en",
+            >>>     "name": "Product relevance project",
+            >>>     "instruction_classes": [
+            >>>       {
+            >>>         "description": "The product is relevant to the query.",
+            >>>         "label": "Relevant",
+            >>>         "value": "relevant"
+            >>>       },
+            >>>       {
+            >>>         "description": "The product is not completely relevant to the query.",
+            >>>         "label": "Irrelevant",
+            >>>         "value": "irrelevant"
+            >>>       }
+            >>>     ],
+            >>>     "instruction_examples": [
+            >>>       {
+            >>>         "description": "The product exactly matches the query.",
+            >>>         "label": "relevant",
+            >>>         "query": "some search query",
+            >>>         "screenshot_url": "https://example.com/1"
+            >>>       },
+            >>>       {
+            >>>         "description": "The product shape matches but the product color does not.",
+            >>>         "label": "irrelevant",
+            >>>         "query": "other search query",
+            >>>         "screenshot_url": "https://example.com/2"
+            >>>       }
+            >>>     ]
+            >>>   }
+            >>> )
+            >>> app_project = toloka_client.create_app_project(app_project)
+            >>> print(app_project.created, app_project.status)
+            ...
+
         Args:
             app_project: The project with parameters.
 
         Returns:
             AppProject: Created App project with updated parameters.
         """
         ...
 
     async def get_app_project(self, app_project_id: str) -> toloka.client.app.AppProject:
         """Gets information from Toloka about an App project.
 
+        Example:
+            >>> app_project = toloka_client.get_app_project('Q2d15QBjpwWuDz8Z321g')
+            >>> print(app_project.created, app_project.name)
+            ...
+
         Args:
             app_project_id: The ID of the project.
 
         Returns:
             AppProject: The App project.
         """
         ...
 
     async def archive_app_project(self, app_project_id: str) -> toloka.client.app.AppProject:
         """Archives an App project.
 
         The project changes its status to `ARCHIVED`.
 
+        Example:
+            >>> toloka_client.archive_app_project('Q2d15QBjpwWuDz8Z321g')
+            ...
+
         Args:
             app_project_id: The ID of the project.
 
         Returns:
             AppProject: The App project with updated status.
         """
         ...
 
     async def unarchive_app_project(self, app_project_id: str) -> toloka.client.app.AppProject:
         """Unarchives an App project.
 
         Previous project status, which was before archiving, is restored.
 
+        Example:
+            >>> toloka_client.unarchive_app_project('Q2d15QBjpwWuDz8Z321g')
+            ...
+
         Args:
             app_project_id: The ID of the project.
 
         Returns:
             AppProject: The App project with updated status.
         """
         ...
@@ -5006,14 +5095,23 @@
     ) -> toloka.client.search_results.AppSearchResult:
         """Finds App solutions that match certain criteria.
 
         The number of returned solutions is limited. To find remaining solutions call `find_apps` with updated search criteria.
 
         To iterate over all matching solutions you may use the [get_apps](toloka.client.TolokaClient.get_apps.md) method.
 
+        Example:
+            >>> search = toloka_client.find_apps()
+            >>> for app in search.content:
+            >>>     print(app.id, app.name)
+            >>>
+            >>> if search.has_more:
+            >>>     print('There are more App solutions...')
+            ...
+
         Args:
             request: Search criteria.
             sort: Sorting options. Default: `None`.
             limit: Returned solutions limit. The maximum allowed limit is 1000.
 
         Returns:
             AppSearchResult: Found solutions and a flag showing whether there are more matching solutions exceeding the limit.
@@ -5034,14 +5132,23 @@
     ) -> toloka.client.search_results.AppSearchResult:
         """Finds App solutions that match certain criteria.
 
         The number of returned solutions is limited. To find remaining solutions call `find_apps` with updated search criteria.
 
         To iterate over all matching solutions you may use the [get_apps](toloka.client.TolokaClient.get_apps.md) method.
 
+        Example:
+            >>> search = toloka_client.find_apps()
+            >>> for app in search.content:
+            >>>     print(app.id, app.name)
+            >>>
+            >>> if search.has_more:
+            >>>     print('There are more App solutions...')
+            ...
+
         Args:
             request: Search criteria.
             sort: Sorting options. Default: `None`.
             limit: Returned solutions limit. The maximum allowed limit is 1000.
 
         Returns:
             AppSearchResult: Found solutions and a flag showing whether there are more matching solutions exceeding the limit.
@@ -5056,14 +5163,20 @@
     ) -> toloka.util.async_utils.AsyncGenAdapter[toloka.client.app.App, None]:
         """Finds all App solutions that match certain criteria.
 
         `get_apps` returns a generator. You can iterate over all found solutions using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort solutions use the [find_apps](toloka.client.TolokaClient.find_apps.md) method.
 
+        Example:
+            >>> apps = toloka_client.get_apps()
+            >>> for app in apps:
+            >>>     print(app.id, app.name)
+            ...
+
         Args:
             request: Search criteria.
             batch_size: Returned solutions limit for each request. The maximum allowed batch_size is 1000.
 
         Yields:
             App: The next matching solution.
         """
@@ -5082,14 +5195,20 @@
     ) -> toloka.util.async_utils.AsyncGenAdapter[toloka.client.app.App, None]:
         """Finds all App solutions that match certain criteria.
 
         `get_apps` returns a generator. You can iterate over all found solutions using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort solutions use the [find_apps](toloka.client.TolokaClient.find_apps.md) method.
 
+        Example:
+            >>> apps = toloka_client.get_apps()
+            >>> for app in apps:
+            >>>     print(app.id, app.name)
+            ...
+
         Args:
             request: Search criteria.
             batch_size: Returned solutions limit for each request. The maximum allowed batch_size is 1000.
 
         Yields:
             App: The next matching solution.
         """
@@ -5098,14 +5217,20 @@
     async def get_app(
         self,
         app_id: str,
         lang: typing.Optional[str] = None
     ) -> toloka.client.app.App:
         """Gets information from Toloka about an App solution.
 
+        Example:
+            >>> app = toloka_client.get_app('2eN4l59qL2xHB5b8Jqp6')
+            >>> print(app.id, app.name)
+            >>> print(app.description)
+            ...
+
         Args:
             app_id: The ID of the solution.
             lang: ISO 639 language code.
 
         Returns:
             App: The App solution.
         """
@@ -5121,14 +5246,27 @@
     ) -> toloka.client.search_results.AppItemSearchResult:
         """Finds task items that match certain criteria in an App project.
 
         The number of returned items is limited. To find remaining items call `find_app_items` with updated search criteria.
 
         To iterate over all matching items you may use the [get_app_items](toloka.client.TolokaClient.get_app_items.md) method.
 
+        Example:
+            Finding items in an App project that were created starting some date.
+            >>> search = toloka_client.find_app_items(
+            >>>     app_project_id = 'Q2d15QBjpwWuDz8Z321g',
+            >>>     created_gte = '2022-06-16',
+            >>>     sort = 'created')
+            >>> for app_item in search.content:
+            >>>     print(app_item.id, app_item.created_at)
+            >>>
+            >>> if search.has_more:
+            >>>     print('...')
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             request: Search criteria.
             sort: Sorting options. Default: `None`.
             limit: Returned items limit. The maximum allowed limit is 1000.
 
         Returns:
@@ -5160,14 +5298,27 @@
     ) -> toloka.client.search_results.AppItemSearchResult:
         """Finds task items that match certain criteria in an App project.
 
         The number of returned items is limited. To find remaining items call `find_app_items` with updated search criteria.
 
         To iterate over all matching items you may use the [get_app_items](toloka.client.TolokaClient.get_app_items.md) method.
 
+        Example:
+            Finding items in an App project that were created starting some date.
+            >>> search = toloka_client.find_app_items(
+            >>>     app_project_id = 'Q2d15QBjpwWuDz8Z321g',
+            >>>     created_gte = '2022-06-16',
+            >>>     sort = 'created')
+            >>> for app_item in search.content:
+            >>>     print(app_item.id, app_item.created_at)
+            >>>
+            >>> if search.has_more:
+            >>>     print('...')
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             request: Search criteria.
             sort: Sorting options. Default: `None`.
             limit: Returned items limit. The maximum allowed limit is 1000.
 
         Returns:
@@ -5184,14 +5335,20 @@
     ) -> toloka.util.async_utils.AsyncGenAdapter[toloka.client.app.AppItem, None]:
         """Finds all App task items that match certain criteria in an App project.
 
         `get_app_items` returns a generator. You can iterate over all found items using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort items use the [find_app_items](toloka.client.TolokaClient.find_app_items.md) method.
 
+        Example:
+            >>> items = toloka_client.get_app_items('Q2d15QBjpwWuDz8Z321g')
+            >>> for item in items:
+            >>>     print(item.id, item.status, item.finished_at)
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             request: Search criteria.
             batch_size: Returned items limit for each request. The maximum allowed batch_size is 1000.
 
         Yields:
             AppItem: The next matching item.
@@ -5221,14 +5378,20 @@
     ) -> toloka.util.async_utils.AsyncGenAdapter[toloka.client.app.AppItem, None]:
         """Finds all App task items that match certain criteria in an App project.
 
         `get_app_items` returns a generator. You can iterate over all found items using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort items use the [find_app_items](toloka.client.TolokaClient.find_app_items.md) method.
 
+        Example:
+            >>> items = toloka_client.get_app_items('Q2d15QBjpwWuDz8Z321g')
+            >>> for item in items:
+            >>>     print(item.id, item.status, item.finished_at)
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             request: Search criteria.
             batch_size: Returned items limit for each request. The maximum allowed batch_size is 1000.
 
         Yields:
             AppItem: The next matching item.
@@ -5239,14 +5402,28 @@
     async def create_app_item(
         self,
         app_project_id: str,
         app_item: toloka.client.app.AppItem
     ) -> toloka.client.app.AppItem:
         """Creates an App task item in Toloka.
 
+        Example:
+            The following example is suitable for a project
+            that requires `query` and `website_url` keys to be present in input data.
+
+            >>> new_item = {
+            >>>     'batch_id' : '4Va2BBWKL88S4QyAgVje',
+            >>>     'input_data' : {
+            >>>         'id':'40', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'
+            >>>     }
+            >>> }
+            >>> new_item = toloka_client.create_app_item(app_project_id = 'Q2d15QBjpwWuDz8Z321g', app_item = new_item)
+            >>> print(new_item.created_at)
+            ...
+
         Args:
             app_project_id: The ID of the App project to create the item in.
             app_item: The task item with parameters.
 
         Returns:
             AppItem: Created App task item with updated parameters.
         """
@@ -5258,14 +5435,28 @@
         app_project_id: str,
         *,
         batch_id: typing.Optional[str] = None,
         input_data: typing.Optional[typing.Dict[str, typing.Any]] = None
     ) -> toloka.client.app.AppItem:
         """Creates an App task item in Toloka.
 
+        Example:
+            The following example is suitable for a project
+            that requires `query` and `website_url` keys to be present in input data.
+
+            >>> new_item = {
+            >>>     'batch_id' : '4Va2BBWKL88S4QyAgVje',
+            >>>     'input_data' : {
+            >>>         'id':'40', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'
+            >>>     }
+            >>> }
+            >>> new_item = toloka_client.create_app_item(app_project_id = 'Q2d15QBjpwWuDz8Z321g', app_item = new_item)
+            >>> print(new_item.created_at)
+            ...
+
         Args:
             app_project_id: The ID of the App project to create the item in.
             app_item: The task item with parameters.
 
         Returns:
             AppItem: Created App task item with updated parameters.
         """
@@ -5275,14 +5466,25 @@
     async def create_app_items(
         self,
         app_project_id: str,
         request: toloka.client.app.AppItemsCreateRequest
     ):
         """Creates task items in an App project in Toloka and adds them to an existing batch.
 
+        Example:
+            The following example is suitable for a project
+            that requires `query` and `website_url` keys to be present in input data.
+
+            >>> new_items = [
+            >>>     {'id':'20', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'},
+            >>>     {'id':'21', 'query':'crowd kit', 'website_url':'https://toloka.ai/en/docs/crowd-kit'}
+            >>> ]
+            >>> toloka_client.create_app_items(app_project_id = 'Q2d15QBjpwWuDz8Z321g', batch_id = '4Va2BBWKL88S4QyAgVje', items = new_items)
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             request: The request parameters.
         """
         ...
 
     @typing.overload
@@ -5291,27 +5493,44 @@
         app_project_id: str,
         *,
         batch_id: typing.Optional[str] = None,
         items: typing.Optional[typing.List[typing.Dict[str, typing.Any]]] = None
     ):
         """Creates task items in an App project in Toloka and adds them to an existing batch.
 
+        Example:
+            The following example is suitable for a project
+            that requires `query` and `website_url` keys to be present in input data.
+
+            >>> new_items = [
+            >>>     {'id':'20', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'},
+            >>>     {'id':'21', 'query':'crowd kit', 'website_url':'https://toloka.ai/en/docs/crowd-kit'}
+            >>> ]
+            >>> toloka_client.create_app_items(app_project_id = 'Q2d15QBjpwWuDz8Z321g', batch_id = '4Va2BBWKL88S4QyAgVje', items = new_items)
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             request: The request parameters.
         """
         ...
 
     async def get_app_item(
         self,
         app_project_id: str,
         app_item_id: str
     ) -> toloka.client.app.AppItem:
         """Gets information from Toloka about an App task item.
 
+        Example:
+            >>> item = toloka_client.get_app_item(app_project_id = 'Q2d15QBjpwWuDz8Z321g', app_item_id = 'V40aPPA2j64TORQyY54Z')
+            >>> print(item.input_data)
+            >>> print(item.output_data)
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             app_item_id: The ID of the item.
 
         Returns:
             AppItem: The App task item.
         """
@@ -5389,14 +5608,20 @@
     ) -> toloka.util.async_utils.AsyncGenAdapter[toloka.client.app.AppBatch, None]:
         """Finds all batches that match certain criteria in an App project.
 
         `get_app_batches` returns a generator. You can iterate over all found batches using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort batches use the [find_app_batches](toloka.client.TolokaClient.find_app_batches.md) method.
 
+        Example:
+            >>> batches = toloka_client.get_app_batches(app_project_id = 'Q2d15QBjpwWuDz8Z321g', status = 'NEW')
+            >>> for batch in batches:
+            >>>     print(batch.id, batch.status, batch.items_count)
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             request: Search criteria.
             batch_size: Returned app batches limit for each request. The maximum allowed batch_size is 1000.
 
         Yields:
             AppBatch: The next matching batch.
@@ -5425,14 +5650,20 @@
     ) -> toloka.util.async_utils.AsyncGenAdapter[toloka.client.app.AppBatch, None]:
         """Finds all batches that match certain criteria in an App project.
 
         `get_app_batches` returns a generator. You can iterate over all found batches using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort batches use the [find_app_batches](toloka.client.TolokaClient.find_app_batches.md) method.
 
+        Example:
+            >>> batches = toloka_client.get_app_batches(app_project_id = 'Q2d15QBjpwWuDz8Z321g', status = 'NEW')
+            >>> for batch in batches:
+            >>>     print(batch.id, batch.status, batch.items_count)
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             request: Search criteria.
             batch_size: Returned app batches limit for each request. The maximum allowed batch_size is 1000.
 
         Yields:
             AppBatch: The next matching batch.
@@ -5443,14 +5674,25 @@
     async def create_app_batch(
         self,
         app_project_id: str,
         request: toloka.client.app.AppBatchCreateRequest
     ) -> toloka.client.app.AppBatch:
         """Creates a batch with task items in an App project in Toloka.
 
+        Example:
+            The following example is suitable for a project
+            that requires `query` and `website_url` keys to be present in input data.
+
+            >>> new_items = [
+            >>>     {'id':'30', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'},
+            >>>     {'id':'31', 'query':'crowd kit', 'website_url':'https://toloka.ai/en/docs/crowd-kit'}
+            >>> ]
+            >>> toloka_client.create_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', items = new_items)
+            ...
+
         Args:
             app_project_id: The ID of the project.
             request: The request parameters.
 
         Returns:
             AppBatch: Created batch with updated parameters.
         """
@@ -5462,14 +5704,25 @@
         app_project_id: str,
         *,
         name: typing.Optional[str] = None,
         items: typing.Optional[typing.List[typing.Dict[str, typing.Any]]] = None
     ) -> toloka.client.app.AppBatch:
         """Creates a batch with task items in an App project in Toloka.
 
+        Example:
+            The following example is suitable for a project
+            that requires `query` and `website_url` keys to be present in input data.
+
+            >>> new_items = [
+            >>>     {'id':'30', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'},
+            >>>     {'id':'31', 'query':'crowd kit', 'website_url':'https://toloka.ai/en/docs/crowd-kit'}
+            >>> ]
+            >>> toloka_client.create_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', items = new_items)
+            ...
+
         Args:
             app_project_id: The ID of the project.
             request: The request parameters.
 
         Returns:
             AppBatch: Created batch with updated parameters.
         """
@@ -5478,14 +5731,19 @@
     async def get_app_batch(
         self,
         app_project_id: str,
         batch_id: str
     ) -> toloka.client.app.AppBatch:
         """Gets information from Toloka about a batch in an App project.
 
+        Example:
+            >>> batch = toloka_client.get_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', app_batch_id = '4Va2BBWKL88S4QyAgVje')
+            >>> print(batch.status, batch.items_count, batch.cost)
+            ...
+
         Args:
             app_project_id: The ID of the project.
             batch_id: The ID of the batch.
 
         Returns:
             AppBatch: The App batch.
         """
@@ -5494,81 +5752,109 @@
     @typing.overload
     async def patch_app_batch(
         self,
         app_project_id: str,
         batch_id: str,
         patch: toloka.client.app.AppBatchPatch
     ) -> toloka.client.app.AppBatch:
-        """Updates an App batch name.
+        """Updates an App batch.
 
         Args:
-            app_project_id: The ID of the project.
+            app_project_id: The ID of the App project containing the batch.
             batch_id: The ID of the batch.
-            patch: New name value.
+            patch: Parameters to update.
+
+        Example:
+            Changing the batch name.
+
+            >>> batch = toloka_client.patch_app_batch(
+            >>>     app_project_id = 'Q2d15QBjpwWuDz8Z321g', batch_id = '4Va2BBWKL88S4QyAgVje',
+            >>>     name = 'Preliminary batch')
+            ...
 
         Returns:
-            AppBatch: The App batch.
+            AppBatch: The updated App batch.
         """
         ...
 
     @typing.overload
     async def patch_app_batch(
         self,
         app_project_id: str,
         batch_id: str,
         *,
         name: typing.Optional[str] = None
     ) -> toloka.client.app.AppBatch:
-        """Updates an App batch name.
+        """Updates an App batch.
 
         Args:
-            app_project_id: The ID of the project.
+            app_project_id: The ID of the App project containing the batch.
             batch_id: The ID of the batch.
-            patch: New name value.
+            patch: Parameters to update.
+
+        Example:
+            Changing the batch name.
+
+            >>> batch = toloka_client.patch_app_batch(
+            >>>     app_project_id = 'Q2d15QBjpwWuDz8Z321g', batch_id = '4Va2BBWKL88S4QyAgVje',
+            >>>     name = 'Preliminary batch')
+            ...
 
         Returns:
-            AppBatch: The App batch.
+            AppBatch: The updated App batch.
         """
         ...
 
     async def start_app_batch(
         self,
         app_project_id: str,
         batch_id: str
     ):
         """Launches annotation of a batch of task items in an App project.
 
+        Example:
+            >>> toloka_client.start_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', app_batch_id = '4Va2BBWKL88S4QyAgVje')
+            ...
+
         Args:
             app_project_id: The ID of the project.
             batch_id: The ID of the batch.
         """
         ...
 
     async def stop_app_batch(
         self,
         app_project_id: str,
         batch_id: str
     ):
         """Stops annotation of a batch of task items in an App project.
 
-        Processing can be stopped only for the batch with the PROCESSING status.
+        Processing can be stopped only for the batch with the `PROCESSING` status.
+
+        Example:
+            >>> toloka_client.stop_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', batch_id = '4Va2BBWKL88S4QyAgVje')
+            ...
 
         Args:
             app_project_id: The ID of the project.
             batch_id: The ID of the batch.
         """
         ...
 
     async def resume_app_batch(
         self,
         app_project_id: str,
         batch_id: str
     ):
         """Resumes annotation of a batch of task items in an App project.
 
-        Processing can be resumed only for the batch with the STOPPING or STOPPED status.
+        Processing can be resumed only for the batch with the `STOPPING` or `STOPPED` status.
+
+        Example:
+            >>> toloka_client.resume_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', batch_id = '4Va2BBWKL88S4QyAgVje')
+            ...
 
         Args:
             app_project_id: The ID of the project.
             batch_id: The ID of the batch.
         """
         ...
```

### Comparing `toloka-kit-1.1.4/src/autoquality/optimizer.py` & `toloka-kit-1.2.0/src/autoquality/optimizer.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/autoquality/optimizer.pyi` & `toloka-kit-1.2.0/src/autoquality/optimizer.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/autoquality/scoring.py` & `toloka-kit-1.2.0/src/autoquality/scoring.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/autoquality/scoring.pyi` & `toloka-kit-1.2.0/src/autoquality/scoring.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/__init__.py` & `toloka-kit-1.2.0/src/client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     'Requester',
     'Skill',
     'SetUserSkillRequest',
     'TaskSuite',
     'Task',
     'Training',
     'UserBonus',
-    'UserBonusCreateRequestParameters',
     'UserRestriction',
     'UserSkill',
     'User',
     'Pool',
     'PoolPatchRequest',
     'Project',
     'AppProject',
@@ -72,33 +71,33 @@
 
 import datetime
 import functools
 import io
 import logging
 import threading
 import time
-import uuid
 
 import attr
 import httpx
 import simplejson
-from httpx import HTTPStatusError, RequestError
+from httpx import HTTPStatusError
 from httpx._types import VerifyTypes
+from toloka.client.batch_create_results import FieldValidationError
 
 try:
     import pandas as pd
     PANDAS_INSTALLED = True
 except ImportError:
     PANDAS_INSTALLED = False
 
 from decimal import Decimal
 from enum import Enum, unique
 from tqdm import tqdm
 from tqdm.contrib.logging import logging_redirect_tqdm
-from typing import BinaryIO, Callable, ClassVar, Generator, List, Optional, Sequence, Tuple, Union
+from typing import BinaryIO, Callable, ClassVar, Dict, Generator, List, Optional, Sequence, Tuple, Union
 from urllib3.util.retry import Retry
 
 from . import actions
 from . import aggregation
 from . import analytics_request
 from . import app
 from . import assignment
@@ -147,21 +146,22 @@
 from .message_thread import (
     Folder, MessageThread, MessageThreadReply, MessageThreadFolders, MessageThreadCompose
 )
 from .operation_log import OperationLogItem
 from .pool import Pool, PoolPatchRequest
 from .primitives.retry import TolokaRetry, SyncRetryingOverURLLibRetry, STATUSES_TO_RETRY
 from .primitives.base import autocast_to_enum
+from .primitives.parameter import IdempotentOperationParameters
 from .project import Project
 from .training import Training
 from .requester import Requester
 from .skill import Skill
 from .task import Task
 from .task_suite import TaskSuite
-from .user_bonus import UserBonus, UserBonusCreateRequestParameters
+from .user_bonus import UserBonus
 from .user_restriction import UserRestriction
 from .user_skill import SetUserSkillRequest, UserSkill
 from .user import User
 from ..util import identity
 from ..util._managing_headers import add_headers, form_additional_headers, top_level_method_var
 from ..util._codegen import expand
 from .webhook_subscription import WebhookSubscription
@@ -251,15 +251,15 @@
         def platform_url(self):
             if self is TolokaClient.Environment.PRODUCTION:
                 return 'https://platform.toloka.ai'
             if self is TolokaClient.Environment.SANDBOX:
                 return 'https://sandbox.toloka.yandex.com'
 
     EXCEPTIONS_TO_RETRY: ClassVar[Tuple[Exception]] = (
-        RequestError, InternalApiError, TooManyRequestsApiError, RemoteServiceUnavailableApiError, HTTPStatusError,
+        InternalApiError, TooManyRequestsApiError, RemoteServiceUnavailableApiError, HTTPStatusError,
     )
 
     token: str
     default_timeout: Union[float, Tuple[float, float]]
     _platform_url: Optional[str]
     url: Optional[str]
     retryer_factory: Optional[Callable[[], Retry]]
@@ -322,28 +322,34 @@
             retry_quotas=retry_quotas,
             total=retries,
             status_forcelist=list(status_list or STATUSES_TO_RETRY),
             allowed_methods=['HEAD', 'GET', 'PUT', 'DELETE', 'OPTIONS', 'TRACE', 'POST', 'PATCH'],
             backoff_factor=2,  # summary retry time more than 10 seconds
         )
 
+    def __is_apikey(self) -> bool:
+        if self.token.count('.') != 2:
+            return False
+        dot_pos = self.token.find('.')
+        return 21 < dot_pos < 25
+
     @property
     def _headers(self):
         headers = {
-            'Authorization': f'OAuth {self.token}',
+            'Authorization': f'ApiKey {self.token}' if self.__is_apikey() else 'OAuth {self.token}',
             'User-Agent': f'python-toloka-client-{__version__}',
         }
         if self.act_under_account_id:
             headers['X-Act-Under-Account-ID'] = self.act_under_account_id
         return headers
 
     def _do_request_with_retries(self, method, path, **kwargs):
         @self.retrying.wraps
-        def wrapped(method, path, **kwargs):
-            response = self._session.request(method, path, **kwargs)
+        def wrapped(method, url, **kwargs):
+            response = self._session.request(method, url, **kwargs)
             raise_on_api_error(response)
             return response
 
         return wrapped(method, path, **kwargs)
 
     @property
     def _session(self):
@@ -398,96 +404,172 @@
             request = attr.evolve(request, **{f'{sort_field}_gt': getattr(items[-1], sort_field)})
             yield from items
             result = find_function(request, sort=[sort_field], limit=batch_size)
             items = getattr(result, items_field)
 
         yield from items
 
-    def _try_to_async_create_objects(self, url, objects, parameters, operation_type):
+    def _async_create_objects_idempotent(
+        self,
+        url,
+        objects,
+        parameters,
+        operation_type,
+    ):
         try:
             response = self._request('post', url, json=unstructure(objects), params=unstructure(parameters))
             insert_operation = structure(response, operation_type)
         except IncorrectActionsApiError as exc:
             if exc.code != 'OPERATION_ALREADY_EXISTS':
                 raise
 
             insert_operation = self.get_operation(operation_id=str(parameters.operation_id))
             if not isinstance(insert_operation, operation_type):
                 raise
+            insert_operation.raise_on_fail()
             logger.info(f'Objects were not created by {top_level_method_var.get()}: '
                         f'operation {parameters.operation_id} is already submitted.')
         return insert_operation
 
-    def _sync_via_async(self, objects, parameters, url, result_type, operation_type, output_id_field, get_method):
+    def _start_sync_via_async(
+        self,
+        objects,
+        parameters: IdempotentOperationParameters,
+        url: str,
+        operation_type: operations.Operation,
+    ):
+        # Index objects to restore sequence in the future
+        is_single = not isinstance(objects, list)
+        if is_single:
+            objects._unexpected['__item_idx'] = '0'
+        else:
+            for item_idx, obj in enumerate(objects):
+                obj._unexpected['__item_idx'] = str(item_idx)
+
+        insert_operation = self._async_create_objects_idempotent(url, objects, parameters, operation_type)
+        insert_operation = self.wait_operation(insert_operation, datetime.timedelta(minutes=60))
+        return insert_operation
+
+    def _sync_via_async_pool_related(
+            self,
+            objects,
+            parameters: IdempotentOperationParameters,
+            url: str,
+            result_type,
+            operation_type: operations.Operation,
+            output_id_field: str,
+            get_method: Callable,
+    ):
         if not parameters.async_mode:
             response = self._request('post', url, json=unstructure(objects), params=unstructure(parameters))
             return structure(response, result_type)
-
-        # Emulates synchronous operation, through asynchronous calls and reading operation logs.
-        client_uuid_to_index = {}
-        for i, obj in enumerate(objects):
-            obj._unexpected['__client_uuid'] = uuid.uuid4().hex
-            client_uuid_to_index[obj._unexpected['__client_uuid']] = str(i)
-
-        insert_operation = self._try_to_async_create_objects(url, objects, parameters, operation_type)
-        insert_operation = self.wait_operation(insert_operation, datetime.timedelta(minutes=60))
+        is_single = not isinstance(objects, list)
+        insert_operation = self._start_sync_via_async(objects, parameters, url, operation_type)
 
         pools = {}
         validation_errors = {}
-
         for log_item in self.get_operation_log(insert_operation.id):
-            if log_item.type not in ['TASK_CREATE', 'TASK_VALIDATE', 'TASK_SUITE_VALIDATE', 'TASK_SUITE_CREATE']:
-                continue
-            if '__client_uuid' in log_item.input and log_item.input['__client_uuid'] in client_uuid_to_index:
-                index = client_uuid_to_index[log_item.input['__client_uuid']]
+            if '__item_idx' in log_item.input:
+                index = log_item.input['__item_idx']
             else:
-                continue
+                continue  # operation could be not just creating objects (e.g. open_pool while creating_object)
             if log_item.success:
                 numerated_ids = pools.setdefault(log_item.input['pool_id'], {})
                 numerated_ids[log_item.output[output_id_field]] = index
             else:
-                validation_errors[index] = {
-                    name: structure(error, batch_create_results.FieldValidationError)
-                    for name, error in log_item.output.items()
-                }
-
-        # Emulates the response as in a synchronous method:
-        # it will throw an exception even if the skip_invalid_items parameter is passed
-        # but no objects are created
-        if not pools:
+                validation_errors[index] = structure(log_item.output, Dict[str, FieldValidationError])
+
+        # Like in sync methods Exception will raise
+        # even if the skip_invalid_items=True but no objects are created
+        if validation_errors and not pools:
             raise ValidationApiError(
                 code='VALIDATION_ERROR',
                 message='Validation failed',
-                payload=validation_errors
+                payload=validation_errors,
             )
 
-        # get object from all pools
-        items = self._collect_from_pools(get_method, pools)
-        return result_type(items=items, validation_errors=validation_errors or {})
+        if is_single:
+            pool_id = list(pools.keys())[0]
+            item_id = list(pools[pool_id].keys())[0]
+            return get_method(item_id)
+        else:
+            items = self._collect_from_pools(get_method, pools)
+            return result_type(items=items, validation_errors=validation_errors)
 
     def _collect_from_pools(self, get_method, pools):
         items = {}
         for pool_id, numerated_ids in pools.items():
             obj_it = get_method(
                 pool_id=pool_id,
                 id_gte=min(numerated_ids.keys()),
                 id_lte=max(numerated_ids.keys()),
             )
             for obj in obj_it:
                 if obj.id in numerated_ids:
                     items[numerated_ids[obj.id]] = obj
         return items
 
+    def _sync_via_async(
+            self,
+            objects: List,
+            parameters: IdempotentOperationParameters,
+            url: str,
+            result_type,
+            operation_type: operations.Operation,
+            output_id_field: str,
+            get_method: Callable,
+    ):
+        if not parameters.async_mode:
+            response = self._request('post', url, json=unstructure(objects), params=unstructure(parameters))
+            return structure(response, result_type)
+        is_single = not isinstance(objects, list)
+        insert_operation = self._start_sync_via_async(objects, parameters, url, operation_type)
+
+        item_id_to_idx = {}
+        validation_errors = {}
+        for log_item in self.get_operation_log(insert_operation.id):
+            if '__item_idx' in log_item.input:
+                index = log_item.input['__item_idx']
+            else:
+                continue  # operation could be not just creating objects (e.g. open_pool while creating_object)
+            if log_item.success:
+                item_id_to_idx[log_item.output[output_id_field]] = index
+            else:
+                validation_errors[index] = log_item.output
+
+        # Like as in sync methods Exception will raise
+        # even if the skip_invalid_items=True but no objects are created
+        if validation_errors and not item_id_to_idx:
+            raise ValidationApiError(
+                code='VALIDATION_ERROR',
+                message='Validation failed',
+                payload=validation_errors,
+            )
+
+        if is_single:
+            item_id = list(item_id_to_idx.keys())[0]
+            return get_method(item_id)
+        else:
+            items = {}
+            obj_it = get_method(
+                id_gte=min(item_id_to_idx.keys()),
+                id_lte=max(item_id_to_idx.keys()),
+            )
+            for obj in obj_it:
+                if obj.id in item_id_to_idx:
+                    items[item_id_to_idx[obj.id]] = obj
+            return result_type(items=items, validation_errors=validation_errors)
+
     # Aggregation section
 
     @expand('request')
     @add_headers('client')
     def aggregate_solutions_by_pool(
         self,
-        request: aggregation.PoolAggregatedSolutionRequest
+        request: aggregation.PoolAggregatedSolutionRequest,
     ) -> operations.AggregatedSolutionOperation:
         """Starts aggregation of responses in all completed tasks in a pool.
 
         The method starts the aggregation process on the Toloka server. To wait for the completion of the operation use the [wait_operation](toloka.client.TolokaClient.wait_operation.md) method.
 
         {% note tip %}
 
@@ -879,49 +961,48 @@
 
     @autocast_to_enum
     @add_headers('client')
     def add_message_thread_to_folders(
         self,
         message_thread_id: str, folders: Union[List[Folder], MessageThreadFolders]
     ) -> MessageThread:
-        """Adds a message chain to one or more folders ("unread", "important" etc.)
+        """Adds a message thread to folders.
 
         Args:
-            message_thread_id: ID of message chain.
-            folders: List of folders, where to move chain.
+            message_thread_id: The ID of the message thread.
+            folders: A list of folders where to add the thread.
 
         Returns:
-            MessageThread: Full object by ID with updated folders.
+            MessageThread: The updated message thread.
 
         Example:
             >>> toloka_client.add_message_thread_to_folders(message_thread_id='1', folders=['IMPORTANT'])
             ...
         """
         if not isinstance(folders, MessageThreadFolders):
             folders = structure({'folders': folders}, MessageThreadFolders)
         response = self._request('post', f'/v1/message-threads/{message_thread_id}/add-to-folders', json=unstructure(folders))
         return structure(response, MessageThread)
 
     @expand('compose')
     @add_headers('client')
     def compose_message_thread(self, compose: MessageThreadCompose) -> MessageThread:
-        """Sends a message to a Toloker.
-
-        The sent message is added to a new message thread.
+        """Creates a message thread and sends the first thread message to Tolokers.
 
         Args:
-            compose: Message parameters.
+            compose: Parameters for creating the message thread.
 
         Returns:
-            MessageThread: New created thread.
+            MessageThread: The created message thread.
 
         Example:
-            If you want to thank Tolokers who have tried to complete your tasks, send them a nice message.
+            A message is sent to all Tolokers who have tried to complete your tasks.
+            The message is in english. Tolokers can't reply to your message.
 
-            >>> message_text = "Amazing job! We've just trained our first model with the data YOU prepared for us. Thank you!"
+            >>> message_text = "Amazing job! We've just trained our first model with the data you prepared for us. Thank you!"
             >>> toloka_client.compose_message_thread(
             >>>     recipients_select_type='ALL',
             >>>     topic={'EN': 'Thank you!'},
             >>>     text={'EN': message_text},
             >>>     answerable=False
             >>> )
             ...
@@ -945,41 +1026,43 @@
             sort: Sorting options. Default: `None`.
             limit: Returned message threads limit. The default limit is 50. The maximum allowed limit is 300.
 
         Returns:
             MessageThreadSearchResult: Found message threads and a flag showing whether there are more matching threads.
 
         Example:
-            Find all message threads in the Inbox folder.
+            Finding all message threads in the `INBOX` folder.
 
             >>> toloka_client.find_message_threads(folder='INBOX')
             ...
         """
         sort = None if sort is None else structure(sort, search_requests.MessageThreadSortItems)
         response = self._search_request('get', '/v1/message-threads', request, sort, limit)
         return structure(response, search_results.MessageThreadSearchResult)
 
     @add_headers('client')
     def reply_message_thread(self, message_thread_id: str, reply: MessageThreadReply) -> MessageThread:
-        """Replies to a message in thread
+        """Sends a reply message in a thread.
 
         Args:
-            message_thread_id: In which thread to reply.
-            reply: Reply message.
+            message_thread_id: The ID of the thread.
+            reply: The reply message.
 
         Returns:
-            MessageThread: New created message.
+            MessageThread: The updated message thread.
 
         Example:
+            Sending a reply to all unread messages.
+
             >>> message_threads = toloka_client.get_message_threads(folder='UNREAD')
             >>> message_reply = {'EN': 'Thank you for your message! I will get back to you soon.'}
             >>> for thread in message_threads:
             >>>     toloka_client.reply_message_thread(
             >>>         message_thread_id=thread.id,
-            >>>         reply=toloka.message_thread.MessageThreadReply(text=message_reply)
+            >>>         reply=toloka.client.message_thread.MessageThreadReply(text=message_reply)
             >>>     )
             ...
         """
         response = self._request('post', f'/v1/message-threads/{message_thread_id}/reply', json=unstructure(reply))
         return structure(response, MessageThread)
 
     @expand('request')
@@ -1011,22 +1094,22 @@
         generator = self._find_all(self.find_message_threads, request, batch_size=batch_size)
         yield from generator
 
     @autocast_to_enum
     @add_headers('client')
     def remove_message_thread_from_folders(self, message_thread_id: str,
                                            folders: Union[List[Folder], MessageThreadFolders]) -> MessageThread:
-        """Deletes a message chain from one or more folders ("unread", "important" etc.)
+        """Removes a message thread from folders.
 
         Args:
-            message_thread_id: ID of message chain.
-            folders:  List of folders, where from to remove chain.
+            message_thread_id: The ID of the message thread.
+            folders: A list of folders.
 
         Returns:
-            MessageThread: Full object by ID with updated folders.
+            MessageThread: The updated message thread.
 
         Example:
             >>> toloka_client.remove_message_thread_from_folders(message_thread_id='1', folders=['IMPORTANT'])
             ...
         """
         if not isinstance(folders, MessageThreadFolders):
             folders = structure({'folders': folders}, MessageThreadFolders)
@@ -2191,39 +2274,39 @@
         """
         response = self._request('put', f'/v1/skills/{skill_id}', json=unstructure(skill))
         return structure(response, Skill)
 
     # Statistics section
 
     @add_headers('client')
-    def get_analytics(self, stats: List[AnalyticsRequest]) -> operations.Operation:
-        """Sends analytics queries, for example, to estimate the percentage of completed tasks in the pool
+    def get_analytics(self, stats: List[AnalyticsRequest]) -> operations.AnalyticsOperation:
+        """Sends analytics requests to Toloka.
 
-        Only pool analytics queries are available.
-        The values of different analytical metrics will be returned in the "details" field of the operation when it is
-        completed. See the example.
         You can request up to 10 metrics at a time.
 
+        The values of different analytical metrics are returned in the `details` field of the operation when it is completed.
+
         Args:
-            stats: Analytics queries list.
+            stats: A list of analytics requests.
 
         Returns:
-            operations.Operation: An operation that you can wait for to get the required statistics.
+            operations.AnalyticsOperation: An object to track the progress of the operation.
 
         Example:
-            How to get task completion percentage for one pool.
+            The example shows how get the percentage of completed tasks in the pool.
 
             >>> from toloka.client.analytics_request import CompletionPercentagePoolAnalytics
-            >>> operation = toloka_client.get_analytics([CompletionPercentagePoolAnalytics(subject_id=pool_id)])
+            >>> operation = toloka_client.get_analytics([CompletionPercentagePoolAnalytics(subject_id='1080020')])
             >>> operation = toloka_client.wait_operation(operation)
-            >>> print(operation.details['value'][0]['result']['value'])
+            >>> print(operation.details['value'][0])
+            >>> completed_task_percentage = operation.details['value'][0]['result']['value']
             ...
         """
         response = self._request('post', '/staging/analytics-2', json=unstructure(stats))
-        return structure(response, operations.Operation)
+        return structure(response, operations.AnalyticsOperation)
 
     # Task section
 
     @expand('parameters')
     @add_headers('client')
     def create_task(self, task: Task, parameters: Optional[task.CreateTaskParameters] = None) -> Task:
         """Creates a new task in Toloka.
@@ -2244,16 +2327,23 @@
             >>> task = toloka.client.Task(
             >>>     input_values={'image': 'https://tlk.s3.yandex.net/dataset/cats_vs_dogs/dogs/048e5760fc5a46faa434922b2447a527.jpg'},
             >>>     pool_id='1'
             >>> )
             >>> toloka_client.create_task(task=task, allow_defaults=True)
             ...
         """
-        response = self._request('post', '/v1/tasks', json=unstructure(task), params=unstructure(parameters))
-        return structure(response, Task)
+        return self._sync_via_async(
+            objects=task,
+            parameters=parameters,
+            url='/v1/tasks',
+            result_type=Task,
+            operation_type=operations.TasksCreateOperation,
+            output_id_field='task_id',
+            get_method=self.get_task,
+        )
 
     @expand('parameters')
     @add_headers('client')
     def create_tasks(
         self,
         tasks: List[Task], parameters: Optional[task.CreateTasksParameters] = None
     ) -> batch_create_results.TaskBatchCreateResult:
@@ -2304,24 +2394,22 @@
             >>>             pool_id = existing_pool_id,
             >>>         )
             >>>     )
             >>> result = toloka_client.create_tasks(golden_tasks, allow_defaults=True)
             >>> print(len(result.items))
             ...
         """
-        if not parameters:
-            parameters = task.CreateTasksParameters()
-        return self._sync_via_async(
+        return self._sync_via_async_pool_related(
             objects=tasks,
             parameters=parameters,
             url='/v1/tasks',
             result_type=batch_create_results.TaskBatchCreateResult,
             operation_type=operations.TasksCreateOperation,
             output_id_field='task_id',
-            get_method=self.get_tasks
+            get_method=self.get_tasks,
         )
 
     @expand('parameters')
     @add_headers('client')
     def create_tasks_async(self, tasks: List[Task],
                            parameters: Optional[task.CreateTasksParameters] = None) -> operations.TasksCreateOperation:
         """Creates tasks in Toloka asynchronously.
@@ -2345,15 +2433,15 @@
             >>> tasks_op = toloka_client.create_tasks_async(training_tasks)
             >>> toloka_client.wait_operation(tasks_op)
             ...
         """
         if not parameters.async_mode:
             logger.warning('async_mode=False ignored in TolokaClient.create_tasks_async')
         parameters.async_mode = True
-        return self._try_to_async_create_objects('/v1/tasks', tasks, parameters, operations.TasksCreateOperation)
+        return self._async_create_objects_idempotent('/v1/tasks', tasks, parameters, operations.TasksCreateOperation)
 
     @expand('request')
     @add_headers('client')
     def find_tasks(self, request: search_requests.TaskSearchRequest,
                    sort: Union[List[str], search_requests.TaskSortItems, None] = None,
                    limit: Optional[int] = None) -> search_results.TaskSearchResult:
         """Finds tasks that match certain criteria.
@@ -2497,23 +2585,29 @@
             >>>     pool_id='1',
             >>>     tasks=[toloka.client.Task(input_values={'label': 'Cats vs Dogs'})],
             >>>     overlap=2
             >>> )
             >>> toloka_client.create_task_suite(new_task_suite)
             ...
         """
-        params = {**(unstructure(parameters) or {}), 'async_mode': False}
-        response = self._request('post', '/v1/task-suites', json=unstructure(task_suite), params=unstructure(params))
-        return structure(response, TaskSuite)
+        return self._sync_via_async(
+            objects=task_suite,
+            parameters=parameters,
+            url='/v1/task-suites',
+            result_type=TaskSuite,
+            operation_type=operations.TaskSuiteCreateBatchOperation,
+            output_id_field='task_suite_id',
+            get_method=self.get_task_suite,
+        )
 
     @expand('parameters')
     @add_headers('client')
     def create_task_suites(
         self,
-        task_suites: List[TaskSuite], parameters: Optional[task_suite.TaskSuiteCreateRequestParameters] = None
+        task_suites: List[TaskSuite], parameters: Optional[task_suite.TaskSuitesCreateRequestParameters] = None
     ) -> batch_create_results.TaskSuiteBatchCreateResult:
         """Creates several task suites in Toloka.
 
         Usually, you don't need to create a task suite manually, because Toloka can group tasks into suites automatically.
 
         Use this method if you need to group specific tasks together or to set different parameters in different task suites.
         Task suites can be created in different pools. You can create general and control tasks or task suites in different pools with a single method call.
@@ -2547,31 +2641,29 @@
             >>>             })
             >>>         ]
             >>>     )
             >>> ]
             >>> task_suites = toloka_client.create_task_suites(task_suites)
             ...
         """
-        if not parameters:
-            parameters = task_suite.TaskSuiteCreateRequestParameters()
-        return self._sync_via_async(
+        return self._sync_via_async_pool_related(
             objects=task_suites,
             parameters=parameters,
             url='/v1/task-suites',
             result_type=batch_create_results.TaskSuiteBatchCreateResult,
             operation_type=operations.TaskSuiteCreateBatchOperation,
             output_id_field='task_suite_id',
-            get_method=self.get_task_suites
+            get_method=self.get_task_suites,
         )
 
     @expand('parameters')
     @add_headers('client')
     def create_task_suites_async(
         self,
-        task_suites: List[TaskSuite], parameters: Optional[task_suite.TaskSuiteCreateRequestParameters] = None
+        task_suites: List[TaskSuite], parameters: Optional[task_suite.TaskSuitesCreateRequestParameters] = None
     ) -> operations.TaskSuiteCreateBatchOperation:
         """Creates several task suites in Toloka asynchronously.
 
         You can send a maximum of 100,000 requests of this kind per minute and 2,000,000 requests per day.
         It is recommended that you create no more than 10,000 task suites in a single request.
 
         See also the [create_task_suites](toloka.client.TolokaClient.create_task_suites.md) method.
@@ -2598,15 +2690,15 @@
             >>> task_suites_op = toloka_client.create_task_suites_async(task_suites)
             >>> toloka_client.wait_operation(task_suites_op)
             ...
         """
         if not parameters.async_mode:
             logger.warning('async_mode=False ignored in TolokaClient.create_task_suites_async')
         parameters.async_mode = True
-        return self._try_to_async_create_objects(
+        return self._async_create_objects_idempotent(
             '/v1/task-suites', task_suites, parameters, operations.TaskSuiteCreateBatchOperation
         )
 
     @expand('request')
     @add_headers('client')
     def find_task_suites(
         self, request: search_requests.TaskSuiteSearchRequest,
@@ -2846,15 +2938,15 @@
     def get_operations(
         self,
         request: search_requests.OperationSearchRequest,
         batch_size: Optional[int] = None
     ) -> Generator[operations.Operation, None, None]:
         """Finds all operations that match certain rules and returns them in an iterable object
 
-       `get_operations` returns a generator. You can iterate over all found operations using the generator. Several requests to the Toloka server are possible while iterating.
+        `get_operations` returns a generator. You can iterate over all found operations using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort operations use the [find_operations](toloka.client.TolokaClient.find_operations.md) method.
 
         Args:
             request: Search criteria.
             batch_size: Returned operations limit for each request. The default batch_size is 50. The maximum allowed batch_size is 500.
 
@@ -2891,15 +2983,15 @@
 
     # User bonus
 
     @expand('parameters')
     @add_headers('client')
     def create_user_bonus(
         self,
-        user_bonus: UserBonus, parameters: Optional[UserBonusCreateRequestParameters] = None
+        user_bonus: UserBonus, parameters: Optional[user_bonus.UserBonusCreateRequestParameters] = None
     ) -> UserBonus:
         """Issues payments directly to a Toloker.
 
         You can send a maximum of 10,000 requests of this kind per day.
 
         Args:
             user_bonus: To whom, how much to pay and for what.
@@ -2925,25 +3017,29 @@
             >>>             'RU': 'Молодец!',
             >>>         },
             >>>         assignment_id='012345'
             >>>     )
             >>> )
             ...
         """
-        response = self._request(
-            'post', '/v1/user-bonuses', json=unstructure(user_bonus),
-            params=({} if parameters is None else unstructure(parameters))
+        return self._sync_via_async(
+            objects=user_bonus,
+            parameters=parameters,
+            url='/v1/user-bonuses',
+            result_type=UserBonus,
+            operation_type=operations.UserBonusCreateBatchOperation,
+            output_id_field='user_bonus_id',
+            get_method=self.get_user_bonus,
         )
-        return structure(response, UserBonus)
 
     @expand('parameters')
     @add_headers('client')
     def create_user_bonuses(
         self,
-        user_bonuses: List[UserBonus], parameters: Optional[UserBonusCreateRequestParameters] = None
+        user_bonuses: List[UserBonus], parameters: Optional[user_bonus.UserBonusesCreateRequestParameters] = None
     ) -> batch_create_results.UserBonusBatchCreateResult:
         """Creates rewards for Tolokers.
 
         Right now it's safer to use asynchronous version: "create_user_bonuses_async"
         You can send a maximum of 10,000 requests of this kind per day.
 
         Args:
@@ -2983,24 +3079,28 @@
             >>>         },
             >>>         assignment_id='2'
             >>>     )
             >>> ]
             >>> toloka_client.create_user_bonuses(new_bonuses)
             ...
         """
-        response = self._request(
-            'post', '/v1/user-bonuses', json=unstructure(user_bonuses),
-            params=({} if parameters is None else unstructure(parameters))
+        return self._sync_via_async(
+            objects=user_bonuses,
+            parameters=parameters,
+            url='/v1/user-bonuses',
+            result_type=batch_create_results.UserBonusBatchCreateResult,
+            operation_type=operations.UserBonusCreateBatchOperation,
+            output_id_field='user_bonus_id',
+            get_method=self.get_user_bonuses,
         )
-        return structure(response, batch_create_results.UserBonusBatchCreateResult)
 
     @expand('parameters')
     @add_headers('client')
     def create_user_bonuses_async(
-        self, user_bonuses: List[UserBonus], parameters: Optional[UserBonusCreateRequestParameters] = None
+        self, user_bonuses: List[UserBonus], parameters: Optional[user_bonus.UserBonusesCreateRequestParameters] = None
     ) -> operations.UserBonusCreateBatchOperation:
         """Issues payments directly to Tolokers, asynchronously creates many `UserBonus` instances.
 
         You can send a maximum of 10,000 requests of this kind per day.
 
         Args:
             user_bonuses: To whom, how much to pay and for what.
@@ -3042,15 +3142,15 @@
             >>> create_bonuses = toloka_client.create_user_bonuses_async(new_bonuses)
             >>> toloka_client.wait_operation(create_bonuses)
             ...
         """
         if not parameters.async_mode:
             logger.warning('async_mode=False ignored in TolokaClient.create_user_bonuses_async')
         parameters.async_mode = True
-        return self._try_to_async_create_objects(
+        return self._async_create_objects_idempotent(
             '/v1/user-bonuses', user_bonuses, parameters, operations.UserBonusCreateBatchOperation
         )
 
     @expand('request')
     @add_headers('client')
     def find_user_bonuses(self, request: search_requests.UserBonusSearchRequest,
                           sort: Union[List[str], search_requests.UserBonusSortItems, None] = None,
@@ -3099,15 +3199,15 @@
     def get_user_bonuses(
         self,
         request: search_requests.UserBonusSearchRequest,
         batch_size: Optional[int] = None
     ) -> Generator[UserBonus, None, None]:
         """Finds all Tolokers' rewards that match certain rules and returns them in an iterable object
 
-       `get_user_bonuses` returns a generator. You can iterate over all found Tolokers' rewards using the generator. Several requests to the Toloka server are possible while iterating.
+        `get_user_bonuses` returns a generator. You can iterate over all found Tolokers' rewards using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort rewards use the [find_user_bonuses](toloka.client.TolokaClient.find_user_bonuses.md) method.
 
         Args:
             request: Search criteria.
             batch_size: Returned Tolokers' rewards limit for each request. The maximum allowed batch_size is 300.
 
@@ -3387,25 +3487,24 @@
         self._raw_request('delete', f'/v1/user-skills/{user_skill_id}')
 
     @add_headers('client')
     def upsert_webhook_subscriptions(
         self,
         subscriptions: List[WebhookSubscription]
     ) -> batch_create_results.WebhookSubscriptionBatchCreateResult:
-        """Creates (upsert) many webhook-subscriptions.
+        """Creates (upsert) webhook subscriptions.
 
         Args:
-            subscriptions: List of webhook-subscriptions, that will be created.
+            subscriptions: A list of webhook subscriptions to be created.
 
         Returns:
-            batch_create_results.WebhookSubscriptionBatchCreateResult: Result of subscriptions creation.
-                Contains created subscriptions in `items` and problems in "validation_errors".
+            batch_create_results.WebhookSubscriptionBatchCreateResult: The result of the operation.
 
         Raises:
-            ValidationApiError: If no subscriptions were created.
+            ValidationApiError: No subscriptions were created.
 
         Example:
             How to create several subscriptions.
 
             >>> created_result = toloka_client.upsert_webhook_subscriptions([
             >>>     {
             >>>         'webhook_url': 'https://awesome-requester.com/toloka-webhook',
@@ -3555,14 +3654,26 @@
                           limit: Optional[int] = None) -> search_results.AppProjectSearchResult:
         """Finds App projects that match certain criteria.
 
         The number of returned projects is limited. To find remaining projects call `find_app_projects` with updated search criteria.
 
         To iterate over all matching projects you may use the [get_app_projects](toloka.client.TolokaClient.get_app_projects.md) method.
 
+        Example:
+            Searching active projects based on the App solution with the specified ID.
+
+            >>> search = toloka_client.find_app_projects(
+            >>>     app_id = '9lZaMl363jahzra1rrYq', status = 'READY')
+            >>> for app_project in search.content:
+            >>>     print(app_project.id, app_project.name)
+            >>>
+            >>> if search.has_more:
+            >>>     print('There are more App projects...')
+            ...
+
         Args:
             request: Search criteria.
             sort: The order and direction of sorting the results.
             limit: Returned projects limit. The maximum limit is 5000.
 
         Returns:
             AppProjectSearchResult: Found projects and a flag showing whether there are more matching projects exceeding the limit.
@@ -3584,14 +3695,20 @@
     ) -> Generator[AppProject, None, None]:
         """Finds all App projects that match certain criteria.
 
         `get_app_projects` returns a generator. You can iterate over all found projects using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort App projects use the [find_app_projects](toloka.client.TolokaClient.find_app_projects.md) method.
 
+        Example:
+            >>> app_projects = toloka_client.get_app_projects(scope='MY')
+            >>> for app_project in app_projects:
+            >>>     print(app_project.id, app_project.status, app_project.name)
+            ...
+
         Args:
             request: Search criteria.
             batch_size: Returned projects limit for each request. The maximum batch_size is 5000.
 
         Yields:
             AppProject: The next matching App project.
         """
@@ -3602,14 +3719,53 @@
         generator = self._find_all(self.find_app_projects, request, items_field='content', batch_size=batch_size)
         yield from generator
 
     @add_headers('client')
     def create_app_project(self, app_project: AppProject) -> AppProject:
         """Creates an App project in Toloka.
 
+        Example:
+            >>> app_project = toloka.AppProject(
+            >>>   app_id='9lZaMl363jahzra1rrYq',
+            >>>   name='Example project (product relevance)',
+            >>>   parameters={
+            >>>     "default_language": "en",
+            >>>     "name": "Product relevance project",
+            >>>     "instruction_classes": [
+            >>>       {
+            >>>         "description": "The product is relevant to the query.",
+            >>>         "label": "Relevant",
+            >>>         "value": "relevant"
+            >>>       },
+            >>>       {
+            >>>         "description": "The product is not completely relevant to the query.",
+            >>>         "label": "Irrelevant",
+            >>>         "value": "irrelevant"
+            >>>       }
+            >>>     ],
+            >>>     "instruction_examples": [
+            >>>       {
+            >>>         "description": "The product exactly matches the query.",
+            >>>         "label": "relevant",
+            >>>         "query": "some search query",
+            >>>         "screenshot_url": "https://example.com/1"
+            >>>       },
+            >>>       {
+            >>>         "description": "The product shape matches but the product color does not.",
+            >>>         "label": "irrelevant",
+            >>>         "query": "other search query",
+            >>>         "screenshot_url": "https://example.com/2"
+            >>>       }
+            >>>     ]
+            >>>   }
+            >>> )
+            >>> app_project = toloka_client.create_app_project(app_project)
+            >>> print(app_project.created, app_project.status)
+            ...
+
         Args:
             app_project: The project with parameters.
 
         Returns:
             AppProject: Created App project with updated parameters.
         """
 
@@ -3619,14 +3775,19 @@
         response = self._request('post', '/app/v0/app-projects', json=unstructure(app_project))
         return structure(response, AppProject)
 
     @add_headers('client')
     def get_app_project(self, app_project_id: str) -> AppProject:
         """Gets information from Toloka about an App project.
 
+        Example:
+            >>> app_project = toloka_client.get_app_project('Q2d15QBjpwWuDz8Z321g')
+            >>> print(app_project.created, app_project.name)
+            ...
+
         Args:
             app_project_id: The ID of the project.
 
         Returns:
             AppProject: The App project.
         """
 
@@ -3638,14 +3799,18 @@
 
     @add_headers('client')
     def archive_app_project(self, app_project_id: str) -> AppProject:
         """Archives an App project.
 
         The project changes its status to `ARCHIVED`.
 
+        Example:
+            >>> toloka_client.archive_app_project('Q2d15QBjpwWuDz8Z321g')
+            ...
+
         Args:
             app_project_id: The ID of the project.
 
         Returns:
             AppProject: The App project with updated status.
         """
 
@@ -3657,14 +3822,18 @@
 
     @add_headers('client')
     def unarchive_app_project(self, app_project_id: str) -> AppProject:
         """Unarchives an App project.
 
         Previous project status, which was before archiving, is restored.
 
+        Example:
+            >>> toloka_client.unarchive_app_project('Q2d15QBjpwWuDz8Z321g')
+            ...
+
         Args:
             app_project_id: The ID of the project.
 
         Returns:
             AppProject: The App project with updated status.
         """
 
@@ -3683,14 +3852,23 @@
     ) -> search_results.AppSearchResult:
         """Finds App solutions that match certain criteria.
 
         The number of returned solutions is limited. To find remaining solutions call `find_apps` with updated search criteria.
 
         To iterate over all matching solutions you may use the [get_apps](toloka.client.TolokaClient.get_apps.md) method.
 
+        Example:
+            >>> search = toloka_client.find_apps()
+            >>> for app in search.content:
+            >>>     print(app.id, app.name)
+            >>>
+            >>> if search.has_more:
+            >>>     print('There are more App solutions...')
+            ...
+
         Args:
             request: Search criteria.
             sort: Sorting options. Default: `None`.
             limit: Returned solutions limit. The maximum allowed limit is 1000.
 
         Returns:
             AppSearchResult: Found solutions and a flag showing whether there are more matching solutions exceeding the limit.
@@ -3712,14 +3890,20 @@
     ) -> Generator[App, None, None]:
         """Finds all App solutions that match certain criteria.
 
         `get_apps` returns a generator. You can iterate over all found solutions using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort solutions use the [find_apps](toloka.client.TolokaClient.find_apps.md) method.
 
+        Example:
+            >>> apps = toloka_client.get_apps()
+            >>> for app in apps:
+            >>>     print(app.id, app.name)
+            ...
+
         Args:
             request: Search criteria.
             batch_size: Returned solutions limit for each request. The maximum allowed batch_size is 1000.
 
         Yields:
             App: The next matching solution.
         """
@@ -3730,14 +3914,20 @@
         generator = self._find_all(self.find_apps, request, items_field='content', batch_size=batch_size)
         yield from generator
 
     @add_headers('client')
     def get_app(self, app_id: str, lang: Optional[str] = None) -> App:
         """Gets information from Toloka about an App solution.
 
+        Example:
+            >>> app = toloka_client.get_app('2eN4l59qL2xHB5b8Jqp6')
+            >>> print(app.id, app.name)
+            >>> print(app.description)
+            ...
+
         Args:
             app_id: The ID of the solution.
             lang: ISO 639 language code.
 
         Returns:
             App: The App solution.
         """
@@ -3757,14 +3947,27 @@
     ) -> search_results.AppItemSearchResult:
         """Finds task items that match certain criteria in an App project.
 
         The number of returned items is limited. To find remaining items call `find_app_items` with updated search criteria.
 
         To iterate over all matching items you may use the [get_app_items](toloka.client.TolokaClient.get_app_items.md) method.
 
+        Example:
+            Finding items in an App project that were created starting some date.
+            >>> search = toloka_client.find_app_items(
+            >>>     app_project_id = 'Q2d15QBjpwWuDz8Z321g',
+            >>>     created_gte = '2022-06-16',
+            >>>     sort = 'created')
+            >>> for app_item in search.content:
+            >>>     print(app_item.id, app_item.created_at)
+            >>>
+            >>> if search.has_more:
+            >>>     print('...')
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             request: Search criteria.
             sort: Sorting options. Default: `None`.
             limit: Returned items limit. The maximum allowed limit is 1000.
 
         Returns:
@@ -3787,14 +3990,20 @@
     ) -> Generator[AppItem, None, None]:
         """Finds all App task items that match certain criteria in an App project.
 
         `get_app_items` returns a generator. You can iterate over all found items using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort items use the [find_app_items](toloka.client.TolokaClient.find_app_items.md) method.
 
+        Example:
+            >>> items = toloka_client.get_app_items('Q2d15QBjpwWuDz8Z321g')
+            >>> for item in items:
+            >>>     print(item.id, item.status, item.finished_at)
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             request: Search criteria.
             batch_size: Returned items limit for each request. The maximum allowed batch_size is 1000.
 
         Yields:
             AppItem: The next matching item.
@@ -3808,14 +4017,28 @@
         yield from generator
 
     @expand('app_item')
     @add_headers('client')
     def create_app_item(self, app_project_id: str, app_item: AppItem) -> AppItem:
         """Creates an App task item in Toloka.
 
+        Example:
+            The following example is suitable for a project
+            that requires `query` and `website_url` keys to be present in input data.
+
+            >>> new_item = {
+            >>>     'batch_id' : '4Va2BBWKL88S4QyAgVje',
+            >>>     'input_data' : {
+            >>>         'id':'40', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'
+            >>>     }
+            >>> }
+            >>> new_item = toloka_client.create_app_item(app_project_id = 'Q2d15QBjpwWuDz8Z321g', app_item = new_item)
+            >>> print(new_item.created_at)
+            ...
+
         Args:
             app_project_id: The ID of the App project to create the item in.
             app_item: The task item with parameters.
 
         Returns:
             AppItem: Created App task item with updated parameters.
         """
@@ -3827,14 +4050,25 @@
         return structure(response, AppItem)
 
     @expand('request')
     @add_headers('client')
     def create_app_items(self, app_project_id: str, request: AppItemsCreateRequest):
         """Creates task items in an App project in Toloka and adds them to an existing batch.
 
+        Example:
+            The following example is suitable for a project
+            that requires `query` and `website_url` keys to be present in input data.
+
+            >>> new_items = [
+            >>>     {'id':'20', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'},
+            >>>     {'id':'21', 'query':'crowd kit', 'website_url':'https://toloka.ai/en/docs/crowd-kit'}
+            >>> ]
+            >>> toloka_client.create_app_items(app_project_id = 'Q2d15QBjpwWuDz8Z321g', batch_id = '4Va2BBWKL88S4QyAgVje', items = new_items)
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             request: The request parameters.
         """
 
         if self.url != self.Environment.PRODUCTION.value:
             raise RuntimeError('this method supports only production environment')
@@ -3842,14 +4076,20 @@
         self._raw_request('post', f'/app/v0/app-projects/{app_project_id}/items/bulk', json=unstructure(request))
         return
 
     @add_headers('client')
     def get_app_item(self, app_project_id: str, app_item_id: str) -> AppItem:
         """Gets information from Toloka about an App task item.
 
+        Example:
+            >>> item = toloka_client.get_app_item(app_project_id = 'Q2d15QBjpwWuDz8Z321g', app_item_id = 'V40aPPA2j64TORQyY54Z')
+            >>> print(item.input_data)
+            >>> print(item.output_data)
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             app_item_id: The ID of the item.
 
         Returns:
             AppItem: The App task item.
         """
@@ -3899,14 +4139,20 @@
     ) -> Generator[AppBatch, None, None]:
         """Finds all batches that match certain criteria in an App project.
 
         `get_app_batches` returns a generator. You can iterate over all found batches using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort batches use the [find_app_batches](toloka.client.TolokaClient.find_app_batches.md) method.
 
+        Example:
+            >>> batches = toloka_client.get_app_batches(app_project_id = 'Q2d15QBjpwWuDz8Z321g', status = 'NEW')
+            >>> for batch in batches:
+            >>>     print(batch.id, batch.status, batch.items_count)
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             request: Search criteria.
             batch_size: Returned app batches limit for each request. The maximum allowed batch_size is 1000.
 
         Yields:
             AppBatch: The next matching batch.
@@ -3920,14 +4166,25 @@
         yield from generator
 
     @expand('request')
     @add_headers('client')
     def create_app_batch(self, app_project_id: str, request: AppBatchCreateRequest) -> AppBatch:
         """Creates a batch with task items in an App project in Toloka.
 
+        Example:
+            The following example is suitable for a project
+            that requires `query` and `website_url` keys to be present in input data.
+
+            >>> new_items = [
+            >>>     {'id':'30', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'},
+            >>>     {'id':'31', 'query':'crowd kit', 'website_url':'https://toloka.ai/en/docs/crowd-kit'}
+            >>> ]
+            >>> toloka_client.create_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', items = new_items)
+            ...
+
         Args:
             app_project_id: The ID of the project.
             request: The request parameters.
 
         Returns:
             AppBatch: Created batch with updated parameters.
         """
@@ -3938,14 +4195,19 @@
         response = self._request('post', f'/app/v0/app-projects/{app_project_id}/batches', json=unstructure(request))
         return structure(response, AppBatch)
 
     @add_headers('client')
     def get_app_batch(self, app_project_id: str, batch_id: str) -> AppBatch:
         """Gets information from Toloka about a batch in an App project.
 
+        Example:
+            >>> batch = toloka_client.get_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', app_batch_id = '4Va2BBWKL88S4QyAgVje')
+            >>> print(batch.status, batch.items_count, batch.cost)
+            ...
+
         Args:
             app_project_id: The ID of the project.
             batch_id: The ID of the batch.
 
         Returns:
             AppBatch: The App batch.
         """
@@ -3955,37 +4217,49 @@
 
         response = self._request('get', f'/app/v0/app-projects/{app_project_id}/batches/{batch_id}')
         return structure(response, AppBatch)
 
     @expand('patch')
     @add_headers('client')
     def patch_app_batch(self, app_project_id: str, batch_id: str, patch: AppBatchPatch) -> AppBatch:
-        """Updates an App batch name.
+        """Updates an App batch.
 
         Args:
-            app_project_id: The ID of the project.
+            app_project_id: The ID of the App project containing the batch.
             batch_id: The ID of the batch.
-            patch: New name value.
+            patch: Parameters to update.
+
+        Example:
+            Changing the batch name.
+
+            >>> batch = toloka_client.patch_app_batch(
+            >>>     app_project_id = 'Q2d15QBjpwWuDz8Z321g', batch_id = '4Va2BBWKL88S4QyAgVje',
+            >>>     name = 'Preliminary batch')
+            ...
 
         Returns:
-            AppBatch: The App batch.
+            AppBatch: The updated App batch.
         """
 
         if self.url != self.Environment.PRODUCTION.value:
             raise RuntimeError('this method supports only production environment')
 
         response = self._request(
             'patch', f'/app/v0/app-projects/{app_project_id}/batches/{batch_id}', json=unstructure(patch)
         )
         return structure(response, AppBatch)
 
     @add_headers('client')
     def start_app_batch(self, app_project_id: str, batch_id: str):
         """Launches annotation of a batch of task items in an App project.
 
+        Example:
+            >>> toloka_client.start_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', app_batch_id = '4Va2BBWKL88S4QyAgVje')
+            ...
+
         Args:
             app_project_id: The ID of the project.
             batch_id: The ID of the batch.
         """
 
         if self.url != self.Environment.PRODUCTION.value:
             raise RuntimeError('this method supports only production environment')
@@ -3993,15 +4267,19 @@
         self._raw_request('post', f'/app/v0/app-projects/{app_project_id}/batches/{batch_id}/start')
         return
 
     @add_headers('client')
     def stop_app_batch(self, app_project_id: str, batch_id: str):
         """Stops annotation of a batch of task items in an App project.
 
-        Processing can be stopped only for the batch with the PROCESSING status.
+        Processing can be stopped only for the batch with the `PROCESSING` status.
+
+        Example:
+            >>> toloka_client.stop_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', batch_id = '4Va2BBWKL88S4QyAgVje')
+            ...
 
         Args:
             app_project_id: The ID of the project.
             batch_id: The ID of the batch.
         """
 
         if self.url != self.Environment.PRODUCTION.value:
@@ -4010,15 +4288,19 @@
         self._raw_request('post', f'/app/v0/app-projects/{app_project_id}/batches/{batch_id}/stop')
         return
 
     @add_headers('client')
     def resume_app_batch(self, app_project_id: str, batch_id: str):
         """Resumes annotation of a batch of task items in an App project.
 
-        Processing can be resumed only for the batch with the STOPPING or STOPPED status.
+        Processing can be resumed only for the batch with the `STOPPING` or `STOPPED` status.
+
+        Example:
+            >>> toloka_client.resume_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', batch_id = '4Va2BBWKL88S4QyAgVje')
+            ...
 
         Args:
             app_project_id: The ID of the project.
             batch_id: The ID of the batch.
         """
 
         if self.url != self.Environment.PRODUCTION.value:
```

### Comparing `toloka-kit-1.1.4/src/client/__init__.pyi` & `toloka-kit-1.2.0/src/client/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,14 @@
     'Requester',
     'Skill',
     'SetUserSkillRequest',
     'TaskSuite',
     'Task',
     'Training',
     'UserBonus',
-    'UserBonusCreateRequestParameters',
     'UserRestriction',
     'UserSkill',
     'User',
     'Pool',
     'PoolPatchRequest',
     'Project',
     'AppProject',
@@ -167,18 +166,15 @@
 from toloka.client.project import Project
 from toloka.client.requester import Requester
 from toloka.client.skill import Skill
 from toloka.client.task import Task
 from toloka.client.task_suite import TaskSuite
 from toloka.client.training import Training
 from toloka.client.user import User
-from toloka.client.user_bonus import (
-    UserBonus,
-    UserBonusCreateRequestParameters,
-)
+from toloka.client.user_bonus import UserBonus
 from toloka.client.user_restriction import UserRestriction
 from toloka.client.user_skill import (
     SetUserSkillRequest,
     UserSkill,
 )
 
 
@@ -1064,45 +1060,44 @@
         ...
 
     def add_message_thread_to_folders(
         self,
         message_thread_id: str,
         folders: typing.Union[typing.List[typing.Union[toloka.client.message_thread.Folder, str]], toloka.client.message_thread.MessageThreadFolders]
     ) -> toloka.client.message_thread.MessageThread:
-        """Adds a message chain to one or more folders ("unread", "important" etc.)
+        """Adds a message thread to folders.
 
         Args:
-            message_thread_id: ID of message chain.
-            folders: List of folders, where to move chain.
+            message_thread_id: The ID of the message thread.
+            folders: A list of folders where to add the thread.
 
         Returns:
-            MessageThread: Full object by ID with updated folders.
+            MessageThread: The updated message thread.
 
         Example:
             >>> toloka_client.add_message_thread_to_folders(message_thread_id='1', folders=['IMPORTANT'])
             ...
         """
         ...
 
     @typing.overload
     def compose_message_thread(self, compose: toloka.client.message_thread.MessageThreadCompose) -> toloka.client.message_thread.MessageThread:
-        """Sends a message to a Toloker.
-
-        The sent message is added to a new message thread.
+        """Creates a message thread and sends the first thread message to Tolokers.
 
         Args:
-            compose: Message parameters.
+            compose: Parameters for creating the message thread.
 
         Returns:
-            MessageThread: New created thread.
+            MessageThread: The created message thread.
 
         Example:
-            If you want to thank Tolokers who have tried to complete your tasks, send them a nice message.
+            A message is sent to all Tolokers who have tried to complete your tasks.
+            The message is in english. Tolokers can't reply to your message.
 
-            >>> message_text = "Amazing job! We've just trained our first model with the data YOU prepared for us. Thank you!"
+            >>> message_text = "Amazing job! We've just trained our first model with the data you prepared for us. Thank you!"
             >>> toloka_client.compose_message_thread(
             >>>     recipients_select_type='ALL',
             >>>     topic={'EN': 'Thank you!'},
             >>>     text={'EN': message_text},
             >>>     answerable=False
             >>> )
             ...
@@ -1116,28 +1111,27 @@
         recipients_select_type: typing.Union[toloka.client.message_thread.RecipientsSelectType, str, None] = None,
         topic: typing.Optional[typing.Dict[str, str]] = None,
         text: typing.Optional[typing.Dict[str, str]] = None,
         answerable: typing.Optional[bool] = None,
         recipients_ids: typing.Optional[typing.List[str]] = None,
         recipients_filter: typing.Optional[toloka.client.filter.FilterCondition] = None
     ) -> toloka.client.message_thread.MessageThread:
-        """Sends a message to a Toloker.
-
-        The sent message is added to a new message thread.
+        """Creates a message thread and sends the first thread message to Tolokers.
 
         Args:
-            compose: Message parameters.
+            compose: Parameters for creating the message thread.
 
         Returns:
-            MessageThread: New created thread.
+            MessageThread: The created message thread.
 
         Example:
-            If you want to thank Tolokers who have tried to complete your tasks, send them a nice message.
+            A message is sent to all Tolokers who have tried to complete your tasks.
+            The message is in english. Tolokers can't reply to your message.
 
-            >>> message_text = "Amazing job! We've just trained our first model with the data YOU prepared for us. Thank you!"
+            >>> message_text = "Amazing job! We've just trained our first model with the data you prepared for us. Thank you!"
             >>> toloka_client.compose_message_thread(
             >>>     recipients_select_type='ALL',
             >>>     topic={'EN': 'Thank you!'},
             >>>     text={'EN': message_text},
             >>>     answerable=False
             >>> )
             ...
@@ -1162,15 +1156,15 @@
             sort: Sorting options. Default: `None`.
             limit: Returned message threads limit. The default limit is 50. The maximum allowed limit is 300.
 
         Returns:
             MessageThreadSearchResult: Found message threads and a flag showing whether there are more matching threads.
 
         Example:
-            Find all message threads in the Inbox folder.
+            Finding all message threads in the `INBOX` folder.
 
             >>> toloka_client.find_message_threads(folder='INBOX')
             ...
         """
         ...
 
     @typing.overload
@@ -1200,42 +1194,44 @@
             sort: Sorting options. Default: `None`.
             limit: Returned message threads limit. The default limit is 50. The maximum allowed limit is 300.
 
         Returns:
             MessageThreadSearchResult: Found message threads and a flag showing whether there are more matching threads.
 
         Example:
-            Find all message threads in the Inbox folder.
+            Finding all message threads in the `INBOX` folder.
 
             >>> toloka_client.find_message_threads(folder='INBOX')
             ...
         """
         ...
 
     def reply_message_thread(
         self,
         message_thread_id: str,
         reply: toloka.client.message_thread.MessageThreadReply
     ) -> toloka.client.message_thread.MessageThread:
-        """Replies to a message in thread
+        """Sends a reply message in a thread.
 
         Args:
-            message_thread_id: In which thread to reply.
-            reply: Reply message.
+            message_thread_id: The ID of the thread.
+            reply: The reply message.
 
         Returns:
-            MessageThread: New created message.
+            MessageThread: The updated message thread.
 
         Example:
+            Sending a reply to all unread messages.
+
             >>> message_threads = toloka_client.get_message_threads(folder='UNREAD')
             >>> message_reply = {'EN': 'Thank you for your message! I will get back to you soon.'}
             >>> for thread in message_threads:
             >>>     toloka_client.reply_message_thread(
             >>>         message_thread_id=thread.id,
-            >>>         reply=toloka.message_thread.MessageThreadReply(text=message_reply)
+            >>>         reply=toloka.client.message_thread.MessageThreadReply(text=message_reply)
             >>>     )
             ...
         """
         ...
 
     @typing.overload
     def get_message_threads(
@@ -1301,22 +1297,22 @@
         ...
 
     def remove_message_thread_from_folders(
         self,
         message_thread_id: str,
         folders: typing.Union[typing.List[typing.Union[toloka.client.message_thread.Folder, str]], toloka.client.message_thread.MessageThreadFolders]
     ) -> toloka.client.message_thread.MessageThread:
-        """Deletes a message chain from one or more folders ("unread", "important" etc.)
+        """Removes a message thread from folders.
 
         Args:
-            message_thread_id: ID of message chain.
-            folders:  List of folders, where from to remove chain.
+            message_thread_id: The ID of the message thread.
+            folders: A list of folders.
 
         Returns:
-            MessageThread: Full object by ID with updated folders.
+            MessageThread: The updated message thread.
 
         Example:
             >>> toloka_client.remove_message_thread_from_folders(message_thread_id='1', folders=['IMPORTANT'])
             ...
         """
         ...
 
@@ -2703,35 +2699,35 @@
 
         Example:
             >>> toloka_client.update_skill(skill_id=old_skill_id, skill=new_skill_object)
             ...
         """
         ...
 
-    def get_analytics(self, stats: typing.List[toloka.client.analytics_request.AnalyticsRequest]) -> toloka.client.operations.Operation:
-        """Sends analytics queries, for example, to estimate the percentage of completed tasks in the pool
+    def get_analytics(self, stats: typing.List[toloka.client.analytics_request.AnalyticsRequest]) -> toloka.client.operations.AnalyticsOperation:
+        """Sends analytics requests to Toloka.
 
-        Only pool analytics queries are available.
-        The values of different analytical metrics will be returned in the "details" field of the operation when it is
-        completed. See the example.
         You can request up to 10 metrics at a time.
 
+        The values of different analytical metrics are returned in the `details` field of the operation when it is completed.
+
         Args:
-            stats: Analytics queries list.
+            stats: A list of analytics requests.
 
         Returns:
-            operations.Operation: An operation that you can wait for to get the required statistics.
+            operations.AnalyticsOperation: An object to track the progress of the operation.
 
         Example:
-            How to get task completion percentage for one pool.
+            The example shows how get the percentage of completed tasks in the pool.
 
             >>> from toloka.client.analytics_request import CompletionPercentagePoolAnalytics
-            >>> operation = toloka_client.get_analytics([CompletionPercentagePoolAnalytics(subject_id=pool_id)])
+            >>> operation = toloka_client.get_analytics([CompletionPercentagePoolAnalytics(subject_id='1080020')])
             >>> operation = toloka_client.wait_operation(operation)
-            >>> print(operation.details['value'][0]['result']['value'])
+            >>> print(operation.details['value'][0])
+            >>> completed_task_percentage = operation.details['value'][0]['result']['value']
             ...
         """
         ...
 
     @typing.overload
     def create_task(
         self,
@@ -2763,17 +2759,18 @@
         ...
 
     @typing.overload
     def create_task(
         self,
         task: toloka.client.task.Task,
         *,
+        operation_id: typing.Optional[uuid.UUID] = ...,
+        async_mode: typing.Optional[bool] = True,
         allow_defaults: typing.Optional[bool] = None,
-        open_pool: typing.Optional[bool] = None,
-        operation_id: typing.Optional[uuid.UUID] = ...
+        open_pool: typing.Optional[bool] = None
     ) -> toloka.client.task.Task:
         """Creates a new task in Toloka.
 
         You can send a maximum of 100,000 requests of this kind per minute and a maximum of 2,000,000 requests per day.
 
         To create several tasks at once use the [create_tasks](toloka.client.TolokaClient.create_tasks.md) method.
 
@@ -2855,19 +2852,19 @@
         ...
 
     @typing.overload
     def create_tasks(
         self,
         tasks: typing.List[toloka.client.task.Task],
         *,
+        operation_id: typing.Optional[uuid.UUID] = ...,
+        async_mode: typing.Optional[bool] = True,
         allow_defaults: typing.Optional[bool] = None,
         open_pool: typing.Optional[bool] = None,
-        operation_id: typing.Optional[uuid.UUID] = ...,
-        skip_invalid_items: typing.Optional[bool] = None,
-        async_mode: typing.Optional[bool] = True
+        skip_invalid_items: typing.Optional[bool] = None
     ) -> toloka.client.batch_create_results.TaskBatchCreateResult:
         """Creates several tasks in Toloka.
 
         You can add together general and control tasks.
         Tasks can be added to different pools.
         Note that pools must be configured before accepting new tasks. For example, [mixer configuration](toloka.client.pool.mixer_config.MixerConfig.md) must be set.
 
@@ -2949,19 +2946,19 @@
         ...
 
     @typing.overload
     def create_tasks_async(
         self,
         tasks: typing.List[toloka.client.task.Task],
         *,
+        operation_id: typing.Optional[uuid.UUID] = ...,
+        async_mode: typing.Optional[bool] = True,
         allow_defaults: typing.Optional[bool] = None,
         open_pool: typing.Optional[bool] = None,
-        operation_id: typing.Optional[uuid.UUID] = ...,
-        skip_invalid_items: typing.Optional[bool] = None,
-        async_mode: typing.Optional[bool] = True
+        skip_invalid_items: typing.Optional[bool] = None
     ) -> toloka.client.operations.TasksCreateOperation:
         """Creates tasks in Toloka asynchronously.
 
         You can send a maximum of 100,000 requests of this kind per minute and a maximum of 2,000,000 requests per day.
 
         See also the [create_tasks](toloka.client.TolokaClient.create_tasks.md) method.
 
@@ -3270,18 +3267,17 @@
 
     @typing.overload
     def create_task_suite(
         self,
         task_suite: toloka.client.task_suite.TaskSuite,
         *,
         operation_id: typing.Optional[uuid.UUID] = ...,
-        skip_invalid_items: typing.Optional[bool] = None,
+        async_mode: typing.Optional[bool] = True,
         allow_defaults: typing.Optional[bool] = None,
-        open_pool: typing.Optional[bool] = None,
-        async_mode: typing.Optional[bool] = True
+        open_pool: typing.Optional[bool] = None
     ) -> toloka.client.task_suite.TaskSuite:
         """Creates a task suite in Toloka.
 
         Usually, you don't need to create a task suite manually, because Toloka can group tasks into suites automatically.
 
         Use this method if you need to group specific tasks together or to set different parameters in different task suites.
 
@@ -3306,15 +3302,15 @@
         """
         ...
 
     @typing.overload
     def create_task_suites(
         self,
         task_suites: typing.List[toloka.client.task_suite.TaskSuite],
-        parameters: typing.Optional[toloka.client.task_suite.TaskSuiteCreateRequestParameters] = None
+        parameters: typing.Optional[toloka.client.task_suite.TaskSuitesCreateRequestParameters] = None
     ) -> toloka.client.batch_create_results.TaskSuiteBatchCreateResult:
         """Creates several task suites in Toloka.
 
         Usually, you don't need to create a task suite manually, because Toloka can group tasks into suites automatically.
 
         Use this method if you need to group specific tasks together or to set different parameters in different task suites.
         Task suites can be created in different pools. You can create general and control tasks or task suites in different pools with a single method call.
@@ -3356,18 +3352,18 @@
 
     @typing.overload
     def create_task_suites(
         self,
         task_suites: typing.List[toloka.client.task_suite.TaskSuite],
         *,
         operation_id: typing.Optional[uuid.UUID] = ...,
-        skip_invalid_items: typing.Optional[bool] = None,
+        async_mode: typing.Optional[bool] = True,
         allow_defaults: typing.Optional[bool] = None,
         open_pool: typing.Optional[bool] = None,
-        async_mode: typing.Optional[bool] = True
+        skip_invalid_items: typing.Optional[bool] = None
     ) -> toloka.client.batch_create_results.TaskSuiteBatchCreateResult:
         """Creates several task suites in Toloka.
 
         Usually, you don't need to create a task suite manually, because Toloka can group tasks into suites automatically.
 
         Use this method if you need to group specific tasks together or to set different parameters in different task suites.
         Task suites can be created in different pools. You can create general and control tasks or task suites in different pools with a single method call.
@@ -3407,15 +3403,15 @@
         """
         ...
 
     @typing.overload
     def create_task_suites_async(
         self,
         task_suites: typing.List[toloka.client.task_suite.TaskSuite],
-        parameters: typing.Optional[toloka.client.task_suite.TaskSuiteCreateRequestParameters] = None
+        parameters: typing.Optional[toloka.client.task_suite.TaskSuitesCreateRequestParameters] = None
     ) -> toloka.client.operations.TaskSuiteCreateBatchOperation:
         """Creates several task suites in Toloka asynchronously.
 
         You can send a maximum of 100,000 requests of this kind per minute and 2,000,000 requests per day.
         It is recommended that you create no more than 10,000 task suites in a single request.
 
         See also the [create_task_suites](toloka.client.TolokaClient.create_task_suites.md) method.
@@ -3447,18 +3443,18 @@
 
     @typing.overload
     def create_task_suites_async(
         self,
         task_suites: typing.List[toloka.client.task_suite.TaskSuite],
         *,
         operation_id: typing.Optional[uuid.UUID] = ...,
-        skip_invalid_items: typing.Optional[bool] = None,
+        async_mode: typing.Optional[bool] = True,
         allow_defaults: typing.Optional[bool] = None,
         open_pool: typing.Optional[bool] = None,
-        async_mode: typing.Optional[bool] = True
+        skip_invalid_items: typing.Optional[bool] = None
     ) -> toloka.client.operations.TaskSuiteCreateBatchOperation:
         """Creates several task suites in Toloka asynchronously.
 
         You can send a maximum of 100,000 requests of this kind per minute and 2,000,000 requests per day.
         It is recommended that you create no more than 10,000 task suites in a single request.
 
         See also the [create_task_suites](toloka.client.TolokaClient.create_task_suites.md) method.
@@ -3867,26 +3863,26 @@
         request: toloka.client.search_requests.OperationSearchRequest,
         batch_size: typing.Optional[int] = None
     ) -> typing.Generator[toloka.client.operations.Operation, None, None]:
         """Finds all operations that match certain rules and returns them in an iterable object
 
         `get_operations` returns a generator. You can iterate over all found operations using the generator. Several requests to the Toloka server are possible while iterating.
 
-         If you need to sort operations use the [find_operations](toloka.client.TolokaClient.find_operations.md) method.
+        If you need to sort operations use the [find_operations](toloka.client.TolokaClient.find_operations.md) method.
+
+        Args:
+            request: Search criteria.
+            batch_size: Returned operations limit for each request. The default batch_size is 50. The maximum allowed batch_size is 500.
 
-         Args:
-             request: Search criteria.
-             batch_size: Returned operations limit for each request. The default batch_size is 50. The maximum allowed batch_size is 500.
-
-         Yields:
-             Operation: The next matching operations.
-
-         Example:
-             >>> bonuses = list(toloka_client.get_operations(submitted_lt='2021-06-01T00:00:00'))
-             ...
+        Yields:
+            Operation: The next matching operations.
+
+        Example:
+            >>> bonuses = list(toloka_client.get_operations(submitted_lt='2021-06-01T00:00:00'))
+            ...
         """
         ...
 
     @typing.overload
     def get_operations(
         self,
         type: typing.Optional[toloka.client.operations.OperationType] = None,
@@ -3905,26 +3901,26 @@
         finished_gte: typing.Optional[datetime.datetime] = None,
         batch_size: typing.Optional[int] = None
     ) -> typing.Generator[toloka.client.operations.Operation, None, None]:
         """Finds all operations that match certain rules and returns them in an iterable object
 
         `get_operations` returns a generator. You can iterate over all found operations using the generator. Several requests to the Toloka server are possible while iterating.
 
-         If you need to sort operations use the [find_operations](toloka.client.TolokaClient.find_operations.md) method.
+        If you need to sort operations use the [find_operations](toloka.client.TolokaClient.find_operations.md) method.
+
+        Args:
+            request: Search criteria.
+            batch_size: Returned operations limit for each request. The default batch_size is 50. The maximum allowed batch_size is 500.
+
+        Yields:
+            Operation: The next matching operations.
 
-         Args:
-             request: Search criteria.
-             batch_size: Returned operations limit for each request. The default batch_size is 50. The maximum allowed batch_size is 500.
-
-         Yields:
-             Operation: The next matching operations.
-
-         Example:
-             >>> bonuses = list(toloka_client.get_operations(submitted_lt='2021-06-01T00:00:00'))
-             ...
+        Example:
+            >>> bonuses = list(toloka_client.get_operations(submitted_lt='2021-06-01T00:00:00'))
+            ...
         """
         ...
 
     def get_operation_log(self, operation_id: str) -> typing.List[toloka.client.operation_log.OperationLogItem]:
         """Reads information about validation errors and which task (or task suites) were created
 
         You don't need to call this method if you use "create_tasks" for creating tasks ("create_task_suites" for task suites).
@@ -3985,15 +3981,15 @@
 
     @typing.overload
     def create_user_bonus(
         self,
         user_bonus: toloka.client.user_bonus.UserBonus,
         *,
         operation_id: typing.Optional[uuid.UUID] = ...,
-        skip_invalid_items: typing.Optional[bool] = None
+        async_mode: typing.Optional[bool] = True
     ) -> toloka.client.user_bonus.UserBonus:
         """Issues payments directly to a Toloker.
 
         You can send a maximum of 10,000 requests of this kind per day.
 
         Args:
             user_bonus: To whom, how much to pay and for what.
@@ -4025,15 +4021,15 @@
         """
         ...
 
     @typing.overload
     def create_user_bonuses(
         self,
         user_bonuses: typing.List[toloka.client.user_bonus.UserBonus],
-        parameters: typing.Optional[toloka.client.user_bonus.UserBonusCreateRequestParameters] = None
+        parameters: typing.Optional[toloka.client.user_bonus.UserBonusesCreateRequestParameters] = None
     ) -> toloka.client.batch_create_results.UserBonusBatchCreateResult:
         """Creates rewards for Tolokers.
 
         Right now it's safer to use asynchronous version: "create_user_bonuses_async"
         You can send a maximum of 10,000 requests of this kind per day.
 
         Args:
@@ -4081,14 +4077,15 @@
 
     @typing.overload
     def create_user_bonuses(
         self,
         user_bonuses: typing.List[toloka.client.user_bonus.UserBonus],
         *,
         operation_id: typing.Optional[uuid.UUID] = ...,
+        async_mode: typing.Optional[bool] = True,
         skip_invalid_items: typing.Optional[bool] = None
     ) -> toloka.client.batch_create_results.UserBonusBatchCreateResult:
         """Creates rewards for Tolokers.
 
         Right now it's safer to use asynchronous version: "create_user_bonuses_async"
         You can send a maximum of 10,000 requests of this kind per day.
 
@@ -4135,15 +4132,15 @@
         """
         ...
 
     @typing.overload
     def create_user_bonuses_async(
         self,
         user_bonuses: typing.List[toloka.client.user_bonus.UserBonus],
-        parameters: typing.Optional[toloka.client.user_bonus.UserBonusCreateRequestParameters] = None
+        parameters: typing.Optional[toloka.client.user_bonus.UserBonusesCreateRequestParameters] = None
     ) -> toloka.client.operations.UserBonusCreateBatchOperation:
         """Issues payments directly to Tolokers, asynchronously creates many `UserBonus` instances.
 
         You can send a maximum of 10,000 requests of this kind per day.
 
         Args:
             user_bonuses: To whom, how much to pay and for what.
@@ -4190,14 +4187,15 @@
 
     @typing.overload
     def create_user_bonuses_async(
         self,
         user_bonuses: typing.List[toloka.client.user_bonus.UserBonus],
         *,
         operation_id: typing.Optional[uuid.UUID] = ...,
+        async_mode: typing.Optional[bool] = True,
         skip_invalid_items: typing.Optional[bool] = None
     ) -> toloka.client.operations.UserBonusCreateBatchOperation:
         """Issues payments directly to Tolokers, asynchronously creates many `UserBonus` instances.
 
         You can send a maximum of 10,000 requests of this kind per day.
 
         Args:
@@ -4328,26 +4326,26 @@
         request: toloka.client.search_requests.UserBonusSearchRequest,
         batch_size: typing.Optional[int] = None
     ) -> typing.Generator[toloka.client.user_bonus.UserBonus, None, None]:
         """Finds all Tolokers' rewards that match certain rules and returns them in an iterable object
 
         `get_user_bonuses` returns a generator. You can iterate over all found Tolokers' rewards using the generator. Several requests to the Toloka server are possible while iterating.
 
-         If you need to sort rewards use the [find_user_bonuses](toloka.client.TolokaClient.find_user_bonuses.md) method.
+        If you need to sort rewards use the [find_user_bonuses](toloka.client.TolokaClient.find_user_bonuses.md) method.
 
-         Args:
-             request: Search criteria.
-             batch_size: Returned Tolokers' rewards limit for each request. The maximum allowed batch_size is 300.
-
-         Yields:
-             UserBonus: The next matching Toloker's reward.
-
-         Example:
-             >>> bonuses = list(toloka_client.get_user_bonuses(created_lt='2021-06-01T00:00:00'))
-             ...
+        Args:
+            request: Search criteria.
+            batch_size: Returned Tolokers' rewards limit for each request. The maximum allowed batch_size is 300.
+
+        Yields:
+            UserBonus: The next matching Toloker's reward.
+
+        Example:
+            >>> bonuses = list(toloka_client.get_user_bonuses(created_lt='2021-06-01T00:00:00'))
+            ...
         """
         ...
 
     @typing.overload
     def get_user_bonuses(
         self,
         user_id: typing.Optional[str] = None,
@@ -4363,26 +4361,26 @@
         created_gte: typing.Optional[datetime.datetime] = None,
         batch_size: typing.Optional[int] = None
     ) -> typing.Generator[toloka.client.user_bonus.UserBonus, None, None]:
         """Finds all Tolokers' rewards that match certain rules and returns them in an iterable object
 
         `get_user_bonuses` returns a generator. You can iterate over all found Tolokers' rewards using the generator. Several requests to the Toloka server are possible while iterating.
 
-         If you need to sort rewards use the [find_user_bonuses](toloka.client.TolokaClient.find_user_bonuses.md) method.
+        If you need to sort rewards use the [find_user_bonuses](toloka.client.TolokaClient.find_user_bonuses.md) method.
+
+        Args:
+            request: Search criteria.
+            batch_size: Returned Tolokers' rewards limit for each request. The maximum allowed batch_size is 300.
+
+        Yields:
+            UserBonus: The next matching Toloker's reward.
 
-         Args:
-             request: Search criteria.
-             batch_size: Returned Tolokers' rewards limit for each request. The maximum allowed batch_size is 300.
-
-         Yields:
-             UserBonus: The next matching Toloker's reward.
-
-         Example:
-             >>> bonuses = list(toloka_client.get_user_bonuses(created_lt='2021-06-01T00:00:00'))
-             ...
+        Example:
+            >>> bonuses = list(toloka_client.get_user_bonuses(created_lt='2021-06-01T00:00:00'))
+            ...
         """
         ...
 
     @typing.overload
     def find_user_restrictions(
         self,
         request: toloka.client.search_requests.UserRestrictionSearchRequest,
@@ -4798,25 +4796,24 @@
         Example:
             >>> toloka_client.delete_user_skill(user_skill_id='1')
             ...
         """
         ...
 
     def upsert_webhook_subscriptions(self, subscriptions: typing.List[toloka.client.webhook_subscription.WebhookSubscription]) -> toloka.client.batch_create_results.WebhookSubscriptionBatchCreateResult:
-        """Creates (upsert) many webhook-subscriptions.
+        """Creates (upsert) webhook subscriptions.
 
         Args:
-            subscriptions: List of webhook-subscriptions, that will be created.
+            subscriptions: A list of webhook subscriptions to be created.
 
         Returns:
-            batch_create_results.WebhookSubscriptionBatchCreateResult: Result of subscriptions creation.
-                Contains created subscriptions in `items` and problems in "validation_errors".
+            batch_create_results.WebhookSubscriptionBatchCreateResult: The result of the operation.
 
         Raises:
-            ValidationApiError: If no subscriptions were created.
+            ValidationApiError: No subscriptions were created.
 
         Example:
             How to create several subscriptions.
 
             >>> created_result = toloka_client.upsert_webhook_subscriptions([
             >>>     {
             >>>         'webhook_url': 'https://awesome-requester.com/toloka-webhook',
@@ -5069,14 +5066,26 @@
     ) -> toloka.client.search_results.AppProjectSearchResult:
         """Finds App projects that match certain criteria.
 
         The number of returned projects is limited. To find remaining projects call `find_app_projects` with updated search criteria.
 
         To iterate over all matching projects you may use the [get_app_projects](toloka.client.TolokaClient.get_app_projects.md) method.
 
+        Example:
+            Searching active projects based on the App solution with the specified ID.
+
+            >>> search = toloka_client.find_app_projects(
+            >>>     app_id = '9lZaMl363jahzra1rrYq', status = 'READY')
+            >>> for app_project in search.content:
+            >>>     print(app_project.id, app_project.name)
+            >>>
+            >>> if search.has_more:
+            >>>     print('There are more App projects...')
+            ...
+
         Args:
             request: Search criteria.
             sort: The order and direction of sorting the results.
             limit: Returned projects limit. The maximum limit is 5000.
 
         Returns:
             AppProjectSearchResult: Found projects and a flag showing whether there are more matching projects exceeding the limit.
@@ -5109,14 +5118,26 @@
     ) -> toloka.client.search_results.AppProjectSearchResult:
         """Finds App projects that match certain criteria.
 
         The number of returned projects is limited. To find remaining projects call `find_app_projects` with updated search criteria.
 
         To iterate over all matching projects you may use the [get_app_projects](toloka.client.TolokaClient.get_app_projects.md) method.
 
+        Example:
+            Searching active projects based on the App solution with the specified ID.
+
+            >>> search = toloka_client.find_app_projects(
+            >>>     app_id = '9lZaMl363jahzra1rrYq', status = 'READY')
+            >>> for app_project in search.content:
+            >>>     print(app_project.id, app_project.name)
+            >>>
+            >>> if search.has_more:
+            >>>     print('There are more App projects...')
+            ...
+
         Args:
             request: Search criteria.
             sort: The order and direction of sorting the results.
             limit: Returned projects limit. The maximum limit is 5000.
 
         Returns:
             AppProjectSearchResult: Found projects and a flag showing whether there are more matching projects exceeding the limit.
@@ -5131,14 +5152,20 @@
     ) -> typing.Generator[toloka.client.app.AppProject, None, None]:
         """Finds all App projects that match certain criteria.
 
         `get_app_projects` returns a generator. You can iterate over all found projects using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort App projects use the [find_app_projects](toloka.client.TolokaClient.find_app_projects.md) method.
 
+        Example:
+            >>> app_projects = toloka_client.get_app_projects(scope='MY')
+            >>> for app_project in app_projects:
+            >>>     print(app_project.id, app_project.status, app_project.name)
+            ...
+
         Args:
             request: Search criteria.
             batch_size: Returned projects limit for each request. The maximum batch_size is 5000.
 
         Yields:
             AppProject: The next matching App project.
         """
@@ -5169,63 +5196,121 @@
     ) -> typing.Generator[toloka.client.app.AppProject, None, None]:
         """Finds all App projects that match certain criteria.
 
         `get_app_projects` returns a generator. You can iterate over all found projects using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort App projects use the [find_app_projects](toloka.client.TolokaClient.find_app_projects.md) method.
 
+        Example:
+            >>> app_projects = toloka_client.get_app_projects(scope='MY')
+            >>> for app_project in app_projects:
+            >>>     print(app_project.id, app_project.status, app_project.name)
+            ...
+
         Args:
             request: Search criteria.
             batch_size: Returned projects limit for each request. The maximum batch_size is 5000.
 
         Yields:
             AppProject: The next matching App project.
         """
         ...
 
     def create_app_project(self, app_project: toloka.client.app.AppProject) -> toloka.client.app.AppProject:
         """Creates an App project in Toloka.
 
+        Example:
+            >>> app_project = toloka.AppProject(
+            >>>   app_id='9lZaMl363jahzra1rrYq',
+            >>>   name='Example project (product relevance)',
+            >>>   parameters={
+            >>>     "default_language": "en",
+            >>>     "name": "Product relevance project",
+            >>>     "instruction_classes": [
+            >>>       {
+            >>>         "description": "The product is relevant to the query.",
+            >>>         "label": "Relevant",
+            >>>         "value": "relevant"
+            >>>       },
+            >>>       {
+            >>>         "description": "The product is not completely relevant to the query.",
+            >>>         "label": "Irrelevant",
+            >>>         "value": "irrelevant"
+            >>>       }
+            >>>     ],
+            >>>     "instruction_examples": [
+            >>>       {
+            >>>         "description": "The product exactly matches the query.",
+            >>>         "label": "relevant",
+            >>>         "query": "some search query",
+            >>>         "screenshot_url": "https://example.com/1"
+            >>>       },
+            >>>       {
+            >>>         "description": "The product shape matches but the product color does not.",
+            >>>         "label": "irrelevant",
+            >>>         "query": "other search query",
+            >>>         "screenshot_url": "https://example.com/2"
+            >>>       }
+            >>>     ]
+            >>>   }
+            >>> )
+            >>> app_project = toloka_client.create_app_project(app_project)
+            >>> print(app_project.created, app_project.status)
+            ...
+
         Args:
             app_project: The project with parameters.
 
         Returns:
             AppProject: Created App project with updated parameters.
         """
         ...
 
     def get_app_project(self, app_project_id: str) -> toloka.client.app.AppProject:
         """Gets information from Toloka about an App project.
 
+        Example:
+            >>> app_project = toloka_client.get_app_project('Q2d15QBjpwWuDz8Z321g')
+            >>> print(app_project.created, app_project.name)
+            ...
+
         Args:
             app_project_id: The ID of the project.
 
         Returns:
             AppProject: The App project.
         """
         ...
 
     def archive_app_project(self, app_project_id: str) -> toloka.client.app.AppProject:
         """Archives an App project.
 
         The project changes its status to `ARCHIVED`.
 
+        Example:
+            >>> toloka_client.archive_app_project('Q2d15QBjpwWuDz8Z321g')
+            ...
+
         Args:
             app_project_id: The ID of the project.
 
         Returns:
             AppProject: The App project with updated status.
         """
         ...
 
     def unarchive_app_project(self, app_project_id: str) -> toloka.client.app.AppProject:
         """Unarchives an App project.
 
         Previous project status, which was before archiving, is restored.
 
+        Example:
+            >>> toloka_client.unarchive_app_project('Q2d15QBjpwWuDz8Z321g')
+            ...
+
         Args:
             app_project_id: The ID of the project.
 
         Returns:
             AppProject: The App project with updated status.
         """
         ...
@@ -5239,14 +5324,23 @@
     ) -> toloka.client.search_results.AppSearchResult:
         """Finds App solutions that match certain criteria.
 
         The number of returned solutions is limited. To find remaining solutions call `find_apps` with updated search criteria.
 
         To iterate over all matching solutions you may use the [get_apps](toloka.client.TolokaClient.get_apps.md) method.
 
+        Example:
+            >>> search = toloka_client.find_apps()
+            >>> for app in search.content:
+            >>>     print(app.id, app.name)
+            >>>
+            >>> if search.has_more:
+            >>>     print('There are more App solutions...')
+            ...
+
         Args:
             request: Search criteria.
             sort: Sorting options. Default: `None`.
             limit: Returned solutions limit. The maximum allowed limit is 1000.
 
         Returns:
             AppSearchResult: Found solutions and a flag showing whether there are more matching solutions exceeding the limit.
@@ -5267,14 +5361,23 @@
     ) -> toloka.client.search_results.AppSearchResult:
         """Finds App solutions that match certain criteria.
 
         The number of returned solutions is limited. To find remaining solutions call `find_apps` with updated search criteria.
 
         To iterate over all matching solutions you may use the [get_apps](toloka.client.TolokaClient.get_apps.md) method.
 
+        Example:
+            >>> search = toloka_client.find_apps()
+            >>> for app in search.content:
+            >>>     print(app.id, app.name)
+            >>>
+            >>> if search.has_more:
+            >>>     print('There are more App solutions...')
+            ...
+
         Args:
             request: Search criteria.
             sort: Sorting options. Default: `None`.
             limit: Returned solutions limit. The maximum allowed limit is 1000.
 
         Returns:
             AppSearchResult: Found solutions and a flag showing whether there are more matching solutions exceeding the limit.
@@ -5289,14 +5392,20 @@
     ) -> typing.Generator[toloka.client.app.App, None, None]:
         """Finds all App solutions that match certain criteria.
 
         `get_apps` returns a generator. You can iterate over all found solutions using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort solutions use the [find_apps](toloka.client.TolokaClient.find_apps.md) method.
 
+        Example:
+            >>> apps = toloka_client.get_apps()
+            >>> for app in apps:
+            >>>     print(app.id, app.name)
+            ...
+
         Args:
             request: Search criteria.
             batch_size: Returned solutions limit for each request. The maximum allowed batch_size is 1000.
 
         Yields:
             App: The next matching solution.
         """
@@ -5315,14 +5424,20 @@
     ) -> typing.Generator[toloka.client.app.App, None, None]:
         """Finds all App solutions that match certain criteria.
 
         `get_apps` returns a generator. You can iterate over all found solutions using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort solutions use the [find_apps](toloka.client.TolokaClient.find_apps.md) method.
 
+        Example:
+            >>> apps = toloka_client.get_apps()
+            >>> for app in apps:
+            >>>     print(app.id, app.name)
+            ...
+
         Args:
             request: Search criteria.
             batch_size: Returned solutions limit for each request. The maximum allowed batch_size is 1000.
 
         Yields:
             App: The next matching solution.
         """
@@ -5331,14 +5446,20 @@
     def get_app(
         self,
         app_id: str,
         lang: typing.Optional[str] = None
     ) -> toloka.client.app.App:
         """Gets information from Toloka about an App solution.
 
+        Example:
+            >>> app = toloka_client.get_app('2eN4l59qL2xHB5b8Jqp6')
+            >>> print(app.id, app.name)
+            >>> print(app.description)
+            ...
+
         Args:
             app_id: The ID of the solution.
             lang: ISO 639 language code.
 
         Returns:
             App: The App solution.
         """
@@ -5354,14 +5475,27 @@
     ) -> toloka.client.search_results.AppItemSearchResult:
         """Finds task items that match certain criteria in an App project.
 
         The number of returned items is limited. To find remaining items call `find_app_items` with updated search criteria.
 
         To iterate over all matching items you may use the [get_app_items](toloka.client.TolokaClient.get_app_items.md) method.
 
+        Example:
+            Finding items in an App project that were created starting some date.
+            >>> search = toloka_client.find_app_items(
+            >>>     app_project_id = 'Q2d15QBjpwWuDz8Z321g',
+            >>>     created_gte = '2022-06-16',
+            >>>     sort = 'created')
+            >>> for app_item in search.content:
+            >>>     print(app_item.id, app_item.created_at)
+            >>>
+            >>> if search.has_more:
+            >>>     print('...')
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             request: Search criteria.
             sort: Sorting options. Default: `None`.
             limit: Returned items limit. The maximum allowed limit is 1000.
 
         Returns:
@@ -5393,14 +5527,27 @@
     ) -> toloka.client.search_results.AppItemSearchResult:
         """Finds task items that match certain criteria in an App project.
 
         The number of returned items is limited. To find remaining items call `find_app_items` with updated search criteria.
 
         To iterate over all matching items you may use the [get_app_items](toloka.client.TolokaClient.get_app_items.md) method.
 
+        Example:
+            Finding items in an App project that were created starting some date.
+            >>> search = toloka_client.find_app_items(
+            >>>     app_project_id = 'Q2d15QBjpwWuDz8Z321g',
+            >>>     created_gte = '2022-06-16',
+            >>>     sort = 'created')
+            >>> for app_item in search.content:
+            >>>     print(app_item.id, app_item.created_at)
+            >>>
+            >>> if search.has_more:
+            >>>     print('...')
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             request: Search criteria.
             sort: Sorting options. Default: `None`.
             limit: Returned items limit. The maximum allowed limit is 1000.
 
         Returns:
@@ -5417,14 +5564,20 @@
     ) -> typing.Generator[toloka.client.app.AppItem, None, None]:
         """Finds all App task items that match certain criteria in an App project.
 
         `get_app_items` returns a generator. You can iterate over all found items using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort items use the [find_app_items](toloka.client.TolokaClient.find_app_items.md) method.
 
+        Example:
+            >>> items = toloka_client.get_app_items('Q2d15QBjpwWuDz8Z321g')
+            >>> for item in items:
+            >>>     print(item.id, item.status, item.finished_at)
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             request: Search criteria.
             batch_size: Returned items limit for each request. The maximum allowed batch_size is 1000.
 
         Yields:
             AppItem: The next matching item.
@@ -5454,14 +5607,20 @@
     ) -> typing.Generator[toloka.client.app.AppItem, None, None]:
         """Finds all App task items that match certain criteria in an App project.
 
         `get_app_items` returns a generator. You can iterate over all found items using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort items use the [find_app_items](toloka.client.TolokaClient.find_app_items.md) method.
 
+        Example:
+            >>> items = toloka_client.get_app_items('Q2d15QBjpwWuDz8Z321g')
+            >>> for item in items:
+            >>>     print(item.id, item.status, item.finished_at)
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             request: Search criteria.
             batch_size: Returned items limit for each request. The maximum allowed batch_size is 1000.
 
         Yields:
             AppItem: The next matching item.
@@ -5472,14 +5631,28 @@
     def create_app_item(
         self,
         app_project_id: str,
         app_item: toloka.client.app.AppItem
     ) -> toloka.client.app.AppItem:
         """Creates an App task item in Toloka.
 
+        Example:
+            The following example is suitable for a project
+            that requires `query` and `website_url` keys to be present in input data.
+
+            >>> new_item = {
+            >>>     'batch_id' : '4Va2BBWKL88S4QyAgVje',
+            >>>     'input_data' : {
+            >>>         'id':'40', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'
+            >>>     }
+            >>> }
+            >>> new_item = toloka_client.create_app_item(app_project_id = 'Q2d15QBjpwWuDz8Z321g', app_item = new_item)
+            >>> print(new_item.created_at)
+            ...
+
         Args:
             app_project_id: The ID of the App project to create the item in.
             app_item: The task item with parameters.
 
         Returns:
             AppItem: Created App task item with updated parameters.
         """
@@ -5491,14 +5664,28 @@
         app_project_id: str,
         *,
         batch_id: typing.Optional[str] = None,
         input_data: typing.Optional[typing.Dict[str, typing.Any]] = None
     ) -> toloka.client.app.AppItem:
         """Creates an App task item in Toloka.
 
+        Example:
+            The following example is suitable for a project
+            that requires `query` and `website_url` keys to be present in input data.
+
+            >>> new_item = {
+            >>>     'batch_id' : '4Va2BBWKL88S4QyAgVje',
+            >>>     'input_data' : {
+            >>>         'id':'40', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'
+            >>>     }
+            >>> }
+            >>> new_item = toloka_client.create_app_item(app_project_id = 'Q2d15QBjpwWuDz8Z321g', app_item = new_item)
+            >>> print(new_item.created_at)
+            ...
+
         Args:
             app_project_id: The ID of the App project to create the item in.
             app_item: The task item with parameters.
 
         Returns:
             AppItem: Created App task item with updated parameters.
         """
@@ -5508,14 +5695,25 @@
     def create_app_items(
         self,
         app_project_id: str,
         request: toloka.client.app.AppItemsCreateRequest
     ):
         """Creates task items in an App project in Toloka and adds them to an existing batch.
 
+        Example:
+            The following example is suitable for a project
+            that requires `query` and `website_url` keys to be present in input data.
+
+            >>> new_items = [
+            >>>     {'id':'20', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'},
+            >>>     {'id':'21', 'query':'crowd kit', 'website_url':'https://toloka.ai/en/docs/crowd-kit'}
+            >>> ]
+            >>> toloka_client.create_app_items(app_project_id = 'Q2d15QBjpwWuDz8Z321g', batch_id = '4Va2BBWKL88S4QyAgVje', items = new_items)
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             request: The request parameters.
         """
         ...
 
     @typing.overload
@@ -5524,27 +5722,44 @@
         app_project_id: str,
         *,
         batch_id: typing.Optional[str] = None,
         items: typing.Optional[typing.List[typing.Dict[str, typing.Any]]] = None
     ):
         """Creates task items in an App project in Toloka and adds them to an existing batch.
 
+        Example:
+            The following example is suitable for a project
+            that requires `query` and `website_url` keys to be present in input data.
+
+            >>> new_items = [
+            >>>     {'id':'20', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'},
+            >>>     {'id':'21', 'query':'crowd kit', 'website_url':'https://toloka.ai/en/docs/crowd-kit'}
+            >>> ]
+            >>> toloka_client.create_app_items(app_project_id = 'Q2d15QBjpwWuDz8Z321g', batch_id = '4Va2BBWKL88S4QyAgVje', items = new_items)
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             request: The request parameters.
         """
         ...
 
     def get_app_item(
         self,
         app_project_id: str,
         app_item_id: str
     ) -> toloka.client.app.AppItem:
         """Gets information from Toloka about an App task item.
 
+        Example:
+            >>> item = toloka_client.get_app_item(app_project_id = 'Q2d15QBjpwWuDz8Z321g', app_item_id = 'V40aPPA2j64TORQyY54Z')
+            >>> print(item.input_data)
+            >>> print(item.output_data)
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             app_item_id: The ID of the item.
 
         Returns:
             AppItem: The App task item.
         """
@@ -5622,14 +5837,20 @@
     ) -> typing.Generator[toloka.client.app.AppBatch, None, None]:
         """Finds all batches that match certain criteria in an App project.
 
         `get_app_batches` returns a generator. You can iterate over all found batches using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort batches use the [find_app_batches](toloka.client.TolokaClient.find_app_batches.md) method.
 
+        Example:
+            >>> batches = toloka_client.get_app_batches(app_project_id = 'Q2d15QBjpwWuDz8Z321g', status = 'NEW')
+            >>> for batch in batches:
+            >>>     print(batch.id, batch.status, batch.items_count)
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             request: Search criteria.
             batch_size: Returned app batches limit for each request. The maximum allowed batch_size is 1000.
 
         Yields:
             AppBatch: The next matching batch.
@@ -5658,14 +5879,20 @@
     ) -> typing.Generator[toloka.client.app.AppBatch, None, None]:
         """Finds all batches that match certain criteria in an App project.
 
         `get_app_batches` returns a generator. You can iterate over all found batches using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort batches use the [find_app_batches](toloka.client.TolokaClient.find_app_batches.md) method.
 
+        Example:
+            >>> batches = toloka_client.get_app_batches(app_project_id = 'Q2d15QBjpwWuDz8Z321g', status = 'NEW')
+            >>> for batch in batches:
+            >>>     print(batch.id, batch.status, batch.items_count)
+            ...
+
         Args:
             app_project_id: The ID of the App project.
             request: Search criteria.
             batch_size: Returned app batches limit for each request. The maximum allowed batch_size is 1000.
 
         Yields:
             AppBatch: The next matching batch.
@@ -5676,14 +5903,25 @@
     def create_app_batch(
         self,
         app_project_id: str,
         request: toloka.client.app.AppBatchCreateRequest
     ) -> toloka.client.app.AppBatch:
         """Creates a batch with task items in an App project in Toloka.
 
+        Example:
+            The following example is suitable for a project
+            that requires `query` and `website_url` keys to be present in input data.
+
+            >>> new_items = [
+            >>>     {'id':'30', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'},
+            >>>     {'id':'31', 'query':'crowd kit', 'website_url':'https://toloka.ai/en/docs/crowd-kit'}
+            >>> ]
+            >>> toloka_client.create_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', items = new_items)
+            ...
+
         Args:
             app_project_id: The ID of the project.
             request: The request parameters.
 
         Returns:
             AppBatch: Created batch with updated parameters.
         """
@@ -5695,14 +5933,25 @@
         app_project_id: str,
         *,
         name: typing.Optional[str] = None,
         items: typing.Optional[typing.List[typing.Dict[str, typing.Any]]] = None
     ) -> toloka.client.app.AppBatch:
         """Creates a batch with task items in an App project in Toloka.
 
+        Example:
+            The following example is suitable for a project
+            that requires `query` and `website_url` keys to be present in input data.
+
+            >>> new_items = [
+            >>>     {'id':'30', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'},
+            >>>     {'id':'31', 'query':'crowd kit', 'website_url':'https://toloka.ai/en/docs/crowd-kit'}
+            >>> ]
+            >>> toloka_client.create_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', items = new_items)
+            ...
+
         Args:
             app_project_id: The ID of the project.
             request: The request parameters.
 
         Returns:
             AppBatch: Created batch with updated parameters.
         """
@@ -5711,14 +5960,19 @@
     def get_app_batch(
         self,
         app_project_id: str,
         batch_id: str
     ) -> toloka.client.app.AppBatch:
         """Gets information from Toloka about a batch in an App project.
 
+        Example:
+            >>> batch = toloka_client.get_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', app_batch_id = '4Va2BBWKL88S4QyAgVje')
+            >>> print(batch.status, batch.items_count, batch.cost)
+            ...
+
         Args:
             app_project_id: The ID of the project.
             batch_id: The ID of the batch.
 
         Returns:
             AppBatch: The App batch.
         """
@@ -5727,82 +5981,110 @@
     @typing.overload
     def patch_app_batch(
         self,
         app_project_id: str,
         batch_id: str,
         patch: toloka.client.app.AppBatchPatch
     ) -> toloka.client.app.AppBatch:
-        """Updates an App batch name.
+        """Updates an App batch.
 
         Args:
-            app_project_id: The ID of the project.
+            app_project_id: The ID of the App project containing the batch.
             batch_id: The ID of the batch.
-            patch: New name value.
+            patch: Parameters to update.
+
+        Example:
+            Changing the batch name.
+
+            >>> batch = toloka_client.patch_app_batch(
+            >>>     app_project_id = 'Q2d15QBjpwWuDz8Z321g', batch_id = '4Va2BBWKL88S4QyAgVje',
+            >>>     name = 'Preliminary batch')
+            ...
 
         Returns:
-            AppBatch: The App batch.
+            AppBatch: The updated App batch.
         """
         ...
 
     @typing.overload
     def patch_app_batch(
         self,
         app_project_id: str,
         batch_id: str,
         *,
         name: typing.Optional[str] = None
     ) -> toloka.client.app.AppBatch:
-        """Updates an App batch name.
+        """Updates an App batch.
 
         Args:
-            app_project_id: The ID of the project.
+            app_project_id: The ID of the App project containing the batch.
             batch_id: The ID of the batch.
-            patch: New name value.
+            patch: Parameters to update.
+
+        Example:
+            Changing the batch name.
+
+            >>> batch = toloka_client.patch_app_batch(
+            >>>     app_project_id = 'Q2d15QBjpwWuDz8Z321g', batch_id = '4Va2BBWKL88S4QyAgVje',
+            >>>     name = 'Preliminary batch')
+            ...
 
         Returns:
-            AppBatch: The App batch.
+            AppBatch: The updated App batch.
         """
         ...
 
     def start_app_batch(
         self,
         app_project_id: str,
         batch_id: str
     ):
         """Launches annotation of a batch of task items in an App project.
 
+        Example:
+            >>> toloka_client.start_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', app_batch_id = '4Va2BBWKL88S4QyAgVje')
+            ...
+
         Args:
             app_project_id: The ID of the project.
             batch_id: The ID of the batch.
         """
         ...
 
     def stop_app_batch(
         self,
         app_project_id: str,
         batch_id: str
     ):
         """Stops annotation of a batch of task items in an App project.
 
-        Processing can be stopped only for the batch with the PROCESSING status.
+        Processing can be stopped only for the batch with the `PROCESSING` status.
+
+        Example:
+            >>> toloka_client.stop_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', batch_id = '4Va2BBWKL88S4QyAgVje')
+            ...
 
         Args:
             app_project_id: The ID of the project.
             batch_id: The ID of the batch.
         """
         ...
 
     def resume_app_batch(
         self,
         app_project_id: str,
         batch_id: str
     ):
         """Resumes annotation of a batch of task items in an App project.
 
-        Processing can be resumed only for the batch with the STOPPING or STOPPED status.
+        Processing can be resumed only for the batch with the `STOPPING` or `STOPPED` status.
+
+        Example:
+            >>> toloka_client.resume_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', batch_id = '4Va2BBWKL88S4QyAgVje')
+            ...
 
         Args:
             app_project_id: The ID of the project.
             batch_id: The ID of the batch.
         """
         ...
```

### Comparing `toloka-kit-1.1.4/src/client/_converter.py` & `toloka-kit-1.2.0/src/client/_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 import pkg_resources
 from typing import List, Union
 
 import cattr
 from ..util._extendable_enum import ExtendableStrEnum
 
 _CATTRS_VERSION = tuple(map(int, pkg_resources.get_distribution('cattrs').version.split('.')))
+
 if _CATTRS_VERSION < (22, 2, 0):
     converter = cattr.Converter()
 else:
     converter = cattr.converters.BaseConverter()
 
 converter.register_structure_hook_func(
     lambda type_: hasattr(type_, 'structure'),
-    lambda data, type_: type_.structure(data)  # type: ignore
+    lambda data, type_: getattr(type_, 'structure').__func__(type_, data)  # type: ignore
 )
 converter.register_unstructure_hook_func(  # type: ignore
     lambda obj: hasattr(obj, 'unstructure'),
     lambda obj: obj.unstructure()  # type: ignore
 )
 
-
 converter.register_structure_hook(uuid.UUID, lambda data, type_: type_(data))  # type: ignore
 converter.register_unstructure_hook(uuid.UUID, str)
 
 converter.register_structure_hook(
     Union[str, List[str]],
     lambda data, type_: converter.structure(data, List[str] if isinstance(data, list) else str)  # type: ignore
 )
```

### Comparing `toloka-kit-1.1.4/src/client/actions.py` & `toloka-kit-1.2.0/src/client/actions.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/actions.pyi` & `toloka-kit-1.2.0/src/client/actions.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/aggregation.py` & `toloka-kit-1.2.0/src/client/aggregation.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/aggregation.pyi` & `toloka-kit-1.2.0/src/client/aggregation.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/analytics_request.py` & `toloka-kit-1.2.0/src/client/analytics_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 from .primitives.base import BaseTolokaObject
 from ..util._codegen import attribute
 from ..util._docstrings import inherit_docstrings
 from ..util._extendable_enum import ExtendableStrEnum
 
 
 class AnalyticsRequest(BaseTolokaObject, spec_field='subject', spec_enum='Subject'):
-    """Base class for all analytics requests in Toloka
+    """A base class for analytics requests.
 
-    How to use this requests and get some useful information see in example in "TolokaClient.get_analytics".
+    Make analytics requests to Toloka with the [get_analytics](toloka.client.TolokaClient.get_analytics.md) method.
 
     Attributes:
-        subject_id: ID of the object you want to get analytics about.
+        subject_id: The ID of an object to get analytics about.
     """
     @unique
     class Subject(ExtendableStrEnum):
         POOL = 'POOL'
 
     subject_id: str = attribute(required=True)
 
@@ -40,17 +40,18 @@
 @inherit_docstrings
 class PoolAnalyticsRequest(
     AnalyticsRequest,
     spec_value=AnalyticsRequest.Subject.POOL,
     spec_field='name',
     spec_enum='Subject'
 ):
-    """Base class for all analytics requests about pools
+    """A base class for analytics requests about pools.
 
-    Right now you can get analytics only about pool.
+    Attributes:
+        subject_id: The ID of a pool to get analytics about.
     """
 
     @unique
     class Subject(ExtendableStrEnum):
         REAL_TASKS_COUNT = 'real_tasks_count'
         SUBMITTED_ASSIGNMENTS_COUNT = 'submitted_assignments_count'
         SKIPPED_ASSIGNMENTS_COUNT = 'skipped_assignments_count'
@@ -63,96 +64,98 @@
         UNIQUE_SUBMITTERS_COUNT = 'unique_submitters_count'
         ACTIVE_WORKERS_BY_FILTER_COUNT = 'active_workers_by_filter_count'
         ESTIMATED_ASSIGNMENTS_COUNT = 'estimated_assignments_count'
 
 
 @inherit_docstrings
 class RealTasksCountPoolAnalytics(PoolAnalyticsRequest, spec_value=PoolAnalyticsRequest.Subject.REAL_TASKS_COUNT):
-    """The number of tasks in the pool
+    """Counts the number of general tasks in a pool.
 
-    It does not take into account the overlap, how many tasks will be on one page, or the presence of golden tasks.
+    Note, that `RealTasksCountPoolAnalytics` doesn't take into account control and training tasks, and task overlap.
     """
     pass
 
 
 @inherit_docstrings
 class SubmittedAssignmentsCountPoolAnalytics(PoolAnalyticsRequest, spec_value=PoolAnalyticsRequest.Subject.SUBMITTED_ASSIGNMENTS_COUNT):
-    """The total number of completed assignments in the pool.
+    """Counts the total number of completed assignments in a pool.
 
-    The assignments can have one of the following statuses: "submitted", "approved", or "rejected".
+    It counts assignments with the `SUBMITTED`, `ACCEPTED`, or `REJECTED` status.
     """
     pass
 
 
 @inherit_docstrings
 class SkippedAssignmentsCountPoolAnalytics(PoolAnalyticsRequest, spec_value=PoolAnalyticsRequest.Subject.SKIPPED_ASSIGNMENTS_COUNT):
-    """Number of assignments in the "skipped" status in the pool
+    """Counts the number of assignments with the `SKIPPED` status in a pool.
     """
     pass
 
 
 @inherit_docstrings
 class RejectedAssignmentsCountPoolAnalytics(PoolAnalyticsRequest, spec_value=PoolAnalyticsRequest.Subject.REJECTED_ASSIGNMENTS_COUNT):
-    """Number of assignments in the "rejected" status in the pool
+    """Counts the number of assignments with the `REJECTED` status in a pool.
     """
     pass
 
 
 @inherit_docstrings
 class ApprovedAssignmentsCountPoolAnalytics(PoolAnalyticsRequest, spec_value=PoolAnalyticsRequest.Subject.APPROVED_ASSIGNMENTS_COUNT):
-    """Number of assignments in the "approved" status in the pool
+    """Counts the number of assignments with the `ACCEPTED` status in a pool.
 
-    Do not confuse it with the submitted status.
-    "Submitted" status means that the task was completed by a Toloker and sent for review.
-    "Approved" status means that the task has passed review and money has been paid for it.
+    Do not confuse these task statuses:
+        * `SUBMITTED` tasks are completed by Tolokers and sent for a review.
+        * `ACCEPTED` tasks have passed the review and have been paid for.
     """
     pass
 
 
 @inherit_docstrings
 class CompletionPercentagePoolAnalytics(PoolAnalyticsRequest, spec_value=PoolAnalyticsRequest.Subject.COMPLETION_PERCENTAGE):
-    """Approximate percentage of completed tasks in the pool
+    """Calculates the percentage of completed tasks in a pool.
     """
     pass
 
 
 @inherit_docstrings
 class AvgSubmitAssignmentMillisPoolAnalytics(PoolAnalyticsRequest, spec_value=PoolAnalyticsRequest.Subject.AVG_SUBMIT_ASSIGNMENT_MILLIS):
-    """Average time to complete one task page in milliseconds
+    """Calculates the average time in milliseconds for completing one task suite.
     """
     pass
 
 
 @inherit_docstrings
 class SpentBudgetPoolAnalytics(PoolAnalyticsRequest, spec_value=PoolAnalyticsRequest.Subject.SPENT_BUDGET):
-    """How much money has already been spent on this pool, excluding fee
+    """Shows money spent on a pool, excluding fees.
     """
     pass
 
 
 @inherit_docstrings
 class UniqueWorkersCountPoolAnalytics(PoolAnalyticsRequest, spec_value=PoolAnalyticsRequest.Subject.UNIQUE_WORKERS_COUNT):
-    """The number of unique Tolokers who took tasks from the pool
+    """Counts the number of Tolokers who took tasks from a pool.
     """
     pass
 
 
 @inherit_docstrings
 class UniqueSubmittersCountPoolAnalytics(PoolAnalyticsRequest, spec_value=PoolAnalyticsRequest.Subject.UNIQUE_SUBMITTERS_COUNT):
-    """The number of unique Tolokers who have submitted to the pool
+    """Counts the number of Tolokers who completed at least one task suite in a pool.
     """
     pass
 
 
 @inherit_docstrings
 class ActiveWorkersByFilterCountPoolAnalytics(PoolAnalyticsRequest, spec_value=PoolAnalyticsRequest.Subject.ACTIVE_WORKERS_BY_FILTER_COUNT):
-    """The number of active Tolokers matching the pool filters for the last hours
+    """Counts the number of active Tolokers that match pool filters.
+
+    Active Tolokers are Tolokers who viewed and completed tasks recently.
 
     Attributes:
-        interval_hours: The number of hours to take into account when collecting statistics.
+        interval_hours: The interval in hours to take into account.
     """
     interval_hours: int = attribute(required=True)
 
 
 @inherit_docstrings
 class EstimatedAssignmentsCountPoolAnalytics(PoolAnalyticsRequest, spec_value=PoolAnalyticsRequest.Subject.ESTIMATED_ASSIGNMENTS_COUNT):
     """The approximate number of responses to task pages.
```

### Comparing `toloka-kit-1.1.4/src/client/analytics_request.pyi` & `toloka-kit-1.2.0/src/client/analytics_request.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 ]
 import toloka.client.primitives.base
 import toloka.util._extendable_enum
 import typing
 
 
 class AnalyticsRequest(toloka.client.primitives.base.BaseTolokaObject):
-    """Base class for all analytics requests in Toloka
+    """A base class for analytics requests.
 
-    How to use this requests and get some useful information see in example in "TolokaClient.get_analytics".
+    Make analytics requests to Toloka with the [get_analytics](toloka.client.TolokaClient.get_analytics.md) method.
 
     Attributes:
-        subject_id: ID of the object you want to get analytics about.
+        subject_id: The ID of an object to get analytics about.
     """
 
     class Subject(toloka.util._extendable_enum.ExtendableStrEnum):
         """An enumeration.
         """
 
         POOL = 'POOL'
@@ -40,20 +40,18 @@
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     subject_id: str
 
 
 class PoolAnalyticsRequest(AnalyticsRequest):
-    """Base class for all analytics requests about pools
-
-    Right now you can get analytics only about pool.
+    """A base class for analytics requests about pools.
 
     Attributes:
-        subject_id: ID of the object you want to get analytics about.
+        subject_id: The ID of a pool to get analytics about.
     """
 
     class Subject(toloka.util._extendable_enum.ExtendableStrEnum):
         """An enumeration.
         """
 
         REAL_TASKS_COUNT = 'real_tasks_count'
@@ -75,187 +73,189 @@
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     subject_id: str
 
 
 class RealTasksCountPoolAnalytics(PoolAnalyticsRequest):
-    """The number of tasks in the pool
+    """Counts the number of general tasks in a pool.
 
-    It does not take into account the overlap, how many tasks will be on one page, or the presence of golden tasks.
+    Note, that `RealTasksCountPoolAnalytics` doesn't take into account control and training tasks, and task overlap.
 
     Attributes:
-        subject_id: ID of the object you want to get analytics about.
+        subject_id: The ID of a pool to get analytics about.
     """
 
     def __init__(self, *, subject_id: str) -> None:
         """Method generated by attrs for class RealTasksCountPoolAnalytics.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     subject_id: str
 
 
 class SubmittedAssignmentsCountPoolAnalytics(PoolAnalyticsRequest):
-    """The total number of completed assignments in the pool.
+    """Counts the total number of completed assignments in a pool.
 
-    The assignments can have one of the following statuses: "submitted", "approved", or "rejected".
+    It counts assignments with the `SUBMITTED`, `ACCEPTED`, or `REJECTED` status.
 
     Attributes:
-        subject_id: ID of the object you want to get analytics about.
+        subject_id: The ID of a pool to get analytics about.
     """
 
     def __init__(self, *, subject_id: str) -> None:
         """Method generated by attrs for class SubmittedAssignmentsCountPoolAnalytics.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     subject_id: str
 
 
 class SkippedAssignmentsCountPoolAnalytics(PoolAnalyticsRequest):
-    """Number of assignments in the "skipped" status in the pool
+    """Counts the number of assignments with the `SKIPPED` status in a pool.
 
     Attributes:
-        subject_id: ID of the object you want to get analytics about.
+        subject_id: The ID of a pool to get analytics about.
     """
 
     def __init__(self, *, subject_id: str) -> None:
         """Method generated by attrs for class SkippedAssignmentsCountPoolAnalytics.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     subject_id: str
 
 
 class RejectedAssignmentsCountPoolAnalytics(PoolAnalyticsRequest):
-    """Number of assignments in the "rejected" status in the pool
+    """Counts the number of assignments with the `REJECTED` status in a pool.
 
     Attributes:
-        subject_id: ID of the object you want to get analytics about.
+        subject_id: The ID of a pool to get analytics about.
     """
 
     def __init__(self, *, subject_id: str) -> None:
         """Method generated by attrs for class RejectedAssignmentsCountPoolAnalytics.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     subject_id: str
 
 
 class ApprovedAssignmentsCountPoolAnalytics(PoolAnalyticsRequest):
-    """Number of assignments in the "approved" status in the pool
+    """Counts the number of assignments with the `ACCEPTED` status in a pool.
 
-    Do not confuse it with the submitted status.
-    "Submitted" status means that the task was completed by a Toloker and sent for review.
-    "Approved" status means that the task has passed review and money has been paid for it.
+    Do not confuse these task statuses:
+        * `SUBMITTED` tasks are completed by Tolokers and sent for a review.
+        * `ACCEPTED` tasks have passed the review and have been paid for.
 
     Attributes:
-        subject_id: ID of the object you want to get analytics about.
+        subject_id: The ID of a pool to get analytics about.
     """
 
     def __init__(self, *, subject_id: str) -> None:
         """Method generated by attrs for class ApprovedAssignmentsCountPoolAnalytics.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     subject_id: str
 
 
 class CompletionPercentagePoolAnalytics(PoolAnalyticsRequest):
-    """Approximate percentage of completed tasks in the pool
+    """Calculates the percentage of completed tasks in a pool.
 
     Attributes:
-        subject_id: ID of the object you want to get analytics about.
+        subject_id: The ID of a pool to get analytics about.
     """
 
     def __init__(self, *, subject_id: str) -> None:
         """Method generated by attrs for class CompletionPercentagePoolAnalytics.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     subject_id: str
 
 
 class AvgSubmitAssignmentMillisPoolAnalytics(PoolAnalyticsRequest):
-    """Average time to complete one task page in milliseconds
+    """Calculates the average time in milliseconds for completing one task suite.
 
     Attributes:
-        subject_id: ID of the object you want to get analytics about.
+        subject_id: The ID of a pool to get analytics about.
     """
 
     def __init__(self, *, subject_id: str) -> None:
         """Method generated by attrs for class AvgSubmitAssignmentMillisPoolAnalytics.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     subject_id: str
 
 
 class SpentBudgetPoolAnalytics(PoolAnalyticsRequest):
-    """How much money has already been spent on this pool, excluding fee
+    """Shows money spent on a pool, excluding fees.
 
     Attributes:
-        subject_id: ID of the object you want to get analytics about.
+        subject_id: The ID of a pool to get analytics about.
     """
 
     def __init__(self, *, subject_id: str) -> None:
         """Method generated by attrs for class SpentBudgetPoolAnalytics.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     subject_id: str
 
 
 class UniqueWorkersCountPoolAnalytics(PoolAnalyticsRequest):
-    """The number of unique Tolokers who took tasks from the pool
+    """Counts the number of Tolokers who took tasks from a pool.
 
     Attributes:
-        subject_id: ID of the object you want to get analytics about.
+        subject_id: The ID of a pool to get analytics about.
     """
 
     def __init__(self, *, subject_id: str) -> None:
         """Method generated by attrs for class UniqueWorkersCountPoolAnalytics.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     subject_id: str
 
 
 class UniqueSubmittersCountPoolAnalytics(PoolAnalyticsRequest):
-    """The number of unique Tolokers who have submitted to the pool
+    """Counts the number of Tolokers who completed at least one task suite in a pool.
 
     Attributes:
-        subject_id: ID of the object you want to get analytics about.
+        subject_id: The ID of a pool to get analytics about.
     """
 
     def __init__(self, *, subject_id: str) -> None:
         """Method generated by attrs for class UniqueSubmittersCountPoolAnalytics.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     subject_id: str
 
 
 class ActiveWorkersByFilterCountPoolAnalytics(PoolAnalyticsRequest):
-    """The number of active Tolokers matching the pool filters for the last hours
+    """Counts the number of active Tolokers that match pool filters.
+
+    Active Tolokers are Tolokers who viewed and completed tasks recently.
 
     Attributes:
-        subject_id: ID of the object you want to get analytics about.
-        interval_hours: The number of hours to take into account when collecting statistics.
+        subject_id: The ID of a pool to get analytics about.
+        interval_hours: The interval in hours to take into account.
     """
 
     def __init__(
         self,
         *,
         subject_id: str,
         interval_hours: int
@@ -269,15 +269,15 @@
     interval_hours: int
 
 
 class EstimatedAssignmentsCountPoolAnalytics(PoolAnalyticsRequest):
     """The approximate number of responses to task pages.
 
     Attributes:
-        subject_id: ID of the object you want to get analytics about.
+        subject_id: The ID of a pool to get analytics about.
     """
 
     def __init__(self, *, subject_id: str) -> None:
         """Method generated by attrs for class EstimatedAssignmentsCountPoolAnalytics.
         """
         ...
```

### Comparing `toloka-kit-1.1.4/src/client/app/__init__.py` & `toloka-kit-1.2.0/src/client/app/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,282 +1,284 @@
-__all__ = [
-    'AppProject',
-    'App',
-    'AppItem',
-    'AppItemsCreateRequest',
-    'AppBatch',
-    'AppBatchCreateRequest',
-    'AppBatchPatch',
-]
-import datetime
-import decimal
-from enum import unique
-from typing import Dict, Any, List
-
-from ..primitives.base import BaseTolokaObject
-from ..project.field_spec import FieldSpec
-from ...util._codegen import attribute
-from ...util._extendable_enum import ExtendableStrEnum
-
-
-class _AppError(BaseTolokaObject):
-    """
-    A structure for describing errors which may appear while working with App projects.
-
-    Attributes:
-        code: The short name of the error.
-        message: The detailed description of the error.
-        payload: Additional data provided with the error.
-    """
-    code: str
-    message: str
-    payload: Any
-
-
-class AppLightestResult(BaseTolokaObject):
-    """Brief information about the project template.
-
-    Attributes:
-        id: The ID of the App solution.
-        name: The solution name.
-    """
-    id: str
-    name: str
-
-
-class AppProject(BaseTolokaObject):
-    """An [App](https://toloka.ai/en/docs/toloka-apps/concepts/) project.
-
-    An App project is based on one of App solutions. It is created with a template interface and preconfigured data specification and quality control rules.
-
-    To get available App solutions use the [get_apps](toloka.client.TolokaClient.get_apps.md) method.
-
-    Attributes:
-        app_id: The ID of the App solution used to create the project.
-        parent_app_project_id: The ID of the parent project. It is set if this project is a clone of other project. Otherwise it is empty.
-        name: The project name.
-        parameters: Parameters of the solution. The parameters should follow the schema described in the `param_spec` field of the [solution](toloka.client.app.App.md).
-        id: The ID of the project.
-        status: The project status:
-            * `CREATING` — Toloka is checking the project.
-            * `READY` — The project is active.
-            * `ARCHIVED` — The project was archived.
-            * `ERROR` — Project creation failed due to errors.
-        created: The date and time when the project was created.
-        item_price: The price you pay for a processed item.
-        errors: Errors found during a project check.
-        read_only:
-        app: Brief information about the project template.
-    """
-
-    @unique
-    class Status(ExtendableStrEnum):
-        CREATING = 'CREATING'
-        READY = 'READY'
-        ARCHIVED = 'ARCHIVED'
-        ERROR = 'ERROR'
-
-    app_id: str
-    parent_app_project_id: str
-    name: str
-    parameters: Dict
-
-    id: str = attribute(readonly=True)
-    status: Status = attribute(readonly=True, autocast=True)
-    created: datetime.datetime = attribute(readonly=True)
-    item_price: decimal.Decimal = attribute(readonly=True)
-    errors: List[_AppError] = attribute(readonly=True)
-    read_only: bool = attribute(readonly=True)
-    app: AppLightestResult = attribute(readonly=True)
-
-
-class App(BaseTolokaObject):
-    """An [App](https://toloka.ai/en/docs/toloka-apps/concepts/) solution.
-
-    Each App solution targets specific type of tasks which can be solved using Toloka.
-
-    Attributes:
-        id: The ID of the App solution.
-        name: The solution name.
-        image: A link to the solution interface preview image.
-        description: The solution description.
-        constraints_description: The description of limitations.
-        default_item_price: The default cost of one annotated item.
-        param_spec: The specification of parameters used to create a project.
-        input_spec: The schema of solution input data.
-        output_spec: The schema of solution output data.
-        examples: Example description of tasks which can be solved with this solution.
-        input_format_info: Information about the input data format.
-    """
-
-    id: str
-    name: str
-    image: str
-    description: str
-    constraints_description: str
-    default_item_price: decimal.Decimal
-    param_spec: Dict
-    input_spec: Dict[str, FieldSpec]
-    output_spec: Dict[str, FieldSpec]
-    examples: Any
-    input_format_info: Dict
-
-
-class AppItem(BaseTolokaObject):
-    """A task item.
-
-    Items are uploaded to Toloka and are grouped in batches. After uploading the status of items is set to `NEW`. Items with that status can be edited. Then entire batches are sent for labeling.
-
-    Attributes:
-        id: The ID of the item.
-        app_project_id: The ID of the project that contains the item.
-        batch_id: The ID of the batch that contains the item.
-        input_data: Input data. It must follow the solution schema described in `App.input_spec`.
-        status: The item status:
-            * `NEW` — The item is uploaded to Toloka and ready for processing.
-            * `PROCESSING` — The item is being processed by Tolokers.
-            * `COMPLETED` — Item annotation is completed.
-            * `ERROR` — An error occurred during processing.
-            * `CANCELLED` — Item processing cancelled.
-            * `ARCHIVE` — The item is archived.
-            * `NO_MONEY` — There are not enough money for processing.
-        output_data: Annotated data.
-        errors: Errors occurred during annotation.
-        created_at: The date and time when the item was created.
-        started_at: The date and time when the item processing started.
-        finished_at: The date and time when the item processing was completed.
-    """
-
-    @unique
-    class Status(ExtendableStrEnum):
-        NEW = 'NEW'
-        PROCESSING = 'PROCESSING'
-        COMPLETED = 'COMPLETED'
-        ERROR = 'ERROR'
-        CANCELLED = 'CANCELLED'
-        ARCHIVE = 'ARCHIVE'
-        NO_MONEY = 'NO_MONEY'
-        STOPPED = 'STOPPED'
-
-    batch_id: str
-    input_data: Dict[str, Any]
-
-    id: str = attribute(readonly=True)
-    app_project_id: str = attribute(readonly=True)
-    status: Status = attribute(readonly=True, autocast=True)
-    output_data: Dict[str, Any] = attribute(readonly=True)
-    errors: List[_AppError] = attribute(readonly=True)
-    created_at: datetime.datetime = attribute(readonly=True)
-    started_at: datetime.datetime = attribute(readonly=True)
-    finished_at: datetime.datetime = attribute(readonly=True)
-
-
-class AppItemsCreateRequest(BaseTolokaObject):
-    """Parameters of a request for creating multiple items.
-
-    Attributes:
-        batch_id: The ID of the batch to place items to.
-        items: A list with items. The items must follow the solution schema described in `App.input_spec`.
-    """
-
-    batch_id: str
-    items: List[Dict[str, Any]]
-
-
-class AppItemImport(BaseTolokaObject):
-    """Meta-information on asynchronous loading operation (possible via UI).
-
-    Attributes:
-        id:
-        records_count: Number of items in the loading operation.
-        records_processed: Number of successfully loaded items in the loading operation.
-        errors: Errors during the loading operation.
-    """
-    id: str
-    records_count: int
-    records_processed: int
-    errors: Dict
-
-
-class AppBatch(BaseTolokaObject):
-    """An App batch.
-
-    A batch contains task items that are sent for labeling together.
-
-    Attributes:
-        id: The ID of the batch.
-        app_project_id: The ID of the project containing the batch.
-        name: The batch name.
-        status: The batch status:
-            * `NEW` — The processing of the batch items is not started.
-            * `PROCESSING` — Batch items are being processed by Tolokers.
-            * `COMPLETED` — Annotation of all batch items is completed.
-            * `ERROR` — An error occurred during processing.
-            * `CANCELLED` — Batch processing cancelled.
-            * `ARCHIVE` — The batch is archived.
-            * `NO_MONEY` — There are not enough money for processing.
-        items_count: The number of items in the batch.
-        item_price: The cost of processing a single item in the batch.
-        cost: The cost of processing the batch.
-        cost_of_processed: Cost of already processed task items.
-        created_at: The date and time when the batch was created.
-        started_at: The date and time when batch processing started.
-        finished_at: The date and time when batch processing was completed.
-        read_only:
-        last_items_import: Meta-information on asynchronous loading operation (possible via UI).
-        confidence_avg: Average labeling quality.
-        items_processed_count: Number of labeled items.
-        eta: Expected date and time when batch processing will be completed.
-        items_per_state: Statistics on the number of items in each state.
-    """
-
-    @unique
-    class Status(ExtendableStrEnum):
-        NEW = 'NEW'
-        PROCESSING = 'PROCESSING'
-        COMPLETED = 'COMPLETED'
-        ERROR = 'ERROR'
-        CANCELLED = 'CANCELLED'
-        NO_MONEY = 'NO_MONEY'
-        ARCHIVE = 'ARCHIVE'
-        LOADING = 'LOADING'
-        STOPPING = 'STOPPING'
-        STOPPED = 'STOPPED'
-
-    id: str
-    app_project_id: str
-    name: str
-    status: Status = attribute(autocast=True)
-    items_count: int
-    item_price: decimal.Decimal
-    cost: decimal.Decimal
-    cost_of_processed: decimal.Decimal
-    created_at: datetime.datetime
-    started_at: datetime.datetime
-    finished_at: datetime.datetime
-    read_only: bool
-    last_items_import: AppItemImport
-    confidence_avg: float
-    items_processed_count: int
-    eta: datetime.datetime
-    items_per_state: Dict
-
-
-class AppBatchCreateRequest(BaseTolokaObject):
-    """Parameters of a request for creating multiple App task items in a batch.
-
-    Attributes:
-        name: Batch name.
-        items: A list with task items. The items must follow the solution schema described in `App.input_spec`.
-    """
-
-    name: str
-    items: List[Dict[str, Any]]
-
-
-class AppBatchPatch(BaseTolokaObject):
-    """"Parameters for changing name of a specific AppBatch
-
-    Attributes:
-        name: Batch name.
-    """
-    name: str
+__all__ = [
+    'AppProject',
+    'App',
+    'AppItem',
+    'AppItemsCreateRequest',
+    'AppBatch',
+    'AppBatchCreateRequest',
+    'AppBatchPatch',
+]
+import datetime
+import decimal
+from enum import unique
+from typing import Dict, Any, List
+
+from ..primitives.base import BaseTolokaObject
+from ..project.field_spec import FieldSpec
+from ...util._codegen import attribute
+from ...util._extendable_enum import ExtendableStrEnum
+
+
+class _AppError(BaseTolokaObject):
+    """
+    A structure for describing errors which may appear while working with App projects.
+
+    Attributes:
+        code: The short name of the error.
+        message: The detailed description of the error.
+        payload: Additional data provided with the error.
+    """
+    code: str
+    message: str
+    payload: Any
+
+
+class AppLightestResult(BaseTolokaObject):
+    """Brief information about the project template.
+
+    Attributes:
+        id: The ID of the App solution.
+        name: The solution name.
+    """
+    id: str
+    name: str
+
+
+class AppProject(BaseTolokaObject):
+    """An [App](https://toloka.ai/en/docs/toloka-apps/concepts/) project.
+
+    An App project is based on one of App solutions. It is created with a template interface and preconfigured data specification and quality control rules.
+
+    To get available App solutions use the [get_apps](toloka.client.TolokaClient.get_apps.md) method.
+
+    Attributes:
+        app_id: The ID of the App solution used to create the project.
+        parent_app_project_id: The ID of the parent project. It is set if this project is a clone of other project. Otherwise it is empty.
+        name: The project name.
+        parameters: Parameters of the solution. The parameters should follow the schema described in the `param_spec` field of the [solution](toloka.client.app.App.md).
+        id: The ID of the project.
+        status: The project status:
+            * `CREATING` — Toloka is checking the project.
+            * `READY` — The project is active.
+            * `ARCHIVED` — The project was archived.
+            * `ERROR` — Project creation failed due to errors.
+        created: The date and time when the project was created.
+        item_price: The price you pay for a processed item.
+        errors: Errors found during a project check.
+        read_only:
+            * `True` — The project is read-only.
+            * `False` — The project can be modified.
+        app: Brief information about the project template.
+    """
+
+    @unique
+    class Status(ExtendableStrEnum):
+        CREATING = 'CREATING'
+        READY = 'READY'
+        ARCHIVED = 'ARCHIVED'
+        ERROR = 'ERROR'
+
+    app_id: str
+    parent_app_project_id: str
+    name: str
+    parameters: Dict
+
+    id: str = attribute(readonly=True)
+    status: Status = attribute(readonly=True, autocast=True)
+    created: datetime.datetime = attribute(readonly=True)
+    item_price: decimal.Decimal = attribute(readonly=True)
+    errors: List[_AppError] = attribute(readonly=True)
+    read_only: bool = attribute(readonly=True)
+    app: AppLightestResult = attribute(readonly=True)
+
+
+class App(BaseTolokaObject):
+    """An [App](https://toloka.ai/en/docs/toloka-apps/concepts/) solution.
+
+    Each App solution targets specific type of tasks which can be solved using Toloka.
+
+    Attributes:
+        id: The ID of the App solution.
+        name: The solution name.
+        image: A link to the solution interface preview image.
+        description: The solution description.
+        constraints_description: The description of limitations.
+        default_item_price: The default cost of one annotated item.
+        param_spec: The specification of parameters used to create a project.
+        input_spec: The schema of solution input data.
+        output_spec: The schema of solution output data.
+        examples: Example description of tasks which can be solved with this solution.
+        input_format_info: Information about the input data format.
+    """
+
+    id: str
+    name: str
+    image: str
+    description: str
+    constraints_description: str
+    default_item_price: decimal.Decimal
+    param_spec: Dict
+    input_spec: Dict[str, FieldSpec]
+    output_spec: Dict[str, FieldSpec]
+    examples: Any
+    input_format_info: Dict
+
+
+class AppItem(BaseTolokaObject):
+    """A task item.
+
+    Items are uploaded to Toloka and are grouped in batches. After uploading the status of items is set to `NEW`. Items with that status can be edited. Then entire batches are sent for labeling.
+
+    Attributes:
+        id: The ID of the item.
+        app_project_id: The ID of the project that contains the item.
+        batch_id: The ID of the batch that contains the item.
+        input_data: Input data. It must follow the solution schema described in `App.input_spec`.
+        status: The item status:
+            * `NEW` — The item is uploaded to Toloka and ready for processing.
+            * `PROCESSING` — The item is being processed by Tolokers.
+            * `COMPLETED` — Item annotation is completed.
+            * `ERROR` — An error occurred during processing.
+            * `CANCELLED` — Item processing cancelled.
+            * `ARCHIVE` — The item is archived.
+            * `NO_MONEY` — There are not enough money for processing.
+        output_data: Annotated data.
+        errors: Errors occurred during annotation.
+        created_at: The date and time when the item was created.
+        started_at: The date and time when the item processing started.
+        finished_at: The date and time when the item processing was completed.
+    """
+
+    @unique
+    class Status(ExtendableStrEnum):
+        NEW = 'NEW'
+        PROCESSING = 'PROCESSING'
+        COMPLETED = 'COMPLETED'
+        ERROR = 'ERROR'
+        CANCELLED = 'CANCELLED'
+        ARCHIVE = 'ARCHIVE'
+        NO_MONEY = 'NO_MONEY'
+        STOPPED = 'STOPPED'
+
+    batch_id: str
+    input_data: Dict[str, Any]
+
+    id: str = attribute(readonly=True)
+    app_project_id: str = attribute(readonly=True)
+    status: Status = attribute(readonly=True, autocast=True)
+    output_data: Dict[str, Any] = attribute(readonly=True)
+    errors: List[_AppError] = attribute(readonly=True)
+    created_at: datetime.datetime = attribute(readonly=True)
+    started_at: datetime.datetime = attribute(readonly=True)
+    finished_at: datetime.datetime = attribute(readonly=True)
+
+
+class AppItemsCreateRequest(BaseTolokaObject):
+    """Parameters of a request for creating multiple items.
+
+    Attributes:
+        batch_id: The ID of the batch to place items to.
+        items: A list with items. The items must follow the solution schema described in `App.input_spec`.
+    """
+
+    batch_id: str
+    items: List[Dict[str, Any]]
+
+
+class AppItemImport(BaseTolokaObject):
+    """Meta-information on asynchronous loading operation (possible via UI).
+
+    Attributes:
+        id:
+        records_count: The number of items in the loading operation.
+        records_processed: The number of successfully loaded items in the loading operation.
+        errors: Errors during the loading operation.
+    """
+    id: str
+    records_count: int
+    records_processed: int
+    errors: Dict
+
+
+class AppBatch(BaseTolokaObject):
+    """An App batch.
+
+    A batch contains task items that are sent for labeling together.
+
+    Attributes:
+        id: The ID of the batch.
+        app_project_id: The ID of the project containing the batch.
+        name: The batch name.
+        status: The batch status:
+            * `NEW` — The processing of the batch items is not started.
+            * `PROCESSING` — Batch items are being processed by Tolokers.
+            * `COMPLETED` — Annotation of all batch items is completed.
+            * `ERROR` — An error occurred during processing.
+            * `CANCELLED` — Batch processing cancelled.
+            * `ARCHIVE` — The batch is archived.
+            * `NO_MONEY` — There are not enough money for processing.
+        items_count: The number of items in the batch.
+        item_price: The cost of processing a single item in the batch.
+        cost: The cost of processing the batch.
+        cost_of_processed: Cost of already processed task items.
+        created_at: The date and time when the batch was created.
+        started_at: The date and time when batch processing started.
+        finished_at: The date and time when batch processing was completed.
+        read_only:
+        last_items_import: Meta-information on asynchronous loading operation (possible via UI).
+        confidence_avg: Average labeling quality.
+        items_processed_count: The number of labeled items.
+        eta: Expected date and time when batch processing will be completed.
+        items_per_state: Statistics on the number of items in each state.
+    """
+
+    @unique
+    class Status(ExtendableStrEnum):
+        NEW = 'NEW'
+        PROCESSING = 'PROCESSING'
+        COMPLETED = 'COMPLETED'
+        ERROR = 'ERROR'
+        CANCELLED = 'CANCELLED'
+        NO_MONEY = 'NO_MONEY'
+        ARCHIVE = 'ARCHIVE'
+        LOADING = 'LOADING'
+        STOPPING = 'STOPPING'
+        STOPPED = 'STOPPED'
+
+    id: str
+    app_project_id: str
+    name: str
+    status: Status = attribute(autocast=True)
+    items_count: int
+    item_price: decimal.Decimal
+    cost: decimal.Decimal
+    cost_of_processed: decimal.Decimal
+    created_at: datetime.datetime
+    started_at: datetime.datetime
+    finished_at: datetime.datetime
+    read_only: bool
+    last_items_import: AppItemImport
+    confidence_avg: float
+    items_processed_count: int
+    eta: datetime.datetime
+    items_per_state: Dict
+
+
+class AppBatchCreateRequest(BaseTolokaObject):
+    """Parameters of a request for creating multiple App task items in a batch.
+
+    Attributes:
+        name: The batch name.
+        items: A list with task items. The items must follow the solution schema described in the `App.input_spec`.
+    """
+
+    name: str
+    items: List[Dict[str, Any]]
+
+
+class AppBatchPatch(BaseTolokaObject):
+    """Parameters of a request for updating an App batch.
+
+    Attributes:
+        name: The new batch name.
+    """
+    name: str
```

### Comparing `toloka-kit-1.1.4/src/client/app/__init__.pyi` & `toloka-kit-1.2.0/src/client/app/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -82,14 +82,16 @@
             * `READY` — The project is active.
             * `ARCHIVED` — The project was archived.
             * `ERROR` — Project creation failed due to errors.
         created: The date and time when the project was created.
         item_price: The price you pay for a processed item.
         errors: Errors found during a project check.
         read_only:
+            * `True` — The project is read-only.
+            * `False` — The project can be modified.
         app: Brief information about the project template.
     """
 
     class Status(toloka.util._extendable_enum.ExtendableStrEnum):
         """An enumeration.
         """
 
@@ -276,16 +278,16 @@
 
 
 class AppItemImport(toloka.client.primitives.base.BaseTolokaObject):
     """Meta-information on asynchronous loading operation (possible via UI).
 
     Attributes:
         id:
-        records_count: Number of items in the loading operation.
-        records_processed: Number of successfully loaded items in the loading operation.
+        records_count: The number of items in the loading operation.
+        records_processed: The number of successfully loaded items in the loading operation.
         errors: Errors during the loading operation.
     """
 
     def __init__(
         self,
         *,
         id: typing.Optional[str] = None,
@@ -327,15 +329,15 @@
         cost_of_processed: Cost of already processed task items.
         created_at: The date and time when the batch was created.
         started_at: The date and time when batch processing started.
         finished_at: The date and time when batch processing was completed.
         read_only:
         last_items_import: Meta-information on asynchronous loading operation (possible via UI).
         confidence_avg: Average labeling quality.
-        items_processed_count: Number of labeled items.
+        items_processed_count: The number of labeled items.
         eta: Expected date and time when batch processing will be completed.
         items_per_state: Statistics on the number of items in each state.
     """
 
     class Status(toloka.util._extendable_enum.ExtendableStrEnum):
         """An enumeration.
         """
@@ -396,16 +398,16 @@
     items_per_state: typing.Optional[typing.Dict]
 
 
 class AppBatchCreateRequest(toloka.client.primitives.base.BaseTolokaObject):
     """Parameters of a request for creating multiple App task items in a batch.
 
     Attributes:
-        name: Batch name.
-        items: A list with task items. The items must follow the solution schema described in `App.input_spec`.
+        name: The batch name.
+        items: A list with task items. The items must follow the solution schema described in the `App.input_spec`.
     """
 
     def __init__(
         self,
         *,
         name: typing.Optional[str] = None,
         items: typing.Optional[typing.List[typing.Dict[str, typing.Any]]] = None
@@ -416,18 +418,18 @@
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     name: typing.Optional[str]
     items: typing.Optional[typing.List[typing.Dict[str, typing.Any]]]
 
 
 class AppBatchPatch(toloka.client.primitives.base.BaseTolokaObject):
-    """"Parameters for changing name of a specific AppBatch
+    """Parameters of a request for updating an App batch.
 
     Attributes:
-        name: Batch name.
+        name: The new batch name.
     """
 
     def __init__(self, *, name: typing.Optional[str] = None) -> None:
         """Method generated by attrs for class AppBatchPatch.
         """
         ...
```

### Comparing `toloka-kit-1.1.4/src/client/assignment.py` & `toloka-kit-1.2.0/src/client/assignment.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/assignment.pyi` & `toloka-kit-1.2.0/src/client/assignment.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/attachment.py` & `toloka-kit-1.2.0/src/client/attachment.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,62 @@
-__all__ = [
-    'Attachment',
-    'AssignmentAttachment'
-]
-
-import datetime
-from enum import unique
-
-from .owner import Owner
-from .primitives.base import BaseTolokaObject
-from ..util._docstrings import inherit_docstrings
-from ..util._extendable_enum import ExtendableStrEnum
-
-
-class Attachment(BaseTolokaObject, spec_enum='Type', spec_field='attachment_type'):
-    """Attachment
-
-    Files uploaded by Tolokers are saved in Toloka.
-    Attributes:
-        id: File ID.
-        name: File name.
-        details: Information about the pool, the task, and the Toloker who uploaded the file.
-        created: Date the file was uploaded to Toloka.
-        media_type: MIME data type.
-        owner: Owner
-    """
-
-    @unique
-    class Type(ExtendableStrEnum):
-        ASSIGNMENT_ATTACHMENT = 'ASSIGNMENT_ATTACHMENT'
-
-    ASSIGNMENT_ATTACHMENT = Type.ASSIGNMENT_ATTACHMENT
-
-    class Details(BaseTolokaObject):
-        """Information about the pool, task, and the Toloker from which the file was received.
-
-        Attributes:
-            user_id: ID of the Toloker from whom the file was received.
-            assignment_id: ID for issuing a set of tasks to the Toloker.
-            pool_id: Pool ID.
-        """
-
-        user_id: str
-        assignment_id: str
-        pool_id: str
-
-    id: str
-    name: str
-    details: Details
-    created: datetime.datetime
-    media_type: str
-
-    owner: Owner
-
-
-@inherit_docstrings
-class AssignmentAttachment(Attachment, spec_value=Attachment.Type.ASSIGNMENT_ATTACHMENT):
-    """Assignment Attachment.
-    """
-
-    pass
+__all__ = [
+    'Attachment',
+    'AssignmentAttachment'
+]
+
+import datetime
+from enum import unique
+
+from .owner import Owner
+from .primitives.base import BaseTolokaObject
+from ..util._docstrings import inherit_docstrings
+from ..util._extendable_enum import ExtendableStrEnum
+
+
+class Attachment(BaseTolokaObject, spec_enum='Type', spec_field='attachment_type'):
+    """An attachment.
+
+    Files attached to tasks by Tolokers are uploaded to Toloka.
+
+    Attributes:
+        id: The file ID.
+        name: The file name.
+        details: Attachment details: a pool, task, and Toloker who uploaded the file.
+        created: The date and time when the file was uploaded.
+        media_type: The file [MIME](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types) data type.
+        owner: The owner of the attachment.
+    """
+
+    @unique
+    class Type(ExtendableStrEnum):
+        ASSIGNMENT_ATTACHMENT = 'ASSIGNMENT_ATTACHMENT'
+
+    ASSIGNMENT_ATTACHMENT = Type.ASSIGNMENT_ATTACHMENT
+
+    class Details(BaseTolokaObject):
+        """Attachment details.
+
+        Attributes:
+            user_id: The ID of the Toloker who attached the file.
+            assignment_id: The ID of the assignment with the file.
+            pool_id: The ID of the pool.
+        """
+
+        user_id: str
+        assignment_id: str
+        pool_id: str
+
+    id: str
+    name: str
+    details: Details
+    created: datetime.datetime
+    media_type: str
+
+    owner: Owner
+
+
+@inherit_docstrings
+class AssignmentAttachment(Attachment, spec_value=Attachment.Type.ASSIGNMENT_ATTACHMENT):
+    """An attachment to an assignment.
+    """
+
+    pass
```

### Comparing `toloka-kit-1.1.4/src/client/attachment.pyi` & `toloka-kit-1.2.0/src/client/attachment.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -6,39 +6,40 @@
 import toloka.client.owner
 import toloka.client.primitives.base
 import toloka.util._extendable_enum
 import typing
 
 
 class Attachment(toloka.client.primitives.base.BaseTolokaObject):
-    """Attachment
+    """An attachment.
+
+    Files attached to tasks by Tolokers are uploaded to Toloka.
 
-    Files uploaded by Tolokers are saved in Toloka.
     Attributes:
-        id: File ID.
-        name: File name.
-        details: Information about the pool, the task, and the Toloker who uploaded the file.
-        created: Date the file was uploaded to Toloka.
-        media_type: MIME data type.
-        owner: Owner
+        id: The file ID.
+        name: The file name.
+        details: Attachment details: a pool, task, and Toloker who uploaded the file.
+        created: The date and time when the file was uploaded.
+        media_type: The file [MIME](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types) data type.
+        owner: The owner of the attachment.
     """
 
     class Type(toloka.util._extendable_enum.ExtendableStrEnum):
         """An enumeration.
         """
 
         ASSIGNMENT_ATTACHMENT = 'ASSIGNMENT_ATTACHMENT'
 
     class Details(toloka.client.primitives.base.BaseTolokaObject):
-        """Information about the pool, task, and the Toloker from which the file was received.
+        """Attachment details.
 
         Attributes:
-            user_id: ID of the Toloker from whom the file was received.
-            assignment_id: ID for issuing a set of tasks to the Toloker.
-            pool_id: Pool ID.
+            user_id: The ID of the Toloker who attached the file.
+            assignment_id: The ID of the assignment with the file.
+            pool_id: The ID of the pool.
         """
 
         def __init__(
             self,
             *,
             user_id: typing.Optional[str] = None,
             assignment_id: typing.Optional[str] = None,
@@ -73,23 +74,23 @@
     details: typing.Optional[Details]
     created: typing.Optional[datetime.datetime]
     media_type: typing.Optional[str]
     owner: typing.Optional[toloka.client.owner.Owner]
 
 
 class AssignmentAttachment(Attachment):
-    """Assignment Attachment.
+    """An attachment to an assignment.
 
     Attributes:
-        id: File ID.
-        name: File name.
-        details: Information about the pool, the task, and the Toloker who uploaded the file.
-        created: Date the file was uploaded to Toloka.
-        media_type: MIME data type.
-        owner: Owner
+        id: The file ID.
+        name: The file name.
+        details: Attachment details: a pool, task, and Toloker who uploaded the file.
+        created: The date and time when the file was uploaded.
+        media_type: The file [MIME](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types) data type.
+        owner: The owner of the attachment.
     """
 
     def __init__(
         self,
         *,
         id: typing.Optional[str] = None,
         name: typing.Optional[str] = None,
```

### Comparing `toloka-kit-1.1.4/src/client/batch_create_results.pyi` & `toloka-kit-1.2.0/src/client/batch_create_results.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 import toloka.client.task_suite
 import toloka.client.user_bonus
 import toloka.client.webhook_subscription
 import typing
 
 
 class FieldValidationError(toloka.client.primitives.base.BaseTolokaObject):
-    """Error that contains information about an invalid field.
+    """An error that contains information about an invalid field.
 
     Attributes:
-        code: An error code.
-        message: An error message.
-        params: Additional parameters describing the error.
+        code: The error code.
+        message: The error message.
+        params: A list with additional parameters describing the error.
     """
 
     def __init__(
         self,
         *,
         code: typing.Optional[str] = None,
         message: typing.Optional[str] = None,
@@ -36,19 +36,21 @@
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     code: typing.Optional[str]
     message: typing.Optional[str]
     params: typing.Optional[typing.List[typing.Any]]
 
 
 class TaskBatchCreateResult(toloka.client.primitives.base.BaseTolokaObject):
-    """The results of the tasks creation operation.
+    """The result of a task creation.
+
+    `TaskBatchCreateResult` is returned by the [create_tasks](toloka.client.TolokaClient.create_tasks.md) method.
 
     Attributes:
-        items: A list of created tasks.
-        validation_errors: A list with validation errors in input tasks. The list is filled if the request parameter `skip_invalid_items` is `True`.
+        items: A dictionary with created tasks. The indexes of a `create_tasks` input list are used as keys in the dictionary.
+        validation_errors: A dictionary with validation errors in input tasks. It is filled if the request parameter `skip_invalid_items` is `True`.
     """
 
     def __init__(
         self,
         *,
         items: typing.Optional[typing.Dict[str, toloka.client.task.Task]] = None,
         validation_errors: typing.Optional[typing.Dict[str, typing.Dict[str, FieldValidationError]]] = None
@@ -59,19 +61,21 @@
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     items: typing.Optional[typing.Dict[str, toloka.client.task.Task]]
     validation_errors: typing.Optional[typing.Dict[str, typing.Dict[str, FieldValidationError]]]
 
 
 class TaskSuiteBatchCreateResult(toloka.client.primitives.base.BaseTolokaObject):
-    """The results of the task suites creation operation.
+    """The result of a task suite creation.
+
+    `TaskSuiteBatchCreateResult` is returned by the [create_task_suites](toloka.client.TolokaClient.create_task_suites.md) method.
 
     Attributes:
-        items: A list of created task suites.
-        validation_errors: A list with validation errors in input task suites. The list is filled if the request parameter `skip_invalid_items` is `True`.
+        items: A dictionary with created task suites. The indexes of a `create_task_suites` input list are used as keys in the dictionary.
+        validation_errors: A dictionary with validation errors in input task suites. It is filled if the request parameter `skip_invalid_items` is `True`.
     """
 
     def __init__(
         self,
         *,
         items: typing.Optional[typing.Dict[str, toloka.client.task_suite.TaskSuite]] = None,
         validation_errors: typing.Optional[typing.Dict[str, typing.Dict[str, FieldValidationError]]] = None
@@ -82,19 +86,21 @@
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     items: typing.Optional[typing.Dict[str, toloka.client.task_suite.TaskSuite]]
     validation_errors: typing.Optional[typing.Dict[str, typing.Dict[str, FieldValidationError]]]
 
 
 class UserBonusBatchCreateResult(toloka.client.primitives.base.BaseTolokaObject):
-    """The results of the creating rewards for Tolokers.
+    """The result of issuing rewards for Tolokers.
+
+    `UserBonusBatchCreateResult` is returned by the [create_user_bonuses](toloka.client.TolokaClient.create_user_bonuses.md) method.
 
     Attributes:
-        items: A list of created rewards.
-        validation_errors: A list with validation errors. The list is filled if the request parameter `skip_invalid_items` is `True`.
+        items: A dictionary with created rewards. The indexes of a `create_user_bonuses` input list are used as keys in the dictionary.
+        validation_errors: A dictionary with validation errors. It is filled if the request parameter `skip_invalid_items` is `True`.
     """
 
     def __init__(
         self,
         *,
         items: typing.Optional[typing.Dict[str, toloka.client.user_bonus.UserBonus]] = None,
         validation_errors: typing.Optional[typing.Dict[str, typing.Dict[str, FieldValidationError]]] = None
@@ -105,19 +111,21 @@
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     items: typing.Optional[typing.Dict[str, toloka.client.user_bonus.UserBonus]]
     validation_errors: typing.Optional[typing.Dict[str, typing.Dict[str, FieldValidationError]]]
 
 
 class WebhookSubscriptionBatchCreateResult(toloka.client.primitives.base.BaseTolokaObject):
-    """A list with the results of the webhook-subscriptions creation operation.
+    """The result of creating webhook subscriptions.
+
+    `WebhookSubscriptionBatchCreateResult` is returned by the [upsert_webhook_subscriptions](toloka.client.TolokaClient.upsert_webhook_subscriptions.md) method.
 
     Attributes:
-        items: Object with created webhook-subscriptions.
-        validation_errors: Object with validation errors.
+        items: A dictionary with created subscriptions. The indexes of a `upsert_webhook_subscriptions` input list are used as keys in the dictionary.
+        validation_errors: A dictionary with validation errors.
     """
 
     def __init__(
         self,
         *,
         items: typing.Optional[typing.Dict[str, toloka.client.webhook_subscription.WebhookSubscription]] = None,
         validation_errors: typing.Optional[typing.Dict[str, typing.Dict[str, FieldValidationError]]] = None
```

### Comparing `toloka-kit-1.1.4/src/client/clone_results.pyi` & `toloka-kit-1.2.0/src/client/clone_results.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 import toloka.client.pool
 import toloka.client.project
 import toloka.client.training
 import typing
 
 
 class CloneResults(tuple):
-    """Objects created as a result of deep cloning of the project
+    """The result of a project deep cloning.
+
+    `CloneResults` is returned by the [clone_project](toloka.client.TolokaClient.clone_project.md) method.
 
     Attributes:
-        project (Project): New project
-        pools (List[Pool]): New pools. Can be empty.
-        trainings (List[Training]): New trainings. Can be empty.
+        project: The cloned project.
+        pools: A list of cloned pools.
+        trainings: A list of cloned trainings.
     """
 
     @staticmethod
     def __new__(
         _cls,
         project: toloka.client.project.Project,
         pools: typing.List[toloka.client.pool.Pool],
```

### Comparing `toloka-kit-1.1.4/src/client/collectors.py` & `toloka-kit-1.2.0/src/client/collectors.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/collectors.pyi` & `toloka-kit-1.2.0/src/client/collectors.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/conditions.py` & `toloka-kit-1.2.0/src/client/conditions.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/conditions.pyi` & `toloka-kit-1.2.0/src/client/conditions.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/error_codes.py` & `toloka-kit-1.2.0/src/client/error_codes.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 __all__ = [
     'CommonErrorCodes',
     'InternalErrorCodes',
-    'ValidationErrorCodes'
+    'ValidationErrorCodes',
 ]
-from enum import Enum, unique
+import enum
 
 
-@unique
-class CommonErrorCodes(Enum):
-    """Types of error codes returned by the API
+class CommonErrorCodes(enum.Enum):
+    """Common error codes returned by Toloka.
     """
 
     ACCESS_DENIED = 'ACCESS_DENIED'
     AUTHENTICATION_ERROR = 'AUTHENTICATION_ERROR'
     CONFLICT_STATE = 'CONFLICT_STATE'
     DOES_NOT_EXIST = 'DOES_NOT_EXIST'
     INTERNAL_ERROR = 'INTERNAL_ERROR'
     REMOTE_SERVICE_UNAVAILABLE = 'REMOTE_SERVICE_UNAVAILABLE'
     TOO_MANY_REQUESTS = 'TOO_MANY_REQUESTS'
     VALIDATION_ERROR = 'VALIDATION_ERROR'
 
 
-@unique
-class InternalErrorCodes(Enum):
-    """Types of internal error codes returned by the API
+class InternalErrorCodes(enum.Enum):
+    """Internal error codes returned by Toloka.
     """
 
     ACCOUNT_ALREADY_USED = 'ACCOUNT_ALREADY_USED'
     ACCOUNT_MUST_BE_IDENTIFIED = 'ACCOUNT_MUST_BE_IDENTIFIED'
     ADJUSTER_NOT_FOUND = 'ADJUSTER_NOT_FOUND'
     ALL_ASSIGNMENTS_EXHAUSTED = 'ALL_ASSIGNMENTS_EXHAUSTED'
     ASSIGNMENTS_AGGREGATION_DENIED = 'ASSIGNMENTS_AGGREGATION_DENIED'
@@ -82,24 +80,22 @@
     UNABLE_TO_UPLOAD_FILE = 'UNABLE_TO_UPLOAD_FILE'
     UNARCHIVED_POOLS_CONFLICT = 'UNARCHIVED_POOLS_CONFLICT'
     UNSUPPORTED_ALGORITHM = 'UNSUPPORTED_ALGORITHM'
     UNSUPPORTED_REGION = 'UNSUPPORTED_REGION'
     USER_ALREADY_REGISTERED = 'USER_ALREADY_REGISTERED'
     USER_HAS_PDD_ALIAS = 'USER_HAS_PDD_ALIAS'
     WITHDRAWAL_TRANSACTION_CANNOT_BE_CANCELLED = 'WITHDRAWAL_TRANSACTION_CANNOT_BE_CANCELLED'
-    WITHDRAWAL_TRANSACTION_CANNOT_BE_CANCELLED_DUE_TO_TIME_LIMIT = \
-        'WITHDRAWAL_TRANSACTION_CANNOT_BE_CANCELLED_DUE_TO_TIME_LIMIT'
+    WITHDRAWAL_TRANSACTION_CANNOT_BE_CANCELLED_DUE_TO_TIME_LIMIT = 'WITHDRAWAL_TRANSACTION_CANNOT_BE_CANCELLED_DUE_TO_TIME_LIMIT'
     WORKER_SKILL_EXISTS = 'WORKER_SKILL_EXISTS'
     WRONG_FILE_FORMAT = 'WRONG_FILE_FORMAT'
     WRONG_REVISION = 'WRONG_REVISION'
 
 
-@unique
-class ValidationErrorCodes(Enum):
-    """Types of validation error codes returned by the API
+class ValidationErrorCodes(enum.Enum):
+    """Validation error codes returned by Toloka.
     """
 
     ARRAY_EXPECTED = 'ARRAY_EXPECTED'
     ARRAY_SIZE_GREATER_THAN_MAX = 'ARRAY_SIZE_GREATER_THAN_MAX'
     ARRAY_SIZE_LESS_THAN_MIN = 'ARRAY_SIZE_LESS_THAN_MIN'
     ARRAY_SIZE_OUT_OF_BOUNDS = 'ARRAY_SIZE_OUT_OF_BOUNDS'
     BLANK_STRING_NOT_ALLOWED = 'BLANK_STRING_NOT_ALLOWED'
```

### Comparing `toloka-kit-1.1.4/src/client/error_codes.pyi` & `toloka-kit-1.2.0/src/client/error_codes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,136 +1,140 @@
-__all__ = [
-    'CommonErrorCodes',
-    'InternalErrorCodes',
-    'ValidationErrorCodes',
-]
-import enum
-
-
-class CommonErrorCodes(enum.Enum):
-    """Types of error codes returned by the API
-    """
-
-    ACCESS_DENIED = 'ACCESS_DENIED'
-    AUTHENTICATION_ERROR = 'AUTHENTICATION_ERROR'
-    CONFLICT_STATE = 'CONFLICT_STATE'
-    DOES_NOT_EXIST = 'DOES_NOT_EXIST'
-    INTERNAL_ERROR = 'INTERNAL_ERROR'
-    REMOTE_SERVICE_UNAVAILABLE = 'REMOTE_SERVICE_UNAVAILABLE'
-    TOO_MANY_REQUESTS = 'TOO_MANY_REQUESTS'
-    VALIDATION_ERROR = 'VALIDATION_ERROR'
-
-
-class InternalErrorCodes(enum.Enum):
-    """Types of internal error codes returned by the API
-    """
-
-    ACCOUNT_ALREADY_USED = 'ACCOUNT_ALREADY_USED'
-    ACCOUNT_MUST_BE_IDENTIFIED = 'ACCOUNT_MUST_BE_IDENTIFIED'
-    ADJUSTER_NOT_FOUND = 'ADJUSTER_NOT_FOUND'
-    ALL_ASSIGNMENTS_EXHAUSTED = 'ALL_ASSIGNMENTS_EXHAUSTED'
-    ASSIGNMENTS_AGGREGATION_DENIED = 'ASSIGNMENTS_AGGREGATION_DENIED'
-    ASSIGNMENTS_COUNT_CONFLICT = 'ASSIGNMENTS_COUNT_CONFLICT'
-    BATCH_INITIALIZATION_ERROR = 'BATCH_INITIALIZATION_ERROR'
-    BATCH_REJECTED = 'BATCH_REJECTED'
-    BILLING_NOT_SYNCHRONIZED = 'BILLING_NOT_SYNCHRONIZED'
-    CAPTCHA_REQUIRED = 'CAPTCHA_REQUIRED'
-    DELETE_ALL_TASKS_CONFLICT = 'DELETE_ALL_TASKS_CONFLICT'
-    EMPTY_POOL = 'EMPTY_POOL'
-    INAPPROPRIATE_STATUS = 'INAPPROPRIATE_STATUS'
-    INCORRECT_RECIPIENTS = 'INCORRECT_RECIPIENTS'
-    INVALID_OPERATION_TYPE = 'INVALID_OPERATION_TYPE'
-    INVALID_REFERRAL_CODE = 'INVALID_REFERRAL_CODE'
-    INVALID_WORKER_STATUS_ERROR = 'INVALID_WORKER_STATUS_ERROR'
-    MIXER_CONFIG_REQUIRED = 'MIXER_CONFIG_REQUIRED'
-    NEED_PHONE_CONFIRMATION = 'NEED_PHONE_CONFIRMATION'
-    NOT_ENOUGH_BALANCE = 'NOT_ENOUGH_BALANCE'
-    OAUTH_AUTHENTICATION_ERROR = 'OAUTH_AUTHENTICATION_ERROR'
-    OPERATION_ALREADY_EXISTS = 'OPERATION_ALREADY_EXISTS'
-    OPERATION_EXECUTION_ERROR = 'OPERATION_EXECUTION_ERROR'
-    OPERATION_LOGS_ARCHIVED = 'OPERATION_LOGS_ARCHIVED'
-    PAYONEER_ACCOUNT_NOT_ACTIVE = 'PAYONEER_ACCOUNT_NOT_ACTIVE'
-    PAYPAL_AUTH_CODE_INVALID = 'PAYPAL_AUTH_CODE_INVALID'
-    PAYPAL_UNVERIFIED_USER = 'PAYPAL_UNVERIFIED_USER'
-    POOL_ASSIGNMENTS_COUNT_EXCEEDED = 'POOL_ASSIGNMENTS_COUNT_EXCEEDED'
-    POOL_ASSIGNMENTS_EXHAUSTED = 'POOL_ASSIGNMENTS_EXHAUSTED'
-    POOL_INAPPROPRIATE_STATUS = 'POOL_INAPPROPRIATE_STATUS'
-    POOL_INVALID_FILTER_FOR_MAP_ISSUING = 'POOL_INVALID_FILTER_FOR_MAP_ISSUING'
-    POOL_IS_TRAINING = 'POOL_IS_TRAINING'
-    POOL_LOCKED_BY_ANOTHER_OPERATION = 'POOL_LOCKED_BY_ANOTHER_OPERATION'
-    POOL_TASKS_COUNT_EXCEEDED = 'POOL_TASKS_COUNT_EXCEEDED'
-    POOL_TASK_SUITES_COUNT_EXCEEDED = 'POOL_TASK_SUITES_COUNT_EXCEEDED'
-    POOL_TASK_TYPE_CONFLICT = 'POOL_TASK_TYPE_CONFLICT'
-    PROJECT_INAPPROPRIATE_STATUS = 'PROJECT_INAPPROPRIATE_STATUS'
-    RESULTS_EXPIRED = 'RESULTS_EXPIRED'
-    SECURE_PHONE_DUPLICATION = 'SECURE_PHONE_DUPLICATION'
-    SECURE_PHONE_MISSING = 'SECURE_PHONE_MISSING'
-    SECURE_PHONE_WAS_CHANGED = 'SECURE_PHONE_WAS_CHANGED'
-    SKILL_IS_TRAINING = 'SKILL_IS_TRAINING'
-    SKILL_IS_USED = 'SKILL_IS_USED'
-    SKILL_IS_USED_BY_PROJECTS = 'SKILL_IS_USED_BY_PROJECTS'
-    SKILL_REMOVED = 'SKILL_REMOVED'
-    SUBMITTED_ASSIGNMENTS_CONFLICT = 'SUBMITTED_ASSIGNMENTS_CONFLICT'
-    SYNC_POOL_CLONE_ERROR = 'SYNC_POOL_CLONE_ERROR'
-    SYSTEM_SCOPE_MODIFICATION = 'SYSTEM_SCOPE_MODIFICATION'
-    TASK_VALIDATION_ERROR = 'TASK_VALIDATION_ERROR'
-    THERE_IS_ACTIVE_ASSIGNMENT = 'THERE_IS_ACTIVE_ASSIGNMENT'
-    THERE_IS_REJECTED_ASSIGNMENT = 'THERE_IS_REJECTED_ASSIGNMENT'
-    TOO_MANY_ACTIVE_ASSIGNMENTS = 'TOO_MANY_ACTIVE_ASSIGNMENTS'
-    TRAINING_ARCHIVE_CONFLICT = 'TRAINING_ARCHIVE_CONFLICT'
-    UNABLE_TO_UPLOAD_FILE = 'UNABLE_TO_UPLOAD_FILE'
-    UNARCHIVED_POOLS_CONFLICT = 'UNARCHIVED_POOLS_CONFLICT'
-    UNSUPPORTED_ALGORITHM = 'UNSUPPORTED_ALGORITHM'
-    UNSUPPORTED_REGION = 'UNSUPPORTED_REGION'
-    USER_ALREADY_REGISTERED = 'USER_ALREADY_REGISTERED'
-    USER_HAS_PDD_ALIAS = 'USER_HAS_PDD_ALIAS'
-    WITHDRAWAL_TRANSACTION_CANNOT_BE_CANCELLED = 'WITHDRAWAL_TRANSACTION_CANNOT_BE_CANCELLED'
-    WITHDRAWAL_TRANSACTION_CANNOT_BE_CANCELLED_DUE_TO_TIME_LIMIT = 'WITHDRAWAL_TRANSACTION_CANNOT_BE_CANCELLED_DUE_TO_TIME_LIMIT'
-    WORKER_SKILL_EXISTS = 'WORKER_SKILL_EXISTS'
-    WRONG_FILE_FORMAT = 'WRONG_FILE_FORMAT'
-    WRONG_REVISION = 'WRONG_REVISION'
-
-
-class ValidationErrorCodes(enum.Enum):
-    """Types of validation error codes returned by the API
-    """
-
-    ARRAY_EXPECTED = 'ARRAY_EXPECTED'
-    ARRAY_SIZE_GREATER_THAN_MAX = 'ARRAY_SIZE_GREATER_THAN_MAX'
-    ARRAY_SIZE_LESS_THAN_MIN = 'ARRAY_SIZE_LESS_THAN_MIN'
-    ARRAY_SIZE_OUT_OF_BOUNDS = 'ARRAY_SIZE_OUT_OF_BOUNDS'
-    BLANK_STRING_NOT_ALLOWED = 'BLANK_STRING_NOT_ALLOWED'
-    BOOLEAN_EXPECTED = 'BOOLEAN_EXPECTED'
-    CHARACTER_NOT_ALLOWED = 'CHARACTER_NOT_ALLOWED'
-    DATE_OUT_OF_RANGE = 'DATE_OUT_OF_RANGE'
-    DUPLICATE_VALUE_IN_ARRAY = 'DUPLICATE_VALUE_IN_ARRAY'
-    EMPTY_OBJECT_NOT_ALLOWED = 'EMPTY_OBJECT_NOT_ALLOWED'
-    ENTITY_ACCESS_DENIED = 'ENTITY_ACCESS_DENIED'
-    ENTITY_DOES_NOT_EXIST = 'ENTITY_DOES_NOT_EXIST'
-    FLOAT_EXPECTED = 'FLOAT_EXPECTED'
-    INTEGER_EXPECTED = 'INTEGER_EXPECTED'
-    INVALID_COORDINATES_SYNTAX = 'INVALID_COORDINATES_SYNTAX'
-    INVALID_DATE_SYNTAX = 'INVALID_DATE_SYNTAX'
-    INVALID_DATE_TIME_SYNTAX = 'INVALID_DATE_TIME_SYNTAX'
-    INVALID_REGEX_SYNTAX = 'INVALID_REGEX_SYNTAX'
-    INVALID_URL_SYNTAX = 'INVALID_URL_SYNTAX'
-    INVALID_VALUE = 'INVALID_VALUE'
-    JSON_EXPECTED = 'JSON_EXPECTED'
-    MAX_ONE_PROPERTY_ALLOWED = 'MAX_ONE_PROPERTY_ALLOWED'
-    NAME_LENGTH_LESS_THAN_MIN = 'NAME_LENGTH_LESS_THAN_MIN'
-    NOT_NULL_BODY = 'NOT_NULL_BODY'
-    OBJECT_EXPECTED = 'OBJECT_EXPECTED'
-    OBJECT_SIZE_BYTES_GREATER_THAN_MAX = 'OBJECT_SIZE_BYTES_GREATER_THAN_MAX'
-    PATTERN_MISMATCH = 'PATTERN_MISMATCH'
-    SIMPLE_VALUE_EXPECTED = 'SIMPLE_VALUE_EXPECTED'
-    STRING_EXPECTED = 'STRING_EXPECTED'
-    STRING_LENGTH_GREATER_THAN_MAX = 'STRING_LENGTH_GREATER_THAN_MAX'
-    STRING_LENGTH_LESS_THAN_MIN = 'STRING_LENGTH_LESS_THAN_MIN'
-    STRING_LENGTH_OUT_OF_BOUNDS = 'STRING_LENGTH_OUT_OF_BOUNDS'
-    UNKNOWN_ENUM_VALUE = 'UNKNOWN_ENUM_VALUE'
-    UUID_EXPECTED = 'UUID_EXPECTED'
-    VALUES_REQUIRED = 'VALUES_REQUIRED'
-    VALUE_GREATER_THAN_MAX = 'VALUE_GREATER_THAN_MAX'
-    VALUE_LESS_THAN_MIN = 'VALUE_LESS_THAN_MIN'
-    VALUE_NOT_ALLOWED = 'VALUE_NOT_ALLOWED'
-    VALUE_OUT_OF_BOUNDS = 'VALUE_OUT_OF_BOUNDS'
-    VALUE_REQUIRED = 'VALUE_REQUIRED'
+__all__ = [
+    'CommonErrorCodes',
+    'InternalErrorCodes',
+    'ValidationErrorCodes'
+]
+from enum import Enum, unique
+
+
+@unique
+class CommonErrorCodes(Enum):
+    """Common error codes returned by Toloka.
+    """
+
+    ACCESS_DENIED = 'ACCESS_DENIED'
+    AUTHENTICATION_ERROR = 'AUTHENTICATION_ERROR'
+    CONFLICT_STATE = 'CONFLICT_STATE'
+    DOES_NOT_EXIST = 'DOES_NOT_EXIST'
+    INTERNAL_ERROR = 'INTERNAL_ERROR'
+    REMOTE_SERVICE_UNAVAILABLE = 'REMOTE_SERVICE_UNAVAILABLE'
+    TOO_MANY_REQUESTS = 'TOO_MANY_REQUESTS'
+    VALIDATION_ERROR = 'VALIDATION_ERROR'
+
+
+@unique
+class InternalErrorCodes(Enum):
+    """Internal error codes returned by Toloka.
+    """
+
+    ACCOUNT_ALREADY_USED = 'ACCOUNT_ALREADY_USED'
+    ACCOUNT_MUST_BE_IDENTIFIED = 'ACCOUNT_MUST_BE_IDENTIFIED'
+    ADJUSTER_NOT_FOUND = 'ADJUSTER_NOT_FOUND'
+    ALL_ASSIGNMENTS_EXHAUSTED = 'ALL_ASSIGNMENTS_EXHAUSTED'
+    ASSIGNMENTS_AGGREGATION_DENIED = 'ASSIGNMENTS_AGGREGATION_DENIED'
+    ASSIGNMENTS_COUNT_CONFLICT = 'ASSIGNMENTS_COUNT_CONFLICT'
+    BATCH_INITIALIZATION_ERROR = 'BATCH_INITIALIZATION_ERROR'
+    BATCH_REJECTED = 'BATCH_REJECTED'
+    BILLING_NOT_SYNCHRONIZED = 'BILLING_NOT_SYNCHRONIZED'
+    CAPTCHA_REQUIRED = 'CAPTCHA_REQUIRED'
+    DELETE_ALL_TASKS_CONFLICT = 'DELETE_ALL_TASKS_CONFLICT'
+    EMPTY_POOL = 'EMPTY_POOL'
+    INAPPROPRIATE_STATUS = 'INAPPROPRIATE_STATUS'
+    INCORRECT_RECIPIENTS = 'INCORRECT_RECIPIENTS'
+    INVALID_OPERATION_TYPE = 'INVALID_OPERATION_TYPE'
+    INVALID_REFERRAL_CODE = 'INVALID_REFERRAL_CODE'
+    INVALID_WORKER_STATUS_ERROR = 'INVALID_WORKER_STATUS_ERROR'
+    MIXER_CONFIG_REQUIRED = 'MIXER_CONFIG_REQUIRED'
+    NEED_PHONE_CONFIRMATION = 'NEED_PHONE_CONFIRMATION'
+    NOT_ENOUGH_BALANCE = 'NOT_ENOUGH_BALANCE'
+    OAUTH_AUTHENTICATION_ERROR = 'OAUTH_AUTHENTICATION_ERROR'
+    OPERATION_ALREADY_EXISTS = 'OPERATION_ALREADY_EXISTS'
+    OPERATION_EXECUTION_ERROR = 'OPERATION_EXECUTION_ERROR'
+    OPERATION_LOGS_ARCHIVED = 'OPERATION_LOGS_ARCHIVED'
+    PAYONEER_ACCOUNT_NOT_ACTIVE = 'PAYONEER_ACCOUNT_NOT_ACTIVE'
+    PAYPAL_AUTH_CODE_INVALID = 'PAYPAL_AUTH_CODE_INVALID'
+    PAYPAL_UNVERIFIED_USER = 'PAYPAL_UNVERIFIED_USER'
+    POOL_ASSIGNMENTS_COUNT_EXCEEDED = 'POOL_ASSIGNMENTS_COUNT_EXCEEDED'
+    POOL_ASSIGNMENTS_EXHAUSTED = 'POOL_ASSIGNMENTS_EXHAUSTED'
+    POOL_INAPPROPRIATE_STATUS = 'POOL_INAPPROPRIATE_STATUS'
+    POOL_INVALID_FILTER_FOR_MAP_ISSUING = 'POOL_INVALID_FILTER_FOR_MAP_ISSUING'
+    POOL_IS_TRAINING = 'POOL_IS_TRAINING'
+    POOL_LOCKED_BY_ANOTHER_OPERATION = 'POOL_LOCKED_BY_ANOTHER_OPERATION'
+    POOL_TASKS_COUNT_EXCEEDED = 'POOL_TASKS_COUNT_EXCEEDED'
+    POOL_TASK_SUITES_COUNT_EXCEEDED = 'POOL_TASK_SUITES_COUNT_EXCEEDED'
+    POOL_TASK_TYPE_CONFLICT = 'POOL_TASK_TYPE_CONFLICT'
+    PROJECT_INAPPROPRIATE_STATUS = 'PROJECT_INAPPROPRIATE_STATUS'
+    RESULTS_EXPIRED = 'RESULTS_EXPIRED'
+    SECURE_PHONE_DUPLICATION = 'SECURE_PHONE_DUPLICATION'
+    SECURE_PHONE_MISSING = 'SECURE_PHONE_MISSING'
+    SECURE_PHONE_WAS_CHANGED = 'SECURE_PHONE_WAS_CHANGED'
+    SKILL_IS_TRAINING = 'SKILL_IS_TRAINING'
+    SKILL_IS_USED = 'SKILL_IS_USED'
+    SKILL_IS_USED_BY_PROJECTS = 'SKILL_IS_USED_BY_PROJECTS'
+    SKILL_REMOVED = 'SKILL_REMOVED'
+    SUBMITTED_ASSIGNMENTS_CONFLICT = 'SUBMITTED_ASSIGNMENTS_CONFLICT'
+    SYNC_POOL_CLONE_ERROR = 'SYNC_POOL_CLONE_ERROR'
+    SYSTEM_SCOPE_MODIFICATION = 'SYSTEM_SCOPE_MODIFICATION'
+    TASK_VALIDATION_ERROR = 'TASK_VALIDATION_ERROR'
+    THERE_IS_ACTIVE_ASSIGNMENT = 'THERE_IS_ACTIVE_ASSIGNMENT'
+    THERE_IS_REJECTED_ASSIGNMENT = 'THERE_IS_REJECTED_ASSIGNMENT'
+    TOO_MANY_ACTIVE_ASSIGNMENTS = 'TOO_MANY_ACTIVE_ASSIGNMENTS'
+    TRAINING_ARCHIVE_CONFLICT = 'TRAINING_ARCHIVE_CONFLICT'
+    UNABLE_TO_UPLOAD_FILE = 'UNABLE_TO_UPLOAD_FILE'
+    UNARCHIVED_POOLS_CONFLICT = 'UNARCHIVED_POOLS_CONFLICT'
+    UNSUPPORTED_ALGORITHM = 'UNSUPPORTED_ALGORITHM'
+    UNSUPPORTED_REGION = 'UNSUPPORTED_REGION'
+    USER_ALREADY_REGISTERED = 'USER_ALREADY_REGISTERED'
+    USER_HAS_PDD_ALIAS = 'USER_HAS_PDD_ALIAS'
+    WITHDRAWAL_TRANSACTION_CANNOT_BE_CANCELLED = 'WITHDRAWAL_TRANSACTION_CANNOT_BE_CANCELLED'
+    WITHDRAWAL_TRANSACTION_CANNOT_BE_CANCELLED_DUE_TO_TIME_LIMIT = \
+        'WITHDRAWAL_TRANSACTION_CANNOT_BE_CANCELLED_DUE_TO_TIME_LIMIT'
+    WORKER_SKILL_EXISTS = 'WORKER_SKILL_EXISTS'
+    WRONG_FILE_FORMAT = 'WRONG_FILE_FORMAT'
+    WRONG_REVISION = 'WRONG_REVISION'
+
+
+@unique
+class ValidationErrorCodes(Enum):
+    """Validation error codes returned by Toloka.
+    """
+
+    ARRAY_EXPECTED = 'ARRAY_EXPECTED'
+    ARRAY_SIZE_GREATER_THAN_MAX = 'ARRAY_SIZE_GREATER_THAN_MAX'
+    ARRAY_SIZE_LESS_THAN_MIN = 'ARRAY_SIZE_LESS_THAN_MIN'
+    ARRAY_SIZE_OUT_OF_BOUNDS = 'ARRAY_SIZE_OUT_OF_BOUNDS'
+    BLANK_STRING_NOT_ALLOWED = 'BLANK_STRING_NOT_ALLOWED'
+    BOOLEAN_EXPECTED = 'BOOLEAN_EXPECTED'
+    CHARACTER_NOT_ALLOWED = 'CHARACTER_NOT_ALLOWED'
+    DATE_OUT_OF_RANGE = 'DATE_OUT_OF_RANGE'
+    DUPLICATE_VALUE_IN_ARRAY = 'DUPLICATE_VALUE_IN_ARRAY'
+    EMPTY_OBJECT_NOT_ALLOWED = 'EMPTY_OBJECT_NOT_ALLOWED'
+    ENTITY_ACCESS_DENIED = 'ENTITY_ACCESS_DENIED'
+    ENTITY_DOES_NOT_EXIST = 'ENTITY_DOES_NOT_EXIST'
+    FLOAT_EXPECTED = 'FLOAT_EXPECTED'
+    INTEGER_EXPECTED = 'INTEGER_EXPECTED'
+    INVALID_COORDINATES_SYNTAX = 'INVALID_COORDINATES_SYNTAX'
+    INVALID_DATE_SYNTAX = 'INVALID_DATE_SYNTAX'
+    INVALID_DATE_TIME_SYNTAX = 'INVALID_DATE_TIME_SYNTAX'
+    INVALID_REGEX_SYNTAX = 'INVALID_REGEX_SYNTAX'
+    INVALID_URL_SYNTAX = 'INVALID_URL_SYNTAX'
+    INVALID_VALUE = 'INVALID_VALUE'
+    JSON_EXPECTED = 'JSON_EXPECTED'
+    MAX_ONE_PROPERTY_ALLOWED = 'MAX_ONE_PROPERTY_ALLOWED'
+    NAME_LENGTH_LESS_THAN_MIN = 'NAME_LENGTH_LESS_THAN_MIN'
+    NOT_NULL_BODY = 'NOT_NULL_BODY'
+    OBJECT_EXPECTED = 'OBJECT_EXPECTED'
+    OBJECT_SIZE_BYTES_GREATER_THAN_MAX = 'OBJECT_SIZE_BYTES_GREATER_THAN_MAX'
+    PATTERN_MISMATCH = 'PATTERN_MISMATCH'
+    SIMPLE_VALUE_EXPECTED = 'SIMPLE_VALUE_EXPECTED'
+    STRING_EXPECTED = 'STRING_EXPECTED'
+    STRING_LENGTH_GREATER_THAN_MAX = 'STRING_LENGTH_GREATER_THAN_MAX'
+    STRING_LENGTH_LESS_THAN_MIN = 'STRING_LENGTH_LESS_THAN_MIN'
+    STRING_LENGTH_OUT_OF_BOUNDS = 'STRING_LENGTH_OUT_OF_BOUNDS'
+    UNKNOWN_ENUM_VALUE = 'UNKNOWN_ENUM_VALUE'
+    UUID_EXPECTED = 'UUID_EXPECTED'
+    VALUES_REQUIRED = 'VALUES_REQUIRED'
+    VALUE_GREATER_THAN_MAX = 'VALUE_GREATER_THAN_MAX'
+    VALUE_LESS_THAN_MIN = 'VALUE_LESS_THAN_MIN'
+    VALUE_NOT_ALLOWED = 'VALUE_NOT_ALLOWED'
+    VALUE_OUT_OF_BOUNDS = 'VALUE_OUT_OF_BOUNDS'
+    VALUE_REQUIRED = 'VALUE_REQUIRED'
```

### Comparing `toloka-kit-1.1.4/src/client/exceptions.py` & `toloka-kit-1.2.0/src/client/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,85 +14,92 @@
     'FailedOperation',
 ]
 
 import json
 from typing import Any, List, Optional
 
 import attr
-from httpx import HTTPStatusError, Response as HTTPXResponse
+import httpx
+from httpx import HTTPStatusError
 
 from .error_codes import CommonErrorCodes, InternalErrorCodes
 from ..util._docstrings import inherit_docstrings
 
 
 # Client errors
 @attr.attrs(auto_attribs=True, str=True, kw_only=True)
 class SpecClassIdentificationError(Exception):
-    """Raised when cannot find spec_сlass for spec_field value.
+    """An exception that is raised when a specification сlass can't be find for a field specification name.
 
     Attributes:
-        spec_field: value that defines spec_class type
-        spec_enum: enum class containing spec_class possible types
+        spec_field: The field specification name.
+        spec_enum: An enumeration with all known specification names.
     """
 
     spec_field: Optional[str] = None
     spec_enum: Optional[str] = None
 
 
 @attr.attrs(auto_attribs=True, str=True, kw_only=True)
 class FailedOperation(Exception):
-    """Raised when an operation failed.
+    """An exception that is raised when an operation fails.
 
-    Could be raised when an inner operation failed.
+    It could be raised when an inner operation fails.
 
     Attributes:
-        operation: Instance of failed operation.
+        operation: The instance of the failed operation.
     """
     operation: Optional[Any] = None
 
 
 # API errors
 @attr.attrs(auto_attribs=True, kw_only=True)
 class ApiError(Exception):
-    """Error returned from the API Call.
+    """A base class for exceptions that are raised when API methods return errors.
 
     Attributes:
-        status_code: response status code.
-        request_id: request ID
-        code: error code string
-        message: error message
-        payload: additional payload
+        status_code: A HTTP response status code.
+        request_id: The ID of the request that returns an error.
+        code: An error code.
+        message: An error description.
+        payload: Additional data describing an error.
     """
 
-    status_code: Optional[int] = None
     request_id: Optional[str] = None
     code: Optional[str] = None
     message: Optional[str] = None
     payload: Optional[Any] = None
 
+    status_code: Optional[int] = None
+    response: Optional[httpx.Response] = None
+
     def __str__(self):
         head = f'You have got a(n) {type(self).__name__} with http status code: {self.status_code}'
         code = f'Code of error: {self.code}'
         error_details = f'Error details: {self.message}'
         if self.payload:
-            additional_info = 'Additional information about the error:\n' + json.dumps(self.payload, indent=4)
+            try:
+                payload_str = json.dumps(self.payload, indent=4)
+            except TypeError:
+                payload_str = f'failed to parse payload as JSON! Falling back to raw representation:\n{self.payload}'
+            additional_info = 'Additional information about the error:\n' + payload_str
         else:
             additional_info = ''
         request_id = f'request id: {self.request_id}. It needs to be specified when contacting support.'
         lines = [line for line in [head, code, error_details, additional_info, request_id] if line]
         result = '\n'.join(lines)
         return result
 
 
 @inherit_docstrings
 class ValidationApiError(ApiError):
-    """Field validation error returned from the API Call.
+    """An exception for a field validation error returned by an API method.
 
     Attributes:
-        invalid_fields: the list of the invalid fields
+        invalid_fields: A list of invalid fields.
     """
 
     _invalid_fields: Optional[List[str]] = None
 
     @property
     def invalid_fields(self) -> List[str]:
         if self._invalid_fields is None:
@@ -150,23 +157,26 @@
     CommonErrorCodes.CONFLICT_STATE.value: ConflictStateApiError,
     CommonErrorCodes.TOO_MANY_REQUESTS.value: TooManyRequestsApiError,
     CommonErrorCodes.REMOTE_SERVICE_UNAVAILABLE.value: RemoteServiceUnavailableApiError,
     **{code.value: IncorrectActionsApiError for code in InternalErrorCodes}
 }
 
 
-def raise_on_api_error(response: HTTPXResponse):
+def raise_on_api_error(response: httpx.Response):
     if 200 <= response.status_code < 300:
         return
 
     if not response.content:
         raise HTTPStatusError(message='No content', response=response, request=response.request)
 
     response_json = response.json()
     error_class = _ERROR_MAP.get(response_json['code'], ApiError)
 
     class_fields = [field.name for field in attr.fields(error_class)]
     for key in response_json.copy().keys():
         if key not in class_fields:
             response_json.pop(key)
 
-    raise error_class(status_code=response.status_code, **response_json)
+    error = error_class(**response_json)
+    error.status_code = response.status_code
+    error.response = response
+    raise error
```

### Comparing `toloka-kit-1.1.4/src/client/exceptions.pyi` & `toloka-kit-1.2.0/src/client/exceptions.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     'FailedOperation',
 ]
 import httpx
 import typing
 
 
 class SpecClassIdentificationError(Exception):
-    """Raised when cannot find spec_сlass for spec_field value.
+    """An exception that is raised when a specification сlass can't be find for a field specification name.
 
     Attributes:
-        spec_field: value that defines spec_class type
-        spec_enum: enum class containing spec_class possible types
+        spec_field: The field specification name.
+        spec_enum: An enumeration with all known specification names.
     """
 
     def __init__(
         self,
         *,
         spec_field: typing.Optional[str] = None,
         spec_enum: typing.Optional[str] = None
@@ -36,203 +36,214 @@
         ...
 
     spec_field: typing.Optional[str]
     spec_enum: typing.Optional[str]
 
 
 class FailedOperation(Exception):
-    """Raised when an operation failed.
+    """An exception that is raised when an operation fails.
 
-    Could be raised when an inner operation failed.
+    It could be raised when an inner operation fails.
 
     Attributes:
-        operation: Instance of failed operation.
+        operation: The instance of the failed operation.
     """
 
     def __init__(self, *, operation: typing.Optional[typing.Any] = None) -> None:
         """Method generated by attrs for class FailedOperation.
         """
         ...
 
     operation: typing.Optional[typing.Any]
 
 
 class ApiError(Exception):
-    """Error returned from the API Call.
+    """A base class for exceptions that are raised when API methods return errors.
 
     Attributes:
-        status_code: response status code.
-        request_id: request ID
-        code: error code string
-        message: error message
-        payload: additional payload
+        status_code: A HTTP response status code.
+        request_id: The ID of the request that returns an error.
+        code: An error code.
+        message: An error description.
+        payload: Additional data describing an error.
     """
 
     def __init__(
         self,
         *,
-        status_code: typing.Optional[int] = None,
         request_id: typing.Optional[str] = None,
         code: typing.Optional[str] = None,
         message: typing.Optional[str] = None,
-        payload: typing.Optional[typing.Any] = None
+        payload: typing.Optional[typing.Any] = None,
+        status_code: typing.Optional[int] = None,
+        response: typing.Optional[httpx.Response] = None
     ) -> None:
         """Method generated by attrs for class ApiError.
         """
         ...
 
-    status_code: typing.Optional[int]
     request_id: typing.Optional[str]
     code: typing.Optional[str]
     message: typing.Optional[str]
     payload: typing.Optional[typing.Any]
+    status_code: typing.Optional[int]
+    response: typing.Optional[httpx.Response]
 
 
 class ValidationApiError(ApiError):
-    """Field validation error returned from the API Call.
+    """An exception for a field validation error returned by an API method.
 
     Attributes:
-        status_code: response status code.
-        request_id: request ID
-        code: error code string
-        message: error message
-        payload: additional payload
-        invalid_fields: the list of the invalid fields
+        request_id: The ID of the request that returns an error.
+        code: An error code.
+        message: An error description.
+        payload: Additional data describing an error.
+        status_code: A HTTP response status code.
+        invalid_fields: A list of invalid fields.
     """
 
-    status_code: typing.Optional[int]
     request_id: typing.Optional[str]
     code: typing.Optional[str]
     message: typing.Optional[str]
     payload: typing.Optional[typing.Any]
+    status_code: typing.Optional[int]
+    response: typing.Optional[httpx.Response]
     _invalid_fields: typing.Optional[typing.List[str]]
 
 
 class InternalApiError(ApiError):
     """Attributes:
-        status_code: response status code.
-        request_id: request ID
-        code: error code string
-        message: error message
-        payload: additional payload
+        request_id: The ID of the request that returns an error.
+        code: An error code.
+        message: An error description.
+        payload: Additional data describing an error.
+        status_code: A HTTP response status code.
     """
 
-    status_code: typing.Optional[int]
     request_id: typing.Optional[str]
     code: typing.Optional[str]
     message: typing.Optional[str]
     payload: typing.Optional[typing.Any]
+    status_code: typing.Optional[int]
+    response: typing.Optional[httpx.Response]
 
 
 class AuthenticationApiError(ApiError):
     """Attributes:
-        status_code: response status code.
-        request_id: request ID
-        code: error code string
-        message: error message
-        payload: additional payload
+        request_id: The ID of the request that returns an error.
+        code: An error code.
+        message: An error description.
+        payload: Additional data describing an error.
+        status_code: A HTTP response status code.
     """
 
-    status_code: typing.Optional[int]
     request_id: typing.Optional[str]
     code: typing.Optional[str]
     message: typing.Optional[str]
     payload: typing.Optional[typing.Any]
+    status_code: typing.Optional[int]
+    response: typing.Optional[httpx.Response]
 
 
 class AccessDeniedApiError(ApiError):
     """Attributes:
-        status_code: response status code.
-        request_id: request ID
-        code: error code string
-        message: error message
-        payload: additional payload
+        request_id: The ID of the request that returns an error.
+        code: An error code.
+        message: An error description.
+        payload: Additional data describing an error.
+        status_code: A HTTP response status code.
     """
 
-    status_code: typing.Optional[int]
     request_id: typing.Optional[str]
     code: typing.Optional[str]
     message: typing.Optional[str]
     payload: typing.Optional[typing.Any]
+    status_code: typing.Optional[int]
+    response: typing.Optional[httpx.Response]
 
 
 class RemoteServiceUnavailableApiError(ApiError):
     """Attributes:
-        status_code: response status code.
-        request_id: request ID
-        code: error code string
-        message: error message
-        payload: additional payload
+        request_id: The ID of the request that returns an error.
+        code: An error code.
+        message: An error description.
+        payload: Additional data describing an error.
+        status_code: A HTTP response status code.
     """
 
-    status_code: typing.Optional[int]
     request_id: typing.Optional[str]
     code: typing.Optional[str]
     message: typing.Optional[str]
     payload: typing.Optional[typing.Any]
+    status_code: typing.Optional[int]
+    response: typing.Optional[httpx.Response]
 
 
 class DoesNotExistApiError(ApiError):
     """Attributes:
-        status_code: response status code.
-        request_id: request ID
-        code: error code string
-        message: error message
-        payload: additional payload
+        request_id: The ID of the request that returns an error.
+        code: An error code.
+        message: An error description.
+        payload: Additional data describing an error.
+        status_code: A HTTP response status code.
     """
 
-    status_code: typing.Optional[int]
     request_id: typing.Optional[str]
     code: typing.Optional[str]
     message: typing.Optional[str]
     payload: typing.Optional[typing.Any]
+    status_code: typing.Optional[int]
+    response: typing.Optional[httpx.Response]
 
 
 class ConflictStateApiError(ApiError):
     """Attributes:
-        status_code: response status code.
-        request_id: request ID
-        code: error code string
-        message: error message
-        payload: additional payload
+        request_id: The ID of the request that returns an error.
+        code: An error code.
+        message: An error description.
+        payload: Additional data describing an error.
+        status_code: A HTTP response status code.
     """
 
-    status_code: typing.Optional[int]
     request_id: typing.Optional[str]
     code: typing.Optional[str]
     message: typing.Optional[str]
     payload: typing.Optional[typing.Any]
+    status_code: typing.Optional[int]
+    response: typing.Optional[httpx.Response]
 
 
 class TooManyRequestsApiError(ApiError):
     """Attributes:
-        status_code: response status code.
-        request_id: request ID
-        code: error code string
-        message: error message
-        payload: additional payload
+        request_id: The ID of the request that returns an error.
+        code: An error code.
+        message: An error description.
+        payload: Additional data describing an error.
+        status_code: A HTTP response status code.
     """
 
-    status_code: typing.Optional[int]
     request_id: typing.Optional[str]
     code: typing.Optional[str]
     message: typing.Optional[str]
     payload: typing.Optional[typing.Any]
+    status_code: typing.Optional[int]
+    response: typing.Optional[httpx.Response]
 
 
 class IncorrectActionsApiError(ApiError):
     """Attributes:
-        status_code: response status code.
-        request_id: request ID
-        code: error code string
-        message: error message
-        payload: additional payload
+        request_id: The ID of the request that returns an error.
+        code: An error code.
+        message: An error description.
+        payload: Additional data describing an error.
+        status_code: A HTTP response status code.
     """
 
-    status_code: typing.Optional[int]
     request_id: typing.Optional[str]
     code: typing.Optional[str]
     message: typing.Optional[str]
     payload: typing.Optional[typing.Any]
+    status_code: typing.Optional[int]
+    response: typing.Optional[httpx.Response]
 
 
 def raise_on_api_error(response: httpx.Response): ...
```

### Comparing `toloka-kit-1.1.4/src/client/filter.py` & `toloka-kit-1.2.0/src/client/filter.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/filter.pyi` & `toloka-kit-1.2.0/src/client/filter.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/message_thread.py` & `toloka-kit-1.2.0/src/client/message_thread.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,120 +16,122 @@
 from .primitives.base import BaseTolokaObject
 from ..util._codegen import attribute
 from ..util._extendable_enum import ExtendableStrEnum
 
 
 @unique
 class RecipientsSelectType(ExtendableStrEnum):
-    """Method for specifying recipients.
+    """The way of specifying message recipients.
 
     Attributes:
-        DIRECT: specify IDs of Tolokers.
-        FILTER: select Tolokers using a filter.
-        ALL: send a message to all Tolokers who have tried to complete your tasks at least once.
+        DIRECT: A list of Toloker IDs.
+        FILTER: A filter for selecting Tolokers.
+        ALL: All Tolokers who completed any of your tasks at least once.
     """
 
     DIRECT = 'DIRECT'
     FILTER = 'FILTER'
     ALL = 'ALL'
 
 
 @unique
 class Folder(ExtendableStrEnum):
-    """Folders for a thread.
+    """A folder with threads.
     """
 
     INBOX = 'INBOX'
     OUTBOX = 'OUTBOX'
     AUTOMATIC_NOTIFICATION = 'AUTOMATIC_NOTIFICATION'
     IMPORTANT = 'IMPORTANT'
     UNREAD = 'UNREAD'
 
 
 class Interlocutor(BaseTolokaObject):
-    """Information about the sender or recipient.
+    """Information about a message sender or recipient.
 
     Attributes:
-        id: ID of the sender or recipient.
-        role: Role of the sender or recipient in Toloka.
-        myself: Marks a sender or recipient with your ID. If the ID belongs to you, the value is `True`.
+        id: The ID of the sender or recipient.
+        role: The role in Toloka.
+        myself: A flag that is set to `True` when the ID is yours.
     """
 
     @unique
     class InterlocutorRole(ExtendableStrEnum):
-        """Role of the sender or recipient in Toloka.
+        """A role in Toloka.
 
         Attributes:
             USER: A Toloker.
-            REQUESTER: A requester.
+            REQUESTER: A Requester.
             ADMINISTRATOR: An administrator.
-            SYSTEM: For messages sent automatically.
+            SYSTEM: The Toloka itself. This role is used for messages that are sent automatically.
         """
 
         USER = 'USER'
         REQUESTER = 'REQUESTER'
         ADMINISTRATOR = 'ADMINISTRATOR'
         SYSTEM = 'SYSTEM'
 
     id: str
     role: InterlocutorRole = attribute(autocast=True)
     myself: bool
 
 
 class MessageThread(BaseTolokaObject):
-    """Message thread.
+    """A message thread.
 
-    The sent message is added to the new message thread. Until the first response is received the message chain is in
-    the folder UNREAD. If there are several addresses in the chain and one of them responds, a new message chain
-    will be created
-    Attributes:
-        id: Message thread ID.
-        topic: Message thread title.
-        interlocutors_inlined: Access information about the sender and recipients.
-            * `True` — information is available in the field interlocutors.
-            * `False` — information is available on a separate request.
-        interlocutors: Information about the sender and recipients, sorted by IDs.
-        messages_inlined: Access to message threads:
-            * `True` — The message is available in the messages field.
-            * `False` — The message is available in a separate request.
-        messages: Messages in the thread. Sorted by creation date (new first).
-        meta: Meta
-        answerable: Ability to reply to a message:
-            * `True` — The Toloker can respond to the message.
-            * `False` — The Toloker cannot respond to the message.
-        folders: Folders where the thread is located.
-        compose_details: For messages that you sent: details of the POST request for creating the message.
-        created: The date the first message in the chain was created.
+    A message thread is created when you send a new message. Then responses are placed to the thread.
+    Until the first response is received the message thread is in the `UNREAD` folder.
+
+    If the message has several recipients then a message thread is created for each recipient when they responds.
+
+    Attributes:
+        id: The ID of the thread.
+        topic: The message thread title. `topic` is a dictionary with two letter language codes as keys.
+        interlocutors_inlined: The way of accessing information about the sender and recipients:
+            * `True` — Information is available in the `interlocutors` list.
+            * `False` — Information is available on a separate request.
+        interlocutors: A list with information about the sender and recipients, sorted by IDs.
+        messages_inlined: The way of accessing messages:
+            * `True` — The messages are in the `messages` list.
+            * `False` — The messages are available on a separate request.
+        messages: A list with thread messages. The list is sorted by creation date: newer messages come first.
+        meta: Thread meta information.
+        answerable:
+            * `True` — Tolokers can respond to your messages.
+            * `False` — Tolokers can't respond to your messages.
+        folders: Folders containing the thread.
+        compose_details: The details of selecting recipients. This information is provided if the first message in the thread was yours.
+        created: The date and time when the first message in the thread was created.
     """
 
     class ComposeDetails(BaseTolokaObject):
-        """For messages that you sent: details of the POST request for creating the message.
+        """The details of selecting recipients.
 
         Attributes:
-            recipients_select_type: Method for specifying recipients.
-            recipients_ids: List of recipients IDs.
-            recipients_filter: Condition to filter recipients.
+            recipients_select_type: The way of specifying message recipients.
+            recipients_ids: A list of Toloker IDs. It is filled if `recipients_select_type` is `DIRECT`.
+            recipients_filter: A filter for selecting Tolokers. It is set if `recipients_select_type` is `FILTER`.
         """
 
         recipients_select_type: RecipientsSelectType = attribute(autocast=True)
         recipients_ids: List[str]
         recipients_filter: FilterCondition
 
     class Meta(BaseTolokaObject):
         pool_id: str
         project_id: str
         assignment_id: str
 
     class Message(BaseTolokaObject):
-        """Message in the thread.
+        """A message in a thread.
 
         Attributes:
-            text: Message text.
+            text: The message text. The `text` is a dictionary with two letter language codes as keys.
             from_: Information about the sender.
-            created: Date the message was created.
+            created: The date and time when the message was created.
         """
 
         text: Dict[str, str]
         from_: Interlocutor = attribute(origin='from')
         created: datetime.datetime
 
     id: str
@@ -145,48 +147,49 @@
     folders: List[Folder]
     compose_details: ComposeDetails
 
     created: datetime.datetime
 
 
 class MessageThreadReply(BaseTolokaObject):
-    """Reply to message thread.
+    """A reply in a message thread.
 
     Attributes:
-        text: Message text. You can provide text in several languages (the message will come in the Toloker's language).
-            Format: {"<language RU / EN/TR/ID / FR>": "<message text>"}.
+        text: A dictionary with the message text.
+            Two letter language code is a key in the dictionary. The message in a preferred Toloker's language is sent, if available.
     """
 
     text: Dict[str, str]
 
 
 class MessageThreadFolders(BaseTolokaObject):
-    """Add a message thread to one or more folders
+    """Folders for a message thread.
 
     Attributes:
-        folders: Folders to add/remove a message thread to/from.
+        folders: A list of folders for a message thread.
     """
 
     folders: List[Folder]
 
 
 class MessageThreadCompose(BaseTolokaObject):
-    """Sent message to a Toloker.
+    """Parameters for creating a message thread with the first message.
+
+    The `topic` and `text` parameters are dictionaries.
+    Two letter language code is a key in the dictionaries. If available, the text in a Toloker preferred language is used.
 
     Attributes:
-        recipients_select_type: Method for specifying recipients
-        topic: Post title. You can provide a title in several languages (the message will come in the Toloker's language).
-            Format: "<language RU/EN/TR/ID/FR>": "<topic text>".
-        text: Message text. You can provide text in several languages (the message will come in the Toloker's language).
-            Format: "<language RU/EN/TR/ID/FR>": "<message text>".
-        answerable: Ability to reply to a message:
-            * `True` — The Toloker can respond to the message.
-            * `False` — The Toloker can't respond to the message.
-        recipients_ids: List of IDs of Tolokers to whom the message will be sent.
-        recipients_filter: Filter to select recipients.
+        recipients_select_type: The way of specifying message recipients.
+        topic: The message thread title.
+        text: The message text.
+        answerable:
+            * `True` — Tolokers can respond to your messages.
+            * `False` — Tolokers can't respond to your messages.
+        recipients_ids: A list of Toloker IDs. It is filled if `recipients_select_type` is `DIRECT`.
+        recipients_filter: A filter for selecting Tolokers. It is set if `recipients_select_type` is `FILTER`.
     """
 
     recipients_select_type: RecipientsSelectType = attribute(autocast=True)
     topic: Dict[str, str]
     text: Dict[str, str]
     answerable: bool
     recipients_ids: List[str]
```

### Comparing `toloka-kit-1.1.4/src/client/message_thread.pyi` & `toloka-kit-1.2.0/src/client/task_suite.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,280 +1,229 @@
 __all__ = [
-    'RecipientsSelectType',
-    'Folder',
-    'Interlocutor',
-    'MessageThread',
-    'MessageThreadReply',
-    'MessageThreadFolders',
-    'MessageThreadCompose',
+    'TaskSuite',
+    'TaskSuiteCreateRequestParameters',
+    'TaskSuitesCreateRequestParameters',
+    'TaskSuiteOverlapPatch',
+    'TaskSuitePatch',
 ]
 import datetime
-import toloka.client.filter
 import toloka.client.primitives.base
-import toloka.util._extendable_enum
+import toloka.client.primitives.infinite_overlap
+import toloka.client.primitives.parameter
+import toloka.client.task
 import typing
+import uuid
 
 
-class RecipientsSelectType(toloka.util._extendable_enum.ExtendableStrEnum):
-    """Method for specifying recipients.
+class TaskSuite(toloka.client.primitives.infinite_overlap.InfiniteOverlapParametersMixin, toloka.client.primitives.base.BaseTolokaObject):
+    """A set of tasks assigned to a Toloker at once.
 
-    Attributes:
-        DIRECT: specify IDs of Tolokers.
-        FILTER: select Tolokers using a filter.
-        ALL: send a message to all Tolokers who have tried to complete your tasks at least once.
-    """
-
-    DIRECT = 'DIRECT'
-    FILTER = 'FILTER'
-    ALL = 'ALL'
-
-
-class Folder(toloka.util._extendable_enum.ExtendableStrEnum):
-    """Folders for a thread.
-    """
-
-    INBOX = 'INBOX'
-    OUTBOX = 'OUTBOX'
-    AUTOMATIC_NOTIFICATION = 'AUTOMATIC_NOTIFICATION'
-    IMPORTANT = 'IMPORTANT'
-    UNREAD = 'UNREAD'
-
-
-class Interlocutor(toloka.client.primitives.base.BaseTolokaObject):
-    """Information about the sender or recipient.
+    A task suite contains one or more tasks. Tolokers are paid after completing all tasks in a task suite.
 
     Attributes:
-        id: ID of the sender or recipient.
-        role: Role of the sender or recipient in Toloka.
-        myself: Marks a sender or recipient with your ID. If the ID belongs to you, the value is `True`.
+        pool_id: The ID of a pool that the task suite belongs to.
+        tasks: The tasks.
+        reserved_for: IDs of Tolokers who have access to the task suite.
+        unavailable_for: IDs of Tolokers who don't have access to the task suite.
+        issuing_order_override: The priority of a task suite.
+            It influences the order of assigning task suites to Tolokers in pools with the `issue_task_suites_in_creation_order` parameter set to `True`.
+            Allowed range: from -99999.99999 to 99999.99999.
+        mixed: [The way of grouping tasks](https://toloka.ai/en/docs/guide/concepts/distribute-tasks-by-pages) to create the task suite.
+            * `True` — The tasks are mixed automatically using the smart mixing approach.
+            * `False` — The tasks are grouped manually.
+
+            Default value: `False`.
+        traits_all_of: The task suite can be assigned to Tolokers who have all of the specified traits.
+        traits_any_of: The task suite can be assigned to Tolokers who have any of the specified traits.
+        traits_none_of_any: The task suite can not be assigned to Tolokers who have any of the specified traits.
+        longitude: The longitude of the point on the map for the task suite.
+        latitude: The latitude of the point on the map for the task suite.
+        id: The ID of the task suite. Read-only field.
+        remaining_overlap: The number of times left for this task suite to be assigned to Tolokers. Read-only field.
+        automerged:
+            * `True` — The task suite was created after [merging tasks](https://toloka.ai/en/docs/api/concepts/tasks#task-merge).
+            * `False` — There are no merged tasks in the task suite.
+        created: The UTC date and time when the task suite was created. Read-only field.
     """
 
-    class InterlocutorRole(toloka.util._extendable_enum.ExtendableStrEnum):
-        """Role of the sender or recipient in Toloka.
+    @typing.overload
+    def add_base_task(self, base_task: toloka.client.task.BaseTask) -> 'TaskSuite': ...
 
-        Attributes:
-            USER: A Toloker.
-            REQUESTER: A requester.
-            ADMINISTRATOR: An administrator.
-            SYSTEM: For messages sent automatically.
-        """
-
-        USER = 'USER'
-        REQUESTER = 'REQUESTER'
-        ADMINISTRATOR = 'ADMINISTRATOR'
-        SYSTEM = 'SYSTEM'
+    @typing.overload
+    def add_base_task(
+        self,
+        *,
+        input_values: typing.Optional[typing.Dict[str, typing.Any]] = None,
+        known_solutions: typing.Optional[typing.List[toloka.client.task.BaseTask.KnownSolution]] = None,
+        message_on_unknown_solution: typing.Optional[str] = None
+    ) -> 'TaskSuite': ...
 
     def __init__(
         self,
         *,
+        infinite_overlap=None,
+        overlap=None,
+        pool_id: typing.Optional[str] = None,
+        tasks: typing.Optional[typing.List[toloka.client.task.BaseTask]] = ...,
+        reserved_for: typing.Optional[typing.List[str]] = None,
+        unavailable_for: typing.Optional[typing.List[str]] = None,
+        issuing_order_override: typing.Optional[float] = None,
+        mixed: typing.Optional[bool] = None,
+        traits_all_of: typing.Optional[typing.List[str]] = None,
+        traits_any_of: typing.Optional[typing.List[str]] = None,
+        traits_none_of_any: typing.Optional[typing.List[str]] = None,
+        longitude: typing.Optional[float] = None,
+        latitude: typing.Optional[float] = None,
         id: typing.Optional[str] = None,
-        role: typing.Union[InterlocutorRole, str, None] = None,
-        myself: typing.Optional[bool] = None
+        remaining_overlap: typing.Optional[int] = None,
+        automerged: typing.Optional[bool] = None,
+        created: typing.Optional[datetime.datetime] = None
     ) -> None:
-        """Method generated by attrs for class Interlocutor.
+        """Method generated by attrs for class TaskSuite.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
+    _infinite_overlap: typing.Optional[bool]
+    _overlap: typing.Optional[int]
+    pool_id: typing.Optional[str]
+    tasks: typing.Optional[typing.List[toloka.client.task.BaseTask]]
+    reserved_for: typing.Optional[typing.List[str]]
+    unavailable_for: typing.Optional[typing.List[str]]
+    issuing_order_override: typing.Optional[float]
+    mixed: typing.Optional[bool]
+    traits_all_of: typing.Optional[typing.List[str]]
+    traits_any_of: typing.Optional[typing.List[str]]
+    traits_none_of_any: typing.Optional[typing.List[str]]
+    longitude: typing.Optional[float]
+    latitude: typing.Optional[float]
     id: typing.Optional[str]
-    role: typing.Optional[InterlocutorRole]
-    myself: typing.Optional[bool]
+    remaining_overlap: typing.Optional[int]
+    automerged: typing.Optional[bool]
+    created: typing.Optional[datetime.datetime]
 
 
-class MessageThread(toloka.client.primitives.base.BaseTolokaObject):
-    """Message thread.
+class TaskSuiteCreateRequestParameters(toloka.client.primitives.parameter.IdempotentOperationParameters):
+    """Parameters for creating task suite.
 
-    The sent message is added to the new message thread. Until the first response is received the message chain is in
-    the folder UNREAD. If there are several addresses in the chain and one of them responds, a new message chain
-    will be created
     Attributes:
-        id: Message thread ID.
-        topic: Message thread title.
-        interlocutors_inlined: Access information about the sender and recipients.
-            * `True` — information is available in the field interlocutors.
-            * `False` — information is available on a separate request.
-        interlocutors: Information about the sender and recipients, sorted by IDs.
-        messages_inlined: Access to message threads:
-            * `True` — The message is available in the messages field.
-            * `False` — The message is available in a separate request.
-        messages: Messages in the thread. Sorted by creation date (new first).
-        meta: Meta
-        answerable: Ability to reply to a message:
-            * `True` — The Toloker can respond to the message.
-            * `False` — The Toloker cannot respond to the message.
-        folders: Folders where the thread is located.
-        compose_details: For messages that you sent: details of the POST request for creating the message.
-        created: The date the first message in the chain was created.
-    """
+        operation_id: The ID of the operation conforming to the [RFC4122 standard](https://tools.ietf.org/html/rfc4122).
+        async_mode: Request processing mode:
+            * `True` — Asynchronous operation is started internally.
+            * `False` — The request is processed synchronously.
+
+            Default value: `True`.
+        allow_defaults: Active overlap setting:
+            * `True` — Use the overlap that is set in the `defaults.default_overlap_for_new_task_suites` pool parameter.
+            * `False` — Use the overlap that is set in the `overlap` task suite parameter.
 
-    class ComposeDetails(toloka.client.primitives.base.BaseTolokaObject):
-        """For messages that you sent: details of the POST request for creating the message.
-
-        Attributes:
-            recipients_select_type: Method for specifying recipients.
-            recipients_ids: List of recipients IDs.
-            recipients_filter: Condition to filter recipients.
-        """
-
-        def __init__(
-            self,
-            *,
-            recipients_select_type: typing.Union[RecipientsSelectType, str, None] = None,
-            recipients_ids: typing.Optional[typing.List[str]] = None,
-            recipients_filter: typing.Optional[toloka.client.filter.FilterCondition] = None
-        ) -> None:
-            """Method generated by attrs for class MessageThread.ComposeDetails.
-            """
-            ...
-
-        _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
-        recipients_select_type: typing.Optional[RecipientsSelectType]
-        recipients_ids: typing.Optional[typing.List[str]]
-        recipients_filter: typing.Optional[toloka.client.filter.FilterCondition]
-
-    class Meta(toloka.client.primitives.base.BaseTolokaObject):
-        def __init__(
-            self,
-            *,
-            pool_id: typing.Optional[str] = None,
-            project_id: typing.Optional[str] = None,
-            assignment_id: typing.Optional[str] = None
-        ) -> None:
-            """Method generated by attrs for class MessageThread.Meta.
-            """
-            ...
-
-        _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
-        pool_id: typing.Optional[str]
-        project_id: typing.Optional[str]
-        assignment_id: typing.Optional[str]
-
-    class Message(toloka.client.primitives.base.BaseTolokaObject):
-        """Message in the thread.
-
-        Attributes:
-            text: Message text.
-            from_: Information about the sender.
-            created: Date the message was created.
-        """
-
-        def __init__(
-            self,
-            *,
-            text: typing.Optional[typing.Dict[str, str]] = None,
-            from_: typing.Optional[Interlocutor] = None,
-            created: typing.Optional[datetime.datetime] = None
-        ) -> None:
-            """Method generated by attrs for class MessageThread.Message.
-            """
-            ...
-
-        _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
-        text: typing.Optional[typing.Dict[str, str]]
-        from_: typing.Optional[Interlocutor]
-        created: typing.Optional[datetime.datetime]
+            Default value: `False`.
+        open_pool: Open the pool immediately after creating a task suite, if the pool is closed.
+    """
 
     def __init__(
         self,
         *,
-        id: typing.Optional[str] = None,
-        topic: typing.Optional[typing.Dict[str, str]] = None,
-        interlocutors_inlined: typing.Optional[bool] = None,
-        interlocutors: typing.Optional[typing.List[Interlocutor]] = None,
-        messages_inlined: typing.Optional[bool] = None,
-        messages: typing.Optional[typing.List[Message]] = None,
-        meta: typing.Optional[Meta] = None,
-        answerable: typing.Optional[bool] = None,
-        folders: typing.Optional[typing.List[Folder]] = None,
-        compose_details: typing.Optional[ComposeDetails] = None,
-        created: typing.Optional[datetime.datetime] = None
+        operation_id: typing.Optional[uuid.UUID] = ...,
+        async_mode: typing.Optional[bool] = True,
+        allow_defaults: typing.Optional[bool] = None,
+        open_pool: typing.Optional[bool] = None
     ) -> None:
-        """Method generated by attrs for class MessageThread.
+        """Method generated by attrs for class TaskSuiteCreateRequestParameters.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
-    id: typing.Optional[str]
-    topic: typing.Optional[typing.Dict[str, str]]
-    interlocutors_inlined: typing.Optional[bool]
-    interlocutors: typing.Optional[typing.List[Interlocutor]]
-    messages_inlined: typing.Optional[bool]
-    messages: typing.Optional[typing.List[Message]]
-    meta: typing.Optional[Meta]
-    answerable: typing.Optional[bool]
-    folders: typing.Optional[typing.List[Folder]]
-    compose_details: typing.Optional[ComposeDetails]
-    created: typing.Optional[datetime.datetime]
-
+    operation_id: typing.Optional[uuid.UUID]
+    async_mode: typing.Optional[bool]
+    allow_defaults: typing.Optional[bool]
+    open_pool: typing.Optional[bool]
+
+
+class TaskSuitesCreateRequestParameters(TaskSuiteCreateRequestParameters):
+    """Parameters for creating task suites.
+
+    Attributes:
+        operation_id: The ID of the operation conforming to the [RFC4122 standard](https://tools.ietf.org/html/rfc4122).
+        async_mode: Request processing mode:
+            * `True` — Asynchronous operation is started internally.
+            * `False` — The request is processed synchronously. A maximum of 5000 task suites can be added in a single request in this mode.
+            Default value: `True`.
+        allow_defaults: Active overlap setting:
+            * `True` — Use the overlap that is set in the `defaults.default_overlap_for_new_task_suites` pool parameter.
+            * `False` — Use the overlap that is set in the `overlap` task suite parameter.
+
+            Default value: `False`.
+        open_pool: Open the pool immediately after creating a task suite, if the pool is closed.
+        skip_invalid_items: Task suite validation option:
+            * `True` — All valid task suites are added. If a task suite does not pass validation, then it is not added to Toloka.
+            * `False` — If any task suite does not pass validation, then operation is cancelled and no task suites are added to Toloka.
 
-class MessageThreadReply(toloka.client.primitives.base.BaseTolokaObject):
-    """Reply to message thread.
-
-    Attributes:
-        text: Message text. You can provide text in several languages (the message will come in the Toloker's language).
-            Format: {"<language RU / EN/TR/ID / FR>": "<message text>"}.
+            Default value: `False`.
     """
 
-    def __init__(self, *, text: typing.Optional[typing.Dict[str, str]] = None) -> None:
-        """Method generated by attrs for class MessageThreadReply.
+    def __init__(
+        self,
+        *,
+        operation_id: typing.Optional[uuid.UUID] = ...,
+        async_mode: typing.Optional[bool] = True,
+        allow_defaults: typing.Optional[bool] = None,
+        open_pool: typing.Optional[bool] = None,
+        skip_invalid_items: typing.Optional[bool] = None
+    ) -> None:
+        """Method generated by attrs for class TaskSuitesCreateRequestParameters.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
-    text: typing.Optional[typing.Dict[str, str]]
+    operation_id: typing.Optional[uuid.UUID]
+    async_mode: typing.Optional[bool]
+    allow_defaults: typing.Optional[bool]
+    open_pool: typing.Optional[bool]
+    skip_invalid_items: typing.Optional[bool]
 
 
-class MessageThreadFolders(toloka.client.primitives.base.BaseTolokaObject):
-    """Add a message thread to one or more folders
+class TaskSuiteOverlapPatch(toloka.client.primitives.base.BaseTolokaObject):
+    """Parameters for stopping assigning a task suite.
 
     Attributes:
-        folders: Folders to add/remove a message thread to/from.
+        overlap: The new overlap value.
     """
 
-    def __init__(self, *, folders: typing.Optional[typing.List[Folder]] = None) -> None:
-        """Method generated by attrs for class MessageThreadFolders.
+    def __init__(self, *, overlap: typing.Optional[int] = None) -> None:
+        """Method generated by attrs for class TaskSuiteOverlapPatch.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
-    folders: typing.Optional[typing.List[Folder]]
+    overlap: typing.Optional[int]
 
 
-class MessageThreadCompose(toloka.client.primitives.base.BaseTolokaObject):
-    """Sent message to a Toloker.
+class TaskSuitePatch(toloka.client.primitives.infinite_overlap.InfiniteOverlapParametersMixin, toloka.client.primitives.base.BaseTolokaObject):
+    """Parameters for changing a task suite.
 
     Attributes:
-        recipients_select_type: Method for specifying recipients
-        topic: Post title. You can provide a title in several languages (the message will come in the Toloker's language).
-            Format: "<language RU/EN/TR/ID/FR>": "<topic text>".
-        text: Message text. You can provide text in several languages (the message will come in the Toloker's language).
-            Format: "<language RU/EN/TR/ID/FR>": "<message text>".
-        answerable: Ability to reply to a message:
-            * `True` — The Toloker can respond to the message.
-            * `False` — The Toloker can't respond to the message.
-        recipients_ids: List of IDs of Tolokers to whom the message will be sent.
-        recipients_filter: Filter to select recipients.
-    """
+        issuing_order_override: The priority of a task suite.
+            It influences the order of assigning task suites to Tolokers in pools with the `issue_task_suites_in_creation_order` parameter set to `True`.
+            Allowed range: from -99999.99999 to 99999.99999. Default value: 0.
+        open_pool: Open the pool immediately after changing a task suite, if the pool is closed.
 
-    def unstructure(self) -> typing.Optional[dict]: ...
+            Default value: `False`.
+    """
 
     def __init__(
         self,
         *,
-        recipients_select_type: typing.Union[RecipientsSelectType, str, None] = None,
-        topic: typing.Optional[typing.Dict[str, str]] = None,
-        text: typing.Optional[typing.Dict[str, str]] = None,
-        answerable: typing.Optional[bool] = None,
-        recipients_ids: typing.Optional[typing.List[str]] = None,
-        recipients_filter: typing.Optional[toloka.client.filter.FilterCondition] = None
+        infinite_overlap=None,
+        overlap=None,
+        issuing_order_override: typing.Optional[float] = None,
+        open_pool: typing.Optional[bool] = None
     ) -> None:
-        """Method generated by attrs for class MessageThreadCompose.
+        """Method generated by attrs for class TaskSuitePatch.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
-    recipients_select_type: typing.Optional[RecipientsSelectType]
-    topic: typing.Optional[typing.Dict[str, str]]
-    text: typing.Optional[typing.Dict[str, str]]
-    answerable: typing.Optional[bool]
-    recipients_ids: typing.Optional[typing.List[str]]
-    recipients_filter: typing.Optional[toloka.client.filter.FilterCondition]
+    _infinite_overlap: typing.Optional[bool]
+    _overlap: typing.Optional[int]
+    issuing_order_override: typing.Optional[float]
+    open_pool: typing.Optional[bool]
```

### Comparing `toloka-kit-1.1.4/src/client/operation_log.pyi` & `toloka-kit-1.2.0/src/client/operation_log.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/operations.py` & `toloka-kit-1.2.0/src/client/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,15 +350,14 @@
     All parameters are for reference only and describe the initial parameters of the request that this operation monitors.
 
     Attributes:
         parameters.skip_invalid_items: Validation parameters for JSON objects:
             * `True` — Create rewards using `UserBonus` instances that passed validation. Skip the rest of the `UserBonus` instances.
             * `False` — If at least one of the `UserBonus` instances didn't pass validation, stop the operation and
                 don't create any rewards.
-        details.pool_id:
         details.total_count: The number of bonuses in the request.
         details.valid_count: The number of JSON objects with bonus information that have passed validation.
         details.not_valid_count: The number of JSON objects with bonus information that failed validation.
         details.success_count: Number of bonuses issued.
         details.failed_count: The number of bonuses that were not issued.
     """
```

### Comparing `toloka-kit-1.1.4/src/client/operations.pyi` & `toloka-kit-1.2.0/src/client/operations.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -886,15 +886,14 @@
         progress: The percentage of the operation completed.
         parameters: Operation parameters (depending on the operation type).
         details: Details of the operation completion.
         parameters.skip_invalid_items: Validation parameters for JSON objects:
             * `True` — Create rewards using `UserBonus` instances that passed validation. Skip the rest of the `UserBonus` instances.
             * `False` — If at least one of the `UserBonus` instances didn't pass validation, stop the operation and
                 don't create any rewards.
-        details.pool_id: 
         details.total_count: The number of bonuses in the request.
         details.valid_count: The number of JSON objects with bonus information that have passed validation.
         details.not_valid_count: The number of JSON objects with bonus information that failed validation.
         details.success_count: Number of bonuses issued.
         details.failed_count: The number of bonuses that were not issued.
     """
```

### Comparing `toloka-kit-1.1.4/src/client/owner.py` & `toloka-kit-1.2.0/src/client/owner.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/owner.pyi` & `toloka-kit-1.2.0/src/client/owner.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/pool/__init__.py` & `toloka-kit-1.2.0/src/client/pool/__init__.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/pool/__init__.pyi` & `toloka-kit-1.2.0/src/client/pool/__init__.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/pool/dynamic_overlap_config.py` & `toloka-kit-1.2.0/src/client/pool/dynamic_overlap_config.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/pool/dynamic_overlap_config.pyi` & `toloka-kit-1.2.0/src/client/pool/dynamic_overlap_config.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/pool/dynamic_pricing_config.py` & `toloka-kit-1.2.0/src/client/pool/dynamic_pricing_config.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/pool/dynamic_pricing_config.pyi` & `toloka-kit-1.2.0/src/client/pool/dynamic_pricing_config.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/pool/mixer_config.py` & `toloka-kit-1.2.0/src/client/pool/mixer_config.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/pool/mixer_config.pyi` & `toloka-kit-1.2.0/src/client/pool/mixer_config.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/pool/speed_quality_balance_config.py` & `toloka-kit-1.2.0/src/client/pool/speed_quality_balance_config.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/pool/speed_quality_balance_config.pyi` & `toloka-kit-1.2.0/src/client/pool/speed_quality_balance_config.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/primitives/base.py` & `toloka-kit-1.2.0/src/client/primitives/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 from enum import Enum
 from functools import update_wrapper, partial
 from typing import Any, ClassVar, Dict, List, Optional, Type, TypeVar, Union, Tuple
 
 import attr
 import simplejson as json
 
+
 from ...util._extendable_enum import ExtendableStrEnumMetaclass
 from .._converter import converter
 from ..exceptions import SpecClassIdentificationError
 from ...util._codegen import (
     attribute, expand, fix_attrs_converters, REQUIRED_KEY, ORIGIN_KEY, AUTOCAST_KEY,
     universal_decorator,
 )
+from ...util._typing import generate_type_var_mapping
 
 E = TypeVar('E', bound=Enum)
 
 logger = logging.getLogger(__file__)
 
 
 class VariantRegistry:
@@ -281,14 +283,16 @@
         data.update(converter.unstructure(self.get_variant_specs()))
         assert '_unexpected' not in data
         return data or None
 
     @classmethod
     def structure(cls, data: Any):
 
+        cls, type_var_mapping = generate_type_var_mapping(cls)
+
         # If a class is an incomplete variant type we structure it into
         # one of its subclasses
         if cls.is_variant_incomplete():
             # TODO: Optimize copying
             data = dict(data)  # Do not modify input data
             spec_field = cls._variant_registry.field
             data_field = data.pop(spec_field)
@@ -310,18 +314,18 @@
         for field in attr.fields(cls):
             key = field.metadata.get(ORIGIN_KEY, field.name)
             if key not in data:
                 continue
 
             value = data.pop(key)
             if field.type is not None:
-                value = converter.structure(value, field.type)
+                target_type = _get_mapped_type(field.type, type_var_mapping)
+                value = converter.structure(value, target_type)
 
             kwargs[field.name] = value
-
         obj = cls(**kwargs)
         obj._unexpected = data
         return obj
 
     def to_json(self, pretty: bool = False) -> str:
         basic_config = {
             'use_decimal': True,
@@ -333,14 +337,44 @@
             return json.dumps(self.unstructure(), separators=(',', ':'), **basic_config)
 
     @classmethod
     def from_json(cls, json_str: str):
         return cls.structure(json.loads(json_str, use_decimal=True))
 
 
+def _get_mapped_type(t, mapping):
+    if isinstance(t, typing.TypeVar):
+        return mapping.get(t.__name__, t)
+    try:
+        origin_type = t.__dict__['__origin__']
+        type_args = t.__dict__.get('__args__', [])
+    except AttributeError:
+        return t
+    except KeyError:
+        return t
+    mapped_args = tuple(_get_mapped_type(t_arg, mapping) for t_arg in type_args)
+
+    # TODO: support all generic types
+    origin_type_mapped = {
+        tuple: typing.Tuple,
+        list: typing.List,
+        dict: typing.Dict,
+    }
+    origin_type = origin_type_mapped.get(origin_type, origin_type)
+
+    if origin_type in [typing.Union, typing.List, typing.Dict, typing.Tuple] and not mapped_args:
+        return origin_type
+    if origin_type in [typing.Union, typing.List, typing.Tuple]:
+        return origin_type[mapped_args]
+    if origin_type in [typing.Dict]:
+        return typing.Dict[mapped_args[0], mapped_args[1]]
+
+    return t
+
+
 @universal_decorator(has_parameters=False)
 def autocast_to_enum(func: typing.Callable) -> typing.Callable:
     """Function decorator that performs str -> Enum conversion when decorated function is called
 
     This decorator modifies function so that every argument annotated with any subclass of Enum type (including Enum
     itself) can be passed a value of str (or any )
     """
```

### Comparing `toloka-kit-1.1.4/src/client/primitives/base.pyi` & `toloka-kit-1.2.0/src/client/primitives/base.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/primitives/infinite_overlap.py` & `toloka-kit-1.2.0/src/client/primitives/infinite_overlap.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/primitives/infinite_overlap.pyi` & `toloka-kit-1.2.0/src/client/primitives/infinite_overlap.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/primitives/operators.py` & `toloka-kit-1.2.0/src/client/primitives/operators.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/primitives/operators.pyi` & `toloka-kit-1.2.0/src/client/primitives/operators.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/primitives/retry.py` & `toloka-kit-1.2.0/src/client/primitives/retry.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,58 @@
 __all__ = [
-    'TolokaRetry', 'SyncRetryingOverURLLibRetry', 'AsyncRetryingOverURLLibRetry', 'STATUSES_TO_RETRY'
+    'TolokaRetry', 'SyncRetryingOverURLLibRetry', 'AsyncRetryingOverURLLibRetry', 'STATUSES_TO_RETRY',
 ]
 
 import json
 import logging
-import socket
+import sys
 from functools import wraps
 from inspect import signature
 from typing import Callable, List, Optional, Tuple, Type, Union
 
 import httpx
 import urllib3
 import urllib3.exceptions
-from tenacity import AsyncRetrying, BaseRetrying, RetryCallState, Retrying
+from httpx import URL
+from tenacity import AsyncRetrying, BaseRetrying, RetryCallState, Retrying, WrappedFn
 from tenacity.retry import retry_base
 from tenacity.stop import stop_base
 from tenacity.wait import wait_base
-from urllib3.connectionpool import ConnectionPool
+from typing_extensions import Protocol, runtime_checkable
 from urllib3.response import HTTPResponse  # type: ignore
 from urllib3.util.retry import Retry  # type: ignore
 
+from .adapters import httpx_exception_to_urllib3_exception, map_urllib3_exception_for_retrying
+
 logger = logging.getLogger(__name__)
 
 STATUSES_TO_RETRY = {408, 429, 500, 503, 504}
 
 
 class TolokaRetry(Retry):
-    """Retry toloka quotas. By default only minutes quotas.
+    """Retry toloka quotas. By default, only minutes quotas.
 
     Args:
         retry_quotas (Union[List[str], str, None]): List of quotas that will be retried.
             None or empty list for not retrying quotas.
             You can specify quotas:
             * MIN - Retry minutes quotas.
             * HOUR - Retry hourly quotas. This is means that the program just sleeps for an hour! Be careful.
             * DAY - Retry daily quotas. We strongly not recommended retrying these quotas.
     """
+
     class Unit:
         MIN = 'MIN'
         HOUR = 'HOUR'
         DAY = 'DAY'
 
     seconds_to_wait = {
         Unit.MIN: 60,
-        Unit.HOUR: 60*60,
-        Unit.DAY: 60*60*24,
+        Unit.HOUR: 60 * 60,
+        Unit.DAY: 60 * 60 * 24,
     }
 
     _retry_quotas: Union[List[str], str, None] = None
 
     def __init__(self, *args, retry_quotas: Union[List[str], str, None] = Unit.MIN, **kwargs):
         if isinstance(retry_quotas, str):
             self._retry_quotas = [retry_quotas]
@@ -92,214 +96,232 @@
                 if data:
                     self._last_response = json.loads(response.data.decode("utf-8"))
         except json.JSONDecodeError:
             pass
         return super(TolokaRetry, self).increment(*args, **kwargs)
 
 
-def httpx_exception_to_urllib_exception(exception: BaseException) -> BaseException:
-    """Maps the httpx exception to the corresponding urllib3 exception."""
-
-    if isinstance(exception, httpx.HTTPError):
-        mapped_exception = urllib3.exceptions.HTTPError()
-    elif isinstance(exception, httpx.RequestError):
-        mapped_exception = urllib3.exceptions.RequestError(
-            pool=ConnectionPool(str(exception.request.url)), url=str(exception.request.url), message=str(exception)
-        )
-    elif isinstance(exception, httpx.TransportError):
-        mapped_exception = urllib3.exceptions.HTTPError(),
-    elif isinstance(exception, httpx.TimeoutException):
-        mapped_exception = urllib3.exceptions.TimeoutError(),
-    elif isinstance(exception, httpx.ConnectTimeout):
-        mapped_exception = urllib3.exceptions.ConnectTimeoutError(),
-    elif isinstance(exception, httpx.ReadTimeout):
-        mapped_exception = urllib3.exceptions.ReadTimeoutError(
-            pool=ConnectionPool(str(exception.request.url)), url=str(exception.request.url), message=str(exception)
-        )
-    elif isinstance(exception, httpx.WriteTimeout):
-        return socket.timeout()
-    elif isinstance(exception, httpx.PoolTimeout):
-        mapped_exception = urllib3.exceptions.NewConnectionError(
-            pool=ConnectionPool(str(exception.request.url)), message=str(exception)
-        )
-    elif isinstance(exception, httpx.NetworkError):
-        mapped_exception = urllib3.exceptions.HTTPError()
-    elif isinstance(exception, httpx.ConnectError):
-        mapped_exception = urllib3.exceptions.ConnectionError()
-    elif isinstance(exception, httpx.ReadError):
-        mapped_exception = socket.error()
-    elif isinstance(exception, httpx.WriteError):
-        mapped_exception = socket.error()
-    elif isinstance(exception, httpx.CloseError):
-        mapped_exception = urllib3.exceptions.ConnectionError()
-    elif isinstance(exception, httpx.ProtocolError):
-        mapped_exception = urllib3.exceptions.ProtocolError()
-    elif isinstance(exception, httpx.LocalProtocolError):
-        mapped_exception = urllib3.exceptions.ProtocolError()
-    elif isinstance(exception, httpx.RemoteProtocolError):
-        mapped_exception = urllib3.exceptions.ProtocolError()
-    elif isinstance(exception, httpx.ProxyError):
-        mapped_exception = urllib3.exceptions.ProxyError(error=exception, message=str(exception))
-    elif isinstance(exception, httpx.UnsupportedProtocol):
-        mapped_exception = urllib3.exceptions.URLSchemeUnknown(scheme=exception.request.url.scheme)
-    elif isinstance(exception, httpx.DecodingError):
-        mapped_exception = urllib3.exceptions.DecodeError()
-    elif isinstance(exception, httpx.TooManyRedirects):
-        mapped_exception = urllib3.exceptions.ResponseError()
-    elif isinstance(exception, httpx.HTTPStatusError):
-        mapped_exception = urllib3.exceptions.ResponseError()
-    elif isinstance(exception, httpx.InvalidURL):
-        mapped_exception = urllib3.exceptions.LocationValueError()
-    elif isinstance(exception, httpx.CookieConflict):
-        mapped_exception = urllib3.exceptions.ResponseError()
-    elif isinstance(exception, httpx.StreamError):
-        mapped_exception = socket.error()
-    elif isinstance(exception, httpx.StreamConsumed):
-        mapped_exception = socket.error()
-    elif isinstance(exception, httpx.StreamClosed):
-        mapped_exception = socket.error()
-    else:
-        mapped_exception = urllib3.exceptions.HTTPError()
-    mapped_exception.__cause__ = exception
-    return mapped_exception
+@runtime_checkable
+class HTTPXRequestFn(Protocol):
+    def __call__(self, method: str, url: Union[URL, str], **kwargs) -> HTTPResponse:
+        ...
 
 
 class RetryingOverURLLibRetry(BaseRetrying):
-    """Adapter class that allows usage of the urllib3 Retry class with the tenacity retrying mechanism.
+    """Adapter class that allows usage of the urllib3 Retry class in httpx using the tenacity retrying mechanism.
 
     Wrapped function should make a single request using HTTPX library and either return httpx.Response or raise an
     exception.
+
+    This class tries to follow the behavior of urllib3.connectionpool.HTTPConnectionPool.urlopen as close as possible:
+    * If an exception is raised during the request:
+        * urllib3 catches a subset of all possible exceptions, calls `Retry.increment` with the raised error and
+            recursively calls urlopen;
+        * this class matches the raised exception against exception_to_retry field in retry callback: if the exception
+            is not matched the retry callback returns False and the exception is raised in user code. Otherwise, retry
+            callback returns True and the `Retry.increment` is called inside the `after` callback with the
+            corresponding urllib3 exception.
+    * If request returned a response:
+        * urllib3 checks if retry should happen using `Retry.is_retry` method, calls `Retry.increment` with the
+            received urllib3.Response object and makes recursive call with the new `Retry` instance. If not retry
+            should happen the response object is returned;
+        * this class calls `Retry.is_retry` method in `retry` callback. If no retry should happen `retry` callback
+            returns False and the execution control is returned to the user code. If retry should happen, this class
+            increments `Retry` instance using the `urllib3.Response` object constructed from the `httpx.Response`.
+    * Retrying is stopped when `Retry.is_exhausted` returns False:
+        * urllib3 achieves this by raising an exception inside `Retry.increment`;
+        * this class catches this exception when calling `Retry.increment` inside the `after` callback and explicitly
+            calls `is_exhausted` inside the `stop` callback.
+
+    Usage of proxies is currently not supported
     """
 
-    def __init__(self, base_url: str, retry: Retry, exception_to_retry: Tuple[Type[Exception], ...], **kwargs):
+    def __init__(self, base_url: str, retry: Retry, exception_to_retry: Tuple[Type[Exception], ...] = (), **kwargs):
         self.base_url = base_url
-        self.urllib_retry = retry
-        self.exception_to_retry = exception_to_retry
+        self.urllib3_retry = retry
+
+        # default exceptions are based on:
+        #   * exceptions that are caught in urllib3.connectionpool.HTTPConnectionPool.urlopen
+        #   * toloka.client.primitives.adapters.httpx_exception_to_urllib3_exception mapping
+        self.exception_to_retry = (
+            httpx.TimeoutException,  # urllib3.exceptions.TimeoutError
+            httpx.NetworkError,  # SocketError or NewConnectionError
+            httpx.ProtocolError,  # urllib3.exceptions.ProtocolError
+            *exception_to_retry
+        )
 
         super().__init__(
             stop=self._get_stop_callback(),
             wait=self._get_wait_callback(),
             after=self._get_after_callback(),
             retry=self._get_retry_callback(),
             **kwargs,
         )
 
+    def wraps(self, f: WrappedFn) -> WrappedFn:
+        # This check contradicts Liskov substitution principle, so it is not enforced by type hints. However, it is
+        # handy to use inheritance here to define SyncRetryingOverURLLibRetry and AsyncRetryingOverURLLibRetry despite
+        # the fact that they are not substitutable for the BaseRetrying.
+        assert isinstance(f, HTTPXRequestFn), 'Wrapped function should be callable with (method, url, **kwargs)'
+        return super().wraps(f)
+
     def __getstate__(self):
         return {
-            'base_url': self.base_url, 'urllib_retry': self.urllib_retry, 'exception_to_retry': self.exception_to_retry
+            'base_url': self.base_url, 'urllib3_retry': self.urllib3_retry,
+            'exception_to_retry': self.exception_to_retry
         }
 
     def __setstate__(self, state):
         self.__init__(
-            base_url=state['base_url'], retry=state['urllib_retry'], exception_to_retry=state['exception_to_retry']
+            base_url=state['base_url'], retry=state['urllib3_retry'], exception_to_retry=state['exception_to_retry']
         )
 
-    def _patch_with_urllib_retry(self, func: Callable):
+    def _patch_with_urllib3_retry(self, func: Callable):
         """Ensures that retry_state contains current urllib3 Retry instance before function call."""
 
         @wraps(func)
         def wrapped(*args, **kwargs):
             bound_args = signature(func).bind(*args, **kwargs)
             retry_state = bound_args.arguments['retry_state']
-            if getattr(retry_state, 'urllib_retry', None) is None:
-                retry_state.urllib_retry = self.urllib_retry
+            if getattr(retry_state, 'urllib3_retry', None) is None:
+                retry_state.urllib3_retry = self.urllib3_retry
             return func(*args, **kwargs)
+
         return wrapped
 
     @staticmethod
-    def _get_urllib_response(retry_state: RetryCallState):
+    def _get_urllib_response(retry_state: RetryCallState) -> Optional[urllib3.HTTPResponse]:
         """Constructs urllib3 response from httpx response."""
 
+        httpx_response: Optional[httpx.Response]
         if retry_state.outcome.failed:
+            httpx_response = getattr(retry_state.outcome.exception(), 'response', None)
+        else:
+            httpx_response = retry_state.outcome.result()
+
+        if httpx_response is None:
             return None
 
         _httpx_to_urllib_http_version = {'HTTP/2': 20, 'HTTP/1.1': 11}
-        httpx_response: httpx.Response = retry_state.outcome.result()
         return urllib3.HTTPResponse(
             body=httpx_response.content,
             headers=httpx_response.headers,
             status=httpx_response.status_code,
             version=_httpx_to_urllib_http_version[httpx_response.http_version],
             reason=httpx_response.reason_phrase,
             preload_content=True,
             decode_content=False,
             request_method=httpx_response.request.method,
             request_url=httpx_response.request.url,
         )
 
-    def _get_stop_callback(self):
+    def _get_stop_callback(self) -> stop_base:
 
         class IsExhausted(stop_base):
             """Callback wrapped in callable class to match BaseRetrying signature."""
 
-            @self._patch_with_urllib_retry
+            @self._patch_with_urllib3_retry
             def __call__(self, retry_state):
-                return retry_state.urllib_retry.is_exhausted()
+                retry: Retry = retry_state.urllib3_retry  # noqa:
+                return retry.is_exhausted()
 
         return IsExhausted()
 
-    def _get_wait_callback(self):
+    def _get_wait_callback(self) -> wait_base:
         outer_self = self
 
         class GetBackoffTime(wait_base):
             """Callback wrapped in callable class to match BaseRetrying signature."""
 
-            @self._patch_with_urllib_retry
+            @self._patch_with_urllib3_retry
             def __call__(self, retry_state):
                 response = outer_self._get_urllib_response(retry_state)
-                if response and retry_state.urllib_retry.respect_retry_after_header:
-                    retry_after = retry_state.urllib_retry.get_retry_after(response)
+                retry: Retry = retry_state.urllib3_retry  # noqa:
+                if response and retry.respect_retry_after_header:
+                    retry_after = retry.get_retry_after(response)
                     if retry_after:
                         return retry_state
-                return retry_state.urllib_retry.get_backoff_time()
+                return retry.get_backoff_time()
 
         return GetBackoffTime()
 
-    def _get_retry_callback(self):
-
+    def _get_retry_callback(self) -> retry_base:
         class IsRetry(retry_base):
             """Callback wrapped in callable class to match BaseRetrying signature."""
 
-            @self._patch_with_urllib_retry
+            def _should_retry_exception(self, retry_state) -> bool:
+                """Returns False if either can't map the exception"""
+
+                exception = retry_state.outcome.exception()
+                urllib3_exception = httpx_exception_to_urllib3_exception(exception)
+
+                try:
+                    map_urllib3_exception_for_retrying(urllib3_exception)
+                except RuntimeError:
+                    # exception will be reraised
+                    return False
+
+                return isinstance(exception, retry_state.retry_object.exception_to_retry)
+
+            @self._patch_with_urllib3_retry
             def __call__(self, retry_state):
+                httpx_response: Optional[httpx.Response]
                 if retry_state.outcome.failed:
-                    exception = retry_state.outcome.exception()
-                    return isinstance(exception, retry_state.retry_object.exception_to_retry)
+                    httpx_response = getattr(retry_state.outcome.exception(), 'response', None)
+                else:
+                    httpx_response = retry_state.outcome.result()
 
-                httpx_response: httpx.Response = retry_state.outcome.result()
-                has_retry_after = bool(httpx_response.headers.get("Retry-After", False))
+                if httpx_response is None:
+                    return self._should_retry_exception(retry_state)
 
-                return retry_state.urllib_retry.is_retry(
+                has_retry_after = bool(httpx_response.headers.get("Retry-After", False))
+                retry: Retry = retry_state.urllib3_retry  # noqa:
+                return retry.is_retry(
                     method=httpx_response.request.method, status_code=httpx_response.status_code,
                     has_retry_after=has_retry_after
                 )
 
         return IsRetry()
 
     def _get_after_callback(self):
 
-        @self._patch_with_urllib_retry
+        @self._patch_with_urllib3_retry
         def increment(retry_state: RetryCallState):
-            retry: Retry = retry_state.urllib_retry
+            """This function:
+            * tries to extract response from retry_state: either from the retry_state outcome or the raised exception
+                `response` field
+            * if response is found maps it to urllib3.HTTPReponse object and passes it to the wrapped urllib3.Retry
+                increment method
+            * otherwise maps the httpx exception to the urllib3 exception and passes it to the wrapped urllib3.Retry
+                increment method
+            """
+
+            retry: Retry = retry_state.urllib3_retry  # noqa:
             bound_args = signature(retry_state.fn).bind(*retry_state.args, **retry_state.kwargs)
 
             response = self._get_urllib_response(retry_state)
-            exception = retry_state.outcome.exception() if retry_state.outcome.failed else None
+            exception = None
+            if response is None:
+                exception = httpx_exception_to_urllib3_exception(retry_state.outcome.exception())
+                # should not raise RuntimeError as it is checked inside the retry callback
+                exception = map_urllib3_exception_for_retrying(exception)
 
             try:
-                retry_state.urllib_retry = retry.increment(
+                retry_state.urllib3_retry = retry.increment(
                     method=bound_args.arguments['method'],
-                    url=f'{self.base_url}{bound_args.arguments["path"]}',
+                    url=f'{self.base_url}{bound_args.arguments["url"]}',
                     response=response,
-                    error=httpx_exception_to_urllib_exception(exception) if exception else None,
+                    error=exception,
+                    _stacktrace=sys.exc_info()[2]
                 )
             except urllib3.exceptions.MaxRetryError:
                 # retry.increment raises MaxRetryError when exhausted. We want to delegate checking if the process
-                # should be stopped to the stop callback.
-                retry_state.urllib_retry = Retry(total=-1)
+                # should be stopped to the stop callback. MaxRetryError is raised if and only if retry.is_exhausted of
+                # the resulting exception is True.
+                retry_state.urllib3_retry = Retry(total=-1)
 
         return increment
 
 
 class SyncRetryingOverURLLibRetry(RetryingOverURLLibRetry, Retrying):
     pass
```

### Comparing `toloka-kit-1.1.4/src/client/project/__init__.py` & `toloka-kit-1.2.0/src/client/project/__init__.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/project/__init__.pyi` & `toloka-kit-1.2.0/src/client/project/__init__.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/project/field_spec.py` & `toloka-kit-1.2.0/src/client/project/field_spec.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/project/field_spec.pyi` & `toloka-kit-1.2.0/src/client/project/field_spec.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/project/localization.py` & `toloka-kit-1.2.0/src/client/project/localization.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/project/localization.pyi` & `toloka-kit-1.2.0/src/client/project/localization.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/project/task_spec.py` & `toloka-kit-1.2.0/src/client/project/task_spec.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/project/task_spec.pyi` & `toloka-kit-1.2.0/src/client/project/task_spec.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/project/template_builder/__init__.py` & `toloka-kit-1.2.0/src/client/project/template_builder/__init__.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 __all__ = [
-
     'actions',
     'base',
     'conditions',
     'data',
     'fields',
     'helpers',
     'layouts',
     'plugins',
     'view',
-
     'TemplateBuilder',
     'get_input_and_output',
+    'RefComponent',
     'BulkActionV1',
     'NotifyActionV1',
     'OpenCloseActionV1',
     'OpenLinkActionV1',
     'PlayPauseActionV1',
     'RotateActionV1',
     'SetActionV1',
@@ -95,149 +94,147 @@
     'LinkGroupViewV1',
     'ListViewV1',
     'MapViewV1',
     'MarkdownViewV1',
     'TextViewV1',
     'VideoViewV1',
 ]
-
-from typing import Dict, List, Any, Union, Tuple
-
-from . import actions
-from . import base
-from . import conditions
-from . import data
-from . import fields
-from . import helpers
-from . import layouts
-from . import plugins
-from . import view
-
-from .actions import (
+import toloka.client.primitives.base
+import toloka.client.project.field_spec
+import toloka.client.project.template_builder.base
+import typing
+
+from toloka.client.project.template_builder import (
+    actions,
+    base,
+    conditions,
+    data,
+    fields,
+    helpers,
+    layouts,
+    plugins,
+    view,
+)
+from toloka.client.project.template_builder.actions import (
     BulkActionV1,
     NotifyActionV1,
     OpenCloseActionV1,
     OpenLinkActionV1,
     PlayPauseActionV1,
     RotateActionV1,
     SetActionV1,
     ToggleActionV1,
 )
-from .conditions import (
+from toloka.client.project.template_builder.base import RefComponent
+from toloka.client.project.template_builder.conditions import (
     AllConditionV1,
     AnyConditionV1,
     DistanceConditionV1,
     EmptyConditionV1,
     EqualsConditionV1,
     LinkOpenedConditionV1,
     NotConditionV1,
     PlayedConditionV1,
     PlayedFullyConditionV1,
     RequiredConditionV1,
     SameDomainConditionV1,
     SchemaConditionV1,
     SubArrayConditionV1,
 )
-from .data import (
+from toloka.client.project.template_builder.data import (
     InputData,
     InternalData,
     LocalData,
     LocationData,
     OutputData,
     RelativeData,
 )
-from .fields import (
+from toloka.client.project.template_builder.fields import (
     AudioFieldV1,
     ButtonRadioFieldV1,
-    GroupFieldOption,
     ButtonRadioGroupFieldV1,
     CheckboxFieldV1,
     CheckboxGroupFieldV1,
     DateFieldV1,
     EmailFieldV1,
     FileFieldV1,
+    GroupFieldOption,
     ImageAnnotationFieldV1,
     ListFieldV1,
     MediaFileFieldV1,
     NumberFieldV1,
     PhoneNumberFieldV1,
     RadioGroupFieldV1,
     SelectFieldV1,
-    TextFieldV1,
     TextAnnotationFieldV1,
+    TextFieldV1,
     TextareaFieldV1,
 )
-from .helpers import (
+from toloka.client.project.template_builder.helpers import (
     ConcatArraysHelperV1,
     Entries2ObjectHelperV1,
     IfHelperV1,
     JoinHelperV1,
     Object2EntriesHelperV1,
     ReplaceHelperV1,
     SearchQueryHelperV1,
     SwitchHelperV1,
     TextTransformHelperV1,
     TransformHelperV1,
     TranslateHelperV1,
     YandexDiskProxyHelperV1,
 )
-from .layouts import (
+from toloka.client.project.template_builder.layouts import (
     BarsLayoutV1,
     ColumnsLayoutV1,
     CompareLayoutItem,
     CompareLayoutV1,
     SideBySideLayoutV1,
     SidebarLayoutV1,
 )
-from .plugins import (
+from toloka.client.project.template_builder.plugins import (
+    HotkeysPluginV1,
     ImageAnnotationHotkeysPluginV1,
     TextAnnotationHotkeysPluginV1,
-    HotkeysPluginV1,
-    TriggerPluginV1,
     TolokaPluginV1,
+    TriggerPluginV1,
 )
-from .view import (
+from toloka.client.project.template_builder.view import (
     ActionButtonViewV1,
     AlertViewV1,
     AudioViewV1,
     CollapseViewV1,
     DeviceFrameViewV1,
     DividerViewV1,
     GroupViewV1,
     IframeViewV1,
     ImageViewV1,
     LabeledListViewV1,
-    LinkViewV1,
     LinkGroupViewV1,
+    LinkViewV1,
     ListViewV1,
     MapViewV1,
     MarkdownViewV1,
     TextViewV1,
     VideoViewV1,
 )
-from .base import ComponentType, BaseComponent, base_component_or
-from ..field_spec import FieldSpec, JsonSpec
-from ...primitives.base import BaseTolokaObject
-from ....util import traverse_dicts_recursively
-
-
-class TemplateBuilder(BaseTolokaObject):
-
-    view: BaseComponent  # noqa: F811
-    plugins: List[BaseComponent]  # noqa: F811
-    vars: Dict[str, base_component_or(Any)]
-
 
-def get_input_and_output(tb_config: Union[dict, TemplateBuilder]) -> Tuple[Dict[str, FieldSpec], Dict[str, FieldSpec]]:
-    input_spec = {}
-    output_spec = {}
 
-    if isinstance(tb_config, TemplateBuilder):
-        tb_config = tb_config.unstructure()
+class TemplateBuilder(toloka.client.primitives.base.BaseTolokaObject):
+    def __init__(
+        self,
+        *,
+        view: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
+        plugins: typing.Optional[typing.List[toloka.client.project.template_builder.base.BaseComponent]] = None,
+        vars: typing.Optional[typing.Dict[str, typing.Any]] = None
+    ) -> None:
+        """Method generated by attrs for class TemplateBuilder.
+        """
+        ...
+
+    _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
+    view: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
+    plugins: typing.Optional[typing.List[toloka.client.project.template_builder.base.BaseComponent]]
+    vars: typing.Optional[typing.Dict[str, typing.Any]]
 
-    for obj in traverse_dicts_recursively(tb_config):
-        if obj.get('type') == ComponentType.DATA_INPUT.value:
-            input_spec[obj['path']] = JsonSpec()
-        elif obj.get('type') == ComponentType.DATA_OUTPUT.value:
-            output_spec[obj['path']] = JsonSpec()
 
-    return input_spec, output_spec
+def get_input_and_output(tb_config: typing.Union[dict, TemplateBuilder]) -> typing.Tuple[typing.Dict[str, toloka.client.project.field_spec.FieldSpec], typing.Dict[str, toloka.client.project.field_spec.FieldSpec]]: ...
```

### Comparing `toloka-kit-1.1.4/src/client/project/template_builder/actions.pyi` & `toloka-kit-1.2.0/src/client/project/template_builder/actions.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -11,33 +11,33 @@
 ]
 import toloka.client.project.template_builder.base
 import toloka.util._extendable_enum
 import typing
 
 
 class BaseActionV1(toloka.client.project.template_builder.base.BaseComponent, metaclass=toloka.client.project.template_builder.base.VersionedBaseComponentMetaclass):
-    """Perform various actions, such as showing notifications.
+    """A base class for actions.
     """
 
     def __init__(self, *, version: typing.Optional[str] = '1.0.0') -> None:
         """Method generated by attrs for class BaseActionV1.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     version: typing.Optional[str]
 
 
 class BulkActionV1(BaseActionV1):
-    """Use this component to call multiple actions at the same time, like to show more than one notification when a button is clicked.
+    """A group of actions to be called together.
+
+    For more information, see [action.bulk](https://toloka.ai/docs/template-builder/reference/action.bulk).
 
-    Actions are invoked in the order in which they are listed. This means that if two actions write a value to the same
-    variable, the variable will always have the second value.
     Attributes:
-        payload: An array of actions that you want to call.
+        payload: A list of actions.
     """
 
     def __init__(
         self,
         payload: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[toloka.client.project.template_builder.base.BaseComponent]]] = None,
         *,
         version: typing.Optional[str] = '1.0.0'
@@ -48,42 +48,40 @@
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     version: typing.Optional[str]
     payload: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[toloka.client.project.template_builder.base.BaseComponent]]]
 
 
 class NotifyActionV1(BaseActionV1):
-    """The component creates a message in the lower-left corner of the screen.
+    """The action shows a popup message.
+
+    For more information, see [action.notify](https://toloka.ai/docs/template-builder/reference/action.notify).
 
-    You can set the how long the message will be active, the delay before displaying it, and the background color.
     Attributes:
-        payload: Parameters for the message.
+        payload: Popup parameters.
     """
 
     class Payload(toloka.client.project.template_builder.base.BaseTemplate):
-        """Parameters for the message.
+        """Popup parameters.
 
         Attributes:
-            content: Message text
-            theme: The background color of the message.
-            delay: The duration of the delay (in milliseconds) before the message appears.
-            duration: The duration of the message activity (in milliseconds), which includes the duration of the delay
-                before displaying it.
-                For example, if duration is 1000 and delay is 400, the message will be displayed for
-                600 milliseconds.
+            content: Popup content. You can assign text or other components to the `content`.
+            theme: A background color.
+            delay: A delay in milliseconds before showing the popup.
+            duration: A duration in milliseconds of showing the popup. It includes the delay.
         """
 
         class Theme(toloka.util._extendable_enum.ExtendableStrEnum):
-            """The background color of the message.
+            """The background color of a popup.
 
             Attributes:
-                INFO: blue
-                SUCCESS: green
-                WARNING: yellow
-                DANGER: red
+                INFO: Blue.
+                SUCCESS: Green.
+                WARNING: Yellow.
+                DANGER: Red.
             """
 
             DANGER = 'danger'
             INFO = 'info'
             SUCCESS = 'success'
             WARNING = 'warning'
 
@@ -117,21 +115,23 @@
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     version: typing.Optional[str]
     payload: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, Payload]]
 
 
 class OpenCloseActionV1(BaseActionV1):
-    """This component changes the display mode of another component by opening or closing it.
+    """The action changes the display mode of another component.
+
+    It can expand an [image](toloka.client.project.template_builder.view.ImageViewV1.md) to a full screen
+    or collapse a [section](toloka.client.project.template_builder.view.CollapseViewV1.md).
+
+    For more information, see [action.open-close](https://toloka.ai/docs/template-builder/reference/action.open-close).
 
-    What happens to the component depends on the type of component:
-        view.image — expands the image to full screen.
-        view.collapse — expands or collapses a collapsible section of content.
     Attributes:
-        view: Points to the component to perform the action with.
+        view: References the component to perform the action with.
     """
 
     def __init__(
         self,
         view: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, toloka.client.project.template_builder.base.RefComponent]] = None,
         *,
         version: typing.Optional[str] = '1.0.0'
@@ -142,19 +142,20 @@
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     version: typing.Optional[str]
     view: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, toloka.client.project.template_builder.base.RefComponent]]
 
 
 class OpenLinkActionV1(BaseActionV1):
-    """Opens a new tab in the browser with the specified web page.
+    """The action opens an URL in a new browser tab.
+
+    For more information, see [action.open-link](https://toloka.ai/docs/template-builder/reference/action.open-link).
 
-    For example, you can open a link when a button is clicked.
     Attributes:
-        payload: URL of the web page.
+        payload: The URL.
     """
 
     def __init__(
         self,
         payload: typing.Optional[typing.Any] = None,
         *,
         version: typing.Optional[str] = '1.0.0'
@@ -165,21 +166,20 @@
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     version: typing.Optional[str]
     payload: typing.Optional[typing.Any]
 
 
 class PlayPauseActionV1(BaseActionV1):
-    """This component controls audio or video playback. It stops playback in progress or starts if it is stopped.
+    """The action pauses an audio or video player or resumes it.
 
-    For example, this component will allow you to play two videos simultaneously.
+    For more information, see [action.play-pause](https://toloka.ai/docs/template-builder/reference/action.play-pause).
 
-    You can also stop or start playback for some event (plugin. trigger) or by pressing the hotkey (plugin.hotkeys).
     Attributes:
-        view: Points to the component that plays audio or video.
+        view: A reference to the audio or video player.
     """
 
     def __init__(
         self,
         view: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, toloka.client.project.template_builder.base.RefComponent]] = None,
         *,
         version: typing.Optional[str] = '1.0.0'
@@ -190,20 +190,21 @@
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     version: typing.Optional[str]
     view: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, toloka.client.project.template_builder.base.RefComponent]]
 
 
 class RotateActionV1(BaseActionV1):
-    """Rotates the specified component by 90 degrees.
+    """The action rotates a component by 90 degrees.
+
+    For more information, see [action.rotate](https://toloka.ai/docs/template-builder/reference/action.rotate).
 
-    By default it rotates to the right, but you can specify the direction in the payload property.
     Attributes:
-        view: Points to the component to perform the action with.
-        payload: Sets the direction of rotation.
+        view: A reference to the component.
+        payload: The direction of rotation.
     """
 
     class Payload(toloka.util._extendable_enum.ExtendableStrEnum):
         """An enumeration.
         """
 
         LEFT = 'left'
@@ -223,51 +224,80 @@
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     version: typing.Optional[str]
     view: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, toloka.client.project.template_builder.base.RefComponent]]
     payload: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, Payload]]
 
 
 class SetActionV1(BaseActionV1):
-    """Sets the value from payload in the data in the data property.
+    """The action sets the value of a data field.
+
+    For more information, see [action.set](https://toloka.ai/docs/template-builder/reference/action.set).
+
+    Example:
+        The [hot key](toloka.client.project.template_builder.plugins.HotkeysPluginV1.md) `1`
+        fills a [text field](toloka.client.project.template_builder.fields.TextFieldV1.md) with a predefined text.
+        The [RefComponent](toloka.client.project.template_builder.base.RefComponent.md) is used to reference the output data field.
+
+        >>> from toloka.client.project.template_builder import *
+        >>> from toloka.client.project.template_builder.base import RefComponent
+        >>>
+        >>> tb_config = TemplateBuilder(
+        >>>     vars={'0': OutputData('result')},
+        >>>     view=TextFieldV1(
+        >>>         data=RefComponent('vars.0'),
+        >>>         label=InputData('question'),
+        >>>     ),
+        >>>     plugins=[
+        >>>         HotkeysPluginV1(
+        >>>             key_1=SetActionV1(
+        >>>                 data=RefComponent('vars.0'),
+        >>>                 payload='It is not a question'
+        >>>             )
+        >>>         )
+        >>>     ]
+        >>> )
+        ...
 
     Attributes:
-        data: Data with values that will be processed or changed.
-        payload: The value to write to the data.
+        data: The data field to set.
+        payload: The value.
     """
 
     def __init__(
         self,
-        data: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
+        data: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, toloka.client.project.template_builder.base.RefComponent]] = None,
         payload: typing.Optional[typing.Any] = None,
         *,
         version: typing.Optional[str] = '1.0.0'
     ) -> None:
         """Method generated by attrs for class SetActionV1.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     version: typing.Optional[str]
-    data: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
+    data: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, toloka.client.project.template_builder.base.RefComponent]]
     payload: typing.Optional[typing.Any]
 
 
 class ToggleActionV1(BaseActionV1):
-    """The component changes the value in the data from true to false and vice versa.
+    """The action toggles the value of a boolean data field.
+
+    For more information, see [action.toggle](https://toloka.ai/docs/template-builder/reference/action.toggle).
 
     Attributes:
-        data: Data in which the value will be changed. The data type must be boolean.
+        data: The data field.
     """
 
     def __init__(
         self,
-        data: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
+        data: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, toloka.client.project.template_builder.base.RefComponent]] = None,
         *,
         version: typing.Optional[str] = '1.0.0'
     ) -> None:
         """Method generated by attrs for class ToggleActionV1.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     version: typing.Optional[str]
-    data: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
+    data: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, toloka.client.project.template_builder.base.RefComponent]]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `toloka-kit-1.1.4/src/client/project/template_builder/base.py` & `toloka-kit-1.2.0/src/client/project/template_builder/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,216 +1,228 @@
-__all__ = [
-    'ComponentType',
-    'BaseTemplateMetaclass',
-    'BaseTemplate',
-    'BaseComponent',
-    'BaseComponentOr',
-    'base_component_or',
-    'VersionedBaseComponentMetaclass',
-    'UnknownComponent',
-    'RefComponent',
-    'ListDirection',
-    'ListSize'
-]
-from enum import unique
-from typing import ClassVar, Type, Optional, Any, Union
-
-from ..._converter import converter
-from ...primitives.base import BaseTolokaObject, BaseTolokaObjectMetaclass
-from ...exceptions import SpecClassIdentificationError
-from ....util._codegen import attribute
-from ....util._extendable_enum import ExtendableStrEnum
-
-
-# TODO: split into several enums
-@unique
-class ComponentType(ExtendableStrEnum):
-    ACTION_BULK = 'action.bulk'
-    ACTION_NOTIFY = 'action.notify'
-    ACTION_OPEN_CLOSE = 'action.open-close'
-    ACTION_OPEN_LINK = 'action.open-link'
-    ACTION_PLAY_PAUSE = 'action.play-pause'
-    ACTION_ROTATE = 'action.rotate'
-    ACTION_SET = 'action.set'
-    ACTION_TOGGLE = 'action.toggle'
-    CONDITION_ALL = 'condition.all'
-    CONDITION_ANY = 'condition.any'
-    CONDITION_EMPTY = 'condition.empty'
-    CONDITION_EQUALS = 'condition.equals'
-    CONDITION_LINK_OPENED = 'condition.link-opened'
-    CONDITION_NOT = 'condition.not'
-    CONDITION_PLAYED = 'condition.played'
-    CONDITION_PLAYED_FULLY = 'condition.played-fully'
-    CONDITION_REQUIRED = 'condition.required'
-    CONDITION_SAME_DOMAIN = 'condition.same-domain'
-    CONDITION_SCHEMA = 'condition.schema'
-    CONDITION_SUB_ARRAY = 'condition.sub-array'
-    CONDITION_YANDEX_DISTANCE = '@yandex-toloka/condition.distance'
-    DATA_INPUT = 'data.input'
-    DATA_INTERNAL = 'data.internal'
-    DATA_LOCAL = 'data.local'
-    DATA_LOCATION = '@yandex-toloka/data.location'
-    DATA_OUTPUT = 'data.output'
-    DATA_RELATIVE = 'data.relative'
-    FIELD_AUDIO = 'field.audio'
-    FIELD_BUTTON_RADIO = 'field.button-radio'
-    FIELD_BUTTON_RADIO_GROUP = 'field.button-radio-group'
-    FIELD_CHECKBOX = 'field.checkbox'
-    FIELD_CHECKBOX_GROUP = 'field.checkbox-group'
-    FIELD_DATE = 'field.date'
-    FIELD_EMAIL = 'field.email'
-    FIELD_FILE = 'field.file'
-    FIELD_IMAGE_ANNOTATION = 'field.image-annotation'
-    FIELD_LIST = 'field.list'
-    FIELD_MEDIA_FILE = 'field.media-file'
-    FIELD_NUMBER = 'field.number'
-    FIELD_PHONE_NUMBER = 'field.phone-number'
-    FIELD_RADIO_GROUP = 'field.radio-group'
-    FIELD_SELECT = 'field.select'
-    FIELD_TEXT = 'field.text'
-    FIELD_TEXT_ANNOTATION = 'field.text-annotation'
-    FIELD_TEXTAREA = 'field.textarea'
-    HELPER_CONCAT_ARRAYS = 'helper.concat-arrays'
-    HELPER_ENTRIES2OBJECT = 'helper.entries2object'
-    HELPER_IF = 'helper.if'
-    HELPER_JOIN = 'helper.join'
-    HELPER_OBJECT2ENTRIES = 'helper.object2entries'
-    HELPER_REPLACE = 'helper.replace'
-    HELPER_SEARCH_QUERY = 'helper.search-query'
-    HELPER_SWITCH = 'helper.switch'
-    HELPER_TEXT_TRANSFORM = 'helper.text-transform'
-    HELPER_TRANSFORM = 'helper.transform'
-    HELPER_TRANSLATE = 'helper.translate'
-    HELPER_YANDEX_DISK_PROXY = '@yandex-toloka/helper.proxy'
-    LAYOUT_BARS = 'layout.bars'
-    LAYOUT_COLUMNS = 'layout.columns'
-    LAYOUT_COMPARE = 'layout.compare'
-    LAYOUT_SIDE_BY_SIDE = 'layout.side-by-side'
-    LAYOUT_SIDEBAR = 'layout.sidebar'
-    PLUGIN_IMAGE_ANNOTATION_HOTKEYS = 'plugin.field.image-annotation.hotkeys'
-    PLUGIN_TEXT_ANNOTATION_HOTKEYS = 'plugin.field.text-annotation.hotkeys'
-    PLUGIN_HOTKEYS = 'plugin.hotkeys'
-    PLUGIN_TRIGGER = 'plugin.trigger'
-    PLUGIN_TOLOKA = 'plugin.toloka'
-    VIEW_ACTION_BUTTON = 'view.action-button'
-    VIEW_ALERT = 'view.alert'
-    VIEW_AUDIO = 'view.audio'
-    VIEW_COLLAPSE = 'view.collapse'
-    VIEW_DEVICE_FRAME = 'view.device-frame'
-    VIEW_DIVIDER = 'view.divider'
-    VIEW_GROUP = 'view.group'
-    VIEW_IFRAME = 'view.iframe'
-    VIEW_IMAGE = 'view.image'
-    VIEW_LABELED_LIST = 'view.labeled-list'
-    VIEW_LINK = 'view.link'
-    VIEW_LINK_GROUP = 'view.link-group'
-    VIEW_LIST = 'view.list'
-    VIEW_MAP = 'view.map'
-    VIEW_MARKDOWN = 'view.markdown'
-    VIEW_TEXT = 'view.text'
-    VIEW_VIDEO = 'view.video'
-
-
-class BaseTemplateMetaclass(BaseTolokaObjectMetaclass):
-    def __new__(mcs, *args, kw_only=False, **kwargs):
-        return super().__new__(mcs, *args, kw_only=kw_only, **kwargs)
-
-
-class BaseTemplate(BaseTolokaObject, metaclass=BaseTemplateMetaclass):
-
-    @classmethod
-    def structure(cls, data: dict):
-        if "$ref" in data and cls is not RefComponent:  # avoid recursion
-            return RefComponent.structure(data)
-        return super().structure(data)
-
-
-class BaseComponent(BaseTemplate, spec_enum=ComponentType, spec_field='type'):
-
-    @classmethod
-    def structure(cls, data: dict):
-        if not isinstance(data, dict):
-            raise TypeError
-
-        try:
-            return super().structure(data)
-        except SpecClassIdentificationError:
-            return UnknownComponent.structure(data)
-
-
-class BaseComponentOr(BaseTolokaObject):
-    type_: ClassVar[Type]
-    union_type: ClassVar[Type]
-
-    @classmethod
-    def structure(cls, data):
-        try:
-            return converter.structure(data, BaseComponent)
-        except Exception:
-            # TODO: add logging
-            # TODO: too general
-            return converter.structure(data, cls.type_)
-
-
-def base_component_or(type_: Type, class_name_suffix: Optional[str] = None):
-    if not hasattr(base_component_or, '_cache'):
-        base_component_or._cache = {}
-
-    if type_ not in base_component_or._cache:
-        name = f'BaseComponentOr{class_name_suffix or ("Any" if type_ == Any else type_.__name__)}'
-        cls = BaseTolokaObjectMetaclass(name, (BaseComponentOr,), {})
-        cls.__module__ = __name__
-        cls.type_ = type_
-        cls.union_type = cls.type_ if cls.type_ is Any else Union[BaseComponent, cls.type_]
-        base_component_or._cache[type_] = cls
-
-    return base_component_or._cache[type_]
-
-
-class VersionedBaseComponentMetaclass(BaseTemplateMetaclass):
-
-    def _validate_v1(self, attribute, value: str) -> str:
-        if not value.startswith('1.'):
-            raise ValueError('only v1 components are supported')
-        return value
-
-    def __new__(mcs, name, bases, namespace, **kwargs):
-        if 'version' not in namespace:
-            namespace['version'] = attribute(
-                default='1.0.0',
-                validator=VersionedBaseComponentMetaclass._validate_v1,
-                on_setattr=VersionedBaseComponentMetaclass._validate_v1,
-                kw_only=True
-            )
-            namespace.setdefault('__annotations__', {})['version'] = str
-        return super().__new__(mcs, name, bases, namespace, **kwargs)
-
-
-class UnknownComponent(BaseTemplate):
-    pass
-
-
-class RefComponent(BaseTemplate):
-    """If you need to insert the same or similar code snippets many times, reuse them.
-
-    This helps make your configuration shorter and makes it easier for you to edit duplicate chunks of code.
-
-    You can insert a code snippet from another part of the configuration anywhere inside the configuration. To do this,
-    use the structure RefComponent("path.to.element").
-
-    This is useful when you need to insert the same snippet at multiple places in your code. For example, if you need
-    to run the same action using multiple buttons, put this action in a variable and call it using RefComponent.
-    """
-
-    ref: str = attribute(origin='$ref')  # example: "vars.path.to.element"
-
-
-@unique
-class ListDirection(ExtendableStrEnum):
-    HORIZONTAL = 'horizontal'
-    VERTICAL = 'vertical'
-
-
-@unique
-class ListSize(ExtendableStrEnum):
-    M = 'm'
-    S = 's'
+__all__ = [
+    'ComponentType',
+    'BaseTemplateMetaclass',
+    'BaseTemplate',
+    'BaseComponent',
+    'BaseComponentOr',
+    'base_component_or',
+    'VersionedBaseComponentMetaclass',
+    'UnknownComponent',
+    'RefComponent',
+    'ListDirection',
+    'ListSize'
+]
+from enum import unique
+from typing import ClassVar, Type, Optional, Any, Union
+
+from ..._converter import converter
+from ...primitives.base import BaseTolokaObject, BaseTolokaObjectMetaclass
+from ...exceptions import SpecClassIdentificationError
+from ....util._codegen import attribute
+from ....util._extendable_enum import ExtendableStrEnum
+
+
+# TODO: split into several enums
+@unique
+class ComponentType(ExtendableStrEnum):
+    ACTION_BULK = 'action.bulk'
+    ACTION_NOTIFY = 'action.notify'
+    ACTION_OPEN_CLOSE = 'action.open-close'
+    ACTION_OPEN_LINK = 'action.open-link'
+    ACTION_PLAY_PAUSE = 'action.play-pause'
+    ACTION_ROTATE = 'action.rotate'
+    ACTION_SET = 'action.set'
+    ACTION_TOGGLE = 'action.toggle'
+    CONDITION_ALL = 'condition.all'
+    CONDITION_ANY = 'condition.any'
+    CONDITION_EMPTY = 'condition.empty'
+    CONDITION_EQUALS = 'condition.equals'
+    CONDITION_LINK_OPENED = 'condition.link-opened'
+    CONDITION_NOT = 'condition.not'
+    CONDITION_PLAYED = 'condition.played'
+    CONDITION_PLAYED_FULLY = 'condition.played-fully'
+    CONDITION_REQUIRED = 'condition.required'
+    CONDITION_SAME_DOMAIN = 'condition.same-domain'
+    CONDITION_SCHEMA = 'condition.schema'
+    CONDITION_SUB_ARRAY = 'condition.sub-array'
+    CONDITION_YANDEX_DISTANCE = '@yandex-toloka/condition.distance'
+    DATA_INPUT = 'data.input'
+    DATA_INTERNAL = 'data.internal'
+    DATA_LOCAL = 'data.local'
+    DATA_LOCATION = '@yandex-toloka/data.location'
+    DATA_OUTPUT = 'data.output'
+    DATA_RELATIVE = 'data.relative'
+    FIELD_AUDIO = 'field.audio'
+    FIELD_BUTTON_RADIO = 'field.button-radio'
+    FIELD_BUTTON_RADIO_GROUP = 'field.button-radio-group'
+    FIELD_CHECKBOX = 'field.checkbox'
+    FIELD_CHECKBOX_GROUP = 'field.checkbox-group'
+    FIELD_DATE = 'field.date'
+    FIELD_EMAIL = 'field.email'
+    FIELD_FILE = 'field.file'
+    FIELD_IMAGE_ANNOTATION = 'field.image-annotation'
+    FIELD_LIST = 'field.list'
+    FIELD_MEDIA_FILE = 'field.media-file'
+    FIELD_NUMBER = 'field.number'
+    FIELD_PHONE_NUMBER = 'field.phone-number'
+    FIELD_RADIO_GROUP = 'field.radio-group'
+    FIELD_SELECT = 'field.select'
+    FIELD_TEXT = 'field.text'
+    FIELD_TEXT_ANNOTATION = 'field.text-annotation'
+    FIELD_TEXTAREA = 'field.textarea'
+    HELPER_CONCAT_ARRAYS = 'helper.concat-arrays'
+    HELPER_ENTRIES2OBJECT = 'helper.entries2object'
+    HELPER_IF = 'helper.if'
+    HELPER_JOIN = 'helper.join'
+    HELPER_OBJECT2ENTRIES = 'helper.object2entries'
+    HELPER_REPLACE = 'helper.replace'
+    HELPER_SEARCH_QUERY = 'helper.search-query'
+    HELPER_SWITCH = 'helper.switch'
+    HELPER_TEXT_TRANSFORM = 'helper.text-transform'
+    HELPER_TRANSFORM = 'helper.transform'
+    HELPER_TRANSLATE = 'helper.translate'
+    HELPER_YANDEX_DISK_PROXY = '@yandex-toloka/helper.proxy'
+    LAYOUT_BARS = 'layout.bars'
+    LAYOUT_COLUMNS = 'layout.columns'
+    LAYOUT_COMPARE = 'layout.compare'
+    LAYOUT_SIDE_BY_SIDE = 'layout.side-by-side'
+    LAYOUT_SIDEBAR = 'layout.sidebar'
+    PLUGIN_IMAGE_ANNOTATION_HOTKEYS = 'plugin.field.image-annotation.hotkeys'
+    PLUGIN_TEXT_ANNOTATION_HOTKEYS = 'plugin.field.text-annotation.hotkeys'
+    PLUGIN_HOTKEYS = 'plugin.hotkeys'
+    PLUGIN_TRIGGER = 'plugin.trigger'
+    PLUGIN_TOLOKA = 'plugin.toloka'
+    VIEW_ACTION_BUTTON = 'view.action-button'
+    VIEW_ALERT = 'view.alert'
+    VIEW_AUDIO = 'view.audio'
+    VIEW_COLLAPSE = 'view.collapse'
+    VIEW_DEVICE_FRAME = 'view.device-frame'
+    VIEW_DIVIDER = 'view.divider'
+    VIEW_GROUP = 'view.group'
+    VIEW_IFRAME = 'view.iframe'
+    VIEW_IMAGE = 'view.image'
+    VIEW_LABELED_LIST = 'view.labeled-list'
+    VIEW_LINK = 'view.link'
+    VIEW_LINK_GROUP = 'view.link-group'
+    VIEW_LIST = 'view.list'
+    VIEW_MAP = 'view.map'
+    VIEW_MARKDOWN = 'view.markdown'
+    VIEW_TEXT = 'view.text'
+    VIEW_VIDEO = 'view.video'
+
+
+class BaseTemplateMetaclass(BaseTolokaObjectMetaclass):
+    def __new__(mcs, *args, kw_only=False, **kwargs):
+        return super().__new__(mcs, *args, kw_only=kw_only, **kwargs)
+
+
+class BaseTemplate(BaseTolokaObject, metaclass=BaseTemplateMetaclass):
+
+    @classmethod
+    def structure(cls, data: dict):
+        if "$ref" in data and cls is not RefComponent:  # avoid recursion
+            return RefComponent.structure(data)
+        return super().structure(data)
+
+
+class BaseComponent(BaseTemplate, spec_enum=ComponentType, spec_field='type'):
+
+    @classmethod
+    def structure(cls, data: dict):
+        if not isinstance(data, dict):
+            raise TypeError
+
+        try:
+            return super().structure(data)
+        except SpecClassIdentificationError:
+            return UnknownComponent.structure(data)
+
+
+class BaseComponentOr(BaseTolokaObject):
+    type_: ClassVar[Type]
+    union_type: ClassVar[Type]
+
+    @classmethod
+    def structure(cls, data):
+        try:
+            return converter.structure(data, BaseComponent)
+        except Exception:
+            # TODO: add logging
+            # TODO: too general
+            return converter.structure(data, cls.type_)
+
+
+def base_component_or(type_: Type, class_name_suffix: Optional[str] = None):
+    if not hasattr(base_component_or, '_cache'):
+        base_component_or._cache = {}
+
+    if type_ not in base_component_or._cache:
+        name = f'BaseComponentOr{class_name_suffix or ("Any" if type_ == Any else type_.__name__)}'
+        cls = BaseTolokaObjectMetaclass(name, (BaseComponentOr,), {})
+        cls.__module__ = __name__
+        cls.type_ = type_
+        cls.union_type = cls.type_ if cls.type_ is Any else Union[BaseComponent, cls.type_]
+        base_component_or._cache[type_] = cls
+
+    return base_component_or._cache[type_]
+
+
+class VersionedBaseComponentMetaclass(BaseTemplateMetaclass):
+
+    def _validate_v1(self, attribute, value: str) -> str:
+        if not value.startswith('1.'):
+            raise ValueError('only v1 components are supported')
+        return value
+
+    def __new__(mcs, name, bases, namespace, **kwargs):
+        if 'version' not in namespace:
+            namespace['version'] = attribute(
+                default='1.0.0',
+                validator=VersionedBaseComponentMetaclass._validate_v1,
+                on_setattr=VersionedBaseComponentMetaclass._validate_v1,
+                kw_only=True
+            )
+            namespace.setdefault('__annotations__', {})['version'] = str
+        return super().__new__(mcs, name, bases, namespace, **kwargs)
+
+
+class UnknownComponent(BaseTemplate):
+    pass
+
+
+class RefComponent(BaseTemplate):
+    """A reference to a component.
+
+    Pass to the `RefComponent` constructor a path in the Template Builder component hierarchy.
+
+    For more information, see [Reuse code](https://toloka.ai/docs/template-builder/best-practices/reuse).
+
+    Example:
+        >>> from toloka.client.project.template_builder import *
+        >>> from toloka.client.project.template_builder.base import RefComponent
+        >>>
+        >>> tb_config = TemplateBuilder(
+        >>>     vars = {
+        >>>         '0' : InputData('question'),
+        >>>         '1' : OutputData('answer')
+        >>>     },
+        >>>     view = TextFieldV1(
+        >>>         data = RefComponent('vars.1'),
+        >>>         label = RefComponent('vars.0')
+        >>>     )
+        >>> )
+        ...
+    """
+
+    ref: str = attribute(origin='$ref')  # example: "vars.path.to.element"
+
+
+@unique
+class ListDirection(ExtendableStrEnum):
+    HORIZONTAL = 'horizontal'
+    VERTICAL = 'vertical'
+
+
+@unique
+class ListSize(ExtendableStrEnum):
+    M = 'm'
+    S = 's'
```

### Comparing `toloka-kit-1.1.4/src/client/project/template_builder/base.pyi` & `toloka-kit-1.2.0/src/client/project/template_builder/base.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -178,23 +178,35 @@
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
 
 
 class RefComponent(BaseTemplate):
-    """If you need to insert the same or similar code snippets many times, reuse them.
+    """A reference to a component.
 
-    This helps make your configuration shorter and makes it easier for you to edit duplicate chunks of code.
+    Pass to the `RefComponent` constructor a path in the Template Builder component hierarchy.
 
-    You can insert a code snippet from another part of the configuration anywhere inside the configuration. To do this,
-    use the structure RefComponent("path.to.element").
+    For more information, see [Reuse code](https://toloka.ai/docs/template-builder/best-practices/reuse).
 
-    This is useful when you need to insert the same snippet at multiple places in your code. For example, if you need
-    to run the same action using multiple buttons, put this action in a variable and call it using RefComponent.
+    Example:
+        >>> from toloka.client.project.template_builder import *
+        >>> from toloka.client.project.template_builder.base import RefComponent
+        >>>
+        >>> tb_config = TemplateBuilder(
+        >>>     vars = {
+        >>>         '0' : InputData('question'),
+        >>>         '1' : OutputData('answer')
+        >>>     },
+        >>>     view = TextFieldV1(
+        >>>         data = RefComponent('vars.1'),
+        >>>         label = RefComponent('vars.0')
+        >>>     )
+        >>> )
+        ...
     """
 
     def __init__(self, ref: typing.Optional[str] = None) -> None:
         """Method generated by attrs for class RefComponent.
         """
         ...
```

### Comparing `toloka-kit-1.1.4/src/client/project/template_builder/conditions.py` & `toloka-kit-1.2.0/src/client/project/template_builder/conditions.py`

 * *Files 23% similar despite different names*

```diff
@@ -28,39 +28,33 @@
         if 'hint' not in namespace:
             namespace['hint'] = attribute(kw_only=True)
             namespace.setdefault('__annotations__', {})['hint'] = base_component_or(Any)
         return super().__new__(mcs, name, bases, namespace, **kwargs)
 
 
 class BaseConditionV1(BaseComponent, metaclass=BaseConditionV1Metaclass):
-    """Check an expression against a condition.
-
-    For example, you can check that a text field is filled in.
+    """A base class for conditions.
 
     Attributes:
-        hint: Validation error message that a Toloker will see.
+        hint: A hint that is shown if the condition is not met.
     """
 
     pass
 
 
 @inherit_docstrings
 class AllConditionV1(BaseConditionV1, spec_value=ComponentType.CONDITION_ALL):
-    """Checks that all child conditions are met.
+    """Checks that all nested conditions are met.
 
-    If any of the conditions is not met, the component returns 'false'.
+    For more information, see [condition.all](https://toloka.ai/docs/template-builder/reference/condition.all).
 
-    If you only need one out of several conditions to be met, use the condition.any component. You can also combine
-    these components.
     Attributes:
-        conditions: A set of conditions that must be met.
+        conditions: A list of conditions.
 
     Example:
-        How to check several conditions.
-
         >>> coordinates_validation = tb.conditions.AllConditionV1(
         >>>     [
         >>>         tb.conditions.RequiredConditionV1(
         >>>             tb.data.OutputData('performer_coordinates'),
         >>>             hint="Couldn't get your coordinates. Please enable geolocation.",
         >>>         ),
         >>>         tb.conditions.DistanceConditionV1(
@@ -75,40 +69,39 @@
     """
 
     conditions: base_component_or(List[BaseComponent], 'ListBaseComponent')  # noqa: F821
 
 
 @inherit_docstrings
 class AnyConditionV1(BaseConditionV1, spec_value=ComponentType.CONDITION_ANY):
-    """Checks that at least one of the child conditions is met.
+    """Checks that at least one nested condition is met.
 
-    If none of the conditions is met, the component returns false.
+    For more information, see [condition.any](https://toloka.ai/docs/template-builder/reference/condition.any).
 
-    If you need all conditions to be met, use the condition.all component. You can also combine these components.
     Attributes:
-        conditions: A set of conditions, at least one of which must be met.
+        conditions: A list of conditions.
     """
 
     conditions: base_component_or(List[BaseComponent], 'ListBaseComponent')  # noqa: F821
 
 
 @inherit_docstrings
 class DistanceConditionV1(BaseConditionV1, spec_value=ComponentType.CONDITION_YANDEX_DISTANCE):
-    """This component checks whether the sent coordinates match the ones that you specified
+    """Checks a distance between two coordinates.
 
-    For example, you want a Toloker to take a photo of a specific place. The condition.distance component checks whether
-    the photo was taken at the location that you specified.
+    For more information, see [condition.distance](https://toloka.ai/docs/template-builder/reference/condition.distance).
 
     Attributes:
-        from_: First point.
-        to_: Second point.
-        max: The distance in meters by which the X and Y coordinates may differ.
+        from_: The first point.
+        to_: The second point.
+        max: The maximum distance in meters.
 
     Example:
-        How to check that a Toloker is in the right place.
+        The following condition gets Toloker's [location](toloka.client.project.template_builder.data.LocationData.md)
+        and checks that it is near the task location.
 
         >>> distance_condition = tb.conditions.DistanceConditionV1(
         >>>     tb.data.LocationData(),
         >>>     tb.data.InputData('coordinates'),
         >>>     500,
         >>>     hint='You are too far from the destination coordinates.',
         >>> ),
@@ -118,179 +111,145 @@
     from_: base_component_or(str) = attribute(origin='from')
     to_: base_component_or(str) = attribute(origin='to')
     max: base_component_or(float)
 
 
 @inherit_docstrings
 class EmptyConditionV1(BaseConditionV1, spec_value=ComponentType.CONDITION_EMPTY):
-    """Checks that the data is empty (undefined).
+    """Checks that data is empty or undefined.
 
-    Returns false if the data received a value.
+    For more information, see [condition.empty](https://toloka.ai/docs/template-builder/reference/condition.empty).
 
-    You can check:
-        Template data (data.*).
-        Data for the input field (field.*) that contains condition.empty.
     Attributes:
-        data: Data to check. If not specified, data is checked in the component that contains condition.empty.
+        data: Data to check. If not specified, data of the parent component is checked.
     """
 
     data: base_component_or(Any)
 
 
 @inherit_docstrings
 class EqualsConditionV1(BaseConditionV1, spec_value=ComponentType.CONDITION_EQUALS):
-    """Checks whether the original value is equal to the specified value.
+    """Checks whether two values are equal.
 
-    If it matches, it returns true, otherwise it returns false.
+    For more information, see [condition.equals](https://toloka.ai/docs/template-builder/reference/condition.equals).
 
-    When substituting values, you can refer to data.* or another element using $ref. You can also use helpers and
-    conditions to get the value.
     Attributes:
-        to: The value to compare with the original.
-            How to pass a value:
-            * Specify the value itself, like the number 42 or a string.
-            * Get the value from your data.
-            * Refer to another element using $ref.
-            * Use helpers and conditions to get the value.
-        data: Original value. If not specified, it uses the value returned by the parent component (the component that
-            contains condition.equals).
-            How to pass a value:
-                * Specify the value itself, like the number 42 or a string.
-                * Get the value from your data.
-                * Refer to another element using $ref.
-                * Use helpers and conditions to get the value.
+        data: The first value. If it is not specified, then the value returned by the parent component is used.
+        to: The value to compare with.
     """
 
     to: base_component_or(Any)
     data: base_component_or(Any)
 
 
 @inherit_docstrings
 class LinkOpenedConditionV1(BaseConditionV1, spec_value=ComponentType.CONDITION_LINK_OPENED):
-    """Checks that the Toloker clicked the link.
+    """Checks that a Toloker clicked a link.
 
-    Important: To trigger the condition, the Toloker must follow the link from the Toloka interface — you must give Tolokers
-    this option. The condition will not work if the Toloker opens the link from the browser address bar.
+    For more information, see [condition.link-opened](https://toloka.ai/docs/template-builder/reference/condition.link-opened).
 
-    This condition can be used in the view.link component and also anywhere you can use (conditions).
     Attributes:
-        url: The link that must be clicked.
+        url: The link URL.
     """
 
     url: base_component_or(Any)
 
 
 @inherit_docstrings
 class NotConditionV1(BaseConditionV1, spec_value=ComponentType.CONDITION_NOT):
-    """Returns the inverse of the specified condition.
+    """Inverts a condition.
+
+    For more information, see [condition.not](https://toloka.ai/docs/template-builder/reference/condition.not).
 
-    For example, if the specified condition is met (returns true), then condition.not will return false.
     Attributes:
-        condition: The condition for which the inverse is returned.
+        condition: The condition to invert.
     """
 
     condition: BaseComponent
 
 
 @inherit_docstrings
 class PlayedConditionV1(BaseConditionV1, spec_value=ComponentType.CONDITION_PLAYED):
-    """Checks the start of playback.
+    """Checks that playback has started.
 
-    Validation will be passed if playback is started. To play media with the condition.played check, you can use
-    view.audio and view.video. The condition.played check only works in the player's validation property.
+    For more information, see [condition.played](https://toloka.ai/docs/template-builder/reference/condition.played).
     """
 
     pass
 
 
 @inherit_docstrings
 class PlayedFullyConditionV1(BaseConditionV1, spec_value=ComponentType.CONDITION_PLAYED_FULLY):
-    """This component checks for the end of playback.
+    """Checks that playback is complete.
 
-    Validation is passed if playback is finished. To play media with the condition.played-fully check, you can use
-    view.audio and view.video. The condition.played-fully check only works in the player's validation property.
+    For more information, see [condition.played-fully](https://toloka.ai/docs/template-builder/reference/condition.played-fully).
     """
 
     pass
 
 
 @inherit_docstrings
 class RequiredConditionV1(BaseConditionV1, spec_value=ComponentType.CONDITION_REQUIRED):
-    """Checks that the data is filled in. This way you can get the Toloker to answer all the required questions.
+    """Checks that a data field is present in a response.
+
+    For more information, see [condition.required](https://toloka.ai/docs/template-builder/reference/condition.required).
 
-    If used inside the validation property, you can omit the data property and the same property will be used from the
-    parent component field (the one that contains the condition.required component).
     Attributes:
-        data: Data to be filled in. If the property is not specified, the data of the parent component (the one that
-            contains condition.required) is used.
+        data: The data field. If it is not specified, the data of the parent component is used.
 
     Example:
         How to check that image is uploaded.
 
         >>> image = tb.fields.MediaFileFieldV1(
         >>>     tb.data.OutputData('image'),
         >>>     tb.fields.MediaFileFieldV1.Accept(photo=True, gallery=True),
-        >>>     validation=tb.conditions.RequiredConditionV1(hint='Your must upload photo.'),
+        >>>     validation=tb.conditions.RequiredConditionV1(hint='You must upload a photo.'),
         >>> )
         ...
     """
 
     data: base_component_or(Any)
 
 
 @inherit_docstrings
 class SameDomainConditionV1(BaseConditionV1, spec_value=ComponentType.CONDITION_SAME_DOMAIN):
-    """Checks if the link that you entered belongs to a specific site. If it does, returns true, otherwise, false.
+    """Checks that domains in two URLs are the same.
 
-    Links must be specified in full, including the protocol (http, https, ftp).
-
-    The `www.` subdomain is ignored when checking, meaning that links to `www.example.com`
-    and `example.com` are considered to be the same.
-
-    How to pass a link address:
-
-    * Specify it explicitly as a string.
-    * [Get the value](https://toloka.ai/en/docs/template-builder/operations/work-with-data) from your data.
-    * Refer to another element using `$ref`.
-    * Use [helpers](https://toloka.ai/en/docs/template-builder/reference/helpers) and
-      [conditions](https://toloka.ai/en/docs/template-builder/reference/conditions) to get the value.
+    For more information, see [condition.same-domain](https://toloka.ai/docs/template-builder/reference/condition.same-domain).
 
     Attributes:
-        data: The link address to be checked. If you don't specify it, the value returned by the parent component
-            (the one that contains condition.same-domain) is used.
-        original: The link address that your link is compared to.
+        data: The first URL. If it is not specified, then the value returned by the parent component is used.
+        original: The second URL.
     """
 
     data: base_component_or(Any)
     original: base_component_or(Any)
 
 
 @inherit_docstrings
 class SchemaConditionV1(BaseConditionV1, spec_value=ComponentType.CONDITION_SCHEMA):
-    """Allows validating data using JSON Schema. This is a special format for describing data in JSON format.
+    """Validates data using the [JSON Schema](https://json-schema.org/learn/getting-started-step-by-step.html).
 
-    For example, you can describe the data type, the minimum and maximum values, and specify that all values must be
-    unique.
+    For more information, see [condition.schema](https://toloka.ai/docs/template-builder/reference/condition.schema).
 
-    This component is useful in the following cases:
-        * If available components don't provide everything you need to configure validation.
-        * If you already have a prepared JSON Schema configuration for the check and you want to use it.
     Attributes:
-        data: Data that should be checked.
+        data: Data to be validated.
         schema: The schema for validating data.
     """
 
     data: base_component_or(Any)
     schema: Dict  # TODO: support base_component_or(Dict)
 
 
 @inherit_docstrings
 class SubArrayConditionV1(BaseConditionV1, spec_value=ComponentType.CONDITION_SUB_ARRAY):
-    """Checks that the array in data is a subarray for parent.
+    """Checks that an array is a subarray of another array.
+
+    For more information, see [condition.sub-array](https://toloka.ai/docs/template-builder/reference/condition.sub-array).
 
     Attributes:
-        data: Subarray that is checked for in parent.
-        parent: The array where data is searched for.
+        data: The array to check.
+        parent: The array to look in.
     """
 
     data: base_component_or(Any)
     parent: base_component_or(Any)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `toloka-kit-1.1.4/src/client/project/template_builder/conditions.pyi` & `toloka-kit-1.2.0/src/client/project/template_builder/conditions.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -26,20 +26,18 @@
         bases,
         namespace,
         **kwargs
     ): ...
 
 
 class BaseConditionV1(toloka.client.project.template_builder.base.BaseComponent, metaclass=BaseConditionV1Metaclass):
-    """Check an expression against a condition.
-
-    For example, you can check that a text field is filled in.
+    """A base class for conditions.
 
     Attributes:
-        hint: Validation error message that a Toloker will see.
+        hint: A hint that is shown if the condition is not met.
     """
 
     def __init__(
         self,
         *,
         hint: typing.Optional[typing.Any] = None,
         version: typing.Optional[str] = '1.0.0'
@@ -50,28 +48,23 @@
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     hint: typing.Optional[typing.Any]
     version: typing.Optional[str]
 
 
 class AllConditionV1(BaseConditionV1):
-    """Checks that all child conditions are met.
-
-    If any of the conditions is not met, the component returns 'false'.
+    """Checks that all nested conditions are met.
 
-    If you only need one out of several conditions to be met, use the condition.any component. You can also combine
-    these components.
+    For more information, see [condition.all](https://toloka.ai/docs/template-builder/reference/condition.all).
 
     Attributes:
-        conditions: A set of conditions that must be met.
-        hint: Validation error message that a Toloker will see.
+        conditions: A list of conditions.
+        hint: A hint that is shown if the condition is not met.
 
     Examples:
-        How to check several conditions.
-
         >>> coordinates_validation = tb.conditions.AllConditionV1(
         >>>     [
         >>>         tb.conditions.RequiredConditionV1(
         >>>             tb.data.OutputData('performer_coordinates'),
         >>>             hint="Couldn't get your coordinates. Please enable geolocation.",
         >>>         ),
         >>>         tb.conditions.DistanceConditionV1(
@@ -99,23 +92,21 @@
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     hint: typing.Optional[typing.Any]
     version: typing.Optional[str]
     conditions: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[toloka.client.project.template_builder.base.BaseComponent]]]
 
 
 class AnyConditionV1(BaseConditionV1):
-    """Checks that at least one of the child conditions is met.
+    """Checks that at least one nested condition is met.
 
-    If none of the conditions is met, the component returns false.
-
-    If you need all conditions to be met, use the condition.all component. You can also combine these components.
+    For more information, see [condition.any](https://toloka.ai/docs/template-builder/reference/condition.any).
 
     Attributes:
-        conditions: A set of conditions, at least one of which must be met.
-        hint: Validation error message that a Toloker will see.
+        conditions: A list of conditions.
+        hint: A hint that is shown if the condition is not met.
     """
 
     def __init__(
         self,
         conditions: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[toloka.client.project.template_builder.base.BaseComponent]]] = None,
         *,
         hint: typing.Optional[typing.Any] = None,
@@ -128,27 +119,27 @@
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     hint: typing.Optional[typing.Any]
     version: typing.Optional[str]
     conditions: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[toloka.client.project.template_builder.base.BaseComponent]]]
 
 
 class DistanceConditionV1(BaseConditionV1):
-    """This component checks whether the sent coordinates match the ones that you specified
+    """Checks a distance between two coordinates.
 
-    For example, you want a Toloker to take a photo of a specific place. The condition.distance component checks whether
-    the photo was taken at the location that you specified.
+    For more information, see [condition.distance](https://toloka.ai/docs/template-builder/reference/condition.distance).
 
     Attributes:
-        from_: First point.
-        to_: Second point.
-        max: The distance in meters by which the X and Y coordinates may differ.
-        hint: Validation error message that a Toloker will see.
+        from_: The first point.
+        to_: The second point.
+        max: The maximum distance in meters.
+        hint: A hint that is shown if the condition is not met.
 
     Examples:
-        How to check that a Toloker is in the right place.
+        The following condition gets Toloker's [location](toloka.client.project.template_builder.data.LocationData.md)
+        and checks that it is near the task location.
 
         >>> distance_condition = tb.conditions.DistanceConditionV1(
         >>>     tb.data.LocationData(),
         >>>     tb.data.InputData('coordinates'),
         >>>     500,
         >>>     hint='You are too far from the destination coordinates.',
         >>> ),
@@ -173,25 +164,21 @@
     version: typing.Optional[str]
     from_: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]]
     to_: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]]
     max: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, float]]
 
 
 class EmptyConditionV1(BaseConditionV1):
-    """Checks that the data is empty (undefined).
-
-    Returns false if the data received a value.
+    """Checks that data is empty or undefined.
 
-    You can check:
-        Template data (data.*).
-        Data for the input field (field.*) that contains condition.empty.
+    For more information, see [condition.empty](https://toloka.ai/docs/template-builder/reference/condition.empty).
 
     Attributes:
-        data: Data to check. If not specified, data is checked in the component that contains condition.empty.
-        hint: Validation error message that a Toloker will see.
+        data: Data to check. If not specified, data of the parent component is checked.
+        hint: A hint that is shown if the condition is not met.
     """
 
     def __init__(
         self,
         data: typing.Optional[typing.Any] = None,
         *,
         hint: typing.Optional[typing.Any] = None,
@@ -204,36 +191,22 @@
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     hint: typing.Optional[typing.Any]
     version: typing.Optional[str]
     data: typing.Optional[typing.Any]
 
 
 class EqualsConditionV1(BaseConditionV1):
-    """Checks whether the original value is equal to the specified value.
-
-    If it matches, it returns true, otherwise it returns false.
+    """Checks whether two values are equal.
 
-    When substituting values, you can refer to data.* or another element using $ref. You can also use helpers and
-    conditions to get the value.
+    For more information, see [condition.equals](https://toloka.ai/docs/template-builder/reference/condition.equals).
 
     Attributes:
-        to: The value to compare with the original.
-            How to pass a value:
-            * Specify the value itself, like the number 42 or a string.
-            * Get the value from your data.
-            * Refer to another element using $ref.
-            * Use helpers and conditions to get the value.
-        data: Original value. If not specified, it uses the value returned by the parent component (the component that
-            contains condition.equals).
-            How to pass a value:
-                * Specify the value itself, like the number 42 or a string.
-                * Get the value from your data.
-                * Refer to another element using $ref.
-                * Use helpers and conditions to get the value.
-        hint: Validation error message that a Toloker will see.
+        to: The value to compare with.
+        data: The first value. If it is not specified, then the value returned by the parent component is used.
+        hint: A hint that is shown if the condition is not met.
     """
 
     def __init__(
         self,
         to: typing.Optional[typing.Any] = None,
         data: typing.Optional[typing.Any] = None,
         *,
@@ -248,24 +221,21 @@
     hint: typing.Optional[typing.Any]
     version: typing.Optional[str]
     to: typing.Optional[typing.Any]
     data: typing.Optional[typing.Any]
 
 
 class LinkOpenedConditionV1(BaseConditionV1):
-    """Checks that the Toloker clicked the link.
+    """Checks that a Toloker clicked a link.
 
-    Important: To trigger the condition, the Toloker must follow the link from the Toloka interface — you must give Tolokers
-    this option. The condition will not work if the Toloker opens the link from the browser address bar.
-
-    This condition can be used in the view.link component and also anywhere you can use (conditions).
+    For more information, see [condition.link-opened](https://toloka.ai/docs/template-builder/reference/condition.link-opened).
 
     Attributes:
-        url: The link that must be clicked.
-        hint: Validation error message that a Toloker will see.
+        url: The link URL.
+        hint: A hint that is shown if the condition is not met.
     """
 
     def __init__(
         self,
         url: typing.Optional[typing.Any] = None,
         *,
         hint: typing.Optional[typing.Any] = None,
@@ -278,21 +248,21 @@
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     hint: typing.Optional[typing.Any]
     version: typing.Optional[str]
     url: typing.Optional[typing.Any]
 
 
 class NotConditionV1(BaseConditionV1):
-    """Returns the inverse of the specified condition.
+    """Inverts a condition.
 
-    For example, if the specified condition is met (returns true), then condition.not will return false.
+    For more information, see [condition.not](https://toloka.ai/docs/template-builder/reference/condition.not).
 
     Attributes:
-        condition: The condition for which the inverse is returned.
-        hint: Validation error message that a Toloker will see.
+        condition: The condition to invert.
+        hint: A hint that is shown if the condition is not met.
     """
 
     def __init__(
         self,
         condition: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         *,
         hint: typing.Optional[typing.Any] = None,
@@ -305,21 +275,20 @@
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     hint: typing.Optional[typing.Any]
     version: typing.Optional[str]
     condition: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
 
 
 class PlayedConditionV1(BaseConditionV1):
-    """Checks the start of playback.
+    """Checks that playback has started.
 
-    Validation will be passed if playback is started. To play media with the condition.played check, you can use
-    view.audio and view.video. The condition.played check only works in the player's validation property.
+    For more information, see [condition.played](https://toloka.ai/docs/template-builder/reference/condition.played).
 
     Attributes:
-        hint: Validation error message that a Toloker will see.
+        hint: A hint that is shown if the condition is not met.
     """
 
     def __init__(
         self,
         *,
         hint: typing.Optional[typing.Any] = None,
         version: typing.Optional[str] = '1.0.0'
@@ -330,21 +299,20 @@
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     hint: typing.Optional[typing.Any]
     version: typing.Optional[str]
 
 
 class PlayedFullyConditionV1(BaseConditionV1):
-    """This component checks for the end of playback.
+    """Checks that playback is complete.
 
-    Validation is passed if playback is finished. To play media with the condition.played-fully check, you can use
-    view.audio and view.video. The condition.played-fully check only works in the player's validation property.
+    For more information, see [condition.played-fully](https://toloka.ai/docs/template-builder/reference/condition.played-fully).
 
     Attributes:
-        hint: Validation error message that a Toloker will see.
+        hint: A hint that is shown if the condition is not met.
     """
 
     def __init__(
         self,
         *,
         hint: typing.Optional[typing.Any] = None,
         version: typing.Optional[str] = '1.0.0'
@@ -355,31 +323,29 @@
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     hint: typing.Optional[typing.Any]
     version: typing.Optional[str]
 
 
 class RequiredConditionV1(BaseConditionV1):
-    """Checks that the data is filled in. This way you can get the Toloker to answer all the required questions.
+    """Checks that a data field is present in a response.
 
-    If used inside the validation property, you can omit the data property and the same property will be used from the
-    parent component field (the one that contains the condition.required component).
+    For more information, see [condition.required](https://toloka.ai/docs/template-builder/reference/condition.required).
 
     Attributes:
-        data: Data to be filled in. If the property is not specified, the data of the parent component (the one that
-            contains condition.required) is used.
-        hint: Validation error message that a Toloker will see.
+        data: The data field. If it is not specified, the data of the parent component is used.
+        hint: A hint that is shown if the condition is not met.
 
     Examples:
         How to check that image is uploaded.
 
         >>> image = tb.fields.MediaFileFieldV1(
         >>>     tb.data.OutputData('image'),
         >>>     tb.fields.MediaFileFieldV1.Accept(photo=True, gallery=True),
-        >>>     validation=tb.conditions.RequiredConditionV1(hint='Your must upload photo.'),
+        >>>     validation=tb.conditions.RequiredConditionV1(hint='You must upload a photo.'),
         >>> )
         ...
     """
 
     def __init__(
         self,
         data: typing.Optional[typing.Any] = None,
@@ -394,34 +360,22 @@
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     hint: typing.Optional[typing.Any]
     version: typing.Optional[str]
     data: typing.Optional[typing.Any]
 
 
 class SameDomainConditionV1(BaseConditionV1):
-    """Checks if the link that you entered belongs to a specific site. If it does, returns true, otherwise, false.
-
-    Links must be specified in full, including the protocol (http, https, ftp).
-
-    The `www.` subdomain is ignored when checking, meaning that links to `www.example.com`
-    and `example.com` are considered to be the same.
+    """Checks that domains in two URLs are the same.
 
-    How to pass a link address:
-
-    * Specify it explicitly as a string.
-    * [Get the value](https://toloka.ai/en/docs/template-builder/operations/work-with-data) from your data.
-    * Refer to another element using `$ref`.
-    * Use [helpers](https://toloka.ai/en/docs/template-builder/reference/helpers) and
-      [conditions](https://toloka.ai/en/docs/template-builder/reference/conditions) to get the value.
+    For more information, see [condition.same-domain](https://toloka.ai/docs/template-builder/reference/condition.same-domain).
 
     Attributes:
-        data: The link address to be checked. If you don't specify it, the value returned by the parent component
-            (the one that contains condition.same-domain) is used.
-        original: The link address that your link is compared to.
-        hint: Validation error message that a Toloker will see.
+        data: The first URL. If it is not specified, then the value returned by the parent component is used.
+        original: The second URL.
+        hint: A hint that is shown if the condition is not met.
     """
 
     def __init__(
         self,
         data: typing.Optional[typing.Any] = None,
         original: typing.Optional[typing.Any] = None,
         *,
@@ -436,27 +390,22 @@
     hint: typing.Optional[typing.Any]
     version: typing.Optional[str]
     data: typing.Optional[typing.Any]
     original: typing.Optional[typing.Any]
 
 
 class SchemaConditionV1(BaseConditionV1):
-    """Allows validating data using JSON Schema. This is a special format for describing data in JSON format.
-
-    For example, you can describe the data type, the minimum and maximum values, and specify that all values must be
-    unique.
+    """Validates data using the [JSON Schema](https://json-schema.org/learn/getting-started-step-by-step.html).
 
-    This component is useful in the following cases:
-        * If available components don't provide everything you need to configure validation.
-        * If you already have a prepared JSON Schema configuration for the check and you want to use it.
+    For more information, see [condition.schema](https://toloka.ai/docs/template-builder/reference/condition.schema).
 
     Attributes:
-        data: Data that should be checked.
+        data: Data to be validated.
         schema: The schema for validating data.
-        hint: Validation error message that a Toloker will see.
+        hint: A hint that is shown if the condition is not met.
     """
 
     def __init__(
         self,
         data: typing.Optional[typing.Any] = None,
         schema: typing.Optional[typing.Dict] = None,
         *,
@@ -471,20 +420,22 @@
     hint: typing.Optional[typing.Any]
     version: typing.Optional[str]
     data: typing.Optional[typing.Any]
     schema: typing.Optional[typing.Dict]
 
 
 class SubArrayConditionV1(BaseConditionV1):
-    """Checks that the array in data is a subarray for parent.
+    """Checks that an array is a subarray of another array.
+
+    For more information, see [condition.sub-array](https://toloka.ai/docs/template-builder/reference/condition.sub-array).
 
     Attributes:
-        data: Subarray that is checked for in parent.
-        parent: The array where data is searched for.
-        hint: Validation error message that a Toloker will see.
+        data: The array to check.
+        parent: The array to look in.
+        hint: A hint that is shown if the condition is not met.
     """
 
     def __init__(
         self,
         data: typing.Optional[typing.Any] = None,
         parent: typing.Optional[typing.Any] = None,
         *,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `toloka-kit-1.1.4/src/client/project/template_builder/fields.py` & `toloka-kit-1.2.0/src/client/project/template_builder/fields.py`

 * *Files 21% similar despite different names*

```diff
@@ -54,239 +54,229 @@
             namespace['validation'] = attribute(kw_only=True)
             annotations['validation'] = BaseComponent
         namespace['__annotations__'] = annotations
         return super().__new__(mcs, name, bases, namespace, **kwargs)
 
 
 class BaseFieldV1(BaseComponent, metaclass=BaseFieldV1Metaclass):
-    """Fields for entering data, such as a text field or drop-down list.
+    """A base class for input data fields.
+
+    Input fields are used to get data from Tolokers.
 
     Attributes:
-        data: Data with values that will be processed or changed.
-        label: Label above the component.
-        hint: Hint text.
-        validation: Validation based on condition.
+        data: A data path.
+        label: A label above the component.
+        hint: A hint.
+        validation: Validation rules.
     """
 
     pass
 
 
 @inherit_docstrings
 class AudioFieldV1(BaseFieldV1, spec_value=ComponentType.FIELD_AUDIO):
-    """Component for recording audio.
+    """A component for recording audio.
 
-    Works in the mobile app. In a browser, this component opens a window for uploading an audio file.
+    For more information, see [field.audio](https://toloka.ai/docs/template-builder/reference/field.audio).
 
     Attributes:
-        multiple: Determines whether multiple audio files can be recorded (or uploaded):
-            * `False` (default) — forbidden.
-            * `True` — allowed.
+        multiple:
+            * `True` — Multiple audio files can be recorded or uploaded.
+            * `False` — A single file can be recorded or uploaded.
+
+            Default value: `False`.
     """
 
     multiple: base_component_or(Any) = attribute(kw_only=True)
 
 
 @inherit_docstrings
 class ButtonRadioFieldV1(BaseFieldV1, spec_value=ComponentType.FIELD_BUTTON_RADIO):
-    """A component in the form of a button.
+    """A button to choose an answer.
 
-    A Toloker makes a choice by clicking on it.
+    For more information, see [field.button-radio](https://toloka.ai/docs/template-builder/reference/field.button-radio).
 
-    The size of the button depends on the size of the label.
     Attributes:
-        value_to_set: The value of the output data when the button is clicked.
+        value_to_set: A value to write to data.
     """
 
     value_to_set: base_component_or(Any) = attribute(origin='valueToSet')
 
 
 class GroupFieldOption(BaseTemplate):
-    """Option.
+    """A single option for components with multiple options.
 
     Attributes:
-        value: Returned value.
-        label: The text on the object.
-        hint: Additional information.
+        value: A value that is saved in data when the option is selected.
+        label: An option text.
+        hint: An additional description.
     """
 
     value: base_component_or(Any)
     label: base_component_or(Any)
     hint: base_component_or(Any) = attribute(kw_only=True)
 
 
 @inherit_docstrings
 class ButtonRadioGroupFieldV1(BaseFieldV1, spec_value=ComponentType.FIELD_BUTTON_RADIO_GROUP):
-    """A component with buttons that allow the Toloker to choose between the specified values.
+    """A group of buttons for choosing one option.
 
-    The minimum number of elements is one. Any type of data can be returned.
+    For more information, see [field.button-radio-group](https://toloka.ai/docs/template-builder/reference/field.button-radio-group).
 
-    The size of the button is determined by the length of the text on it.
     Attributes:
-        options: Array of information about the buttons.
+        options: A list of options.
 
     Example:
-        How to add buttons for classification task.
-
         >>> classification_buttons = tb.fields.ButtonRadioGroupFieldV1(
-        >>>     tb.data.OutputData(path='class'),
-        >>>     [
+        >>>     data=tb.data.OutputData(path='class'),
+        >>>     options=[
         >>>         tb.fields.GroupFieldOption('Cat', 'cat'),
         >>>         tb.fields.GroupFieldOption('Dog', 'dog'),
         >>>     ],
         >>>     validation=tb.conditions.RequiredConditionV1(hint='Choose one of the answer options'),
         >>> )
         ...
     """
 
     options: base_component_or(List[base_component_or(GroupFieldOption)], 'ListBaseComponentOrGroupFieldOption')  # noqa: F821
 
 
 @inherit_docstrings
 class CheckboxFieldV1(BaseFieldV1, spec_value=ComponentType.FIELD_CHECKBOX):
-    """Checkbox.
+    """A checkbox.
+
+    For more information, see [field.checkbox](https://toloka.ai/docs/template-builder/reference/field.checkbox).
 
     Attributes:
-        disabled: Property that disables the component. If `True`, the component will not be unavailable.
-        preserve_false: Property that specifies whether to return false values in the results. By default, if the
-            component returns `False`, this result will not be added to the output. To add `False` to the results, specify
-            `preserve_false=True`.
+        disabled: Disabling the checkbox.
+        preserve_false:
+            * `False` — If the checkbox is not selected then `False` is not added to the output data.
+            * `True` — The output data is always present whether the checkbox is selected or not.
+
+            Default value: `False`.
     """
 
     disabled: base_component_or(bool) = attribute(kw_only=True)
     preserve_false: base_component_or(bool) = attribute(origin='preserveFalse', kw_only=True)
 
 
 @inherit_docstrings
 class CheckboxGroupFieldV1(BaseFieldV1, spec_value=ComponentType.FIELD_CHECKBOX_GROUP):
-    """A group of options for selecting one or more responses.
+    """A group of checkboxes.
+
+    This component creates a dictionary in the output data. Values from `options` are used as keys in the dictionary.
+
+    For more information, see [field.checkbox-group](https://toloka.ai/docs/template-builder/reference/field.checkbox-group).
 
     Attributes:
-        options: Options, where value is the key that the option controls, and label is the text near the option.
-        disabled: If `True', the options are inactive.
-        preserve_false: Property that specifies whether to return false values in the results. By default, if the
-            component returns false, this result will not be added to the output. To add false to the results, specify
-            `preserve_false = True`.
+        options: A list of options.
+        disabled: Disabling the checkbox group.
+        preserve_false:
+            * `False` — If a checkbox from the group is not selected then its key is not added to the dictionary.
+            * `True` — The output dictionary contains all keys whether checkboxes are selected or not.
+
+            Default value: `False`.
     """
 
     options: base_component_or(List[base_component_or(GroupFieldOption)], 'ListBaseComponentOrGroupFieldOption')  # noqa: F821
     disabled: base_component_or(bool) = attribute(kw_only=True)
     preserve_false: base_component_or(bool) = attribute(origin='preserveFalse', kw_only=True)
 
 
 @inherit_docstrings
 class DateFieldV1(BaseFieldV1, spec_value=ComponentType.FIELD_DATE):
-    """A component for entering the date and time in the desired format and range.
+    """A field for entering a date and time.
+
+    For more information, see [field.date](https://toloka.ai/docs/template-builder/reference/field.date).
 
-    You can set a list of dates that the Toloker cannot select.
     Attributes:
-        data: Data with values that will be processed or changed.
-        format: Format of the date entered by the Toloker:
-            * date-time — date and time.
-            * date — date only.
-        label: Label above the component.
-        block_list: List of dates that the Toloker cannot select.
-            * block_list[]: Date that the Toloker cannot select.
-        hint: Hint text.
-        max: The latest date and time in the YYYY-MM-DD hh:mm format that the Toloker can select. Where:
-            * YYYY is the year.
-            * MM is the month.
-            * DD is the day.
-            * hh is the time in hours.
-            * mm is the time in minutes.
-        min: The earliest date and time in the YYYY-MM-DD hh:mm format that the Toloker can select. Where:
-            * YYYY is the year.
-            * MM is the month.
-            * DD is the day.
-            * hh is the time in hours.
-            * mm is the time in minutes.
-        placeholder: A semi-transparent label that is shown in the box when it is empty.
-        validation: Validation based on condition.
+        format: The format of the field:
+            * `date-time` — Date and time.
+            * `date` — Date only.
+        block_list: A list of dates that a Toloker can't select.
+        max: The latest date and time in the `YYYY-MM-DD hh:mm` format that a Toloker can select.
+        min: The earliest date and time in the `YYYY-MM-DD hh:mm` format that a Toloker can select.
+        placeholder: A text that is shown when no date is entered.
     """
 
     format: base_component_or(Any)
     block_list: base_component_or(List[base_component_or(Any)], 'ListBaseComponentOrAny') = attribute(  # noqa: F821
         origin='blockList',
         kw_only=True
     )
     max: base_component_or(Any) = attribute(kw_only=True)
     min: base_component_or(Any) = attribute(kw_only=True)
     placeholder: base_component_or(Any) = attribute(kw_only=True)
 
 
 @inherit_docstrings
 class EmailFieldV1(BaseFieldV1, spec_value=ComponentType.FIELD_EMAIL):
-    """Creates a field for entering an email address.
+    """A field for entering an email address.
+
+    For more information, see [field.email](https://toloka.ai/docs/template-builder/reference/field.email).
 
-    Checks that the text contains the @ character. You can set other conditions yourself.
     Attributes:
-        placeholder: A semi-transparent label that is shown in an empty field.
+        placeholder: A text that is shown when no address is entered.
     """
 
     placeholder: Any = attribute(kw_only=True)
 
 
 @inherit_docstrings
 class FileFieldV1(BaseFieldV1, spec_value=ComponentType.FIELD_FILE):
-    """This component can be used for uploading files. It's displayed in the interface as an upload button.
+    """A component for uploading files.
 
-    You can restrict the file types to upload in the "accept" property. By default, only one file can be uploaded,
-    but you can allow multiple files in the "multiple" property.
+    For more information, see [field.file](https://toloka.ai/docs/template-builder/reference/field.file).
 
-    If a Toloker logs in from a mobile device, it's more convenient to use field.media-file — it's adapted for mobile
-    devices and makes it easier to upload photos and videos.
     Attributes:
-        accept: A list of file types that can be uploaded. By default, you can upload any files.
-            Specify the types in the [certain format](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types).
-            For example, you can allow only images to be uploaded by adding the image/jpeg and image/png types.
-        multiple: Determines whether multiple files can be uploaded:
-            * `False` (default) — forbidden.
-            * `True` — allowed.
+        accept: A list of file types that can be uploaded.
+            Use [MIME types](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types).
+            For example, `image/jpeg`.
+            By default, you can upload any files.
+        multiple:
+            * `True` — Multiple files can be uploaded.
+            * `False` — A single file can be uploaded.
+
+            Default value: `False`.
     """
 
     accept: base_component_or(List[base_component_or(str)], 'ListBaseComponentOrStr')  # noqa: F821
     multiple: base_component_or(bool) = attribute(kw_only=True)
 
 
 @inherit_docstrings
 class ImageAnnotationFieldV1(BaseFieldV1, spec_value=ComponentType.FIELD_IMAGE_ANNOTATION):
-    """Adds an interface for selecting areas in images.
+    """A component for annotating areas in an image.
 
-    If you need to select different types of objects, classify the areas using the labels property.
+    For more information, see [field.image-annotation](https://toloka.ai/docs/template-builder/reference/field.image-annotation).
 
-    You can select areas using points, polygons, and rectangles. In the shapes property, you can keep some of the
-    selection modes and hide the rest.
     Attributes:
-        image: The image you want to select areas in.
-        disabled: Determines whether adding and deleting areas is allowed:
-            * `False` (default) — Allowed.
-            * `True` — Not allowed.
-            You can use this feature when creating an interface to check whether the selection is correct,
-             or if you need to allow selection only when a certain condition is met.
-        full_height: If `True`, the element takes up all the vertical free space. The element is set to a minimum height
-            of 400 pixels.
-        labels: Used to classify areas.
-            You can add several area types. When adding an area type, a button to select it appears in the interface,
-            and when setting a new value, a new area selection color is added.
-            This feature is instrumental if you need to select different types of objects: you can use one color to
-            select cars and a different one for pedestrians.
-        min_width: Minimum width of the element in pixels. Takes priority over max_width.
-        ratio: An array of two numbers that sets the relative dimensions of the sides: width (first number) to height
-            (second number). Not valid if `full_height=True`.
-        shapes: Used to add and hide selection modes: points, polygons, and rectangles. All three modes are available
-            by default.
-            Use this property if you only need to keep certain modes. Modes with the `True` value are available.
+        image: The URL of the image.
+        disabled: Disabling the component:
+            * `False` — Annotating is allowed.
+            * `True` — Annotating is disabled.
+
+            Default value: `False`.
+        full_height: If `True`, the component takes up all the vertical free space.
+            Note, that the minimum height required by the component is 400 pixels.
+        labels: Labels used to classify image areas.
+        min_width: The minimum width of the component in pixels.
+        ratio: A list with the aspect ratio of the component. Specify the relative width and then the height.
+            This setting is not used if `full_height=True`.
+        shapes: Area selection modes: `point`, `polygon`, and `rectangle`.
+            Use mode names as keys in the `shapes` dictionary. Modes set to `True` are available in the component.
+            By default, all modes are available.
     """
 
     class Label(BaseTemplate):
-        """At least two objects must be added to the array.
+        """An image area class.
 
         Attributes:
-            label: Text on the button for selecting a selection color.
-            value: The value to be written to the labels property data. Displayed to Tolokers as color options when
-                selecting areas.
+            label: A text on a button for selecting the area class.
+            value: A value used in output data.
         """
 
         label: base_component_or(str)
         value: base_component_or(str)
 
     @unique
     class Shape(ExtendableStrEnum):
@@ -302,250 +292,249 @@
     ratio: base_component_or(List[base_component_or(float)], 'ListBaseComponentOrFloat') = attribute(kw_only=True)  # noqa: F821
     shapes: base_component_or(Dict[base_component_or(Shape), base_component_or(bool)],
                               'DictBaseComponentOrShapeBaseComponentOrBool') = attribute(kw_only=True)  # noqa: F821
 
 
 @inherit_docstrings
 class ListFieldV1(BaseFieldV1, spec_value=ComponentType.FIELD_LIST):
-    """A component that allows a Toloker to add and remove list items, such as text fields to fill in.
+    """A component that allows a Toloker to add and remove list items, such as text fields.
 
-    This way you can allow a Toloker to give multiple answers to a question.
+    Use RelativeData(toloka.client.project.template_builder.data.RelativeData.md) in list items,
+    otherwise all list items will change the same data.
 
-    The list items can contain any component, including a list of other components. For example, this allows you to
-    create a table where you can add and delete rows.
+    For more information, see [field.list](https://toloka.ai/docs/template-builder/reference/field.list).
 
-    To add a new list item, the Toloker clicks the button. To remove an item, they click on the x on the right (it appears
-    when hovering over a list item).
-
-    To prevent a Toloker from adding too many list items, set the maximum list length. You can also use the editable
-    property to block Tolokers from changing a component, like when a certain event occurs.
-    Attributes:
-        render: Interface template for list items, such as a text field.
-            In nested field.* components, use data.relative for recording responses, otherwise all the list items will
-            have the same value.
-        button_label: Text on the button for adding list items.
-        direction: The direction of the list.
-        editable: A property that indicates whether adding and removing list items is allowed. Set false to disable.
-            By default it is `True` (allowed).
-        max_length: Maximum number of list items.
-        size: The distance between list items. Acceptable values in ascending order: s, m (default).
+    Attributes:
+        render: A template for the list item.
+        button_label: A text on a button that adds the list item.
+        direction: The direction of the list:
+            * `horizontal`
+            * `vertical`
+        editable:
+            * `True` — A Toloker can add or remove list items.
+            * `False` — The list can't be changed.
+
+            Default value: `True`.
+        max_length: The maximum number of list items.
+        size: The distance between list items:
+            * `s` — Small.
+            * `m` — Medium.
+
+            Default value: `m`.
     """
 
     render: BaseComponent
     button_label: base_component_or(Any) = attribute(kw_only=True)
     direction: base_component_or(ListDirection) = attribute(kw_only=True)
     editable: base_component_or(bool) = attribute(kw_only=True)
     max_length: base_component_or(float) = attribute(kw_only=True)
     size: base_component_or(ListSize) = attribute(kw_only=True)
 
 
 @inherit_docstrings
 class MediaFileFieldV1(BaseFieldV1, spec_value=ComponentType.FIELD_MEDIA_FILE):
-    """Adds buttons for different types of uploads: uploading photos or videos, selecting files from the file manager or choosing from the gallery.
-    In the accept property, select which buttons you need.
+    """A component for uploading media files.
 
-    By default, only one file can be uploaded, but you can allow multiple files in the multiple property.
+    For more information, see [field.media-file](https://toloka.ai/docs/template-builder/reference/field.media-file).
 
-    This component is convenient when using mobile devices. To upload files from a computer, it's better to use
-    field.file for a more flexible configuration of the file types.
     Attributes:
-        accept: Adds different buttons for four types of uploads. Pass the `True` value for the ones that you need.
-            For example, if you need a button for uploading files from the gallery, add the `gallery=True`.
-        multiple: Determines whether multiple files can be uploaded:
+        accept: Selecting file sources. Every source adds an upload button.
+        multiple:
+            * `True` — Multiple files can be uploaded.
+            * `False` — A single file can be uploaded.
+
+            Default value: `False`.
 
     Example:
-        How to allow Tolokers to upload images and make photos.
+        A component for uploading an image or taking a photo.
 
         >>> image_loader = tb.fields.MediaFileFieldV1(
         >>>     label='Upload a photo',
         >>>     data=tb.data.OutputData(path='image'),
         >>>     validation=tb.conditions.RequiredConditionV1(),
         >>>     accept=tb.fields.MediaFileFieldV1.Accept(photo=True, gallery=True),
-        >>>     multiple=False,
+        >>>     multiple=False
         >>> )
         ...
     """
 
     class Accept(BaseTemplate):
-        """Adds different buttons for four types of uploads.
+        """A choice of buttons for uploading media files from different sources.
 
         Attributes:
-            file_system: Adds a button for uploading files from the file manager.
-            gallery: Adds a button for uploading files from the gallery.
-            photo: Adds a button for uploading images.
-            video: Adds a button for uploading videos.
+            file_system: Files from a file manager.
+            gallery: Files from a gallery.
+            photo: Taking photos.
+            video: Taking videos.
         """
 
         file_system: base_component_or(bool) = attribute(origin='fileSystem', kw_only=True)
         gallery: base_component_or(bool) = attribute(kw_only=True)
         photo: base_component_or(bool) = attribute(kw_only=True)
         video: base_component_or(bool) = attribute(kw_only=True)
 
     accept: base_component_or(Accept)
     multiple: base_component_or(bool) = attribute(kw_only=True)
 
 
 @inherit_docstrings
 class NumberFieldV1(BaseFieldV1, spec_value=ComponentType.FIELD_NUMBER):
-    """A component that allows you to enter a number.
+    """A field for entering a number.
 
-    The box already has validation: by default, Tolokers can enter only numbers and decimal separators. They can use either
-    a dot or a comma as a separator, but there will always be a dot in the output.
+    For more information, see [field.number](https://toloka.ai/docs/template-builder/reference/field.number).
 
-    When the Toloker is entering a number, the separator automatically changes to the one specified in the regional settings.
-
-    Negative numbers are allowed by default. To disable them, use the validation property. Pressing the up or down arrow
-    keys will increase or decrease the number by one.
     Attributes:
-        maximum: Maximum number that can be entered.
-        minimum: Minimum number that can be entered.
-        placeholder: A semi-transparent label that is shown in the box when it is empty.
+        maximum: The maximum number that can be entered.
+        minimum: The minimum number that can be entered.
+        placeholder: A text that is shown if no number is entered.
     """
 
     maximum: base_component_or(int) = attribute(kw_only=True)
     minimum: base_component_or(int) = attribute(kw_only=True)
     placeholder: base_component_or(Any) = attribute(kw_only=True)
 
 
 @inherit_docstrings
 class PhoneNumberFieldV1(BaseFieldV1, spec_value=ComponentType.FIELD_PHONE_NUMBER):
-    """Creates a field for entering a phone number.
+    """A field for entering a phone number.
+
+    For more information, see [field.phone-number](https://toloka.ai/docs/template-builder/reference/field.phone-number).
 
-    Allows entering numbers, spaces, and the +, ( ), - characters. Only numbers and the + character at the beginning
-    will remain in the data. For example, if you enter +7 (012) 345-67-89, the data gets the +70123456789 value.
     Attributes:
-        placeholder: A semi-transparent label that is shown in an empty field.
+        placeholder: A text that is shown if no phone number is entered.
     """
 
     placeholder: base_component_or(str) = attribute(kw_only=True)
 
 
 @inherit_docstrings
 class RadioGroupFieldV1(BaseFieldV1, spec_value=ComponentType.FIELD_RADIO_GROUP):
-    """A component for selecting one value out of several options. It is designed as a group of circles arranged vertically.
+    """A component for selecting one value out of several options.
 
-    If you want it to look like normal buttons, use field.button-radio-group.
+    For more information, see [field.radio-group](https://toloka.ai/docs/template-builder/reference/field.radio-group).
 
-    The minimum number of buttons is one. Any type of data can be returned.
     Attributes:
-        options: List of options to choose from
-        disabled: This property prevents clicking the button. If the value is `True`, the button is not active (the Toloker
-            will not be able to click it).
+        options: A list of options.
+        disabled: Disabling the component:
+            * `False` — Selecting an option is allowed.
+            * `True` — Selecting an option is disabled.
 
-    Example:
-        How to add label selector to interface.
+            Default value: `False`.
 
+    Example:
         >>> radio_group_field = tb.fields.RadioGroupFieldV1(
-        >>>     tb.data.OutputData(path='result'),
-        >>>     [
+        >>>     data=tb.data.OutputData(path='result'),
+        >>>     options=[
         >>>         tb.fields.GroupFieldOption('Cat', 'cat'),
         >>>         tb.fields.GroupFieldOption('Dog', 'dog'),
         >>>     ],
         >>>     validation=tb.conditions.RequiredConditionV1()
         >>> )
         ...
     """
 
     options: base_component_or(List[base_component_or(GroupFieldOption)], 'ListBaseComponentOrGroupFieldOption')  # noqa: F821
     disabled: base_component_or(bool) = attribute(kw_only=True)
 
 
 @inherit_docstrings
 class SelectFieldV1(BaseFieldV1, spec_value=ComponentType.FIELD_SELECT):
-    """Button for selecting from a drop-down list.
+    """A field for selecting from a drop-down list of options.
 
-    Use this component when the list is long and only one option can be chosen.
+    For more information, see [field.select](https://toloka.ai/docs/template-builder/reference/field.select).
 
-    For short lists (2-4 items), it's better to use field.radio-group or field.button-radio-group, where all the
-    options are visible at once.
-
-    To allow selecting multiple options, use the field.checkbox-group component.
     Attributes:
-        options: Options to choose from.
-        placeholder: The text that will be displayed if none of the options is selected.
+        options: A list of options.
+        placeholder: A text that is shown if no option is selected.
     """
 
     class Option(BaseTemplate):
-        """Options to choose from.
+        """An option.
 
         Attributes:
-            label: The name of the option to display in the list.
-            value: The value to write to the data in the data property.
+            label: An option text.
+            value: A value that is saved in data when the option is selected.
         """
 
         label: base_component_or(Any)
         value: base_component_or(Any)
 
     options: base_component_or(List[base_component_or(Option)], 'ListBaseComponentOrOption')  # noqa: F821
     placeholder: base_component_or(Any) = attribute(kw_only=True)
 
 
 @inherit_docstrings
 class TextFieldV1(BaseFieldV1, spec_value=ComponentType.FIELD_TEXT):
-    """A component that allows entering a single line of text.
+    """A field for entering a single text line.
+
+    For more information, see [field.text](https://toloka.ai/docs/template-builder/reference/field.text).
 
     Attributes:
-        disabled: If `True`, editing is not available.
-        placeholder: A semi-transparent label that is shown in the box when it is empty.
+        disabled: Disabling the field:
+            * `True` — A Toloker can't enter a text in the field.
+            * `False` — Editing the field is allowed.
+
+            Default value: `False`.
+        placeholder: A text that is shown if no value is entered.
     """
 
     disabled: base_component_or(bool) = attribute(kw_only=True)
     placeholder: base_component_or(Any) = attribute(kw_only=True)
 
 
 @inherit_docstrings
 class TextAnnotationFieldV1(BaseFieldV1, spec_value=ComponentType.FIELD_TEXT_ANNOTATION):
-    """A component for text segmentation.
+    """A component for text annotation.
 
-    Use it to select multiple words, individual words, or letters in the text and label them with values. You can create
-    multiple categories to label parts of the text, like all nouns and adjectives.
-
-    You can use plugin.field.text-annotation.hotkeys to assign keyboard shortcuts for selecting categories.
+    For more information, see [field.text-annotation](https://toloka.ai/docs/template-builder/reference/field.text-annotation).
 
     Attributes:
-        adjust: If the property value is set to words, only words can be selected in the text. If you don't use this
-            property, any part of a line can be selected.
-        content: The text where the Toloker has to select part of a line.
-        disabled: This property blocks the component. If `True`, the component is unavailable to the Toloker. The
-            default value is `False`.
-        labels: A category.
+        adjust: If `adjust` is set to `words`, entire words are selected and annotated.
+            If `adjust` is omitted, any part of a text can be selected.
+        content: A text for annotation.
+        disabled: Disabling the component.
+            Default value: `False`.
+        labels: A list of annotation categories.
     """
 
     class Label(BaseTemplate):
-        """
+        """An annotation category.
+
         Attributes:
-            label: Specify the category name in the label property.
-            value: Specify the category value in the value property.
+            label: A category name.
+            value: A value that is saved in data.
         """
 
         label: base_component_or(str)
         value: base_component_or(str)
 
     adjust: base_component_or(str) = attribute(kw_only=True)
     content: base_component_or(str) = attribute(kw_only=True)
     disabled: base_component_or(bool) = attribute(kw_only=True)
     labels: base_component_or(List[base_component_or(Label)], 'ListBaseComponentOrLabel') = attribute(kw_only=True)  # noqa: F821
 
 
 @inherit_docstrings
 class TextareaFieldV1(BaseFieldV1, spec_value=ComponentType.FIELD_TEXTAREA):
-    """Box for entering multi-line text.
+    """A field for entering multiline text.
 
-    Use in tasks that require an extended response. For single-line responses, use the field.text component.
+    For more information, see [field.textarea](https://toloka.ai/docs/template-builder/reference/field.textarea).
 
-    The size of the box does not automatically adjust to the length of the text. Tolokers can change the height by
-    dragging the lower-right corner. To change the default size of the box, use the rows property.
-
-    Note that formatting is not available in the text box.
     Attributes:
-        disabled: If `True`, editing is not available.
-        placeholder: A semi-transparent label that is shown when the box is empty. Use it to provide an example or a
-            hint for the response.
-        resizable: Changing the box size. When set to `True` (the default value), the Toloker can change the height. To
-            prevent resizing, set the value to `False`.
-        rows: The height of the text box in lines.
+        disabled:
+            * `False` — A Toloker can edit the field.
+            * `True` — The field is disabled.
+
+            Default value: `False`.
+        placeholder: A text that is shown if the field is empty.
+        resizable:
+            * `True` — A Toloker can change the height of the field.
+            * `False` — The field is not resizable.
+
+            Default value: `True`.
+        rows: The height of the field in text lines.
     """
 
     disabled: base_component_or(bool) = attribute(kw_only=True)
     placeholder: base_component_or(Any) = attribute(kw_only=True)
     resizable: base_component_or(bool) = attribute(kw_only=True)
     rows: base_component_or(float) = attribute(kw_only=True)
```

### Comparing `toloka-kit-1.1.4/src/client/project/template_builder/fields.pyi` & `toloka-kit-1.2.0/src/client/project/template_builder/fields.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -33,21 +33,23 @@
         bases,
         namespace,
         **kwargs
     ): ...
 
 
 class BaseFieldV1(toloka.client.project.template_builder.base.BaseComponent, metaclass=BaseFieldV1Metaclass):
-    """Fields for entering data, such as a text field or drop-down list.
+    """A base class for input data fields.
+
+    Input fields are used to get data from Tolokers.
 
     Attributes:
-        data: Data with values that will be processed or changed.
-        label: Label above the component.
-        hint: Hint text.
-        validation: Validation based on condition.
+        data: A data path.
+        label: A label above the component.
+        hint: A hint.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         data: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         *,
         hint: typing.Optional[typing.Any] = None,
@@ -64,26 +66,27 @@
     hint: typing.Optional[typing.Any]
     label: typing.Optional[typing.Any]
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
 
 
 class AudioFieldV1(BaseFieldV1):
-    """Component for recording audio.
+    """A component for recording audio.
 
-    Works in the mobile app. In a browser, this component opens a window for uploading an audio file.
+    For more information, see [field.audio](https://toloka.ai/docs/template-builder/reference/field.audio).
 
     Attributes:
-        data: Data with values that will be processed or changed.
-        multiple: Determines whether multiple audio files can be recorded (or uploaded):
-            * `False` (default) — forbidden.
-            * `True` — allowed.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        data: A data path.
+        multiple: * `True` — Multiple audio files can be recorded or uploaded.
+            * `False` — A single file can be recorded or uploaded.
+
+            Default value: `False`.
+        hint: A hint.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         data: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         *,
         multiple: typing.Optional[typing.Any] = None,
@@ -102,26 +105,24 @@
     label: typing.Optional[typing.Any]
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
     multiple: typing.Optional[typing.Any]
 
 
 class ButtonRadioFieldV1(BaseFieldV1):
-    """A component in the form of a button.
+    """A button to choose an answer.
 
-    A Toloker makes a choice by clicking on it.
-
-    The size of the button depends on the size of the label.
+    For more information, see [field.button-radio](https://toloka.ai/docs/template-builder/reference/field.button-radio).
 
     Attributes:
-        data: Data with values that will be processed or changed.
-        value_to_set: The value of the output data when the button is clicked.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        data: A data path.
+        value_to_set: A value to write to data.
+        hint: A hint.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         data: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         value_to_set: typing.Optional[typing.Any] = None,
         *,
@@ -140,20 +141,20 @@
     label: typing.Optional[typing.Any]
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
     value_to_set: typing.Optional[typing.Any]
 
 
 class GroupFieldOption(toloka.client.project.template_builder.base.BaseTemplate):
-    """Option.
+    """A single option for components with multiple options.
 
     Attributes:
-        value: Returned value.
-        label: The text on the object.
-        hint: Additional information.
+        value: A value that is saved in data when the option is selected.
+        label: An option text.
+        hint: An additional description.
     """
 
     def __init__(
         self,
         value: typing.Optional[typing.Any] = None,
         label: typing.Optional[typing.Any] = None,
         *,
@@ -166,33 +167,29 @@
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     value: typing.Optional[typing.Any]
     label: typing.Optional[typing.Any]
     hint: typing.Optional[typing.Any]
 
 
 class ButtonRadioGroupFieldV1(BaseFieldV1):
-    """A component with buttons that allow the Toloker to choose between the specified values.
-
-    The minimum number of elements is one. Any type of data can be returned.
+    """A group of buttons for choosing one option.
 
-    The size of the button is determined by the length of the text on it.
+    For more information, see [field.button-radio-group](https://toloka.ai/docs/template-builder/reference/field.button-radio-group).
 
     Attributes:
-        data: Data with values that will be processed or changed.
-        options: Array of information about the buttons.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        data: A data path.
+        options: A list of options.
+        hint: A hint.
+        label: A label above the component.
+        validation: Validation rules.
 
     Examples:
-        How to add buttons for classification task.
-
         >>> classification_buttons = tb.fields.ButtonRadioGroupFieldV1(
-        >>>     tb.data.OutputData(path='class'),
-        >>>     [
+        >>>     data=tb.data.OutputData(path='class'),
+        >>>     options=[
         >>>         tb.fields.GroupFieldOption('Cat', 'cat'),
         >>>         tb.fields.GroupFieldOption('Dog', 'dog'),
         >>>     ],
         >>>     validation=tb.conditions.RequiredConditionV1(hint='Choose one of the answer options'),
         >>> )
         ...
     """
@@ -217,25 +214,28 @@
     label: typing.Optional[typing.Any]
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
     options: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, GroupFieldOption]]]]
 
 
 class CheckboxFieldV1(BaseFieldV1):
-    """Checkbox.
+    """A checkbox.
+
+    For more information, see [field.checkbox](https://toloka.ai/docs/template-builder/reference/field.checkbox).
 
     Attributes:
-        data: Data with values that will be processed or changed.
-        disabled: Property that disables the component. If `True`, the component will not be unavailable.
-        preserve_false: Property that specifies whether to return false values in the results. By default, if the
-            component returns `False`, this result will not be added to the output. To add `False` to the results, specify
-            `preserve_false=True`.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        data: A data path.
+        disabled: Disabling the checkbox.
+        preserve_false: * `False` — If the checkbox is not selected then `False` is not added to the output data.
+            * `True` — The output data is always present whether the checkbox is selected or not.
+
+            Default value: `False`.
+        hint: A hint.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         data: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         *,
         disabled: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]] = None,
@@ -256,26 +256,31 @@
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
     disabled: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]
     preserve_false: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]
 
 
 class CheckboxGroupFieldV1(BaseFieldV1):
-    """A group of options for selecting one or more responses.
+    """A group of checkboxes.
+
+    This component creates a dictionary in the output data. Values from `options` are used as keys in the dictionary.
+
+    For more information, see [field.checkbox-group](https://toloka.ai/docs/template-builder/reference/field.checkbox-group).
 
     Attributes:
-        data: Data with values that will be processed or changed.
-        options: Options, where value is the key that the option controls, and label is the text near the option.
-        disabled: If `True', the options are inactive.
-        preserve_false: Property that specifies whether to return false values in the results. By default, if the
-            component returns false, this result will not be added to the output. To add false to the results, specify
-            `preserve_false = True`.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        data: A data path.
+        options: A list of options.
+        disabled: Disabling the checkbox group.
+        preserve_false: * `False` — If a checkbox from the group is not selected then its key is not added to the dictionary.
+            * `True` — The output dictionary contains all keys whether checkboxes are selected or not.
+
+            Default value: `False`.
+        hint: A hint.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         data: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         options: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, GroupFieldOption]]]] = None,
         *,
@@ -298,41 +303,30 @@
     version: typing.Optional[str]
     options: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, GroupFieldOption]]]]
     disabled: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]
     preserve_false: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]
 
 
 class DateFieldV1(BaseFieldV1):
-    """A component for entering the date and time in the desired format and range.
+    """A field for entering a date and time.
 
-    You can set a list of dates that the Toloker cannot select.
+    For more information, see [field.date](https://toloka.ai/docs/template-builder/reference/field.date).
 
     Attributes:
-        data: Data with values that will be processed or changed.
-        format: Format of the date entered by the Toloker:
-            * date-time — date and time.
-            * date — date only.
-        block_list: List of dates that the Toloker cannot select.
-            * block_list[]: Date that the Toloker cannot select.
-        max: The latest date and time in the YYYY-MM-DD hh:mm format that the Toloker can select. Where:
-            * YYYY is the year.
-            * MM is the month.
-            * DD is the day.
-            * hh is the time in hours.
-            * mm is the time in minutes.
-        min: The earliest date and time in the YYYY-MM-DD hh:mm format that the Toloker can select. Where:
-            * YYYY is the year.
-            * MM is the month.
-            * DD is the day.
-            * hh is the time in hours.
-            * mm is the time in minutes.
-        placeholder: A semi-transparent label that is shown in the box when it is empty.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        data: A data path.
+        format: The format of the field:
+            * `date-time` — Date and time.
+            * `date` — Date only.
+        block_list: A list of dates that a Toloker can't select.
+        max: The latest date and time in the `YYYY-MM-DD hh:mm` format that a Toloker can select.
+        min: The earliest date and time in the `YYYY-MM-DD hh:mm` format that a Toloker can select.
+        placeholder: A text that is shown when no date is entered.
+        hint: A hint.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         data: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         format: typing.Optional[typing.Any] = None,
         *,
@@ -359,24 +353,24 @@
     block_list: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Any]]]
     max: typing.Optional[typing.Any]
     min: typing.Optional[typing.Any]
     placeholder: typing.Optional[typing.Any]
 
 
 class EmailFieldV1(BaseFieldV1):
-    """Creates a field for entering an email address.
+    """A field for entering an email address.
 
-    Checks that the text contains the @ character. You can set other conditions yourself.
+    For more information, see [field.email](https://toloka.ai/docs/template-builder/reference/field.email).
 
     Attributes:
-        data: Data with values that will be processed or changed.
-        placeholder: A semi-transparent label that is shown in an empty field.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        data: A data path.
+        placeholder: A text that is shown when no address is entered.
+        hint: A hint.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         data: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         *,
         placeholder: typing.Optional[typing.Any] = None,
@@ -395,33 +389,31 @@
     label: typing.Optional[typing.Any]
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
     placeholder: typing.Optional[typing.Any]
 
 
 class FileFieldV1(BaseFieldV1):
-    """This component can be used for uploading files. It's displayed in the interface as an upload button.
+    """A component for uploading files.
 
-    You can restrict the file types to upload in the "accept" property. By default, only one file can be uploaded,
-    but you can allow multiple files in the "multiple" property.
-
-    If a Toloker logs in from a mobile device, it's more convenient to use field.media-file — it's adapted for mobile
-    devices and makes it easier to upload photos and videos.
+    For more information, see [field.file](https://toloka.ai/docs/template-builder/reference/field.file).
 
     Attributes:
-        data: Data with values that will be processed or changed.
-        accept: A list of file types that can be uploaded. By default, you can upload any files.
-            Specify the types in the [certain format](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types).
-            For example, you can allow only images to be uploaded by adding the image/jpeg and image/png types.
-        multiple: Determines whether multiple files can be uploaded:
-            * `False` (default) — forbidden.
-            * `True` — allowed.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        data: A data path.
+        accept: A list of file types that can be uploaded.
+            Use [MIME types](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types).
+            For example, `image/jpeg`.
+            By default, you can upload any files.
+        multiple: * `True` — Multiple files can be uploaded.
+            * `False` — A single file can be uploaded.
+
+            Default value: `False`.
+        hint: A hint.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         data: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         accept: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]]]] = None,
         *,
@@ -442,54 +434,46 @@
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
     accept: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]]]]
     multiple: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]
 
 
 class ImageAnnotationFieldV1(BaseFieldV1):
-    """Adds an interface for selecting areas in images.
-
-    If you need to select different types of objects, classify the areas using the labels property.
+    """A component for annotating areas in an image.
 
-    You can select areas using points, polygons, and rectangles. In the shapes property, you can keep some of the
-    selection modes and hide the rest.
+    For more information, see [field.image-annotation](https://toloka.ai/docs/template-builder/reference/field.image-annotation).
 
     Attributes:
-        data: Data with values that will be processed or changed.
-        image: The image you want to select areas in.
-        disabled: Determines whether adding and deleting areas is allowed:
-            * `False` (default) — Allowed.
-            * `True` — Not allowed.
-            You can use this feature when creating an interface to check whether the selection is correct,
-             or if you need to allow selection only when a certain condition is met.
-        full_height: If `True`, the element takes up all the vertical free space. The element is set to a minimum height
-            of 400 pixels.
-        labels: Used to classify areas.
-            You can add several area types. When adding an area type, a button to select it appears in the interface,
-            and when setting a new value, a new area selection color is added.
-            This feature is instrumental if you need to select different types of objects: you can use one color to
-            select cars and a different one for pedestrians.
-        min_width: Minimum width of the element in pixels. Takes priority over max_width.
-        ratio: An array of two numbers that sets the relative dimensions of the sides: width (first number) to height
-            (second number). Not valid if `full_height=True`.
-        shapes: Used to add and hide selection modes: points, polygons, and rectangles. All three modes are available
-            by default.
-            Use this property if you only need to keep certain modes. Modes with the `True` value are available.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        data: A data path.
+        image: The URL of the image.
+        disabled: Disabling the component:
+            * `False` — Annotating is allowed.
+            * `True` — Annotating is disabled.
+
+            Default value: `False`.
+        full_height: If `True`, the component takes up all the vertical free space.
+            Note, that the minimum height required by the component is 400 pixels.
+        labels: Labels used to classify image areas.
+        min_width: The minimum width of the component in pixels.
+        ratio: A list with the aspect ratio of the component. Specify the relative width and then the height.
+            This setting is not used if `full_height=True`.
+        shapes: Area selection modes: `point`, `polygon`, and `rectangle`.
+            Use mode names as keys in the `shapes` dictionary. Modes set to `True` are available in the component.
+            By default, all modes are available.
+        hint: A hint.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     class Label(toloka.client.project.template_builder.base.BaseTemplate):
-        """At least two objects must be added to the array.
+        """An image area class.
 
         Attributes:
-            label: Text on the button for selecting a selection color.
-            value: The value to be written to the labels property data. Displayed to Tolokers as color options when
-                selecting areas.
+            label: A text on a button for selecting the area class.
+            value: A value used in output data.
         """
 
         def __init__(
             self,
             label: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]] = None,
             value: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]] = None
         ) -> None:
@@ -541,41 +525,41 @@
     labels: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, Label]]]]
     min_width: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, float]]
     ratio: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, float]]]]
     shapes: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.Dict[typing.Union[toloka.client.project.template_builder.base.BaseComponent, Shape], typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]]]
 
 
 class ListFieldV1(BaseFieldV1):
-    """A component that allows a Toloker to add and remove list items, such as text fields to fill in.
+    """A component that allows a Toloker to add and remove list items, such as text fields.
 
-    This way you can allow a Toloker to give multiple answers to a question.
+    Use RelativeData(toloka.client.project.template_builder.data.RelativeData.md) in list items,
+    otherwise all list items will change the same data.
 
-    The list items can contain any component, including a list of other components. For example, this allows you to
-    create a table where you can add and delete rows.
+    For more information, see [field.list](https://toloka.ai/docs/template-builder/reference/field.list).
 
-    To add a new list item, the Toloker clicks the button. To remove an item, they click on the x on the right (it appears
-    when hovering over a list item).
-
-    To prevent a Toloker from adding too many list items, set the maximum list length. You can also use the editable
-    property to block Tolokers from changing a component, like when a certain event occurs.
-
-    Attributes:
-        data: Data with values that will be processed or changed.
-        render: Interface template for list items, such as a text field.
-            In nested field.* components, use data.relative for recording responses, otherwise all the list items will
-            have the same value.
-        button_label: Text on the button for adding list items.
-        direction: The direction of the list.
-        editable: A property that indicates whether adding and removing list items is allowed. Set false to disable.
-            By default it is `True` (allowed).
-        max_length: Maximum number of list items.
-        size: The distance between list items. Acceptable values in ascending order: s, m (default).
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+    Attributes:
+        data: A data path.
+        render: A template for the list item.
+        button_label: A text on a button that adds the list item.
+        direction: The direction of the list:
+            * `horizontal`
+            * `vertical`
+        editable: * `True` — A Toloker can add or remove list items.
+            * `False` — The list can't be changed.
+
+            Default value: `True`.
+        max_length: The maximum number of list items.
+        size: The distance between list items:
+            * `s` — Small.
+            * `m` — Medium.
+
+            Default value: `m`.
+        hint: A hint.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         data: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         render: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         *,
@@ -604,53 +588,50 @@
     direction: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, toloka.client.project.template_builder.base.ListDirection]]
     editable: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]
     max_length: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, float]]
     size: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, toloka.client.project.template_builder.base.ListSize]]
 
 
 class MediaFileFieldV1(BaseFieldV1):
-    """Adds buttons for different types of uploads: uploading photos or videos, selecting files from the file manager or choosing from the gallery.
-
-    In the accept property, select which buttons you need.
-
-    By default, only one file can be uploaded, but you can allow multiple files in the multiple property.
+    """A component for uploading media files.
 
-    This component is convenient when using mobile devices. To upload files from a computer, it's better to use
-    field.file for a more flexible configuration of the file types.
+    For more information, see [field.media-file](https://toloka.ai/docs/template-builder/reference/field.media-file).
 
     Attributes:
-        data: Data with values that will be processed or changed.
-        accept: Adds different buttons for four types of uploads. Pass the `True` value for the ones that you need.
-            For example, if you need a button for uploading files from the gallery, add the `gallery=True`.
-        multiple: Determines whether multiple files can be uploaded:
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        data: A data path.
+        accept: Selecting file sources. Every source adds an upload button.
+        multiple: * `True` — Multiple files can be uploaded.
+            * `False` — A single file can be uploaded.
+
+            Default value: `False`.
+        hint: A hint.
+        label: A label above the component.
+        validation: Validation rules.
 
     Examples:
-        How to allow Tolokers to upload images and make photos.
+        A component for uploading an image or taking a photo.
 
         >>> image_loader = tb.fields.MediaFileFieldV1(
         >>>     label='Upload a photo',
         >>>     data=tb.data.OutputData(path='image'),
         >>>     validation=tb.conditions.RequiredConditionV1(),
         >>>     accept=tb.fields.MediaFileFieldV1.Accept(photo=True, gallery=True),
-        >>>     multiple=False,
+        >>>     multiple=False
         >>> )
         ...
     """
 
     class Accept(toloka.client.project.template_builder.base.BaseTemplate):
-        """Adds different buttons for four types of uploads.
+        """A choice of buttons for uploading media files from different sources.
 
         Attributes:
-            file_system: Adds a button for uploading files from the file manager.
-            gallery: Adds a button for uploading files from the gallery.
-            photo: Adds a button for uploading images.
-            video: Adds a button for uploading videos.
+            file_system: Files from a file manager.
+            gallery: Files from a gallery.
+            photo: Taking photos.
+            video: Taking videos.
         """
 
         def __init__(
             self,
             *,
             file_system: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]] = None,
             gallery: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]] = None,
@@ -689,32 +670,26 @@
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
     accept: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, Accept]]
     multiple: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]
 
 
 class NumberFieldV1(BaseFieldV1):
-    """A component that allows you to enter a number.
-
-    The box already has validation: by default, Tolokers can enter only numbers and decimal separators. They can use either
-    a dot or a comma as a separator, but there will always be a dot in the output.
+    """A field for entering a number.
 
-    When the Toloker is entering a number, the separator automatically changes to the one specified in the regional settings.
-
-    Negative numbers are allowed by default. To disable them, use the validation property. Pressing the up or down arrow
-    keys will increase or decrease the number by one.
+    For more information, see [field.number](https://toloka.ai/docs/template-builder/reference/field.number).
 
     Attributes:
-        data: Data with values that will be processed or changed.
-        maximum: Maximum number that can be entered.
-        minimum: Minimum number that can be entered.
-        placeholder: A semi-transparent label that is shown in the box when it is empty.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        data: A data path.
+        maximum: The maximum number that can be entered.
+        minimum: The minimum number that can be entered.
+        placeholder: A text that is shown if no number is entered.
+        hint: A hint.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         data: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         *,
         maximum: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, int]] = None,
@@ -737,25 +712,24 @@
     version: typing.Optional[str]
     maximum: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, int]]
     minimum: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, int]]
     placeholder: typing.Optional[typing.Any]
 
 
 class PhoneNumberFieldV1(BaseFieldV1):
-    """Creates a field for entering a phone number.
+    """A field for entering a phone number.
 
-    Allows entering numbers, spaces, and the +, ( ), - characters. Only numbers and the + character at the beginning
-    will remain in the data. For example, if you enter +7 (012) 345-67-89, the data gets the +70123456789 value.
+    For more information, see [field.phone-number](https://toloka.ai/docs/template-builder/reference/field.phone-number).
 
     Attributes:
-        data: Data with values that will be processed or changed.
-        placeholder: A semi-transparent label that is shown in an empty field.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        data: A data path.
+        placeholder: A text that is shown if no phone number is entered.
+        hint: A hint.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         data: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         *,
         placeholder: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]] = None,
@@ -774,35 +748,34 @@
     label: typing.Optional[typing.Any]
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
     placeholder: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]]
 
 
 class RadioGroupFieldV1(BaseFieldV1):
-    """A component for selecting one value out of several options. It is designed as a group of circles arranged vertically.
-
-    If you want it to look like normal buttons, use field.button-radio-group.
+    """A component for selecting one value out of several options.
 
-    The minimum number of buttons is one. Any type of data can be returned.
+    For more information, see [field.radio-group](https://toloka.ai/docs/template-builder/reference/field.radio-group).
 
     Attributes:
-        data: Data with values that will be processed or changed.
-        options: List of options to choose from
-        disabled: This property prevents clicking the button. If the value is `True`, the button is not active (the Toloker
-            will not be able to click it).
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        data: A data path.
+        options: A list of options.
+        disabled: Disabling the component:
+            * `False` — Selecting an option is allowed.
+            * `True` — Selecting an option is disabled.
 
-    Examples:
-        How to add label selector to interface.
+            Default value: `False`.
+        hint: A hint.
+        label: A label above the component.
+        validation: Validation rules.
 
+    Examples:
         >>> radio_group_field = tb.fields.RadioGroupFieldV1(
-        >>>     tb.data.OutputData(path='result'),
-        >>>     [
+        >>>     data=tb.data.OutputData(path='result'),
+        >>>     options=[
         >>>         tb.fields.GroupFieldOption('Cat', 'cat'),
         >>>         tb.fields.GroupFieldOption('Dog', 'dog'),
         >>>     ],
         >>>     validation=tb.conditions.RequiredConditionV1()
         >>> )
         ...
     """
@@ -829,38 +802,33 @@
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
     options: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, GroupFieldOption]]]]
     disabled: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]
 
 
 class SelectFieldV1(BaseFieldV1):
-    """Button for selecting from a drop-down list.
-
-    Use this component when the list is long and only one option can be chosen.
-
-    For short lists (2-4 items), it's better to use field.radio-group or field.button-radio-group, where all the
-    options are visible at once.
+    """A field for selecting from a drop-down list of options.
 
-    To allow selecting multiple options, use the field.checkbox-group component.
+    For more information, see [field.select](https://toloka.ai/docs/template-builder/reference/field.select).
 
     Attributes:
-        data: Data with values that will be processed or changed.
-        options: Options to choose from.
-        placeholder: The text that will be displayed if none of the options is selected.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        data: A data path.
+        options: A list of options.
+        placeholder: A text that is shown if no option is selected.
+        hint: A hint.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     class Option(toloka.client.project.template_builder.base.BaseTemplate):
-        """Options to choose from.
+        """An option.
 
         Attributes:
-            label: The name of the option to display in the list.
-            value: The value to write to the data in the data property.
+            label: An option text.
+            value: A value that is saved in data when the option is selected.
         """
 
         def __init__(
             self,
             label: typing.Optional[typing.Any] = None,
             value: typing.Optional[typing.Any] = None
         ) -> None:
@@ -894,23 +862,29 @@
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
     options: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, Option]]]]
     placeholder: typing.Optional[typing.Any]
 
 
 class TextFieldV1(BaseFieldV1):
-    """A component that allows entering a single line of text.
+    """A field for entering a single text line.
+
+    For more information, see [field.text](https://toloka.ai/docs/template-builder/reference/field.text).
 
     Attributes:
-        data: Data with values that will be processed or changed.
-        disabled: If `True`, editing is not available.
-        placeholder: A semi-transparent label that is shown in the box when it is empty.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        data: A data path.
+        disabled: Disabling the field:
+            * `True` — A Toloker can't enter a text in the field.
+            * `False` — Editing the field is allowed.
+
+            Default value: `False`.
+        placeholder: A text that is shown if no value is entered.
+        hint: A hint.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         data: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         *,
         disabled: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]] = None,
@@ -931,38 +905,37 @@
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
     disabled: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]
     placeholder: typing.Optional[typing.Any]
 
 
 class TextAnnotationFieldV1(BaseFieldV1):
-    """A component for text segmentation.
+    """A component for text annotation.
 
-    Use it to select multiple words, individual words, or letters in the text and label them with values. You can create
-    multiple categories to label parts of the text, like all nouns and adjectives.
-
-    You can use plugin.field.text-annotation.hotkeys to assign keyboard shortcuts for selecting categories.
+    For more information, see [field.text-annotation](https://toloka.ai/docs/template-builder/reference/field.text-annotation).
 
     Attributes:
-        data: Data with values that will be processed or changed.
-        adjust: If the property value is set to words, only words can be selected in the text. If you don't use this
-            property, any part of a line can be selected.
-        content: The text where the Toloker has to select part of a line.
-        disabled: This property blocks the component. If `True`, the component is unavailable to the Toloker. The
-            default value is `False`.
-        labels: A category.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        data: A data path.
+        adjust: If `adjust` is set to `words`, entire words are selected and annotated.
+            If `adjust` is omitted, any part of a text can be selected.
+        content: A text for annotation.
+        disabled: Disabling the component.
+            Default value: `False`.
+        labels: A list of annotation categories.
+        hint: A hint.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     class Label(toloka.client.project.template_builder.base.BaseTemplate):
-        """Attributes:
-            label: Specify the category name in the label property.
-            value: Specify the category value in the value property.
+        """An annotation category.
+
+        Attributes:
+            label: A category name.
+            value: A value that is saved in data.
         """
 
         def __init__(
             self,
             label: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]] = None,
             value: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]] = None
         ) -> None:
@@ -1000,34 +973,33 @@
     adjust: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]]
     content: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]]
     disabled: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]
     labels: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, Label]]]]
 
 
 class TextareaFieldV1(BaseFieldV1):
-    """Box for entering multi-line text.
+    """A field for entering multiline text.
 
-    Use in tasks that require an extended response. For single-line responses, use the field.text component.
+    For more information, see [field.textarea](https://toloka.ai/docs/template-builder/reference/field.textarea).
 
-    The size of the box does not automatically adjust to the length of the text. Tolokers can change the height by
-    dragging the lower-right corner. To change the default size of the box, use the rows property.
+    Attributes:
+        data: A data path.
+        disabled: * `False` — A Toloker can edit the field.
+            * `True` — The field is disabled.
 
-    Note that formatting is not available in the text box.
+            Default value: `False`.
+        placeholder: A text that is shown if the field is empty.
+        resizable: * `True` — A Toloker can change the height of the field.
+            * `False` — The field is not resizable.
 
-    Attributes:
-        data: Data with values that will be processed or changed.
-        disabled: If `True`, editing is not available.
-        placeholder: A semi-transparent label that is shown when the box is empty. Use it to provide an example or a
-            hint for the response.
-        resizable: Changing the box size. When set to `True` (the default value), the Toloker can change the height. To
-            prevent resizing, set the value to `False`.
-        rows: The height of the text box in lines.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+            Default value: `True`.
+        rows: The height of the field in text lines.
+        hint: A hint.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         data: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         *,
         disabled: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]] = None,
```

### Comparing `toloka-kit-1.1.4/src/client/project/template_builder/helpers.pyi` & `toloka-kit-1.2.0/src/client/project/template_builder/helpers.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -15,35 +15,33 @@
 ]
 import toloka.client.project.template_builder.base
 import toloka.util._extendable_enum
 import typing
 
 
 class BaseHelperV1(toloka.client.project.template_builder.base.BaseComponent, metaclass=toloka.client.project.template_builder.base.VersionedBaseComponentMetaclass):
-    """Perform various operations, such as if-then-else or switch-case.
+    """A base class for helpers.
     """
 
     def __init__(self, *, version: typing.Optional[str] = '1.0.0') -> None:
         """Method generated by attrs for class BaseHelperV1.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     version: typing.Optional[str]
 
 
 class ConcatArraysHelperV1(BaseHelperV1):
-    """Merging multiple arrays into a single array.
+    """Concatenates multiple arrays into a single array.
+
+    For more information, see [helper.concat-arrays](https://toloka.ai/docs/template-builder/reference/helper.concat-arrays).
 
-    For example, let's say you have multiple arrays:
-    `([1, 2, 3], [4, 5, 6], [7, 8, 9])`
-    Their elements can be combined into a single array to show simultaneously:
-    `[1, 2, 3, 4, 5, 6, 7, 8, 9]`
     Attributes:
-        items: Arrays to combine.
+        items: Arrays to concatenate.
     """
 
     def __init__(
         self,
         items: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Any]]] = None,
         *,
         version: typing.Optional[str] = '1.0.0'
@@ -54,34 +52,24 @@
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     version: typing.Optional[str]
     items: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Any]]]
 
 
 class Entries2ObjectHelperV1(BaseHelperV1):
-    """Creating an object from a specified array of key-value pairs.
+    """Creates an object from an array of key-value pairs.
 
-    For example, let's say you have an array like this:
+    For example,
+    `[ {"key":"foo", "value":"hello"}, {"key":"bar","value":"world"} ]`
+    is converted to `{ "foo": "hello", "bar": "world" }`.
 
-    >>> [
-    >>>     {
-    >>>         "key": "foo",
-    >>>         "value": "hello"
-    >>>     },
-    >>>     {
-    >>>         "key": "bar",
-    >>>         "value": "world"
-    >>>     }
-    >>> ]
-    ...
+    For more information, see [helper.entries2object](https://toloka.ai/docs/template-builder/reference/helper.entries2object).
 
-    It is converted to an object whose elements consist of the values of the original array:
-    `{ "foo": "hello", "bar": "world" }`
     Attributes:
-        entries: Source array of key-value pairs.
+        entries: A source array of key-value pairs.
     """
 
     class Entry(toloka.client.project.template_builder.base.BaseTemplate):
         def __init__(
             self,
             key: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]] = None,
             value: typing.Optional[typing.Any] = None
@@ -106,36 +94,29 @@
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     version: typing.Optional[str]
     entries: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, Entry]]]]
 
 
 class IfHelperV1(BaseHelperV1):
-    """The If...Then...Else operator.
+    """The `if then else` operator.
 
-    Allows you to execute either one block of code or another, depending on the condition. If you need more options,
-    use helper.switch.
+    For more information, see [helper.if](https://toloka.ai/docs/template-builder/reference/helper.if).
 
-    For example, if you want to conduct a survey, you can use the helper.if component to ask the gender of the
-    respondent and add different sets of questions, depending on whether the respondent is male or female.
-    How it works: If the condition in if is true (returns true), the code specified in the then property will be
-    executed. Otherwise (the condition is false and returns false) the code specified in else will be executed.
-    The else property is optional. For example, let's say you ask a Toloker "Do you like the image?". You can make a
-    comment field appear when a negative response is received, but nothing happens when a positive response is received.
-    Attributes:
-        condition: Condition to check.
-        then: The element that is returned if the condition from the condition property is true (returns true).
-        else_: The element that is returned if the condition from the condition property is false (returns false).
+    Attributes:
+        condition: A condition to check.
+        then: A component that is returned if the condition is `True`.
+        else_: A component that is returned if the condition is `False`.
 
     Example:
-        How to show a part of the interface by condition.
+        How to conditionally show a part of the interface.
 
         >>> hidden_ui = tb.helpers.IfHelperV1(
-        >>>     tb.conditions.EqualsConditionV1(tb.data.OutputData('show_me'), 'show'),
-        >>>     tb.view.ListViewV1([header, buttons, images]),
+        >>>     condition=tb.conditions.EqualsConditionV1(tb.data.OutputData('show_me'), 'show'),
+        >>>     then=tb.view.ListViewV1([header, buttons, images]),
         >>> )
         ...
     """
 
     def __init__(
         self,
         condition: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
@@ -152,20 +133,21 @@
     version: typing.Optional[str]
     condition: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     then: typing.Optional[typing.Any]
     else_: typing.Optional[typing.Any]
 
 
 class JoinHelperV1(BaseHelperV1):
-    """The component combines two or more strings into one.
+    """Joins strings into a single string.
+
+    For more information, see [helper.join](https://toloka.ai/docs/template-builder/reference/helper.join).
 
-    You can add a delimiter to separate the strings, such as a space or comma.
     Attributes:
-        items: Array of strings to join.
-        by: Delimiter for joining strings. You can use any number of characters in the delimiter.
+        items: A list of strings to join.
+        by: A delimiter. You can use any number of characters in the delimiter.
     """
 
     def __init__(
         self,
         items: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]]]] = None,
         by: typing.Optional[typing.Any] = None,
         *,
@@ -178,40 +160,24 @@
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     version: typing.Optional[str]
     items: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]]]]
     by: typing.Optional[typing.Any]
 
 
 class Object2EntriesHelperV1(BaseHelperV1):
-    """Creating an array of key-value pairs from the specified object.
+    """Creates an array of key-value pairs from an object.
 
-    For example, let's say you have an object that looks like this:
+    For example,
+    `{ "foo": "hello", "bar": "world" }` is converted to
+    `[ {"key":"foo", "value":"hello"}, {"key":"bar","value":"world"} ]`.
 
-    >>> {
-    >>>     "foo": "hello",
-    >>>     "bar": "world"
-    >>> }
-    ...
-
-    It will be converted to an array whose objects will pair data from the source object and their designations:
-
-    >>> [
-    >>>     {
-    >>>         "key": "foo",
-    >>>         "value": "hello"
-    >>>     },
-    >>>     {
-    >>>         "key": "bar",
-    >>>         "value": "world"
-    >>>     }
-    >>> ]
-    ...
+    For more information, see [helper.object2entries](https://toloka.ai/docs/template-builder/reference/helper.object2entries).
 
     Attributes:
-        data: The object to convert.
+        data: An object to convert.
     """
 
     def __init__(
         self,
         data: typing.Optional[typing.Any] = None,
         *,
         version: typing.Optional[str] = '1.0.0'
@@ -222,23 +188,22 @@
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     version: typing.Optional[str]
     data: typing.Optional[typing.Any]
 
 
 class ReplaceHelperV1(BaseHelperV1):
-    """Allows you to replace some parts of the string with others.
+    """Replaces a substring in a string.
+
+    For more information, see [helper.replace](https://toloka.ai/docs/template-builder/reference/helper.replace).
 
-    This helper function returns a string in which all occurrences of `find` in `data` are replaced with `replace`.
-    Because the helper.replace helper returns a string, it can be used in properties that accept string values.
     Attributes:
-        data: Data to perform the replacement on.
-        find: The value to search for — the string whose occurrences must be found in data and replaced with the string
-            from replace.
-        replace: The value to insert in place of the matches of the find value.
+        data: An input string.
+        find: A substring to look for.
+        replace: A substring to replace with.
     """
 
     def __init__(
         self,
         data: typing.Optional[typing.Any] = None,
         find: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]] = None,
         replace: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]] = None,
@@ -253,20 +218,21 @@
     version: typing.Optional[str]
     data: typing.Optional[typing.Any]
     find: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]]
     replace: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]]
 
 
 class SearchQueryHelperV1(BaseHelperV1):
-    """Component for creating a string with a search query reference.
+    """Creates a query for a search engine.
+
+    For more information, see [helper.search-query](https://toloka.ai/docs/template-builder/reference/helper.search-query).
 
-    The list of available search engines is specified in the engine enum.
     Attributes:
-        query: Search query.
-        engine: Search engine.
+        query: A query.
+        engine: A search engine.
     """
 
     class Engine(toloka.util._extendable_enum.ExtendableStrEnum):
         """An enumeration.
         """
 
         YANDEX = 'yandex'
@@ -295,43 +261,30 @@
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     version: typing.Optional[str]
     query: typing.Optional[typing.Any]
     engine: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, Engine]]
 
 
 class SwitchHelperV1(BaseHelperV1):
-    """A switch-case construction.
-
-    Checks various conditions sequentially and executes the code from the result property when the corresponding
-    condition is true.
+    """Chooses one variant from multiple cases.
 
-    You can use it to perform an action or display an additional interface element only when a certain condition is met.
-    View example in the sandbox.
+    For more information, see [helper.switch](https://toloka.ai/docs/template-builder/reference/helper.switch).
 
-    This helper is similar to a series of If...Then...Else logical expressions, so it is useful if there are more than
-    two conditions for sequential verification. If you need to check one or two conditions, use the helper.if component.
-    How the helper works:
-        * The helper checks (conditions) from the array of cases objects, starting from the first one.
-        * If the condition is true (returns true), the helper returns the result (block of code) specified in the result
-          property for the condition object in the cases array. The helper quits and subsequent conditions are not
-          checked.
-        * If the condition is false (returns false), the helper checks the subsequent condition.
-        * If all conditions are false as a result of all checks, the helper returns the value specified in the default
-          property (if it is not defined, the helper returns nothing).
     Attributes:
-        cases: An array of objects consisting of condition and result property pairs.
-        default: Element that is returned if none of the checked conditions returned true.
+        cases: A list of cases.
+            A case consists of a condition and a resulting component.
+        default: A component that is returned if none of the conditions is `True`.
     """
 
     class Case(toloka.client.project.template_builder.base.BaseTemplate):
-        """Case.
+        """A case for the `SwitchHelperV1`.
 
         Attributes:
-            condition: Condition to check.
-            result: The element that is returned if the condition from the condition property is true (returns true).
+            condition: A case condition.
+            result: A component that is returned if the condition is `True`.
         """
 
         def __init__(
             self,
             condition: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
             result: typing.Optional[typing.Any] = None
         ) -> None:
@@ -357,23 +310,24 @@
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     version: typing.Optional[str]
     cases: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, Case]]]]
     default: typing.Optional[typing.Any]
 
 
 class TextTransformHelperV1(BaseHelperV1):
-    """Allows you to change the case of the text, like make all letters uppercase.
+    """Converts a text to uppercase, lowercase, or capitalize it.
 
-    For example, you can use this component to automatically process input data.
+    For more information, see [helper.text-transform](https://toloka.ai/docs/template-builder/reference/helper.text-transform).
 
-    This component is available in property values with the string type, for example in the content property in the
-    view.text component.
     Attributes:
-        data: The text string in which you want to change the case.
-        transformation: Conversion mode.
+        data: A text to convert.
+        transformation: A conversion mode:
+            * `uppercase` — Makes all letters uppercase.
+            * `lowercase` — Makes all letters lowercase.
+            * `capitalize` — Capitalizes the first letter in the text, and leaves the rest lowercase. Note, that if there are several sentences, the rest of them are not capitalized.
     """
 
     class Transformation(toloka.util._extendable_enum.ExtendableStrEnum):
         """An enumeration.
         """
 
         UPPERCASE = 'uppercase'
@@ -394,26 +348,24 @@
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     version: typing.Optional[str]
     data: typing.Optional[typing.Any]
     transformation: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, Transformation]]
 
 
 class TransformHelperV1(BaseHelperV1):
-    """Creates a new array by transforming each of the elements in the original array.
+    """Creates a new array by transforming elements of another array.
+
+    For example, you can create an array of `view.image` components from an array of links to images.
+
+    For more information, see [helper.transform](https://toloka.ai/docs/template-builder/reference/helper.transform).
 
-    For example, you can convert an array of image links to view.image components to display these images. This may be
-    useful if the number of images in the array is unknown in advance
     Attributes:
-        into: Template to transform elements in the array. The array value can be substituted using the data.local
-            component. To do this, use the construction { "type": "data.local", "path": "item"}
-        items: The array that you want to convert. You can specify an array in three ways:
-            * Specify the array itself. Example: ["one", "two", "three"].
-            * Insert a reference to data (input, output, or internal). Example: {"type": "data.input",
-                "path": "path.to.data"}.
-            * Use a reference to another configuration element. Example: {"$ref": "vars.myarray"}.
+        into: The template of an element of the new array.
+            To insert values from the source array use the [LocalData](toloka.client.project.template_builder.data.LocalData.md) component with the data `path` set to `item`.
+        items: The source array.
     """
 
     def __init__(
         self,
         into: typing.Optional[typing.Any] = None,
         items: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Any]]] = None,
         *,
@@ -426,29 +378,20 @@
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     version: typing.Optional[str]
     into: typing.Optional[typing.Any]
     items: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Any]]]
 
 
 class TranslateHelperV1(BaseHelperV1):
-    """Component for translating interface elements to other languages.
-
-    In the properties that should be displayed in different languages, add:
+    """A component for translating interface elements to other languages.
 
-    >>> {
-    >>>     "type": "helper.translate",
-    >>>     "key": "<key name>"
-    >>> }
-    ...
-
-    Adding the key property displays a field for entering the key text. Enter the text in the source language. In the
-    "Translations" step, add translations for the keys in the desired languages.
+    For more information, see [helper.translate](https://toloka.ai/docs/template-builder/reference/helper.translate).
 
     Attributes:
-        key: The key for a text property that you will translate to other languages.
+        key: The key of a phrase that has translations.
     """
 
     def __init__(
         self,
         key: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]] = None,
         *,
         version: typing.Optional[str] = '1.0.0'
@@ -459,22 +402,20 @@
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     version: typing.Optional[str]
     key: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]]
 
 
 class YandexDiskProxyHelperV1(BaseHelperV1):
-    """You can use this component to download files from Yandex&#160;Disk.
+    """A component for downloading files from Yandex&#160;Disk.
+
+    For more information, see [helper.proxy](https://toloka.ai/docs/template-builder/reference/helper.proxy).
 
-    To use YandexDiskProxyHelper, connect Yandex&#160;Disk to your Toloka account and add the proxy by following
-    the [instructions](https://toloka.ai/en/docs/guide/concepts/prepare-data)
-    Select the component that you want to add, such as view.image for an image or view.audio for an audio file.
-    In the url property of this component, use YandexDiskProxyHelper.
     Attributes:
-        path: Path to the file in the <Proxy name>/<File name>.<type> format
+        path: A path to a file in the `/<Proxy name>/<File name>.<type>` format.
     """
 
     def __init__(
         self,
         path: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]] = None,
         *,
         version: typing.Optional[str] = '1.0.0'
```

### Comparing `toloka-kit-1.1.4/src/client/project/template_builder/layouts.pyi` & `toloka-kit-1.2.0/src/client/project/template_builder/layouts.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -20,20 +20,20 @@
         bases,
         namespace,
         **kwargs
     ): ...
 
 
 class BaseLayoutV1(toloka.client.project.template_builder.base.BaseComponent, metaclass=BaseLayoutV1Metaclass):
-    """Options for positioning elements in the interface, such as in columns or side-by-side.
+    """A base component for layouts.
 
-    If you have more than one element in the interface, these components will help you arrange them the way you want.
+    Layout components are used for positioning elements in the interface, such as in columns or side-by-side.
 
     Attributes:
-        validation: Validation based on condition.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         *,
         validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         version: typing.Optional[str] = '1.0.0'
@@ -44,26 +44,23 @@
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
 
 
 class BarsLayoutV1(BaseLayoutV1):
-    """A component that adds top and bottom bars to the content.
+    """A layout with top and bottom bars.
 
-    You can use other components inside each part of this component, such as images, text, or options.
-
-    The top bar is located at the top edge of the component, and the bottom one is at the bottom edge. The content is
-    placed between the bars and takes up all available space.
+    For more information, see [layout.bars](https://toloka.ai/docs/template-builder/reference/layout.bars).
 
     Attributes:
         content: The main content.
-        bar_after: The bar displayed at the bottom edge of the component.
-        bar_before: The bar displayed at the top edge of the component.
-        validation: Validation based on condition.
+        bar_after: The bar displayed below the main content.
+        bar_before: The bar displayed above the main content.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         content: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         *,
         bar_after: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
@@ -80,41 +77,36 @@
     version: typing.Optional[str]
     content: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     bar_after: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     bar_before: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
 
 
 class ColumnsLayoutV1(BaseLayoutV1):
-    """A component for placing content in columns.
+    """A layout with columns.
 
-    Use it to customize the display of content: set the column width and adjust the vertical alignment of content.
+    For more information, see [layout.columns](https://toloka.ai/docs/template-builder/reference/layout.columns).
 
     Attributes:
-        items: Columns to divide the interface into.
-        full_height: Switches the component to column mode at full height and with individual scrolling. Otherwise, the
-            height is determined by the height of the column that is filled in the most.
-        min_width: The minimum width of the component; if it is narrower, columns are output sequentially, one by one.
-        ratio: An array of values that specify the relative width of columns. For example, if you have 3 columns, the
-            value [1,2,1] divides the space into 4 parts and the column in the middle is twice as large as the other
-            columns.
-            If the number of columns exceeds the number of values in the ratio property, the values are repeated. For
-            example, if you have 4 columns and the ratio is set to [1,2], the result is the same as for [1,2,1,2].
-            If the number of columns is less than the number of values in the ratio property, extra values are simply
-            ignored.
-        vertical_align: Vertical alignment of column content.
-        validation: Validation based on condition.
+        items: A list of components. Every component is placed in an individual column.
+        full_height: A height mode:
+            * `True` — The component occupies all available vertical space. Columns have individual scrolling.
+            * `False` — The height of the component is determined by the highest column.
+        min_width: The minimum width of the component when columns are used. If the component is narrower than `min_width`, then all content is shown in one column.
+        ratio: A list of relative column widths.
+        vertical_align: The vertical alignment of column content.
+        validation: Validation rules.
     """
 
     class VerticalAlign(toloka.util._extendable_enum.ExtendableStrEnum):
-        """Vertical alignment of column content.
+        """The vertical alignment of column content.
 
         Attributes:
-            TOP: Aligned to the top of a column.
-            MIDDLE: Aligned to the middle of the column that is filled in the most.
-            BOTTOM: Aligned to the bottom of a column.
+            TOP: Aligning to the top of a column.
+            MIDDLE: Aligning to the middle of the highest.
+            BOTTOM: Aligning to the bottom of a column.
         """
 
         BOTTOM = 'bottom'
         MIDDLE = 'middle'
         TOP = 'top'
 
     def __init__(
@@ -139,20 +131,19 @@
     full_height: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]
     min_width: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, float]]
     ratio: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, float]]]]
     vertical_align: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, VerticalAlign]]
 
 
 class CompareLayoutItem(toloka.client.project.template_builder.base.BaseTemplate):
-    """The compared element.
+    """An item for the `CompareLayoutV1`.
 
     Attributes:
-        content: The content of the element that's being compared. Add images, audio recordings, videos, links,
-            or other types of data.
-        controls: Configure the input fields to make the Toloker select an item.
+        content: The content of the item.
+        controls: Item controls.
     """
 
     def __init__(
         self,
         content: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         controls: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None
     ) -> None:
@@ -162,34 +153,27 @@
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     content: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     controls: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
 
 
 class CompareLayoutV1(BaseLayoutV1):
-    """Use it to arrange interface elements for comparing them. For example, you can compare several photos.
-
-    Selection buttons can be placed under each of the compared items. You can also add common elements, such as a
-    field for comments.
-
-    Differences from layout.side-by-side:
+    """A layout for comparing several items.
 
-    * No buttons for hiding items. These are useful if you need to compare 5 photos at once and it's
-    difficult to choose between two of them.
-    * You can add individual selection buttons for every item being compared.
+    For more information, see [layout.compare](https://toloka.ai/docs/template-builder/reference/layout.compare).
 
     Attributes:
-        common_controls: The common fields of the component. Add information blocks that are common to all the
-            elements being compared.
-        items: An array with properties of the elements being compared. Set the appearance of the component blocks.
-        min_width: Minimum width of the element in pixels. Default: 400 pixels.
-        wide_common_controls: This property increases the common field size of the elements being compared.
-            It's set to false by default: the common fields are displayed in the center, not stretched. If true,
-            the fields are wider than with the default value.
-        validation: Validation based on condition.
+        common_controls: A component containing common controls.
+        items: A list of items to be compared.
+        min_width: The minimum width of the component in pixels. Default value: `400`.
+        wide_common_controls: * `True` — The common controls are stretched horizontally.
+            * `False` — The common controls are centered.
+
+            Default value: `False`.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         common_controls: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         items: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, CompareLayoutItem]]]] = None,
         *,
@@ -208,26 +192,23 @@
     common_controls: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     items: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, CompareLayoutItem]]]]
     min_width: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, float]]
     wide_common_controls: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]
 
 
 class SideBySideLayoutV1(BaseLayoutV1):
-    """The component displays several data blocks of the same width on a single horizontal panel.
-
-    For example, you can use this to compare several photos.
+    """A layout with several blocks of the same width on a single horizontal panel.
 
-    You can set the minimum width for data blocks.
+    For more information, see [layout.side-by-side](https://toloka.ai/docs/template-builder/reference/layout.side-by-side).
 
     Attributes:
-        controls: Components that let Tolokers perform the required actions.
-            For example: field.checkbox-group or field.button-radio-group.
-        items: An array of data blocks.
-        min_item_width: The minimum width of a data block, at least 400 pixels.
-        validation: Validation based on condition.
+        controls: A component with controls.
+        items: A list of blocks.
+        min_item_width: The minimum width of a block, at least 400 pixels.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         controls: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         items: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[toloka.client.project.template_builder.base.BaseComponent]]] = None,
         *,
@@ -244,37 +225,32 @@
     version: typing.Optional[str]
     controls: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     items: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[toloka.client.project.template_builder.base.BaseComponent]]]
     min_item_width: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, float]]
 
 
 class SidebarLayoutV1(BaseLayoutV1):
-    """An option for placing (layout) items, which lets you arrange on a page:
-
-    * The main content block.
-    * An adjacent panel with controls.
+    """A layout with a main content block and a panel with controls.
 
-    The minWidth property sets the threshold for switching between widescreen and compact modes: when the width of the
-    layout.sidebar component itself becomes less than the value set by the minWidth property, compact mode is enabled.
-
-    In widescreen mode, the control panel is located to the right of the main block.
-
-    In compact mode, controls stretch to the entire width and are located under each other.
-
-    To add an extra panel with controls, use the extraControls property.
-
-    Attributes:
-        content: Content placed in the main area.
-        controls: Content of the control panel.
-        controls_width: The width of the control panel in widescreen mode. In compact mode, the panel takes up the
-            entire available width. Default: 200 pixels.
-        extra_controls: An additional panel with controls. Located below the main panel.
-        min_width: The minimum width, in pixels, for widescreen mode. If the component width becomes less than the
-            specified value, the interface switches to compact mode. Default: 400 pixels.
-        validation: Validation based on condition.
+    The component supports modes:
+        * Widescreen — The control panel is placed to the right of the main block.
+        * Compact — The controls are placed under the main block and stretch to the entire width.
+
+    For more information, see [layout.sidebar](https://toloka.ai/docs/template-builder/reference/layout.sidebar).
+
+    Attributes:
+        content: The main block.
+        controls: The control panel.
+        controls_width: The width in pixels of the control panel in the widescreen mode.
+            Default value: `200`.
+        extra_controls: An additional panel with controls. It is placed below the controls.
+        min_width: The minimum width in pixels of the component in a widescreen mode.
+            If the component width is less than the specified value, the interface switches to the compact mode.
+            Default value: `400`.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         content: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         controls: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         *,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `toloka-kit-1.1.4/src/client/project/template_builder/plugins.pyi` & `toloka-kit-1.2.0/src/client/project/template_builder/plugins.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -8,48 +8,46 @@
 ]
 import toloka.client.project.template_builder.base
 import toloka.util._extendable_enum
 import typing
 
 
 class BasePluginV1(toloka.client.project.template_builder.base.BaseComponent, metaclass=toloka.client.project.template_builder.base.VersionedBaseComponentMetaclass):
-    """Plugins that provide expanded functionality. For example, you can use plugin.hotkeys to set up shortcuts.
+    """A base class for plugins.
     """
 
     def __init__(self, *, version: typing.Optional[str] = '1.0.0') -> None:
         """Method generated by attrs for class BasePluginV1.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     version: typing.Optional[str]
 
 
 class ImageAnnotationHotkeysPluginV1(BasePluginV1):
-    """Used to set hotkeys for the field.image-annotation component.
+    """Hotkeys for the [ImageAnnotationFieldV1](toloka.client.project.template_builder.fields.ImageAnnotationFieldV1.md) component.
 
-    You can set hotkeys to select area types and selection modes and to confirm or cancel area creation. When setting
-    hotkeys, you can use the up and down arrows (up,down), numbers, and Latin letters.
+    For more information, see [plugin.field.image-annotation.hotkeys](https://toloka.ai/docs/template-builder/reference/plugin.field.image-annotation.hotkeys).
 
     Attributes:
-        cancel: Keyboard shortcut for canceling area creation.
-        confirm: Keyboard shortcut for confirming area creation.
-        labels: Keyboard shortcuts for choosing area types. They're assigned to buttons in the order they are shown if
-            you enabled the option to choose multiple area types.
-        modes: Keyboard shortcuts for choosing selection modes.
+        cancel: A hotkey for canceling area creation.
+        confirm: A hotkey for confirming area creation.
+        labels: A list of hotkeys for choosing area labels.
+        modes: Hotkeys for switching selection modes.
     """
 
     class Mode(toloka.client.project.template_builder.base.BaseTemplate):
-        """Mode
+        """Selection mode hotkeys.
 
         Attributes:
-            point: Keyboard shortcut for selecting areas using points.
-            polygon: Keyboard shortcut for selecting areas using polygons.
-            rectangle: Keyboard shortcut for selecting areas using rectangles.
-            select: Keyboard shortcut for selecting shapes and points.
+            point: A hotkey for a point selection mode.
+            polygon: A hotkey for a polygon selection mode.
+            rectangle: A hotkey for a rectangle selection mode.
+            select: A hotkey for a mode for editing selections.
         """
 
         def __init__(
             self,
             *,
             point: typing.Optional[str] = None,
             polygon: typing.Optional[str] = None,
@@ -102,21 +100,21 @@
     cancel: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]]
     confirm: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]]
     labels: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[str]]]
     modes: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, Mode]]
 
 
 class TextAnnotationHotkeysPluginV1(BasePluginV1):
-    """Use this to set keyboard shortcuts for the field.text-annotation component.
+    """Hotkeys for the [TextAnnotationFieldV1](toloka.client.project.template_builder.fields.TextAnnotationFieldV1.md) component.
+
+    For more information, see [plugin.field.text-annotation.hotkeys](https://toloka.ai/docs/template-builder/reference/plugin.field.text-annotation.hotkeys).
 
     Attributes:
-        labels: Keyboard shortcuts for selecting categories. They're assigned to buttons with categories in the order
-            they're shown.
-        remove: Use this property to allow a Toloker to deselect an entire line or part of it. The key that you
-            assign to this property will deselect.
+        labels: A list of hotkeys for choosing labels.
+        remove: A hotkey for clearing the label of the annotated text.
     """
 
     def __init__(
         self,
         labels: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[str]]] = None,
         remove: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]] = None,
         *,
@@ -129,22 +127,25 @@
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     version: typing.Optional[str]
     labels: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[str]]]
     remove: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]]
 
 
 class HotkeysPluginV1(BasePluginV1):
-    """Lets you set keyboard shortcuts for actions.
+    """Hotkeys for actions.
 
-    Attributes:
-        key_ + [a-z|0-9|up|down]: An action that is triggered when you press the specified keyboard key. The keyboard
-            shortcut is set in the key, and the action is specified in the value
+    You can use as hotkeys:
+    * Letters
+    * Numbers
+    * Up and down arrows
+
+    Choose a hotkey using a named parameter of the `HotkeysPluginV1` and assign an action to it.
 
     Example:
-        How to create hotkeys for classification buttons.
+        Creating hotkeys for classification buttons.
 
         >>> hot_keys_plugin = tb.HotkeysPluginV1(
         >>>     key_1=tb.SetActionV1(tb.OutputData('result'), 'cat'),
         >>>     key_2=tb.SetActionV1(tb.OutputData('result'), 'dog'),
         >>>     key_3=tb.SetActionV1(tb.OutputData('result'), 'other'),
         >>> )
         ...
@@ -236,35 +237,31 @@
     key_8: typing.Optional[typing.Any]
     key_9: typing.Optional[typing.Any]
     key_up: typing.Optional[typing.Any]
     key_down: typing.Optional[typing.Any]
 
 
 class TriggerPluginV1(BasePluginV1):
-    """Use this to configure triggers that trigger a specific action when an event occurs.
+    """A plugin for triggering actions when events occur.
 
-    The action is set in the action property, and the event is described in the other fields.
+    For more information, see [plugin.trigger](https://toloka.ai/docs/template-builder/reference/plugin.trigger).
 
-    The event can be triggered immediately when the task is loaded ("fireImmediately": true) or when data changes in
-    the property specified in onChangeOf.
-
-    You can also set conditions in the conditions property that must be met in order for the trigger to fire.
     Attributes:
-        action: The action to perform when the trigger fires.
-        condition: The condition that must be met in order to fire the trigger.
-        fire_immediately: Flag indicating whether the trigger should be fired immediately after the task is loaded.
-        on_change_of: The data that triggers the action when changed.
+        action: An action to trigger.
+        condition: A condition that must be met in order to trigger the action.
+        fire_immediately: If `True` then the action is triggered immediately after the task is loaded.
+        on_change_of: The data change event that triggers the action.
 
     Example:
-        How to save Toloker's coordinates to the output.
+        How to save Toloker's coordinates.
 
         >>> coordinates_save_plugin = tb.plugins.TriggerPluginV1(
         >>>     fire_immediately=True,
         >>>     action=tb.actions.SetActionV1(
-        >>>         data=tb.data.OutputData(path='performer_coordinates'),
+        >>>         data=tb.data.OutputData(path='toloker_coordinates'),
         >>>         payload=tb.data.LocationData()
         >>>     ),
         >>> )
         ...
     """
 
     def __init__(
@@ -287,38 +284,40 @@
     fire_immediately: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]
     on_change_of: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
 
 
 class TolokaPluginV1(BasePluginV1):
     """A plugin with extra settings for tasks in Toloka.
 
+    For more information, see [plugin.toloka](https://toloka.ai/docs/template-builder/reference/plugin.toloka).
+
     Attributes:
         layout: Settings for the task appearance in Toloka.
         notifications: Notifications shown at the top of the page.
 
     Example:
-        How to set the task width on the task page.
+        Setting the width of the task block on a page.
 
         >>> task_width_plugin = tb.plugins.TolokaPluginV1(
-        >>>     'scroll',
+        >>>     kind='scroll',
         >>>     task_width=400,
         >>> )
         ...
     """
 
     class TolokaPluginLayout(toloka.client.project.template_builder.base.BaseTemplate):
-        """How to display task.
+        """A task block layout.
         """
 
         class Kind(toloka.util._extendable_enum.ExtendableStrEnum):
-            """An enumeration.
+            """A task block layout mode.
 
             Attributes:
-                SCROLL: (default) display multiple tasks on the page at the same time.
-                PAGER: display only one task on the page, with a button to switch between tasks at the bottom.
+                SCROLL: All tasks from a task suite are displayed on a page. It is the default mode.
+                PAGER: A single task is displayed on a page. Buttons at the bottom of the page show other tasks from a task suite.
             """
 
             PAGER = 'pager'
             SCROLL = 'scroll'
 
         def __init__(
             self,
```

### Comparing `toloka-kit-1.1.4/src/client/project/template_builder/view.py` & `toloka-kit-1.2.0/src/client/project/template_builder/view.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,478 +1,489 @@
-__all__ = [
-    'BaseViewV1',
-    'ActionButtonViewV1',
-    'AlertViewV1',
-    'AudioViewV1',
-    'CollapseViewV1',
-    'DeviceFrameViewV1',
-    'DividerViewV1',
-    'GroupViewV1',
-    'IframeViewV1',
-    'ImageViewV1',
-    'LabeledListViewV1',
-    'LinkViewV1',
-    'LinkGroupViewV1',
-    'ListViewV1',
-    'MapViewV1',
-    'MarkdownViewV1',
-    'TextViewV1',
-    'VideoViewV1'
-]
-from enum import unique
-from typing import List, Any
-
-from .base import (
-    BaseTemplate,
-    BaseComponent,
-    ListDirection,
-    ListSize,
-    ComponentType,
-    VersionedBaseComponentMetaclass,
-    base_component_or
-)
-from ....util._codegen import attribute
-from ....util._extendable_enum import ExtendableStrEnum
-from ....util._docstrings import inherit_docstrings
-
-
-class BaseViewV1Metaclass(VersionedBaseComponentMetaclass):
-    def __new__(mcs, name, bases, namespace, **kwargs):
-
-        if 'hint' not in namespace:
-            namespace['hint'] = attribute(kw_only=True)
-            namespace.setdefault('__annotations__', {})['hint'] = base_component_or(Any)
-        if 'label' not in namespace:
-            namespace['label'] = attribute(kw_only=True)
-            namespace.setdefault('__annotations__', {})['label'] = base_component_or(Any)
-        if 'validation' not in namespace:
-            namespace['validation'] = attribute(kw_only=True)
-            namespace.setdefault('__annotations__', {})['validation'] = BaseComponent
-        return super().__new__(mcs, name, bases, namespace, **kwargs)
-
-
-class BaseViewV1(BaseComponent, metaclass=BaseViewV1Metaclass):
-    """Elements displayed in the interface, such as text, list, audio player, or image.
-
-    Attributes:
-        label: Label above the component.
-        hint: Hint text.
-        validation: Validation based on condition.
-    """
-
-    pass
-
-
-@inherit_docstrings
-class ActionButtonViewV1(BaseViewV1, spec_value=ComponentType.VIEW_ACTION_BUTTON):
-    """Button that calls an action.
-
-    When clicking the button, an action specified in the action property is called.
-    Attributes:
-        action: Action called when clicking the button.
-        label: Button text.
-    """
-
-    action: BaseComponent
-
-
-@inherit_docstrings
-class AlertViewV1(BaseViewV1, spec_value=ComponentType.VIEW_ALERT):
-    """The component creates a color block to highlight important information.
-
-    You can use both plain text and other visual components inside it.
-    Attributes:
-        content: Content of the block with important information.
-        theme: Determines the block color.
-    """
-
-    @unique
-    class Theme(ExtendableStrEnum):
-        """An enumeration
-
-        Attributes:
-            INFO: (default) Blue.
-            SUCCESS: Green.
-            WARNING: Yellow.
-            DANGER: Red.
-        """
-
-        DANGER = 'danger'
-        INFO = 'info'
-        SUCCESS = 'success'
-        WARNING = 'warning'
-
-    content: BaseComponent
-    theme: base_component_or(Theme) = attribute(kw_only=True)
-
-
-@inherit_docstrings
-class AudioViewV1(BaseViewV1, spec_value=ComponentType.VIEW_AUDIO):
-    """The component plays audio.
-
-    Format support depends on the Toloker's browser, OS, and device. We recommend using MP3.
-    Attributes:
-        url: Audio link.
-        loop: Automatically replay audio.
-    """
-
-    url: base_component_or(Any)
-    loop: base_component_or(bool) = attribute(kw_only=True)
-
-
-@inherit_docstrings
-class CollapseViewV1(BaseViewV1, spec_value=ComponentType.VIEW_COLLAPSE):
-    """Expandable block.
-
-    Lets you add hidden content that doesn't need to be shown initially or that takes up a large space.
-
-    The block heading is always visible.
-
-    If you set the defaultOpened property to true, the block is expanded immediately, but it can be collapsed.
-    Attributes:
-        label: Block heading.
-        content: Content hidden in the block.
-        default_opened: If true, the block is immediately displayed in expanded form. By default, false (the block is
-            collapsed).
-    """
-
-    label: base_component_or(Any)
-    content: BaseComponent
-    default_opened: base_component_or(bool) = attribute(origin='defaultOpened', kw_only=True)
-
-
-@inherit_docstrings
-class DeviceFrameViewV1(BaseViewV1, spec_value=ComponentType.VIEW_DEVICE_FRAME):
-    """Wraps the content of a component in a frame that is similar to a mobile phone.
-
-    You can place other components inside the frame.
-    Attributes:
-        content: Content inside the frame.
-        full_height: If true, the element takes up all the vertical free space. The element is set to a minimum height
-            of 400 pixels.
-        max_width: Maximum width of the element in pixels, must be greater than min_width.
-        min_width: Minimum width of the element in pixels. Takes priority over max_width.
-        ratio: An array of two numbers that sets the relative dimensions of the sides: width (first number) to
-            height (second number). Not valid if full_height=true.
-    """
-
-    content: BaseComponent
-    full_height: base_component_or(bool) = attribute(origin='fullHeight', kw_only=True)
-    max_width: base_component_or(float) = attribute(origin='maxWidth', kw_only=True)
-    min_width: base_component_or(float) = attribute(origin='minWidth', kw_only=True)
-    ratio: base_component_or(List[base_component_or(float)], 'ListBaseComponentOrFloat') = attribute(kw_only=True)  # noqa: F821
-
-
-@inherit_docstrings
-class DividerViewV1(BaseViewV1, spec_value=ComponentType.VIEW_DIVIDER):
-    """Horizontal delimiter.
-
-    You can place extra elements in the center of the delimiter, like a popup hint and label.
-    Attributes:
-        label: A label in the center of the delimiter. Line breaks are not supported.
-    """
-
-    pass
-
-
-@inherit_docstrings
-class GroupViewV1(BaseViewV1, spec_value=ComponentType.VIEW_GROUP):
-    """Groups components visually into framed blocks.
-
-    Attributes:
-        content: Content of a group block.
-        label: Group heading.
-        hint: Explanation of the group heading. To insert a new line, use
-            .
-    """
-
-    content: BaseComponent
-
-
-@inherit_docstrings
-class IframeViewV1(BaseViewV1, spec_value=ComponentType.VIEW_IFRAME):
-    """Displays the web page at the URL in an iframe window.
-
-    Attributes:
-        url: URL of the web page.
-        full_height: If true, the element takes up all the vertical free space. The element is set to a minimum height
-            of 400 pixels.
-        max_width: Maximum width of the element in pixels, must be greater than min_width.
-        min_width: Minimum width of the element in pixels. Takes priority over max_width.
-        ratio: An array of two numbers that sets the relative dimensions of the sides: width (first number) to
-            height (second number). Not valid if full_height=true.
-    """
-
-    url: base_component_or(str)
-    full_height: base_component_or(bool) = attribute(origin='fullHeight', kw_only=True)
-    max_width: base_component_or(float) = attribute(origin='maxWidth', kw_only=True)
-    min_width: base_component_or(float) = attribute(origin='minWidth', kw_only=True)
-    ratio: base_component_or(List[base_component_or(float)], 'ListBaseComponentOrFloat') = attribute(kw_only=True)  # noqa: F821
-
-
-@inherit_docstrings
-class ImageViewV1(BaseViewV1, spec_value=ComponentType.VIEW_IMAGE):
-    """Displays an image.
-
-    Attributes:
-        url: Image link.
-        full_height: If true, the element takes up all the vertical free space. The element is set to a minimum height
-            of 400 pixels.
-        max_width: Maximum width of the element in pixels, must be greater than min_width.
-        min_width: Minimum width of the element in pixels. Takes priority over max_width.
-        no_border: Controls the display of a frame around an image. By default, true (the frame is hidden). Set false
-            to display the frame.
-        no_lazy_load: Disables lazy loading. If true, images start loading immediately, even if they aren't in the
-            viewport. Useful for icons. By default, false (lazy loading is enabled). In this mode, images start loading
-            only when a Toloker scrolls to them.
-        popup: Specifies whether opening a full-size image with a click is allowed. By default, it is true (allowed).
-        ratio: An array of two numbers that sets the relative dimensions of the sides: width (first number) to
-            height (second number). Not valid if full_height=true.
-        scrollable: When set to true, an image has scroll bars if it doesn't fit in the parent element.
-            If false, the image fits in the parent element and, when clicked, opens in its original size in the module
-            window.
-            Images in SVG format with no size specified always fit in their parent elements.
-    """
-
-    url: base_component_or(Any)
-    full_height: base_component_or(bool) = attribute(origin='fullHeight', kw_only=True)
-    max_width: base_component_or(float) = attribute(origin='maxWidth', kw_only=True)
-    min_width: base_component_or(float) = attribute(origin='minWidth', kw_only=True)
-    no_border: base_component_or(bool) = attribute(origin='noBorder', kw_only=True)
-    no_lazy_load: base_component_or(bool) = attribute(origin='noLazyLoad', kw_only=True)
-    popup: base_component_or(bool) = attribute(kw_only=True)
-    ratio: base_component_or(List[base_component_or(float)], 'ListBaseComponentOrFloat') = attribute(kw_only=True)  # noqa: F821
-    rotatable: base_component_or(bool) = attribute(kw_only=True)
-    scrollable: base_component_or(bool) = attribute(kw_only=True)
-
-
-@inherit_docstrings
-class LabeledListViewV1(BaseViewV1, spec_value=ComponentType.VIEW_LABELED_LIST):
-    """Displaying components as a list with labels placed on the left.
-
-    If you don't need labels, use view.list.
-    Attributes:
-        items: List items.
-        min_width: The minimum width of list content. If the component width is less than the specified value, it
-            switches to compact mode.
-    """
-
-    class Item(BaseTemplate):
-        """Item.
-
-        Attributes:
-            content: List item content.
-            label: A label displayed next to a list item.
-            center_label: If true, a label is center-aligned relative to the content of a list item (content). Use it
-                if the list consists of large items, such as images or multi-line text.
-                By default, false (the label is aligned to the top of the content block).
-            hint: A pop-up hint displayed next to a label.
-        """
-
-        content: BaseComponent
-        label: base_component_or(Any)
-        center_label: base_component_or(bool) = attribute(origin='centerLabel', kw_only=True)
-        hint: base_component_or(Any) = attribute(kw_only=True)
-
-    items: base_component_or(List[base_component_or(Item)], 'ListBaseComponentOrItem')  # noqa: F821
-    min_width: base_component_or(float) = attribute(origin='minWidth', kw_only=True)
-
-
-@inherit_docstrings
-class LinkViewV1(BaseViewV1, spec_value=ComponentType.VIEW_LINK):
-    """Universal way to add a link.
-
-    This link changes color when clicked.
-
-    We recommend using this component if you need to insert a link without additional formatting.
-
-    If you want to insert a button that will open the link, use the view.action-button and action.open-link components.
-
-    To insert a link with a search query, use helper.search-query.
-    Attributes:
-        url: Link URL.
-        content: Link text displayed to the Toloker.
-    """
-
-    url: base_component_or(Any)
-    content: base_component_or(Any) = attribute(kw_only=True)
-
-
-@inherit_docstrings
-class LinkGroupViewV1(BaseViewV1, spec_value=ComponentType.VIEW_LINK_GROUP):
-    """Puts links into groups
-
-    The most important link in a group can be highlighted with a border: set the theme property to primary for this link.
-    This only groups links, unlike GroupViewV1.
-
-    Attributes:
-        links: Array of links that make up a group.
-
-    Example:
-        How to add several links.
-
-        >>> links = tb.view.LinkGroupViewV1(
-        >>>     [
-        >>>         tb.view.LinkGroupViewV1.Link(
-        >>>             'https://any.com/useful/url/1',
-        >>>             'Example1',
-        >>>         ),
-        >>>         tb.view.LinkGroupViewV1.Link(
-        >>>             'https://any.com/useful/url/2',
-        >>>             'Example2',
-        >>>         ),
-        >>>     ]
-        >>> )
-        ...
-    """
-
-    class Link(BaseTemplate):
-        """Link parameters
-
-        Attributes:
-            url: Link address
-            content: Link text that's displayed to a Toloker. Unvisited links are blue and underlined, and visited links are purple.
-            theme: Defines the appearance of the link. If you specify "theme": "primary", it's a button, otherwise it's a text link.
-        """
-
-        url: base_component_or(str)
-        content: base_component_or(str)
-        theme: base_component_or(str) = attribute(kw_only=True)
-
-    links: base_component_or(List[base_component_or(Link)], 'ListBaseComponentOrLink')  # noqa: F821
-
-
-@inherit_docstrings
-class ListViewV1(BaseViewV1, spec_value=ComponentType.VIEW_LIST):
-    """Block for displaying data in a list.
-
-    Attributes:
-        items:  Array of list items.
-        direction: Determines the direction of the list.
-        size: Specifies the size of the margins between elements. Acceptable values in ascending order: s, m (default
-            value).
-    """
-
-    items: base_component_or(List[BaseComponent], 'ListBaseComponent')  # noqa: F821
-    direction: base_component_or(ListDirection) = attribute(kw_only=True)
-    size: base_component_or(ListSize) = attribute(kw_only=True)
-
-
-@inherit_docstrings
-class MarkdownViewV1(BaseViewV1, spec_value=ComponentType.VIEW_MARKDOWN):
-    """Block for displaying text in Markdown.
-
-    The contents of the block are written to the content property in a single line. To insert line breaks, use \\n
-    Straight quotation marks (") must be escaped like this: \\".
-
-    Note that the view.markdown component is resource-intensive and might overload weak devices.
-    Do not use this component to display plain text. If you need to display text without formatting, use the view.text
-    component. If you need to insert a link, use view.link, and for an image use view.image.
-    Links with Markdown are appended with target="_blank" (the link opens in a new tab), as well as
-    rel="noopener noreferrer"
-
-    Attributes:
-        content: Text in Markdown.
-
-    Example:
-        How to add a title and description on the task interface.
-
-        >>> header = tb.view.MarkdownViewV1('# Some Header:\n---\nSome detailed description')
-        ...
-    """
-
-    content: base_component_or(Any)
-
-
-@inherit_docstrings
-class TextViewV1(BaseViewV1, spec_value=ComponentType.VIEW_TEXT):
-    """Block for displaying text.
-
-    If you need formatted text, use view.markdown.
-    Attributes:
-        content: The text displayed in the block. To insert a new line, use \n
-
-    Example:
-        How to show labeled field from the task inputs.
-
-        >>> text_view = tb.view.TextViewV1(tb.data.InputData('input_field_name'), label='My label:')
-        ...
-    """
-
-    content: base_component_or(Any)
-
-
-@inherit_docstrings
-class VideoViewV1(BaseViewV1, spec_value=ComponentType.VIEW_VIDEO):
-    """Player for video playback.
-
-    The player is a rectangular block with a frame and buttons to control the video. You can set the block size using
-    the ratio, fullHeight, minWidth, and maxWidth properties.
-
-    The video resolution does not affect the size of the block — the video will fit into the block and will not be
-    cropped.
-    Attributes:
-        url: Link to the video file.
-        full_height: If true, the element takes up all the vertical free space. The element is set to a minimum height
-            of 400 pixels.
-        max_width: Maximum width of the element in pixels, must be greater than min_width.
-        min_width: Minimum width of the element in pixels. Takes priority over max_width.
-        ratio: The aspect ratio of the video block. An array of two numbers: the first sets the width of the block and
-            the second sets the height.
-    """
-
-    url: base_component_or(Any)
-    full_height: base_component_or(bool) = attribute(origin='fullHeight', kw_only=True)
-    max_width: base_component_or(float) = attribute(origin='maxWidth', kw_only=True)
-    min_width: base_component_or(float) = attribute(origin='minWidth', kw_only=True)
-    ratio: base_component_or(List[base_component_or(float)], 'ListBaseComponentOrFloat') = attribute(kw_only=True)  # noqa: F821
-
-
-@inherit_docstrings
-class MapViewV1(BaseViewV1, spec_value=ComponentType.VIEW_MAP):
-    """Adds a map to your task.
-
-    Use this component to set the targets for the tasks with the markers, select the areas with polygons.
-    Specify the position and colors for the elements on the map.
-
-    You can set the following map properties: scale, position of the map center, label, and hint for Tolokers.
-    Attributes:
-        center: Determines the position of the map center. Specify the coordinates in the string format, for example,
-            "29.748713,-95.404287", or use the data.location component to set the center of the map to the
-            Toloker's current position.
-        markers: Specifies the markers present on the map.
-        polygons: Specifies the polygonal objects that you can use to select areas on the map.
-        zoom: The map initial scale. Use the values from 0 to 19. Bigger values give a more detailed map view.
-    """
-
-    class Marker(BaseTemplate):
-        """Marker parameters.
-
-        Attributes:
-            position: Determines the marker position. Specify the coordinates in the string format, for example,
-                "29.748713,-95.404287", or use the data.location component to set the marker to the Toloker's current
-                position.
-            color: Determines the marker color. Use the hexadecimal values preceded by the # sign to specify the color.
-            label: The label for the marker that tells Tolokers what this marker is for and helps distinguish it
-                from other markers.
-        """
-        position: base_component_or(str)
-        color: base_component_or(str) = attribute(kw_only=True)
-        label: base_component_or(str) = attribute(kw_only=True)
-
-    class Polygon(BaseTemplate):
-        """Polygon parameters.
-
-        Attributes:
-            points: The list of the polygonal selection area points.
-                Specify the coordinates in the string format, for example, "29.748713,-95.404287".
-            color: Determines the polygonal selection area color. Use the hexadecimal values preceded by the # sign to
-                specify the color.
-        """
-        points: base_component_or(List[base_component_or(str)], 'ListBaseComponentOrStr')  # noqa: F821
-        color: base_component_or(str) = attribute(kw_only=True)
-
-    center: base_component_or(str)
-    markers: base_component_or(List[base_component_or(Marker)], 'ListBaseComponentOrMarker') = attribute(kw_only=True)  # noqa: F821
-    polygons: base_component_or(List[base_component_or(Polygon)], 'ListBaseComponentOrPolygon') = attribute(  # noqa: F821
-        kw_only=True)
-    zoom: base_component_or(int) = attribute(kw_only=True)
+__all__ = [
+    'BaseViewV1',
+    'ActionButtonViewV1',
+    'AlertViewV1',
+    'AudioViewV1',
+    'CollapseViewV1',
+    'DeviceFrameViewV1',
+    'DividerViewV1',
+    'GroupViewV1',
+    'IframeViewV1',
+    'ImageViewV1',
+    'LabeledListViewV1',
+    'LinkViewV1',
+    'LinkGroupViewV1',
+    'ListViewV1',
+    'MapViewV1',
+    'MarkdownViewV1',
+    'TextViewV1',
+    'VideoViewV1'
+]
+from enum import unique
+from typing import List, Any
+
+from .base import (
+    BaseTemplate,
+    BaseComponent,
+    ListDirection,
+    ListSize,
+    ComponentType,
+    VersionedBaseComponentMetaclass,
+    base_component_or
+)
+from ....util._codegen import attribute
+from ....util._extendable_enum import ExtendableStrEnum
+from ....util._docstrings import inherit_docstrings
+
+
+class BaseViewV1Metaclass(VersionedBaseComponentMetaclass):
+    def __new__(mcs, name, bases, namespace, **kwargs):
+
+        if 'hint' not in namespace:
+            namespace['hint'] = attribute(kw_only=True)
+            namespace.setdefault('__annotations__', {})['hint'] = base_component_or(Any)
+        if 'label' not in namespace:
+            namespace['label'] = attribute(kw_only=True)
+            namespace.setdefault('__annotations__', {})['label'] = base_component_or(Any)
+        if 'validation' not in namespace:
+            namespace['validation'] = attribute(kw_only=True)
+            namespace.setdefault('__annotations__', {})['validation'] = BaseComponent
+        return super().__new__(mcs, name, bases, namespace, **kwargs)
+
+
+class BaseViewV1(BaseComponent, metaclass=BaseViewV1Metaclass):
+    """A base class for components that present data, such as a text, list, audio player, or image.
+
+    Attributes:
+        label: A label above the component.
+        hint: A hint text.
+        validation: Validation rules.
+    """
+
+    pass
+
+
+@inherit_docstrings
+class ActionButtonViewV1(BaseViewV1, spec_value=ComponentType.VIEW_ACTION_BUTTON):
+    """A button that calls an action.
+
+    For more information, see [view.action-button](https://toloka.ai/docs/template-builder/reference/view.action-button).
+
+    Attributes:
+        action: The action.
+        label: A label on the button.
+    """
+
+    action: BaseComponent
+
+
+@inherit_docstrings
+class AlertViewV1(BaseViewV1, spec_value=ComponentType.VIEW_ALERT):
+    """A view used to highlight important information.
+
+    For more information, see [view.alert](https://toloka.ai/docs/template-builder/reference/view.alert).
+
+    Attributes:
+        content: The content.
+        theme: The theme that sets the background color. The default color is blue.
+    """
+
+    @unique
+    class Theme(ExtendableStrEnum):
+        """A view background color.
+
+        Attributes:
+            INFO: Blue.
+            SUCCESS: Green.
+            WARNING: Yellow.
+            DANGER: Red.
+        """
+
+        DANGER = 'danger'
+        INFO = 'info'
+        SUCCESS = 'success'
+        WARNING = 'warning'
+
+    content: BaseComponent
+    theme: base_component_or(Theme) = attribute(kw_only=True)
+
+
+@inherit_docstrings
+class AudioViewV1(BaseViewV1, spec_value=ComponentType.VIEW_AUDIO):
+    """An audio player.
+
+    For more information, see [view.audio](https://toloka.ai/docs/template-builder/reference/view.audio).
+
+    Attributes:
+        url: A link to the audio.
+        loop:
+            * `True` — Play audio in a loop.
+            * `False` — Play once.
+    """
+
+    url: base_component_or(Any)
+    loop: base_component_or(bool) = attribute(kw_only=True)
+
+
+@inherit_docstrings
+class CollapseViewV1(BaseViewV1, spec_value=ComponentType.VIEW_COLLAPSE):
+    """An expandable block.
+
+    For more information, see [view.collapse](https://toloka.ai/docs/template-builder/reference/view.collapse).
+
+    Attributes:
+        label: The block heading.
+        content: The block content.
+        default_opened: Initial state of the block:
+            `True` — Expanded
+            `False` — Collapsed
+
+            Default value: `False`.
+    """
+
+    label: base_component_or(Any)
+    content: BaseComponent
+    default_opened: base_component_or(bool) = attribute(origin='defaultOpened', kw_only=True)
+
+
+@inherit_docstrings
+class DeviceFrameViewV1(BaseViewV1, spec_value=ComponentType.VIEW_DEVICE_FRAME):
+    """A view with a frame that is similar to a mobile phone frame.
+
+    For more information, see [view.device-frame](https://toloka.ai/docs/template-builder/reference/view.device-frame).
+
+    Attributes:
+        content: The content of the frame.
+        full_height: If `True`, the component takes up all the vertical free space.
+            Note, that the minimum height required by the component is 400 pixels.
+        max_width: The maximum width of the component in pixels.
+        min_width: The minimum width of the component in pixels. It takes priority over the `max_width`.
+        ratio: A list with the aspect ratio of the component. Specify the relative width first and then the relative height.
+            This setting is not used if `full_height=True`.
+    """
+
+    content: BaseComponent
+    full_height: base_component_or(bool) = attribute(origin='fullHeight', kw_only=True)
+    max_width: base_component_or(float) = attribute(origin='maxWidth', kw_only=True)
+    min_width: base_component_or(float) = attribute(origin='minWidth', kw_only=True)
+    ratio: base_component_or(List[base_component_or(float)], 'ListBaseComponentOrFloat') = attribute(kw_only=True)  # noqa: F821
+
+
+@inherit_docstrings
+class DividerViewV1(BaseViewV1, spec_value=ComponentType.VIEW_DIVIDER):
+    """A horizontal delimiter.
+
+    For more information, see [view.divider](https://toloka.ai/docs/template-builder/reference/view.divider).
+
+    Attributes:
+        label: A label in the center of the delimiter. Note, that line breaks are not supported.
+    """
+
+    pass
+
+
+@inherit_docstrings
+class GroupViewV1(BaseViewV1, spec_value=ComponentType.VIEW_GROUP):
+    """A view with a frame.
+
+    For more information, see [view.group](https://toloka.ai/docs/template-builder/reference/view.group).
+
+    Attributes:
+        content: A content.
+        label: A header.
+        hint: A hint. To insert a line break in the hint, use `\n`.
+    """
+
+    content: BaseComponent
+
+
+@inherit_docstrings
+class IframeViewV1(BaseViewV1, spec_value=ComponentType.VIEW_IFRAME):
+    """A frame displaying a web page.
+
+    For more information, see [view.iframe](https://toloka.ai/docs/template-builder/reference/view.iframe).
+
+    Attributes:
+        url: The URL of the web page.
+        full_height: If `True`, the component takes up all the vertical free space.
+            Note, that the minimum height required by the component is 400 pixels.
+        max_width: The maximum width of the component in pixels.
+        min_width: The minimum width of the component in pixels. It takes priority over the `max_width`.
+        ratio: A list with the aspect ratio of the component. Specify the relative width first and then the relative height.
+            This setting is not used if `full_height=True`.
+    """
+
+    url: base_component_or(str)
+    full_height: base_component_or(bool) = attribute(origin='fullHeight', kw_only=True)
+    max_width: base_component_or(float) = attribute(origin='maxWidth', kw_only=True)
+    min_width: base_component_or(float) = attribute(origin='minWidth', kw_only=True)
+    ratio: base_component_or(List[base_component_or(float)], 'ListBaseComponentOrFloat') = attribute(kw_only=True)  # noqa: F821
+
+
+@inherit_docstrings
+class ImageViewV1(BaseViewV1, spec_value=ComponentType.VIEW_IMAGE):
+    """A component for displaying an image.
+
+    For more information, see [view.image](https://toloka.ai/docs/template-builder/reference/view.image).
+
+    Attributes:
+        url: The URL of the image.
+        full_height: If `True`, the component takes up all the vertical free space.
+            Note, that the minimum height required by the component is 400 pixels.
+        max_width: The maximum width of the component in pixels.
+        min_width: The minimum width of the component in pixels. It takes priority over the `max_width`.
+        no_border: Displaying borders around the image.
+            * `True` — The borders are hidden.
+            * `False` — The borders are visible.
+
+            Default value: `True`.
+        no_lazy_load: Loading mode:
+            * `False` — The component starts loading the image when the component becomes visible to a Toloker.
+            * `True` — The image is loaded immediately. This mode is useful for icons.
+
+            Default value: `False` — lazy loading is enabled.
+        popup: If `True`, a Toloker can open a full sized image in a popup. It is a default behavior.
+        ratio: A list with the aspect ratio of the component. Specify the relative width first and then the relative height.
+            This setting is not used if `full_height=True`.
+        rotatable: If `True`, an image can be rotated.
+        scrollable: The way of displaying an image which is larger than the component:
+            * `True` — Scroll bars are shown.
+            * `False` — The image is scaled to fit the component.
+
+            Note, that images in SVG format with no size specified always fit the component.
+    """
+
+    url: base_component_or(Any)
+    full_height: base_component_or(bool) = attribute(origin='fullHeight', kw_only=True)
+    max_width: base_component_or(float) = attribute(origin='maxWidth', kw_only=True)
+    min_width: base_component_or(float) = attribute(origin='minWidth', kw_only=True)
+    no_border: base_component_or(bool) = attribute(origin='noBorder', kw_only=True)
+    no_lazy_load: base_component_or(bool) = attribute(origin='noLazyLoad', kw_only=True)
+    popup: base_component_or(bool) = attribute(kw_only=True)
+    ratio: base_component_or(List[base_component_or(float)], 'ListBaseComponentOrFloat') = attribute(kw_only=True)  # noqa: F821
+    rotatable: base_component_or(bool) = attribute(kw_only=True)
+    scrollable: base_component_or(bool) = attribute(kw_only=True)
+
+
+@inherit_docstrings
+class LabeledListViewV1(BaseViewV1, spec_value=ComponentType.VIEW_LABELED_LIST):
+    """A list of components with labels placed on the left.
+
+    For more information, see [view.labeled-list](https://toloka.ai/docs/template-builder/reference/view.labeled-list).
+
+    Attributes:
+        items: List items.
+        min_width: The minimum width of the component.
+            If the width is less than the specified value, the list is displayed in compact mode.
+            Labels are placed above the items in this mode.
+    """
+
+    class Item(BaseTemplate):
+        """A labeled list item.
+
+        Attributes:
+            content: The content of the item.
+            label: An item label.
+            center_label: Label vertical alignment.
+                * `True` — The label is centered.
+                * `False` — The label is aligned to the top of the item content.
+
+                Default value: `False`.
+            hint: A hint.
+        """
+
+        content: BaseComponent
+        label: base_component_or(Any)
+        center_label: base_component_or(bool) = attribute(origin='centerLabel', kw_only=True)
+        hint: base_component_or(Any) = attribute(kw_only=True)
+
+    items: base_component_or(List[base_component_or(Item)], 'ListBaseComponentOrItem')  # noqa: F821
+    min_width: base_component_or(float) = attribute(origin='minWidth', kw_only=True)
+
+
+@inherit_docstrings
+class LinkViewV1(BaseViewV1, spec_value=ComponentType.VIEW_LINK):
+    """A component showing a link.
+
+    For more information, see [view.link](https://toloka.ai/docs/template-builder/reference/view.link).
+
+    Attributes:
+        url: A URL.
+        content: A link text.
+    """
+
+    url: base_component_or(Any)
+    content: base_component_or(Any) = attribute(kw_only=True)
+
+
+@inherit_docstrings
+class LinkGroupViewV1(BaseViewV1, spec_value=ComponentType.VIEW_LINK_GROUP):
+    """A group of links.
+
+    For more information, see [view.link-group](https://toloka.ai/docs/template-builder/reference/view.link-group).
+
+    Attributes:
+        links: A list of links.
+
+    Example:
+        >>> links = tb.view.LinkGroupViewV1(
+        >>>     [
+        >>>         tb.view.LinkGroupViewV1.Link(
+        >>>             'https://any.com/useful/url/1',
+        >>>             'Example1',
+        >>>         ),
+        >>>         tb.view.LinkGroupViewV1.Link(
+        >>>             'https://any.com/useful/url/2',
+        >>>             'Example2',
+        >>>         ),
+        >>>     ]
+        >>> )
+        ...
+    """
+
+    class Link(BaseTemplate):
+        """A link for the `LinkGroupViewV1`.
+
+        Attributes:
+            url: A URL.
+            content: A link text.
+            theme: The appearance of the link.
+                If `theme` is omitted, the link is displayed as an underlined text.
+                If `theme` is set to `primary`, a button is displayed.
+        """
+
+        url: base_component_or(str)
+        content: base_component_or(str)
+        theme: base_component_or(str) = attribute(kw_only=True)
+
+    links: base_component_or(List[base_component_or(Link)], 'ListBaseComponentOrLink')  # noqa: F821
+
+
+@inherit_docstrings
+class ListViewV1(BaseViewV1, spec_value=ComponentType.VIEW_LIST):
+    """A list of components.
+
+    For more information, see [view.list](https://toloka.ai/docs/template-builder/reference/view.list).
+
+    Attributes:
+        items: List items.
+        direction: The direction of the list:
+            * `vertical`
+            * `horizontal`
+
+            Default value: `vertical`.
+        size: A spacing between list items:
+            `m` — The default spacing.
+            `s` — Narrower spacing.
+    """
+
+    items: base_component_or(List[BaseComponent], 'ListBaseComponent')  # noqa: F821
+    direction: base_component_or(ListDirection) = attribute(kw_only=True)
+    size: base_component_or(ListSize) = attribute(kw_only=True)
+
+
+@inherit_docstrings
+class MarkdownViewV1(BaseViewV1, spec_value=ComponentType.VIEW_MARKDOWN):
+    """A component for formatting Markdown.
+
+    The Markdown content must not contain line breaks. To insert them, place `\n` in the text.
+    Straight quotation marks must be escaped: `\"`.
+
+    For more information, see [view.markdown](https://toloka.ai/docs/template-builder/reference/view.markdown).
+
+    Attributes:
+        content: A text with Markdown.
+
+    Example:
+        Adding a title and description using Markdown.
+
+        >>> header = tb.view.MarkdownViewV1('# Some Header:\n---\nSome detailed description')
+        ...
+    """
+
+    content: base_component_or(Any)
+
+
+@inherit_docstrings
+class TextViewV1(BaseViewV1, spec_value=ComponentType.VIEW_TEXT):
+    """A view for displaying a text.
+
+    For more information, see [view.text](https://toloka.ai/docs/template-builder/reference/view.text).
+
+    Attributes:
+        content: The text. To insert a new line, use `\n`.
+
+    Example:
+        >>> text_view = tb.view.TextViewV1(tb.data.InputData('input_field_name'), label='My label:')
+        ...
+    """
+
+    content: base_component_or(Any)
+
+
+@inherit_docstrings
+class VideoViewV1(BaseViewV1, spec_value=ComponentType.VIEW_VIDEO):
+    """A video player.
+
+    For more information, see [view.video](https://toloka.ai/docs/template-builder/reference/view.video).
+
+    Attributes:
+        url: The video URL.
+        full_height: If `True`, the component takes up all the vertical free space.
+            Note, that the minimum height required by the component is 400 pixels.
+        max_width: The maximum width of the component in pixels.
+        min_width: The minimum width of the component in pixels. It takes priority over the `max_width`.
+        ratio: A list with the aspect ratio of the component. Specify the relative width first and then the relative height.
+    """
+
+    url: base_component_or(Any)
+    full_height: base_component_or(bool) = attribute(origin='fullHeight', kw_only=True)
+    max_width: base_component_or(float) = attribute(origin='maxWidth', kw_only=True)
+    min_width: base_component_or(float) = attribute(origin='minWidth', kw_only=True)
+    ratio: base_component_or(List[base_component_or(float)], 'ListBaseComponentOrFloat') = attribute(kw_only=True)  # noqa: F821
+
+
+@inherit_docstrings
+class MapViewV1(BaseViewV1, spec_value=ComponentType.VIEW_MAP):
+    """A component for displaying a map.
+
+    For more information, see [view.map](https://toloka.ai/docs/template-builder/reference/view.map).
+
+    Attributes:
+        center: The coordinates of the map center. You can use:
+            * A string. For example, `29.748713,-95.404287`
+            * The [LocationData](toloka.client.project.template_builder.data.LocationData.md) to set Toloker's current position.
+        markers: A list of map markers.
+        polygons: A list of areas highlighted on the map.
+        zoom: An initial map scale. Use values from 0 to 19. Higher values zoom in the map.
+    """
+
+    class Marker(BaseTemplate):
+        """A map marker.
+
+        Attributes:
+            position: The coordinates of the marker. You can use:
+                * A string. For example, `29.748713,-95.404287`.
+                * The [LocationData](toloka.client.project.template_builder.data.LocationData.md) to set Toloker's current position.
+            color: The marker color. Use the hexadecimal values preceded by the `#`. For example, `#f00` makes the marker red.
+            label: A marker label.
+        """
+        position: base_component_or(str)
+        color: base_component_or(str) = attribute(kw_only=True)
+        label: base_component_or(str) = attribute(kw_only=True)
+
+    class Polygon(BaseTemplate):
+        """A map polygon.
+
+        Attributes:
+            points: A list of polygon coordinates.
+                Specify the coordinates in the string format, for example `29.748713,-95.404287`.
+            color: The color of the polygon. Use the hexadecimal values preceded by the `#`. For example, `#f00` makes the polygon red.
+        """
+        points: base_component_or(List[base_component_or(str)], 'ListBaseComponentOrStr')  # noqa: F821
+        color: base_component_or(str) = attribute(kw_only=True)
+
+    center: base_component_or(str)
+    markers: base_component_or(List[base_component_or(Marker)], 'ListBaseComponentOrMarker') = attribute(kw_only=True)  # noqa: F821
+    polygons: base_component_or(List[base_component_or(Polygon)], 'ListBaseComponentOrPolygon') = attribute(  # noqa: F821
+        kw_only=True)
+    zoom: base_component_or(int) = attribute(kw_only=True)
```

### Comparing `toloka-kit-1.1.4/src/client/project/template_builder/view.pyi` & `toloka-kit-1.2.0/src/client/project/template_builder/view.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -31,20 +31,20 @@
         bases,
         namespace,
         **kwargs
     ): ...
 
 
 class BaseViewV1(toloka.client.project.template_builder.base.BaseComponent, metaclass=BaseViewV1Metaclass):
-    """Elements displayed in the interface, such as text, list, audio player, or image.
+    """A base class for components that present data, such as a text, list, audio player, or image.
 
     Attributes:
-        label: Label above the component.
-        hint: Hint text.
-        validation: Validation based on condition.
+        label: A label above the component.
+        hint: A hint text.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         *,
         hint: typing.Optional[typing.Any] = None,
         label: typing.Optional[typing.Any] = None,
@@ -59,23 +59,23 @@
     hint: typing.Optional[typing.Any]
     label: typing.Optional[typing.Any]
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
 
 
 class ActionButtonViewV1(BaseViewV1):
-    """Button that calls an action.
+    """A button that calls an action.
 
-    When clicking the button, an action specified in the action property is called.
+    For more information, see [view.action-button](https://toloka.ai/docs/template-builder/reference/view.action-button).
 
     Attributes:
-        action: Action called when clicking the button.
-        hint: Hint text.
-        label: Button text.
-        validation: Validation based on condition.
+        action: The action.
+        hint: A hint text.
+        label: A label on the button.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         action: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         *,
         hint: typing.Optional[typing.Any] = None,
@@ -92,31 +92,31 @@
     label: typing.Optional[typing.Any]
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
     action: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
 
 
 class AlertViewV1(BaseViewV1):
-    """The component creates a color block to highlight important information.
+    """A view used to highlight important information.
 
-    You can use both plain text and other visual components inside it.
+    For more information, see [view.alert](https://toloka.ai/docs/template-builder/reference/view.alert).
 
     Attributes:
-        content: Content of the block with important information.
-        theme: Determines the block color.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        content: The content.
+        theme: The theme that sets the background color. The default color is blue.
+        hint: A hint text.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     class Theme(toloka.util._extendable_enum.ExtendableStrEnum):
-        """An enumeration
+        """A view background color.
 
         Attributes:
-            INFO: (default) Blue.
+            INFO: Blue.
             SUCCESS: Green.
             WARNING: Yellow.
             DANGER: Red.
         """
 
         DANGER = 'danger'
         INFO = 'info'
@@ -143,24 +143,25 @@
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
     content: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     theme: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, Theme]]
 
 
 class AudioViewV1(BaseViewV1):
-    """The component plays audio.
+    """An audio player.
 
-    Format support depends on the Toloker's browser, OS, and device. We recommend using MP3.
+    For more information, see [view.audio](https://toloka.ai/docs/template-builder/reference/view.audio).
 
     Attributes:
-        url: Audio link.
-        loop: Automatically replay audio.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        url: A link to the audio.
+        loop: * `True` — Play audio in a loop.
+            * `False` — Play once.
+        hint: A hint text.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         url: typing.Optional[typing.Any] = None,
         *,
         loop: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]] = None,
@@ -179,29 +180,28 @@
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
     url: typing.Optional[typing.Any]
     loop: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]
 
 
 class CollapseViewV1(BaseViewV1):
-    """Expandable block.
+    """An expandable block.
 
-    Lets you add hidden content that doesn't need to be shown initially or that takes up a large space.
-
-    The block heading is always visible.
-
-    If you set the defaultOpened property to true, the block is expanded immediately, but it can be collapsed.
+    For more information, see [view.collapse](https://toloka.ai/docs/template-builder/reference/view.collapse).
 
     Attributes:
-        content: Content hidden in the block.
-        label: Block heading.
-        default_opened: If true, the block is immediately displayed in expanded form. By default, false (the block is
-            collapsed).
-        hint: Hint text.
-        validation: Validation based on condition.
+        content: The block content.
+        label: The block heading.
+        default_opened: Initial state of the block:
+            `True` — Expanded
+            `False` — Collapsed
+
+            Default value: `False`.
+        hint: A hint text.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         content: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         *,
         label: typing.Optional[typing.Any] = None,
@@ -220,29 +220,29 @@
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
     content: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     default_opened: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]
 
 
 class DeviceFrameViewV1(BaseViewV1):
-    """Wraps the content of a component in a frame that is similar to a mobile phone.
+    """A view with a frame that is similar to a mobile phone frame.
 
-    You can place other components inside the frame.
+    For more information, see [view.device-frame](https://toloka.ai/docs/template-builder/reference/view.device-frame).
 
     Attributes:
-        content: Content inside the frame.
-        full_height: If true, the element takes up all the vertical free space. The element is set to a minimum height
-            of 400 pixels.
-        max_width: Maximum width of the element in pixels, must be greater than min_width.
-        min_width: Minimum width of the element in pixels. Takes priority over max_width.
-        ratio: An array of two numbers that sets the relative dimensions of the sides: width (first number) to
-            height (second number). Not valid if full_height=true.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        content: The content of the frame.
+        full_height: If `True`, the component takes up all the vertical free space.
+            Note, that the minimum height required by the component is 400 pixels.
+        max_width: The maximum width of the component in pixels.
+        min_width: The minimum width of the component in pixels. It takes priority over the `max_width`.
+        ratio: A list with the aspect ratio of the component. Specify the relative width first and then the relative height.
+            This setting is not used if `full_height=True`.
+        hint: A hint text.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         content: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         *,
         full_height: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]] = None,
@@ -267,22 +267,22 @@
     full_height: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]
     max_width: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, float]]
     min_width: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, float]]
     ratio: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, float]]]]
 
 
 class DividerViewV1(BaseViewV1):
-    """Horizontal delimiter.
+    """A horizontal delimiter.
 
-    You can place extra elements in the center of the delimiter, like a popup hint and label.
+    For more information, see [view.divider](https://toloka.ai/docs/template-builder/reference/view.divider).
 
     Attributes:
-        hint: Hint text.
-        label: A label in the center of the delimiter. Line breaks are not supported.
-        validation: Validation based on condition.
+        hint: A hint text.
+        label: A label in the center of the delimiter. Note, that line breaks are not supported.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         *,
         hint: typing.Optional[typing.Any] = None,
         label: typing.Optional[typing.Any] = None,
@@ -297,22 +297,28 @@
     hint: typing.Optional[typing.Any]
     label: typing.Optional[typing.Any]
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
 
 
 class GroupViewV1(BaseViewV1):
-    """Groups components visually into framed blocks.
+    """A view with a frame.
+
+    For more information, see [view.group](https://toloka.ai/docs/template-builder/reference/view.group).
+
+        Attributes:
+            content: A content.
+            label: A header.
+            hint: A hint. To insert a line break in the hint, use `
+    `.
 
     Attributes:
-        content: Content of a group block.
-        hint: Explanation of the group heading. To insert a new line, use
-            .
-        label: Group heading.
-        validation: Validation based on condition.
+        hint: A hint text.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         content: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
         *,
         hint: typing.Optional[typing.Any] = None,
@@ -329,27 +335,29 @@
     label: typing.Optional[typing.Any]
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
     content: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
 
 
 class IframeViewV1(BaseViewV1):
-    """Displays the web page at the URL in an iframe window.
+    """A frame displaying a web page.
+
+    For more information, see [view.iframe](https://toloka.ai/docs/template-builder/reference/view.iframe).
 
     Attributes:
-        url: URL of the web page.
-        full_height: If true, the element takes up all the vertical free space. The element is set to a minimum height
-            of 400 pixels.
-        max_width: Maximum width of the element in pixels, must be greater than min_width.
-        min_width: Minimum width of the element in pixels. Takes priority over max_width.
-        ratio: An array of two numbers that sets the relative dimensions of the sides: width (first number) to
-            height (second number). Not valid if full_height=true.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        url: The URL of the web page.
+        full_height: If `True`, the component takes up all the vertical free space.
+            Note, that the minimum height required by the component is 400 pixels.
+        max_width: The maximum width of the component in pixels.
+        min_width: The minimum width of the component in pixels. It takes priority over the `max_width`.
+        ratio: A list with the aspect ratio of the component. Specify the relative width first and then the relative height.
+            This setting is not used if `full_height=True`.
+        hint: A hint text.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         url: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]] = None,
         *,
         full_height: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]] = None,
@@ -374,37 +382,46 @@
     full_height: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]
     max_width: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, float]]
     min_width: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, float]]
     ratio: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, float]]]]
 
 
 class ImageViewV1(BaseViewV1):
-    """Displays an image.
+    """A component for displaying an image.
+
+    For more information, see [view.image](https://toloka.ai/docs/template-builder/reference/view.image).
 
     Attributes:
-        url: Image link.
-        full_height: If true, the element takes up all the vertical free space. The element is set to a minimum height
-            of 400 pixels.
-        max_width: Maximum width of the element in pixels, must be greater than min_width.
-        min_width: Minimum width of the element in pixels. Takes priority over max_width.
-        no_border: Controls the display of a frame around an image. By default, true (the frame is hidden). Set false
-            to display the frame.
-        no_lazy_load: Disables lazy loading. If true, images start loading immediately, even if they aren't in the
-            viewport. Useful for icons. By default, false (lazy loading is enabled). In this mode, images start loading
-            only when a Toloker scrolls to them.
-        popup: Specifies whether opening a full-size image with a click is allowed. By default, it is true (allowed).
-        ratio: An array of two numbers that sets the relative dimensions of the sides: width (first number) to
-            height (second number). Not valid if full_height=true.
-        scrollable: When set to true, an image has scroll bars if it doesn't fit in the parent element.
-            If false, the image fits in the parent element and, when clicked, opens in its original size in the module
-            window.
-            Images in SVG format with no size specified always fit in their parent elements.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        url: The URL of the image.
+        full_height: If `True`, the component takes up all the vertical free space.
+            Note, that the minimum height required by the component is 400 pixels.
+        max_width: The maximum width of the component in pixels.
+        min_width: The minimum width of the component in pixels. It takes priority over the `max_width`.
+        no_border: Displaying borders around the image.
+            * `True` — The borders are hidden.
+            * `False` — The borders are visible.
+
+            Default value: `True`.
+        no_lazy_load: Loading mode:
+            * `False` — The component starts loading the image when the component becomes visible to a Toloker.
+            * `True` — The image is loaded immediately. This mode is useful for icons.
+
+            Default value: `False` — lazy loading is enabled.
+        popup: If `True`, a Toloker can open a full sized image in a popup. It is a default behavior.
+        ratio: A list with the aspect ratio of the component. Specify the relative width first and then the relative height.
+            This setting is not used if `full_height=True`.
+        rotatable: If `True`, an image can be rotated.
+        scrollable: The way of displaying an image which is larger than the component:
+            * `True` — Scroll bars are shown.
+            * `False` — The image is scaled to fit the component.
+
+            Note, that images in SVG format with no size specified always fit the component.
+        hint: A hint text.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         url: typing.Optional[typing.Any] = None,
         *,
         full_height: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]] = None,
@@ -439,37 +456,40 @@
     popup: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]
     ratio: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, float]]]]
     rotatable: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]
     scrollable: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]
 
 
 class LabeledListViewV1(BaseViewV1):
-    """Displaying components as a list with labels placed on the left.
+    """A list of components with labels placed on the left.
 
-    If you don't need labels, use view.list.
+    For more information, see [view.labeled-list](https://toloka.ai/docs/template-builder/reference/view.labeled-list).
 
     Attributes:
         items: List items.
-        min_width: The minimum width of list content. If the component width is less than the specified value, it
-            switches to compact mode.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        min_width: The minimum width of the component.
+            If the width is less than the specified value, the list is displayed in compact mode.
+            Labels are placed above the items in this mode.
+        hint: A hint text.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     class Item(toloka.client.project.template_builder.base.BaseTemplate):
-        """Item.
+        """A labeled list item.
 
         Attributes:
-            content: List item content.
-            label: A label displayed next to a list item.
-            center_label: If true, a label is center-aligned relative to the content of a list item (content). Use it
-                if the list consists of large items, such as images or multi-line text.
-                By default, false (the label is aligned to the top of the content block).
-            hint: A pop-up hint displayed next to a label.
+            content: The content of the item.
+            label: An item label.
+            center_label: Label vertical alignment.
+                * `True` — The label is centered.
+                * `False` — The label is aligned to the top of the item content.
+
+                Default value: `False`.
+            hint: A hint.
         """
 
         def __init__(
             self,
             content: typing.Optional[toloka.client.project.template_builder.base.BaseComponent] = None,
             label: typing.Optional[typing.Any] = None,
             *,
@@ -506,30 +526,24 @@
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
     items: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, Item]]]]
     min_width: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, float]]
 
 
 class LinkViewV1(BaseViewV1):
-    """Universal way to add a link.
-
-    This link changes color when clicked.
-
-    We recommend using this component if you need to insert a link without additional formatting.
-
-    If you want to insert a button that will open the link, use the view.action-button and action.open-link components.
+    """A component showing a link.
 
-    To insert a link with a search query, use helper.search-query.
+    For more information, see [view.link](https://toloka.ai/docs/template-builder/reference/view.link).
 
     Attributes:
-        url: Link URL.
-        content: Link text displayed to the Toloker.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        url: A URL.
+        content: A link text.
+        hint: A hint text.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         url: typing.Optional[typing.Any] = None,
         *,
         content: typing.Optional[typing.Any] = None,
@@ -548,28 +562,25 @@
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
     url: typing.Optional[typing.Any]
     content: typing.Optional[typing.Any]
 
 
 class LinkGroupViewV1(BaseViewV1):
-    """Puts links into groups
+    """A group of links.
 
-    The most important link in a group can be highlighted with a border: set the theme property to primary for this link.
-    This only groups links, unlike GroupViewV1.
+    For more information, see [view.link-group](https://toloka.ai/docs/template-builder/reference/view.link-group).
 
     Attributes:
-        links: Array of links that make up a group.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        links: A list of links.
+        hint: A hint text.
+        label: A label above the component.
+        validation: Validation rules.
 
     Examples:
-        How to add several links.
-
         >>> links = tb.view.LinkGroupViewV1(
         >>>     [
         >>>         tb.view.LinkGroupViewV1.Link(
         >>>             'https://any.com/useful/url/1',
         >>>             'Example1',
         >>>         ),
         >>>         tb.view.LinkGroupViewV1.Link(
@@ -578,20 +589,22 @@
         >>>         ),
         >>>     ]
         >>> )
         ...
     """
 
     class Link(toloka.client.project.template_builder.base.BaseTemplate):
-        """Link parameters
+        """A link for the `LinkGroupViewV1`.
 
         Attributes:
-            url: Link address
-            content: Link text that's displayed to a Toloker. Unvisited links are blue and underlined, and visited links are purple.
-            theme: Defines the appearance of the link. If you specify "theme": "primary", it's a button, otherwise it's a text link.
+            url: A URL.
+            content: A link text.
+            theme: The appearance of the link.
+                If `theme` is omitted, the link is displayed as an underlined text.
+                If `theme` is set to `primary`, a button is displayed.
         """
 
         def __init__(
             self,
             url: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]] = None,
             content: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]] = None,
             *,
@@ -624,24 +637,31 @@
     label: typing.Optional[typing.Any]
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
     links: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, Link]]]]
 
 
 class ListViewV1(BaseViewV1):
-    """Block for displaying data in a list.
+    """A list of components.
+
+    For more information, see [view.list](https://toloka.ai/docs/template-builder/reference/view.list).
 
     Attributes:
-        items:  Array of list items.
-        direction: Determines the direction of the list.
-        size: Specifies the size of the margins between elements. Acceptable values in ascending order: s, m (default
-            value).
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        items: List items.
+        direction: The direction of the list:
+            * `vertical`
+            * `horizontal`
+
+            Default value: `vertical`.
+        size: A spacing between list items:
+            `m` — The default spacing.
+            `s` — Narrower spacing.
+        hint: A hint text.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         items: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[toloka.client.project.template_builder.base.BaseComponent]]] = None,
         *,
         direction: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, toloka.client.project.template_builder.base.ListDirection]] = None,
@@ -662,40 +682,37 @@
     version: typing.Optional[str]
     items: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[toloka.client.project.template_builder.base.BaseComponent]]]
     direction: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, toloka.client.project.template_builder.base.ListDirection]]
     size: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, toloka.client.project.template_builder.base.ListSize]]
 
 
 class MarkdownViewV1(BaseViewV1):
-    """Block for displaying text in Markdown.
+    """A component for formatting Markdown.
 
-    The contents of the block are written to the content property in a single line. To insert line breaks, use \n
-        Straight quotation marks (") must be escaped like this: \".
+    The Markdown content must not contain line breaks. To insert them, place `
+    ` in the text.
+        Straight quotation marks must be escaped: `"`.
 
-        Note that the view.markdown component is resource-intensive and might overload weak devices.
-        Do not use this component to display plain text. If you need to display text without formatting, use the view.text
-        component. If you need to insert a link, use view.link, and for an image use view.image.
-        Links with Markdown are appended with target="_blank" (the link opens in a new tab), as well as
-        rel="noopener noreferrer"
+        For more information, see [view.markdown](https://toloka.ai/docs/template-builder/reference/view.markdown).
 
         Attributes:
-            content: Text in Markdown.
+            content: A text with Markdown.
 
         Example:
-            How to add a title and description on the task interface.
+            Adding a title and description using Markdown.
 
             >>> header = tb.view.MarkdownViewV1('# Some Header:
     ---
     Some detailed description')
             ...
 
     Attributes:
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        hint: A hint text.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         content: typing.Optional[typing.Any] = None,
         *,
         hint: typing.Optional[typing.Any] = None,
@@ -712,29 +729,30 @@
     label: typing.Optional[typing.Any]
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
     content: typing.Optional[typing.Any]
 
 
 class TextViewV1(BaseViewV1):
-    """Block for displaying text.
+    """A view for displaying a text.
 
-    If you need formatted text, use view.markdown.
+    For more information, see [view.text](https://toloka.ai/docs/template-builder/reference/view.text).
 
-    Attributes:
-        content: The text displayed in the block. To insert a new line, use 
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        Attributes:
+            content: The text. To insert a new line, use `
+    `.
 
-    Examples:
-        How to show labeled field from the task inputs.
+        Example:
+            >>> text_view = tb.view.TextViewV1(tb.data.InputData('input_field_name'), label='My label:')
+            ...
 
-        >>> text_view = tb.view.TextViewV1(tb.data.InputData('input_field_name'), label='My label:')
-        ...
+    Attributes:
+        hint: A hint text.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         content: typing.Optional[typing.Any] = None,
         *,
         hint: typing.Optional[typing.Any] = None,
@@ -751,33 +769,28 @@
     label: typing.Optional[typing.Any]
     validation: typing.Optional[toloka.client.project.template_builder.base.BaseComponent]
     version: typing.Optional[str]
     content: typing.Optional[typing.Any]
 
 
 class VideoViewV1(BaseViewV1):
-    """Player for video playback.
-
-    The player is a rectangular block with a frame and buttons to control the video. You can set the block size using
-    the ratio, fullHeight, minWidth, and maxWidth properties.
+    """A video player.
 
-    The video resolution does not affect the size of the block — the video will fit into the block and will not be
-    cropped.
+    For more information, see [view.video](https://toloka.ai/docs/template-builder/reference/view.video).
 
     Attributes:
-        url: Link to the video file.
-        full_height: If true, the element takes up all the vertical free space. The element is set to a minimum height
-            of 400 pixels.
-        max_width: Maximum width of the element in pixels, must be greater than min_width.
-        min_width: Minimum width of the element in pixels. Takes priority over max_width.
-        ratio: The aspect ratio of the video block. An array of two numbers: the first sets the width of the block and
-            the second sets the height.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        url: The video URL.
+        full_height: If `True`, the component takes up all the vertical free space.
+            Note, that the minimum height required by the component is 400 pixels.
+        max_width: The maximum width of the component in pixels.
+        min_width: The minimum width of the component in pixels. It takes priority over the `max_width`.
+        ratio: A list with the aspect ratio of the component. Specify the relative width first and then the relative height.
+        hint: A hint text.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     def __init__(
         self,
         url: typing.Optional[typing.Any] = None,
         *,
         full_height: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]] = None,
@@ -802,43 +815,39 @@
     full_height: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, bool]]
     max_width: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, float]]
     min_width: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, float]]
     ratio: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, float]]]]
 
 
 class MapViewV1(BaseViewV1):
-    """Adds a map to your task.
-
-    Use this component to set the targets for the tasks with the markers, select the areas with polygons.
-    Specify the position and colors for the elements on the map.
+    """A component for displaying a map.
 
-    You can set the following map properties: scale, position of the map center, label, and hint for Tolokers.
+    For more information, see [view.map](https://toloka.ai/docs/template-builder/reference/view.map).
 
     Attributes:
-        center: Determines the position of the map center. Specify the coordinates in the string format, for example,
-            "29.748713,-95.404287", or use the data.location component to set the center of the map to the
-            Toloker's current position.
-        markers: Specifies the markers present on the map.
-        polygons: Specifies the polygonal objects that you can use to select areas on the map.
-        zoom: The map initial scale. Use the values from 0 to 19. Bigger values give a more detailed map view.
-        hint: Hint text.
-        label: Label above the component.
-        validation: Validation based on condition.
+        center: The coordinates of the map center. You can use:
+            * A string. For example, `29.748713,-95.404287`
+            * The [LocationData](toloka.client.project.template_builder.data.LocationData.md) to set Toloker's current position.
+        markers: A list of map markers.
+        polygons: A list of areas highlighted on the map.
+        zoom: An initial map scale. Use values from 0 to 19. Higher values zoom in the map.
+        hint: A hint text.
+        label: A label above the component.
+        validation: Validation rules.
     """
 
     class Marker(toloka.client.project.template_builder.base.BaseTemplate):
-        """Marker parameters.
+        """A map marker.
 
         Attributes:
-            position: Determines the marker position. Specify the coordinates in the string format, for example,
-                "29.748713,-95.404287", or use the data.location component to set the marker to the Toloker's current
-                position.
-            color: Determines the marker color. Use the hexadecimal values preceded by the # sign to specify the color.
-            label: The label for the marker that tells Tolokers what this marker is for and helps distinguish it
-                from other markers.
+            position: The coordinates of the marker. You can use:
+                * A string. For example, `29.748713,-95.404287`.
+                * The [LocationData](toloka.client.project.template_builder.data.LocationData.md) to set Toloker's current position.
+            color: The marker color. Use the hexadecimal values preceded by the `#`. For example, `#f00` makes the marker red.
+            label: A marker label.
         """
 
         def __init__(
             self,
             position: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]] = None,
             *,
             color: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]] = None,
@@ -850,21 +859,20 @@
 
         _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
         position: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]]
         color: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]]
         label: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]]
 
     class Polygon(toloka.client.project.template_builder.base.BaseTemplate):
-        """Polygon parameters.
+        """A map polygon.
 
         Attributes:
-            points: The list of the polygonal selection area points.
-                Specify the coordinates in the string format, for example, "29.748713,-95.404287".
-            color: Determines the polygonal selection area color. Use the hexadecimal values preceded by the # sign to
-                specify the color.
+            points: A list of polygon coordinates.
+                Specify the coordinates in the string format, for example `29.748713,-95.404287`.
+            color: The color of the polygon. Use the hexadecimal values preceded by the `#`. For example, `#f00` makes the polygon red.
         """
 
         def __init__(
             self,
             points: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, typing.List[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]]]] = None,
             *,
             color: typing.Optional[typing.Union[toloka.client.project.template_builder.base.BaseComponent, str]] = None
```

### Comparing `toloka-kit-1.1.4/src/client/project/view_spec.py` & `toloka-kit-1.2.0/src/client/project/view_spec.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/project/view_spec.pyi` & `toloka-kit-1.2.0/src/client/project/view_spec.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/quality_control.py` & `toloka-kit-1.2.0/src/client/quality_control.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/quality_control.pyi` & `toloka-kit-1.2.0/src/client/quality_control.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/requester.py` & `toloka-kit-1.2.0/src/client/requester.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/requester.pyi` & `toloka-kit-1.2.0/src/client/requester.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/search_requests.py` & `toloka-kit-1.2.0/src/client/search_requests.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/search_requests.pyi` & `toloka-kit-1.2.0/src/client/search_requests.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/search_results.py` & `toloka-kit-1.2.0/src/client/search_results.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/search_results.pyi` & `toloka-kit-1.2.0/src/client/search_results.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/skill.py` & `toloka-kit-1.2.0/src/client/skill.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/skill.pyi` & `toloka-kit-1.2.0/src/client/skill.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/solution.py` & `toloka-kit-1.2.0/src/client/solution.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/solution.pyi` & `toloka-kit-1.2.0/src/client/solution.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/task.py` & `toloka-kit-1.2.0/src/client/task.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 __all__ = [
     'BaseTask',
     'Task',
     'CreateTaskParameters',
-    'CreateTaskAsyncParameters',
     'CreateTasksParameters',
     'TaskOverlapPatch',
     'TaskPatch'
 ]
 import datetime
-import uuid
 from typing import Any, Dict, List
-from uuid import UUID
 
 from .primitives.base import BaseTolokaObject
 from .primitives.infinite_overlap import InfiniteOverlapParametersMixin
-from .primitives.parameter import Parameters
+from .primitives.parameter import IdempotentOperationParameters
 from ..util._codegen import attribute
 from ..util._docstrings import inherit_docstrings
 
 
 class BaseTask(BaseTolokaObject):
     """A base class for tasks.
 
@@ -100,67 +97,54 @@
     traits_any_of: List[str]
     traits_none_of_any: List[str]
     origin_task_id: str = attribute(readonly=True)
     created: datetime.datetime = attribute(readonly=True)
     baseline_solutions: List[BaselineSolution]
 
 
-class CreateTaskParameters(Parameters):
+@inherit_docstrings
+class CreateTaskParameters(IdempotentOperationParameters):
     """Parameters used with the [create_task](toloka.client.TolokaClient.create_task.md) method.
 
+    If the operation is started in an asynchronous mode,
+    we recommend that you send the `operation_id` to avoid creating the same tasks multiple times. You can use this ID later to get information about the operation.
+
     Attributes:
         allow_defaults: Active overlap setting:
             * `True` — Use the overlap that is set in the `defaults.default_overlap_for_new_tasks` pool parameter.
             * `False` — Use the overlap that is set in the `overlap` task parameter.
 
             Default value: `False`.
         open_pool: Open the pool immediately after creating a task suite, if the pool is closed.
             Default value: `False`.
+        async_mode: Request processing mode:
+            * `True` — Asynchronous operation is started internally and `create_tasks` waits for the completion of it. It is recommended to create no more than 10,000 tasks per request in this mode.
+            * `False` — The request is processed synchronously. A maximum of 5000 tasks can be added in a single request in this mode.
+            Default value: `True`.
     """
-
     allow_defaults: bool
     open_pool: bool
-    operation_id: UUID = attribute(factory=uuid.uuid4)
-
-
-@inherit_docstrings
-class CreateTaskAsyncParameters(CreateTaskParameters):
-    """Parameters used with the [create_tasks_async](toloka.client.TolokaClient.create_tasks_async.md) method.
-
-    Send the `operation_id` to avoid creating the same tasks multiple times. You can use this ID later to get information about the operation.
-
-    Attributes:
-        operation_id: The ID of the operation conforming to the [RFC4122 standard](https://tools.ietf.org/html/rfc4122).
-    """
-    pass
 
 
 @inherit_docstrings
 class CreateTasksParameters(CreateTaskParameters):
-    """Parameters used with the [create_tasks](toloka.client.TolokaClient.create_tasks.md) method.
+    """Parameters used with the [create_tasks](toloka.client.TolokaClient.create_tasks.md)
+    and [create_tasks_async](toloka.client.TolokaClient.create_tasks_async.md) methods.
 
     If the operation is started in an asynchronous mode,
     we recommend that you send the `operation_id` to avoid creating the same tasks multiple times. You can use this ID later to get information about the operation.
 
     Attributes:
         skip_invalid_items: Task validation option:
             * `True` — All valid tasks are added. If a task does not pass validation, then it is not added to Toloka. All such tasks are listed in the response.
             * `False` — If any task does not pass validation, then the operation is cancelled and no tasks are added to Toloka.
 
             Default value: `False`.
-        operation_id: The ID of the operation conforming to the [RFC4122 standard](https://tools.ietf.org/html/rfc4122). Use it if the `async_mode` is set to `True`.
-        async_mode: Request processing mode:
-            * `True` — Asynchronous operation is started internally and `create_tasks` waits for the completion of it. It is recommended to create no more than 10,000 tasks per request in this mode.
-            * `False` — The request is processed synchronously. A maximum of 5000 tasks can be added in a single request in this mode.
-
-            Default value: `False`.
     """
-
     skip_invalid_items: bool
-    async_mode: bool = attribute(default=True)
 
 
 class TaskOverlapPatch(BaseTolokaObject):
     """Parameters for changing the overlap of a task.
 
     Attributes:
         overlap: The new overlap value.
```

### Comparing `toloka-kit-1.1.4/src/client/task.pyi` & `toloka-kit-1.2.0/src/client/task.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 __all__ = [
     'BaseTask',
     'Task',
     'CreateTaskParameters',
-    'CreateTaskAsyncParameters',
     'CreateTasksParameters',
     'TaskOverlapPatch',
     'TaskPatch',
 ]
 import datetime
 import toloka.client.primitives.base
 import toloka.client.primitives.infinite_overlap
@@ -165,123 +164,101 @@
     traits_all_of: typing.Optional[typing.List[str]]
     traits_any_of: typing.Optional[typing.List[str]]
     traits_none_of_any: typing.Optional[typing.List[str]]
     created: typing.Optional[datetime.datetime]
     baseline_solutions: typing.Optional[typing.List[BaselineSolution]]
 
 
-class CreateTaskParameters(toloka.client.primitives.parameter.Parameters):
+class CreateTaskParameters(toloka.client.primitives.parameter.IdempotentOperationParameters):
     """Parameters used with the [create_task](toloka.client.TolokaClient.create_task.md) method.
 
+    If the operation is started in an asynchronous mode,
+    we recommend that you send the `operation_id` to avoid creating the same tasks multiple times. You can use this ID later to get information about the operation.
+
     Attributes:
+        operation_id: The ID of the operation conforming to the [RFC4122 standard](https://tools.ietf.org/html/rfc4122).
+        async_mode: Request processing mode:
+            * `True` — Asynchronous operation is started internally and `create_tasks` waits for the completion of it. It is recommended to create no more than 10,000 tasks per request in this mode.
+            * `False` — The request is processed synchronously. A maximum of 5000 tasks can be added in a single request in this mode.
+            Default value: `True`.
         allow_defaults: Active overlap setting:
             * `True` — Use the overlap that is set in the `defaults.default_overlap_for_new_tasks` pool parameter.
             * `False` — Use the overlap that is set in the `overlap` task parameter.
 
             Default value: `False`.
         open_pool: Open the pool immediately after creating a task suite, if the pool is closed.
             Default value: `False`.
     """
 
     def __init__(
         self,
         *,
+        operation_id: typing.Optional[uuid.UUID] = ...,
+        async_mode: typing.Optional[bool] = True,
         allow_defaults: typing.Optional[bool] = None,
-        open_pool: typing.Optional[bool] = None,
-        operation_id: typing.Optional[uuid.UUID] = ...
+        open_pool: typing.Optional[bool] = None
     ) -> None:
         """Method generated by attrs for class CreateTaskParameters.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
-    allow_defaults: typing.Optional[bool]
-    open_pool: typing.Optional[bool]
     operation_id: typing.Optional[uuid.UUID]
-
-
-class CreateTaskAsyncParameters(CreateTaskParameters):
-    """Parameters used with the [create_tasks_async](toloka.client.TolokaClient.create_tasks_async.md) method.
-
-    Send the `operation_id` to avoid creating the same tasks multiple times. You can use this ID later to get information about the operation.
-
-    Attributes:
-        allow_defaults: Active overlap setting:
-            * `True` — Use the overlap that is set in the `defaults.default_overlap_for_new_tasks` pool parameter.
-            * `False` — Use the overlap that is set in the `overlap` task parameter.
-
-            Default value: `False`.
-        open_pool: Open the pool immediately after creating a task suite, if the pool is closed.
-            Default value: `False`.
-        operation_id: The ID of the operation conforming to the [RFC4122 standard](https://tools.ietf.org/html/rfc4122).
-    """
-
-    def __init__(
-        self,
-        *,
-        allow_defaults: typing.Optional[bool] = None,
-        open_pool: typing.Optional[bool] = None,
-        operation_id: typing.Optional[uuid.UUID] = ...
-    ) -> None:
-        """Method generated by attrs for class CreateTaskAsyncParameters.
-        """
-        ...
-
-    _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
+    async_mode: typing.Optional[bool]
     allow_defaults: typing.Optional[bool]
     open_pool: typing.Optional[bool]
-    operation_id: typing.Optional[uuid.UUID]
 
 
 class CreateTasksParameters(CreateTaskParameters):
-    """Parameters used with the [create_tasks](toloka.client.TolokaClient.create_tasks.md) method.
+    """Parameters used with the [create_tasks](toloka.client.TolokaClient.create_tasks.md)
+
+    and [create_tasks_async](toloka.client.TolokaClient.create_tasks_async.md) methods.
 
     If the operation is started in an asynchronous mode,
     we recommend that you send the `operation_id` to avoid creating the same tasks multiple times. You can use this ID later to get information about the operation.
 
     Attributes:
+        operation_id: The ID of the operation conforming to the [RFC4122 standard](https://tools.ietf.org/html/rfc4122).
+        async_mode: Request processing mode:
+            * `True` — Asynchronous operation is started internally and `create_tasks` waits for the completion of it. It is recommended to create no more than 10,000 tasks per request in this mode.
+            * `False` — The request is processed synchronously. A maximum of 5000 tasks can be added in a single request in this mode.
+            Default value: `True`.
         allow_defaults: Active overlap setting:
             * `True` — Use the overlap that is set in the `defaults.default_overlap_for_new_tasks` pool parameter.
             * `False` — Use the overlap that is set in the `overlap` task parameter.
 
             Default value: `False`.
         open_pool: Open the pool immediately after creating a task suite, if the pool is closed.
             Default value: `False`.
-        operation_id: The ID of the operation conforming to the [RFC4122 standard](https://tools.ietf.org/html/rfc4122). Use it if the `async_mode` is set to `True`.
         skip_invalid_items: Task validation option:
             * `True` — All valid tasks are added. If a task does not pass validation, then it is not added to Toloka. All such tasks are listed in the response.
             * `False` — If any task does not pass validation, then the operation is cancelled and no tasks are added to Toloka.
 
             Default value: `False`.
-        async_mode: Request processing mode:
-            * `True` — Asynchronous operation is started internally and `create_tasks` waits for the completion of it. It is recommended to create no more than 10,000 tasks per request in this mode.
-            * `False` — The request is processed synchronously. A maximum of 5000 tasks can be added in a single request in this mode.
-
-            Default value: `False`.
     """
 
     def __init__(
         self,
         *,
+        operation_id: typing.Optional[uuid.UUID] = ...,
+        async_mode: typing.Optional[bool] = True,
         allow_defaults: typing.Optional[bool] = None,
         open_pool: typing.Optional[bool] = None,
-        operation_id: typing.Optional[uuid.UUID] = ...,
-        skip_invalid_items: typing.Optional[bool] = None,
-        async_mode: typing.Optional[bool] = True
+        skip_invalid_items: typing.Optional[bool] = None
     ) -> None:
         """Method generated by attrs for class CreateTasksParameters.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
+    operation_id: typing.Optional[uuid.UUID]
+    async_mode: typing.Optional[bool]
     allow_defaults: typing.Optional[bool]
     open_pool: typing.Optional[bool]
-    operation_id: typing.Optional[uuid.UUID]
     skip_invalid_items: typing.Optional[bool]
-    async_mode: typing.Optional[bool]
 
 
 class TaskOverlapPatch(toloka.client.primitives.base.BaseTolokaObject):
     """Parameters for changing the overlap of a task.
 
     Attributes:
         overlap: The new overlap value.
```

### Comparing `toloka-kit-1.1.4/src/client/task_distribution_function.py` & `toloka-kit-1.2.0/src/client/task_distribution_function.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/task_distribution_function.pyi` & `toloka-kit-1.2.0/src/client/task_distribution_function.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/task_suite.py` & `toloka-kit-1.2.0/src/client/task_suite.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 __all__ = [
     'TaskSuite',
     'TaskSuiteCreateRequestParameters',
+    'TaskSuitesCreateRequestParameters',
     'TaskSuiteOverlapPatch',
     'TaskSuitePatch'
 ]
 import datetime
-import uuid
 from typing import List
-from uuid import UUID
 
 import attr
 
 from .primitives.base import BaseTolokaObject
 from .primitives.infinite_overlap import InfiniteOverlapParametersMixin
-from .primitives.parameter import Parameters
+from .primitives.parameter import IdempotentOperationParameters
 from .task import BaseTask
 from ..util._codegen import attribute, expand
+from ..util._docstrings import inherit_docstrings
 
 
 class TaskSuite(InfiniteOverlapParametersMixin, BaseTolokaObject):
     """A set of tasks assigned to a Toloker at once.
 
     A task suite contains one or more tasks. Tolokers are paid after completing all tasks in a task suite.
 
@@ -72,42 +72,46 @@
 
     @expand('base_task')
     def add_base_task(self, base_task: BaseTask) -> 'TaskSuite':
         self.tasks.append(base_task)
         return self
 
 
-class TaskSuiteCreateRequestParameters(Parameters):
-    """Parameters for creating task suites.
+@inherit_docstrings
+class TaskSuiteCreateRequestParameters(IdempotentOperationParameters):
+    """Parameters for creating task suite.
 
     Attributes:
-        operation_id: The ID of the operation conforming to the [RFC4122 standard](https://tools.ietf.org/html/rfc4122). Use it if the `async_mode` is set to `True`.
-        skip_invalid_items: Task suite validation option:
-            * `True` — All valid task suites are added. If a task suite does not pass validation, then it is not added to Toloka.
-            * `False` — If any task suite does not pass validation, then operation is cancelled and no task suites are added to Toloka.
-
-            Default value: `False`.
         allow_defaults: Active overlap setting:
             * `True` — Use the overlap that is set in the `defaults.default_overlap_for_new_task_suites` pool parameter.
             * `False` — Use the overlap that is set in the `overlap` task suite parameter.
 
             Default value: `False`.
         open_pool: Open the pool immediately after creating a task suite, if the pool is closed.
+    """
+    allow_defaults: bool
+    open_pool: bool
+
+
+@inherit_docstrings
+class TaskSuitesCreateRequestParameters(TaskSuiteCreateRequestParameters):
+    """Parameters for creating task suites.
+
+    Attributes:
+        skip_invalid_items: Task suite validation option:
+            * `True` — All valid task suites are added. If a task suite does not pass validation, then it is not added to Toloka.
+            * `False` — If any task suite does not pass validation, then operation is cancelled and no task suites are added to Toloka.
+
+            Default value: `False`.
         async_mode: Request processing mode:
             * `True` — Asynchronous operation is started internally.
             * `False` — The request is processed synchronously. A maximum of 5000 task suites can be added in a single request in this mode.
-
             Default value: `True`.
     """
-
-    operation_id: UUID = attribute(factory=uuid.uuid4)
     skip_invalid_items: bool
-    allow_defaults: bool
-    open_pool: bool
-    async_mode: bool = attribute(default=True)
 
 
 class TaskSuiteOverlapPatch(BaseTolokaObject):
     """Parameters for stopping assigning a task suite.
 
     Attributes:
         overlap: The new overlap value.
```

### Comparing `toloka-kit-1.1.4/src/client/training.py` & `toloka-kit-1.2.0/src/client/training.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/training.pyi` & `toloka-kit-1.2.0/src/client/training.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/user.py` & `toloka-kit-1.2.0/src/client/user.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/user.pyi` & `toloka-kit-1.2.0/src/client/user.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/user_bonus.py` & `toloka-kit-1.2.0/src/client/user_bonus.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 __all__ = [
     'UserBonus',
-    'UserBonusCreateRequestParameters'
+    'UserBonusCreateRequestParameters',
+    'UserBonusesCreateRequestParameters',
 ]
 
-import uuid
-
 from attr.validators import optional, instance_of
 import datetime
 from decimal import Decimal
 from typing import Dict
 
 from .primitives.base import BaseTolokaObject
-from .primitives.parameter import Parameters
+from .primitives.parameter import IdempotentOperationParameters
 from ..util._codegen import attribute
+from ..util._docstrings import inherit_docstrings
 
 
 class UserBonus(BaseTolokaObject):
     """Issuing a bonus to a specific Toloker.
 
     It's addition to payment for completed tasks.
 
@@ -83,25 +83,29 @@
     assignment_id: str
 
     # Readonly
     id: str = attribute(readonly=True)
     created: datetime.datetime = attribute(readonly=True)
 
 
-class UserBonusCreateRequestParameters(Parameters):
+@inherit_docstrings
+class UserBonusCreateRequestParameters(IdempotentOperationParameters):
+    """Parameters for creating bonus for Toloker.
+
+    Used in methods 'create_user_bonus' of the class TolokaClient.
+    """
+    ...
+
+
+@inherit_docstrings
+class UserBonusesCreateRequestParameters(UserBonusCreateRequestParameters):
     """Parameters for creating bonuses for Tolokers.
 
-    Used in methods 'create_user_bonus', 'create_user_bonuses' и 'create_user_bonuses_async' of the class TolokaClient,
+    Used in methods 'create_user_bonuses' и 'create_user_bonuses_async' of the class TolokaClient,
     to clarify the behavior when creating bonuses.
 
     Attributes:
-        operation_id: Operation ID. If asynchronous creation is used, by this identifier you can later get
-            results of creating bonuses.
         skip_invalid_items: Validation parameters of objects:
             * `True` — Award a bonus if the object with bonus information passed validation. Otherwise, skip the bonus.
             * `False` — Default behavior. Stop the operation and don't award bonuses if at least one object didn't pass validation.
     """
-
-    operation_id: uuid.UUID = attribute(factory=uuid.uuid4)
     skip_invalid_items: bool
-
-    async_mode: bool = attribute(init=False)
```

### Comparing `toloka-kit-1.1.4/src/client/user_bonus.pyi` & `toloka-kit-1.2.0/src/client/user_bonus.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 __all__ = [
     'UserBonus',
     'UserBonusCreateRequestParameters',
+    'UserBonusesCreateRequestParameters',
 ]
 import datetime
 import decimal
 import toloka.client.primitives.base
 import toloka.client.primitives.parameter
 import typing
 import uuid
@@ -93,35 +94,69 @@
     public_message: typing.Optional[typing.Dict[str, str]]
     without_message: typing.Optional[bool]
     assignment_id: typing.Optional[str]
     id: typing.Optional[str]
     created: typing.Optional[datetime.datetime]
 
 
-class UserBonusCreateRequestParameters(toloka.client.primitives.parameter.Parameters):
+class UserBonusCreateRequestParameters(toloka.client.primitives.parameter.IdempotentOperationParameters):
+    """Parameters for creating bonus for Toloker.
+
+    Used in methods 'create_user_bonus' of the class TolokaClient.
+
+    Attributes:
+        operation_id: The ID of the operation conforming to the [RFC4122 standard](https://tools.ietf.org/html/rfc4122).
+        async_mode: Request processing mode:
+            * `True` — Asynchronous operation is started internally.
+            * `False` — The request is processed synchronously.
+
+            Default value: `True`.
+    """
+
+    def __init__(
+        self,
+        *,
+        operation_id: typing.Optional[uuid.UUID] = ...,
+        async_mode: typing.Optional[bool] = True
+    ) -> None:
+        """Method generated by attrs for class UserBonusCreateRequestParameters.
+        """
+        ...
+
+    _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
+    operation_id: typing.Optional[uuid.UUID]
+    async_mode: typing.Optional[bool]
+
+
+class UserBonusesCreateRequestParameters(UserBonusCreateRequestParameters):
     """Parameters for creating bonuses for Tolokers.
 
-    Used in methods 'create_user_bonus', 'create_user_bonuses' и 'create_user_bonuses_async' of the class TolokaClient,
+    Used in methods 'create_user_bonuses' и 'create_user_bonuses_async' of the class TolokaClient,
     to clarify the behavior when creating bonuses.
 
     Attributes:
-        operation_id: Operation ID. If asynchronous creation is used, by this identifier you can later get
-            results of creating bonuses.
+        operation_id: The ID of the operation conforming to the [RFC4122 standard](https://tools.ietf.org/html/rfc4122).
+        async_mode: Request processing mode:
+            * `True` — Asynchronous operation is started internally.
+            * `False` — The request is processed synchronously.
+
+            Default value: `True`.
         skip_invalid_items: Validation parameters of objects:
             * `True` — Award a bonus if the object with bonus information passed validation. Otherwise, skip the bonus.
             * `False` — Default behavior. Stop the operation and don't award bonuses if at least one object didn't pass validation.
     """
 
     def __init__(
         self,
         *,
         operation_id: typing.Optional[uuid.UUID] = ...,
+        async_mode: typing.Optional[bool] = True,
         skip_invalid_items: typing.Optional[bool] = None
     ) -> None:
-        """Method generated by attrs for class UserBonusCreateRequestParameters.
+        """Method generated by attrs for class UserBonusesCreateRequestParameters.
         """
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     operation_id: typing.Optional[uuid.UUID]
-    skip_invalid_items: typing.Optional[bool]
     async_mode: typing.Optional[bool]
+    skip_invalid_items: typing.Optional[bool]
```

### Comparing `toloka-kit-1.1.4/src/client/user_restriction.py` & `toloka-kit-1.2.0/src/client/user_restriction.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/user_restriction.pyi` & `toloka-kit-1.2.0/src/client/user_restriction.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/user_skill.py` & `toloka-kit-1.2.0/src/client/user_skill.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/user_skill.pyi` & `toloka-kit-1.2.0/src/client/user_skill.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/webhook_subscription.py` & `toloka-kit-1.2.0/src/client/webhook_subscription.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/client/webhook_subscription.pyi` & `toloka-kit-1.2.0/src/client/webhook_subscription.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/metrics/__init__.py` & `toloka-kit-1.2.0/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/metrics/__init__.pyi` & `toloka-kit-1.2.0/src/metrics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/metrics/collector.py` & `toloka-kit-1.2.0/src/metrics/collector.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/metrics/collector.pyi` & `toloka-kit-1.2.0/src/metrics/collector.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/metrics/jupyter_dashboard.py` & `toloka-kit-1.2.0/src/metrics/jupyter_dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 __all__ = [
     'DashBoard',
     'Chart',
 ]
 
 import plotly.graph_objects as go
 from jupyter_dash import JupyterDash
-import dash_core_components as dcc
-import dash_html_components as html
+from dash import dcc
+from dash import html
 from dash.dependencies import Input, Output
 
 import asyncio
 from collections import namedtuple
 import datetime
 import logging
 import math
```

### Comparing `toloka-kit-1.1.4/src/metrics/jupyter_dashboard.pyi` & `toloka-kit-1.2.0/src/metrics/jupyter_dashboard.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/metrics/metrics.py` & `toloka-kit-1.2.0/src/metrics/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from ..client import (
     Requester,
     TolokaClient,
 )
 from ..util._managing_headers import add_headers
 from ..util.async_utils import Cooldown
 from ..streaming import cursor
-from ..streaming.cursor import TolokaClientSyncOrAsyncType
+from ..streaming.cursor import TolokaClientSyncOrAsyncType, DEFAULT_LAG
 
 
 def bind_client(metrics: List['BaseMetric'], toloka_client: TolokaClientSyncOrAsyncType) -> None:
     """Sets/updates toloka_client for all metrics in list.
 
     Examples:
         How to bind same client for all metrics:
@@ -189,14 +189,16 @@
 
 
 @attr.s(auto_attribs=True)
 class NewUserBonuses(BaseMetric):
     """Tracking rewards for Tolokers: reward count or money amount.
 
     Args:
+        cursor_time_lag: Time lag for cursor. This controls time lag between user bonuses being added and this metric
+            being updated. See BaseCursor.time_lag for details and reasoning behind this.
         count_name: Metric name for a count of new bonuses.
         money_name: Metric name for amount of money in new bonuses.
         join_events: Count all events in one point.  Default `False`.
 
     Example:
         How to collect this metrics:
         >>> def print_metric(metric_dict):
@@ -208,14 +210,15 @@
 
         >>> {
         >>>     'bonus_count': [(datetime.datetime(2021, 11, 18, 8, 29, 9, 734373), 0)],
         >>>     'bonus_money': [(datetime.datetime(2021, 11, 18, 8, 29, 9, 734377), Decimal('0'))]
         >>> }
         ...
     """
+    _cursor_time_lag: datetime.timedelta = DEFAULT_LAG
     _count_name: Optional[str] = None
     _money_name: Optional[str] = None
 
     _join_events: bool = False
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
@@ -232,14 +235,15 @@
         return [name for name in (self._count_name, self._money_name) if name is not None]
 
     @cached_property
     def _cursor(self) -> cursor.UserBonusCursor:
         return cursor.UserBonusCursor(
             toloka_client=self.atoloka_client,
             created_gte=datetime.datetime.now(datetime.timezone.utc),
+            time_lag=self._cursor_time_lag,
         )
 
     async def _get_lines_impl(self) -> Dict[str, List[Tuple[Any, Any]]]:
         result = {}
 
         it = self._cursor
         event_list = [event async for event in it]
@@ -267,14 +271,16 @@
 
 @attr.s(auto_attribs=True)
 class NewUserSkills(BaseMetric):
     """Tracking Tolokers' skills.
 
     Args:
         skill_id: Which skill we will be tracking.
+        cursor_time_lag: Time lag for cursor. This controls time lag between user skills being updated and this metric
+            being updated. See BaseCursor.time_lag for details and reasoning behind this.
         count_name: Metric name for a count of new skill assignments. When skill changes it counts to.
         value_name: Metric name for exact values of new skill level for each skill assignment. It could be useful to track mean value or some medians.
         join_events: Count all events in one point.  Default `False`. "Values" never join.
 
     Example:
         How to collect this metrics:
         >>> def print_metric(metric_dict):
@@ -297,14 +303,15 @@
         >>> {
         >>>     'count': [(datetime.datetime(2021, 11, 18, 8, 31, 54, 11000), 1)],
         >>>     'values':  [(datetime.datetime(2021, 11, 18, 8, 31, 54, 11000), Decimal('50.000000000000'))],
         >>> }
         ...
     """
     _skill_id: str = attr.ib(kw_only=False)
+    _cursor_time_lag: datetime.timedelta = DEFAULT_LAG
     _count_name: Optional[str] = None
     _value_name: Optional[str] = None
 
     _join_events: bool = False
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
@@ -322,14 +329,15 @@
     @cached_property
     def _cursor(self) -> cursor.UserSkillCursor:
         return cursor.UserSkillCursor(
             toloka_client=self.atoloka_client,
             skill_id=self._skill_id,
             created_gte=datetime.datetime.now(datetime.timezone.utc),
             event_type='MODIFIED',
+            time_lag=self._cursor_time_lag,
         )
 
     async def _get_lines_impl(self) -> Dict[str, List[Tuple[Any, Any]]]:
         result = {}
 
         it = self._cursor
         event_list = [event async for event in it]
@@ -355,14 +363,16 @@
 class NewMessageThreads(BaseMetric):
     """Tracking the new messages
 
     Could count messages in projects or pools. If you want to track messages count in several projects/pools, don't get several
     NewMessageThreads instance. You can gather all in one instance.
 
     Args:
+        cursor_time_lag: Time lag for cursor. This controls time lag between message threads being created and this
+            metric being updated. See BaseCursor.time_lag for details and reasoning behind this.
         count_name: Metric name for a count of new messages.
         projects_name: Dictionary that allows count messages on exact projects. {project_id: line_name}
         pools_name: Dictionary that allows count messages on exact pools. {pool_id: line_name}
         join_events: Count all events in one point. Default `False`. "Values" never join.
 
     Example:
         How to collect this metrics:
@@ -394,14 +404,15 @@
         >>>     'my_working_pool': [(datetime.datetime(2021, 11, 19, 12, 42, 50, 554830), 0)],
         >>>     'pedestrian_proj': [(datetime.datetime(2021, 11, 19, 12, 42, 50, 554830), 1)],
         >>>     # total count != sum of other counts, because could exist different pools and projects
         >>>     'checking_proj': [(datetime.datetime(2021, 11, 19, 12, 42, 50, 554830), 1)],
         >>> }
         ...
     """
+    _cursor_time_lag: datetime.timedelta = DEFAULT_LAG
     _count_name: Optional[str] = None
     _projects_name: Dict[str, str] = {}  # {project_id: line_name}
     _pools_name: Dict[str, str] = {}  # {pool_id: line_name}
     _join_events: bool = False
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
@@ -424,14 +435,15 @@
         return line_names
 
     @cached_property
     def _cursor(self) -> cursor.MessageThreadCursor:
         return cursor.MessageThreadCursor(
             toloka_client=self.atoloka_client,
             created_gte=datetime.datetime.now(datetime.timezone.utc),
+            time_lag=self._cursor_time_lag,
         )
 
     async def _get_lines_impl(self) -> Dict[str, List[Tuple[Any, Any]]]:
         result = defaultdict(list)
 
         it = self._cursor
         event_list = [event async for event in it]
```

### Comparing `toloka-kit-1.1.4/src/metrics/metrics.pyi` & `toloka-kit-1.2.0/src/metrics/metrics.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -149,14 +149,16 @@
     balance_name: typing.Optional[str]
 
 
 class NewUserBonuses(BaseMetric):
     """Tracking rewards for Tolokers: reward count or money amount.
 
     Args:
+        cursor_time_lag: Time lag for cursor. This controls time lag between user bonuses being added and this metric
+            being updated. See BaseCursor.time_lag for details and reasoning behind this.
         count_name: Metric name for a count of new bonuses.
         money_name: Metric name for amount of money in new bonuses.
         join_events: Count all events in one point.  Default `False`.
 
     Example:
         How to collect this metrics:
         >>> def print_metric(metric_dict):
@@ -176,14 +178,15 @@
     def get_line_names(self) -> typing.List[str]:
         """Returns a list of metric names that can be generated by this class instance.
         """
         ...
 
     def __init__(
         self,
+        cursor_time_lag: datetime.timedelta = ...,
         count_name: typing.Optional[str] = None,
         money_name: typing.Optional[str] = None,
         join_events: bool = False,
         *,
         toloka_client: toloka.client.TolokaClient = None,
         atoloka_client: toloka.async_client.client.AsyncTolokaClient = None,
         timeout: datetime.timedelta = ...
@@ -191,24 +194,27 @@
         """Method generated by attrs for class NewUserBonuses.
         """
         ...
 
     toloka_client: toloka.client.TolokaClient
     atoloka_client: toloka.async_client.client.AsyncTolokaClient
     timeout: datetime.timedelta
+    _cursor_time_lag: datetime.timedelta
     _count_name: typing.Optional[str]
     _money_name: typing.Optional[str]
     _join_events: bool
 
 
 class NewUserSkills(BaseMetric):
     """Tracking Tolokers' skills.
 
     Args:
         skill_id: Which skill we will be tracking.
+        cursor_time_lag: Time lag for cursor. This controls time lag between user skills being updated and this metric
+            being updated. See BaseCursor.time_lag for details and reasoning behind this.
         count_name: Metric name for a count of new skill assignments. When skill changes it counts to.
         value_name: Metric name for exact values of new skill level for each skill assignment. It could be useful to track mean value or some medians.
         join_events: Count all events in one point.  Default `False`. "Values" never join.
 
     Example:
         How to collect this metrics:
         >>> def print_metric(metric_dict):
@@ -239,14 +245,15 @@
         """Returns a list of metric names that can be generated by this class instance.
         """
         ...
 
     def __init__(
         self,
         skill_id: str,
+        cursor_time_lag: datetime.timedelta = ...,
         count_name: typing.Optional[str] = None,
         value_name: typing.Optional[str] = None,
         join_events: bool = False,
         *,
         toloka_client: toloka.client.TolokaClient = None,
         atoloka_client: toloka.async_client.client.AsyncTolokaClient = None,
         timeout: datetime.timedelta = ...
@@ -255,26 +262,29 @@
         """
         ...
 
     toloka_client: toloka.client.TolokaClient
     atoloka_client: toloka.async_client.client.AsyncTolokaClient
     timeout: datetime.timedelta
     _skill_id: str
+    _cursor_time_lag: datetime.timedelta
     _count_name: typing.Optional[str]
     _value_name: typing.Optional[str]
     _join_events: bool
 
 
 class NewMessageThreads(BaseMetric):
     """Tracking the new messages
 
     Could count messages in projects or pools. If you want to track messages count in several projects/pools, don't get several
     NewMessageThreads instance. You can gather all in one instance.
 
     Args:
+        cursor_time_lag: Time lag for cursor. This controls time lag between message threads being created and this
+            metric being updated. See BaseCursor.time_lag for details and reasoning behind this.
         count_name: Metric name for a count of new messages.
         projects_name: Dictionary that allows count messages on exact projects. {project_id: line_name}
         pools_name: Dictionary that allows count messages on exact pools. {pool_id: line_name}
         join_events: Count all events in one point. Default `False`. "Values" never join.
 
     Example:
         How to collect this metrics:
@@ -314,14 +324,15 @@
     def get_line_names(self) -> typing.List[str]:
         """Returns a list of metric names that can be generated by this class instance.
         """
         ...
 
     def __init__(
         self,
+        cursor_time_lag: datetime.timedelta = ...,
         count_name: typing.Optional[str] = None,
         projects_name: typing.Dict[str, str] = ...,
         pools_name: typing.Dict[str, str] = ...,
         join_events: bool = False,
         *,
         toloka_client: toloka.client.TolokaClient = None,
         atoloka_client: toloka.async_client.client.AsyncTolokaClient = None,
@@ -330,11 +341,12 @@
         """Method generated by attrs for class NewMessageThreads.
         """
         ...
 
     toloka_client: toloka.client.TolokaClient
     atoloka_client: toloka.async_client.client.AsyncTolokaClient
     timeout: datetime.timedelta
+    _cursor_time_lag: datetime.timedelta
     _count_name: typing.Optional[str]
     _projects_name: typing.Dict[str, str]
     _pools_name: typing.Dict[str, str]
     _join_events: bool
```

### Comparing `toloka-kit-1.1.4/src/metrics/pool_metrics.py` & `toloka-kit-1.2.0/src/metrics/pool_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,16 @@
         created_name: Metric name for a count of created events. Default None.
         submitted_name: Metric name for a count of submitted events. Default 'submitted_events_in_pool'.
         accepted_name : Metric name for a count of accepted events. Default 'accepted_events_in_pool'.
         rejected_name : Metric name for a count of rejected events. Default 'rejected_events_in_pool'.
         skipped_name: Metric name for a count of skipped events. Default None.
         expired_name: Metric name for a count of expired events. Default None.
         join_events: Count all events in one point.  Default `False`.
+        cursor_time_lag: Time lag for cursor. This controls time lag between assignments being added and this metric
+            being updated. See BaseCursor.time_lag for details and reasoning behind this.
 
     Raises:
         ValueError: If all metric names are set to None or if there are duplicate metric names.
 
     Example:
         How to collect this metrics:
         >>> def print_metric(metric_dict):
@@ -94,14 +96,16 @@
     _created_name: Optional[str] = None
     _submitted_name: Optional[str] = None
     _accepted_name: Optional[str] = None
     _rejected_name: Optional[str] = None
     _skipped_name: Optional[str] = None
     _expired_name: Optional[str] = None
 
+    _cursor_time_lag: datetime.timedelta = cursor.DEFAULT_LAG
+
     _join_events: bool = False
 
     _status_dict = {
         '_created_name': 'CREATED',
         '_submitted_name': 'SUBMITTED',
         '_accepted_name': 'ACCEPTED',
         '_rejected_name': 'REJECTED',
@@ -133,14 +137,15 @@
         for attr_name, status_value in self._status_dict.items():
             metric_name = getattr(self, attr_name)
             if metric_name:
                 cursors[metric_name] = cursor.AssignmentCursor(
                     pool_id=self.pool_id,
                     event_type=status_value,
                     toloka_client=self.atoloka_client,
+                    time_lag=self._cursor_time_lag,
                     **{f'{status_value.lower()}_gte': start_time},
                 )
         return cursors
 
     async def _get_lines_impl(self) -> Dict[str, List[Tuple[Any, Any]]]:
         result = {}
         for metric_name, it in self._cursors.items():
@@ -449,14 +454,16 @@
     Be careful: if you set in quality controls to ban Tolokers 'on project', bans 'on pool' will never happen.
 
     Args:
         pool_id: From which pool track metrics.
         count_name: Metric name for a count of bans.
         filter_by_comment: Allow to split Toloker restriction into several lines based on comment.
             Dictionary where, key - comment string, and value - name for line in which will be aggregated bans with this comments.
+        cursor_time_lag: Time lag for cursor. This controls time lag between user restrictions being added and this
+            metric being updated. See BaseCursor.time_lag for details and reasoning behind this.
         join_events: Count all events in one point. Default `False`.
 
     Example:
         How to collect this metrics:
         >>> def print_metric(metric_dict):
         >>>     print(metric_dict)
         >>>
@@ -487,14 +494,15 @@
         >>>     'honeypots': [(datetime.datetime(2021, 11, 18, 13, 32, 52, 475000), 1)],
         >>>     'fast': [(datetime.datetime(2021, 11, 18, 13, 32, 50, 453000), 1)],
         >>> }
         ...
     """
     _count_name: Optional[str] = None
     _filter_by_comment: Optional[Dict[str, str]] = None  # {'comment': 'line_name'}
+    _cursor_time_lag: datetime.timedelta = cursor.DEFAULT_LAG
 
     _join_events: bool = False
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         metric_names = self.get_line_names()
         if not metric_names:
@@ -511,15 +519,16 @@
         return line_names
 
     @cached_property
     def _cursor(self) -> cursor.UserRestrictionCursor:
         return cursor.UserRestrictionCursor(
             toloka_client=self.atoloka_client,
             created_gte=datetime.datetime.now(datetime.timezone.utc),
-            pool_id=self.pool_id
+            pool_id=self.pool_id,
+            time_lag=self._cursor_time_lag,
         )
 
     async def _get_lines_impl(self) -> Dict[str, List[Tuple[Any, Any]]]:
         result = defaultdict(list)
 
         it = self._cursor
         event_list = [event async for event in it]
```

### Comparing `toloka-kit-1.1.4/src/metrics/pool_metrics.pyi` & `toloka-kit-1.2.0/src/metrics/pool_metrics.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,16 @@
         created_name: Metric name for a count of created events. Default None.
         submitted_name: Metric name for a count of submitted events. Default 'submitted_events_in_pool'.
         accepted_name : Metric name for a count of accepted events. Default 'accepted_events_in_pool'.
         rejected_name : Metric name for a count of rejected events. Default 'rejected_events_in_pool'.
         skipped_name: Metric name for a count of skipped events. Default None.
         expired_name: Metric name for a count of expired events. Default None.
         join_events: Count all events in one point.  Default `False`.
+        cursor_time_lag: Time lag for cursor. This controls time lag between assignments being added and this metric
+            being updated. See BaseCursor.time_lag for details and reasoning behind this.
 
     Raises:
         ValueError: If all metric names are set to None or if there are duplicate metric names.
 
     Example:
         How to collect this metrics:
         >>> def print_metric(metric_dict):
@@ -84,14 +86,15 @@
         pool_id: str,
         created_name: typing.Optional[str] = None,
         submitted_name: typing.Optional[str] = None,
         accepted_name: typing.Optional[str] = None,
         rejected_name: typing.Optional[str] = None,
         skipped_name: typing.Optional[str] = None,
         expired_name: typing.Optional[str] = None,
+        cursor_time_lag: datetime.timedelta = ...,
         join_events: bool = False,
         *,
         toloka_client: toloka.client.TolokaClient = None,
         atoloka_client: toloka.async_client.client.AsyncTolokaClient = None,
         timeout: datetime.timedelta = ...
     ) -> None:
         """Method generated by attrs for class AssignmentEventsInPool.
@@ -104,14 +107,15 @@
     pool_id: str
     _created_name: typing.Optional[str]
     _submitted_name: typing.Optional[str]
     _accepted_name: typing.Optional[str]
     _rejected_name: typing.Optional[str]
     _skipped_name: typing.Optional[str]
     _expired_name: typing.Optional[str]
+    _cursor_time_lag: datetime.timedelta
     _join_events: bool
 
 
 class PoolCompletedPercentage(BasePoolMetric):
     """Track pool completion in percentage
 
     You can't gather this metric from a pool with infinite task suites. For example, if you have infinite overlap on a pool.
@@ -374,14 +378,16 @@
     Be careful: if you set in quality controls to ban Tolokers 'on project', bans 'on pool' will never happen.
 
     Args:
         pool_id: From which pool track metrics.
         count_name: Metric name for a count of bans.
         filter_by_comment: Allow to split Toloker restriction into several lines based on comment.
             Dictionary where, key - comment string, and value - name for line in which will be aggregated bans with this comments.
+        cursor_time_lag: Time lag for cursor. This controls time lag between user restrictions being added and this
+            metric being updated. See BaseCursor.time_lag for details and reasoning behind this.
         join_events: Count all events in one point. Default `False`.
 
     Example:
         How to collect this metrics:
         >>> def print_metric(metric_dict):
         >>>     print(metric_dict)
         >>>
@@ -421,14 +427,15 @@
         ...
 
     def __init__(
         self,
         pool_id: str,
         count_name: typing.Optional[str] = None,
         filter_by_comment: typing.Optional[typing.Dict[str, str]] = None,
+        cursor_time_lag: datetime.timedelta = ...,
         join_events: bool = False,
         *,
         toloka_client: toloka.client.TolokaClient = None,
         atoloka_client: toloka.async_client.client.AsyncTolokaClient = None,
         timeout: datetime.timedelta = ...
     ) -> None:
         """Method generated by attrs for class BansInPool.
@@ -437,8 +444,9 @@
 
     toloka_client: toloka.client.TolokaClient
     atoloka_client: toloka.async_client.client.AsyncTolokaClient
     timeout: datetime.timedelta
     pool_id: str
     _count_name: typing.Optional[str]
     _filter_by_comment: typing.Optional[typing.Dict[str, str]]
+    _cursor_time_lag: datetime.timedelta
     _join_events: bool
```

### Comparing `toloka-kit-1.1.4/src/streaming/__init__.py` & `toloka-kit-1.2.0/src/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/streaming/__init__.pyi` & `toloka-kit-1.2.0/src/streaming/__init__.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/streaming/cursor.py` & `toloka-kit-1.2.0/src/streaming/cursor.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,16 +10,18 @@
     'UserSkillCursor',
 ]
 
 import asyncio
 import attr
 import copy
 import functools
-from datetime import datetime
+from datetime import datetime, timedelta, timezone
 from typing import Any, AsyncIterator, Awaitable, Callable, Iterator, List, Optional, Set, Tuple, Union
+
+from toloka.util._docstrings import inherit_docstrings
 from typing_extensions import Protocol
 
 from ..async_client import AsyncTolokaClient
 from ..client import (
     Assignment,
     MessageThread,
     Task,
@@ -41,15 +43,16 @@
 class ResponseObjectType(Protocol):
     items: Optional[List[Any]]
     has_more: Optional[bool]
 
 
 TolokaClientSyncOrAsyncType = Union[TolokaClient, AsyncTolokaClient]
 
-DATETIME_MIN = datetime.fromtimestamp(0)
+DATETIME_MIN = datetime.fromtimestamp(0, tz=timezone.utc)
+DEFAULT_LAG = timedelta(minutes=1)
 
 
 @attr.s
 class _ByIdCursor:
     """Iterate by id only."""
     fetcher: Callable[[BaseSearchRequest], ResponseObjectType] = attr.ib()
     request: BaseSearchRequest = attr.ib()
@@ -73,16 +76,25 @@
                 self.request = attr.evolve(self.request, id_gt=item.id)
             if not response.has_more:
                 return
 
 
 @attr.s
 class BaseCursor:
+    """Base class for all cursors.
+
+    Args:
+        _time_lag: Time lag between cursor time field upper bound and real time. Default is 1 minute. This lag is
+            required to keep cursor consistent. Lowering this value will make cursor process events faster, but raises
+            probability of missing some events in case of concurrent operations.
+    """
+
     toloka_client: TolokaClientSyncOrAsyncType = attr.ib()
     _request: BaseSearchRequest = attr.ib()
+    _time_lag: timedelta = attr.ib(default=DEFAULT_LAG)
     _prev_response: Optional[ResponseObjectType] = attr.ib(default=None, init=False)
     _seen_ids: Set[str] = attr.ib(factory=set, init=False)
 
     @attr.s
     class CursorFetchContext:
         """Context manager to return from `BaseCursor.try_fetch_all method`.
         Commit cursor state only if no error occured.
@@ -154,28 +166,36 @@
 
     @property
     def _time_field_gt(self) -> str:
         return f'{self._get_time_field()}_gt'  # To use after iteration by id.
 
     def __iter__(self) -> Iterator[BaseEvent]:
         fetcher = self._get_fetcher()
+        self._request = attr.evolve(
+            self._request, **{self._time_field_lte: datetime.now(tz=timezone.utc) - self._time_lag}
+        )
         while True:
             response = fetcher(self._request, sort=self._get_time_field())  # Diff between sync and async.
             if response.items:
                 max_time = self._get_time(response.items[-1])
                 self._prev_response = response
                 for item in response.items:
                     if item.id not in self._seen_ids:
                         self._request = attr.evolve(self._request, **{self._time_field_gte: self._get_time(item)})
                         self._seen_ids.add(item.id)
                         yield self._construct_event(item)
 
                 if not response.has_more:
                     return
 
+                # Multiple items can have the same time field value. If items with the same time field value are split
+                # between responses due to the fetcher limit they will be fetched twice and filtered by _seen_ids field
+                # afterward. But there is a corner case when all items in the response have the same time field value.
+                # As the result we will fetch the same items over and over again. To avoid this we need fallback to
+                # iteration over id field.
                 if self._get_time(response.items[0]) == max_time:
                     fixed_time_request = attr.evolve(self._request, **{self._time_field_lte: max_time})
                     for item in _ByIdCursor(fetcher, fixed_time_request):  # Diff between sync and async.
                         if item.id not in self._seen_ids:
                             self._seen_ids.add(item.id)
                             yield self._construct_event(item)
                     self._request = attr.evolve(self._request, **{self._time_field_gt: max_time})
@@ -183,28 +203,36 @@
                 # Strip it to the current response size.
                 self._seen_ids = {item.id for item in response.items}
             else:
                 return
 
     async def __aiter__(self) -> AsyncIterator[BaseEvent]:
         fetcher = self._get_fetcher()
+        self._request = attr.evolve(
+            self._request, **{self._time_field_lte: datetime.now(tz=timezone.utc) - self._time_lag}
+        )
         while True:
             response = await ensure_async(fetcher)(self._request, sort=self._get_time_field())  # Diff between sync and async.
             if response.items:
                 max_time = self._get_time(response.items[-1])
                 self._prev_response = response
                 for item in response.items:
                     if item.id not in self._seen_ids:
                         self._request = attr.evolve(self._request, **{self._time_field_gte: self._get_time(item)})
                         self._seen_ids.add(item.id)
                         yield self._construct_event(item)
 
                 if not response.has_more:
                     return
 
+                # Multiple items can have the same time field value. If items with the same time field value are split
+                # between responses due to the fetcher limit they will be fetched twice and filtered by _seen_ids field
+                # afterward. But there is a corner case when all items in the response have the same time field value.
+                # As the result we will fetch the same items over and over again. To avoid this we need fallback to
+                # iteration over id field.
                 if self._get_time(response.items[0]) == max_time:
                     fixed_time_request = attr.evolve(self._request, **{self._time_field_lte: max_time})
                     async for item in _ByIdCursor(fetcher, fixed_time_request):  # Diff between sync and async.
                         if item.id not in self._seen_ids:
                             self._seen_ids.add(item.id)
                             yield self._construct_event(item)
                     self._request = attr.evolve(self._request, **{self._time_field_gt: max_time})
@@ -213,17 +241,18 @@
                 self._seen_ids = {item.id for item in response.items}
             else:
                 return
 
 
 @expand('request')
 @fix_attrs_converters
+@inherit_docstrings
 @attr.s
 class AssignmentCursor(BaseCursor):
-    """Iterator over Assignment objects of seleted AssignmentEventType.
+    """Iterator over Assignment objects of selected AssignmentEventType.
 
     Args:
         toloka_client: TolokaClient object that is being used to search assignments.
         request: Base request to search assignments by.
         event_type: Assignments event's type to search.
 
     Examples:
@@ -238,14 +267,15 @@
 
     BATCH_SIZE = 1000
 
     _event_type: AssignmentEvent.Type = attr.ib(converter=functools.partial(structure, cl=AssignmentEvent.Type))
     _request: search_requests.AssignmentSearchRequest = attr.ib(
         factory=search_requests.AssignmentSearchRequest,
     )
+    _time_lag: timedelta = attr.ib(default=DEFAULT_LAG)
 
     def _get_fetcher(self) -> Callable[..., search_results.AssignmentSearchResult]:
         async def _async_fetcher(*args, **kwargs):
             return await self.toloka_client.find_assignments(*args, limit=self.BATCH_SIZE, **kwargs)
 
         method = self.toloka_client.find_assignments
         if asyncio.iscoroutinefunction(method) or asyncio.iscoroutinefunction(getattr(method, '__call__', None)):
@@ -259,14 +289,15 @@
         return AssignmentEvent(assignment=item,
                                event_type=self._event_type,
                                event_time=getattr(item, self._event_type.time_key))
 
 
 @expand('request')
 @fix_attrs_converters
+@inherit_docstrings
 @attr.s
 class TaskCursor(BaseCursor):
     """Iterator over tasks by create time.
 
     Args:
         toloka_client: TolokaClient object that is being used to search tasks.
         request: Base request to search tasks by.
@@ -293,14 +324,15 @@
 
     def _construct_event(self, item: Task) -> TaskEvent:
         return TaskEvent(task=item, event_time=item.created)
 
 
 @expand('request')
 @fix_attrs_converters
+@inherit_docstrings
 @attr.s
 class UserBonusCursor(BaseCursor):
     """Iterator over `UserBonus` instances by create time.
 
     Args:
         toloka_client: TolokaClient object that is being used to search `UserBonus` instances.
         request: Base request to search `UserBonus` instances by.
@@ -327,14 +359,15 @@
 
     def _construct_event(self, item: UserBonus) -> UserBonusEvent:
         return UserBonusEvent(user_bonus=item, event_time=item.created)
 
 
 @expand('request')
 @fix_attrs_converters
+@inherit_docstrings
 @attr.s
 class UserSkillCursor(BaseCursor):
     """Iterator over UserSkillEvent objects of a selected event_type.
 
     Args:
         toloka_client: TolokaClient object that is being used to search skills.
         request: Base request to search skills by.
@@ -350,14 +383,15 @@
         ...
     """
 
     _event_type: UserSkillEvent.Type = attr.ib(converter=functools.partial(structure, cl=UserSkillEvent.Type))
     _request: search_requests.UserSkillSearchRequest = attr.ib(
         factory=search_requests.UserSkillSearchRequest,
     )
+    _time_lag: timedelta = attr.ib(default=DEFAULT_LAG)
 
     def _get_fetcher(self) -> Callable[..., search_results.UserSkillSearchResult]:
         return self.toloka_client.find_user_skills
 
     def _get_time_field(self) -> str:
         return self._event_type.time_key
 
@@ -365,14 +399,15 @@
         return UserSkillEvent(user_skill=item,
                               event_type=self._event_type,
                               event_time=getattr(item, self._event_type.time_key))
 
 
 @expand('request')
 @fix_attrs_converters
+@inherit_docstrings
 @attr.s
 class UserRestrictionCursor(BaseCursor):
     """Iterator over Toloker restrictions by create time.
 
     Args:
         toloka_client: TolokaClient object that is being used to search Toloker restrictions.
         request: Base request to search Toloker restrictions.
@@ -399,14 +434,15 @@
 
     def _construct_event(self, item: UserRestriction) -> UserRestrictionEvent:
         return UserRestrictionEvent(user_restriction=item, event_time=getattr(item, self._get_time_field()))
 
 
 @expand('request')
 @fix_attrs_converters
+@inherit_docstrings
 @attr.s
 class MessageThreadCursor(BaseCursor):
     """Iterator over messages by create time.
 
     Args:
         toloka_client: TolokaClient object that is being used to search messages.
         request: Base request to search messages.
```

### Comparing `toloka-kit-1.1.4/src/streaming/cursor.pyi` & `toloka-kit-1.2.0/src/streaming/cursor.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -14,19 +14,18 @@
 import toloka.client
 import toloka.client.assignment
 import toloka.client.message_thread
 import toloka.client.search_requests
 import toloka.client.user_restriction
 import toloka.streaming.event
 import typing
+import typing_extensions
 
 
-class ResponseObjectType(typing.Protocol):
-    def __subclasshook__(other): ...
-
+class ResponseObjectType(typing_extensions.Protocol):
     def __init__(
         self,
         *args,
         **kwargs
     ): ...
 
     items: typing.Optional[typing.List[typing.Any]]
@@ -34,14 +33,22 @@
 
 
 TolokaClientSyncOrAsyncType = typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient]
 
 DATETIME_MIN = ...
 
 class BaseCursor:
+    """Base class for all cursors.
+
+    Args:
+        _time_lag: Time lag between cursor time field upper bound and real time. Default is 1 minute. This lag is
+            required to keep cursor consistent. Lowering this value will make cursor process events faster, but raises
+            probability of missing some events in case of concurrent operations.
+    """
+
     class CursorFetchContext:
         """Context manager to return from `BaseCursor.try_fetch_all method`.
         Commit cursor state only if no error occured.
         """
 
         def __enter__(self) -> typing.List[toloka.streaming.event.BaseEvent]: ...
 
@@ -79,33 +86,38 @@
     def __iter__(self) -> typing.Iterator[toloka.streaming.event.BaseEvent]: ...
 
     def __aiter__(self) -> typing.AsyncIterator[toloka.streaming.event.BaseEvent]: ...
 
     def __init__(
         self,
         toloka_client: typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient],
-        request: toloka.client.search_requests.BaseSearchRequest
+        request: toloka.client.search_requests.BaseSearchRequest,
+        time_lag: datetime.timedelta = ...
     ) -> None:
         """Method generated by attrs for class BaseCursor.
         """
         ...
 
     toloka_client: typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient]
     _request: toloka.client.search_requests.BaseSearchRequest
+    _time_lag: datetime.timedelta
     _prev_response: typing.Optional[ResponseObjectType]
     _seen_ids: typing.Set[str]
 
 
 class AssignmentCursor(BaseCursor):
-    """Iterator over Assignment objects of seleted AssignmentEventType.
+    """Iterator over Assignment objects of selected AssignmentEventType.
 
     Args:
         toloka_client: TolokaClient object that is being used to search assignments.
-        request: Base request to search assignments by.
         event_type: Assignments event's type to search.
+        request: Base request to search assignments by.
+        _time_lag: Time lag between cursor time field upper bound and real time. Default is 1 minute. This lag is
+            required to keep cursor consistent. Lowering this value will make cursor process events faster, but raises
+            probability of missing some events in case of concurrent operations.
 
     Examples:
         Iterate over assignment acceptances events.
 
         >>> it = AssignmentCursor(pool_id='123', event_type='ACCEPTED', toloka_client=toloka_client)
         >>> current_events = list(it)
         >>> # ... new events may occur ...
@@ -114,15 +126,16 @@
     """
 
     @typing.overload
     def __init__(
         self,
         toloka_client: typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient],
         event_type: typing.Any,
-        request: toloka.client.search_requests.AssignmentSearchRequest = ...
+        request: toloka.client.search_requests.AssignmentSearchRequest = ...,
+        time_lag: datetime.timedelta = ...
     ) -> None:
         """Method generated by attrs for class AssignmentCursor.
         """
         ...
 
     @typing.overload
     def __init__(
@@ -157,33 +170,38 @@
         skipped_lt: typing.Optional[datetime.datetime] = None,
         skipped_lte: typing.Optional[datetime.datetime] = None,
         skipped_gt: typing.Optional[datetime.datetime] = None,
         skipped_gte: typing.Optional[datetime.datetime] = None,
         expired_lt: typing.Optional[datetime.datetime] = None,
         expired_lte: typing.Optional[datetime.datetime] = None,
         expired_gt: typing.Optional[datetime.datetime] = None,
-        expired_gte: typing.Optional[datetime.datetime] = None
+        expired_gte: typing.Optional[datetime.datetime] = None,
+        time_lag: datetime.timedelta = ...
     ) -> None:
         """Method generated by attrs for class AssignmentCursor.
         """
         ...
 
     toloka_client: typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient]
     _request: toloka.client.search_requests.AssignmentSearchRequest
+    _time_lag: datetime.timedelta
     _prev_response: typing.Optional[ResponseObjectType]
     _seen_ids: typing.Set[str]
     _event_type: toloka.streaming.event.AssignmentEvent.Type
 
 
 class TaskCursor(BaseCursor):
     """Iterator over tasks by create time.
 
     Args:
         toloka_client: TolokaClient object that is being used to search tasks.
         request: Base request to search tasks by.
+        _time_lag: Time lag between cursor time field upper bound and real time. Default is 1 minute. This lag is
+            required to keep cursor consistent. Lowering this value will make cursor process events faster, but raises
+            probability of missing some events in case of concurrent operations.
 
     Examples:
         Iterate over tasks.
 
         >>> it = TaskCursor(pool_id='123', toloka_client=toloka_client)
         >>> current_tasks = list(it)
         >>> # ... new tasks could appear ...
@@ -191,24 +209,26 @@
         ...
     """
 
     @typing.overload
     def __init__(
         self,
         toloka_client: typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient],
+        time_lag: datetime.timedelta = ...,
         request: toloka.client.search_requests.TaskSearchRequest = ...
     ) -> None:
         """Method generated by attrs for class TaskCursor.
         """
         ...
 
     @typing.overload
     def __init__(
         self,
         toloka_client: typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient],
+        time_lag: datetime.timedelta = ...,
         pool_id: typing.Optional[str] = None,
         overlap: typing.Optional[int] = None,
         id_lt: typing.Optional[str] = None,
         id_lte: typing.Optional[str] = None,
         id_gt: typing.Optional[str] = None,
         id_gte: typing.Optional[str] = None,
         created_lt: typing.Optional[datetime.datetime] = None,
@@ -222,24 +242,28 @@
     ) -> None:
         """Method generated by attrs for class TaskCursor.
         """
         ...
 
     toloka_client: typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient]
     _request: toloka.client.search_requests.TaskSearchRequest
+    _time_lag: datetime.timedelta
     _prev_response: typing.Optional[ResponseObjectType]
     _seen_ids: typing.Set[str]
 
 
 class UserBonusCursor(BaseCursor):
     """Iterator over `UserBonus` instances by create time.
 
     Args:
         toloka_client: TolokaClient object that is being used to search `UserBonus` instances.
         request: Base request to search `UserBonus` instances by.
+        _time_lag: Time lag between cursor time field upper bound and real time. Default is 1 minute. This lag is
+            required to keep cursor consistent. Lowering this value will make cursor process events faster, but raises
+            probability of missing some events in case of concurrent operations.
 
     Examples:
         Iterate over `UserBonus` instances.
 
         >>> it = UserBonusCursor(toloka_client=toloka_client)
         >>> current_bonuses = list(it)
         >>> # ... new `UserBonus` instances could appear ...
@@ -247,24 +271,26 @@
         ...
     """
 
     @typing.overload
     def __init__(
         self,
         toloka_client: typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient],
+        time_lag: datetime.timedelta = ...,
         request: toloka.client.search_requests.UserBonusSearchRequest = ...
     ) -> None:
         """Method generated by attrs for class UserBonusCursor.
         """
         ...
 
     @typing.overload
     def __init__(
         self,
         toloka_client: typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient],
+        time_lag: datetime.timedelta = ...,
         user_id: typing.Optional[str] = None,
         assignment_id: typing.Optional[str] = None,
         private_comment: typing.Optional[str] = None,
         id_lt: typing.Optional[str] = None,
         id_lte: typing.Optional[str] = None,
         id_gt: typing.Optional[str] = None,
         id_gte: typing.Optional[str] = None,
@@ -275,25 +301,29 @@
     ) -> None:
         """Method generated by attrs for class UserBonusCursor.
         """
         ...
 
     toloka_client: typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient]
     _request: toloka.client.search_requests.UserBonusSearchRequest
+    _time_lag: datetime.timedelta
     _prev_response: typing.Optional[ResponseObjectType]
     _seen_ids: typing.Set[str]
 
 
 class UserSkillCursor(BaseCursor):
     """Iterator over UserSkillEvent objects of a selected event_type.
 
     Args:
         toloka_client: TolokaClient object that is being used to search skills.
-        request: Base request to search skills by.
         event_type: Skill event type to search.
+        request: Base request to search skills by.
+        _time_lag: Time lag between cursor time field upper bound and real time. Default is 1 minute. This lag is
+            required to keep cursor consistent. Lowering this value will make cursor process events faster, but raises
+            probability of missing some events in case of concurrent operations.
 
     Examples:
         Iterate over skills acceptances events.
 
         >>> it = UserSkillCursor(event_type='MODIFIED', toloka_client=toloka_client)
         >>> current_events = list(it)
         >>> # ... new skills could be set ...
@@ -302,15 +332,16 @@
     """
 
     @typing.overload
     def __init__(
         self,
         toloka_client: typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient],
         event_type: typing.Any,
-        request: toloka.client.search_requests.UserSkillSearchRequest = ...
+        request: toloka.client.search_requests.UserSkillSearchRequest = ...,
+        time_lag: datetime.timedelta = ...
     ) -> None:
         """Method generated by attrs for class UserSkillCursor.
         """
         ...
 
     @typing.overload
     def __init__(
@@ -326,33 +357,38 @@
         created_lt: typing.Optional[datetime.datetime] = None,
         created_lte: typing.Optional[datetime.datetime] = None,
         created_gt: typing.Optional[datetime.datetime] = None,
         created_gte: typing.Optional[datetime.datetime] = None,
         modified_lt: typing.Optional[datetime.datetime] = None,
         modified_lte: typing.Optional[datetime.datetime] = None,
         modified_gt: typing.Optional[datetime.datetime] = None,
-        modified_gte: typing.Optional[datetime.datetime] = None
+        modified_gte: typing.Optional[datetime.datetime] = None,
+        time_lag: datetime.timedelta = ...
     ) -> None:
         """Method generated by attrs for class UserSkillCursor.
         """
         ...
 
     toloka_client: typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient]
     _request: toloka.client.search_requests.UserSkillSearchRequest
+    _time_lag: datetime.timedelta
     _prev_response: typing.Optional[ResponseObjectType]
     _seen_ids: typing.Set[str]
     _event_type: toloka.streaming.event.UserSkillEvent.Type
 
 
 class UserRestrictionCursor(BaseCursor):
     """Iterator over Toloker restrictions by create time.
 
     Args:
         toloka_client: TolokaClient object that is being used to search Toloker restrictions.
         request: Base request to search Toloker restrictions.
+        _time_lag: Time lag between cursor time field upper bound and real time. Default is 1 minute. This lag is
+            required to keep cursor consistent. Lowering this value will make cursor process events faster, but raises
+            probability of missing some events in case of concurrent operations.
 
     Examples:
         Iterate over Toloker restrictions in a project.
 
         >>> it = UserRestrictionCursor(toloka_client=toloka_client, project_id=my_proj_id)
         >>> current_restrictions = list(it)
         >>> # ... new restrictions could appear ...
@@ -360,24 +396,26 @@
         ...
     """
 
     @typing.overload
     def __init__(
         self,
         toloka_client: typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient],
+        time_lag: datetime.timedelta = ...,
         request: toloka.client.search_requests.UserRestrictionSearchRequest = ...
     ) -> None:
         """Method generated by attrs for class UserRestrictionCursor.
         """
         ...
 
     @typing.overload
     def __init__(
         self,
         toloka_client: typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient],
+        time_lag: datetime.timedelta = ...,
         scope: typing.Optional[toloka.client.user_restriction.UserRestriction.Scope] = None,
         user_id: typing.Optional[str] = None,
         project_id: typing.Optional[str] = None,
         pool_id: typing.Optional[str] = None,
         id_lt: typing.Optional[str] = None,
         id_lte: typing.Optional[str] = None,
         id_gt: typing.Optional[str] = None,
@@ -389,24 +427,28 @@
     ) -> None:
         """Method generated by attrs for class UserRestrictionCursor.
         """
         ...
 
     toloka_client: typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient]
     _request: toloka.client.search_requests.UserRestrictionSearchRequest
+    _time_lag: datetime.timedelta
     _prev_response: typing.Optional[ResponseObjectType]
     _seen_ids: typing.Set[str]
 
 
 class MessageThreadCursor(BaseCursor):
     """Iterator over messages by create time.
 
     Args:
         toloka_client: TolokaClient object that is being used to search messages.
         request: Base request to search messages.
+        _time_lag: Time lag between cursor time field upper bound and real time. Default is 1 minute. This lag is
+            required to keep cursor consistent. Lowering this value will make cursor process events faster, but raises
+            probability of missing some events in case of concurrent operations.
 
     Examples:
         Iterate over all messages.
 
         >>> it = MessageThreadCursor(toloka_client=toloka_client)
         >>> all_messages = list(it)
         >>> # ... new messages could appear ...
@@ -414,24 +456,26 @@
         ...
     """
 
     @typing.overload
     def __init__(
         self,
         toloka_client: typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient],
+        time_lag: datetime.timedelta = ...,
         request: toloka.client.search_requests.MessageThreadSearchRequest = ...
     ) -> None:
         """Method generated by attrs for class MessageThreadCursor.
         """
         ...
 
     @typing.overload
     def __init__(
         self,
         toloka_client: typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient],
+        time_lag: datetime.timedelta = ...,
         folder: typing.Union[str, toloka.client.message_thread.Folder, typing.List[typing.Union[str, toloka.client.message_thread.Folder]]] = None,
         folder_ne: typing.Union[str, toloka.client.message_thread.Folder, typing.List[typing.Union[str, toloka.client.message_thread.Folder]]] = None,
         id_lt: typing.Optional[str] = None,
         id_lte: typing.Optional[str] = None,
         id_gt: typing.Optional[str] = None,
         id_gte: typing.Optional[str] = None,
         created_lt: typing.Optional[datetime.datetime] = None,
@@ -441,9 +485,10 @@
     ) -> None:
         """Method generated by attrs for class MessageThreadCursor.
         """
         ...
 
     toloka_client: typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient]
     _request: toloka.client.search_requests.MessageThreadSearchRequest
+    _time_lag: datetime.timedelta
     _prev_response: typing.Optional[ResponseObjectType]
     _seen_ids: typing.Set[str]
```

### Comparing `toloka-kit-1.1.4/src/streaming/event.py` & `toloka-kit-1.2.0/src/streaming/event.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/streaming/event.pyi` & `toloka-kit-1.2.0/src/streaming/event.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/streaming/locker.py` & `toloka-kit-1.2.0/src/streaming/locker.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/streaming/locker.pyi` & `toloka-kit-1.2.0/src/streaming/locker.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/streaming/observer.py` & `toloka-kit-1.2.0/src/streaming/observer.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,27 +13,30 @@
 from typing import Any, Awaitable, Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 from ..client.primitives.base import autocast_to_enum
 from ..client.assignment import Assignment
 from ..client.pool import Pool
 from ..util.async_utils import AsyncInterfaceWrapper, ComplexException, ensure_async, get_task_traceback
 from ..util._managing_headers import add_headers
-from .cursor import AssignmentCursor, TolokaClientSyncOrAsyncType
+from .cursor import AssignmentCursor, TolokaClientSyncOrAsyncType, DEFAULT_LAG
 from .event import AssignmentEvent
 
 logger = logging.getLogger(__name__)
 
 
 @attr.s
 class BaseObserver:
     name: Optional[str] = attr.ib(default=None, kw_only=True)
     _enabled: bool = attr.ib(default=True, init=False)
     _deleted: bool = attr.ib(default=False, init=False)
 
-    def _get_unique_key(self) -> Tuple:
+    def get_unique_key(self) -> Tuple:
+        """This method should return identifier for this observer that is unique in the current pipeline context.
+        """
+
         return (self.__class__.__name__, self.name or '')
 
     def inject(self, injection: Any) -> None:
         raise NotImplementedError
 
     async def __call__(self) -> None:
         raise NotImplementedError
@@ -123,16 +126,16 @@
 
 @attr.s
 class BasePoolObserver(BaseObserver):
 
     toloka_client: AsyncInterfaceWrapper[TolokaClientSyncOrAsyncType] = attr.ib(converter=_wrap_client_to_async_converter)
     pool_id: str = attr.ib()
 
-    def _get_unique_key(self) -> Tuple:
-        return super()._get_unique_key() + (self.pool_id,)
+    def get_unique_key(self) -> Tuple:
+        return super().get_unique_key() + (self.pool_id,)
 
     @add_headers('streaming')
     async def should_resume(self) -> bool:
         logger.info('Check resume by pool status: %s', self.pool_id)
         pool = await self.toloka_client.get_pool(self.pool_id)
         logger.info('Pool status for %s: %s', self.pool_id, pool.status)
         if pool.is_open():
@@ -183,16 +186,16 @@
         >>> observer.on_status_change(lambda pool: ...)
         ...
     """
 
     _callbacks: Dict[Pool.Status, List[CallbackForPoolAsyncType]] = attr.ib(factory=dict, init=False)
     _previous_status: Optional[Pool.Status] = attr.ib(default=None, init=False)
 
-    def _get_unique_key(self) -> Tuple:
-        return super()._get_unique_key() + tuple(sorted(
+    def get_unique_key(self) -> Tuple:
+        return super().get_unique_key() + tuple(sorted(
             (status.value, _get_callbacks_unique_key(callbacks))
             for status, callbacks in self._callbacks.items()
         ))
 
     def inject(self, injection: 'PoolStatusObserver') -> None:
         injection_callbacks_by_status = {
             status: callbacks
@@ -272,15 +275,15 @@
 class _CallbacksCursorConsumer:
     """Store cursor and related callbacks.
     Allow to run callbacks at fetched data and move the cursor in case of success.
     """
     cursor: AssignmentCursor = attr.ib()
     callbacks: List[CallbackForAssignmentEventsAsyncType] = attr.ib(factory=list, init=False)
 
-    def _get_unique_key(self) -> Tuple:
+    def get_unique_key(self) -> Tuple:
         return self.cursor._event_type.value, _get_callbacks_unique_key(self.callbacks)
 
     def inject(self, injection: '_CallbacksCursorConsumer') -> None:
         self.cursor.inject(injection.cursor)
         self.callbacks = _inject_callbacks(self.callbacks, injection.callbacks)
 
     def add_callback(self, callback: CallbackForAssignmentEventsType) -> None:
@@ -318,42 +321,45 @@
         * on_expired
 
     Corresponding assignment events will be passed to the triggered callbacks.
 
     Attributes:
         toloka_client: TolokaClient instance or async wrapper around it.
         pool_id: Pool ID.
+        cursor_time_lag: Time lag for cursor. This controls time lag between assignments being added and them being
+            seen by this observer. See BaseCursor.time_lag for details and reasoning behind this.
 
     Examples:
         Send submitted assignments for verification.
 
         >>> def handle_submitted(evets: List[AssignmentEvent]) -> None:
         >>>     verification_tasks = [create_veridication_task(item.assignment) for item in evets]
         >>>     toloka_client.create_tasks(verification_tasks, open_pool=True)
         >>>
         >>> observer = AssignmentsObserver(toloka_client, pool_id='123')
         >>> observer.on_submitted(handle_submitted)
         ...
     """
 
+    cursor_time_lag: datetime.timedelta = attr.ib(default=DEFAULT_LAG)
     _callbacks: Dict[AssignmentEvent.Type, _CallbacksCursorConsumer] = attr.ib(factory=dict, init=False)
 
-    def _get_unique_key(self) -> Tuple:
-        return super()._get_unique_key() + tuple(sorted(
-            consumer._get_unique_key()
+    def get_unique_key(self) -> Tuple:
+        return super().get_unique_key() + tuple(sorted(
+            consumer.get_unique_key()
             for consumer in self._callbacks.values()
         ))
 
     def inject(self, injection: 'AssignmentsObserver') -> None:
         injection_consumer_by_key = {
-            consumer._get_unique_key(): consumer
+            consumer.get_unique_key(): consumer
             for consumer in injection._callbacks.values()
         }
         for consumer in self._callbacks.values():
-            key = consumer._get_unique_key()
+            key = consumer.get_unique_key()
             consumer.inject(injection_consumer_by_key[key])
 
     # Setup section.
 
     @autocast_to_enum
     def register_callback(
         self,
@@ -367,15 +373,20 @@
             callback: Sync or async callable that pass List[AssignmentEvent] of desired event type.
             event_type: Selected event type.
 
         Returns:
             The same callable passed as callback.
         """
         if event_type not in self._callbacks:
-            cursor = AssignmentCursor(pool_id=self.pool_id, event_type=event_type, toloka_client=self.toloka_client)
+            cursor = AssignmentCursor(
+                pool_id=self.pool_id,
+                event_type=event_type,
+                toloka_client=self.toloka_client,
+                time_lag=self.cursor_time_lag
+            )
             self._callbacks[event_type] = _CallbacksCursorConsumer(cursor)
         self._callbacks[event_type].add_callback(callback)
         return callback
 
     def on_any_event(self, callback: CallbackForAssignmentEventsType) -> CallbackForAssignmentEventsType:
         for event_type in AssignmentEvent.Type.__members__.values():
             self.register_callback(callback, event_type)
```

### Comparing `toloka-kit-1.1.4/src/streaming/observer.pyi` & `toloka-kit-1.2.0/src/streaming/observer.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 import toloka.streaming.cursor
 import toloka.streaming.event
 import toloka.util.async_utils
 import typing
 
 
 class BaseObserver:
+    def get_unique_key(self) -> typing.Tuple:
+        """This method should return identifier for this observer that is unique in the current pipeline context.
+        """
+        ...
+
     def inject(self, injection: typing.Any) -> None: ...
 
     async def __call__(self) -> None: ...
 
     async def should_resume(self) -> bool: ...
 
     def delete(self) -> None:
@@ -47,14 +52,16 @@
 
     name: typing.Optional[str]
     _enabled: bool
     _deleted: bool
 
 
 class BasePoolObserver(BaseObserver):
+    def get_unique_key(self) -> typing.Tuple: ...
+
     async def should_resume(self) -> bool: ...
 
     def __init__(
         self,
         toloka_client: typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient],
         pool_id: str,
         *,
@@ -101,14 +108,16 @@
 
         Call something at any status change.
 
         >>> observer.on_status_change(lambda pool: ...)
         ...
     """
 
+    def get_unique_key(self) -> typing.Tuple: ...
+
     def inject(self, injection: 'PoolStatusObserver') -> None: ...
 
     def register_callback(
         self,
         callback: typing.Union[typing.Callable[[toloka.client.pool.Pool], None], typing.Callable[[toloka.client.pool.Pool], typing.Awaitable[None]]],
         changed_to: typing.Union[toloka.client.pool.Pool.Status, str]
     ) -> typing.Union[typing.Callable[[toloka.client.pool.Pool], None], typing.Callable[[toloka.client.pool.Pool], typing.Awaitable[None]]]:
@@ -154,14 +163,16 @@
 
 
 class _CallbacksCursorConsumer:
     """Store cursor and related callbacks.
     Allow to run callbacks at fetched data and move the cursor in case of success.
     """
 
+    def get_unique_key(self) -> typing.Tuple: ...
+
     def inject(self, injection: '_CallbacksCursorConsumer') -> None: ...
 
     def add_callback(self, callback: typing.Union[typing.Callable[[typing.List[toloka.streaming.event.AssignmentEvent]], None], typing.Callable[[typing.List[toloka.streaming.event.AssignmentEvent]], typing.Awaitable[None]]]) -> None: ...
 
     async def __call__(self, pool_id: str) -> None: ...
 
     def __init__(self, cursor: toloka.streaming.cursor.AssignmentCursor) -> None:
@@ -186,27 +197,31 @@
         * on_expired
 
     Corresponding assignment events will be passed to the triggered callbacks.
 
     Attributes:
         toloka_client: TolokaClient instance or async wrapper around it.
         pool_id: Pool ID.
+        cursor_time_lag: Time lag for cursor. This controls time lag between assignments being added and them being
+            seen by this observer. See BaseCursor.time_lag for details and reasoning behind this.
 
     Examples:
         Send submitted assignments for verification.
 
         >>> def handle_submitted(evets: List[AssignmentEvent]) -> None:
         >>>     verification_tasks = [create_veridication_task(item.assignment) for item in evets]
         >>>     toloka_client.create_tasks(verification_tasks, open_pool=True)
         >>>
         >>> observer = AssignmentsObserver(toloka_client, pool_id='123')
         >>> observer.on_submitted(handle_submitted)
         ...
     """
 
+    def get_unique_key(self) -> typing.Tuple: ...
+
     def inject(self, injection: 'AssignmentsObserver') -> None: ...
 
     def register_callback(
         self,
         callback: typing.Union[typing.Callable[[typing.List[toloka.streaming.event.AssignmentEvent]], None], typing.Callable[[typing.List[toloka.streaming.event.AssignmentEvent]], typing.Awaitable[None]]],
         event_type: typing.Union[toloka.streaming.event.AssignmentEvent.Type, str]
     ) -> typing.Union[typing.Callable[[typing.List[toloka.streaming.event.AssignmentEvent]], None], typing.Callable[[typing.List[toloka.streaming.event.AssignmentEvent]], typing.Awaitable[None]]]:
@@ -236,20 +251,22 @@
 
     def on_expired(self, callback: typing.Union[typing.Callable[[typing.List[toloka.streaming.event.AssignmentEvent]], None], typing.Callable[[typing.List[toloka.streaming.event.AssignmentEvent]], typing.Awaitable[None]]]) -> typing.Union[typing.Callable[[typing.List[toloka.streaming.event.AssignmentEvent]], None], typing.Callable[[typing.List[toloka.streaming.event.AssignmentEvent]], typing.Awaitable[None]]]: ...
 
     def __init__(
         self,
         toloka_client: typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient],
         pool_id: str,
+        cursor_time_lag: datetime.timedelta = ...,
         *,
         name: typing.Optional[str] = None
     ) -> None:
         """Method generated by attrs for class AssignmentsObserver.
         """
         ...
 
     name: typing.Optional[str]
     _enabled: bool
     _deleted: bool
     toloka_client: toloka.util.async_utils.AsyncInterfaceWrapper[typing.Union[toloka.client.TolokaClient, toloka.async_client.client.AsyncTolokaClient]]
     pool_id: str
+    cursor_time_lag: datetime.timedelta
     _callbacks: typing.Dict[toloka.streaming.event.AssignmentEvent.Type, _CallbacksCursorConsumer]
```

### Comparing `toloka-kit-1.1.4/src/streaming/pipeline.py` & `toloka-kit-1.2.0/src/streaming/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     def __eq__(self, other) -> bool:
         if not isinstance(other, _Worker):
             return False
         return self.name == other.name
 
     @classmethod
     def _from_observer(cls, observer: BaseObserver) -> '_Worker':
-        return cls(str(observer._get_unique_key()), observer)
+        return cls(str(observer.get_unique_key()), observer)
 
     @staticmethod
     def _no_one_should_resume(workers: Iterable['_Worker']) -> bool:
         return all(not worker.should_resume for worker in workers)
 
     def _is_deleted(self) -> bool:
         return getattr(self.observer, '_deleted', False)
@@ -134,15 +134,15 @@
 
     MIN_SLEEP_SECONDS = 10  # Allow lock to be taken in concurrent cases.
 
     period: timedelta = attr.ib(default=timedelta(seconds=60))
     storage: Optional[BaseStorage] = attr.ib(default=None)
     iteration_mode: IterationMode = attr.ib(default=IterationMode.FIRST_COMPLETED)
     name: Optional[str] = attr.ib(default=None, kw_only=True)
-    _observers: Dict[int, BaseObserver] = attr.ib(factory=dict, init=False)
+    _observers: Dict[Tuple, BaseObserver] = attr.ib(factory=dict, init=False)
     _got_sigint: bool = attr.ib(default=False, init=False)
 
     @contextmanager
     def _lock(self, key: str) -> ContextManager[Any]:
         if self.storage:
             with self.storage.lock(key) as lock:
                 yield lock
@@ -175,15 +175,15 @@
                 logger.info('Cleanup storage %s with keys count: %d', type(self.storage).__name__, len(keys))
                 self.storage.cleanup(pipeline_key, keys, lock)
             except Exception:
                 logger.exception('Got an exception while running cleanup at: %s', type(self.storage).__name__)
 
     def _get_unique_key(self) -> Tuple:
         return (self.__class__.__name__, self.name or '', tuple(sorted(
-            observer._get_unique_key()
+            observer.get_unique_key()
             for observer in self._observers.values()
         )))
 
     def register(self, observer: BaseObserver) -> BaseObserver:
         """Register given observer.
 
         Args:
@@ -201,15 +201,19 @@
             ...
 
             One-line version.
 
             >>> toloka_loop.register(SomeObserver(pool_id='123')).do_some_preparations(...)
             ...
         """
-        self._observers[id(observer)] = observer
+        observer_key = observer.get_unique_key()
+        if observer_key in self._observers:
+            raise ValueError(f'Failed to register observer to pipeline: observer with key {observer_key} is already '
+                             f'registered')
+        self._observers[observer_key] = observer
         return observer
 
     def observers_iter(self) -> Iterator[BaseObserver]:
         """Iterate over registered observers.
 
         Returns:
             An iterator over all registered observers except deleted ones.
@@ -263,22 +267,30 @@
             pending: currently not running workers
         """
         pipeline_key: str = attr.ib()
         workers: Dict[_Worker, None] = attr.ib(on_setattr=attr.setters.frozen, factory=lambda: {})
         waiting: Dict[_Worker, asyncio.Task] = attr.ib(on_setattr=attr.setters.frozen, factory=lambda: {})
         pending: Dict[_Worker, datetime] = attr.ib(on_setattr=attr.setters.frozen, factory=lambda: {})
 
-        def add_new_observers(self, new_observers: Iterable[BaseObserver]) -> None:
+        def update_observers(self, pipeline: 'Pipeline'):
+            known_observers_keys = {worker.observer.get_unique_key() for worker in self.workers.keys()}
+            new_observers = [
+                observer
+                for observer in pipeline.observers_iter()
+                if observer.get_unique_key() not in known_observers_keys
+            ]
+            if len(new_observers) > 0:
+                logger.info(f'New observers found in quantity: {len(new_observers)}')
             new_workers = _OrderedSet(_Worker._from_observer(observer) for observer in new_observers)
             self.workers.update(new_workers)
             self.pending.update({worker: datetime.min for worker in new_workers})
 
     def _create_state(self):
         state = Pipeline.RunState(pipeline_key=str(self._get_unique_key()))
-        state.add_new_observers(self.observers_iter())
+        state.update_observers(self)
         with self._lock(state.pipeline_key):
             # Get checkpoint from the storage.
             self._storage_load(state.pipeline_key, state.workers)
         return state
 
     async def run_manually(self) -> AsyncGenerator['Pipeline.RunState', None]:
         if not self._observers:
@@ -313,15 +325,15 @@
                         still_pending[worker] = time_to_start
                 state.pending.clear()
                 state.pending.update(still_pending)
 
                 if to_remove:
                     logger.info('Found observers to remove count: %d', len(to_remove))
                     for worker in to_remove:
-                        self._observers.pop(id(worker.observer))
+                        self._observers.pop(worker.observer.get_unique_key())
                         state.workers.pop(worker)
 
                 if not self._got_sigint:
                     logger.info('Observers to run count: %d', len(to_start))
                     for worker in to_start:
                         task = asyncio.get_event_loop().create_task(worker())
                         task.worker = worker
@@ -360,30 +372,23 @@
                     if self._got_sigint:
                         raise KeyboardInterrupt
                     if _Worker._no_one_should_resume(state.workers):  # If stop condition at all workers, run in check_mode.
                         check_mode = True
                 else:
                     check_mode = False
 
-            self._update_observers(state)
+            state.update_observers(self)
 
             if self._got_sigint:
                 logger.warning('Execute next iteration immediately due to SIGINT handling')
             elif check_mode:
                 logger.warning('Execute next iteration immediately due to check mode handling')
             else:
                 yield state
 
-    def _update_observers(self, state):
-        new_observers_ids = self._observers.keys() - {id(worker.observer) for worker in state.workers}
-        if new_observers_ids:
-            logger.info('New observers found in quantity: %d', len(new_observers_ids))
-            new_observers = (self._observers[id_] for id_ in new_observers_ids)
-            state.add_new_observers(new_observers)
-
     async def _initialize_run(self):
         state = self._create_state()
         loop = asyncio.get_event_loop()
         loop.add_signal_handler(signal.SIGINT, self._sigint_handler, loop, state.waiting)
         self._got_sigint = False
         return state
```

### Comparing `toloka-kit-1.1.4/src/streaming/pipeline.pyi` & `toloka-kit-1.2.0/src/streaming/pipeline.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
         Attributes:
             workers: all known workers
             waiting: currently running workers
             pending: currently not running workers
         """
 
-        def add_new_observers(self, new_observers: typing.Iterable[toloka.streaming.observer.BaseObserver]) -> None: ...
+        def update_observers(self, pipeline: 'Pipeline'): ...
 
         def __init__(
             self,
             pipeline_key: str,
             workers: typing.Dict[_Worker, None] = ...,
             waiting: typing.Dict[_Worker, asyncio.Task] = ...,
             pending: typing.Dict[_Worker, datetime.datetime] = ...
@@ -179,9 +179,9 @@
         """
         ...
 
     period: datetime.timedelta
     storage: typing.Optional[toloka.streaming.storage.BaseStorage]
     iteration_mode: IterationMode
     name: typing.Optional[str]
-    _observers: typing.Dict[int, toloka.streaming.observer.BaseObserver]
+    _observers: typing.Dict[typing.Tuple, toloka.streaming.observer.BaseObserver]
     _got_sigint: bool
```

### Comparing `toloka-kit-1.1.4/src/streaming/storage.py` & `toloka-kit-1.2.0/src/streaming/storage.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/streaming/storage.pyi` & `toloka-kit-1.2.0/src/streaming/storage.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 __all__ = [
     'BaseStorage',
     'JSONLocalStorage',
     'S3Storage',
 ]
 import toloka.streaming.locker
 import typing
+import typing_extensions
 
 
 Pickleable = typing.TypeVar('Pickleable')
 
 class BaseStorage:
     def lock(self, key: str) -> typing.ContextManager[typing.Any]: ...
 
@@ -105,33 +106,31 @@
         """
         ...
 
     locker: typing.Optional[toloka.streaming.locker.BaseLocker]
     dirname: str
 
 
-class ObjectSummaryCollection(typing.Protocol):
+class ObjectSummaryCollection(typing_extensions.Protocol):
     def filter(
         self,
         Prefix,
         **kwargs
     ) -> 'ObjectSummaryCollection': ...
 
     def delete(self, **kwargs): ...
 
-    def __subclasshook__(other): ...
-
     def __init__(
         self,
         *args,
         **kwargs
     ): ...
 
 
-class BucketType(typing.Protocol):
+class BucketType(typing_extensions.Protocol):
     def upload_fileobj(
         self,
         Fileobj,
         Key,
         ExtraArgs=None,
         **kwargs
     ): ...
@@ -139,16 +138,14 @@
     def download_fileobj(
         self,
         Fileobj,
         ExtraArgs=None,
         **kwargs
     ): ...
 
-    def __subclasshook__(other): ...
-
     def __init__(
         self,
         *args,
         **kwargs
     ): ...
 
     objects: ObjectSummaryCollection
```

### Comparing `toloka-kit-1.1.4/src/util/__init__.py` & `toloka-kit-1.2.0/src/util/__init__.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/util/_codegen.py` & `toloka-kit-1.2.0/src/util/_codegen.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 __all__: list = [
     'attribute',
     'fix_attrs_converters',
     'universal_decorator',
     'expand'
 ]
+
+import datetime
 import functools
 import inspect
 import linecache
 import uuid
 from inspect import isclass, signature, Signature, Parameter, BoundArguments
 from textwrap import dedent, indent
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type
@@ -249,15 +251,20 @@
         ''')
 
     expanded_func = _compile_function(
         f'{func.__name__}_expanded_by_{arg_name}',
         func_sig.replace(parameters=new_params),
         function_body,
         inspect.iscoroutinefunction(func),
-        {arg_type.__name__: arg_type, 'func': func, 'NOTHING': attr.NOTHING}
+        {
+            arg_type.__name__: arg_type,
+            'func': func,
+            'NOTHING': attr.NOTHING,
+            'datetime': datetime,
+        }
     )
     expanded_func.__doc__ = func.__doc__
     return expanded_func
 
 
 def _check_arg_type_compatibility(func_sig: Signature, arg_name: str, arg_type: Optional[Type], bound: BoundArguments) -> Tuple[bool, Optional[str]]:
     arg_param: Parameter = func_sig.parameters[arg_name]
```

### Comparing `toloka-kit-1.1.4/src/util/_codegen.pyi` & `toloka-kit-1.2.0/src/util/_codegen.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/util/_docstrings.py` & `toloka-kit-1.2.0/src/util/_docstrings.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/util/_docstrings.pyi` & `toloka-kit-1.2.0/src/util/_docstrings.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/util/_extendable_enum.py` & `toloka-kit-1.2.0/src/util/_extendable_enum.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/util/_extendable_enum.pyi` & `toloka-kit-1.2.0/src/util/_extendable_enum.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/util/_managing_headers.py` & `toloka-kit-1.2.0/src/util/_managing_headers.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/util/_managing_headers.pyi` & `toloka-kit-1.2.0/src/util/_managing_headers.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/util/async_utils.py` & `toloka-kit-1.2.0/src/util/async_utils.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/util/async_utils.pyi` & `toloka-kit-1.2.0/src/util/async_utils.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/src/util/stored.py` & `toloka-kit-1.2.0/src/util/stored.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/tests/test_aggregated_solution.py` & `toloka-kit-1.2.0/tests/test_aggregated_solution.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/tests/test_analytics_request.py` & `toloka-kit-1.2.0/tests/test_analytics_request.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/tests/test_assignment.py` & `toloka-kit-1.2.0/tests/test_assignment.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/tests/test_attachment.py` & `toloka-kit-1.2.0/tests/test_attachment.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/tests/test_client.py` & `toloka-kit-1.2.0/tests/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import copy
-from decimal import Decimal
-
 import pickle
+import ssl
+from decimal import Decimal
 
 import httpx
 import pytest
 import simplejson
-import ssl
+import toloka.client as client
 from pytest_lazyfixture import lazy_fixture
-
 from toloka.client import TolokaClient
-import toloka.client as client
 
-from .testutils.util_functions import check_headers
 from .conftest import SyncOverAsyncTolokaClient
+from .testutils.util_functions import check_headers
 
 
 @pytest.fixture
 def random_url():
     return 'https://testing.toloka.yandex.ru'
```

### Comparing `toloka-kit-1.1.4/tests/test_deep_clone_project.py` & `toloka-kit-1.2.0/tests/test_deep_clone_project.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/tests/test_exceptions.py` & `toloka-kit-1.2.0/tests/test_exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,7 +46,21 @@
     {
         "filter.and.0.value": {
             "code": "SIMPLE_VALUE_EXPECTED",
             "message": "Value must not be an object or an array"
         }
     }
     request id: asd123. It needs to be specified when contacting support.''')
+
+
+def test_api_error_with_bad_payload_falls_back_to_printing_raw_response():
+    bad_payload = object()
+    assert str(ApiError(status_code=500, request_id='asd123', code='INTERNAL_ERROR', payload=bad_payload)) == dedent(
+        f'''\
+        You have got a(n) ApiError with http status code: 500
+        Code of error: INTERNAL_ERROR
+        Error details: None
+        Additional information about the error:
+        failed to parse payload as JSON! Falling back to raw representation:
+        {str(bad_payload)}
+        request id: asd123. It needs to be specified when contacting support.'''
+    )
```

### Comparing `toloka-kit-1.1.4/tests/test_filter.py` & `toloka-kit-1.2.0/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/tests/test_message_thread.py` & `toloka-kit-1.2.0/tests/test_message_thread.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/tests/test_operation.py` & `toloka-kit-1.2.0/tests/test_operation.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/tests/test_operation_log.py` & `toloka-kit-1.2.0/tests/test_operation_log.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/tests/test_project.py` & `toloka-kit-1.2.0/tests/test_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,15 +306,15 @@
 
     respx_mock.post(f'{toloka_url}/projects').mock(side_effect=project)
 
     project = client.structure(simple_project_map, client.project.Project)
     with caplog.at_level(logging.INFO):
         caplog.clear()
         result = toloka_client.create_project(project)
-        assert caplog.record_tuples == [(
+        assert [log for log in caplog.record_tuples if log[0] == 'toloka.client'] == [(
             'toloka.client', logging.INFO,
             'A new project with ID "10" has been created. Link to open in web interface: https://sandbox.toloka.yandex.com/requester/project/10'
         )]
         assert project == result
 
 
 def test_create_project_check_validation_errors(respx_mock, toloka_client, toloka_url):
```

### Comparing `toloka-kit-1.1.4/tests/test_requester.py` & `toloka-kit-1.2.0/tests/test_requester.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/tests/test_serialization.py` & `toloka-kit-1.2.0/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/tests/test_skill.py` & `toloka-kit-1.2.0/tests/test_skill.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
     respx_mock.post(f'{toloka_url}/skills').mock(side_effect=create_skill)
 
     # Request object syntax
     with caplog.at_level(logging.INFO):
         caplog.clear()
         result = toloka_client.create_skill(client.Skill(**skill_header))
-        assert caplog.record_tuples == [(
+        assert [log for log in caplog.record_tuples if log[0] == 'toloka.client'] == [(
             'toloka.client',
             logging.INFO,
             'A new skill with ID "21" has been created. Link to open in web interface: https://sandbox.toloka.yandex.com/requester/quality/skill/21'
         )]
         assert skill_sample == client.unstructure(result)
 
     # Expanded syntax
```

### Comparing `toloka-kit-1.1.4/tests/test_task.py` & `toloka-kit-1.2.0/tests/test_training.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,819 +1,609 @@
 import datetime
-import re
+import logging
 from operator import itemgetter
-from uuid import uuid4
 
 import httpx
 import pytest
 import simplejson
-import simplejson as json
 import toloka.client as client
 from httpx import QueryParams
-from toloka.client.exceptions import IncorrectActionsApiError
 
 from .testutils.util_functions import check_headers
 
 
 @pytest.fixture
-def task_map():
+def training_map():
     return {
-        'pool_id': '21',
-        'input_values': {'image': 'http://images.com/1.png'},
-        'known_solutions': [
-            {
-                'output_values': {'color': 'white'},
-                'correctness_weight': 1.0,
-            },
-            {
-                'output_values': {'color': 'gray'},
-                'correctness_weight': 0.71,
-            },
-        ],
-        'message_on_unknown_solution': 'Main color is white',
-        'baseline_solutions': [
-            {
-                'output_values': {'color': 'white'},
-                'confidence_weight': 1.0,
-            },
-            {
-                'output_values': {'color': 'gray'},
-                'confidence_weight': 0.71,
-            },
-        ],
-        'overlap': 3,
-        'infinite_overlap': False,
-        'remaining_overlap': 3,
-        'unavailable_for': ['user-1id'],
-        'reserved_for': ['user-2id'],
-        'traits_all_of': ['trait-1'],
-        'traits_any_of': ['trait-2'],
-        'traits_none_of_any': ['trait-3'],
+        'project_id': '10',
+        'private_name': 'training_v12_231',
+        'may_contain_adult_content': True,
+        'mix_tasks_in_creation_order': True,
+        'shuffle_tasks_in_task_suite': True,
+        'training_tasks_in_task_suite_count': 3,
+        'task_suites_required_to_pass': 5,
+        'retry_training_after_days': 1,
+        'inherited_instructions': True,
+        'metadata': {'testKey': ['testValue']},
+        'assignment_max_duration_seconds': 600,
+        'public_instructions': 'text'
     }
 
 
-def test_task_from_json(task_map):
-    task = client.structure(task_map, client.task.Task)
-    task_json = json.dumps(task_map, use_decimal=True, ensure_ascii=False)
-    task_from_json = client.task.Task.from_json(task_json)
-    assert task == task_from_json
+@pytest.fixture
+def training_map_with_readonly(training_map):
+    return {
+        **training_map,
+        'id': '21',
+        'owner': {'id': 'requester-1', 'myself': True, 'company_id': '1'},
+        'created': '2015-12-16T12:55:01',
+        'last_started': '2015-12-17T08:00:01',
+        'last_stopped': '2015-12-18T08:00:01',
+        'last_close_reason': 'MANUAL',
+        'status': 'CLOSED',
+    }
 
 
-def test_task_to_json(task_map):
-    task = client.structure(task_map, client.task.Task)
-    task_json = task.to_json()
-    task_json_basic = json.dumps(task_map, use_decimal=True, ensure_ascii=False)
-    assert json.loads(task_json) == json.loads(task_json_basic)
+@pytest.fixture
+def open_training_map_with_readonly(training_map_with_readonly):
+    return {
+        **training_map_with_readonly,
+        'status': 'OPEN'
+    }
 
 
 @pytest.fixture
-def task_map_with_readonly(task_map):
-    return {**task_map, 'created': '2016-10-09T11:42:01'}
+def archived_training_map_with_readonly(training_map_with_readonly):
+    return {
+        **training_map_with_readonly,
+        'status': 'ARCHIVED'
+    }
 
 
-def test_create_task(respx_mock, toloka_client, toloka_url, task_map, task_map_with_readonly):
+def test_find_trainings(respx_mock, toloka_client, toloka_url, training_map_with_readonly):
+    raw_result = {'items': [training_map_with_readonly], 'has_more': False}
 
-    def tasks(request):
+    def trainings(request):
         expected_headers = {
             'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
-            'X-Top-Level-Method': 'create_task',
-            'X-Low-Level-Method': 'create_task',
+            'X-Top-Level-Method': 'find_trainings',
+            'X-Low-Level-Method': 'find_trainings',
         }
         check_headers(request, expected_headers)
 
-        assert task_map == simplejson.loads(request.content)
-        return httpx.Response(json=task_map_with_readonly, status_code=201)
+        assert QueryParams(
+            project_id='10',
+            id_gt='20',
+            last_started_lt='2016-03-23T12:59:00',
+            sort='created,-id',
+        ) == request.url.params
+        return httpx.Response(json=raw_result, status_code=200)
+
+    respx_mock.get(f'{toloka_url}/trainings').mock(side_effect=trainings)
+
+    # Request object syntax
+    request = client.search_requests.TrainingSearchRequest(
+        project_id='10',
+        id_gt='20',
+        last_started_lt=datetime.datetime(2016, 3, 23, 12, 59, 0, tzinfo=datetime.timezone.utc),
+    )
+    sort = client.search_requests.TrainingSortItems(['created', '-id'])
+    result = toloka_client.find_trainings(request, sort=sort)
+    assert raw_result == client.unstructure(result)
 
-    respx_mock.post(f'{toloka_url}/tasks').mock(side_effect=tasks)
-    result = toloka_client.create_task(client.structure(task_map, client.task.Task))
-    assert task_map_with_readonly == client.unstructure(result)
+    # Expanded syntax
+    result = toloka_client.find_trainings(
+        project_id='10',
+        id_gt='20',
+        last_started_lt=datetime.datetime(2016, 3, 23, 12, 59, 0, tzinfo=datetime.timezone.utc),
+        sort=['created', '-id'],
+    )
+    assert raw_result == client.unstructure(result)
 
 
-def test_create_tasks_with_error(respx_mock, toloka_client, toloka_url, task_map, task_map_with_readonly):
-    tasks_map = [task_map, {'pool_id': '21', 'input_values': {'image': None}}]
-    raw_result = {
-        'items': {'0': task_map_with_readonly},
-        'validation_errors': {
-            '1': {'input_values.image': {'code': 'VALUE_REQUIRED', 'message': 'May not be null'}},
-        }
-    }
+def test_get_trainings(respx_mock, toloka_client, toloka_url, training_map_with_readonly):
+    trainings = [dict(training_map_with_readonly, id=str(i)) for i in range(100)]
+    trainings.sort(key=itemgetter('id'))
+    expected_trainings = [training for training in trainings if training['id'] > '20']
 
-    def tasks(request):
+    def get_trainings(request):
         expected_headers = {
             'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
-            'X-Top-Level-Method': 'create_tasks',
-            'X-Low-Level-Method': 'create_tasks',
+            'X-Top-Level-Method': 'get_trainings',
+            'X-Low-Level-Method': 'find_trainings',
         }
         check_headers(request, expected_headers)
 
+        params = request.url.params
+        id_gt = params['id_gt']
+        params = params.remove('id_gt')
         assert QueryParams(
-            allow_defaults='true', async_mode='false', operation_id=request.url.params['operation_id']
-        ) == request.url.params
-        assert tasks_map == simplejson.loads(request.content)
-        return httpx.Response(json=raw_result, status_code=201)
+            project_id='10',
+            last_started_lt='2016-03-23T12:59:00',
+            sort='id',
+        ) == params
 
-    respx_mock.post(f'{toloka_url}/tasks').mock(side_effect=tasks)
+        items = [training for training in trainings if id_gt is None or training['id'] > id_gt][:3]
+        return httpx.Response(json={'items': items, 'has_more': items[-1]['id'] != trainings[-1]['id']}, status_code=200)
 
-    # raise ValueError(client.unstructure(client.task.CreateTasksParameters(allow_defaults=True)))
+    respx_mock.get(f'{toloka_url}/trainings').mock(side_effect=get_trainings)
 
     # Request object syntax
-    result = toloka_client.create_tasks(
-        [client.structure(task, client.task.Task) for task in tasks_map],
-        client.task.CreateTasksParameters(allow_defaults=True, async_mode=False)
+    request = client.search_requests.TrainingSearchRequest(
+        project_id='10',
+        id_gt='20',
+        last_started_lt=datetime.datetime(2016, 3, 23, 12, 59, 0, tzinfo=datetime.timezone.utc),
     )
-    assert raw_result == client.unstructure(result)
+    result = toloka_client.get_trainings(request)
+    assert expected_trainings == client.unstructure(list(result))
 
     # Expanded syntax
-    result = toloka_client.create_tasks(
-        [client.structure(task, client.task.Task) for task in tasks_map],
-        allow_defaults=True,
-        async_mode=False,
+    result = toloka_client.get_trainings(
+        project_id='10',
+        id_gt='20',
+        last_started_lt=datetime.datetime(2016, 3, 23, 12, 59, 0, tzinfo=datetime.timezone.utc),
     )
-    assert raw_result == client.unstructure(result)
+    assert expected_trainings == client.unstructure(list(result))
 
 
-@pytest.fixture
-def tasks_map():
-    return [
-        {'pool_id': '21', 'input_values': {'image': 'http://images.com/1.png'}},
-        {'pool_id': '22', 'input_values': {'image': 'http://images.com/2.png'}},
-        {'pool_id': '22', 'input_values': {'imagis': 'http://images.com/3.png'}}
-    ]
-
+def test_get_training(respx_mock, toloka_client, toloka_url, training_map_with_readonly):
 
-@pytest.fixture
-def operation_running_map():
-    return {
-        'id': '281073ea-ab34-416e-a028-47421ff1b166',
-        'type': 'TASK.BATCH_CREATE',
-        'status': 'RUNNING',
-        'submitted': '2016-10-10T20:33:01',
-        'started': '2016-10-10T23:33:00',
-        'parameters': {'skip_invalid_items': True, 'allow_defaults': True, 'open_pool': True},
-        'details': {'items_count': 2},
-    }
-
-
-@pytest.fixture
-def operation_success_map(operation_running_map):
-    return dict(operation_running_map, status='SUCCESS')
-
-
-@pytest.fixture
-def create_tasks_log():
-    return [
-        {
-            'input': {
-                'input_values': {
-                    'image': 'http://images.com/1.png'
-                },
-                'pool_id': '21',
-                '__client_uuid': 'e3e70682c2094cac629f6fbed82c07cd',
-            },
-            'output': {
-                'task_id': '00014495f0--60213f7c25a8b84e2ffb7a2c'
-            },
-            'success': True,
-            'type': 'TASK_CREATE'
-        },
-        {
-            'input': {
-                'input_values': {
-                    'image': 'http://images.com/2.png'
-                },
-                'pool_id': '22',
-                '__client_uuid': 'f728b4fa42485e3a0a5d2f346baa9455',
-            },
-            'output': {
-                'task_id': '00014495f0--60213f7c25a8b84e2ffb7a3b'
-            },
-            'success': True,
-            'type': 'TASK_CREATE'
-        },
-        {
-            'input': {
-                'input_values': {
-                    'image': 'http://images.com/2.png'
-                },
-                'pool_id': '22',
-                '__client_uuid': 'eb1167b367a9c3787c65c1e582e2e662',
-            },
-            'output': {
-                'input_values.image': {
-                    'code': 'VALUE_REQUIRED',
-                    'message': 'Value must be present and not equal to null'
-                },
-                'input_values.imagis': {
-                    'code': 'VALUE_NOT_ALLOWED',
-                    'message': 'Unknown field name'
-                }
-            },
-            'success': False,
-            'type': 'TASK_VALIDATE'
-        },
-        {
-            'input': {
-                'pool_id': 22
-            },
-            'output': {
-                'code': 'EMPTY_POOL',
-                'message': 'Pool contains no tasks. Operation is not allowed',
-                'request_id': 'ao_c8e4cb72-8d4b-4894-bc6e-65a403e6337e',
-            },
-            'success': False,
-            'type': 'POOL_OPEN',
-        },
-    ]
-
-
-@pytest.fixture
-def created_tasks_21_map():
-    return [
-        {
-            'id': '00014495f0--60213f7c25a8b84e2ffb7a2c',
-            'pool_id': '21',
-            'input_values': {'image': 'http://images.com/1.png'},
-            'overlap': 1,
-            'infinite_overlap': False,
-            'remaining_overlap': 1,
-        }
-    ]
-
-
-@pytest.fixture
-def created_tasks_22_map():
-    return [
-        {
-            'id': '00014495f0--60213f7c25a8b84e2ffb7a3b',
-            'pool_id': '22',
-            'input_values': {'image': 'http://images.com/2.png'},
-            'overlap': 1,
-            'infinite_overlap': False,
-            'remaining_overlap': 1,
-        }
-    ]
-
-
-@pytest.fixture
-def task_create_result_map():
-    return {
-        'items': {
-            '0': {
-                'input_values': {'image': 'http://images.com/1.png'},
-                'id': '00014495f0--60213f7c25a8b84e2ffb7a2c',
-                'infinite_overlap': False,
-                'overlap': 1,
-                'pool_id': '21',
-                'remaining_overlap': 1
-            },
-            '1': {
-                'input_values': {'image': 'http://images.com/2.png'},
-                'id': '00014495f0--60213f7c25a8b84e2ffb7a3b',
-                'infinite_overlap': False,
-                'overlap': 1,
-                'pool_id': '22',
-                'remaining_overlap': 1
-            },
-        },
-        'validation_errors':
-        {
-            '2': {
-                'input_values.image': {
-                    'code': 'VALUE_REQUIRED',
-                    'message': 'Value must be present and not equal to null'
-                },
-                'input_values.imagis': {
-                    'code': 'VALUE_NOT_ALLOWED',
-                    'message': 'Unknown field name'
-                },
-            },
-        }
-    }
-
-
-def test_create_tasks_sync_through_async(
-    respx_mock, toloka_client, toloka_url, no_uuid_random,
-    tasks_map, operation_running_map, operation_success_map,
-    create_tasks_log, created_tasks_21_map, created_tasks_22_map,
-    task_create_result_map
-):
-
-    def check_tasks(request):
+    def get_training(request):
         expected_headers = {
             'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
-            'X-Top-Level-Method': 'create_tasks',
-            'X-Low-Level-Method': 'create_tasks',
+            'X-Top-Level-Method': 'get_training',
+            'X-Low-Level-Method': 'get_training',
         }
         check_headers(request, expected_headers)
 
-        assert QueryParams(
-            operation_id='281073ea-ab34-416e-a028-47421ff1b166',
-            skip_invalid_items='true',
-            allow_defaults='true',
-            open_pool='true',
-            async_mode='true',
-        ) == request.url.params
-        imcoming_tasks = []
-        for t in simplejson.loads(request.content):
-            assert '__client_uuid' in t
-            t.pop('__client_uuid')
-            imcoming_tasks.append(t)
-        assert tasks_map == imcoming_tasks
-        return httpx.Response(json=operation_running_map, status_code=201)
-
-    def operation_success(request):
-        expected_headers = {
-            'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
-            'X-Top-Level-Method': 'create_tasks',
-            'X-Low-Level-Method': 'get_operation',
-        }
-        check_headers(request, expected_headers)
+        return httpx.Response(json=training_map_with_readonly, status_code=200)
 
-        return httpx.Response(json=operation_success_map, status_code=201)
+    respx_mock.get(f'{toloka_url}/trainings/21').mock(side_effect=get_training)
+    assert training_map_with_readonly == client.unstructure(toloka_client.get_training('21'))
 
-    def tasks_log(request):
-        expected_headers = {
-            'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
-            'X-Top-Level-Method': 'create_tasks',
-            'X-Low-Level-Method': 'get_operation_log',
-        }
-        check_headers(request, expected_headers)
 
-        return httpx.Response(json=create_tasks_log, status_code=201)
+def test_create_training(respx_mock, toloka_client, toloka_url, training_map, training_map_with_readonly, caplog):
 
-    def return_tasks_by_pool(request):
+    def trainings(request):
         expected_headers = {
             'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
-            'X-Top-Level-Method': 'create_tasks',
-            'X-Low-Level-Method': 'find_tasks',
+            'X-Top-Level-Method': 'create_training',
+            'X-Low-Level-Method': 'create_training',
         }
         check_headers(request, expected_headers)
 
-        params = request.url.params
-        res_map = created_tasks_21_map if params['pool_id'] == '21' else created_tasks_22_map
-        return httpx.Response(json={'items': res_map, 'has_more': False}, status_code=201)
-
-    # mocks
-    # create_task -> operation
-    respx_mock.post(f'{toloka_url}/tasks').mock(side_effect=check_tasks,)
-    # wait_operation -> operation Success
-    respx_mock.get(f'{toloka_url}/operations/{operation_running_map["id"]}').mock(side_effect=operation_success)
-    # get_log -> log_res
-    respx_mock.get(f'{toloka_url}/operations/{operation_running_map["id"]}/log').mock(side_effect=tasks_log)
-    # get tasks from pools (2 calls - for each pool)
-    respx_mock.get(f'{toloka_url}/tasks').mock(side_effect=return_tasks_by_pool)
+        assert training_map == simplejson.loads(request.content)
+        return httpx.Response(json=training_map_with_readonly, status_code=201)
 
-    # Expanded syntax
-    result = toloka_client.create_tasks(
-        [client.structure(task, client.task.Task) for task in tasks_map],
-        operation_id='281073ea-ab34-416e-a028-47421ff1b166',
-        skip_invalid_items=True,
-        allow_defaults=True,
-        open_pool=True,
-    )
-    assert task_create_result_map == client.unstructure(result)
+    respx_mock.post(f'{toloka_url}/trainings').mock(side_effect=trainings)
+    training = client.structure(training_map, client.training.Training)
+    with caplog.at_level(logging.INFO):
+        caplog.clear()
+        result = toloka_client.create_training(training)
+        assert [log for log in caplog.record_tuples if log[0] == 'toloka.client'] == [(
+            'toloka.client',
+            logging.INFO,
+            'A new training with ID "21" has been created. Link to open in web interface: https://sandbox.toloka.yandex.com/requester/project/10/training/21'
+        )]
+        assert training_map_with_readonly == client.unstructure(result)
 
 
-def test_create_tasks_sync(respx_mock, toloka_client, toloka_url, tasks_map, task_create_result_map):
+def test_update_training(respx_mock, toloka_client, toloka_url, training_map_with_readonly):
+    updated_training = {
+        **training_map_with_readonly,
+        'private_name': 'updated name',
+    }
 
-    def task(request):
+    def trainings(request):
         expected_headers = {
             'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
-            'X-Top-Level-Method': 'create_tasks',
-            'X-Low-Level-Method': 'create_tasks',
+            'X-Top-Level-Method': 'update_training',
+            'X-Low-Level-Method': 'update_training',
         }
         check_headers(request, expected_headers)
 
-        return httpx.Response(json=task_create_result_map, status_code=201)
+        assert updated_training == simplejson.loads(request.content)
+        return httpx.Response(json=updated_training, status_code=200)
 
-    respx_mock.post(f'{toloka_url}/tasks').mock(side_effect=task)
+    respx_mock.put(f'{toloka_url}/trainings/21').mock(side_effect=trainings)
+    result = toloka_client.update_training('21', client.structure(updated_training, client.training.Training))
+    assert updated_training == client.unstructure(result)
 
-    # Expanded syntax
-    result = toloka_client.create_tasks(
-        [client.structure(task, client.task.Task) for task in tasks_map],
-        operation_id='281073ea-ab34-416e-a028-47421ff1b166',
-        skip_invalid_items=True,
-        allow_defaults=True,
-        open_pool=True,
-        async_mode=False,
-    )
-    assert task_create_result_map == client.unstructure(result)
+
+@pytest.fixture
+def open_operation_map():
+    return {
+        'id': 'open-training-op1id',
+        'type': 'TRAINING.OPEN',
+        'status': 'RUNNING',
+        'submitted': '2016-03-07T15:47:00',
+        'started': '2016-03-07T15:47:21',
+        'parameters': {'training_id': '21'},
+    }
 
 
 @pytest.fixture
-def create_tasks_operation_map():
+def complete_open_operation_map(open_operation_map):
     return {
-        'id': '281073ea-ab34-416e-a028-47421ff1b166',
-        'type': 'TASK.BATCH_CREATE',
+        **open_operation_map,
         'status': 'SUCCESS',
-        'submitted': '2016-10-10T20:33:01',
-        'started': '2016-10-10T23:33:00',
-        'parameters': {'skip_invalid_items': True, 'allow_defaults': True, 'open_pool': True},
-        'details': {'items_count': 2},
+        'finished': '2016-03-07T15:48:03',
     }
 
 
-def test_create_tasks_async(respx_mock, toloka_client, toloka_url, tasks_map, create_tasks_operation_map):
+def test_open_training_async(respx_mock, toloka_client, toloka_url, open_operation_map, complete_open_operation_map):
 
-    def tasks(request):
+    def open_operation(request):
         expected_headers = {
             'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
-            'X-Top-Level-Method': 'create_tasks_async',
-            'X-Low-Level-Method': 'create_tasks_async',
+            'X-Top-Level-Method': 'open_training_async',
+            'X-Low-Level-Method': 'open_training_async',
         }
         check_headers(request, expected_headers)
 
-        assert QueryParams(
-            operation_id='281073ea-ab34-416e-a028-47421ff1b166',
-            skip_invalid_items='true',
-            allow_defaults='true',
-            open_pool='true',
-            async_mode='true',
-        ) == request.url.params
-        assert tasks_map == simplejson.loads(request.content)
-        return httpx.Response(json=create_tasks_operation_map, status_code=201)
+        return httpx.Response(json=open_operation_map, status_code=202)
 
-    respx_mock.post(f'{toloka_url}/tasks').mock(side_effect=tasks)
+    def complete_open_operation(request):
+        expected_headers = {
+            'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
+            'X-Top-Level-Method': 'wait_operation',
+            'X-Low-Level-Method': 'get_operation',
+        }
+        check_headers(request, expected_headers)
 
-    # Request object syntax
-    result = toloka_client.create_tasks_async(
-        [client.structure(task, client.task.Task) for task in tasks_map],
-        client.task.CreateTasksParameters(
-            operation_id='281073ea-ab34-416e-a028-47421ff1b166',
-            skip_invalid_items=True,
-            allow_defaults=True,
-            open_pool=True,
-        )
-    )
-    assert create_tasks_operation_map == client.unstructure(result)
+        return httpx.Response(json=complete_open_operation_map, status_code=200)
 
-    # Expanded syntax
-    result = toloka_client.create_tasks_async(
-        [client.structure(task, client.task.Task) for task in tasks_map],
-        operation_id='281073ea-ab34-416e-a028-47421ff1b166',
-        skip_invalid_items=True,
-        allow_defaults=True,
-        open_pool=True,
-    )
-    assert create_tasks_operation_map == client.unstructure(result)
+    respx_mock.post(f'{toloka_url}/trainings/21/open').mock(side_effect=open_operation)
+    respx_mock.get(f'{toloka_url}/operations/{open_operation_map["id"]}').mock(side_effect=complete_open_operation)
 
+    operation = toloka_client.open_training_async('21')
+    assert open_operation_map == client.unstructure(operation)
 
-def test_create_tasks_retry_sync_through_async(
-    respx_mock, toloka_client, toloka_url, tasks_map, task_create_result_map, operation_success_map, create_tasks_log,
-    no_uuid_random, created_tasks_21_map, created_tasks_22_map,
-):
-    requests_count = 0
-    first_request_op_id = None
-
-    def tasks(request):
-        nonlocal requests_count
-        nonlocal first_request_op_id
-
-        requests_count += 1
-        if requests_count == 1:
-            first_request_op_id = request.url.params['operation_id']
-            return httpx.Response(status_code=500)
-
-        assert request.url.params['operation_id'] == first_request_op_id
-        unstructured_error = client.unstructure(IncorrectActionsApiError(
-            code='OPERATION_ALREADY_EXISTS',
-        ))
-        del unstructured_error['status_code']
-
-        return httpx.Response(
-            json=unstructured_error,
-            status_code=409
-        )
+    complete_operation = toloka_client.wait_operation(operation)
+    assert complete_open_operation_map == client.unstructure(complete_operation)
 
-    def tasks_log(request):
-        return httpx.Response(json=create_tasks_log, status_code=201)
 
-    def return_tasks_by_pool(request):
-        params = request.url.params
-        res_map = created_tasks_21_map if params['pool_id'] == '21' else created_tasks_22_map
-        return httpx.Response(json={'items': res_map, 'has_more': False}, status_code=201)
+def test_open_training(respx_mock, toloka_client, toloka_url,
+                       open_operation_map, complete_open_operation_map, training_map_with_readonly):
 
-    respx_mock.get(
-        url__regex=rf'{toloka_url}/operations/.*(?<!log)$'
-    ).mock(httpx.Response(json=operation_success_map, status_code=200))
-    respx_mock.post(f'{toloka_url}/tasks').mock(side_effect=tasks)
-    respx_mock.get(re.compile(rf'{toloka_url}/operations/.*/log')).mock(side_effect=tasks_log)
-    respx_mock.get(f'{toloka_url}/tasks').mock(side_effect=return_tasks_by_pool)
+    def open_operation(request):
+        expected_headers = {
+            'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
+            'X-Top-Level-Method': 'open_training',
+            'X-Low-Level-Method': 'open_training_async',
+        }
+        check_headers(request, expected_headers)
 
-    result = toloka_client.create_tasks(
-        tasks=[client.structure(task, client.task.Task) for task in tasks_map]
-    )
+        return httpx.Response(json=open_operation_map, status_code=202)
 
-    assert requests_count == 2
-    assert task_create_result_map == client.unstructure(result)
+    def complete_open(request):
+        expected_headers = {
+            'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
+            'X-Top-Level-Method': 'open_training',
+            'X-Low-Level-Method': 'get_operation',
+        }
+        check_headers(request, expected_headers)
 
+        return httpx.Response(json=complete_open_operation_map, status_code=200)
 
-def test_create_tasks_async_retry(
-    respx_mock, toloka_client, toloka_url, tasks_map, task_create_result_map, operation_success_map
-):
-    requests_count = 0
-    first_request_op_id = None
-
-    def tasks(request):
-        nonlocal requests_count
-        nonlocal first_request_op_id
-
-        requests_count += 1
-        if requests_count == 1:
-            first_request_op_id = request.url.params['operation_id']
-            return httpx.Response(status_code=500)
-
-        assert request.url.params['operation_id'] == first_request_op_id
-        unstructured_error = client.unstructure(
-            IncorrectActionsApiError(
-                code='OPERATION_ALREADY_EXISTS',
-            )
-        )
-        del unstructured_error['status_code']
-
-        return httpx.Response(
-            json=unstructured_error,
-            status_code=409
-        )
+    def training_map(request):
+        expected_headers = {
+            'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
+            'X-Top-Level-Method': 'open_training',
+            'X-Low-Level-Method': 'get_training',
+        }
+        check_headers(request, expected_headers)
 
-    respx_mock.get(
-        re.compile(rf'{toloka_url}/operations/.*')
-    ).mock(httpx.Response(json=operation_success_map, status_code=200))
-    respx_mock.post(f'{toloka_url}/tasks').mock(side_effect=tasks)
+        return httpx.Response(json=training_map_with_readonly, status_code=200)
 
-    result = toloka_client.create_tasks_async(
-        tasks=[client.structure(task, client.task.Task) for task in tasks_map]
-    )
+    respx_mock.post(f'{toloka_url}/trainings/21/open').mock(side_effect=open_operation)
+    respx_mock.get(f'{toloka_url}/operations/{open_operation_map["id"]}').mock(side_effect=complete_open)
+    respx_mock.get(f'{toloka_url}/trainings/21').mock(side_effect=training_map)
 
-    assert requests_count == 2
-    assert operation_success_map == client.unstructure(result)
+    result = toloka_client.open_training('21')
+    assert training_map_with_readonly == client.unstructure(result)
 
 
-def test_find_tasks(respx_mock, toloka_client, toloka_url, task_map_with_readonly):
+@pytest.fixture
+def test_open_training_already_opened(respx_mock, toloka_client, toloka_url, open_training_map_with_readonly):
+    respx_mock.post(f'{toloka_url}/trainings/21/open', [{'status_code': 204}])
+    respx_mock.get(f'{toloka_url}/pools/21').mock(side_effect=open_training_map_with_readonly)
+    assert toloka_client.open_training_async('21') is None
+    result = toloka_client.open_training('21')
+    assert open_training_map_with_readonly == client.unstructure(result)
 
-    raw_result = {'items': [task_map_with_readonly], 'has_more': False}
 
-    def tasks(request):
+@pytest.fixture
+def close_operation_map():
+    return {
+        'id': 'close-training-op1id',
+        'type': 'TRAINING.CLOSE',
+        'status': 'RUNNING',
+        'submitted': '2016-07-22T13:04:00',
+        'started': '2016-07-22T13:04:01',
+        'finished': '2016-07-22T13:04:02',
+        'parameters': {'training_id': '21'},
+    }
+
+
+@pytest.fixture
+def complete_close_operation_map(close_operation_map):
+    return {
+        **close_operation_map,
+        'status': 'SUCCESS',
+        'finished': '2016-03-07T15:48:03',
+    }
+
+
+def test_close_training_async(respx_mock, toloka_client, toloka_url, complete_close_operation_map):
+
+    def complete_close_operation(request):
         expected_headers = {
             'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
-            'X-Top-Level-Method': 'find_tasks',
-            'X-Low-Level-Method': 'find_tasks',
+            'X-Top-Level-Method': 'close_training_async',
+            'X-Low-Level-Method': 'close_training_async',
         }
         check_headers(request, expected_headers)
 
-        assert QueryParams(
-            pool_id='21',
-            created_gt='2001-01-01T12:00:00',
-            overlap_gte='42',
-            sort='id,-created',
-            limit='20',
-        ) == request.url.params
-        return httpx.Response(json=raw_result, status_code=200)
+        return httpx.Response(json=complete_close_operation_map, status_code=202)
 
-    respx_mock.get(f'{toloka_url}/tasks').mock(side_effect=tasks)
+    respx_mock.post(f'{toloka_url}/trainings/21/close').mock(side_effect=complete_close_operation)
+    result = toloka_client.wait_operation(toloka_client.close_training_async('21'))
+    assert complete_close_operation_map == client.unstructure(result)
 
-    # Request object syntax
-    request = client.search_requests.TaskSearchRequest(
-        pool_id=21,
-        created_gt=datetime.datetime(2001, 1, 1, 12, 0, 0, tzinfo=datetime.timezone.utc),
-        overlap_gte=42,
-    )
-    sort = client.search_requests.TaskSortItems(['id', '-created'])
-    result = toloka_client.find_tasks(request, sort=sort, limit=20)
-    assert raw_result == client.unstructure(result)
 
-    # Expanded syntax
-    result = toloka_client.find_tasks(
-        pool_id=21,
-        created_gt=datetime.datetime(2001, 1, 1, 12, 0, 0, tzinfo=datetime.timezone.utc),
-        overlap_gte=42,
-        sort=['id', '-created'],
-        limit=20,
-    )
-    assert raw_result == client.unstructure(result)
+def test_close_training(respx_mock, toloka_client, toloka_url,
+                        close_operation_map, complete_close_operation_map, training_map_with_readonly):
 
+    def close_operation(request):
+        expected_headers = {
+            'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
+            'X-Top-Level-Method': 'close_training',
+            'X-Low-Level-Method': 'close_training_async',
+        }
+        check_headers(request, expected_headers)
 
-def test_get_tasks(respx_mock, toloka_client, toloka_url, task_map_with_readonly):
-    tasks = [dict(task_map_with_readonly, id=str(uuid4())) for _ in range(50)]
-    tasks.sort(key=itemgetter('id'))
+        return httpx.Response(json=close_operation_map, status_code=202)
 
-    def get_tasks(request):
+    def complete_close_operation(request):
         expected_headers = {
             'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
-            'X-Top-Level-Method': 'get_tasks',
-            'X-Low-Level-Method': 'find_tasks',
+            'X-Top-Level-Method': 'close_training',
+            'X-Low-Level-Method': 'get_operation',
         }
         check_headers(request, expected_headers)
 
-        params = request.url.params
-        id_gt = params.get('id_gt', None)
-        params = params.remove('id_gt')
-        assert QueryParams(
-            pool_id='21',
-            created_gt='2001-01-01T12:00:00',
-            overlap_gte='42',
-            sort='id',
-        ) == params
+        return httpx.Response(json=complete_close_operation_map, status_code=200)
 
-        items = [task for task in tasks if id_gt is None or task['id'] > id_gt][:3]
-        return httpx.Response(json={'items': items, 'has_more': items[-1]['id'] != tasks[-1]['id']}, status_code=200)
+    def training(request):
+        expected_headers = {
+            'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
+            'X-Top-Level-Method': 'close_training',
+            'X-Low-Level-Method': 'get_training',
+        }
+        check_headers(request, expected_headers)
 
-    respx_mock.get(f'{toloka_url}/tasks').mock(side_effect=get_tasks)
+        return httpx.Response(json=training_map_with_readonly, status_code=200)
 
-    # Request object syntax
-    request = client.search_requests.TaskSearchRequest(
-        pool_id='21',
-        created_gt=datetime.datetime(2001, 1, 1, 12, 0, 0, tzinfo=datetime.timezone.utc),
-        overlap_gte=42,
-    )
-    result = toloka_client.get_tasks(request)
-    assert tasks == client.unstructure(list(result))
+    respx_mock.post(f'{toloka_url}/trainings/21/close').mock(side_effect=close_operation)
+    respx_mock.get(f'{toloka_url}/operations/{close_operation_map["id"]}').mock(side_effect=complete_close_operation)
+    respx_mock.get(f'{toloka_url}/trainings/21').mock(side_effect=training)
 
-    # Expanded syntax
-    result = toloka_client.get_tasks(
-        pool_id='21',
-        created_gt=datetime.datetime(2001, 1, 1, 12, 0, 0, tzinfo=datetime.timezone.utc),
-        overlap_gte=42,
-    )
-    assert tasks == client.unstructure(list(result))
+    result = toloka_client.close_training('21')
+    assert training_map_with_readonly == client.unstructure(result)
 
 
-def test_get_task(respx_mock, toloka_client, toloka_url, task_map_with_readonly):
+def test_close_training_already_closed(respx_mock, toloka_client, toloka_url, training_map_with_readonly):
 
-    def get_task(request):
+    def training(request):
         expected_headers = {
             'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
-            'X-Top-Level-Method': 'get_task',
-            'X-Low-Level-Method': 'get_task',
+            'X-Top-Level-Method': 'close_training',
+            'X-Low-Level-Method': 'get_training',
         }
         check_headers(request, expected_headers)
 
-        return httpx.Response(json=task_map_with_readonly, status_code=200)
+        return httpx.Response(json=training_map_with_readonly, status_code=200)
 
-    respx_mock.get(f'{toloka_url}/tasks/task-1').mock(side_effect=get_task)
-    result = toloka_client.get_task('task-1')
-    assert task_map_with_readonly == client.unstructure(result)
+    respx_mock.post(f'{toloka_url}/trainings/21/close').respond(status_code=204)
+    respx_mock.get(f'{toloka_url}/trainings/21').mock(side_effect=training)
+    assert toloka_client.close_training_async('21') is None
+    result = toloka_client.close_training('21')
+    assert training_map_with_readonly == client.unstructure(result)
 
 
-def test_patch_task(respx_mock, toloka_client, toloka_url, task_map_with_readonly):
-    raw_request = {'overlap': 10}
-    raw_result = {**task_map_with_readonly, **raw_request}
+@pytest.fixture
+def archive_operation_map():
+    return {
+        'id': 'archive-training-op1id',
+        'type': 'TRAINING.ARCHIVE',
+        'status': 'RUNNING',
+        'submitted': '2016-07-22T13:04:00',
+        'started': '2016-07-22T13:04:01',
+        'finished': '2016-07-22T13:04:02',
+        'parameters': {'training_id': '21'},
+    }
+
 
-    def tasks(request):
+@pytest.fixture
+def complete_archive_operation_map(archive_operation_map):
+    return {
+        **archive_operation_map,
+        'status': 'SUCCESS',
+        'finished': '2016-03-07T15:48:03',
+    }
+
+
+def test_archive_training_async(respx_mock, toloka_client, toloka_url, complete_archive_operation_map):
+
+    def complete_archive_operation(request):
         expected_headers = {
             'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
-            'X-Top-Level-Method': 'patch_task',
-            'X-Low-Level-Method': 'patch_task',
+            'X-Top-Level-Method': 'archive_training_async',
+            'X-Low-Level-Method': 'archive_training_async',
         }
         check_headers(request, expected_headers)
 
-        assert raw_request == simplejson.loads(request.content)
-        return httpx.Response(json=raw_result, status_code=200)
+        return httpx.Response(json=complete_archive_operation_map, status_code=202)
 
-    respx_mock.patch(f'{toloka_url}/tasks/task-1').mock(side_effect=tasks)
+    respx_mock.post(f'{toloka_url}/trainings/21/archive').mock(side_effect=complete_archive_operation)
+    result = toloka_client.wait_operation(toloka_client.archive_training_async('21'))
+    assert complete_archive_operation_map == client.unstructure(result)
 
-    # Request object syntax
-    request = client.structure(raw_request, client.task.TaskPatch)
-    result = toloka_client.patch_task('task-1', request)
-    assert raw_result == client.unstructure(result)
 
-    # Expanded syntax
-    result = toloka_client.patch_task('task-1', overlap=10)
-    assert raw_result == client.unstructure(result)
+def test_archive_training(respx_mock, toloka_client, toloka_url,
+                          archive_operation_map, complete_archive_operation_map, training_map_with_readonly):
 
+    def archive_operation(request):
+        expected_headers = {
+            'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
+            'X-Top-Level-Method': 'archive_training',
+            'X-Low-Level-Method': 'archive_training_async',
+        }
+        check_headers(request, expected_headers)
 
-def test_patch_task_with_baseline_solution(respx_mock, toloka_client, toloka_url, task_map_with_readonly):
-    raw_request = {
-        'baseline_solutions': [{
-            'output_values': {'color': 'green'},
-            'confidence_weight': 4.2,
-        }]
-    }
-    raw_result = {**task_map_with_readonly, **raw_request}
+        return httpx.Response(json=archive_operation_map, status_code=202)
 
-    def tasks(request):
+    def complete_archive_operation(request):
         expected_headers = {
             'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
-            'X-Top-Level-Method': 'patch_task',
-            'X-Low-Level-Method': 'patch_task',
+            'X-Top-Level-Method': 'archive_training',
+            'X-Low-Level-Method': 'get_operation',
         }
         check_headers(request, expected_headers)
 
-        assert raw_request == simplejson.loads(request.content)
-        return httpx.Response(json=raw_result, status_code=200)
+        return httpx.Response(json=complete_archive_operation_map, status_code=200)
+
+    def training(request):
+        expected_headers = {
+            'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
+            'X-Top-Level-Method': 'archive_training',
+            'X-Low-Level-Method': 'get_training',
+        }
+        check_headers(request, expected_headers)
 
-    respx_mock.patch(f'{toloka_url}/tasks/task-1').mock(side_effect=tasks)
+        return httpx.Response(json=training_map_with_readonly, status_code=200)
 
-    # Request object syntax
-    request = client.structure(raw_request, client.task.TaskPatch)
-    result = toloka_client.patch_task('task-1', request)
-    assert raw_result == client.unstructure(result)
+    respx_mock.post(f'{toloka_url}/trainings/21/archive').mock(side_effect=archive_operation)
+    respx_mock.get(
+        f'{toloka_url}/operations/{archive_operation_map["id"]}'
+    ).mock(side_effect=complete_archive_operation)
+    respx_mock.get(f'{toloka_url}/trainings/21').mock(side_effect=training)
 
-    # Expanded syntax
-    result = toloka_client.patch_task(
-        'task-1',
-        baseline_solutions=[
-            client.task.Task.BaselineSolution(
-                output_values={'color': 'green'},
-                confidence_weight=4.2,
-            )
-        ]
-    )
-    assert raw_result == client.unstructure(result)
+    result = toloka_client.archive_training('21')
+    assert training_map_with_readonly == client.unstructure(result)
 
 
-def test_patch_task_with_known_solutions(respx_mock, toloka_client, toloka_url, task_map_with_readonly):
-    raw_request = {
-        'known_solutions': [
-            {
-                'output_values': {'color': 'black'},
-                'correctness_weight': 1.0,
-            },
-        ],
-        'message_on_unknown_solution': 'Main color is black'
-    }
-    raw_result = {**task_map_with_readonly, **raw_request}
+def test_close_archive_training_already_archived(respx_mock, toloka_client, toloka_url,
+                                                 archived_training_map_with_readonly):
 
-    def tasks(request):
+    def archived_training(request):
         expected_headers = {
             'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
-            'X-Top-Level-Method': 'patch_task',
-            'X-Low-Level-Method': 'patch_task',
+            'X-Top-Level-Method': 'archive_training',
+            'X-Low-Level-Method': 'get_training',
         }
         check_headers(request, expected_headers)
 
-        assert raw_request == simplejson.loads(request.content)
-        return httpx.Response(json=raw_result, status_code=200)
+        return httpx.Response(json=archived_training_map_with_readonly, status_code=200)
 
-    respx_mock.patch(f'{toloka_url}/tasks/task-1').mock(side_effect=tasks)
+    respx_mock.post(f'{toloka_url}/trainings/21/archive').respond(status_code=204)
+    respx_mock.get(f'{toloka_url}/trainings/21').mock(side_effect=archived_training)
+    assert toloka_client.archive_training_async('21') is None
+    result = toloka_client.archive_training('21')
+    assert archived_training_map_with_readonly == client.unstructure(result)
 
-    # Request object syntax
-    request = client.structure(raw_request, client.task.TaskPatch)
-    result = toloka_client.patch_task('task-1', request)
-    assert raw_result == client.unstructure(result)
 
-    # Expanded syntax
-    result = toloka_client.patch_task(
-        'task-1',
-        known_solutions=[
-            client.task.Task.KnownSolution(
-                output_values={'color': 'black'},
-                correctness_weight=1.0,
-            )
-        ],
-        message_on_unknown_solution='Main color is black',
-    )
-    assert raw_result == client.unstructure(result)
+@pytest.fixture
+def clone_operation_map():
+    return {
+        'id': 'archive-training-op1id',
+        'type': 'TRAINING.CLONE',
+        'status': 'RUNNING',
+        'submitted': '2016-07-22T13:04:00',
+        'started': '2016-07-22T13:04:01',
+        'finished': '2016-07-22T13:04:02',
+        'parameters': {'training_id': '21'},
+    }
 
 
-def test_task_overlap_or_min(respx_mock, toloka_client, toloka_url, task_map_with_readonly):
-    raw_request = {'overlap': 10}
-    raw_result = {**task_map_with_readonly, 'overlap': 12}
+@pytest.fixture
+def complete_clone_operation_map(clone_operation_map):
+    return {
+        **clone_operation_map,
+        'status': 'SUCCESS',
+        'finished': '2016-03-07T15:48:03',
+        'details': {'training_id': '22'},
+    }
+
 
-    def tasks(request):
+@pytest.fixture
+def cloned_training_map_with_readonly(training_map_with_readonly):
+    return {
+        **training_map_with_readonly,
+        'id': '22'
+    }
+
+
+def test_clone_training_async(respx_mock, toloka_client, toloka_url, complete_clone_operation_map):
+
+    def complete_clone_operation(request):
         expected_headers = {
             'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
-            'X-Top-Level-Method': 'patch_task_overlap_or_min',
-            'X-Low-Level-Method': 'patch_task_overlap_or_min',
+            'X-Top-Level-Method': 'clone_training_async',
+            'X-Low-Level-Method': 'clone_training_async',
         }
         check_headers(request, expected_headers)
 
-        assert raw_request == simplejson.loads(request.content)
-        return httpx.Response(json=raw_result, status_code=200)
+        return httpx.Response(json=complete_clone_operation_map, status_code=202)
 
-    respx_mock.patch(f'{toloka_url}/tasks/task-1/set-overlap-or-min').mock(side_effect=tasks)
+    respx_mock.post(f'{toloka_url}/trainings/21/clone').mock(side_effect=complete_clone_operation)
+    result = toloka_client.wait_operation(toloka_client.clone_training_async('21'))
+    assert complete_clone_operation_map == client.unstructure(result)
 
-    # Request object syntax
-    request = client.structure(raw_request, client.task.TaskPatch)
-    result = toloka_client.patch_task_overlap_or_min('task-1', request)
-    assert raw_result == client.unstructure(result)
 
-    # Expanded syntax
-    result = toloka_client.patch_task_overlap_or_min('task-1', overlap=10)
-    assert raw_result == client.unstructure(result)
+def test_clone_training(respx_mock, toloka_client, toloka_url,
+                        clone_operation_map, complete_clone_operation_map, cloned_training_map_with_readonly, caplog):
 
+    def clone_operation(request):
+        expected_headers = {
+            'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
+            'X-Top-Level-Method': 'clone_training',
+            'X-Low-Level-Method': 'clone_training_async',
+        }
+        check_headers(request, expected_headers)
 
-def test_task_overlap_or_min_infinite_overlap(respx_mock, toloka_client, toloka_url, task_map_with_readonly):
-    raw_request = {'infinite_overlap': True}
-    raw_result = task_map_with_readonly
+        return httpx.Response(json=clone_operation_map, status_code=202)
 
-    def tasks(request):
+    def complete_clone_operation(request):
         expected_headers = {
             'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
-            'X-Top-Level-Method': 'patch_task_overlap_or_min',
-            'X-Low-Level-Method': 'patch_task_overlap_or_min',
+            'X-Top-Level-Method': 'clone_training',
+            'X-Low-Level-Method': 'get_operation',
         }
         check_headers(request, expected_headers)
 
-        assert raw_request == simplejson.loads(request.content)
-        return httpx.Response(json=raw_result, status_code=200)
+        return httpx.Response(json=complete_clone_operation_map, status_code=200)
+
+    def cloned_training(request):
+        expected_headers = {
+            'X-Caller-Context': 'client' if isinstance(toloka_client, client.TolokaClient) else 'async_client',
+            'X-Top-Level-Method': 'clone_training',
+            'X-Low-Level-Method': 'get_training',
+        }
+        check_headers(request, expected_headers)
 
-    respx_mock.patch(f'{toloka_url}/tasks/task-1/set-overlap-or-min').mock(side_effect=tasks)
+        return httpx.Response(json=cloned_training_map_with_readonly, status_code=200)
 
-    # Request object syntax
-    request = client.structure(raw_request, client.task.TaskPatch)
-    result = toloka_client.patch_task_overlap_or_min('task-1', request)
-    assert raw_result == client.unstructure(result)
+    respx_mock.post(f'{toloka_url}/trainings/21/clone').mock(side_effect=clone_operation)
+    respx_mock.get(f'{toloka_url}/operations/{clone_operation_map["id"]}').mock(side_effect=complete_clone_operation)
+    respx_mock.get(f'{toloka_url}/trainings/22').mock(side_effect=cloned_training)
 
-    # Expanded syntax
-    result = toloka_client.patch_task_overlap_or_min('task-1', infinite_overlap=True)
-    assert raw_result == client.unstructure(result)
+    with caplog.at_level(logging.INFO):
+        caplog.clear()
+        result = toloka_client.clone_training('21')
+        assert [log for log in caplog.record_tuples if log[0] == 'toloka.client'] == [(
+            'toloka.client',
+            logging.INFO,
+            'A new training with ID "22" has been cloned. Link to open in web interface: https://sandbox.toloka.yandex.com/requester/project/10/training/22'
+        )]
+        assert cloned_training_map_with_readonly == client.unstructure(result)
```

### Comparing `toloka-kit-1.1.4/tests/test_user.py` & `toloka-kit-1.2.0/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/tests/test_user_restriction.py` & `toloka-kit-1.2.0/tests/test_user_restriction.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/tests/test_user_skill.py` & `toloka-kit-1.2.0/tests/test_user_skill.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/tests/test_webhook_subscription.py` & `toloka-kit-1.2.0/tests/test_webhook_subscription.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.1.4/toloka_kit.egg-info/PKG-INFO` & `toloka-kit-1.2.0/toloka_kit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toloka-kit
-Version: 1.1.4
+Version: 1.2.0
 Summary: Toloka API client
 Author: Vladimir Losev
 Author-email: losev@yandex-team.ru
 License: Apache 2.0
 Project-URL: Documentation, https://toloka.ai/en/docs/toloka-kit
 Project-URL: Source, https://github.com/Toloka/toloka-kit
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -44,32 +45,32 @@
 [![Coverage](https://codecov.io/gh/Toloka/toloka-kit/branch/main/graph/badge.svg)](https://codecov.io/gh/Toloka/toloka-kit)
 [![GitHub Tests](https://github.com/Toloka/toloka-kit/workflows/Tests/badge.svg?branch=main)](//github.com/Toloka/toloka-kit/actions?query=workflow:Tests)
 
 [Toloka website](https://toloka.ai/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) | [Documentation](https://toloka.ai/en/docs/toloka-kit/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) | [Issue tracker](https://github.com/Toloka/toloka-kit/issues)
 
 
 
-Toloka-Kit is a Python library for working with [Toloka API](https://toloka.ai/docs/api/concepts/about.html/?utm_source=github&utm_medium=site&utm_campaign=tolokakit). 
+Toloka-Kit is a Python library for working with [Toloka API](https://toloka.ai/docs/api/?utm_source=github&utm_medium=site&utm_campaign=tolokakit). 
 
 The API allows you to build scalable and fully automated human-in-the-loop ML pipelines, and integrate them into your processes. The toolkit makes integration easier. You can use it with Jupyter notebooks.
 
 * Support for all common Toloka use cases: creating projects, adding pools, uploading tasks, and so on.
 * Toloka entities are represented as Python classes. You can use them instead of accessing the API using JSON representations.
 * There’s no need to validate JSON files and work with them directly.
 * Support of both synchronous and asynchronous (via async/await) executions.
 * Streaming support: build complex pipelines which send and receive data in real time. For example, you can [pass data between two related projects](https://github.com/Toloka/toloka-kit/blob/main/examples/6.streaming_pipelines/streaming_pipelines.ipynb): one for data labeling, and another for its validation. 
 * [AutoQuality](https://medium.com/toloka/automating-crowdsourcing-quality-control-ad057baf00fd) feature which automatically finds the best fitting quality control rules for your project.
 
 ## Prerequisites
 
 Before you begin, make sure that:
 * You are using [Python](https://www.python.org/) v3.7 or higher.
-* You are [registered](https://toloka.ai/docs/guide/concepts/access.html/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) in Toloka as a requester.
-* You have [topped up](https://toloka.ai/docs/guide/concepts/refill.html/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) your Toloka account.
-* You have [set up an OAuth token](https://toloka.ai/docs/api/concepts/access.html/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) to access Toloka API.
+* You are [registered](https://toloka.ai/docs/guide/concepts/access/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) in Toloka as a requester.
+* You have [topped up](https://toloka.ai/docs/guide/concepts/refill/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) your Toloka account.
+* You have [set up an OAuth token](https://toloka.ai/docs/api/concepts/access/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) to access Toloka API.
 
 ## Get Started
 1. Install the Toloka-Kit package. Run the following command in the command shell:
 ```
 $ pip install toloka-kit
 ```
 For production environments, specify the exact package version. For the latest stable version, check the [project page at pypi.org](https://pypi.org/project/toloka-kit/).
@@ -106,20 +107,20 @@
 ```
 
 ## Usage examples
 [Toloka-kit usage examples](https://github.com/Toloka/toloka-kit/tree/main/examples#toloka-kit-usage-examples) - tutorials for specific data labeling tasks. They demonstrate how to work with Toloka API using Toloka-Kit.
 
 ## Documentation
 * [Toloka-Kit documentation](https://toloka.ai/en/docs/toloka-kit/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
-* [Toloka API reference](https://toloka.ai/docs/api/concepts/about.html/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
-* [Toloka web interface documentation](https://toloka.ai/docs/guide/concepts/overview.html/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
+* [Toloka API reference](https://toloka.ai/docs/api/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
+* [Toloka web interface documentation](https://toloka.ai/docs/guide/concepts/overview/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
 
 ## Support
 * To suggest a feature or report a bug, go to our [issues page](https://github.com/Toloka/toloka-kit/issues).
 * If you have any questions, feel free to ask our [Slack community](https://toloka.ai/community/?utm_source=github&utm_medium=site&utm_campaign=tolokakit).
 
 ## Contributing
 Feel free to contribute to toloka-kit. Right now, we need more [usage examples](https://github.com/Toloka/toloka-kit/tree/main/examples#need-more-examples).
 
 ## License
-© YANDEX LLC, 2020.
+© Copyright 2023 Toloka team authors.
 Licensed under the terms of the Apache License, Version 2.0. See [LICENSE](https://github.com/Toloka/toloka-kit/blob/main/LICENSE) for more details.
```

### Comparing `toloka-kit-1.1.4/toloka_kit.egg-info/SOURCES.txt` & `toloka-kit-1.2.0/toloka_kit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,16 @@
 src/client/pool/dynamic_pricing_config.pyi
 src/client/pool/mixer_config.py
 src/client/pool/mixer_config.pyi
 src/client/pool/speed_quality_balance_config.py
 src/client/pool/speed_quality_balance_config.pyi
 src/client/primitives/__init__.py
 src/client/primitives/__init__.pyi
+src/client/primitives/adapters.py
+src/client/primitives/adapters.pyi
 src/client/primitives/base.py
 src/client/primitives/base.pyi
 src/client/primitives/infinite_overlap.py
 src/client/primitives/infinite_overlap.pyi
 src/client/primitives/operators.py
 src/client/primitives/operators.pyi
 src/client/primitives/parameter.py
@@ -194,19 +196,16 @@
 tests/test_message_thread.py
 tests/test_operation.py
 tests/test_operation_log.py
 tests/test_project.py
 tests/test_requester.py
 tests/test_serialization.py
 tests/test_skill.py
-tests/test_task.py
-tests/test_task_suite.py
 tests/test_training.py
 tests/test_user.py
-tests/test_user_bonus.py
 tests/test_user_restriction.py
 tests/test_user_skill.py
 tests/test_webhook_subscription.py
 toloka_kit.egg-info/PKG-INFO
 toloka_kit.egg-info/SOURCES.txt
 toloka_kit.egg-info/dependency_links.txt
 toloka_kit.egg-info/requires.txt
```

