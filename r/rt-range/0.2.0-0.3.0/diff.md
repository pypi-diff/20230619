# Comparing `tmp/rt_range-0.2.0.tar.gz` & `tmp/rt_range-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rt_range-0.2.0.tar", last modified: Fri Jun 16 20:15:18 2023, max compression
+gzip compressed data, was "rt_range-0.3.0.tar", last modified: Mon Jun 19 21:31:40 2023, max compression
```

## Comparing `rt_range-0.2.0.tar` & `rt_range-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:15:18.380720 rt_range-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-16 20:14:59.000000 rt_range-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-16 20:15:18.380720 rt_range-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-16 20:14:59.000000 rt_range-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-16 20:14:59.000000 rt_range-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 20:15:18.380720 rt_range-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:15:18.376720 rt_range-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:15:18.376720 rt_range-0.2.0/src/rt_range/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:15:18.376720 rt_range-0.2.0/src/rt_range/ethernet/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/eth_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:15:18.376720 rt_range-0.2.0/src/rt_range/ethernet/ncom/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/ncom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/ncom/batch_s.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/ncom/ncom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:15:18.380720 rt_range-0.2.0/src/rt_range/ethernet/rcom/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/rcom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/rcom/extended_range_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/rcom/lane_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/rcom/wrapped_ncom_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/rt_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/rt_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-06-16 20:14:59.000000 rt_range-0.2.0/src/rt_range/ethernet/status_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:15:18.376720 rt_range-0.2.0/src/rt_range.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-16 20:15:18.000000 rt_range-0.2.0/src/rt_range.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-16 20:15:18.000000 rt_range-0.2.0/src/rt_range.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:15:18.000000 rt_range-0.2.0/src/rt_range.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-16 20:15:18.000000 rt_range-0.2.0/src/rt_range.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 20:15:18.000000 rt_range-0.2.0/src/rt_range.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:15:18.380720 rt_range-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-16 20:14:59.000000 rt_range-0.2.0/test/test_eth_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-16 20:14:59.000000 rt_range-0.2.0/test/test_ncom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-16 20:14:59.000000 rt_range-0.2.0/test/test_rcom_extended_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-16 20:14:59.000000 rt_range-0.2.0/test/test_rcom_lane.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-16 20:14:59.000000 rt_range-0.2.0/test/test_rcom_wrapped_ncom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-16 20:14:59.000000 rt_range-0.2.0/test/test_rt_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:31:40.632707 rt_range-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-19 21:31:29.000000 rt_range-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-06-19 21:31:40.632707 rt_range-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-19 21:31:29.000000 rt_range-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-19 21:31:29.000000 rt_range-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 21:31:40.632707 rt_range-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:31:40.628707 rt_range-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:31:40.628707 rt_range-0.3.0/src/rt_range/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:31:40.632707 rt_range-0.3.0/src/rt_range/ethernet/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/eth_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:31:40.632707 rt_range-0.3.0/src/rt_range/ethernet/ncom/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/ncom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/ncom/batch_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/ncom/ncom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:31:40.632707 rt_range-0.3.0/src/rt_range/ethernet/rcom/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/rcom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/rcom/extended_range_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/rcom/lane_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/rcom/wrapped_ncom_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/rt_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/rt_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/status_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:31:40.632707 rt_range-0.3.0/src/rt_range.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-06-19 21:31:40.000000 rt_range-0.3.0/src/rt_range.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-19 21:31:40.000000 rt_range-0.3.0/src/rt_range.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 21:31:40.000000 rt_range-0.3.0/src/rt_range.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-19 21:31:40.000000 rt_range-0.3.0/src/rt_range.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 21:31:40.000000 rt_range-0.3.0/src/rt_range.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:31:40.632707 rt_range-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-19 21:31:29.000000 rt_range-0.3.0/test/test_eth_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-19 21:31:29.000000 rt_range-0.3.0/test/test_ncom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-19 21:31:29.000000 rt_range-0.3.0/test/test_rcom_extended_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-19 21:31:29.000000 rt_range-0.3.0/test/test_rcom_lane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-19 21:31:29.000000 rt_range-0.3.0/test/test_rcom_wrapped_ncom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-19 21:31:29.000000 rt_range-0.3.0/test/test_rt_packet.py
```

### Comparing `rt_range-0.2.0/LICENSE.txt` & `rt_range-0.3.0/LICENSE.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [year] [fullname]
+Copyright (c) 2023 Sheetlar
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `rt_range-0.2.0/PKG-INFO` & `rt_range-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: rt_range
-Version: 0.2.0
+Version: 0.3.0
 Summary: OxTS RT-Range data parsing utility
 License: MIT License
         
-        Copyright (c) [year] [fullname]
+        Copyright (c) 2023 Sheetlar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -19,14 +19,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+        
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # OxTS RT-Range data parsing utility
 
 This simple parser is capable of parsing RT-Range Ethernet packets (NCOM and RCOM).
```

### Comparing `rt_range-0.2.0/README.md` & `rt_range-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `rt_range-0.2.0/src/rt_range/common.py` & `rt_range-0.3.0/src/rt_range/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from typing import Iterable
 
 
+def convert_10_pow_m1(value: int):
+    return value / 10
+
+
 def convert_10_pow_m2(value: int):
     return value / 100
 
 
 def convert_10_pow_m3(value: int):
     return value / 1000
 
@@ -21,13 +25,17 @@
     return value / 1000000
 
 
 def convert_10_pow_m7(value: int):
     return value / 10000000
 
 
+def validity_bit0(value: int):
+    return value & 0x7f
+
+
 def flatten(iterable: Iterable):
     for item in iterable:
         if isinstance(item, Iterable) and not isinstance(item, (str, bytes)):
             yield from flatten(item)
         else:
             yield item
```

### Comparing `rt_range-0.2.0/src/rt_range/ethernet/eth_parser.py` & `rt_range-0.3.0/src/rt_range/ethernet/eth_parser.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.2.0/src/rt_range/ethernet/ncom/batch_s.py` & `rt_range-0.3.0/src/rt_range/ethernet/ncom/ncom.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,39 @@
-from rt_range.ethernet.rt_types import Field, Long, UByte, UShort
-from rt_range.ethernet.status_definitions import decode_enum, ncom_position_velocity_orientation_mode, ncom_blended_processing_methods
+from rt_range.common import convert_10_pow_m3, convert_10_pow_m4, convert_10_pow_m5, convert_10_pow_m6
+from rt_range.ethernet.ncom.batch_s import BatchS
+from rt_range.ethernet.rt_packet import Packet
+from rt_range.ethernet.rt_types import Field, UByte, UShort, Word, Float, Double, VariableBlock
+from rt_range.ethernet.status_definitions import decode_enum, ncom_nav_status, ncom_channel_status
 
-BatchS = {  # TODO: Block definitions for other status_channel values
-    0: [Field('time_since_gps', Long, unit='min'),
-        Field('num_satellites', UByte),
-        Field('position_mode', UByte, decode_value=decode_enum(ncom_position_velocity_orientation_mode)),
-        Field('velocity_mode', UByte, decode_value=decode_enum(ncom_position_velocity_orientation_mode)),
-        Field('orientation_mode', UByte, decode_value=decode_enum(ncom_position_velocity_orientation_mode))],
-    3: [Field('north_position_accuracy', UShort, unit='mm'),
-        Field('east_position_accuracy', UShort, unit='mm'),
-        Field('down_position_accuracy', UShort, unit='mm'),
-        Field('age', UByte),
-        Field('ABD_robot_UMAC_interface_status', UByte)],
-    4: [Field('north_velocity_accuracy', UShort, unit='mm/s'),
-        Field('east_velocity_accuracy', UShort, unit='mm/s'),
-        Field('down_velocity_accuracy', UShort, unit='mm/s'),
-        Field('age', UByte),
-        Field('processing_method', UByte, decode_value=decode_enum(ncom_blended_processing_methods))],
-    5: [Field('heading_accuracy', UShort, unit='mm'),
-        Field('pitch_accuracy', UShort, unit='mm'),
-        Field('roll_accuracy', UShort, unit='mm'),
-        Field('age', UByte),
-        Field('reserved', UByte)],
-}
+
+BatchA = [
+    Field('time', UShort, decode_value=convert_10_pow_m3, unit='s'),
+    Field('acceleration_x', Word, decode_value=convert_10_pow_m4, unit='m/s^2'),
+    Field('acceleration_y', Word, decode_value=convert_10_pow_m4, unit='m/s^2'),
+    Field('acceleration_z', Word, decode_value=convert_10_pow_m4, unit='m/s^2'),
+    Field('angular_rate_x', Word, decode_value=convert_10_pow_m5, unit='rad/s'),
+    Field('angular_rate_y', Word, decode_value=convert_10_pow_m5, unit='rad/s'),
+    Field('angular_rate_z', Word, decode_value=convert_10_pow_m5, unit='rad/s'),
+]
+BatchB = [
+    Field('latitude', Double, unit='rad'),
+    Field('longitude', Double, unit='rad'),
+    Field('altitude', Float, unit='m'),
+    Field('north_velocity', Word, decode_value=convert_10_pow_m4, unit='m/s'),
+    Field('east_velocity', Word, decode_value=convert_10_pow_m4, unit='m/s'),
+    Field('down_velocity', Word, decode_value=convert_10_pow_m4, unit='m/s'),
+    Field('heading', Word, decode_value=convert_10_pow_m6, unit='rad'),
+    Field('pitch', Word, decode_value=convert_10_pow_m6, unit='rad'),
+    Field('roll', Word, decode_value=convert_10_pow_m6, unit='rad'),
+]
+
+NCOM = Packet([
+    Field('sync', UByte),  # 0xE7
+    *BatchA,
+    Field('nav_status', UByte, decode_value=decode_enum(ncom_nav_status)),
+    Field('checksum_1', UByte),
+    *BatchB,
+    Field('checksum_2', UByte),
+    Field('status_channel', UByte, decode_value=decode_enum(ncom_channel_status)),
+    VariableBlock(selector=62, name='batch_s', size=8, structure=BatchS),
+    Field('checksum_3', UByte),
+])
```

### Comparing `rt_range-0.2.0/src/rt_range/ethernet/rcom/extended_range_packet.py` & `rt_range-0.3.0/src/rt_range/ethernet/rcom/extended_range_packet.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.2.0/src/rt_range/ethernet/rcom/lane_packet.py` & `rt_range-0.3.0/src/rt_range/ethernet/rcom/lane_packet.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.2.0/src/rt_range/ethernet/rcom/wrapped_ncom_packet.py` & `rt_range-0.3.0/src/rt_range/ethernet/rcom/wrapped_ncom_packet.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.2.0/src/rt_range/ethernet/rt_packet.py` & `rt_range-0.3.0/src/rt_range/ethernet/rt_packet.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.2.0/src/rt_range/ethernet/rt_types.py` & `rt_range-0.3.0/src/rt_range/ethernet/rt_types.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.2.0/src/rt_range/ethernet/status_definitions.py` & `rt_range-0.3.0/src/rt_range/ethernet/status_definitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     17: 'Internal_info_secondary_antenna',
     18: 'Internal_info_IMU',
     19: 'INS_SW_version',
     20: 'Differential_correction_info',
     21: 'Disk_space_log_size',
     22: 'Internal_info_processing_timing',
     23: 'Up_time_GNSS_rejections_PTP_status',
-    24: 'Async_packet_event_input_falling_edge',
+    24: 'Asynchronous_packet_event_input_falling_edge',
     25: 'Reserved',
     26: 'Displacement_lever_arm',
     27: 'Internal_info_dual_antenna_ambiguity',
     28: 'Internal_info_dual_antenna_ambiguity',
     29: 'Initial_settings_NAVconfig',
     30: 'OS_script_version_info',
     31: 'HW_config_info',
@@ -164,14 +164,31 @@
     1: 'Real_time',
     2: 'Simulated',
     3: 'Post_process_forward',
     4: 'Post_process_backward',
     5: 'Post_process_combined',
     6: 'Unknown',
 }
+ncom_ptp_status = {
+    KeyError: 'Value_not_in_documentation',
+    0: 'PTP_status_invalid',
+    1: 'PTP_status_initializing',
+    2: 'PTP_status_faulty',
+    3: 'PTP_status_disabled',
+    4: 'PTP_status_listening',
+    5: 'PTP_status_pre_master',
+    6: 'PTP_status_master',
+    7: 'PTP_status_passive',
+    8: 'PTP_status_uncalibrated',
+    9: 'PTP_status_slave',
+    10: 'PTP_status_locked',
+    11: 'PTP_status_config_error',
+    12: 'PTP_status_critical_error',
+    13: 'PTP_status_unknown',
+}
 rcom_lane_status_channel = {
     KeyError: 'Value_not_in_documentation',
     0: 'GPS_coarse_time',
     1: 'RT-Range_SW_dev_ID',
     2: 'Map_number',
     6: 'OS_and_script_version',
     7: 'UTC_offset_CPU_load',
```

### Comparing `rt_range-0.2.0/src/rt_range.egg-info/PKG-INFO` & `rt_range-0.3.0/src/rt_range.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: rt-range
-Version: 0.2.0
+Version: 0.3.0
 Summary: OxTS RT-Range data parsing utility
 License: MIT License
         
-        Copyright (c) [year] [fullname]
+        Copyright (c) 2023 Sheetlar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -19,14 +19,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+        
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # OxTS RT-Range data parsing utility
 
 This simple parser is capable of parsing RT-Range Ethernet packets (NCOM and RCOM).
```

### Comparing `rt_range-0.2.0/src/rt_range.egg-info/SOURCES.txt` & `rt_range-0.3.0/src/rt_range.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rt_range-0.2.0/test/test_eth_parser.py` & `rt_range-0.3.0/test/test_eth_parser.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.2.0/test/test_ncom.py` & `rt_range-0.3.0/test/test_ncom.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.2.0/test/test_rcom_extended_range.py` & `rt_range-0.3.0/test/test_rcom_extended_range.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.2.0/test/test_rcom_lane.py` & `rt_range-0.3.0/test/test_rcom_lane.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.2.0/test/test_rcom_wrapped_ncom.py` & `rt_range-0.3.0/test/test_rcom_wrapped_ncom.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.2.0/test/test_rt_packet.py` & `rt_range-0.3.0/test/test_rt_packet.py`

 * *Files identical despite different names*

