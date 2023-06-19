# Comparing `tmp/armonik-3.8.2.dev395.tar.gz` & `tmp/armonik-3.8.3.dev470.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "armonik-3.8.2.dev395.tar", last modified: Tue Jun  6 09:03:10 2023, max compression
+gzip compressed data, was "armonik-3.8.3.dev470.tar", last modified: Mon Jun 19 08:16:40 2023, max compression
```

## Comparing `armonik-3.8.2.dev395.tar` & `armonik-3.8.3.dev470.tar`

### file list

```diff
@@ -1,117 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:10.840252 armonik-3.8.2.dev395/
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-06 09:03:10.840252 armonik-3.8.2.dev395/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-06 09:02:54.000000 armonik-3.8.2.dev395/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-06 09:02:54.000000 armonik-3.8.2.dev395/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 09:03:10.840252 armonik-3.8.2.dev395/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:10.824252 armonik-3.8.2.dev395/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:10.824252 armonik-3.8.2.dev395/src/armonik/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-06 09:02:54.000000 armonik-3.8.2.dev395/src/armonik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-06 09:03:05.000000 armonik-3.8.2.dev395/src/armonik/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:10.828252 armonik-3.8.2.dev395/src/armonik/client/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-06 09:02:54.000000 armonik-3.8.2.dev395/src/armonik/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-06-06 09:02:54.000000 armonik-3.8.2.dev395/src/armonik/client/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-06 09:02:54.000000 armonik-3.8.2.dev395/src/armonik/client/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:10.828252 armonik-3.8.2.dev395/src/armonik/common/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-06 09:02:54.000000 armonik-3.8.2.dev395/src/armonik/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-06 09:02:54.000000 armonik-3.8.2.dev395/src/armonik/common/enumwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-06 09:02:54.000000 armonik-3.8.2.dev395/src/armonik/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-06-06 09:02:54.000000 armonik-3.8.2.dev395/src/armonik/common/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:10.824252 armonik-3.8.2.dev395/src/armonik/protogen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:10.832252 armonik-3.8.2.dev395/src/armonik/protogen/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/applications_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/applications_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/applications_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/auth_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/auth_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/auth_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/events_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/events_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/events_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/partitions_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/partitions_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/partitions_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/results_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/results_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16128 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/results_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/sessions_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/sessions_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/sessions_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/submitter_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/submitter_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27332 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/submitter_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/tasks_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/tasks_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/tasks_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/versions_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/versions_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/client/versions_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:10.836252 armonik-3.8.2.dev395/src/armonik/protogen/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/agent_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/agent_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/agent_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/applications_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/applications_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/applications_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/auth_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/auth_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/auth_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/events_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/events_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/events_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/objects_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/objects_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/objects_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/partitions_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/partitions_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/partitions_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/result_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/result_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/result_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/results_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/results_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/results_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/session_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/session_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/session_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/sessions_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/sessions_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/sessions_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/sort_direction_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/sort_direction_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/sort_direction_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/submitter_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/submitter_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/submitter_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/task_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/task_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/task_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/tasks_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19219 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/tasks_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/tasks_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/versions_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/versions_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/versions_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/worker_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/worker_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/common/worker_common_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:10.840252 armonik-3.8.2.dev395/src/armonik/protogen/worker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/worker/agent_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/worker/agent_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/worker/agent_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/worker/worker_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/worker/worker_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-06-06 09:03:04.000000 armonik-3.8.2.dev395/src/armonik/protogen/worker/worker_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:10.840252 armonik-3.8.2.dev395/src/armonik/worker/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-06 09:02:54.000000 armonik-3.8.2.dev395/src/armonik/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-06-06 09:02:54.000000 armonik-3.8.2.dev395/src/armonik/worker/seqlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-06-06 09:02:54.000000 armonik-3.8.2.dev395/src/armonik/worker/taskhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-06 09:02:54.000000 armonik-3.8.2.dev395/src/armonik/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:10.828252 armonik-3.8.2.dev395/src/armonik.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-06 09:03:10.000000 armonik-3.8.2.dev395/src/armonik.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-06-06 09:03:10.000000 armonik-3.8.2.dev395/src/armonik.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:03:10.000000 armonik-3.8.2.dev395/src/armonik.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-06 09:03:10.000000 armonik-3.8.2.dev395/src/armonik.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 09:03:10.000000 armonik-3.8.2.dev395/src/armonik.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:16:40.913707 armonik-3.8.3.dev470/
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-19 08:16:40.913707 armonik-3.8.3.dev470/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-19 08:16:22.000000 armonik-3.8.3.dev470/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-19 08:16:22.000000 armonik-3.8.3.dev470/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 08:16:40.913707 armonik-3.8.3.dev470/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:16:40.897707 armonik-3.8.3.dev470/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:16:40.897707 armonik-3.8.3.dev470/src/armonik/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-19 08:16:22.000000 armonik-3.8.3.dev470/src/armonik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:16:40.901707 armonik-3.8.3.dev470/src/armonik/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-19 08:16:22.000000 armonik-3.8.3.dev470/src/armonik/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-19 08:16:22.000000 armonik-3.8.3.dev470/src/armonik/client/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-06-19 08:16:22.000000 armonik-3.8.3.dev470/src/armonik/client/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-19 08:16:22.000000 armonik-3.8.3.dev470/src/armonik/client/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:16:40.901707 armonik-3.8.3.dev470/src/armonik/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-19 08:16:22.000000 armonik-3.8.3.dev470/src/armonik/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-19 08:16:22.000000 armonik-3.8.3.dev470/src/armonik/common/enumwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-06-19 08:16:22.000000 armonik-3.8.3.dev470/src/armonik/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-19 08:16:22.000000 armonik-3.8.3.dev470/src/armonik/common/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:16:40.897707 armonik-3.8.3.dev470/src/armonik/protogen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:16:40.905707 armonik-3.8.3.dev470/src/armonik/protogen/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/applications_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/applications_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/applications_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/auth_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/auth_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/auth_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/events_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/events_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/events_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/partitions_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/partitions_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/partitions_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/results_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/results_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16128 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/results_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/sessions_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/sessions_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/sessions_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/submitter_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/submitter_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27332 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/submitter_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/tasks_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/tasks_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/tasks_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/versions_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/versions_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/client/versions_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:16:40.909707 armonik-3.8.3.dev470/src/armonik/protogen/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/agent_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/agent_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/agent_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/applications_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/applications_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/applications_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/auth_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/auth_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/auth_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/events_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/events_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/events_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/objects_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/objects_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/objects_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/partitions_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/partitions_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/partitions_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/result_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/result_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/result_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/results_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/results_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/results_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/session_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/session_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/session_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/sessions_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/sessions_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/sessions_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/sort_direction_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/sort_direction_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/sort_direction_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/submitter_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/submitter_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/submitter_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/task_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/task_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/task_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/tasks_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19219 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/tasks_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/tasks_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/versions_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/versions_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/versions_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/worker_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/worker_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/common/worker_common_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:16:40.909707 armonik-3.8.3.dev470/src/armonik/protogen/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/worker/agent_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/worker/agent_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/worker/agent_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/worker/worker_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/worker/worker_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-06-19 08:16:34.000000 armonik-3.8.3.dev470/src/armonik/protogen/worker/worker_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:16:40.913707 armonik-3.8.3.dev470/src/armonik/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-19 08:16:22.000000 armonik-3.8.3.dev470/src/armonik/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-19 08:16:22.000000 armonik-3.8.3.dev470/src/armonik/worker/seqlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-06-19 08:16:22.000000 armonik-3.8.3.dev470/src/armonik/worker/taskhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-19 08:16:22.000000 armonik-3.8.3.dev470/src/armonik/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:16:40.897707 armonik-3.8.3.dev470/src/armonik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-19 08:16:40.000000 armonik-3.8.3.dev470/src/armonik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-06-19 08:16:40.000000 armonik-3.8.3.dev470/src/armonik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:16:40.000000 armonik-3.8.3.dev470/src/armonik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-19 08:16:40.000000 armonik-3.8.3.dev470/src/armonik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 08:16:40.000000 armonik-3.8.3.dev470/src/armonik.egg-info/top_level.txt
```

### Comparing `armonik-3.8.2.dev395/PKG-INFO` & `armonik-3.8.3.dev470/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armonik
-Version: 3.8.2.dev395
+Version: 3.8.3.dev470
 Summary: GRPC python binding for the ArmoniK orchestrator API
 License: Apache v2.0 LICENSE
 Project-URL: Homepage, https://github.com/aneoconsulting/ArmoniK.Api
 Project-URL: Bug Tracker, https://github.com/aneoconsulting/ArmoniK/issues
 Keywords: cloud,HTC,gRPC,ArmoniK,Aneo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `armonik-3.8.2.dev395/README.md` & `armonik-3.8.3.dev470/README.md`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/pyproject.toml` & `armonik-3.8.3.dev470/pyproject.toml`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/client/submitter.py` & `armonik-3.8.3.dev470/src/armonik/client/submitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,25 +228,14 @@
         response_type = response.WhichOneof("type")
         if response_type == "ok":
             return ResultAvailability()
         if response_type == "error":
             return ResultAvailability(errors=[e.detail for e in response.error.errors])
         return None
 
-    def request_output_id(self, session_id: str) -> str:
-        """Request an output id
-
-        Args:
-            session_id: Session Id
-
-        Returns:
-            Output id
-        """
-        return f"{session_id}%{uuid.uuid4()}"
-
 
 def _to_request_stream_internal(request: TaskRequest, is_last: bool, chunk_max_size: int) -> Generator[CreateLargeTaskRequest, None, None]:
     """ Generate the CreateLargeTaskRequests for the given request
 
     Args:
         request: TaskRequest
         is_last: true if the request is the last one to send
```

### Comparing `armonik-3.8.2.dev395/src/armonik/client/tasks.py` & `armonik-3.8.3.dev470/src/armonik/client/tasks.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/common/enumwrapper.py` & `armonik-3.8.3.dev470/src/armonik/common/enumwrapper.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/common/helpers.py` & `armonik-3.8.3.dev470/src/armonik/common/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import timedelta, datetime, timezone
-from typing import List, Optional, cast
+from typing import List, Optional
 
 import google.protobuf.duration_pb2 as duration
 import google.protobuf.timestamp_pb2 as timestamp
 
 from ..protogen.common.submitter_common_pb2 import TaskFilter
 from .enumwrapper import TaskStatus
```

### Comparing `armonik-3.8.2.dev395/src/armonik/common/objects.py` & `armonik-3.8.3.dev470/src/armonik/common/objects.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     max_retries: int
     partition_id: Optional[str] = None
     application_name: Optional[str] = None
     application_version: Optional[str] = None
     application_namespace: Optional[str] = None
     application_service: Optional[str] = None
     engine_type: Optional[str] = None
-    options: Optional[Dict] = field(default_factory=dict)
+    options: Dict[str, str] = field(default_factory=dict)
 
     @classmethod
     def from_message(cls, task_options):
         return cls(max_duration=duration_to_timedelta(task_options.max_duration),
                    max_retries=task_options.max_retries,
                    priority=task_options.priority,
                    partition_id=task_options.partition_id,
@@ -62,31 +62,31 @@
             return WorkerOutput(ok=Empty())
         return WorkerOutput(error=WorkerOutput.Error(details=self.error))
 
 
 @dataclass()
 class TaskDefinition:
     payload: bytes
-    expected_output_ids: List[str]
+    expected_output_ids: List[str] = field(default_factory=list)
     data_dependencies: List[str] = field(default_factory=list)
 
     def __post_init__(self):
         if len(self.expected_output_ids) <= 0:
             raise ValueError("expected_output_ids must be not be empty")
 
 
 @dataclass()
 class Task:
     id: Optional[str] = None
     session_id: Optional[str] = None
     owner_pod_id: Optional[str] = None
-    parent_task_ids: Optional[List[str]] = None
-    data_dependencies: Optional[List[str]] = None
-    expected_output_ids: Optional[List[str]] = None
-    retry_of_ids: Optional[List[str]] = None
+    parent_task_ids: List[str] = field(default_factory=list)
+    data_dependencies: List[str] = field(default_factory=list)
+    expected_output_ids: List[str] = field(default_factory=list)
+    retry_of_ids: List[str] = field(default_factory=list)
     status: TaskStatus = TaskStatus.UNSPECIFIED
     status_message: Optional[str] = None
     options: Optional[TaskOptions] = None
     created_at: Optional[datetime] = None
     submitted_at: Optional[datetime] = None
     started_at: Optional[datetime] = None
     ended_at: Optional[datetime] = None
@@ -98,47 +98,48 @@
 
     def refresh(self, task_client) -> None:
         """Refresh the fields of this task object by using the given task client
 
         Args:
             task_client: ArmoniKTasks client
         """
-        result = task_client.get_task(self.id)
+        result : "Task" = task_client.get_task(self.id)
         self.session_id = result.session_id
         self.owner_pod_id = result.owner_pod_id
-        self.parent_task_ids = list(result.parent_task_ids)
-        self.data_dependencies = list(result.data_dependencies)
-        self.expected_output_ids = list(result.expected_output_ids)
-        self.retry_of_ids = list(result.retry_of_ids)
+        self.parent_task_ids = result.parent_task_ids
+        self.data_dependencies = result.data_dependencies
+        self.expected_output_ids = result.expected_output_ids
+        self.retry_of_ids = result.retry_of_ids
         self.status = TaskStatus(result.status)
         self.status_message = result.status_message
         self.options = result.options
         self.created_at = result.created_at
         self.submitted_at = result.submitted_at
         self.started_at = result.started_at
         self.ended_at = result.ended_at
         self.pod_ttl = result.pod_ttl
         self.output = result.output
         self.pod_hostname = result.pod_hostname
         self.received_at = result.received_at
         self.acquired_at = result.acquired_at
+        self.is_init = True
 
     @classmethod
     def from_message(cls, task_raw: TaskRaw) -> "Task":
         return cls(
             id=task_raw.id,
             session_id=task_raw.session_id,
             owner_pod_id=task_raw.owner_pod_id,
             parent_task_ids=list(task_raw.parent_task_ids),
             data_dependencies=list(task_raw.data_dependencies),
             expected_output_ids=list(task_raw.expected_output_ids),
             retry_of_ids=list(task_raw.retry_of_ids),
             status=TaskStatus(task_raw.status),
             status_message=task_raw.status_message,
-            options=task_raw.options,
+            options=TaskOptions.from_message(task_raw.options),
             created_at=timestamp_to_datetime(task_raw.created_at),
             submitted_at=timestamp_to_datetime(task_raw.submitted_at),
             started_at=timestamp_to_datetime(task_raw.started_at),
             ended_at=timestamp_to_datetime(task_raw.ended_at),
             pod_ttl=timestamp_to_datetime(task_raw.pod_ttl),
             output=Output(
                 error=(task_raw.output.error if not task_raw.output.success else None)),
```

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/client/applications_service_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/client/applications_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/client/applications_service_pb2_grpc.py` & `armonik-3.8.3.dev470/src/armonik/protogen/client/applications_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/client/auth_service_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/client/auth_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/client/auth_service_pb2_grpc.py` & `armonik-3.8.3.dev470/src/armonik/protogen/client/auth_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/client/events_service_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/client/events_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/client/events_service_pb2_grpc.py` & `armonik-3.8.3.dev470/src/armonik/protogen/client/events_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/client/partitions_service_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/client/partitions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/client/partitions_service_pb2_grpc.py` & `armonik-3.8.3.dev470/src/armonik/protogen/client/partitions_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/client/results_service_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/client/results_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/client/results_service_pb2_grpc.py` & `armonik-3.8.3.dev470/src/armonik/protogen/client/results_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/client/sessions_service_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/client/sessions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/client/sessions_service_pb2_grpc.py` & `armonik-3.8.3.dev470/src/armonik/protogen/client/sessions_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/client/submitter_service_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/client/submitter_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/client/submitter_service_pb2_grpc.py` & `armonik-3.8.3.dev470/src/armonik/protogen/client/submitter_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/client/tasks_service_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/client/tasks_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/client/tasks_service_pb2_grpc.py` & `armonik-3.8.3.dev470/src/armonik/protogen/client/tasks_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/client/versions_service_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/client/versions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/client/versions_service_pb2_grpc.py` & `armonik-3.8.3.dev470/src/armonik/protogen/client/versions_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/agent_common_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/common/agent_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/agent_common_pb2.pyi` & `armonik-3.8.3.dev470/src/armonik/protogen/common/agent_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/applications_common_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/common/applications_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/applications_common_pb2.pyi` & `armonik-3.8.3.dev470/src/armonik/protogen/common/applications_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/auth_common_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/common/auth_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/auth_common_pb2.pyi` & `armonik-3.8.3.dev470/src/armonik/protogen/common/auth_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/events_common_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/common/events_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/events_common_pb2.pyi` & `armonik-3.8.3.dev470/src/armonik/protogen/common/events_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/objects_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/common/objects_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/objects_pb2.pyi` & `armonik-3.8.3.dev470/src/armonik/protogen/common/objects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/partitions_common_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/common/partitions_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/partitions_common_pb2.pyi` & `armonik-3.8.3.dev470/src/armonik/protogen/common/partitions_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/result_status_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/common/result_status_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/results_common_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/common/results_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/results_common_pb2.pyi` & `armonik-3.8.3.dev470/src/armonik/protogen/common/results_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/session_status_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/common/session_status_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/sessions_common_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/common/sessions_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/sessions_common_pb2.pyi` & `armonik-3.8.3.dev470/src/armonik/protogen/common/sessions_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/sort_direction_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/common/sort_direction_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/submitter_common_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/common/submitter_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/submitter_common_pb2.pyi` & `armonik-3.8.3.dev470/src/armonik/protogen/common/submitter_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/task_status_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/common/task_status_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/task_status_pb2.pyi` & `armonik-3.8.3.dev470/src/armonik/protogen/common/task_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/tasks_common_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/common/tasks_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/tasks_common_pb2.pyi` & `armonik-3.8.3.dev470/src/armonik/protogen/common/tasks_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/versions_common_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/common/versions_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/versions_common_pb2.pyi` & `armonik-3.8.3.dev470/src/armonik/protogen/common/versions_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/worker_common_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/common/worker_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/common/worker_common_pb2.pyi` & `armonik-3.8.3.dev470/src/armonik/protogen/common/worker_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/worker/agent_service_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/worker/agent_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/worker/agent_service_pb2_grpc.py` & `armonik-3.8.3.dev470/src/armonik/protogen/worker/agent_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/worker/worker_service_pb2.py` & `armonik-3.8.3.dev470/src/armonik/protogen/worker/worker_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/protogen/worker/worker_service_pb2_grpc.py` & `armonik-3.8.3.dev470/src/armonik/protogen/worker/worker_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev395/src/armonik/worker/seqlogger.py` & `armonik-3.8.3.dev470/src/armonik/worker/seqlogger.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         Args:
             message: Message content, can contain '{name}' where name is a keyword argument given to this function (see kwargs)
             exc_info: Optional exc_info to add to an exception record, can be an exception, a boolean (to add the result of sys.exc_info() automatically if true), or the tuple given by sys.exc_info()
             **kwargs: Keyword arguments added to the record
         """
         self.log(logging.ERROR, message, exc_info=exc_info, **kwargs)
 
-    def log(self, level: int, message: str, exc_info: Union[BaseException, Tuple[Type[BaseException], BaseException, Optional[TracebackType]], bool, None] = None, **kwargs):
+    def log(self, level: int, message: str, exc_info: Union[BaseException, Union[Tuple[Union[Type[BaseException], None], Union[BaseException, None], Optional[TracebackType]], None], bool, None] = None, **kwargs):
         """ Log a message
 
         Args:
             level: level of the message
             message: Message content, can contain '{name}' where name is an keyword argument given to this function (see kwargs)
             exc_info: Optional exc_info to add to an exception record, can be an exception, a boolean (to add the result of sys.exc_info() automatically if true), or the tuple given by sys.exc_info()
             **kwargs: Keyword arguments added to the record
@@ -111,16 +111,15 @@
                     "@mt": message,
                 }
                 if exc_info:
                     if isinstance(exc_info, bool):
                         exc_info = sys.exc_info()
                     elif isinstance(exc_info, BaseException):
                         exc_info = (type(exc_info), exc_info, exc_info.__traceback__)
-                    exc_info = "\n".join(traceback.format_exception(*exc_info))
-                    payload["@x"] = exc_info
+                    payload["@x"] = "\n".join(traceback.format_exception(*exc_info))
                 for k, v in kwargs:
                     if k.startswith("@"):
                         k = "@"+k
                     payload[k] = str(v)
                 self._logger.log(level, msg=json.dumps(payload))
         except Exception as e:
             print(f"Couldn't log message : {e}")
```

### Comparing `armonik-3.8.2.dev395/src/armonik/worker/taskhandler.py` & `armonik-3.8.3.dev470/src/armonik/worker/taskhandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import uuid
-from typing import Optional, Dict, List, Tuple, Union
+from typing import Optional, Dict, List, Tuple, Union, cast
 
 from ..common import TaskOptions, TaskDefinition, Task
-from ..protogen.common.agent_common_pb2 import Result, CreateTaskRequest
+from ..protogen.common.agent_common_pb2 import Result, CreateTaskRequest, CreateResultsMetaDataRequest, CreateResultsMetaDataResponse
 from ..protogen.common.objects_pb2 import TaskRequest, InitKeyedDataStream, DataChunk, InitTaskRequest, TaskRequestHeader, Configuration
 from ..protogen.worker.agent_service_pb2_grpc import AgentStub
 
 
 class TaskHandler:
     def __init__(self, request_iterator, agent_client):
         self.request_iterator = request_iterator
@@ -31,20 +31,20 @@
         if current is None:
             raise ValueError("Request stream ended unexpectedly")
 
         if current.compute.WhichOneof("type") != "init_request":
             raise ValueError("Expected a Compute request type with InitRequest to start the stream.")
 
         init_request = current.compute.init_request
-        self.session_id: str = init_request.session_id
-        self.task_id: str = init_request.task_id
-        self.task_options: TaskOptions = TaskOptions.from_message(init_request.task_options)
+        self.session_id = init_request.session_id
+        self.task_id = init_request.task_id
+        self.task_options = TaskOptions.from_message(init_request.task_options)
         self.expected_results = list(init_request.expected_output_keys)
         self.configuration = init_request.configuration
-        self.token: str = current.communication_token
+        self.token = current.communication_token
 
         datachunk = init_request.payload
         self.payload.extend(datachunk.data)
         while not datachunk.data_complete:
             current = next(self.request_iterator, None)
             if current is None:
                 raise ValueError("Request stream ended unexpectedly")
@@ -94,15 +94,15 @@
 
         for t in tasks:
             task_request = TaskRequest()
             task_request.expected_output_keys.extend(t.expected_output_ids)
             task_request.data_dependencies.extend(t.data_dependencies)
             task_request.payload = t.payload
             task_requests.append(task_request)
-
+        assert self.configuration is not None
         create_tasks_reply = self._client.CreateTask(_to_request_stream(task_requests, self.token, task_options.to_message() if task_options is not None else None, self.configuration.data_chunk_max_size))
         ret = create_tasks_reply.WhichOneof("Response")
         if ret is None or ret == "error":
             raise Exception(f'Issue with server when submitting tasks : {create_tasks_reply.error}')
         elif ret == "creation_status_list":
             tasks_created = []
             tasks_creation_failed = []
@@ -111,31 +111,24 @@
                     tasks_created.append(Task(id=creation_status.task_info.task_id, session_id=self.session_id, expected_output_ids=[k for k in creation_status.task_info.expected_output_keys], data_dependencies=[k for k in creation_status.task_info.data_dependencies]))
                 else:
                     tasks_creation_failed.append(creation_status.error)
         else:
             raise Exception("Unknown value")
         return tasks_created, tasks_creation_failed
 
-    def request_output_id(self) -> str:
-        """Request an output id
-
-                Returns:
-                    Output id
-        """
-        return f"{self.token}%{uuid.uuid4()}"
-
     def send_result(self, key: str, data: Union[bytes, bytearray]) -> None:
         """ Send task result
 
         Args:
             key: Result key
             data: Result data
         """
         def result_stream():
             res = Result(communication_token=self.token, init=InitKeyedDataStream(key=key))
+            assert self.configuration is not None
             yield res
             start = 0
             data_len = len(data)
             while start < data_len:
                 chunksize = min(self.configuration.data_chunk_max_size, data_len - start)
                 res = Result(communication_token=self.token, data=DataChunk(data=data[start:start + chunksize]))
                 yield res
@@ -144,14 +137,18 @@
             yield res
             res = Result(communication_token=self.token, init=InitKeyedDataStream(last_result=True))
             yield res
 
         result_reply = self._client.SendResult(result_stream())
         if result_reply.WhichOneof("type") == "error":
             raise Exception(f"Cannot send result id={key}")
+    
+    def get_results_ids(self, names : List[str]) -> Dict[str, str]:
+        return {r.name : r.result_id for r in cast(CreateResultsMetaDataResponse, self._client.CreateResultsMetaData(CreateResultsMetaDataRequest(results=[CreateResultsMetaDataRequest.ResultCreate(name = n) for n in names], session_id=self.session_id, communication_token=self.token))).results}
+
 
 
 def _to_request_stream_internal(request, communication_token, is_last, chunk_max_size):
     req = CreateTaskRequest(
         init_task=InitTaskRequest(
             header=TaskRequestHeader(
                 data_dependencies=request.data_dependencies,
```

### Comparing `armonik-3.8.2.dev395/src/armonik/worker/worker.py` & `armonik-3.8.3.dev470/src/armonik/worker/worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import traceback
 from concurrent import futures
-from typing import Callable
+from typing import Callable, Union
 
 import grpc
 from grpc import Channel
 
 from .seqlogger import ClefLogger
 from ..common import Output, HealthCheckStatus
 from ..protogen.common.objects_pb2 import Empty
@@ -41,15 +41,15 @@
         """
         server = grpc.server(futures.ThreadPoolExecutor(max_workers=1))
         add_WorkerServicer_to_server(self, server)
         server.add_insecure_port(endpoint)
         server.start()
         server.wait_for_termination()
 
-    def Process(self, request_iterator, context) -> ProcessReply:
+    def Process(self, request_iterator, context) -> Union[ProcessReply, None]:
         try:
             self._logger.debug("Received task")
             task_handler = TaskHandler.create(request_iterator, self._client)
             return ProcessReply(output=self.processing_function(task_handler).to_message())
         except Exception as e:
             self._logger.exception(f"Failed task {''.join(traceback.format_exception(type(e) ,e, e.__traceback__))}", exc_info=e)
```

### Comparing `armonik-3.8.2.dev395/src/armonik.egg-info/PKG-INFO` & `armonik-3.8.3.dev470/src/armonik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armonik
-Version: 3.8.2.dev395
+Version: 3.8.3.dev470
 Summary: GRPC python binding for the ArmoniK orchestrator API
 License: Apache v2.0 LICENSE
 Project-URL: Homepage, https://github.com/aneoconsulting/ArmoniK.Api
 Project-URL: Bug Tracker, https://github.com/aneoconsulting/ArmoniK/issues
 Keywords: cloud,HTC,gRPC,ArmoniK,Aneo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `armonik-3.8.2.dev395/src/armonik.egg-info/SOURCES.txt` & `armonik-3.8.3.dev470/src/armonik.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 src/armonik/_version.py
 src/armonik.egg-info/PKG-INFO
 src/armonik.egg-info/SOURCES.txt
 src/armonik.egg-info/dependency_links.txt
 src/armonik.egg-info/requires.txt
 src/armonik.egg-info/top_level.txt
 src/armonik/client/__init__.py
+src/armonik/client/results.py
 src/armonik/client/submitter.py
 src/armonik/client/tasks.py
 src/armonik/common/__init__.py
 src/armonik/common/enumwrapper.py
 src/armonik/common/helpers.py
 src/armonik/common/objects.py
 src/armonik/protogen/client/__init__.py
```

