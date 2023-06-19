# Comparing `tmp/obsws_python-1.4.2.tar.gz` & `tmp/obsws_python-1.5.0.tar.gz`

## Comparing `obsws_python-1.4.2.tar` & `obsws_python-1.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 obsws_python-1.4.2/obsws_python/__init__.py
--rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 obsws_python-1.4.2/obsws_python/baseclient.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 obsws_python-1.4.2/obsws_python/callback.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 obsws_python-1.4.2/obsws_python/error.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 obsws_python-1.4.2/obsws_python/events.py
--rw-r--r--   0        0        0    57933 2020-02-02 00:00:00.000000 obsws_python-1.4.2/obsws_python/reqs.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 obsws_python-1.4.2/obsws_python/subs.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 obsws_python-1.4.2/obsws_python/util.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 obsws_python-1.4.2/obsws_python/version.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 obsws_python-1.4.2/.gitignore
--rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 obsws_python-1.4.2/LICENSE
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 obsws_python-1.4.2/README.md
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 obsws_python-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 obsws_python-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 obsws_python-1.5.0/obsws_python/__init__.py
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 obsws_python-1.5.0/obsws_python/baseclient.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 obsws_python-1.5.0/obsws_python/callback.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 obsws_python-1.5.0/obsws_python/error.py
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 obsws_python-1.5.0/obsws_python/events.py
+-rw-r--r--   0        0        0    57952 2020-02-02 00:00:00.000000 obsws_python-1.5.0/obsws_python/reqs.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 obsws_python-1.5.0/obsws_python/subs.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 obsws_python-1.5.0/obsws_python/util.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 obsws_python-1.5.0/obsws_python/version.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 obsws_python-1.5.0/.gitignore
+-rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 obsws_python-1.5.0/LICENSE
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 obsws_python-1.5.0/README.md
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 obsws_python-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4702 2020-02-02 00:00:00.000000 obsws_python-1.5.0/PKG-INFO
```

### Comparing `obsws_python-1.4.2/obsws_python/baseclient.py` & `obsws_python-1.5.0/obsws_python/baseclient.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,38 +3,52 @@
 import json
 import logging
 from pathlib import Path
 from random import randint
 from typing import Optional
 
 import websocket
+from websocket import WebSocketTimeoutException
 
-from .error import OBSSDKError
+from .error import OBSSDKError, OBSSDKTimeoutError
 
 
 class ObsClient:
     logger = logging.getLogger("baseclient.obsclient")
 
     def __init__(self, **kwargs):
-        defaultkwargs = {"host": "localhost", "port": 4455, "password": "", "subs": 0}
+        defaultkwargs = {
+            "host": "localhost",
+            "port": 4455,
+            "password": "",
+            "subs": 0,
+            "timeout": None,
+        }
         if not any(key in kwargs for key in ("host", "port", "password")):
             kwargs |= self._conn_from_toml()
         kwargs = defaultkwargs | kwargs
         for attr, val in kwargs.items():
             setattr(self, attr, val)
 
         self.logger.info(
-            "Connecting with parameters: host='{host}' port={port} password='{password}' subs={subs}".format(
+            "Connecting with parameters: host='{host}' port={port} password='{password}' subs={subs} timeout={timeout}".format(
                 **self.__dict__
             )
         )
 
-        self.ws = websocket.WebSocket()
-        self.ws.connect(f"ws://{self.host}:{self.port}")
-        self.server_hello = json.loads(self.ws.recv())
+        try:
+            self.ws = websocket.WebSocket()
+            self.ws.connect(f"ws://{self.host}:{self.port}", timeout=self.timeout)
+            self.server_hello = json.loads(self.ws.recv())
+        except ValueError as e:
+            self.logger.error(f"{type(e).__name__}: {e}")
+            raise
+        except (ConnectionRefusedError, WebSocketTimeoutException) as e:
+            self.logger.exception(f"{type(e).__name__}: {e}")
+            raise
 
     def _conn_from_toml(self) -> dict:
         try:
             import tomllib
         except ModuleNotFoundError:
             import tomli as tomllib
 
@@ -101,11 +115,15 @@
         payload = {
             "op": 6,
             "d": {"requestType": req_type, "requestId": randint(1, 1000)},
         }
         if req_data:
             payload["d"]["requestData"] = req_data
         self.logger.debug(f"Sending request {payload}")
-        self.ws.send(json.dumps(payload))
-        response = json.loads(self.ws.recv())
+        try:
+            self.ws.send(json.dumps(payload))
+            response = json.loads(self.ws.recv())
+        except WebSocketTimeoutException as e:
+            self.logger.exception(f"{type(e).__name__}: {e}")
+            raise OBSSDKTimeoutError("Timeout while trying to send the request") from e
         self.logger.debug(f"Response received {response}")
         return response["d"]
```

### Comparing `obsws_python-1.4.2/obsws_python/callback.py` & `obsws_python-1.5.0/obsws_python/callback.py`

 * *Files identical despite different names*

### Comparing `obsws_python-1.4.2/obsws_python/events.py` & `obsws_python-1.5.0/obsws_python/events.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import json
 import logging
 import time
 from threading import Thread
 
+from websocket import WebSocketTimeoutException
+
 from .baseclient import ObsClient
 from .callback import Callback
+from .error import OBSSDKTimeoutError
 from .subs import Subs
 
 """
 A class to interact with obs-websocket events
 defined in official github repo
 https://github.com/obsproject/obs-websocket/blob/master/docs/generated/protocol.md#events
 """
@@ -26,15 +29,15 @@
             self.logger.info(f"Successfully identified {self} with the server")
         self.callback = Callback()
         self.subscribe()
 
     def __repr__(self):
         return type(
             self
-        ).__name__ + "(host='{host}', port={port}, password='{password}', subs={subs})".format(
+        ).__name__ + "(host='{host}', port={port}, password='{password}', subs={subs}, timeout={timeout})".format(
             **self.base_client.__dict__,
         )
 
     def __str__(self):
         return type(self).__name__
 
     def subscribe(self):
@@ -45,15 +48,19 @@
         """
         Continuously listen for events.
 
         Triggers a callback on event received.
         """
         self.running = True
         while self.running:
-            event = json.loads(self.base_client.ws.recv())
+            try:
+                event = json.loads(self.base_client.ws.recv())
+            except WebSocketTimeoutException as e:
+                self.logger.exception(f"{type(e).__name__}: {e}")
+                raise OBSSDKTimeoutError("Timeout while waiting for event") from e
             self.logger.debug(f"Event received {event}")
             type_, data = (
                 event["d"].get("eventType"),
                 event["d"].get("eventData"),
             )
             self.callback.trigger(type_, data if data else {})
             time.sleep(self.DELAY)
```

### Comparing `obsws_python-1.4.2/obsws_python/reqs.py` & `obsws_python-1.5.0/obsws_python/reqs.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         self.base_client.ws.close()
 
     def __repr__(self):
         return type(
             self
-        ).__name__ + "(host='{host}', port={port}, password='{password}')".format(
+        ).__name__ + "(host='{host}', port={port}, password='{password}', timeout={timeout})".format(
             **self.base_client.__dict__,
         )
 
     def __str__(self):
         return type(self).__name__
 
     def send(self, param, data=None, raw=False):
```

### Comparing `obsws_python-1.4.2/obsws_python/subs.py` & `obsws_python-1.5.0/obsws_python/subs.py`

 * *Files identical despite different names*

### Comparing `obsws_python-1.4.2/obsws_python/util.py` & `obsws_python-1.5.0/obsws_python/util.py`

 * *Files identical despite different names*

### Comparing `obsws_python-1.4.2/.gitignore` & `obsws_python-1.5.0/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -43,8 +43,11 @@
 ENV/
 env.bak/
 venv.bak/
 .hatch
 
 # Test/config
 quick.py
-config.toml
+config.toml
+obsws.log
+
+.vscode/
```

### Comparing `obsws_python-1.4.2/LICENSE` & `obsws_python-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `obsws_python-1.4.2/README.md` & `obsws_python-1.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 ### How to Use
 
 By default the clients connect with parameters:
 
 -   `host`: "localhost"
 -   `port`: 4455
 -   `password`: ""
+-   `timeout`: None
 
 You may override these parameters by storing them in a toml config file or passing them as keyword arguments.
 
 Order of precedence: keyword arguments then config file then default values.
 
 #### `config file`
 
@@ -49,15 +50,15 @@
 
 Example `__main__.py`:
 
 ```python
 import obsws_python as obs
 
 # pass conn info if not in config.toml
-cl = obs.ReqClient(host='localhost', port=4455, password='mystrongpass')
+cl = obs.ReqClient(host='localhost', port=4455, password='mystrongpass', timeout=3)
 
 # Toggle the mute state of your Mic input
 cl.toggle_input_mute('Mic/Aux')
 ```
 
 ### Requests
 
@@ -127,14 +128,16 @@
 
 ### Errors
 
 If a request fails an `OBSSDKError` will be raised with a status code.
 
 For a full list of status codes refer to [Codes](https://github.com/obsproject/obs-websocket/blob/master/docs/generated/protocol.md#requeststatus)
 
+If a timeout occurs during sending/receiving a request or receiving an event an `OBSSDKTimeoutError` will be raised.
+
 ### Logging
 
 If you want to see the raw messages simply set log level to DEBUG
 
 example:
 
 ```python
```

### Comparing `obsws_python-1.4.2/pyproject.toml` & `obsws_python-1.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `obsws_python-1.4.2/PKG-INFO` & `obsws_python-1.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obsws-python
-Version: 1.4.2
+Version: 1.5.0
 Summary: A Python SDK for OBS Studio WebSocket v5.0
 Project-URL: Homepage, https://github.com/aatikturk/obsws-python
 Author-email: Adem Atikturk <aatikturk@gmail.com>
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: tomli>=2.0.1; python_version < '3.11'
 Requires-Dist: websocket-client
@@ -40,14 +40,15 @@
 ### How to Use
 
 By default the clients connect with parameters:
 
 -   `host`: "localhost"
 -   `port`: 4455
 -   `password`: ""
+-   `timeout`: None
 
 You may override these parameters by storing them in a toml config file or passing them as keyword arguments.
 
 Order of precedence: keyword arguments then config file then default values.
 
 #### `config file`
 
@@ -66,15 +67,15 @@
 
 Example `__main__.py`:
 
 ```python
 import obsws_python as obs
 
 # pass conn info if not in config.toml
-cl = obs.ReqClient(host='localhost', port=4455, password='mystrongpass')
+cl = obs.ReqClient(host='localhost', port=4455, password='mystrongpass', timeout=3)
 
 # Toggle the mute state of your Mic input
 cl.toggle_input_mute('Mic/Aux')
 ```
 
 ### Requests
 
@@ -144,14 +145,16 @@
 
 ### Errors
 
 If a request fails an `OBSSDKError` will be raised with a status code.
 
 For a full list of status codes refer to [Codes](https://github.com/obsproject/obs-websocket/blob/master/docs/generated/protocol.md#requeststatus)
 
+If a timeout occurs during sending/receiving a request or receiving an event an `OBSSDKTimeoutError` will be raised.
+
 ### Logging
 
 If you want to see the raw messages simply set log level to DEBUG
 
 example:
 
 ```python
```

