# Comparing `tmp/admobilizeapis-2023.2.7.post3.tar.gz` & `tmp/admobilizeapis-2023.6.19.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/admobilizeapis-2023.2.7.post3.tar", last modified: Tue Feb  7 18:37:18 2023, max compression
+gzip compressed data, was "dist/admobilizeapis-2023.6.19.post1.tar", last modified: Mon Jun 19 18:19:16 2023, max compression
```

## Comparing `admobilizeapis-2023.2.7.post3.tar` & `admobilizeapis-2023.6.19.post1.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/
--rw-r--r--   0 root         (0) root         (0)     1201 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/README.md
--rw-r--r--   0 root         (0) root         (0)     1293 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/signagelive/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/signagelive/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)     3240 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/signagelive/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/signagelive/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    18378 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    24106 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/signagelive/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/signagelive/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha2/
--rw-r--r--   0 root         (0) root         (0)    18992 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10609 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha2/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha2/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28083 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)    15271 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9576 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14877 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha3/
--rw-r--r--   0 root         (0) root         (0)    29786 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py
--rw-r--r--   0 root         (0) root         (0)    13543 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha3/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha3/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41623 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1/
--rw-r--r--   0 root         (0) root         (0)    28693 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1/device_manager_pb2.py
--rw-r--r--   0 root         (0) root         (0)    15461 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39106 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v2/
--rw-r--r--   0 root         (0) root         (0)    76701 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v2/device_manager_pb2.py
--rw-r--r--   0 root         (0) root         (0)    20320 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v2/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v2/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)    99455 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/ayuda/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/ayuda/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)    21203 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    15801 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3157 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/ayuda/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/ayuda/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/ayuda/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/ayuda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/malos/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/malos/v1/
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/malos/v1/maloseye_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/malos/v1/driver_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4590 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/malos/v1/driver_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6136 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/malos/v1/maloseye_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/malos/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/malos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/query/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/query/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)    28346 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/query/v1alpha1/query_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14646 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/query/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    31149 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/query/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/query/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/query/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/billing/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/billing/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)     2506 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/billing/v1alpha1/billing_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/billing/v1alpha1/billing_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/billing/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/billing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/salestool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/salestool/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)     5528 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4784 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/salestool/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/salestool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/mlmodel/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/mlmodel/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)     6478 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     5542 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/mlmodel/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/mlmodel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/cmsintegrations/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/cmsintegrations/v1/
--rw-r--r--   0 root         (0) root         (0)    24348 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    29481 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    10026 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/cmsintegrations/v1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/cmsintegrations/v1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/cmsintegrations/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/cmsintegrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/common/
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/common/job_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2623 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/common/admobilize_types_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2897 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/common/job_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4485 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/common/entity_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/common/admobilize_types_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/common/entity_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/vision/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/vision/v1/
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/vision/v1/vision_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/vision/v1/model_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2515 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/vision/v1/vision_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4194 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/vision/v1/model_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/vision/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2912 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/vision/v1/vision_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    25636 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/vision/v1/vision_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/vision/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/wifi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/wifi/v1/
--rw-r--r--   0 root         (0) root         (0)     2457 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/wifi/v1/wifi_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/wifi/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/wifi/v1/wifi_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/wifi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/iam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/iam/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)    25837 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/iam/v1alpha1/iam_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    35932 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4250 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/iam/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/iam/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/iam/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/iam/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/brightauthor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/brightauthor/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)    22301 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/brightauthor/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/brightauthor/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16652 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/brightauthor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/admprovider/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/admprovider/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)    22477 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6954 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/admprovider/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/admprovider/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     8758 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/admprovider/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/admprovider/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/broadsign/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/broadsign/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)    16356 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3174 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/broadsign/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    21841 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/broadsign/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/broadsign/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/broadsign/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/datagateway/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/datagateway/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)     8708 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/datagateway/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8861 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/datagateway/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/notification/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/notification/v1beta1/
--rw-r--r--   0 root         (0) root         (0)    10396 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/notification/v1beta1/notification_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6645 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/notification/v1beta1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/notification/v1beta1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/notification/v1beta1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14597 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/notification/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/proto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/google/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilize/google/longrunning/
--rw-r--r--   0 root         (0) root         (0)    10932 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/google/longrunning/operations_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     8090 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/google/longrunning/operations_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/google/longrunning/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/google/__init__.py
--rw-r--r--   0 root         (0) root         (0)       56 2023-02-07 18:37:17.000000 admobilizeapis-2023.2.7.post3/admobilize/__init__.py
--rw-r--r--   0 root         (0) root         (0)      848 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilizeapis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilizeapis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilizeapis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     6814 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilizeapis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      848 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilizeapis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       11 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilizeapis.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-02-07 18:37:18.000000 admobilizeapis-2023.2.7.post3/admobilizeapis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/google/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/google/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/google/longrunning/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/google/longrunning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8090 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/google/longrunning/operations_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10932 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/google/longrunning/operations_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/wifi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/wifi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/wifi/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/wifi/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/wifi/v1/wifi_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/wifi/v1/wifi_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/datagateway/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/datagateway/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/datagateway/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/datagateway/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8861 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8708 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/iam/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/iam/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/iam/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/iam/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/iam/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    25837 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4250 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/iam/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    35932 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/notification/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/notification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/notification/v1beta1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/notification/v1beta1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/notification/v1beta1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6645 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/notification/v1beta1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10396 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/notification/v1beta1/notification_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14597 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/vision/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/vision/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/vision/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/vision/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/vision/v1/model_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/vision/v1/vision_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/vision/v1/vision_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/vision/v1/vision_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4194 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/vision/v1/model_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    25636 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/vision/v1/vision_pb2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/mlmodel/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/mlmodel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/mlmodel/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)     6478 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/mlmodel/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5542 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/salestool/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/salestool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/salestool/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/salestool/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4784 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     5528 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    15461 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    39106 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    28693 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    10609 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28083 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    18992 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v2/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    20359 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v2/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    99455 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    76701 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha3/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    13543 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    41623 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    29786 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9576 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14877 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    15271 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/admprovider/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/admprovider/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/admprovider/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/admprovider/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6954 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    22477 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     8758 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/malos/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/malos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/malos/v1/
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/malos/v1/driver_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/malos/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4590 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/malos/v1/driver_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6136 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/malos/v1/maloseye_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/malos/v1/maloseye_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/query/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/query/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/query/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/query/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/query/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    14646 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/query/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    31149 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    28346 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/query/v1alpha1/query_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/ayuda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/ayuda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/ayuda/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/ayuda/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    15801 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    21203 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3157 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/signagelive/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/signagelive/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/signagelive/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/signagelive/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18378 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    24106 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3240 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/common/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/common/job_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/common/admobilize_types_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4485 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/common/entity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2623 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/common/admobilize_types_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2897 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/common/job_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/common/entity_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/billing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/billing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/billing/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/billing/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/billing/v1alpha1/billing_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/billing/v1alpha1/billing_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/brightauthor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/brightauthor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/brightauthor/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)    22301 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/brightauthor/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16652 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/cmsintegrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/cmsintegrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/cmsintegrations/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/cmsintegrations/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/cmsintegrations/v1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    29481 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    10026 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/cmsintegrations/v1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    24348 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/broadsign/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/broadsign/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/broadsign/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/broadsign/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21841 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3174 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16356 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      849 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilizeapis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilizeapis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilizeapis.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)     6814 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilizeapis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      849 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilizeapis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilizeapis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/admobilizeapis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1293 2023-06-19 18:19:15.000000 admobilizeapis-2023.6.19.post1/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 18:19:16.000000 admobilizeapis-2023.6.19.post1/setup.cfg
```

### Comparing `admobilizeapis-2023.2.7.post3/README.md` & `admobilizeapis-2023.6.19.post1/README.md`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/setup.py` & `admobilizeapis-2023.6.19.post1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 install_requires = ["google-api-core >= 1.6.0, < 2.0.0dev", "protobuf >= 3.6.0, < 4.0"]
 
 extras_require = {"grpc": ["grpcio>=1.2.0"]}
 
 setup(
     name="admobilizeapis",
-    version='2023.02.07r3',
+    version='2023.06.19r1',
     author="AdMobilize Team",
     author_email="devel@admobilize.com",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python",
```

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/signagelive/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1/device_manager_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1/resources_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v2/device_manager_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v2/resources_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v2/resources_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
-from admobilize.proto.common import job_pb2 as admobilize_dot_common_dot_job__pb2
 from admobilize.proto.common import admobilize_types_pb2 as admobilize_dot_common_dot_admobilize__types__pb2
+from admobilize.proto.common import job_pb2 as admobilize_dot_common_dot_job__pb2
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.admobilize/devicemanagement/v2/resources.proto\x12\x1e\x61\x64mobilize.devicemanagement.v2\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1b\x61\x64mobilize/common/job.proto\x1a(admobilize/common/admobilize_types.proto\"Z\n\nLogMessage\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08severity\x18\x02 \x01(\t\x12\x0b\n\x03msg\x18\x03 \x01(\t\"\xf5\x01\n\x08Solution\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x1b\n\x13\x62igquery_table_name\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\x12!\n\x19\x64\x65\x66\x61ult_install_config_id\x18\x06 \x01(\t\x12\x0e\n\x06schema\x18\x07 \x01(\t\x12/\n\x0b\x63reate_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bupdate_time\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x88\x02\n\x15SolutionConfiguration\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\'\n\x06\x63onfig\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x34\n\x0bsolution_id\x18\x04 \x01(\x0e\x32\x1f.admobilize.common.SolutionName\x12\x14\n\x0c\x64isplay_name\x18\x05 \x01(\t\x12/\n\x0b\x63reate_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bupdate_time\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xb5\x05\n\x12ProjectPreferences\x12P\n\nspeed_unit\x18\x01 \x01(\x0e\x32<.admobilize.devicemanagement.v2.ProjectPreferences.SpeedUnit\x12\x18\n\x10max_session_time\x18\x02 \x01(\x02\x12\x16\n\x0emax_dwell_time\x18\x03 \x01(\x02\x12\x16\n\x0eview_threshold\x18\x04 \x01(\x02\x12\x13\n\x0bview_metric\x18\x05 \x01(\t\x12\x10\n\x08timezone\x18\x06 \x01(\t\x12\x1d\n\x15min_confidence_gender\x18\x07 \x01(\x02\x12\x1d\n\x15max_confidence_gender\x18\x08 \x01(\x02\x12\x1a\n\x12min_confidence_age\x18\t \x01(\x02\x12\x1a\n\x12max_confidence_age\x18\n \x01(\x02\x12\x1e\n\x16min_confidence_emotion\x18\x0b \x01(\x02\x12\x1e\n\x16max_confidence_emotion\x18\x0c \x01(\x02\x12 \n\x18\x65nable_anomaly_detection\x18\r \x01(\x08\x12\x65\n\x12vehicle_multiplier\x18\x0e \x03(\x0b\x32I.admobilize.devicemanagement.v2.ProjectPreferences.VehicleMultiplierEntry\x1a\x38\n\x16VehicleMultiplierEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"c\n\tSpeedUnit\x12\x1a\n\x16SPEED_UNIT_NOT_DEFINED\x10\x00\x12\x12\n\x0eMILES_PER_HOUR\x10\x01\x12\x0f\n\x0bKM_PER_HOUR\x10\x02\x12\x15\n\x11METERS_PER_SECOND\x10\x03\"\xc6\x04\n\x07Project\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x03 \x01(\t\x12\x10\n\x08owner_id\x18\x04 \x01(\t\x12\x43\n\x06labels\x18\x05 \x03(\x0b\x32\x33.admobilize.devicemanagement.v2.Project.LabelsEntry\x12\x0c\n\x04tags\x18\x06 \x03(\t\x12\x15\n\rdevices_count\x18\x07 \x01(\x05\x12/\n\x0b\x63reate_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bupdate_time\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12@\n\x14\x65nabled_integrations\x18\n \x03(\x0e\x32\".admobilize.common.IntegrationName\x12:\n\x11\x65nabled_solutions\x18\x0b \x03(\x0e\x32\x1f.admobilize.common.SolutionName\x12G\n\x0bpreferences\x18\x0c \x01(\x0b\x32\x32.admobilize.devicemanagement.v2.ProjectPreferences\x12\x1a\n\x12provisioning_token\x18\r \x01(\t\x12\x1b\n\x13\x64\x65vices_count_limit\x18\x0e \x01(\x05\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x91\x03\n\x0b\x44\x65viceState\x12\x1b\n\x13\x61\x64mprovider_version\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61lena\x18\x02 \x01(\x08\x12\x10\n\x08platform\x18\x03 \x01(\t\x12\x10\n\x08timezone\x18\x04 \x01(\t\x12.\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x16\x64\x65tections_since_start\x18\x06 \x01(\x04\x12\x37\n\x13last_detection_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rmalos_running\x18\x08 \x01(\x08\x12\x1a\n\x12\x64\x65tections_to_send\x18\t \x01(\x04\x12\x0e\n\x06status\x18\n \x01(\t\x12\x15\n\rmalos_version\x18\x0b \x01(\t\x12\x1d\n\x15\x64\x65tections_per_second\x18\x0c \x01(\x02\x12/\n\x0bupdate_time\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xd3\x01\n\x0c\x44\x65viceConfig\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x30\n\x0fsolution_config\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\"\n\x1a\x64\x65\x66\x61ult_solution_config_id\x18\x03 \x01(\t\x12/\n\x0e\x64\x65\x66\x61ult_config\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12.\n\rcustom_config\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\"(\n\tPublicKey\x12\x0e\n\x06\x66ormat\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\"a\n\x11\x44\x65viceCredentials\x12\x0c\n\x04name\x18\x01 \x01(\t\x12>\n\x0bpublic_keys\x18\x02 \x03(\x0b\x32).admobilize.devicemanagement.v2.PublicKey\"\xe2\x02\n\x13\x44\x65viceIotCoreStatus\x12\x39\n\x15last_config_send_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0flast_event_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0flast_error_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\x13last_heartbeat_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x14last_config_ack_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0flast_state_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xb5\x05\n\x06\x44\x65vice\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x03 \x01(\t\x12\x12\n\ncreator_id\x18\x04 \x01(\t\x12\x12\n\nproject_id\x18\x05 \x01(\t\x12\x1a\n\x12provisioning_token\x18\x06 \x01(\t\x12#\n\x1bprovisioning_token_was_used\x18\x07 \x01(\x08\x12/\n\x0b\x63reate_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bupdate_time\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x42\n\x06labels\x18\n \x03(\x0b\x32\x32.admobilize.devicemanagement.v2.Device.LabelsEntry\x12\x0c\n\x04tags\x18\x0b \x03(\t\x12\x10\n\x08\x61rchived\x18\x0c \x01(\x08\x12\x31\n\x08solution\x18\r \x01(\x0e\x32\x1f.admobilize.common.SolutionName\x12\x38\n\x0cintegrations\x18\x0e \x03(\x0e\x32\".admobilize.common.IntegrationName\x12:\n\x05state\x18\x0f \x01(\x0b\x32+.admobilize.devicemanagement.v2.DeviceState\x12\x1a\n\x12\x65nable_auto_update\x18\x10 \x01(\x08\x12\x10\n\x08has_wifi\x18\x11 \x01(\x08\x12\x46\n\x0f\x64\x65vice_comments\x18\x12 \x03(\x0b\x32-.admobilize.devicemanagement.v2.DeviceComment\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"N\n\rDeviceComment\x12\x0c\n\x04text\x18\x01 \x01(\t\x12/\n\x0b\x63reate_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x8c\x01\n\x13\x44\x65viceWithPublicKey\x12\x36\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32&.admobilize.devicemanagement.v2.Device\x12=\n\npublic_key\x18\x02 \x01(\x0b\x32).admobilize.devicemanagement.v2.PublicKey\"\x88\x02\n\x07License\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x31\n\x08solution\x18\x03 \x01(\x0e\x32\x1f.admobilize.common.SolutionName\x12\x11\n\tdevice_id\x18\x04 \x01(\t\x12.\n\nvalid_from\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bvalid_until\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1a\n\x12\x61\x63\x63ount_admin_name\x18\x07 \x01(\t\x12\x12\n\nproject_id\x18\x08 \x01(\t\x12\x0c\n\x04\x64\x65mo\x18\t \x01(\x08\"\x89\x02\n\x13MoveDevicesMetadata\x12/\n\x0b\x63reate_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ndevice_ids\x18\x03 \x03(\t\x12\x1e\n\x16\x64\x65stination_project_id\x18\x04 \x01(\t\x12\x19\n\x11source_project_id\x18\x05 \x01(\t\x12$\n\x04jobs\x18\x06 \x03(\x0b\x32\x16.admobilize.common.Job\x12\x1e\n\x16requested_cancellation\x18\x07 \x01(\x08\"\xa5\x02\n\x1aRestoreDevicesDataMetadata\x12/\n\x0b\x63reate_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ndevice_ids\x18\x03 \x03(\t\x12\x1e\n\x16\x64\x65stination_project_id\x18\x04 \x01(\t\x12\x1c\n\x14\x64\x65stination_table_id\x18\x05 \x01(\t\x12\x10\n\x08truncate\x18\x06 \x01(\x08\x12$\n\x04jobs\x18\x07 \x03(\x0b\x32\x16.admobilize.common.Job\x12\x1e\n\x16requested_cancellation\x18\x08 \x01(\x08\"U\n\x11\x41WSIoTCredentials\x12\x17\n\x0f\x63\x65rtificate_pem\x18\x01 \x01(\t\x12\x12\n\npublic_key\x18\x02 \x01(\t\x12\x13\n\x0bprivate_key\x18\x03 \x01(\tB\xa0\x01\n\"com.admobilize.devicemanagement.v2B\x0b\x44\x65viceProtoP\x01ZBbitbucket.org/admobilize/admobilizeapis-go/pkg/devicemanagement/v2\xa2\x02\x05\x41\x44MDM\xaa\x02\x1e\x41\x64Mobilize.DeviceManagement.V2b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.admobilize/devicemanagement/v2/resources.proto\x12\x1e\x61\x64mobilize.devicemanagement.v2\x1a(admobilize/common/admobilize_types.proto\x1a\x1b\x61\x64mobilize/common/job.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"Z\n\nLogMessage\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08severity\x18\x02 \x01(\t\x12\x0b\n\x03msg\x18\x03 \x01(\t\"\xf5\x01\n\x08Solution\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x1b\n\x13\x62igquery_table_name\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\x12!\n\x19\x64\x65\x66\x61ult_install_config_id\x18\x06 \x01(\t\x12\x0e\n\x06schema\x18\x07 \x01(\t\x12/\n\x0b\x63reate_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bupdate_time\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x88\x02\n\x15SolutionConfiguration\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\'\n\x06\x63onfig\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x34\n\x0bsolution_id\x18\x04 \x01(\x0e\x32\x1f.admobilize.common.SolutionName\x12\x14\n\x0c\x64isplay_name\x18\x05 \x01(\t\x12/\n\x0b\x63reate_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bupdate_time\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xb5\x05\n\x12ProjectPreferences\x12P\n\nspeed_unit\x18\x01 \x01(\x0e\x32<.admobilize.devicemanagement.v2.ProjectPreferences.SpeedUnit\x12\x18\n\x10max_session_time\x18\x02 \x01(\x02\x12\x16\n\x0emax_dwell_time\x18\x03 \x01(\x02\x12\x16\n\x0eview_threshold\x18\x04 \x01(\x02\x12\x13\n\x0bview_metric\x18\x05 \x01(\t\x12\x10\n\x08timezone\x18\x06 \x01(\t\x12\x1d\n\x15min_confidence_gender\x18\x07 \x01(\x02\x12\x1d\n\x15max_confidence_gender\x18\x08 \x01(\x02\x12\x1a\n\x12min_confidence_age\x18\t \x01(\x02\x12\x1a\n\x12max_confidence_age\x18\n \x01(\x02\x12\x1e\n\x16min_confidence_emotion\x18\x0b \x01(\x02\x12\x1e\n\x16max_confidence_emotion\x18\x0c \x01(\x02\x12 \n\x18\x65nable_anomaly_detection\x18\r \x01(\x08\x12\x65\n\x12vehicle_multiplier\x18\x0e \x03(\x0b\x32I.admobilize.devicemanagement.v2.ProjectPreferences.VehicleMultiplierEntry\x1a\x38\n\x16VehicleMultiplierEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"c\n\tSpeedUnit\x12\x1a\n\x16SPEED_UNIT_NOT_DEFINED\x10\x00\x12\x12\n\x0eMILES_PER_HOUR\x10\x01\x12\x0f\n\x0bKM_PER_HOUR\x10\x02\x12\x15\n\x11METERS_PER_SECOND\x10\x03\"\xc6\x04\n\x07Project\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x03 \x01(\t\x12\x10\n\x08owner_id\x18\x04 \x01(\t\x12\x43\n\x06labels\x18\x05 \x03(\x0b\x32\x33.admobilize.devicemanagement.v2.Project.LabelsEntry\x12\x0c\n\x04tags\x18\x06 \x03(\t\x12\x15\n\rdevices_count\x18\x07 \x01(\x05\x12/\n\x0b\x63reate_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bupdate_time\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12@\n\x14\x65nabled_integrations\x18\n \x03(\x0e\x32\".admobilize.common.IntegrationName\x12:\n\x11\x65nabled_solutions\x18\x0b \x03(\x0e\x32\x1f.admobilize.common.SolutionName\x12G\n\x0bpreferences\x18\x0c \x01(\x0b\x32\x32.admobilize.devicemanagement.v2.ProjectPreferences\x12\x1a\n\x12provisioning_token\x18\r \x01(\t\x12\x1b\n\x13\x64\x65vices_count_limit\x18\x0e \x01(\x05\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xa2\x03\n\x0b\x44\x65viceState\x12\x1b\n\x13\x61\x64mprovider_version\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61lena\x18\x02 \x01(\x08\x12\x10\n\x08platform\x18\x03 \x01(\t\x12\x10\n\x08timezone\x18\x04 \x01(\t\x12.\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x16\x64\x65tections_since_start\x18\x06 \x01(\x04\x12\x37\n\x13last_detection_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rmalos_running\x18\x08 \x01(\x08\x12\x1a\n\x12\x64\x65tections_to_send\x18\t \x01(\x04\x12\x0e\n\x06status\x18\n \x01(\t\x12\x15\n\rmalos_version\x18\x0b \x01(\t\x12\x1d\n\x15\x64\x65tections_per_second\x18\x0c \x01(\x02\x12/\n\x0bupdate_time\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07managed\x18\x0e \x01(\x08\"\xd3\x01\n\x0c\x44\x65viceConfig\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x30\n\x0fsolution_config\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\"\n\x1a\x64\x65\x66\x61ult_solution_config_id\x18\x03 \x01(\t\x12/\n\x0e\x64\x65\x66\x61ult_config\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12.\n\rcustom_config\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\"(\n\tPublicKey\x12\x0e\n\x06\x66ormat\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\"a\n\x11\x44\x65viceCredentials\x12\x0c\n\x04name\x18\x01 \x01(\t\x12>\n\x0bpublic_keys\x18\x02 \x03(\x0b\x32).admobilize.devicemanagement.v2.PublicKey\"\xe2\x02\n\x13\x44\x65viceIotCoreStatus\x12\x39\n\x15last_config_send_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0flast_event_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0flast_error_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\x13last_heartbeat_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x14last_config_ack_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0flast_state_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xb5\x05\n\x06\x44\x65vice\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x03 \x01(\t\x12\x12\n\ncreator_id\x18\x04 \x01(\t\x12\x12\n\nproject_id\x18\x05 \x01(\t\x12\x1a\n\x12provisioning_token\x18\x06 \x01(\t\x12#\n\x1bprovisioning_token_was_used\x18\x07 \x01(\x08\x12/\n\x0b\x63reate_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bupdate_time\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x42\n\x06labels\x18\n \x03(\x0b\x32\x32.admobilize.devicemanagement.v2.Device.LabelsEntry\x12\x0c\n\x04tags\x18\x0b \x03(\t\x12\x10\n\x08\x61rchived\x18\x0c \x01(\x08\x12\x31\n\x08solution\x18\r \x01(\x0e\x32\x1f.admobilize.common.SolutionName\x12\x38\n\x0cintegrations\x18\x0e \x03(\x0e\x32\".admobilize.common.IntegrationName\x12:\n\x05state\x18\x0f \x01(\x0b\x32+.admobilize.devicemanagement.v2.DeviceState\x12\x1a\n\x12\x65nable_auto_update\x18\x10 \x01(\x08\x12\x10\n\x08has_wifi\x18\x11 \x01(\x08\x12\x46\n\x0f\x64\x65vice_comments\x18\x12 \x03(\x0b\x32-.admobilize.devicemanagement.v2.DeviceComment\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"N\n\rDeviceComment\x12\x0c\n\x04text\x18\x01 \x01(\t\x12/\n\x0b\x63reate_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x8c\x01\n\x13\x44\x65viceWithPublicKey\x12\x36\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32&.admobilize.devicemanagement.v2.Device\x12=\n\npublic_key\x18\x02 \x01(\x0b\x32).admobilize.devicemanagement.v2.PublicKey\"\x88\x02\n\x07License\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x31\n\x08solution\x18\x03 \x01(\x0e\x32\x1f.admobilize.common.SolutionName\x12\x11\n\tdevice_id\x18\x04 \x01(\t\x12.\n\nvalid_from\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bvalid_until\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1a\n\x12\x61\x63\x63ount_admin_name\x18\x07 \x01(\t\x12\x12\n\nproject_id\x18\x08 \x01(\t\x12\x0c\n\x04\x64\x65mo\x18\t \x01(\x08\"\x89\x02\n\x13MoveDevicesMetadata\x12/\n\x0b\x63reate_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ndevice_ids\x18\x03 \x03(\t\x12\x1e\n\x16\x64\x65stination_project_id\x18\x04 \x01(\t\x12\x19\n\x11source_project_id\x18\x05 \x01(\t\x12$\n\x04jobs\x18\x06 \x03(\x0b\x32\x16.admobilize.common.Job\x12\x1e\n\x16requested_cancellation\x18\x07 \x01(\x08\"\xa5\x02\n\x1aRestoreDevicesDataMetadata\x12/\n\x0b\x63reate_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ndevice_ids\x18\x03 \x03(\t\x12\x1e\n\x16\x64\x65stination_project_id\x18\x04 \x01(\t\x12\x1c\n\x14\x64\x65stination_table_id\x18\x05 \x01(\t\x12\x10\n\x08truncate\x18\x06 \x01(\x08\x12$\n\x04jobs\x18\x07 \x03(\x0b\x32\x16.admobilize.common.Job\x12\x1e\n\x16requested_cancellation\x18\x08 \x01(\x08\"U\n\x11\x41WSIoTCredentials\x12\x17\n\x0f\x63\x65rtificate_pem\x18\x01 \x01(\t\x12\x12\n\npublic_key\x18\x02 \x01(\t\x12\x13\n\x0bprivate_key\x18\x03 \x01(\tB\xa0\x01\n\"com.admobilize.devicemanagement.v2B\x0b\x44\x65viceProtoP\x01ZBbitbucket.org/admobilize/admobilizeapis-go/pkg/devicemanagement/v2\xa2\x02\x05\x41\x44MDM\xaa\x02\x1e\x41\x64Mobilize.DeviceManagement.V2b\x06proto3')
 
 
 
 _LOGMESSAGE = DESCRIPTOR.message_types_by_name['LogMessage']
 _SOLUTION = DESCRIPTOR.message_types_by_name['Solution']
 _SOLUTIONCONFIGURATION = DESCRIPTOR.message_types_by_name['SolutionConfiguration']
 _PROJECTPREFERENCES = DESCRIPTOR.message_types_by_name['ProjectPreferences']
@@ -209,33 +209,33 @@
   _PROJECTPREFERENCES_SPEEDUNIT._serialized_start=1418
   _PROJECTPREFERENCES_SPEEDUNIT._serialized_end=1517
   _PROJECT._serialized_start=1520
   _PROJECT._serialized_end=2102
   _PROJECT_LABELSENTRY._serialized_start=2057
   _PROJECT_LABELSENTRY._serialized_end=2102
   _DEVICESTATE._serialized_start=2105
-  _DEVICESTATE._serialized_end=2506
-  _DEVICECONFIG._serialized_start=2509
-  _DEVICECONFIG._serialized_end=2720
-  _PUBLICKEY._serialized_start=2722
-  _PUBLICKEY._serialized_end=2762
-  _DEVICECREDENTIALS._serialized_start=2764
-  _DEVICECREDENTIALS._serialized_end=2861
-  _DEVICEIOTCORESTATUS._serialized_start=2864
-  _DEVICEIOTCORESTATUS._serialized_end=3218
-  _DEVICE._serialized_start=3221
-  _DEVICE._serialized_end=3914
+  _DEVICESTATE._serialized_end=2523
+  _DEVICECONFIG._serialized_start=2526
+  _DEVICECONFIG._serialized_end=2737
+  _PUBLICKEY._serialized_start=2739
+  _PUBLICKEY._serialized_end=2779
+  _DEVICECREDENTIALS._serialized_start=2781
+  _DEVICECREDENTIALS._serialized_end=2878
+  _DEVICEIOTCORESTATUS._serialized_start=2881
+  _DEVICEIOTCORESTATUS._serialized_end=3235
+  _DEVICE._serialized_start=3238
+  _DEVICE._serialized_end=3931
   _DEVICE_LABELSENTRY._serialized_start=2057
   _DEVICE_LABELSENTRY._serialized_end=2102
-  _DEVICECOMMENT._serialized_start=3916
-  _DEVICECOMMENT._serialized_end=3994
-  _DEVICEWITHPUBLICKEY._serialized_start=3997
-  _DEVICEWITHPUBLICKEY._serialized_end=4137
-  _LICENSE._serialized_start=4140
-  _LICENSE._serialized_end=4404
-  _MOVEDEVICESMETADATA._serialized_start=4407
-  _MOVEDEVICESMETADATA._serialized_end=4672
-  _RESTOREDEVICESDATAMETADATA._serialized_start=4675
-  _RESTOREDEVICESDATAMETADATA._serialized_end=4968
-  _AWSIOTCREDENTIALS._serialized_start=4970
-  _AWSIOTCREDENTIALS._serialized_end=5055
+  _DEVICECOMMENT._serialized_start=3933
+  _DEVICECOMMENT._serialized_end=4011
+  _DEVICEWITHPUBLICKEY._serialized_start=4014
+  _DEVICEWITHPUBLICKEY._serialized_end=4154
+  _LICENSE._serialized_start=4157
+  _LICENSE._serialized_end=4421
+  _MOVEDEVICESMETADATA._serialized_start=4424
+  _MOVEDEVICESMETADATA._serialized_end=4689
+  _RESTOREDEVICESDATAMETADATA._serialized_start=4692
+  _RESTOREDEVICESDATAMETADATA._serialized_end=4985
+  _AWSIOTCREDENTIALS._serialized_start=4987
+  _AWSIOTCREDENTIALS._serialized_end=5072
 # @@protoc_insertion_point(module_scope)
```

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/ayuda/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/malos/v1/driver_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/malos/v1/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/malos/v1/maloseye_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/malos/v1/maloseye_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/query/v1alpha1/query_service_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/query/v1alpha1/query_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/query/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/query/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/billing/v1alpha1/billing_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/billing/v1alpha1/billing_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/cmsintegrations/v1/resources_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/cmsintegrations/v1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/common/admobilize_types_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/common/admobilize_types_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/common/job_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/common/job_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/common/entity_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/common/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/vision/v1/vision_service_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/vision/v1/vision_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/vision/v1/model_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/vision/v1/model_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/vision/v1/vision_service_pb2_grpc.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/vision/v1/vision_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/vision/v1/vision_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/vision/v1/vision_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/wifi/v1/wifi_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/wifi/v1/wifi_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/iam/v1alpha1/iam_service_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/iam/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/iam/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/admprovider/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/broadsign/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/notification/v1beta1/notification_service_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/notification/v1beta1/notification_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/notification/v1beta1/resources_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/notification/v1beta1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py` & `admobilizeapis-2023.6.19.post1/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/google/longrunning/operations_pb2_grpc.py` & `admobilizeapis-2023.6.19.post1/admobilize/google/longrunning/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilize/google/longrunning/operations_pb2.py` & `admobilizeapis-2023.6.19.post1/admobilize/google/longrunning/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/PKG-INFO` & `admobilizeapis-2023.6.19.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admobilizeapis
-Version: 2023.2.7.post3
+Version: 2023.6.19.post1
 Summary: Protobufs used in AdMobilize Ecosystem
 Home-page: https://www.bitbucket.org/admobilize/admobilizeapis
 Author: AdMobilize Team
 Author-email: devel@admobilize.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `admobilizeapis-2023.2.7.post3/admobilizeapis.egg-info/SOURCES.txt` & `admobilizeapis-2023.6.19.post1/admobilizeapis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.2.7.post3/admobilizeapis.egg-info/PKG-INFO` & `admobilizeapis-2023.6.19.post1/admobilizeapis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admobilizeapis
-Version: 2023.2.7.post3
+Version: 2023.6.19.post1
 Summary: Protobufs used in AdMobilize Ecosystem
 Home-page: https://www.bitbucket.org/admobilize/admobilizeapis
 Author: AdMobilize Team
 Author-email: devel@admobilize.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

