# Comparing `tmp/py2n-0.3.1.tar.gz` & `tmp/py2n-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2n-0.3.1.tar", last modified: Wed Apr 19 15:32:35 2023, max compression
+gzip compressed data, was "py2n-0.3.2.tar", last modified: Mon Jun 19 17:13:21 2023, max compression
```

## Comparing `py2n-0.3.1.tar` & `py2n-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 15:32:35.263144 py2n-0.3.1/
--rw-rw-rw-   0        0        0     1092 2022-12-30 17:18:23.000000 py2n-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     1637 2023-04-19 15:32:35.263144 py2n-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-01-02 15:22:07.000000 py2n-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 15:32:35.240105 py2n-0.3.1/py2n/
--rw-rw-rw-   0        0        0     4671 2023-04-19 15:29:05.000000 py2n-0.3.1/py2n/__init__.py
--rw-rw-rw-   0        0        0      337 2023-01-02 14:07:45.000000 py2n-0.3.1/py2n/const.py
--rw-rw-rw-   0        0        0     1221 2023-01-02 14:07:46.000000 py2n-0.3.1/py2n/exceptions.py
--rw-rw-rw-   0        0        0     1127 2023-01-02 14:07:46.000000 py2n-0.3.1/py2n/model.py
--rw-rw-rw-   0        0        0     4478 2023-01-02 15:20:42.000000 py2n-0.3.1/py2n/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-19 15:32:35.261126 py2n-0.3.1/py2n.egg-info/
--rw-rw-rw-   0        0        0     1637 2023-04-19 15:32:34.000000 py2n-0.3.1/py2n.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-04-19 15:32:35.000000 py2n-0.3.1/py2n.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 15:32:34.000000 py2n-0.3.1/py2n.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 15:32:34.000000 py2n-0.3.1/py2n.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-19 15:32:34.000000 py2n-0.3.1/py2n.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-12-30 20:45:24.000000 py2n-0.3.1/py2n.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-04-19 15:32:35.263144 py2n-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1069 2023-04-19 15:30:41.000000 py2n-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:13:21.132718 py2n-0.3.2/
+-rw-rw-rw-   0        0        0     1092 2022-12-30 17:18:23.000000 py2n-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     1631 2023-06-19 17:13:21.131213 py2n-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      945 2023-06-19 17:12:49.000000 py2n-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 17:13:21.109142 py2n-0.3.2/py2n/
+-rw-rw-rw-   0        0        0     5272 2023-06-19 17:12:49.000000 py2n-0.3.2/py2n/__init__.py
+-rw-rw-rw-   0        0        0      375 2023-06-19 17:12:49.000000 py2n-0.3.2/py2n/const.py
+-rw-rw-rw-   0        0        0     1221 2023-01-02 14:07:46.000000 py2n-0.3.2/py2n/exceptions.py
+-rw-rw-rw-   0        0        0     1220 2023-06-19 17:12:49.000000 py2n-0.3.2/py2n/model.py
+-rw-rw-rw-   0        0        0     5017 2023-06-19 17:12:49.000000 py2n-0.3.2/py2n/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:13:21.130211 py2n-0.3.2/py2n.egg-info/
+-rw-rw-rw-   0        0        0     1631 2023-06-19 17:13:20.000000 py2n-0.3.2/py2n.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-06-19 17:13:20.000000 py2n-0.3.2/py2n.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 17:13:20.000000 py2n-0.3.2/py2n.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-19 17:13:20.000000 py2n-0.3.2/py2n.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-19 17:13:20.000000 py2n-0.3.2/py2n.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-12-30 20:45:24.000000 py2n-0.3.2/py2n.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-06-19 17:13:21.132718 py2n-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1069 2023-06-19 17:12:49.000000 py2n-0.3.2/setup.py
```

### Comparing `py2n-0.3.1/LICENSE` & `py2n-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py2n-0.3.1/PKG-INFO` & `py2n-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2n
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python library for 2N® devices
 Home-page: https://github.com/elektr0nisch/py2n
 Author: Linus Groschke
 Author-email: linus@elektronisch.dev
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
@@ -51,15 +51,15 @@
 
 
 async def run(websession):
     """Use library."""
     device = await Py2NDevice.create(
         websession,
         Py2NConnectionData(
-            ip_address="192.168.1.69",
+            host="192.168.1.69",
             username="username",
             password="password",
         ),
     )
 
     await device.restart()
```

### Comparing `py2n-0.3.1/README.md` & `py2n-0.3.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 async def run(websession):
     """Use library."""
     device = await Py2NDevice.create(
         websession,
         Py2NConnectionData(
-            ip_address="192.168.1.69",
+            host="192.168.1.69",
             username="username",
             password="password",
         ),
     )
 
     await device.restart()
```

### Comparing `py2n-0.3.1/py2n/__init__.py` & `py2n-0.3.2/py2n/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from typing import Any, List
 from datetime import datetime, timedelta, timezone
 
 from .model import Py2NDeviceData, Py2NDeviceSwitch, Py2NConnectionData
 
 from .exceptions import NotInitialized, Py2NError
 
-from .utils import get_info, get_status, restart, test_audio, get_switches, set_switch
+from .utils import get_info, get_status, restart, test_audio, get_switches, get_switch_caps , set_switch
 
 
 class Py2NDevice:
-    def __init__(self, aiohttp_session, options: Py2NConnectionData):
+    def __init__(self, aiohttp_session: aiohttp.ClientSession, options: Py2NConnectionData):
         """Device init."""
-        self.aiohttp_session: aiohttp.ClientSession = aiohttp_session
+        self.aiohttp_session = aiohttp_session
         self.options = options
         self.initialized: bool = False
 
         self._initializing: bool = False
         self._last_error: Py2NError | None = None
 
     @classmethod
@@ -51,21 +51,31 @@
         """Update device data."""
         try:
             info: dict[str, Any] = await get_info(self.aiohttp_session, self.options)
             status: dict[str, Any] = await get_status(
                 self.aiohttp_session, self.options
             )
             switches: List[Any] = await get_switches(self.aiohttp_session, self.options)
+            switch_caps: List[Any] = await get_switch_caps(self.aiohttp_session, self.options)
 
             pySwitches = []
 
             for switch in switches:
+                for caps in switch_caps:
+                    if caps["switch"] == switch["switch"]:
+                        enabled = caps["enabled"]
+                        mode = caps["mode"] if enabled else None
+                        break
                 pySwitches.append(
                     Py2NDeviceSwitch(
-                        switch["switch"], switch["active"], switch["locked"]
+                        id= switch["switch"],
+                        enabled= enabled,
+                        active= switch["active"],
+                        locked=switch["locked"],
+                        mode=mode,
                     )
                 )
 
             self._data = Py2NDeviceData(
                 name=info["deviceName"],
                 model=info["variant"],
                 serial=info["serialNumber"],
@@ -98,43 +108,45 @@
 
         try:
             await test_audio(self.aiohttp_session, self.options)
         except Py2NError as err:
             self._last_error = err
             raise
 
-    async def set_switch(self, switch_id, on) -> None:
+    async def set_switch(self, switch_id: int, on) -> None:
         """Set switch status."""
         if not self.initialized:
             raise NotInitialized
 
-        if not self._data.switches:
-            raise Py2NError("no switches configured")
-
-        if switch_id < 1 | switch_id > len(self._data.switches):
-            raise Py2NError("invalid switch id")
+        switch = self._find_switch(switch_id)
+        if not switch.enabled:
+            raise Py2NError("switch disabled")
 
         try:
             await set_switch(self.aiohttp_session, self.options, switch_id, on)
         except Py2NError as err:
             self._last_error = err
             raise
 
-    def get_switch(self, switch_id) -> bool:
+    def get_switch(self, switch_id: int) -> bool:
         """Get switch status."""
         if not self.initialized:
             raise NotInitialized
 
-        if not self._data.switches:
-            raise Py2NError("no switches configured")
+        switch = self._find_switch(switch_id)
+        return switch.active
 
-        if switch_id < 1 or switch_id > len(self._data.switches):
-            raise Py2NError("invalid switch id")
+    def _find_switch(self, switch_id: int) -> Py2NDeviceSwitch:
+        if not self._data.switches or len(self._data.switches) == 0:
+            raise Py2NError("no switches configured")
 
-        return self._data.switches[switch_id - 1].active
+        for switch in self._data.switches:
+            if switch.id == switch_id:
+                return switch
+        raise Py2NError("invalid switch id")
 
     async def close(self) -> None:
         """Close http session."""
         if not self.initialized:
             raise NotInitialized
 
         await self.aiohttp_session.close()
```

### Comparing `py2n-0.3.1/py2n/exceptions.py` & `py2n-0.3.2/py2n/exceptions.py`

 * *Files identical despite different names*

### Comparing `py2n-0.3.1/py2n/model.py` & `py2n-0.3.2/py2n/model.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,16 +28,18 @@
 
 
 @dataclass
 class Py2NDeviceSwitch:
     """Representation of 2N device switch."""
 
     id: int
+    enabled: bool
     active: bool
     locked: bool
+    mode: str | None #inactive switches do not return a value for "mode"
 
 
 @dataclass
 class Py2NDeviceData:
     """Data collected from a 2N device."""
 
     name: str
```

### Comparing `py2n-0.3.1/py2n/utils.py` & `py2n-0.3.2/py2n/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from .const import (
     HTTP_CALL_TIMEOUT,
     CONTENT_TYPE,
     API_SYSTEM_INFO,
     API_SYSTEM_STATUS,
     API_SYSTEM_RESTART,
+    API_SWITCH_CAPS,
     API_SWITCH_STATUS,
     API_SWITCH_CONTROL,
     API_AUDIO_TEST,
 )
 
 from .model import Py2NConnectionData
 
@@ -92,14 +93,30 @@
         )
     except DeviceApiError as err:
         # some devices don't offer switches
         if err.error == ApiError.NOT_SUPPORTED:
             return []
         raise
 
+    return result["switches"]
+
+async def get_switch_caps(
+    aiohttp_session: aiohttp.ClientSession, options: Py2NConnectionData
+) -> List[Any]:
+    """Get switch caps from device through REST call."""
+    try:
+        result = await api_request(
+            aiohttp_session, options, f"http://{options.host}{API_SWITCH_CAPS}"
+        )
+    except DeviceApiError as err:
+        # some devices don't offer switches
+        if err.error == ApiError.NOT_SUPPORTED:
+            return []
+        raise
+
     return result["switches"]
 
 
 async def set_switch(
     aiohttp_session: aiohttp.ClientSession,
     options: Py2NConnectionData,
     switch_id: int,
```

### Comparing `py2n-0.3.1/py2n.egg-info/PKG-INFO` & `py2n-0.3.2/py2n.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2n
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python library for 2N® devices
 Home-page: https://github.com/elektr0nisch/py2n
 Author: Linus Groschke
 Author-email: linus@elektronisch.dev
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
@@ -51,15 +51,15 @@
 
 
 async def run(websession):
     """Use library."""
     device = await Py2NDevice.create(
         websession,
         Py2NConnectionData(
-            ip_address="192.168.1.69",
+            host="192.168.1.69",
             username="username",
             password="password",
         ),
     )
 
     await device.restart()
```

### Comparing `py2n-0.3.1/setup.py` & `py2n-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setup module for py2n."""
 from pathlib import Path
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "0.3.1"
+VERSION = "0.3.2"
 
 setup(
     name='py2n',
     version=VERSION,
     license="MIT",
     url="https://github.com/elektr0nisch/py2n",
     author="Linus Groschke",
```

