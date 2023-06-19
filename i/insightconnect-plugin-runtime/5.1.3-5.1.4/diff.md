# Comparing `tmp/insightconnect-plugin-runtime-5.1.3.tar.gz` & `tmp/insightconnect-plugin-runtime-5.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insightconnect-plugin-runtime-5.1.3.tar", last modified: Thu Jun  1 13:17:05 2023, max compression
+gzip compressed data, was "insightconnect-plugin-runtime-5.1.4.tar", last modified: Mon Jun 19 09:16:22 2023, max compression
```

## Comparing `insightconnect-plugin-runtime-5.1.3.tar` & `insightconnect-plugin-runtime-5.1.4.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.231957 insightconnect-plugin-runtime-5.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-06-01 13:17:05.231957 insightconnect-plugin-runtime-5.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17497 2023-06-01 13:16:24.000000 insightconnect-plugin-runtime-5.1.3/insightconnect-plugin-swagger.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.223957 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/action.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.227957 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26847 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/api/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.227957 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/clients/aws_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/clients/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.227957 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/data/input_message_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/data/output_message_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21108 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21787 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.223957 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-06-01 13:17:05.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-06-01 13:17:05.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:17:05.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-01 13:17:05.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-01 13:17:05.000000 insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:17:05.231957 insightconnect-plugin-runtime-5.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.227957 insightconnect-plugin-runtime-5.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.227957 insightconnect-plugin-runtime-5.1.3/tests/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.227957 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.227957 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.227957 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.227957 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/actions/
--rwxr-xr-x   0 runner    (1001) docker     (123)      173 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.227957 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/
--rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      930 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.227957 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      631 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      946 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.227957 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/
--rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1077 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.227957 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/connection/
--rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/connection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      375 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/connection/connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      517 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.227957 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/
--rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.227957 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.231957 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/
--rwxr-xr-x   0 runner    (1001) docker     (123)       82 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      960 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      717 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.231957 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/
--rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      680 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.231957 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/util/
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/util/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      467 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.231957 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/tests/test_hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/tests/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:17:05.231957 insightconnect-plugin-runtime-5.1.3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/unit/test_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/unit/test_aws_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/unit/test_custom_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/unit/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/unit/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/unit/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/unit/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/unit/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/unit/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/unit/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/unit/test_server_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/unit/test_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-01 13:15:28.000000 insightconnect-plugin-runtime-5.1.3/tests/unit/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.365905 insightconnect-plugin-runtime-5.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-19 09:16:22.365905 insightconnect-plugin-runtime-5.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17497 2023-06-19 09:15:32.000000 insightconnect-plugin-runtime-5.1.4/insightconnect-plugin-swagger.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.353905 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/action.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26847 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/api/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/clients/aws_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/clients/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/data/input_message_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/data/output_message_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21108 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21787 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.353905 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-19 09:16:22.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-06-19 09:16:22.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 09:16:22.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-19 09:16:22.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-19 09:16:22.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 09:16:22.365905 insightconnect-plugin-runtime-5.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/tests/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      173 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      930 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      631 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      946 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.361905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1077 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.361905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/connection/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/connection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      375 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/connection/connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      517 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.361905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.361905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.361905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       82 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      960 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      717 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.361905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      680 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.361905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/util/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/util/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      467 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.361905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/tests/test_hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.365905 insightconnect-plugin-runtime-5.1.4/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_aws_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_custom_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_server_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_variables.py
```

### Comparing `insightconnect-plugin-runtime-5.1.3/PKG-INFO` & `insightconnect-plugin-runtime-5.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insightconnect-plugin-runtime
-Version: 5.1.3
+Version: 5.1.4
 Summary: InsightConnect Plugin Runtime
 Home-page: https://github.com/rapid7/komand-plugin-sdk-python
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -150,14 +150,15 @@
 Contributions for maintaining and enhancing the InsightConnect Python Plugin Runtime are appreciated. This project uses
 [Black](https://github.com/psf/black) for code formatting and includes a pre-commit hook to auto format code as it is
 contributed. Black is installed as a test dependency and the hook can be initialized by running `pre-commit install` 
 after cloning this repository.
 
 ## Changelog
 
+* 5.1.4 - Fix credential masking when connection is null
 * 5.1.3 - Fix credential masking when some input fields are empty
 * 5.1.2 - Add connection credential masking to the plugin's output and log when displayed as plain text | Add new `OutputMasker` class to handle credential masking    
 * 5.1.1 - Updated exception preset messages
 * 5.1.0 - Add new helper functions
 * 5.0.0 - Add `has_more_pages` property to task output to indicate task pagination status to output consumers
 * 4.10.1 - Remove raising of exception if request id is not available in header
 * 4.10.0 - Add structlog for structured logging
```

### Comparing `insightconnect-plugin-runtime-5.1.3/README.md` & `insightconnect-plugin-runtime-5.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 Contributions for maintaining and enhancing the InsightConnect Python Plugin Runtime are appreciated. This project uses
 [Black](https://github.com/psf/black) for code formatting and includes a pre-commit hook to auto format code as it is
 contributed. Black is installed as a test dependency and the hook can be initialized by running `pre-commit install` 
 after cloning this repository.
 
 ## Changelog
 
+* 5.1.4 - Fix credential masking when connection is null
 * 5.1.3 - Fix credential masking when some input fields are empty
 * 5.1.2 - Add connection credential masking to the plugin's output and log when displayed as plain text | Add new `OutputMasker` class to handle credential masking    
 * 5.1.1 - Updated exception preset messages
 * 5.1.0 - Add new helper functions
 * 5.0.0 - Add `has_more_pages` property to task output to indicate task pagination status to output consumers
 * 4.10.1 - Remove raising of exception if request id is not available in header
 * 4.10.0 - Add structlog for structured logging
```

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect-plugin-swagger.json` & `insightconnect-plugin-runtime-5.1.4/insightconnect-plugin-swagger.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -447,71 +447,71 @@
         "version": "1.0"
     },
     "swagger": "2.0",
     "definitions": {
         "PluginInfo": {
             "type": "object",
             "properties": {
-                "vendor": {
+                "support": {
                     "type": "string"
                 },
-                "threads": {
-                    "type": "integer",
-                    "format": "int32"
+                "version": {
+                    "type": "string"
                 },
-                "support": {
+                "vendor": {
                     "type": "string"
                 },
-                "enable_cache": {
-                    "type": "boolean"
+                "plugin_spec_version": {
+                    "type": "string"
                 },
-                "title": {
+                "description": {
                     "type": "string"
                 },
                 "tags": {
                     "type": "array",
                     "items": {
                         "type": "string"
                     }
                 },
+                "number_of_workers": {
+                    "type": "integer",
+                    "format": "int32"
+                },
                 "sdk_version": {
                     "type": "string"
                 },
-                "description": {
+                "name": {
                     "type": "string"
                 },
-                "name": {
+                "title": {
                     "type": "string"
                 },
-                "number_of_workers": {
+                "threads": {
                     "type": "integer",
                     "format": "int32"
                 },
-                "version": {
-                    "type": "string"
-                },
-                "plugin_spec_version": {
-                    "type": "string"
+                "enable_cache": {
+                    "type": "boolean"
                 }
             }
         },
         "ActionTriggerOutputBody": {
             "type": "object",
             "properties": {
                 "status": {
                     "type": "string"
                 },
+                "log": {
+                    "type": "string"
+                },
                 "output": {
                     "type": "object"
                 },
                 "meta": {
                     "type": "object"
-                },
-                "log": {
-                    "type": "string"
                 }
             },
             "required": [
                 "log",
                 "meta",
                 "output",
                 "status"
@@ -539,28 +539,28 @@
                 "type",
                 "version"
             ]
         },
         "TaskOutputBody": {
             "type": "object",
             "properties": {
-                "status": {
-                    "type": "string"
-                },
                 "state": {
                     "type": "object"
                 },
-                "log": {
-                    "type": "string"
-                },
                 "output": {
                     "type": "object"
                 },
                 "meta": {
                     "type": "object"
+                },
+                "status": {
+                    "type": "string"
+                },
+                "log": {
+                    "type": "string"
                 }
             },
             "required": [
                 "log",
                 "meta",
                 "output",
                 "state",
@@ -588,18 +588,18 @@
                 "type",
                 "version"
             ]
         },
         "ActionTriggerInputBody": {
             "type": "object",
             "properties": {
-                "input": {
+                "connection": {
                     "type": "object"
                 },
-                "connection": {
+                "input": {
                     "type": "object"
                 },
                 "action": {
                     "type": "string"
                 }
             },
             "required": [
@@ -630,23 +630,23 @@
                 "type",
                 "version"
             ]
         },
         "TaskInputBody": {
             "type": "object",
             "properties": {
-                "input": {
-                    "type": "object"
-                },
                 "connection": {
                     "type": "object"
                 },
                 "task": {
                     "type": "string"
                 },
+                "input": {
+                    "type": "object"
+                },
                 "state": {
                     "type": "object"
                 }
             },
             "required": [
                 "connection",
                 "input",
@@ -675,74 +675,74 @@
                 "type",
                 "version"
             ]
         },
         "ActionTriggerDetails": {
             "type": "object",
             "properties": {
-                "input": {
+                "output": {
                     "type": "object"
                 },
+                "description": {
+                    "type": "string"
+                },
                 "title": {
                     "type": "string"
                 },
-                "output": {
+                "input": {
                     "type": "object"
-                },
-                "description": {
-                    "type": "string"
                 }
             }
         },
         "ConnectionDetails": {
             "type": "object",
             "properties": {
                 "type": {
                     "type": "string"
                 },
+                "properties": {
+                    "type": "object"
+                },
                 "title": {
                     "type": "string"
                 },
                 "required": {
                     "type": "array",
                     "items": {
                         "type": "string"
                     }
-                },
-                "properties": {
-                    "type": "object"
                 }
             }
         },
         "ConnectionTestOutput": {
             "type": "object",
             "properties": {
                 "message": {
                     "type": "object"
                 }
             }
         },
         "TaskDetails": {
             "type": "object",
             "properties": {
-                "schedule": {
+                "input": {
                     "type": "object"
                 },
                 "state": {
                     "type": "object"
                 },
-                "input": {
-                    "type": "object"
-                },
-                "title": {
+                "description": {
                     "type": "string"
                 },
                 "output": {
                     "type": "object"
                 },
-                "description": {
+                "schedule": {
+                    "type": "object"
+                },
+                "title": {
                     "type": "string"
                 }
             }
         }
     }
 }
```

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/__init__.py` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/api/endpoints.py` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/api/endpoints.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/api/schemas.py` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/api/schemas.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/cli.py` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/cli.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/clients/aws_client.py` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/clients/aws_client.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/clients/oauth.py` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/clients/oauth.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/connection.py` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/connection.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/data/input_message_schema.json` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/data/input_message_schema.json`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/data/output_message_schema.json` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/data/output_message_schema.json`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/dispatcher.py` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/dispatcher.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/exceptions.py` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/exceptions.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/helper.py` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/helper.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/metrics.py` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/metrics.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/plugin.py` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/plugin.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/schema.py` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/server.py` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/server.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/step.py` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/step.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/trigger.py` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/util.py` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,20 @@
         :param keys_to_check: A dictionary containing the connection details. Defaults to KEYS_TO_CHECK_SECRETS.
         :type: Tuple[str]
         :return: A tuple containing the values of keys to be searched.
         :rtype: List[Any]
         """
 
         connection_values = []
-        for key, value in connection.items():
-            if isinstance(value, dict):
-                connection_values.extend(OutputMasker.extract_connection_values(value))
-            elif isinstance(value, str) and value and key in keys_to_check:
-                connection_values.append(value)
+        if connection and isinstance(connection, dict):
+            for key, value in connection.items():
+                if isinstance(value, dict):
+                    connection_values.extend(OutputMasker.extract_connection_values(value))
+                elif isinstance(value, str) and value and key in keys_to_check:
+                    connection_values.append(value)
         return sorted(set(connection_values))
 
     @staticmethod
     def count_percentage_leak(text: str, body: str) -> Tuple[str, float]:
         """
         count_percentage_leak. Counts the percentage of text that appears in the body string.
```

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime/variables.py` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/variables.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime.egg-info/PKG-INFO` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insightconnect-plugin-runtime
-Version: 5.1.3
+Version: 5.1.4
 Summary: InsightConnect Plugin Runtime
 Home-page: https://github.com/rapid7/komand-plugin-sdk-python
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -150,14 +150,15 @@
 Contributions for maintaining and enhancing the InsightConnect Python Plugin Runtime are appreciated. This project uses
 [Black](https://github.com/psf/black) for code formatting and includes a pre-commit hook to auto format code as it is
 contributed. Black is installed as a test dependency and the hook can be initialized by running `pre-commit install` 
 after cloning this repository.
 
 ## Changelog
 
+* 5.1.4 - Fix credential masking when connection is null
 * 5.1.3 - Fix credential masking when some input fields are empty
 * 5.1.2 - Add connection credential masking to the plugin's output and log when displayed as plain text | Add new `OutputMasker` class to handle credential masking    
 * 5.1.1 - Updated exception preset messages
 * 5.1.0 - Add new helper functions
 * 5.0.0 - Add `has_more_pages` property to task output to indicate task pagination status to output consumers
 * 4.10.1 - Remove raising of exception if request id is not available in header
 * 4.10.0 - Add structlog for structured logging
```

### Comparing `insightconnect-plugin-runtime-5.1.3/insightconnect_plugin_runtime.egg-info/SOURCES.txt` & `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/setup.py` & `insightconnect-plugin-runtime-5.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="insightconnect-plugin-runtime",
-    version="5.1.3",
+    version="5.1.4",
     description="InsightConnect Plugin Runtime",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Rapid7 Integrations Alliance",
     author_email="integrationalliance@rapid7.com",
     url="https://github.com/rapid7/komand-plugin-sdk-python",
     packages=find_packages(),
```

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/plugin/__init__.py` & `insightconnect-plugin-runtime-5.1.4/tests/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/__init__.py` & `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/__init__.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py` & `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py` & `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py` & `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py` & `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py` & `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py` & `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py` & `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py` & `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py` & `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py` & `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py` & `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py` & `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py` & `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/tests/conftest.py` & `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/tests/test_cli.py` & `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/tests/test_hello_world.py` & `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/tests/test_hello_world.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/plugin/hello_world/tests/test_server.py` & `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/unit/test_action.py` & `insightconnect-plugin-runtime-5.1.4/tests/unit/test_action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/unit/test_aws_action.py` & `insightconnect-plugin-runtime-5.1.4/tests/unit/test_aws_action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/unit/test_custom_encoder.py` & `insightconnect-plugin-runtime-5.1.4/tests/unit/test_custom_encoder.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/unit/test_endpoints.py` & `insightconnect-plugin-runtime-5.1.4/tests/unit/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/unit/test_exceptions.py` & `insightconnect-plugin-runtime-5.1.4/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/unit/test_helpers.py` & `insightconnect-plugin-runtime-5.1.4/tests/unit/test_helpers.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/unit/test_metrics.py` & `insightconnect-plugin-runtime-5.1.4/tests/unit/test_metrics.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/unit/test_oauth.py` & `insightconnect-plugin-runtime-5.1.4/tests/unit/test_oauth.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/unit/test_plugin.py` & `insightconnect-plugin-runtime-5.1.4/tests/unit/test_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,14 +126,19 @@
     assert masked_output == output_say_hello_masked_2
 
 
 def test_output_masking_3():
     connection = input_message_body_credential_missed.get("body", {}).get(
         "connection", {}
     )
-    print(f"Connection is: {connection}")
-    print(f"From File: {output_say_hello_unmasked_3}")
     masked_output = OutputMasker.mask_output_data(
         connection, output_say_hello_unmasked_3
     )
-    print(f"Masked: {masked_output}")
     assert masked_output == output_say_hello_masked_3
+
+
+def test_output_masking_when_connection_is_none():
+    connection = None
+    masked_output = OutputMasker.mask_output_data(
+        connection, output_say_hello_unmasked_3
+    )
+    assert masked_output == output_say_hello_unmasked_3
```

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/unit/test_schema.py` & `insightconnect-plugin-runtime-5.1.4/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/unit/test_server_spec.py` & `insightconnect-plugin-runtime-5.1.4/tests/unit/test_server_spec.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.3/tests/unit/test_trigger.py` & `insightconnect-plugin-runtime-5.1.4/tests/unit/test_trigger.py`

 * *Files identical despite different names*

