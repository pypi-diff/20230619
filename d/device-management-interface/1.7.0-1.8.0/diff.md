# Comparing `tmp/device-management-interface-1.7.0.tar.gz` & `tmp/device-management-interface-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/device-management-interface-1.7.0.tar", last modified: Tue Aug 30 08:45:41 2022, max compression
+gzip compressed data, was "dist/device-management-interface-1.8.0.tar", last modified: Mon Sep 12 10:23:42 2022, max compression
```

## Comparing `device-management-interface-1.7.0.tar` & `device-management-interface-1.8.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-08-30 08:45:41.000000 device-management-interface-1.7.0/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      594 2022-08-30 08:45:41.000000 device-management-interface-1.7.0/PKG-INFO
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-08-30 08:45:41.000000 device-management-interface-1.7.0/docs/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4698 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/docs/DeviceImageManagement.md
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      707 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/docs/Examples.md
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-08-30 08:45:41.000000 device-management-interface-1.7.0/docs/images/
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)    37384 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/docs/images/managing_device.png
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    36981 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/docs/images/device_image_management_fsm.png
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     1771 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/docs/images/managing_device.drawio
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     2422 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/docs/images/events_metrics.drawio
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)    36053 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/docs/images/events_metrics.png
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2035 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/docs/images/device_image_management_fsm.drawio
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)    82408 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/docs/images/device_image_management.png
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     2655 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/docs/images/device_image_management.drawio
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2020 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/docs/RpcGuidelines.md
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6240 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/docs/ManagingDevice.md
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1839 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/docs/EventsMetrics.md
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1072 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/README.md
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1510 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/setup.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       38 2022-08-30 08:45:41.000000 device-management-interface-1.7.0/setup.cfg
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-08-30 08:45:41.000000 device-management-interface-1.7.0/protos/
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-08-30 08:45:41.000000 device-management-interface-1.7.0/protos/dmi/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2485 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/protos/dmi/sw_image.proto
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5913 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/protos/dmi/hw_events_mgmt_service.proto
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      378 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/protos/dmi/commons.proto
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    10220 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/protos/dmi/hw_management_service.proto
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4191 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/protos/dmi/sw_management_service.proto
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9807 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/protos/dmi/hw.proto
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4848 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/protos/dmi/hw_metrics_mgmt_service.proto
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       95 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/MANIFEST.in
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-08-30 08:45:41.000000 device-management-interface-1.7.0/python/
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-08-30 08:45:41.000000 device-management-interface-1.7.0/python/device_management_interface.egg-info/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      594 2022-08-30 08:45:41.000000 device-management-interface-1.7.0/python/device_management_interface.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        1 2022-08-30 08:45:41.000000 device-management-interface-1.7.0/python/device_management_interface.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1509 2022-08-30 08:45:41.000000 device-management-interface-1.7.0/python/device_management_interface.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       33 2022-08-30 08:45:41.000000 device-management-interface-1.7.0/python/device_management_interface.egg-info/requires.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        4 2022-08-30 08:45:41.000000 device-management-interface-1.7.0/python/device_management_interface.egg-info/top_level.txt
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-08-30 08:45:41.000000 device-management-interface-1.7.0/python/dmi/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      594 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/python/dmi/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    14658 2022-08-30 08:45:34.000000 device-management-interface-1.7.0/python/dmi/hw_events_mgmt_service_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2022-08-30 08:45:34.000000 device-management-interface-1.7.0/python/dmi/commons_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8217 2022-08-30 08:45:35.000000 device-management-interface-1.7.0/python/dmi/sw_management_service_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2022-08-30 08:45:34.000000 device-management-interface-1.7.0/python/dmi/hw_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8505 2022-08-30 08:45:35.000000 device-management-interface-1.7.0/python/dmi/hw_metrics_mgmt_service_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1668 2022-08-30 08:45:34.000000 device-management-interface-1.7.0/python/dmi/commons_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6477 2022-08-30 08:45:34.000000 device-management-interface-1.7.0/python/dmi/hw_events_mgmt_service_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2022-08-30 08:45:35.000000 device-management-interface-1.7.0/python/dmi/sw_image_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    25493 2022-08-30 08:45:35.000000 device-management-interface-1.7.0/python/dmi/hw_management_service_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11176 2022-08-30 08:45:35.000000 device-management-interface-1.7.0/python/dmi/hw_metrics_mgmt_service_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    23979 2022-08-30 08:45:34.000000 device-management-interface-1.7.0/python/dmi/hw_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3924 2022-08-30 08:45:35.000000 device-management-interface-1.7.0/python/dmi/sw_image_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    28478 2022-08-30 08:45:35.000000 device-management-interface-1.7.0/python/dmi/hw_management_service_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    12015 2022-08-30 08:45:35.000000 device-management-interface-1.7.0/python/dmi/sw_management_service_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        6 2022-08-30 08:45:15.000000 device-management-interface-1.7.0/VERSION
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-09-12 10:23:42.000000 device-management-interface-1.8.0/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      594 2022-09-12 10:23:42.000000 device-management-interface-1.8.0/PKG-INFO
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-09-12 10:23:42.000000 device-management-interface-1.8.0/docs/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4698 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/docs/DeviceImageManagement.md
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      707 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/docs/Examples.md
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-09-12 10:23:42.000000 device-management-interface-1.8.0/docs/images/
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)    37384 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/docs/images/managing_device.png
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    36981 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/docs/images/device_image_management_fsm.png
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     1771 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/docs/images/managing_device.drawio
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     2422 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/docs/images/events_metrics.drawio
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)    36053 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/docs/images/events_metrics.png
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2035 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/docs/images/device_image_management_fsm.drawio
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)    82408 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/docs/images/device_image_management.png
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     2655 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/docs/images/device_image_management.drawio
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2020 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/docs/RpcGuidelines.md
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6240 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/docs/ManagingDevice.md
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1839 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/docs/EventsMetrics.md
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1072 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/README.md
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1510 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/setup.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       38 2022-09-12 10:23:42.000000 device-management-interface-1.8.0/setup.cfg
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-09-12 10:23:42.000000 device-management-interface-1.8.0/protos/
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-09-12 10:23:42.000000 device-management-interface-1.8.0/protos/dmi/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2485 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/protos/dmi/sw_image.proto
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6550 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/protos/dmi/hw_events_mgmt_service.proto
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      378 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/protos/dmi/commons.proto
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    10220 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/protos/dmi/hw_management_service.proto
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4191 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/protos/dmi/sw_management_service.proto
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9833 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/protos/dmi/hw.proto
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4848 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/protos/dmi/hw_metrics_mgmt_service.proto
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       95 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/MANIFEST.in
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-09-12 10:23:42.000000 device-management-interface-1.8.0/python/
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-09-12 10:23:42.000000 device-management-interface-1.8.0/python/device_management_interface.egg-info/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      594 2022-09-12 10:23:42.000000 device-management-interface-1.8.0/python/device_management_interface.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        1 2022-09-12 10:23:42.000000 device-management-interface-1.8.0/python/device_management_interface.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1509 2022-09-12 10:23:42.000000 device-management-interface-1.8.0/python/device_management_interface.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       33 2022-09-12 10:23:42.000000 device-management-interface-1.8.0/python/device_management_interface.egg-info/requires.txt
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        4 2022-09-12 10:23:42.000000 device-management-interface-1.8.0/python/device_management_interface.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-09-12 10:23:42.000000 device-management-interface-1.8.0/python/dmi/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      594 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/python/dmi/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    14717 2022-09-12 10:23:35.000000 device-management-interface-1.8.0/python/dmi/hw_events_mgmt_service_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2022-09-12 10:23:34.000000 device-management-interface-1.8.0/python/dmi/commons_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8217 2022-09-12 10:23:35.000000 device-management-interface-1.8.0/python/dmi/sw_management_service_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2022-09-12 10:23:35.000000 device-management-interface-1.8.0/python/dmi/hw_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8505 2022-09-12 10:23:35.000000 device-management-interface-1.8.0/python/dmi/hw_metrics_mgmt_service_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1668 2022-09-12 10:23:34.000000 device-management-interface-1.8.0/python/dmi/commons_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6477 2022-09-12 10:23:35.000000 device-management-interface-1.8.0/python/dmi/hw_events_mgmt_service_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2022-09-12 10:23:35.000000 device-management-interface-1.8.0/python/dmi/sw_image_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    25493 2022-09-12 10:23:35.000000 device-management-interface-1.8.0/python/dmi/hw_management_service_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11176 2022-09-12 10:23:35.000000 device-management-interface-1.8.0/python/dmi/hw_metrics_mgmt_service_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    24035 2022-09-12 10:23:35.000000 device-management-interface-1.8.0/python/dmi/hw_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3924 2022-09-12 10:23:35.000000 device-management-interface-1.8.0/python/dmi/sw_image_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    28478 2022-09-12 10:23:35.000000 device-management-interface-1.8.0/python/dmi/hw_management_service_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    12015 2022-09-12 10:23:35.000000 device-management-interface-1.8.0/python/dmi/sw_management_service_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        6 2022-09-12 10:23:16.000000 device-management-interface-1.8.0/VERSION
```

### Comparing `device-management-interface-1.7.0/PKG-INFO` & `device-management-interface-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: device-management-interface
-Version: 1.7.0
+Version: 1.8.0
 Summary: Protobuf interface definitions
 Home-page: https://gerrit.opencord.org/plugins/gitiles/device-management-interface
 Author: VOLTHA project
 Author-email: voltha-dev@opencord.org
 License: Apache Software License
 Description: UNKNOWN
 Keywords: protobuf device-management-interface voltha
```

### Comparing `device-management-interface-1.7.0/docs/DeviceImageManagement.md` & `device-management-interface-1.8.0/docs/DeviceImageManagement.md`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/docs/Examples.md` & `device-management-interface-1.8.0/docs/Examples.md`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/docs/images/managing_device.png` & `device-management-interface-1.8.0/docs/images/managing_device.png`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/docs/images/device_image_management_fsm.png` & `device-management-interface-1.8.0/docs/images/device_image_management_fsm.png`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/docs/images/managing_device.drawio` & `device-management-interface-1.8.0/docs/images/managing_device.drawio`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/docs/images/events_metrics.drawio` & `device-management-interface-1.8.0/docs/images/events_metrics.drawio`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/docs/images/events_metrics.png` & `device-management-interface-1.8.0/docs/images/events_metrics.png`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/docs/images/device_image_management_fsm.drawio` & `device-management-interface-1.8.0/docs/images/device_image_management_fsm.drawio`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/docs/images/device_image_management.png` & `device-management-interface-1.8.0/docs/images/device_image_management.png`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/docs/images/device_image_management.drawio` & `device-management-interface-1.8.0/docs/images/device_image_management.drawio`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/docs/RpcGuidelines.md` & `device-management-interface-1.8.0/docs/RpcGuidelines.md`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/docs/ManagingDevice.md` & `device-management-interface-1.8.0/docs/ManagingDevice.md`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/docs/EventsMetrics.md` & `device-management-interface-1.8.0/docs/EventsMetrics.md`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/README.md` & `device-management-interface-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/setup.py` & `device-management-interface-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/protos/dmi/sw_image.proto` & `device-management-interface-1.8.0/protos/dmi/sw_image.proto`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/protos/dmi/hw_events_mgmt_service.proto` & `device-management-interface-1.8.0/protos/dmi/hw_events_mgmt_service.proto`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 
 enum EventIds {
     EVENT_NAME_UNDEFINED = 0;
 
     // Events from the Transceivers
     EVENT_TRANSCEIVER_PLUG_OUT = 100;
     EVENT_TRANSCEIVER_PLUG_IN = 101;
+    // The threshold based events on the transceivers should be configured on
+    // the port components of that transceiver and not on the transceiver
+    // component itself. This is because there could be different thresholds
+    // on the different ports of a transceiver (for example for a transceiver of
+    // type COMBO_GPON_XGSPON the power thresholds could be different for the
+    // GPON and XGSPON ports)
     EVENT_TRANSCEIVER_VOLTAGE_ABOVE_THRESHOLD = 102;
     EVENT_TRANSCEIVER_VOLTAGE_BELOW_THRESHOLD = 103;
     EVENT_TRANSCEIVER_TEMPERATURE_ABOVE_THRESHOLD = 104;
     EVENT_TRANSCEIVER_TEMPERATURE_BELOW_THRESHOLD = 105;
     EVENT_TRANSCEIVER_CURRENT_ABOVE_THRESHOLD = 106;
     EVENT_TRANSCEIVER_CURRENT_BELOW_THRESHOLD = 107;
     EVENT_TRANSCEIVER_RX_POWER_ABOVE_THRESHOLD = 108;
@@ -71,19 +77,24 @@
     EVENT_LINE_CARD_PLUG_OUT = 600;
     EVENT_LINE_CARD_PLUG_IN = 601;
 
     // More to be added
 }
 
 message ValueType {
+    // For val no multiples of units shall be used.
+    // For example, for memory val should be in bytes and not in kilobytes or any
+    // other multiple of the unit byte.
     oneof val{
         int64 int_val = 1;
         uint64 uint_val = 2;
         float float_val = 3;
     }
+
+    DataValueType typeOfVal = 4;
 }
 
 message WaterMarks {
     ValueType high = 1;
     ValueType low = 2;
 }
```

### Comparing `device-management-interface-1.7.0/protos/dmi/hw_management_service.proto` & `device-management-interface-1.8.0/protos/dmi/hw_management_service.proto`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/protos/dmi/sw_management_service.proto` & `device-management-interface-1.8.0/protos/dmi/sw_management_service.proto`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/protos/dmi/hw.proto` & `device-management-interface-1.8.0/protos/dmi/hw.proto`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,15 @@
     VALUE_TYPE_PERCENT_RH = 9;
     VALUE_TYPE_RPM = 10;
     VALUE_TYPE_CMM = 11;
     VALUE_TYPE_TRUTH_VALUE = 12;
     VALUE_TYPE_PERCENT = 13;
     VALUE_TYPE_METERS = 14;
     VALUE_TYPE_BYTES = 15;
+    VALUE_TYPE_DBM = 16;
 }
 
 enum ValueScale {
     VALUE_SCALE_UNDEFINED = 0;
     VALUE_SCALE_YOCTO = 1;
     VALUE_SCALE_ZEPTO = 2;
     VALUE_SCALE_ATTO = 3;
```

### Comparing `device-management-interface-1.7.0/protos/dmi/hw_metrics_mgmt_service.proto` & `device-management-interface-1.8.0/protos/dmi/hw_metrics_mgmt_service.proto`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/python/device_management_interface.egg-info/PKG-INFO` & `device-management-interface-1.8.0/python/device_management_interface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: device-management-interface
-Version: 1.7.0
+Version: 1.8.0
 Summary: Protobuf interface definitions
 Home-page: https://gerrit.opencord.org/plugins/gitiles/device-management-interface
 Author: VOLTHA project
 Author-email: voltha-dev@opencord.org
 License: Apache Software License
 Description: UNKNOWN
 Keywords: protobuf device-management-interface voltha
```

### Comparing `device-management-interface-1.7.0/python/device_management_interface.egg-info/SOURCES.txt` & `device-management-interface-1.8.0/python/device_management_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/python/dmi/__init__.py` & `device-management-interface-1.8.0/python/dmi/__init__.py`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/python/dmi/hw_events_mgmt_service_pb2.py` & `device-management-interface-1.8.0/python/dmi/hw_events_mgmt_service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from dmi import commons_pb2 as dmi_dot_commons__pb2
 from dmi import hw_pb2 as dmi_dot_hw__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n dmi/hw_events_mgmt_service.proto\x12\x03\x64mi\x1a\x11\x64mi/commons.proto\x1a\x0c\x64mi/hw.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/protobuf/empty.proto\"N\n\tValueType\x12\x11\n\x07int_val\x18\x01 \x01(\x03H\x00\x12\x12\n\x08uint_val\x18\x02 \x01(\x04H\x00\x12\x13\n\tfloat_val\x18\x03 \x01(\x02H\x00\x42\x05\n\x03val\"G\n\nWaterMarks\x12\x1c\n\x04high\x18\x01 \x01(\x0b\x32\x0e.dmi.ValueType\x12\x1b\n\x03low\x18\x02 \x01(\x0b\x32\x0e.dmi.ValueType\"]\n\nThresholds\x12 \n\x05upper\x18\x01 \x01(\x0b\x32\x0f.dmi.WaterMarksH\x00\x12 \n\x05lower\x18\x02 \x01(\x0b\x32\x0f.dmi.WaterMarksH\x00\x42\x0b\n\tthreshold\"c\n\x14ThresholdInformation\x12&\n\x0eobserved_value\x18\x01 \x01(\x0b\x32\x0e.dmi.ValueType\x12#\n\nthresholds\x18\x02 \x01(\x0b\x32\x0f.dmi.Thresholds\"g\n\x08\x45ventCfg\x12\x1f\n\x08\x65vent_id\x18\x01 \x01(\x0e\x32\r.dmi.EventIds\x12\x15\n\ris_configured\x18\x02 \x01(\x08\x12#\n\nthresholds\x18\x03 \x01(\x0b\x32\x0f.dmi.Thresholds\")\n\tEventsCfg\x12\x1c\n\x05items\x18\x01 \x03(\x0b\x32\r.dmi.EventCfg\"\xf8\x01\n\x12ListEventsResponse\x12\x1b\n\x06status\x18\x01 \x01(\x0e\x32\x0b.dmi.Status\x12.\n\x06reason\x18\x02 \x01(\x0e\x32\x1e.dmi.ListEventsResponse.Reason\x12\x1e\n\x06\x65vents\x18\x03 \x01(\x0b\x32\x0e.dmi.EventsCfg\x12\x15\n\rreason_detail\x18\x04 \x01(\t\"^\n\x06Reason\x12\x14\n\x10UNDEFINED_REASON\x10\x00\x12\x12\n\x0eUNKNOWN_DEVICE\x10\x01\x12\x12\n\x0eINTERNAL_ERROR\x10\x02\x12\x16\n\x12\x44\x45VICE_UNREACHABLE\x10\x03\"\xab\x01\n\x1a\x45ventsConfigurationRequest\x12\x1e\n\x0b\x64\x65vice_uuid\x18\x01 \x01(\x0b\x32\t.dmi.Uuid\x12!\n\x07\x63hanges\x18\x02 \x01(\x0b\x32\x0e.dmi.EventsCfgH\x00\x12\x1a\n\x10reset_to_default\x18\x03 \x01(\x08H\x00\x12!\n\x0e\x63omponent_uuid\x18\x04 \x01(\x0b\x32\t.dmi.UuidB\x0b\n\toperation\"\xfe\x01\n\x1b\x45ventsConfigurationResponse\x12\x1b\n\x06status\x18\x01 \x01(\x0e\x32\x0b.dmi.Status\x12\x37\n\x06reason\x18\x02 \x01(\x0e\x32\'.dmi.EventsConfigurationResponse.Reason\x12\x15\n\rreason_detail\x18\x03 \x01(\t\"r\n\x06Reason\x12\x14\n\x10UNDEFINED_REASON\x10\x00\x12\x12\n\x0eUNKNOWN_DEVICE\x10\x01\x12\x12\n\x0eINTERNAL_ERROR\x10\x02\x12\x12\n\x0eINVALID_CONFIG\x10\x03\x12\x16\n\x12\x44\x45VICE_UNREACHABLE\x10\x04\"j\n\rEventMetaData\x12\x1e\n\x0b\x64\x65vice_uuid\x18\x01 \x01(\x0b\x32\t.dmi.Uuid\x12!\n\x0e\x63omponent_uuid\x18\x02 \x01(\x0b\x32\t.dmi.Uuid\x12\x16\n\x0e\x63omponent_name\x18\x03 \x01(\t\"\xc8\x01\n\x05\x45vent\x12*\n\x0e\x65vent_metadata\x18\x01 \x01(\x0b\x32\x12.dmi.EventMetaData\x12\x1f\n\x08\x65vent_id\x18\x02 \x01(\x0e\x32\r.dmi.EventIds\x12-\n\traised_ts\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\x0ethreshold_info\x18\x04 \x01(\x0b\x32\x19.dmi.ThresholdInformation\x12\x10\n\x08\x61\x64\x64_info\x18\x05 \x01(\t*\x82\x10\n\x08\x45ventIds\x12\x18\n\x14\x45VENT_NAME_UNDEFINED\x10\x00\x12\x1e\n\x1a\x45VENT_TRANSCEIVER_PLUG_OUT\x10\x64\x12\x1d\n\x19\x45VENT_TRANSCEIVER_PLUG_IN\x10\x65\x12-\n)EVENT_TRANSCEIVER_VOLTAGE_ABOVE_THRESHOLD\x10\x66\x12-\n)EVENT_TRANSCEIVER_VOLTAGE_BELOW_THRESHOLD\x10g\x12\x31\n-EVENT_TRANSCEIVER_TEMPERATURE_ABOVE_THRESHOLD\x10h\x12\x31\n-EVENT_TRANSCEIVER_TEMPERATURE_BELOW_THRESHOLD\x10i\x12-\n)EVENT_TRANSCEIVER_CURRENT_ABOVE_THRESHOLD\x10j\x12-\n)EVENT_TRANSCEIVER_CURRENT_BELOW_THRESHOLD\x10k\x12.\n*EVENT_TRANSCEIVER_RX_POWER_ABOVE_THRESHOLD\x10l\x12.\n*EVENT_TRANSCEIVER_RX_POWER_BELOW_THRESHOLD\x10m\x12.\n*EVENT_TRANSCEIVER_TX_POWER_ABOVE_THRESHOLD\x10n\x12.\n*EVENT_TRANSCEIVER_TX_POWER_BELOW_THRESHOLD\x10o\x12\x1d\n\x19\x45VENT_TRANSCEIVER_FAILURE\x10p\x12\x37\n3EVENT_TRANSCEIVER_VOLTAGE_ABOVE_THRESHOLD_RECOVERED\x10q\x12\x37\n3EVENT_TRANSCEIVER_VOLTAGE_BELOW_THRESHOLD_RECOVERED\x10r\x12;\n7EVENT_TRANSCEIVER_TEMPERATURE_ABOVE_THRESHOLD_RECOVERED\x10s\x12;\n7EVENT_TRANSCEIVER_TEMPERATURE_BELOW_THRESHOLD_RECOVERED\x10t\x12\x37\n3EVENT_TRANSCEIVER_CURRENT_ABOVE_THRESHOLD_RECOVERED\x10u\x12\x37\n3EVENT_TRANSCEIVER_CURRENT_BELOW_THRESHOLD_RECOVERED\x10v\x12\x38\n4EVENT_TRANSCEIVER_RX_POWER_ABOVE_THRESHOLD_RECOVERED\x10w\x12\x38\n4EVENT_TRANSCEIVER_RX_POWER_BELOW_THRESHOLD_RECOVERED\x10x\x12\x38\n4EVENT_TRANSCEIVER_TX_POWER_ABOVE_THRESHOLD_RECOVERED\x10y\x12\x38\n4EVENT_TRANSCEIVER_TX_POWER_BELOW_THRESHOLD_RECOVERED\x10z\x12\'\n#EVENT_TRANSCEIVER_FAILURE_RECOVERED\x10{\x12\x17\n\x12\x45VENT_PSU_PLUG_OUT\x10\xc8\x01\x12\x16\n\x11\x45VENT_PSU_PLUG_IN\x10\xc9\x01\x12\x16\n\x11\x45VENT_PSU_FAILURE\x10\xca\x01\x12 \n\x1b\x45VENT_PSU_FAILURE_RECOVERED\x10\xcb\x01\x12\x16\n\x11\x45VENT_FAN_FAILURE\x10\xac\x02\x12\x17\n\x12\x45VENT_FAN_PLUG_OUT\x10\xad\x02\x12\x16\n\x11\x45VENT_FAN_PLUG_IN\x10\xae\x02\x12 \n\x1b\x45VENT_FAN_FAILURE_RECOVERED\x10\xaf\x02\x12)\n$EVENT_CPU_TEMPERATURE_ABOVE_CRITICAL\x10\x90\x03\x12&\n!EVENT_CPU_TEMPERATURE_ABOVE_FATAL\x10\x91\x03\x12\x33\n.EVENT_CPU_TEMPERATURE_ABOVE_CRITICAL_RECOVERED\x10\x92\x03\x12\x30\n+EVENT_CPU_TEMPERATURE_ABOVE_FATAL_RECOVERED\x10\x93\x03\x12\x1a\n\x15\x45VENT_HW_DEVICE_RESET\x10\xf4\x03\x12/\n*EVENT_HW_DEVICE_TEMPERATURE_ABOVE_CRITICAL\x10\xf5\x03\x12,\n\'EVENT_HW_DEVICE_TEMPERATURE_ABOVE_FATAL\x10\xf6\x03\x12\x39\n4EVENT_HW_DEVICE_TEMPERATURE_ABOVE_CRITICAL_RECOVERED\x10\xf7\x03\x12\x36\n1EVENT_HW_DEVICE_TEMPERATURE_ABOVE_FATAL_RECOVERED\x10\xf8\x03\x12\x1b\n\x16\x45VENT_HW_DEVICE_REBOOT\x10\xf9\x03\x12\'\n\"EVENT_HW_TEMPERATURE_SENSOR_FAILED\x10\xfa\x03\x12,\n\'EVENT_HW_ALL_TEMPERATURE_SENSORS_FAILED\x10\xfb\x03\x12\x1d\n\x18\x45VENT_LINE_CARD_PLUG_OUT\x10\xd8\x04\x12\x1c\n\x17\x45VENT_LINE_CARD_PLUG_IN\x10\xd9\x04\x32\xed\x01\n\x1dNativeEventsManagementService\x12\x36\n\nListEvents\x12\x0f.dmi.HardwareID\x1a\x17.dmi.ListEventsResponse\x12^\n\x19UpdateEventsConfiguration\x12\x1f.dmi.EventsConfigurationRequest\x1a .dmi.EventsConfigurationResponse\x12\x34\n\x0cStreamEvents\x12\x16.google.protobuf.Empty\x1a\n.dmi.Event0\x01\x42;Z9github.com/opencord/device-management-interface/v3/go/dmib\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n dmi/hw_events_mgmt_service.proto\x12\x03\x64mi\x1a\x11\x64mi/commons.proto\x1a\x0c\x64mi/hw.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/protobuf/empty.proto\"u\n\tValueType\x12\x11\n\x07int_val\x18\x01 \x01(\x03H\x00\x12\x12\n\x08uint_val\x18\x02 \x01(\x04H\x00\x12\x13\n\tfloat_val\x18\x03 \x01(\x02H\x00\x12%\n\ttypeOfVal\x18\x04 \x01(\x0e\x32\x12.dmi.DataValueTypeB\x05\n\x03val\"G\n\nWaterMarks\x12\x1c\n\x04high\x18\x01 \x01(\x0b\x32\x0e.dmi.ValueType\x12\x1b\n\x03low\x18\x02 \x01(\x0b\x32\x0e.dmi.ValueType\"]\n\nThresholds\x12 \n\x05upper\x18\x01 \x01(\x0b\x32\x0f.dmi.WaterMarksH\x00\x12 \n\x05lower\x18\x02 \x01(\x0b\x32\x0f.dmi.WaterMarksH\x00\x42\x0b\n\tthreshold\"c\n\x14ThresholdInformation\x12&\n\x0eobserved_value\x18\x01 \x01(\x0b\x32\x0e.dmi.ValueType\x12#\n\nthresholds\x18\x02 \x01(\x0b\x32\x0f.dmi.Thresholds\"g\n\x08\x45ventCfg\x12\x1f\n\x08\x65vent_id\x18\x01 \x01(\x0e\x32\r.dmi.EventIds\x12\x15\n\ris_configured\x18\x02 \x01(\x08\x12#\n\nthresholds\x18\x03 \x01(\x0b\x32\x0f.dmi.Thresholds\")\n\tEventsCfg\x12\x1c\n\x05items\x18\x01 \x03(\x0b\x32\r.dmi.EventCfg\"\xf8\x01\n\x12ListEventsResponse\x12\x1b\n\x06status\x18\x01 \x01(\x0e\x32\x0b.dmi.Status\x12.\n\x06reason\x18\x02 \x01(\x0e\x32\x1e.dmi.ListEventsResponse.Reason\x12\x1e\n\x06\x65vents\x18\x03 \x01(\x0b\x32\x0e.dmi.EventsCfg\x12\x15\n\rreason_detail\x18\x04 \x01(\t\"^\n\x06Reason\x12\x14\n\x10UNDEFINED_REASON\x10\x00\x12\x12\n\x0eUNKNOWN_DEVICE\x10\x01\x12\x12\n\x0eINTERNAL_ERROR\x10\x02\x12\x16\n\x12\x44\x45VICE_UNREACHABLE\x10\x03\"\xab\x01\n\x1a\x45ventsConfigurationRequest\x12\x1e\n\x0b\x64\x65vice_uuid\x18\x01 \x01(\x0b\x32\t.dmi.Uuid\x12!\n\x07\x63hanges\x18\x02 \x01(\x0b\x32\x0e.dmi.EventsCfgH\x00\x12\x1a\n\x10reset_to_default\x18\x03 \x01(\x08H\x00\x12!\n\x0e\x63omponent_uuid\x18\x04 \x01(\x0b\x32\t.dmi.UuidB\x0b\n\toperation\"\xfe\x01\n\x1b\x45ventsConfigurationResponse\x12\x1b\n\x06status\x18\x01 \x01(\x0e\x32\x0b.dmi.Status\x12\x37\n\x06reason\x18\x02 \x01(\x0e\x32\'.dmi.EventsConfigurationResponse.Reason\x12\x15\n\rreason_detail\x18\x03 \x01(\t\"r\n\x06Reason\x12\x14\n\x10UNDEFINED_REASON\x10\x00\x12\x12\n\x0eUNKNOWN_DEVICE\x10\x01\x12\x12\n\x0eINTERNAL_ERROR\x10\x02\x12\x12\n\x0eINVALID_CONFIG\x10\x03\x12\x16\n\x12\x44\x45VICE_UNREACHABLE\x10\x04\"j\n\rEventMetaData\x12\x1e\n\x0b\x64\x65vice_uuid\x18\x01 \x01(\x0b\x32\t.dmi.Uuid\x12!\n\x0e\x63omponent_uuid\x18\x02 \x01(\x0b\x32\t.dmi.Uuid\x12\x16\n\x0e\x63omponent_name\x18\x03 \x01(\t\"\xc8\x01\n\x05\x45vent\x12*\n\x0e\x65vent_metadata\x18\x01 \x01(\x0b\x32\x12.dmi.EventMetaData\x12\x1f\n\x08\x65vent_id\x18\x02 \x01(\x0e\x32\r.dmi.EventIds\x12-\n\traised_ts\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\x0ethreshold_info\x18\x04 \x01(\x0b\x32\x19.dmi.ThresholdInformation\x12\x10\n\x08\x61\x64\x64_info\x18\x05 \x01(\t*\x82\x10\n\x08\x45ventIds\x12\x18\n\x14\x45VENT_NAME_UNDEFINED\x10\x00\x12\x1e\n\x1a\x45VENT_TRANSCEIVER_PLUG_OUT\x10\x64\x12\x1d\n\x19\x45VENT_TRANSCEIVER_PLUG_IN\x10\x65\x12-\n)EVENT_TRANSCEIVER_VOLTAGE_ABOVE_THRESHOLD\x10\x66\x12-\n)EVENT_TRANSCEIVER_VOLTAGE_BELOW_THRESHOLD\x10g\x12\x31\n-EVENT_TRANSCEIVER_TEMPERATURE_ABOVE_THRESHOLD\x10h\x12\x31\n-EVENT_TRANSCEIVER_TEMPERATURE_BELOW_THRESHOLD\x10i\x12-\n)EVENT_TRANSCEIVER_CURRENT_ABOVE_THRESHOLD\x10j\x12-\n)EVENT_TRANSCEIVER_CURRENT_BELOW_THRESHOLD\x10k\x12.\n*EVENT_TRANSCEIVER_RX_POWER_ABOVE_THRESHOLD\x10l\x12.\n*EVENT_TRANSCEIVER_RX_POWER_BELOW_THRESHOLD\x10m\x12.\n*EVENT_TRANSCEIVER_TX_POWER_ABOVE_THRESHOLD\x10n\x12.\n*EVENT_TRANSCEIVER_TX_POWER_BELOW_THRESHOLD\x10o\x12\x1d\n\x19\x45VENT_TRANSCEIVER_FAILURE\x10p\x12\x37\n3EVENT_TRANSCEIVER_VOLTAGE_ABOVE_THRESHOLD_RECOVERED\x10q\x12\x37\n3EVENT_TRANSCEIVER_VOLTAGE_BELOW_THRESHOLD_RECOVERED\x10r\x12;\n7EVENT_TRANSCEIVER_TEMPERATURE_ABOVE_THRESHOLD_RECOVERED\x10s\x12;\n7EVENT_TRANSCEIVER_TEMPERATURE_BELOW_THRESHOLD_RECOVERED\x10t\x12\x37\n3EVENT_TRANSCEIVER_CURRENT_ABOVE_THRESHOLD_RECOVERED\x10u\x12\x37\n3EVENT_TRANSCEIVER_CURRENT_BELOW_THRESHOLD_RECOVERED\x10v\x12\x38\n4EVENT_TRANSCEIVER_RX_POWER_ABOVE_THRESHOLD_RECOVERED\x10w\x12\x38\n4EVENT_TRANSCEIVER_RX_POWER_BELOW_THRESHOLD_RECOVERED\x10x\x12\x38\n4EVENT_TRANSCEIVER_TX_POWER_ABOVE_THRESHOLD_RECOVERED\x10y\x12\x38\n4EVENT_TRANSCEIVER_TX_POWER_BELOW_THRESHOLD_RECOVERED\x10z\x12\'\n#EVENT_TRANSCEIVER_FAILURE_RECOVERED\x10{\x12\x17\n\x12\x45VENT_PSU_PLUG_OUT\x10\xc8\x01\x12\x16\n\x11\x45VENT_PSU_PLUG_IN\x10\xc9\x01\x12\x16\n\x11\x45VENT_PSU_FAILURE\x10\xca\x01\x12 \n\x1b\x45VENT_PSU_FAILURE_RECOVERED\x10\xcb\x01\x12\x16\n\x11\x45VENT_FAN_FAILURE\x10\xac\x02\x12\x17\n\x12\x45VENT_FAN_PLUG_OUT\x10\xad\x02\x12\x16\n\x11\x45VENT_FAN_PLUG_IN\x10\xae\x02\x12 \n\x1b\x45VENT_FAN_FAILURE_RECOVERED\x10\xaf\x02\x12)\n$EVENT_CPU_TEMPERATURE_ABOVE_CRITICAL\x10\x90\x03\x12&\n!EVENT_CPU_TEMPERATURE_ABOVE_FATAL\x10\x91\x03\x12\x33\n.EVENT_CPU_TEMPERATURE_ABOVE_CRITICAL_RECOVERED\x10\x92\x03\x12\x30\n+EVENT_CPU_TEMPERATURE_ABOVE_FATAL_RECOVERED\x10\x93\x03\x12\x1a\n\x15\x45VENT_HW_DEVICE_RESET\x10\xf4\x03\x12/\n*EVENT_HW_DEVICE_TEMPERATURE_ABOVE_CRITICAL\x10\xf5\x03\x12,\n\'EVENT_HW_DEVICE_TEMPERATURE_ABOVE_FATAL\x10\xf6\x03\x12\x39\n4EVENT_HW_DEVICE_TEMPERATURE_ABOVE_CRITICAL_RECOVERED\x10\xf7\x03\x12\x36\n1EVENT_HW_DEVICE_TEMPERATURE_ABOVE_FATAL_RECOVERED\x10\xf8\x03\x12\x1b\n\x16\x45VENT_HW_DEVICE_REBOOT\x10\xf9\x03\x12\'\n\"EVENT_HW_TEMPERATURE_SENSOR_FAILED\x10\xfa\x03\x12,\n\'EVENT_HW_ALL_TEMPERATURE_SENSORS_FAILED\x10\xfb\x03\x12\x1d\n\x18\x45VENT_LINE_CARD_PLUG_OUT\x10\xd8\x04\x12\x1c\n\x17\x45VENT_LINE_CARD_PLUG_IN\x10\xd9\x04\x32\xed\x01\n\x1dNativeEventsManagementService\x12\x36\n\nListEvents\x12\x0f.dmi.HardwareID\x1a\x17.dmi.ListEventsResponse\x12^\n\x19UpdateEventsConfiguration\x12\x1f.dmi.EventsConfigurationRequest\x1a .dmi.EventsConfigurationResponse\x12\x34\n\x0cStreamEvents\x12\x16.google.protobuf.Empty\x1a\n.dmi.Event0\x01\x42;Z9github.com/opencord/device-management-interface/v3/go/dmib\x06proto3')
 
 _EVENTIDS = DESCRIPTOR.enum_types_by_name['EventIds']
 EventIds = enum_type_wrapper.EnumTypeWrapper(_EVENTIDS)
 EVENT_NAME_UNDEFINED = 0
 EVENT_TRANSCEIVER_PLUG_OUT = 100
 EVENT_TRANSCEIVER_PLUG_IN = 101
 EVENT_TRANSCEIVER_VOLTAGE_ABOVE_THRESHOLD = 102
@@ -163,38 +163,38 @@
 _sym_db.RegisterMessage(Event)
 
 _NATIVEEVENTSMANAGEMENTSERVICE = DESCRIPTOR.services_by_name['NativeEventsManagementService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z9github.com/opencord/device-management-interface/v3/go/dmi'
-  _EVENTIDS._serialized_start=1627
-  _EVENTIDS._serialized_end=3677
+  _EVENTIDS._serialized_start=1666
+  _EVENTIDS._serialized_end=3716
   _VALUETYPE._serialized_start=136
-  _VALUETYPE._serialized_end=214
-  _WATERMARKS._serialized_start=216
-  _WATERMARKS._serialized_end=287
-  _THRESHOLDS._serialized_start=289
-  _THRESHOLDS._serialized_end=382
-  _THRESHOLDINFORMATION._serialized_start=384
-  _THRESHOLDINFORMATION._serialized_end=483
-  _EVENTCFG._serialized_start=485
-  _EVENTCFG._serialized_end=588
-  _EVENTSCFG._serialized_start=590
-  _EVENTSCFG._serialized_end=631
-  _LISTEVENTSRESPONSE._serialized_start=634
-  _LISTEVENTSRESPONSE._serialized_end=882
-  _LISTEVENTSRESPONSE_REASON._serialized_start=788
-  _LISTEVENTSRESPONSE_REASON._serialized_end=882
-  _EVENTSCONFIGURATIONREQUEST._serialized_start=885
-  _EVENTSCONFIGURATIONREQUEST._serialized_end=1056
-  _EVENTSCONFIGURATIONRESPONSE._serialized_start=1059
-  _EVENTSCONFIGURATIONRESPONSE._serialized_end=1313
-  _EVENTSCONFIGURATIONRESPONSE_REASON._serialized_start=1199
-  _EVENTSCONFIGURATIONRESPONSE_REASON._serialized_end=1313
-  _EVENTMETADATA._serialized_start=1315
-  _EVENTMETADATA._serialized_end=1421
-  _EVENT._serialized_start=1424
-  _EVENT._serialized_end=1624
-  _NATIVEEVENTSMANAGEMENTSERVICE._serialized_start=3680
-  _NATIVEEVENTSMANAGEMENTSERVICE._serialized_end=3917
+  _VALUETYPE._serialized_end=253
+  _WATERMARKS._serialized_start=255
+  _WATERMARKS._serialized_end=326
+  _THRESHOLDS._serialized_start=328
+  _THRESHOLDS._serialized_end=421
+  _THRESHOLDINFORMATION._serialized_start=423
+  _THRESHOLDINFORMATION._serialized_end=522
+  _EVENTCFG._serialized_start=524
+  _EVENTCFG._serialized_end=627
+  _EVENTSCFG._serialized_start=629
+  _EVENTSCFG._serialized_end=670
+  _LISTEVENTSRESPONSE._serialized_start=673
+  _LISTEVENTSRESPONSE._serialized_end=921
+  _LISTEVENTSRESPONSE_REASON._serialized_start=827
+  _LISTEVENTSRESPONSE_REASON._serialized_end=921
+  _EVENTSCONFIGURATIONREQUEST._serialized_start=924
+  _EVENTSCONFIGURATIONREQUEST._serialized_end=1095
+  _EVENTSCONFIGURATIONRESPONSE._serialized_start=1098
+  _EVENTSCONFIGURATIONRESPONSE._serialized_end=1352
+  _EVENTSCONFIGURATIONRESPONSE_REASON._serialized_start=1238
+  _EVENTSCONFIGURATIONRESPONSE_REASON._serialized_end=1352
+  _EVENTMETADATA._serialized_start=1354
+  _EVENTMETADATA._serialized_end=1460
+  _EVENT._serialized_start=1463
+  _EVENT._serialized_end=1663
+  _NATIVEEVENTSMANAGEMENTSERVICE._serialized_start=3719
+  _NATIVEEVENTSMANAGEMENTSERVICE._serialized_end=3956
 # @@protoc_insertion_point(module_scope)
```

### Comparing `device-management-interface-1.7.0/python/dmi/sw_management_service_pb2.py` & `device-management-interface-1.8.0/python/dmi/sw_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/python/dmi/hw_metrics_mgmt_service_pb2_grpc.py` & `device-management-interface-1.8.0/python/dmi/hw_metrics_mgmt_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/python/dmi/commons_pb2.py` & `device-management-interface-1.8.0/python/dmi/commons_pb2.py`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/python/dmi/hw_events_mgmt_service_pb2_grpc.py` & `device-management-interface-1.8.0/python/dmi/hw_events_mgmt_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/python/dmi/hw_management_service_pb2.py` & `device-management-interface-1.8.0/python/dmi/hw_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/python/dmi/hw_metrics_mgmt_service_pb2.py` & `device-management-interface-1.8.0/python/dmi/hw_metrics_mgmt_service_pb2.py`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/python/dmi/hw_pb2.py` & `device-management-interface-1.8.0/python/dmi/hw_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x64mi/hw.proto\x12\x03\x64mi\x1a\x1fgoogle/protobuf/timestamp.proto\"\x14\n\x04Uuid\x12\x0c\n\x04uuid\x18\x01 \x01(\t\"%\n\nHardwareID\x12\x17\n\x04uuid\x18\x01 \x01(\x0b\x32\t.dmi.Uuid\"\x12\n\x03Uri\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xb5\x02\n\x0e\x43omponentState\x12\x36\n\x12state_last_changed\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\x0b\x61\x64min_state\x18\x02 \x01(\x0e\x32\x18.dmi.ComponentAdminState\x12+\n\noper_state\x18\x03 \x01(\x0e\x32\x17.dmi.ComponentOperState\x12-\n\x0busage_state\x18\x04 \x01(\x0e\x32\x18.dmi.ComponentUsageState\x12-\n\x0b\x61larm_state\x18\x05 \x01(\x0e\x32\x18.dmi.ComponentAlarmState\x12\x31\n\rstandby_state\x18\x06 \x01(\x0e\x32\x1a.dmi.ComponentStandbyState\"\x90\x02\n\x13\x43omponentSensorData\x12\r\n\x05value\x18\x01 \x01(\x05\x12 \n\x04type\x18\x02 \x01(\x0e\x32\x12.dmi.DataValueType\x12\x1e\n\x05scale\x18\x03 \x01(\x0e\x32\x0f.dmi.ValueScale\x12\x11\n\tprecision\x18\x04 \x01(\x05\x12!\n\x06status\x18\x05 \x01(\x0e\x32\x11.dmi.SensorStatus\x12\x15\n\runits_display\x18\x06 \x01(\t\x12-\n\ttimestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x19\n\x11value_update_rate\x18\x08 \x01(\r\x12\x11\n\tdata_type\x18\t \x01(\t\"\xe1\x05\n\x17PortComponentAttributes\x12\x42\n\x0e\x63onnector_type\x18\x01 \x01(\x0e\x32*.dmi.PortComponentAttributes.ConnectorType\x12\x31\n\x05speed\x18\x02 \x01(\x0e\x32\".dmi.PortComponentAttributes.Speed\x12\x37\n\x08protocol\x18\x03 \x01(\x0e\x32%.dmi.PortComponentAttributes.Protocol\x12\x16\n\x0ephysical_label\x18\x04 \x01(\t\x12\x15\n\rmapping_label\x18\x05 \x01(\t\x12\'\n\rpon_id_config\x18\x06 \x01(\x0b\x32\x10.dmi.PonIdConfig\x12\x1d\n\x15speed_autonegotiation\x18\x07 \x01(\x08\"p\n\rConnectorType\x12\x1c\n\x18\x43ONNECTOR_TYPE_UNDEFINED\x10\x00\x12\x08\n\x04RJ45\x10\x01\x12\x0c\n\x08\x46IBER_LC\x10\x02\x12\x0f\n\x0b\x46IBER_SC_PC\x10\x03\x12\r\n\tFIBER_MPO\x10\x04\x12\t\n\x05RS232\x10\x05\"\xae\x01\n\x05Speed\x12\x13\n\x0fSPEED_UNDEFINED\x10\x00\x12\x0b\n\x07\x44YNAMIC\x10\x01\x12\r\n\tGIGABIT_1\x10\x02\x12\x0e\n\nGIGABIT_10\x10\x03\x12\x0e\n\nGIGABIT_25\x10\x04\x12\x0e\n\nGIGABIT_40\x10\x05\x12\x0f\n\x0bGIGABIT_100\x10\x06\x12\x0f\n\x0bGIGABIT_400\x10\x07\x12\x10\n\x0cMEGABIT_2500\x10\x08\x12\x10\n\x0cMEGABIT_1250\x10\t\"|\n\x08Protocol\x12\x16\n\x12PROTOCOL_UNDEFINED\x10\x00\x12\x0c\n\x08\x45THERNET\x10\x01\x12\x08\n\x04GPON\x10\x02\x12\t\n\x05XGPON\x10\x03\x12\n\n\x06XGSPON\x10\x04\x12\t\n\x05GFAST\x10\x05\x12\n\n\x06SERIAL\x10\x06\x12\x08\n\x04\x45PON\x10\x07\x12\x08\n\x04\x42ITS\x10\x08\"H\n\x1dPortComponentChangeAttributes\x12\'\n\rpon_id_config\x18\x01 \x01(\x0b\x32\x10.dmi.PonIdConfig\"P\n$TransceiverComponentChangeAttributes\x12(\n\ntrans_type\x18\x01 \x01(\x0e\x32\x14.dmi.TransceiverType\"B\n\x0bPonIdConfig\x12\x0e\n\x06pon_id\x18\x01 \x01(\x0c\x12#\n\x1bpon_id_transmit_periodicity\x18\x02 \x01(\r\"6\n\x1c\x43ontainerComponentAttributes\x12\x16\n\x0ephysical_label\x18\x01 \x01(\t\"\xb3\x01\n\x16PsuComponentAttributes\x12G\n\x11supported_voltage\x18\x01 \x01(\x0e\x32,.dmi.PsuComponentAttributes.SupportedVoltage\"P\n\x10SupportedVoltage\x12\x1f\n\x1bSUPPORTED_VOLTAGE_UNDEFINED\x10\x00\x12\x07\n\x03V48\x10\x01\x12\x08\n\x04V230\x10\x02\x12\x08\n\x04V115\x10\x03\"\xf0\x03\n\x1fTransceiverComponentsAttributes\x12\x44\n\x0b\x66orm_factor\x18\x01 \x01(\x0e\x32/.dmi.TransceiverComponentsAttributes.FormFactor\x12(\n\ntrans_type\x18\x02 \x01(\x0e\x32\x14.dmi.TransceiverType\x12\x14\n\x0cmax_distance\x18\x03 \x01(\r\x12+\n\x12max_distance_scale\x18\x04 \x01(\x0e\x32\x0f.dmi.ValueScale\x12\x15\n\rrx_wavelength\x18\x05 \x03(\r\x12\x15\n\rtx_wavelength\x18\x06 \x03(\r\x12)\n\x10wavelength_scale\x18\x07 \x01(\x0e\x32\x0f.dmi.ValueScale\"\xc0\x01\n\nFormFactor\x12\x17\n\x13\x46ORM_FACTOR_UNKNOWN\x10\x00\x12\x08\n\x04QSFP\x10\x01\x12\r\n\tQSFP_PLUS\x10\x02\x12\n\n\x06QSFP28\x10\x03\x12\x07\n\x03SFP\x10\x04\x12\x0c\n\x08SFP_PLUS\x10\x05\x12\x07\n\x03XFP\x10\x06\x12\x08\n\x04\x43\x46P4\x10\x07\x12\x08\n\x04\x43\x46P2\x10\x08\x12\x08\n\x04\x43PAK\x10\t\x12\x06\n\x02X2\x10\n\x12\t\n\x05OTHER\x10\x0b\x12\x07\n\x03\x43\x46P\x10\x0c\x12\x0c\n\x08\x43\x46P2_ACO\x10\r\x12\x0c\n\x08\x43\x46P2_DCO\x10\x0e\"\xe8\x05\n\tComponent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12!\n\x05\x63lass\x18\x02 \x01(\x0e\x32\x12.dmi.ComponentType\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0e\n\x06parent\x18\x04 \x01(\t\x12\x16\n\x0eparent_rel_pos\x18\x05 \x01(\x05\x12 \n\x08\x63hildren\x18\x06 \x03(\x0b\x32\x0e.dmi.Component\x12\x14\n\x0chardware_rev\x18\x07 \x01(\t\x12\x14\n\x0c\x66irmware_rev\x18\x08 \x01(\t\x12\x14\n\x0csoftware_rev\x18\t \x01(\t\x12\x12\n\nserial_num\x18\n \x01(\t\x12\x10\n\x08mfg_name\x18\x0b \x01(\t\x12\x12\n\nmodel_name\x18\x0c \x01(\t\x12\r\n\x05\x61lias\x18\r \x01(\t\x12\x10\n\x08\x61sset_id\x18\x0e \x01(\t\x12\x0e\n\x06is_fru\x18\x0f \x01(\x08\x12,\n\x08mfg_date\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\x03uri\x18\x11 \x01(\x0b\x32\x08.dmi.Uri\x12\x17\n\x04uuid\x18\x12 \x01(\x0b\x32\t.dmi.Uuid\x12\"\n\x05state\x18\x13 \x01(\x0b\x32\x13.dmi.ComponentState\x12-\n\x0bsensor_data\x18\x14 \x03(\x0b\x32\x18.dmi.ComponentSensorData\x12\x31\n\tport_attr\x18\x32 \x01(\x0b\x32\x1c.dmi.PortComponentAttributesH\x00\x12;\n\x0e\x63ontainer_attr\x18\x33 \x01(\x0b\x32!.dmi.ContainerComponentAttributesH\x00\x12/\n\x08psu_attr\x18\x34 \x01(\x0b\x32\x1b.dmi.PsuComponentAttributesH\x00\x12@\n\x10transceiver_attr\x18\x35 \x01(\x0b\x32$.dmi.TransceiverComponentsAttributesH\x00\x42\n\n\x08specific\"\x8a\x01\n\x08Hardware\x12/\n\x0blast_change\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x04root\x18\x02 \x01(\x0b\x32\x0e.dmi.Component\x12/\n\x0blast_booted\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xe9\x02\n\x13ModifiableComponent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12!\n\x05\x63lass\x18\x02 \x01(\x0e\x32\x12.dmi.ComponentType\x12\x1e\n\x06parent\x18\x03 \x01(\x0b\x32\x0e.dmi.Component\x12\x16\n\x0eparent_rel_pos\x18\x04 \x01(\x05\x12\r\n\x05\x61lias\x18\x05 \x01(\t\x12\x10\n\x08\x61sset_id\x18\x06 \x01(\t\x12\x15\n\x03uri\x18\x07 \x01(\x0b\x32\x08.dmi.Uri\x12-\n\x0b\x61\x64min_state\x18\x08 \x01(\x0e\x32\x18.dmi.ComponentAdminState\x12\x37\n\tport_attr\x18\x32 \x01(\x0b\x32\".dmi.PortComponentChangeAttributesH\x00\x12=\n\x08trx_attr\x18\x33 \x01(\x0b\x32).dmi.TransceiverComponentChangeAttributesH\x00\x42\n\n\x08specific*\xb4\x03\n\rComponentType\x12\x1c\n\x18\x43OMPONENT_TYPE_UNDEFINED\x10\x00\x12\x1a\n\x16\x43OMPONENT_TYPE_UNKNOWN\x10\x01\x12\x1a\n\x16\x43OMPONENT_TYPE_CHASSIS\x10\x02\x12\x1c\n\x18\x43OMPONENT_TYPE_BACKPLANE\x10\x03\x12\x1c\n\x18\x43OMPONENT_TYPE_CONTAINER\x10\x04\x12\x1f\n\x1b\x43OMPONENT_TYPE_POWER_SUPPLY\x10\x05\x12\x16\n\x12\x43OMPONENT_TYPE_FAN\x10\x06\x12\x19\n\x15\x43OMPONENT_TYPE_SENSOR\x10\x07\x12\x19\n\x15\x43OMPONENT_TYPE_MODULE\x10\x08\x12\x17\n\x13\x43OMPONENT_TYPE_PORT\x10\t\x12\x16\n\x12\x43OMPONENT_TYPE_CPU\x10\n\x12\x1a\n\x16\x43OMPONENT_TYPE_BATTERY\x10\x0b\x12\x1a\n\x16\x43OMPONENT_TYPE_STORAGE\x10\x0c\x12\x19\n\x15\x43OMPONENT_TYPE_MEMORY\x10\r\x12\x1e\n\x1a\x43OMPONENT_TYPE_TRANSCEIVER\x10\x0e*\xb3\x01\n\x13\x43omponentAdminState\x12\x1e\n\x1a\x43OMP_ADMIN_STATE_UNDEFINED\x10\x00\x12\x1c\n\x18\x43OMP_ADMIN_STATE_UNKNOWN\x10\x01\x12\x1b\n\x17\x43OMP_ADMIN_STATE_LOCKED\x10\x02\x12\"\n\x1e\x43OMP_ADMIN_STATE_SHUTTING_DOWN\x10\x03\x12\x1d\n\x19\x43OMP_ADMIN_STATE_UNLOCKED\x10\x04*\xa8\x01\n\x12\x43omponentOperState\x12\x1d\n\x19\x43OMP_OPER_STATE_UNDEFINED\x10\x00\x12\x1b\n\x17\x43OMP_OPER_STATE_UNKNOWN\x10\x01\x12\x1c\n\x18\x43OMP_OPER_STATE_DISABLED\x10\x02\x12\x1b\n\x17\x43OMP_OPER_STATE_ENABLED\x10\x03\x12\x1b\n\x17\x43OMP_OPER_STATE_TESTING\x10\x04*\xa6\x01\n\x13\x43omponentUsageState\x12\x1e\n\x1a\x43OMP_USAGE_STATE_UNDEFINED\x10\x00\x12\x1c\n\x18\x43OMP_USAGE_STATE_UNKNOWN\x10\x01\x12\x19\n\x15\x43OMP_USAGE_STATE_IDLE\x10\x02\x12\x1b\n\x17\x43OMP_USAGE_STATE_ACTIVE\x10\x03\x12\x19\n\x15\x43OMP_USAGE_STATE_BUSY\x10\x04*\x8f\x02\n\x13\x43omponentAlarmState\x12\x1e\n\x1a\x43OMP_ALARM_STATE_UNDEFINED\x10\x00\x12\x1c\n\x18\x43OMP_ALARM_STATE_UNKNOWN\x10\x01\x12!\n\x1d\x43OMP_ALARM_STATE_UNDER_REPAIR\x10\x02\x12\x1d\n\x19\x43OMP_ALARM_STATE_CRITICAL\x10\x03\x12\x1a\n\x16\x43OMP_ALARM_STATE_MAJOR\x10\x04\x12\x1a\n\x16\x43OMP_ALARM_STATE_MINOR\x10\x05\x12\x1c\n\x18\x43OMP_ALARM_STATE_WARNING\x10\x06\x12\"\n\x1e\x43OMP_ALARM_STATE_INDETERMINATE\x10\x07*\xbc\x01\n\x15\x43omponentStandbyState\x12 \n\x1c\x43OMP_STANDBY_STATE_UNDEFINED\x10\x00\x12\x1e\n\x1a\x43OMP_STANDBY_STATE_UNKNOWN\x10\x01\x12\x1a\n\x16\x43OMP_STANDBY_STATE_HOT\x10\x02\x12\x1b\n\x17\x43OMP_STANDBY_STATE_COLD\x10\x03\x12(\n$COMP_STANDBY_STATE_PROVIDING_SERVICE\x10\x04*\x89\x03\n\rDataValueType\x12\x18\n\x14VALUE_TYPE_UNDEFINED\x10\x00\x12\x14\n\x10VALUE_TYPE_OTHER\x10\x01\x12\x16\n\x12VALUE_TYPE_UNKNOWN\x10\x02\x12\x17\n\x13VALUE_TYPE_VOLTS_AC\x10\x03\x12\x17\n\x13VALUE_TYPE_VOLTS_DC\x10\x04\x12\x16\n\x12VALUE_TYPE_AMPERES\x10\x05\x12\x14\n\x10VALUE_TYPE_WATTS\x10\x06\x12\x14\n\x10VALUE_TYPE_HERTZ\x10\x07\x12\x16\n\x12VALUE_TYPE_CELSIUS\x10\x08\x12\x19\n\x15VALUE_TYPE_PERCENT_RH\x10\t\x12\x12\n\x0eVALUE_TYPE_RPM\x10\n\x12\x12\n\x0eVALUE_TYPE_CMM\x10\x0b\x12\x1a\n\x16VALUE_TYPE_TRUTH_VALUE\x10\x0c\x12\x16\n\x12VALUE_TYPE_PERCENT\x10\r\x12\x15\n\x11VALUE_TYPE_METERS\x10\x0e\x12\x14\n\x10VALUE_TYPE_BYTES\x10\x0f*\xa4\x03\n\nValueScale\x12\x19\n\x15VALUE_SCALE_UNDEFINED\x10\x00\x12\x15\n\x11VALUE_SCALE_YOCTO\x10\x01\x12\x15\n\x11VALUE_SCALE_ZEPTO\x10\x02\x12\x14\n\x10VALUE_SCALE_ATTO\x10\x03\x12\x15\n\x11VALUE_SCALE_FEMTO\x10\x04\x12\x14\n\x10VALUE_SCALE_PICO\x10\x05\x12\x14\n\x10VALUE_SCALE_NANO\x10\x06\x12\x15\n\x11VALUE_SCALE_MICRO\x10\x07\x12\x15\n\x11VALUE_SCALE_MILLI\x10\x08\x12\x15\n\x11VALUE_SCALE_UNITS\x10\t\x12\x14\n\x10VALUE_SCALE_KILO\x10\n\x12\x14\n\x10VALUE_SCALE_MEGA\x10\x0b\x12\x14\n\x10VALUE_SCALE_GIGA\x10\x0c\x12\x14\n\x10VALUE_SCALE_TERA\x10\r\x12\x14\n\x10VALUE_SCALE_PETA\x10\x0e\x12\x13\n\x0fVALUE_SCALE_EXA\x10\x0f\x12\x15\n\x11VALUE_SCALE_ZETTA\x10\x10\x12\x15\n\x11VALUE_SCALE_YOTTA\x10\x11*\x82\x01\n\x0cSensorStatus\x12\x1b\n\x17SENSOR_STATUS_UNDEFINED\x10\x00\x12\x14\n\x10SENSOR_STATUS_OK\x10\x01\x12\x1d\n\x19SENSOR_STATUS_UNAVAILABLE\x10\x02\x12 \n\x1cSENSOR_STATUS_NONOPERATIONAL\x10\x03*\xa4\x01\n\x0fTransceiverType\x12\x12\n\x0eTYPE_UNDEFINED\x10\x00\x12\x0c\n\x08\x45THERNET\x10\x01\x12\x08\n\x04GPON\x10\x02\x12\t\n\x05XGPON\x10\x03\x12\n\n\x06XGSPON\x10\x04\x12\x08\n\x04\x43PON\x10\x05\x12\x0b\n\x07NG_PON2\x10\x06\x12\x08\n\x04\x45PON\x10\x07\x12\x15\n\x11\x43OMBO_GPON_XGSPON\x10\x08\x12\x16\n\x11TYPE_NOT_DETECTED\x10\xff\x01\x42;Z9github.com/opencord/device-management-interface/v3/go/dmib\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x64mi/hw.proto\x12\x03\x64mi\x1a\x1fgoogle/protobuf/timestamp.proto\"\x14\n\x04Uuid\x12\x0c\n\x04uuid\x18\x01 \x01(\t\"%\n\nHardwareID\x12\x17\n\x04uuid\x18\x01 \x01(\x0b\x32\t.dmi.Uuid\"\x12\n\x03Uri\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xb5\x02\n\x0e\x43omponentState\x12\x36\n\x12state_last_changed\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\x0b\x61\x64min_state\x18\x02 \x01(\x0e\x32\x18.dmi.ComponentAdminState\x12+\n\noper_state\x18\x03 \x01(\x0e\x32\x17.dmi.ComponentOperState\x12-\n\x0busage_state\x18\x04 \x01(\x0e\x32\x18.dmi.ComponentUsageState\x12-\n\x0b\x61larm_state\x18\x05 \x01(\x0e\x32\x18.dmi.ComponentAlarmState\x12\x31\n\rstandby_state\x18\x06 \x01(\x0e\x32\x1a.dmi.ComponentStandbyState\"\x90\x02\n\x13\x43omponentSensorData\x12\r\n\x05value\x18\x01 \x01(\x05\x12 \n\x04type\x18\x02 \x01(\x0e\x32\x12.dmi.DataValueType\x12\x1e\n\x05scale\x18\x03 \x01(\x0e\x32\x0f.dmi.ValueScale\x12\x11\n\tprecision\x18\x04 \x01(\x05\x12!\n\x06status\x18\x05 \x01(\x0e\x32\x11.dmi.SensorStatus\x12\x15\n\runits_display\x18\x06 \x01(\t\x12-\n\ttimestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x19\n\x11value_update_rate\x18\x08 \x01(\r\x12\x11\n\tdata_type\x18\t \x01(\t\"\xe1\x05\n\x17PortComponentAttributes\x12\x42\n\x0e\x63onnector_type\x18\x01 \x01(\x0e\x32*.dmi.PortComponentAttributes.ConnectorType\x12\x31\n\x05speed\x18\x02 \x01(\x0e\x32\".dmi.PortComponentAttributes.Speed\x12\x37\n\x08protocol\x18\x03 \x01(\x0e\x32%.dmi.PortComponentAttributes.Protocol\x12\x16\n\x0ephysical_label\x18\x04 \x01(\t\x12\x15\n\rmapping_label\x18\x05 \x01(\t\x12\'\n\rpon_id_config\x18\x06 \x01(\x0b\x32\x10.dmi.PonIdConfig\x12\x1d\n\x15speed_autonegotiation\x18\x07 \x01(\x08\"p\n\rConnectorType\x12\x1c\n\x18\x43ONNECTOR_TYPE_UNDEFINED\x10\x00\x12\x08\n\x04RJ45\x10\x01\x12\x0c\n\x08\x46IBER_LC\x10\x02\x12\x0f\n\x0b\x46IBER_SC_PC\x10\x03\x12\r\n\tFIBER_MPO\x10\x04\x12\t\n\x05RS232\x10\x05\"\xae\x01\n\x05Speed\x12\x13\n\x0fSPEED_UNDEFINED\x10\x00\x12\x0b\n\x07\x44YNAMIC\x10\x01\x12\r\n\tGIGABIT_1\x10\x02\x12\x0e\n\nGIGABIT_10\x10\x03\x12\x0e\n\nGIGABIT_25\x10\x04\x12\x0e\n\nGIGABIT_40\x10\x05\x12\x0f\n\x0bGIGABIT_100\x10\x06\x12\x0f\n\x0bGIGABIT_400\x10\x07\x12\x10\n\x0cMEGABIT_2500\x10\x08\x12\x10\n\x0cMEGABIT_1250\x10\t\"|\n\x08Protocol\x12\x16\n\x12PROTOCOL_UNDEFINED\x10\x00\x12\x0c\n\x08\x45THERNET\x10\x01\x12\x08\n\x04GPON\x10\x02\x12\t\n\x05XGPON\x10\x03\x12\n\n\x06XGSPON\x10\x04\x12\t\n\x05GFAST\x10\x05\x12\n\n\x06SERIAL\x10\x06\x12\x08\n\x04\x45PON\x10\x07\x12\x08\n\x04\x42ITS\x10\x08\"H\n\x1dPortComponentChangeAttributes\x12\'\n\rpon_id_config\x18\x01 \x01(\x0b\x32\x10.dmi.PonIdConfig\"P\n$TransceiverComponentChangeAttributes\x12(\n\ntrans_type\x18\x01 \x01(\x0e\x32\x14.dmi.TransceiverType\"B\n\x0bPonIdConfig\x12\x0e\n\x06pon_id\x18\x01 \x01(\x0c\x12#\n\x1bpon_id_transmit_periodicity\x18\x02 \x01(\r\"6\n\x1c\x43ontainerComponentAttributes\x12\x16\n\x0ephysical_label\x18\x01 \x01(\t\"\xb3\x01\n\x16PsuComponentAttributes\x12G\n\x11supported_voltage\x18\x01 \x01(\x0e\x32,.dmi.PsuComponentAttributes.SupportedVoltage\"P\n\x10SupportedVoltage\x12\x1f\n\x1bSUPPORTED_VOLTAGE_UNDEFINED\x10\x00\x12\x07\n\x03V48\x10\x01\x12\x08\n\x04V230\x10\x02\x12\x08\n\x04V115\x10\x03\"\xf0\x03\n\x1fTransceiverComponentsAttributes\x12\x44\n\x0b\x66orm_factor\x18\x01 \x01(\x0e\x32/.dmi.TransceiverComponentsAttributes.FormFactor\x12(\n\ntrans_type\x18\x02 \x01(\x0e\x32\x14.dmi.TransceiverType\x12\x14\n\x0cmax_distance\x18\x03 \x01(\r\x12+\n\x12max_distance_scale\x18\x04 \x01(\x0e\x32\x0f.dmi.ValueScale\x12\x15\n\rrx_wavelength\x18\x05 \x03(\r\x12\x15\n\rtx_wavelength\x18\x06 \x03(\r\x12)\n\x10wavelength_scale\x18\x07 \x01(\x0e\x32\x0f.dmi.ValueScale\"\xc0\x01\n\nFormFactor\x12\x17\n\x13\x46ORM_FACTOR_UNKNOWN\x10\x00\x12\x08\n\x04QSFP\x10\x01\x12\r\n\tQSFP_PLUS\x10\x02\x12\n\n\x06QSFP28\x10\x03\x12\x07\n\x03SFP\x10\x04\x12\x0c\n\x08SFP_PLUS\x10\x05\x12\x07\n\x03XFP\x10\x06\x12\x08\n\x04\x43\x46P4\x10\x07\x12\x08\n\x04\x43\x46P2\x10\x08\x12\x08\n\x04\x43PAK\x10\t\x12\x06\n\x02X2\x10\n\x12\t\n\x05OTHER\x10\x0b\x12\x07\n\x03\x43\x46P\x10\x0c\x12\x0c\n\x08\x43\x46P2_ACO\x10\r\x12\x0c\n\x08\x43\x46P2_DCO\x10\x0e\"\xe8\x05\n\tComponent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12!\n\x05\x63lass\x18\x02 \x01(\x0e\x32\x12.dmi.ComponentType\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0e\n\x06parent\x18\x04 \x01(\t\x12\x16\n\x0eparent_rel_pos\x18\x05 \x01(\x05\x12 \n\x08\x63hildren\x18\x06 \x03(\x0b\x32\x0e.dmi.Component\x12\x14\n\x0chardware_rev\x18\x07 \x01(\t\x12\x14\n\x0c\x66irmware_rev\x18\x08 \x01(\t\x12\x14\n\x0csoftware_rev\x18\t \x01(\t\x12\x12\n\nserial_num\x18\n \x01(\t\x12\x10\n\x08mfg_name\x18\x0b \x01(\t\x12\x12\n\nmodel_name\x18\x0c \x01(\t\x12\r\n\x05\x61lias\x18\r \x01(\t\x12\x10\n\x08\x61sset_id\x18\x0e \x01(\t\x12\x0e\n\x06is_fru\x18\x0f \x01(\x08\x12,\n\x08mfg_date\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\x03uri\x18\x11 \x01(\x0b\x32\x08.dmi.Uri\x12\x17\n\x04uuid\x18\x12 \x01(\x0b\x32\t.dmi.Uuid\x12\"\n\x05state\x18\x13 \x01(\x0b\x32\x13.dmi.ComponentState\x12-\n\x0bsensor_data\x18\x14 \x03(\x0b\x32\x18.dmi.ComponentSensorData\x12\x31\n\tport_attr\x18\x32 \x01(\x0b\x32\x1c.dmi.PortComponentAttributesH\x00\x12;\n\x0e\x63ontainer_attr\x18\x33 \x01(\x0b\x32!.dmi.ContainerComponentAttributesH\x00\x12/\n\x08psu_attr\x18\x34 \x01(\x0b\x32\x1b.dmi.PsuComponentAttributesH\x00\x12@\n\x10transceiver_attr\x18\x35 \x01(\x0b\x32$.dmi.TransceiverComponentsAttributesH\x00\x42\n\n\x08specific\"\x8a\x01\n\x08Hardware\x12/\n\x0blast_change\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x04root\x18\x02 \x01(\x0b\x32\x0e.dmi.Component\x12/\n\x0blast_booted\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xe9\x02\n\x13ModifiableComponent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12!\n\x05\x63lass\x18\x02 \x01(\x0e\x32\x12.dmi.ComponentType\x12\x1e\n\x06parent\x18\x03 \x01(\x0b\x32\x0e.dmi.Component\x12\x16\n\x0eparent_rel_pos\x18\x04 \x01(\x05\x12\r\n\x05\x61lias\x18\x05 \x01(\t\x12\x10\n\x08\x61sset_id\x18\x06 \x01(\t\x12\x15\n\x03uri\x18\x07 \x01(\x0b\x32\x08.dmi.Uri\x12-\n\x0b\x61\x64min_state\x18\x08 \x01(\x0e\x32\x18.dmi.ComponentAdminState\x12\x37\n\tport_attr\x18\x32 \x01(\x0b\x32\".dmi.PortComponentChangeAttributesH\x00\x12=\n\x08trx_attr\x18\x33 \x01(\x0b\x32).dmi.TransceiverComponentChangeAttributesH\x00\x42\n\n\x08specific*\xb4\x03\n\rComponentType\x12\x1c\n\x18\x43OMPONENT_TYPE_UNDEFINED\x10\x00\x12\x1a\n\x16\x43OMPONENT_TYPE_UNKNOWN\x10\x01\x12\x1a\n\x16\x43OMPONENT_TYPE_CHASSIS\x10\x02\x12\x1c\n\x18\x43OMPONENT_TYPE_BACKPLANE\x10\x03\x12\x1c\n\x18\x43OMPONENT_TYPE_CONTAINER\x10\x04\x12\x1f\n\x1b\x43OMPONENT_TYPE_POWER_SUPPLY\x10\x05\x12\x16\n\x12\x43OMPONENT_TYPE_FAN\x10\x06\x12\x19\n\x15\x43OMPONENT_TYPE_SENSOR\x10\x07\x12\x19\n\x15\x43OMPONENT_TYPE_MODULE\x10\x08\x12\x17\n\x13\x43OMPONENT_TYPE_PORT\x10\t\x12\x16\n\x12\x43OMPONENT_TYPE_CPU\x10\n\x12\x1a\n\x16\x43OMPONENT_TYPE_BATTERY\x10\x0b\x12\x1a\n\x16\x43OMPONENT_TYPE_STORAGE\x10\x0c\x12\x19\n\x15\x43OMPONENT_TYPE_MEMORY\x10\r\x12\x1e\n\x1a\x43OMPONENT_TYPE_TRANSCEIVER\x10\x0e*\xb3\x01\n\x13\x43omponentAdminState\x12\x1e\n\x1a\x43OMP_ADMIN_STATE_UNDEFINED\x10\x00\x12\x1c\n\x18\x43OMP_ADMIN_STATE_UNKNOWN\x10\x01\x12\x1b\n\x17\x43OMP_ADMIN_STATE_LOCKED\x10\x02\x12\"\n\x1e\x43OMP_ADMIN_STATE_SHUTTING_DOWN\x10\x03\x12\x1d\n\x19\x43OMP_ADMIN_STATE_UNLOCKED\x10\x04*\xa8\x01\n\x12\x43omponentOperState\x12\x1d\n\x19\x43OMP_OPER_STATE_UNDEFINED\x10\x00\x12\x1b\n\x17\x43OMP_OPER_STATE_UNKNOWN\x10\x01\x12\x1c\n\x18\x43OMP_OPER_STATE_DISABLED\x10\x02\x12\x1b\n\x17\x43OMP_OPER_STATE_ENABLED\x10\x03\x12\x1b\n\x17\x43OMP_OPER_STATE_TESTING\x10\x04*\xa6\x01\n\x13\x43omponentUsageState\x12\x1e\n\x1a\x43OMP_USAGE_STATE_UNDEFINED\x10\x00\x12\x1c\n\x18\x43OMP_USAGE_STATE_UNKNOWN\x10\x01\x12\x19\n\x15\x43OMP_USAGE_STATE_IDLE\x10\x02\x12\x1b\n\x17\x43OMP_USAGE_STATE_ACTIVE\x10\x03\x12\x19\n\x15\x43OMP_USAGE_STATE_BUSY\x10\x04*\x8f\x02\n\x13\x43omponentAlarmState\x12\x1e\n\x1a\x43OMP_ALARM_STATE_UNDEFINED\x10\x00\x12\x1c\n\x18\x43OMP_ALARM_STATE_UNKNOWN\x10\x01\x12!\n\x1d\x43OMP_ALARM_STATE_UNDER_REPAIR\x10\x02\x12\x1d\n\x19\x43OMP_ALARM_STATE_CRITICAL\x10\x03\x12\x1a\n\x16\x43OMP_ALARM_STATE_MAJOR\x10\x04\x12\x1a\n\x16\x43OMP_ALARM_STATE_MINOR\x10\x05\x12\x1c\n\x18\x43OMP_ALARM_STATE_WARNING\x10\x06\x12\"\n\x1e\x43OMP_ALARM_STATE_INDETERMINATE\x10\x07*\xbc\x01\n\x15\x43omponentStandbyState\x12 \n\x1c\x43OMP_STANDBY_STATE_UNDEFINED\x10\x00\x12\x1e\n\x1a\x43OMP_STANDBY_STATE_UNKNOWN\x10\x01\x12\x1a\n\x16\x43OMP_STANDBY_STATE_HOT\x10\x02\x12\x1b\n\x17\x43OMP_STANDBY_STATE_COLD\x10\x03\x12(\n$COMP_STANDBY_STATE_PROVIDING_SERVICE\x10\x04*\x9d\x03\n\rDataValueType\x12\x18\n\x14VALUE_TYPE_UNDEFINED\x10\x00\x12\x14\n\x10VALUE_TYPE_OTHER\x10\x01\x12\x16\n\x12VALUE_TYPE_UNKNOWN\x10\x02\x12\x17\n\x13VALUE_TYPE_VOLTS_AC\x10\x03\x12\x17\n\x13VALUE_TYPE_VOLTS_DC\x10\x04\x12\x16\n\x12VALUE_TYPE_AMPERES\x10\x05\x12\x14\n\x10VALUE_TYPE_WATTS\x10\x06\x12\x14\n\x10VALUE_TYPE_HERTZ\x10\x07\x12\x16\n\x12VALUE_TYPE_CELSIUS\x10\x08\x12\x19\n\x15VALUE_TYPE_PERCENT_RH\x10\t\x12\x12\n\x0eVALUE_TYPE_RPM\x10\n\x12\x12\n\x0eVALUE_TYPE_CMM\x10\x0b\x12\x1a\n\x16VALUE_TYPE_TRUTH_VALUE\x10\x0c\x12\x16\n\x12VALUE_TYPE_PERCENT\x10\r\x12\x15\n\x11VALUE_TYPE_METERS\x10\x0e\x12\x14\n\x10VALUE_TYPE_BYTES\x10\x0f\x12\x12\n\x0eVALUE_TYPE_DBM\x10\x10*\xa4\x03\n\nValueScale\x12\x19\n\x15VALUE_SCALE_UNDEFINED\x10\x00\x12\x15\n\x11VALUE_SCALE_YOCTO\x10\x01\x12\x15\n\x11VALUE_SCALE_ZEPTO\x10\x02\x12\x14\n\x10VALUE_SCALE_ATTO\x10\x03\x12\x15\n\x11VALUE_SCALE_FEMTO\x10\x04\x12\x14\n\x10VALUE_SCALE_PICO\x10\x05\x12\x14\n\x10VALUE_SCALE_NANO\x10\x06\x12\x15\n\x11VALUE_SCALE_MICRO\x10\x07\x12\x15\n\x11VALUE_SCALE_MILLI\x10\x08\x12\x15\n\x11VALUE_SCALE_UNITS\x10\t\x12\x14\n\x10VALUE_SCALE_KILO\x10\n\x12\x14\n\x10VALUE_SCALE_MEGA\x10\x0b\x12\x14\n\x10VALUE_SCALE_GIGA\x10\x0c\x12\x14\n\x10VALUE_SCALE_TERA\x10\r\x12\x14\n\x10VALUE_SCALE_PETA\x10\x0e\x12\x13\n\x0fVALUE_SCALE_EXA\x10\x0f\x12\x15\n\x11VALUE_SCALE_ZETTA\x10\x10\x12\x15\n\x11VALUE_SCALE_YOTTA\x10\x11*\x82\x01\n\x0cSensorStatus\x12\x1b\n\x17SENSOR_STATUS_UNDEFINED\x10\x00\x12\x14\n\x10SENSOR_STATUS_OK\x10\x01\x12\x1d\n\x19SENSOR_STATUS_UNAVAILABLE\x10\x02\x12 \n\x1cSENSOR_STATUS_NONOPERATIONAL\x10\x03*\xa4\x01\n\x0fTransceiverType\x12\x12\n\x0eTYPE_UNDEFINED\x10\x00\x12\x0c\n\x08\x45THERNET\x10\x01\x12\x08\n\x04GPON\x10\x02\x12\t\n\x05XGPON\x10\x03\x12\n\n\x06XGSPON\x10\x04\x12\x08\n\x04\x43PON\x10\x05\x12\x0b\n\x07NG_PON2\x10\x06\x12\x08\n\x04\x45PON\x10\x07\x12\x15\n\x11\x43OMBO_GPON_XGSPON\x10\x08\x12\x16\n\x11TYPE_NOT_DETECTED\x10\xff\x01\x42;Z9github.com/opencord/device-management-interface/v3/go/dmib\x06proto3')
 
 _COMPONENTTYPE = DESCRIPTOR.enum_types_by_name['ComponentType']
 ComponentType = enum_type_wrapper.EnumTypeWrapper(_COMPONENTTYPE)
 _COMPONENTADMINSTATE = DESCRIPTOR.enum_types_by_name['ComponentAdminState']
 ComponentAdminState = enum_type_wrapper.EnumTypeWrapper(_COMPONENTADMINSTATE)
 _COMPONENTOPERSTATE = DESCRIPTOR.enum_types_by_name['ComponentOperState']
 ComponentOperState = enum_type_wrapper.EnumTypeWrapper(_COMPONENTOPERSTATE)
@@ -93,14 +93,15 @@
 VALUE_TYPE_PERCENT_RH = 9
 VALUE_TYPE_RPM = 10
 VALUE_TYPE_CMM = 11
 VALUE_TYPE_TRUTH_VALUE = 12
 VALUE_TYPE_PERCENT = 13
 VALUE_TYPE_METERS = 14
 VALUE_TYPE_BYTES = 15
+VALUE_TYPE_DBM = 16
 VALUE_SCALE_UNDEFINED = 0
 VALUE_SCALE_YOCTO = 1
 VALUE_SCALE_ZEPTO = 2
 VALUE_SCALE_ATTO = 3
 VALUE_SCALE_FEMTO = 4
 VALUE_SCALE_PICO = 5
 VALUE_SCALE_NANO = 6
@@ -269,21 +270,21 @@
   _COMPONENTUSAGESTATE._serialized_start=4468
   _COMPONENTUSAGESTATE._serialized_end=4634
   _COMPONENTALARMSTATE._serialized_start=4637
   _COMPONENTALARMSTATE._serialized_end=4908
   _COMPONENTSTANDBYSTATE._serialized_start=4911
   _COMPONENTSTANDBYSTATE._serialized_end=5099
   _DATAVALUETYPE._serialized_start=5102
-  _DATAVALUETYPE._serialized_end=5495
-  _VALUESCALE._serialized_start=5498
-  _VALUESCALE._serialized_end=5918
-  _SENSORSTATUS._serialized_start=5921
-  _SENSORSTATUS._serialized_end=6051
-  _TRANSCEIVERTYPE._serialized_start=6054
-  _TRANSCEIVERTYPE._serialized_end=6218
+  _DATAVALUETYPE._serialized_end=5515
+  _VALUESCALE._serialized_start=5518
+  _VALUESCALE._serialized_end=5938
+  _SENSORSTATUS._serialized_start=5941
+  _SENSORSTATUS._serialized_end=6071
+  _TRANSCEIVERTYPE._serialized_start=6074
+  _TRANSCEIVERTYPE._serialized_end=6238
   _UUID._serialized_start=54
   _UUID._serialized_end=74
   _HARDWAREID._serialized_start=76
   _HARDWAREID._serialized_end=113
   _URI._serialized_start=115
   _URI._serialized_end=133
   _COMPONENTSTATE._serialized_start=136
```

### Comparing `device-management-interface-1.7.0/python/dmi/sw_image_pb2.py` & `device-management-interface-1.8.0/python/dmi/sw_image_pb2.py`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/python/dmi/hw_management_service_pb2_grpc.py` & `device-management-interface-1.8.0/python/dmi/hw_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `device-management-interface-1.7.0/python/dmi/sw_management_service_pb2_grpc.py` & `device-management-interface-1.8.0/python/dmi/sw_management_service_pb2_grpc.py`

 * *Files identical despite different names*

