# Comparing `tmp/msgx-1.0.1.tar.gz` & `tmp/msgx-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgx-1.0.1.tar", last modified: Fri Jun 16 15:20:00 2023, max compression
+gzip compressed data, was "msgx-1.0.2.tar", last modified: Mon Jun 19 02:22:16 2023, max compression
```

## Comparing `msgx-1.0.1.tar` & `msgx-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 soraxas   (1000) soraxas   (1000)        0 2023-06-16 15:20:00.667143 msgx-1.0.1/
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)     1102 2023-06-16 00:01:15.000000 msgx-1.0.1/LICENSE
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)       33 2023-06-16 15:14:53.000000 msgx-1.0.1/MANIFEST.in
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)     2914 2023-06-16 15:20:00.663810 msgx-1.0.1/PKG-INFO
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)     1913 2023-06-15 23:50:27.000000 msgx-1.0.1/README.md
-drwxr-xr-x   0 soraxas   (1000) soraxas   (1000)        0 2023-06-16 15:20:00.663810 msgx-1.0.1/msgx.egg-info/
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)     2914 2023-06-16 15:20:00.000000 msgx-1.0.1/msgx.egg-info/PKG-INFO
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)      322 2023-06-16 15:20:00.000000 msgx-1.0.1/msgx.egg-info/SOURCES.txt
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)        1 2023-06-16 15:20:00.000000 msgx-1.0.1/msgx.egg-info/dependency_links.txt
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)       33 2023-06-16 15:20:00.000000 msgx-1.0.1/msgx.egg-info/requires.txt
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)        5 2023-06-16 15:20:00.000000 msgx-1.0.1/msgx.egg-info/top_level.txt
-drwxr-xr-x   0 soraxas   (1000) soraxas   (1000)        0 2023-06-16 15:20:00.663810 msgx-1.0.1/python/
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)     2147 2023-06-16 11:43:26.000000 msgx-1.0.1/python/__init__.py
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)       22 2023-06-16 15:19:48.000000 msgx-1.0.1/python/_version.py
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)     1230 2023-06-16 11:41:03.000000 msgx-1.0.1/python/constants.py
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)     2934 2023-06-16 11:41:03.000000 msgx-1.0.1/python/deserialise.py
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)       82 2023-06-16 11:43:26.000000 msgx-1.0.1/python/msg_definitions.py
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)     1448 2023-06-16 15:20:00.000000 msgx-1.0.1/python/msgx.capnp
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)     1461 2023-06-16 15:20:00.000000 msgx-1.0.1/python/ndarray.capnp
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)       38 2023-06-16 15:20:00.667143 msgx-1.0.1/setup.cfg
--rw-r--r--   0 soraxas   (1000) soraxas   (1000)     2346 2023-06-16 15:17:59.000000 msgx-1.0.1/setup.py
+drwxr-xr-x   0 soraxas   (1000) soraxas   (1000)        0 2023-06-19 02:22:16.173621 msgx-1.0.2/
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)     1102 2023-06-16 00:01:15.000000 msgx-1.0.2/LICENSE
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)       33 2023-06-16 15:14:53.000000 msgx-1.0.2/MANIFEST.in
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)     2914 2023-06-19 02:22:16.173621 msgx-1.0.2/PKG-INFO
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)     1913 2023-06-15 23:50:27.000000 msgx-1.0.2/README.md
+drwxr-xr-x   0 soraxas   (1000) soraxas   (1000)        0 2023-06-19 02:22:16.173621 msgx-1.0.2/msgx.egg-info/
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)     2914 2023-06-19 02:22:16.000000 msgx-1.0.2/msgx.egg-info/PKG-INFO
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)      341 2023-06-19 02:22:16.000000 msgx-1.0.2/msgx.egg-info/SOURCES.txt
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)        1 2023-06-19 02:22:16.000000 msgx-1.0.2/msgx.egg-info/dependency_links.txt
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)       33 2023-06-19 02:22:16.000000 msgx-1.0.2/msgx.egg-info/requires.txt
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)        5 2023-06-19 02:22:16.000000 msgx-1.0.2/msgx.egg-info/top_level.txt
+drwxr-xr-x   0 soraxas   (1000) soraxas   (1000)        0 2023-06-19 02:22:16.173621 msgx-1.0.2/python/
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)       83 2023-06-17 12:29:32.000000 msgx-1.0.2/python/__init__.py
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)       22 2023-06-19 02:13:17.000000 msgx-1.0.2/python/_version.py
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)     1313 2023-06-18 12:43:05.000000 msgx-1.0.2/python/constants.py
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)     3684 2023-06-18 14:13:32.000000 msgx-1.0.2/python/deserialise.py
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)      198 2023-06-17 12:07:14.000000 msgx-1.0.2/python/msg_definitions.py
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)     1448 2023-06-19 02:22:16.000000 msgx-1.0.2/python/msgx.capnp
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)     1463 2023-06-19 02:22:16.000000 msgx-1.0.2/python/ndarray.capnp
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)     2294 2023-06-17 12:28:01.000000 msgx-1.0.2/python/reciever.py
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)       38 2023-06-19 02:22:16.173621 msgx-1.0.2/setup.cfg
+-rw-r--r--   0 soraxas   (1000) soraxas   (1000)     2346 2023-06-16 15:17:59.000000 msgx-1.0.2/setup.py
```

### Comparing `msgx-1.0.1/LICENSE` & `msgx-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `msgx-1.0.1/PKG-INFO` & `msgx-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgx
-Version: 1.0.1
+Version: 1.0.2
 Summary: Message Exchange protocol.
 Home-page: https://github.com/soraxas/msgx
 Author: Tin Lai (@soraxas)
 Author-email: oscar@tinyiu.com
 License: MIT
 Keywords: msgx deserialise c++ capnp protobuf zmq
 Classifier: Intended Audience :: Developers
```

### Comparing `msgx-1.0.1/README.md` & `msgx-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `msgx-1.0.1/msgx.egg-info/PKG-INFO` & `msgx-1.0.2/msgx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgx
-Version: 1.0.1
+Version: 1.0.2
 Summary: Message Exchange protocol.
 Home-page: https://github.com/soraxas/msgx
 Author: Tin Lai (@soraxas)
 Author-email: oscar@tinyiu.com
 License: MIT
 Keywords: msgx deserialise c++ capnp protobuf zmq
 Classifier: Intended Audience :: Developers
```

### Comparing `msgx-1.0.1/python/__init__.py` & `msgx-1.0.2/python/reciever.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import time
 import zmq
+import enum
 
-from ._version import __version__
 from . import deserialise
 
 
-MSGX_ADDRESS = "tcp://127.0.0.1:5558"
-MSGX_MODE_DEFAULT = "default"
-MSGX_MODE_ASYNC = "async"
+class MsgXReceiverMode(enum.Enum):
+    Synchronised = enum.auto()
+    Asynchronous = enum.auto()
 
 
 class MsgXReceiver:
     """A class that listen to message from cpp"""
 
-    def __init__(self, address=MSGX_ADDRESS, ctx_mgr=None):
+    def __init__(
+        self, address=None, *, protocol="tcp", ip_address="127.0.0.1", port=5558
+    ):
+        if address is None:
+            address = f"{protocol}://{ip_address}:{port}"
         self.address = address
         self.socket = None
         self.mode = None
 
     # noinspection PyUnresolvedReferences
-    def initialise(self, sleep=1, mode=MSGX_MODE_DEFAULT):
+    def initialise(self, mode, sleep=1):
         if self.mode == mode:
             return
-        if mode == MSGX_MODE_ASYNC:
+        if mode == MsgXReceiverMode.Asynchronous:
             context = zmq.asyncio.Context()
-        elif mode == MSGX_MODE_DEFAULT:
+        elif mode == MsgXReceiverMode.Synchronised:
             context = zmq.Context()
         else:
             raise ValueError("Unknown mode {}".format(mode))
         self.mode = mode
         socket = context.socket(zmq.SUB)
         socket.connect(self.address)
         socket.setsockopt_string(zmq.SUBSCRIBE, "")
@@ -37,24 +41,24 @@
 
     @staticmethod
     def _get_msg(encoded_msg):
         return deserialise.decode_message(encoded_msg)
 
     def get_msg_func(self, flags=0):
         """Return a function that process the incoming encoded msg"""
-        self.initialise(mode=MSGX_MODE_DEFAULT)
+        self.initialise(mode=MsgXReceiverMode.Synchronised)
         encoded_msg = self.socket.recv(flags=flags)
         return lambda: self._get_msg(encoded_msg)
 
     def get_msg(self, flags=0):
         return self.get_msg_func(flags)()
 
     async def get_msg_async_func(self):
         """Return a function that process the incoming encoded msg, async-ly"""
-        self.initialise(mode=MSGX_MODE_ASYNC)
+        self.initialise(mode=MsgXReceiverMode.Asynchronous)
         encoded_msg = await self.socket.recv()
         return lambda: self._get_msg(encoded_msg)
 
     async def get_msg_async(self):
         return (await self.get_msg_async_func())()
```

### Comparing `msgx-1.0.1/python/constants.py` & `msgx-1.0.2/python/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import numpy as np
 
 from . import msg_definitions
 
 Endianness = msg_definitions.ndarray_capnp.Endianness
 DataType = msg_definitions.ndarray_capnp.DataType
 
+# enum endian-ness type
 ENDIANNESS_MAPPING = {
+    Endianness.unspecified: None,
     Endianness.littleEndianOrder: "little",
     Endianness.bigEndianOrder: "big",
     Endianness.middleEndianOrder: None,
 }
 
+# enum ndarray data type
 DATATYPE_MAPPING = {
     DataType.bool8: np.bool8,  # bool
     # signed
     DataType.int8: np.int8,  # char
     DataType.int16: np.int16,  # short
     DataType.int32: np.int32,  # int
     DataType.int64: np.int64,  # long
```

### Comparing `msgx-1.0.1/python/msgx.capnp` & `msgx-1.0.2/python/msgx.capnp`

 * *Files identical despite different names*

### Comparing `msgx-1.0.1/python/ndarray.capnp` & `msgx-1.0.2/python/ndarray.capnp`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     cFloat256              @18;  # cLongDouble
 }
 
 struct NdArray {
     buffer                 @0: Data;
 
     union {
-        oneDimensional     @1: Void;
+        oneDimensional     @1: UInt32;
         multiDimensional :group {
             columnMajor    @2: Bool;
             shape          @3: List(UInt32);
         }
     }
 
     dtype                  @4: DataType;
```

### Comparing `msgx-1.0.1/setup.py` & `msgx-1.0.2/setup.py`

 * *Files identical despite different names*

