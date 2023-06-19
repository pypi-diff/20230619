# Comparing `tmp/dl_myo-0.2.0.tar.gz` & `tmp/dl_myo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dl_myo-0.2.0.tar", max compression
+gzip compressed data, was "dl_myo-1.0.0.tar", max compression
```

## Comparing `dl_myo-0.2.0.tar` & `dl_myo-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0    35131 2023-06-14 22:05:38.798261 dl_myo-0.2.0/LICENSE
--rw-r--r--   0        0        0     2514 2023-06-14 22:05:38.798261 dl_myo-0.2.0/README.md
--rw-r--r--   0        0        0     7012 2023-06-14 22:05:38.802261 dl_myo-0.2.0/myo/__init__.py
--rw-r--r--   0        0        0     3226 2023-06-14 22:05:38.802261 dl_myo-0.2.0/myo/commands.py
--rw-r--r--   0        0        0     5783 2023-06-14 22:05:38.802261 dl_myo-0.2.0/myo/handle.py
--rw-r--r--   0        0        0     9499 2023-06-14 22:05:38.802261 dl_myo-0.2.0/myo/types.py
--rw-r--r--   0        0        0     3194 2023-06-14 22:05:57.490298 dl_myo-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3151 1970-01-01 00:00:00.000000 dl_myo-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35123 2023-06-19 21:19:24.631658 dl_myo-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3837 2023-06-19 21:19:24.631658 dl_myo-1.0.0/README.md
+-rw-r--r--   0        0        0      749 2023-06-19 21:19:24.631658 dl_myo-1.0.0/myo/__init__.py
+-rw-r--r--   0        0        0    10771 2023-06-19 21:19:24.631658 dl_myo-1.0.0/myo/client.py
+-rw-r--r--   0        0        0     3293 2023-06-19 21:19:24.631658 dl_myo-1.0.0/myo/commands.py
+-rw-r--r--   0        0        0      503 2023-06-19 21:19:24.631658 dl_myo-1.0.0/myo/constants.py
+-rw-r--r--   0        0        0     4331 2023-06-19 21:19:24.631658 dl_myo-1.0.0/myo/core.py
+-rw-r--r--   0        0        0     5802 2023-06-19 21:19:24.631658 dl_myo-1.0.0/myo/profile.py
+-rw-r--r--   0        0        0     9161 2023-06-19 21:19:24.631658 dl_myo-1.0.0/myo/types.py
+-rw-r--r--   0        0        0       22 2023-06-19 21:19:24.631658 dl_myo-1.0.0/myo/version.py
+-rw-r--r--   0        0        0     3271 2023-06-19 21:19:41.955942 dl_myo-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4462 1970-01-01 00:00:00.000000 dl_myo-1.0.0/PKG-INFO
```

### Comparing `dl_myo-0.2.0/LICENSE` & `dl_myo-1.0.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -627,15 +627,15 @@
 free software which everyone can redistribute and change under these terms.
 
   To do so, attach the following notices to the program.  It is safest
 to attach them to the start of each source file to most effectively
 state the exclusion of warranty; and each file should have at least
 the "copyright" line and a pointer to where the full notice is found.
 
-    dl-myo: Replacement for MyoConnect without the official Myo dongle
+    dl-myo: Yet another MyoConnect alternative without dongles
     Copyright (C) 2023  Iori Mizutani
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
```

### Comparing `dl_myo-0.2.0/myo/commands.py` & `dl_myo-1.0.0/myo/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-# -*- coding: utf-8 -*-
+"""
+    myo.commands
+    ------------
+    The available commands derived from myohw.h
+"""
+
 from .types import SleepMode, UnlockType, UserActionType
 
 
 # myohw_command_t
 class Command:
     cmd = 0x00
```

### Comparing `dl_myo-0.2.0/myo/handle.py` & `dl_myo-1.0.0/myo/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,17 @@
-# -*- coding: utf-8 -*-
 """
-# myo/handle.py
-#
-# reflection from myo-bluetooth/myohw.h
-# the names are slightly different in dl-myo
-#
+    myo.profile
+    ------------
+    GATTProfile is deducted from the GATT profile
+    while Handle is the cleaned-up version used in dl-myo
 """
 import aenum
 
 
-# fmt: off
-class Handle(aenum.Enum):
-    DEVICE_INFORMATION = 12  # 0x0c
-    MANUFACTURER_NAME_STRING = 13  # 0x0d
-    BATTERY_SERVICE = 15     # 0x0f
-    BATTERY_LEVEL = 16       # 0x10
-    CONTROL_SERVICE = 19     # 0x13
-    FIRMWARE_INFO = 20       # 0x14
-    FIRMWARE_VERSION = 22    # 0x16
-    COMMAND = 24             # 0x18
-    IMU_SERVICE = 26         # 0x1a
-    IMU_DATA = 27            # 0x1b
-    MOTION_EVENT = 30        # 0x1e
-    CLASSIFIER_SERVICE = 33  # 0x21
-    CLASSIFIER_EVENT = 34    # 0x22
-    FV_SERVICE = 37          # 0x25: EMG Filtered Value Service
-    FV_DATA = 38             # 0x26: EMG Filtered Value Data
-    EMG_SERVICE = 41         # 0x29
-    EMG0_DATA = 42           # 0x2a
-    EMG1_DATA = 45           # 0x2d
-    EMG2_DATA = 48           # 0x30
-    EMG3_DATA = 51           # 0x33
-    UNKNOWN_SERVICE = 54     # 0x36
-    UNKNOWN_CHAR = 55        # 0x37
-# fmt: on
-
-
-class UUID:
+class GATTProfile:
     MYO_SERVICE = "d5060001-a904-deb9-4748-2c7f4a124842"
 
     # [Service] (Handle: 12): Device Information
     DEVICE_INFORMATION = "0000180a-0000-1000-8000-00805f9b34fb"
     #  [Characteristic] (Handle: 13): Manufacturer Name String (read)
     #                                 Value: bytearray(b'Thalmic Labs')
     MANUFACTURER_NAME_STRING = "00002a29-0000-1000-8000-00805f9b34fb"
@@ -120,7 +91,34 @@
     # [Service] (Handle: 54): Unknown Service
     UNKNOWN_SERVICE = "d5060006-a904-deb9-4748-2c7f4a124842"
     #   [Characteristic] (Handle: 55): Unknown Characteristic (indicate)
     #     [Descriptor] 00002902-0000-1000-8000-00805f9b34fb
     #                  (Handle: 57): Client Characteristic Configuration
     #                                Value: bytearray(b'')
     UNKNOWN_CHAR = "d5060602-a904-deb9-4748-2c7f4a124842"
+
+
+# fmt: off
+class Handle(aenum.Enum):
+    DEVICE_INFORMATION = 12  # 0x0c
+    MANUFACTURER_NAME_STRING = 13  # 0x0d
+    BATTERY_SERVICE = 15     # 0x0f
+    BATTERY_LEVEL = 16       # 0x10
+    CONTROL_SERVICE = 19     # 0x13
+    FIRMWARE_INFO = 20       # 0x14
+    FIRMWARE_VERSION = 22    # 0x16
+    COMMAND = 24             # 0x18
+    IMU_SERVICE = 26         # 0x1a
+    IMU_DATA = 27            # 0x1b
+    MOTION_EVENT = 30        # 0x1e
+    CLASSIFIER_SERVICE = 33  # 0x21
+    CLASSIFIER_EVENT = 34    # 0x22
+    FV_SERVICE = 37          # 0x25: EMG Filtered Value Service
+    FV_DATA = 38             # 0x26: EMG Filtered Value Data
+    EMG_SERVICE = 41         # 0x29
+    EMG0_DATA = 42           # 0x2a
+    EMG1_DATA = 45           # 0x2d
+    EMG2_DATA = 48           # 0x30
+    EMG3_DATA = 51           # 0x33
+    UNKNOWN_SERVICE = 54     # 0x36
+    UNKNOWN_CHAR = 55        # 0x37
+# fmt: on
```

### Comparing `dl_myo-0.2.0/myo/types.py` & `dl_myo-1.0.0/myo/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,26 @@
-# -*- coding: utf-8 -*-type
 """
-# myo/types.py
-#
-# type reflection from myo-bluetooth/myohw.h
-#
+    myo.types
+    ------------
+    Type reflections from myo-bluetooth/myohw.h
 """
+
+
 import json
 import struct
 
 import aenum
 
-
-class Constant(aenum.NamedConstant):
-    ACCELEROMETER_SCALE = 2048.0
-    CCCD_NOTIFY = b"\x01\x00"
-    CCCD_INDICATE = b"\x02\x00"
-    CCCD_DISABLE = b"\x00\x00"
-    DEFAULT_IMU_SAMPLE_RATE = 50
-    EMG_DEFAULT_STREAMING_RATE = 200
-    GYROSCOPE_SCALE = 16.0
-    ORIENTATION_SCALE = 16384.0
+from .constants import (
+    ACCELEROMETER_SCALE,
+    GYROSCOPE_SCALE,
+    ORIENTATION_SCALE,
+)
 
 
-# -> myohw_arm_t
 class Arm(aenum.Enum):
     RIGHT = 0x01
     LEFT = 0x02
     UNKNOWN = 0xFF
 
 
 # -> myohw_classifier_event_t
@@ -112,15 +106,14 @@
         return {"sample1": self.sample1, "sample2": self.sample2}
 
 
 # for the FV_DATA in the old firmware versions (?)
 # cf. https://github.com/dzhu/myo-raw/blob/6873d04d647702b304b0592ee25994d196659bb0/myo_raw.py#LL276C11-L276C11
 class FVData:
     def __init__(self, data):
-        assert len(data) == 17
         u = struct.unpack('<8Hb', data)
         self.fv = u[:8]
         self.mask = u[8]
 
     def __repr__(self):
         return str(self.fv + (self.mask,))
 
@@ -145,15 +138,14 @@
 # fmt: on
 
 
 # -> myohw_fw_info_t
 class FirmwareInfo:
     def __init__(self, data):
         u = struct.unpack("<6BH12B", data)  # 20 bytes
-        assert len(u) == 19
         ser = list(u[:6])
         ser.reverse()
         ser = [hex(i)[-2:] for i in ser]
         self._serial_number = ":".join(ser).upper()
         self._unlock_pose = Pose(u[6]).name
         self._active_classifier_type = ClassifierModelType(u[7]).name
         self._active_classifier_index = u[8]
@@ -195,27 +187,27 @@
     REVS = 3
 
 
 # -> myohw_imu_data_t
 class IMUData:
     class Orientation:
         def __init__(self, w, x, y, z):
-            self.w = w / Constant.ORIENTATION_SCALE
-            self.x = x / Constant.ORIENTATION_SCALE
-            self.y = y / Constant.ORIENTATION_SCALE
-            self.z = z / Constant.ORIENTATION_SCALE
+            self.w = w / ORIENTATION_SCALE
+            self.x = x / ORIENTATION_SCALE
+            self.y = y / ORIENTATION_SCALE
+            self.z = z / ORIENTATION_SCALE
 
         def to_dict(self):
             return {"w": self.w, "x": self.x, "y": self.y, "z": self.z}
 
     def __init__(self, data):
         u = struct.unpack("<10h", data)
         self.orientation = self.Orientation(u[0], u[1], u[2], u[3])
-        self.accelerometer = [v / Constant.ACCELEROMETER_SCALE for v in u[4:7]]
-        self.gyroscope = [v / Constant.GYROSCOPE_SCALE for v in u[7:10]]
+        self.accelerometer = [v / ACCELEROMETER_SCALE for v in u[4:7]]
+        self.gyroscope = [v / GYROSCOPE_SCALE for v in u[7:10]]
 
     def __repr__(self):
         return str(
             (
                 self.orientation.w,
                 self.orientation.x,
                 self.orientation.y,
```

### Comparing `dl_myo-0.2.0/pyproject.toml` & `dl_myo-1.0.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "dl-myo"
 authors = [
-  { name="Iori Mizutani", email="iori.mizutani@gmail.com" },
+  { name="Iori Mizutani", email="iomz@sazanka.io" },
 ]
 maintainers = [
-  { name="Iori Mizutani", email="iori.mizutani@gmail.com" },
+  { name="Iori Mizutani", email="iomz@sazanka.io" },
 ]
-description = "A replacement middleware to MyoConnect for Myo Armband"
+description = "Yet another MyoConnect alternative without dongles"
 readme = "README.md"
 classifiers = [
     "Environment :: Console",
     "Framework :: AsyncIO",
     "Framework :: Hatch",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
@@ -19,14 +19,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Human Machine Interfaces",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
+dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/iomz/dl-myo"
 "Bug Tracker" = "https://github.com/iomz/dl-myo/issues"
 
 [tool.black]
 line-length = 120
@@ -64,43 +65,47 @@
     "node_modules",
     "venv",
 ]
 # Same as Black.
 line-length = 120
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
-# Assume Python 3.10.
+# Assume Python 3.11.
 target-version = "py311"
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
+"myo/__init__.py" = ["F401"]
 
 [tool.coverage.run]
 branch = true
-
-[tool.coverage.paths]
-tests = ["tests"]
+omit = [
+  # omit the __init__.py
+  "myo/__init__.py",
+  "myo/constants.py",
+  "myo/version.py",
+]
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
 [tool.poetry]
 name = "dl-myo"
-version = "0.2.0"
-description = "A replacement middleware to MyoConnect for Myo Armband"
-authors = ["Iori Mizutani <iori.mizutani@gmail.com>"]
+version = "1.0.0"
+description = "Yet another MyoConnect alternative without dongles"
+authors = ["Iori Mizutani <iomz@sazanka.io>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "myo"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aenum = "^3.1.12"
```

### Comparing `dl_myo-0.2.0/PKG-INFO` & `dl_myo-1.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,45 @@
-Metadata-Version: 2.1
-Name: dl-myo
-Version: 0.2.0
-Summary: A replacement middleware to MyoConnect for Myo Armband
-License: GPLv3
-Author: Iori Mizutani
-Author-email: iori.mizutani@gmail.com
-Requires-Python: >=3.8,<4.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aenum (>=3.1.12,<4.0.0)
-Requires-Dist: bleak (>=0.20.2,<0.21.0)
-Description-Content-Type: text/markdown
-
 # dl-myo (Dongle-less Myo)
 
 [![build status](https://github.com/iomz/dl-myo/workflows/build/badge.svg)](https://github.com/iomz/dl-myo/actions?query=workflow%3Abuild)
 [![image size](https://ghcr-badge.egpl.dev/iomz/dl-myo/size?label=image%20size)](https://github.com/iomz/dl-myo/pkgs/container/dl-myo)
 [![codecov](https://codecov.io/gh/iomz/dl-myo/branch/main/graph/badge.svg?token=7bC3Aa1XNN)](https://codecov.io/gh/iomz/dl-myo)
-[![python Versions](https://img.shields.io/pypi/pyversions/dl-myo.svg)](https://pypi.python.org/pypi/dl-myo)
+[![python versions](https://img.shields.io/pypi/pyversions/dl-myo.svg)](https://pypi.python.org/pypi/dl-myo)
 [![pypi version](https://img.shields.io/pypi/v/dl-myo.svg)](https://pypi.python.org/pypi/dl-myo)
 [![license](https://img.shields.io/pypi/l/dl-myo.svg)](https://pypi.python.org/pypi/dl-myo)
 
-dl-myo is a replacement to MyoConnect for Myo Armband without an official Myo dongle.
-
-If you are fed up with the dongle and still need to use Myo anyway this is the right stuff to grab.
+dl-myo is yet another MyoConnect alternative for Myo Armband without an official Myo dongle.
 
-This project is a reimplementation of [Dongleless-myo](https://github.com/iomz/Dongleless-myo) (originally created by [@mamo91](https://github.com/mamo91) and enhanced by [@MyrikLD](https://github.com/MyrikLD)) using [Bleak](https://github.com/hbldh/bleak) instead of [bluepy](https://github.com/IanHarvey/bluepy), and therefore supports asyncio on multiple platforms.
+If you are fed up with the dongle and still want to use Myo anyway (in Python), this is the right stuff to grab.
 
 The GATT service naming convention reflects the official BLE specification for Myo (i.e., [myohw.h](https://github.com/iomz/myo-bluetooth/blob/master/myohw.h)); however, some services and characteristics differ for a uniform naming.
 
-See [`myo/handle.py`](https://github.com/iomz/dl-myo/blob/main/myo/handle.py) for more detail.
+See [`myo/profile.py`](https://github.com/iomz/dl-myo/blob/main/myo/profile.py) for more detail.
+
+<!-- vim-markdown-toc GFM -->
+
+- [Features](#features)
+- [Platform Support](#platform-support)
+- [Install](#install)
+- [Example](#example)
+  - [Try the example with Docker](#try-the-example-with-docker)
+- [Build with Poetry](#build-with-poetry)
+- [Credits](#credits)
+- [Author](#author)
+
+<!-- vim-markdown-toc -->
+
+## Features
+
+Compared to other Myo libraries/SDKs:
+
+- Full-scratched in Python, no dependency from other runtime (e.g., the official cpp SDK)
+- Multi-platform support based on [Bleak](https://github.com/hbldh/bleak), instead of bluepy or pybluez
+- Stream EMG data (filtered/raw) and IMU data simultaneously using [asyncio](https://docs.python.org/3/library/asyncio.html)
+- A sample docker image provided -- runs just off the shelf
 
 ## Platform Support
 
 | Linux | Raspberry Pi | macOS | Windows |
 | :---: | :----------: | :---: | :-----: |
 |  ✅   |      ✅      |  ✅   |   ✅    |
 
@@ -45,39 +47,55 @@
 
 ```bash
 pip install dl-myo
 ```
 
 ## Example
 
-The script scans a Myo device, connect, set LED colors, vibrates, collect EMG/IMU data for a moment, and then read the avaialable services/characteristics from the device.
+The script scans a Myo device, connect to the device, prints the GATT profile from the device, collect EMG data for 5 seconds, and then disconnect.
 
 Any Myo Armband should have the service UUID `d5060001-a904-deb9-4748-2c7f4a124842`.
 
 ```bash
-python examples/sample.py
+python examples/sample_client.py
 ```
 
 Otherwise, you can also bind to a specific MAC address. For example,
 
 ```bash
-python examples/sample.py --mac D2:3B:85:94:32:8E
+python examples/sample_client.py --mac D2:3B:85:94:32:8E
 ```
 
 ### Try the example with Docker
 
 ```bash
 docker compose pull
 docker compose run --rm dl-myo
 ```
 
-## Build (requires [Poetry](https://python-poetry.org/)
+## Build with Poetry
+
+Install [Poetry](https://python-poetry.org/) first.
 
 ```bash
-poetry install
 poetry build
 ```
 
+## Credits
+
+This project was first inspired by [Dongleless-myo](https://github.com/iomz/Dongleless-myo) (originally created by [@mamo91](https://github.com/mamo91) and enhanced by [@MyrikLD](https://github.com/MyrikLD)) which provides a great starting point using bluepy.
+
+In addition to [Myo Bluetooth Official Protocol](https://github.com/thalmiclabs/myo-bluetooth/), I would like to mention that the following resources on GitHub have been very helpful:
+
+- https://github.com/Alvipe/Open-Myo/issues/5
+- https://github.com/NiklasRosenstein/myo-python/releases/tag/v1.0.4
+- https://github.com/PerlinWarp/Neuro-Breakout
+- https://github.com/balandinodidonato/MyoToolkit/blob/master/Software%20for%20Thalmic's%20Myo%20armband.md
+- https://github.com/cortinico/myonnaise
+- https://github.com/dzhu/myo-raw
+- https://github.com/exelban/myo-armband-nn
+- https://github.com/francocruces/MioConnect
+- https://github.com/hcilab/MyoStream
+
 ## Author
 
 [@iomz](https://github.com/iomz) (Iori Mizutani)
-
```

