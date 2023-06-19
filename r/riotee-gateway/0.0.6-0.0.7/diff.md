# Comparing `tmp/riotee_gateway-0.0.6.tar.gz` & `tmp/riotee_gateway-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riotee_gateway-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "riotee_gateway-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `riotee_gateway-0.0.6.tar` & `riotee_gateway-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1101 2023-06-15 12:39:45.638641 riotee_gateway-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0      518 2023-06-15 12:39:45.638641 riotee_gateway-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      514 2023-06-15 12:39:45.638641 riotee_gateway-0.0.6/riotee_gateway/__init__.py
--rw-r--r--   0        0        0     2904 2023-06-15 12:39:45.638641 riotee_gateway-0.0.6/riotee_gateway/cli.py
--rw-r--r--   0        0        0     2910 2023-06-15 12:39:45.638641 riotee_gateway-0.0.6/riotee_gateway/client.py
--rw-r--r--   0        0        0     3876 2023-06-15 12:39:45.642642 riotee_gateway-0.0.6/riotee_gateway/packet_model.py
--rw-r--r--   0        0        0     2547 2023-06-15 12:39:45.642642 riotee_gateway-0.0.6/riotee_gateway/server.py
--rw-r--r--   0        0        0     1827 2023-06-15 12:39:45.642642 riotee_gateway-0.0.6/riotee_gateway/transceiver.py
--rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 riotee_gateway-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-06-19 11:37:53.609424 riotee_gateway-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0      518 2023-06-19 11:37:53.609424 riotee_gateway-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      573 2023-06-19 11:37:53.609424 riotee_gateway-0.0.7/riotee_gateway/__init__.py
+-rw-r--r--   0        0        0     2904 2023-06-19 11:37:53.609424 riotee_gateway-0.0.7/riotee_gateway/cli.py
+-rw-r--r--   0        0        0     2926 2023-06-19 11:37:53.609424 riotee_gateway-0.0.7/riotee_gateway/client.py
+-rw-r--r--   0        0        0     3763 2023-06-19 11:37:53.609424 riotee_gateway-0.0.7/riotee_gateway/packet_model.py
+-rw-r--r--   0        0        0     2547 2023-06-19 11:37:53.609424 riotee_gateway-0.0.7/riotee_gateway/server.py
+-rw-r--r--   0        0        0     1856 2023-06-19 11:37:53.609424 riotee_gateway-0.0.7/riotee_gateway/transceiver.py
+-rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 riotee_gateway-0.0.7/PKG-INFO
```

### Comparing `riotee_gateway-0.0.6/LICENSE.txt` & `riotee_gateway-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `riotee_gateway-0.0.6/pyproject.toml` & `riotee_gateway-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `riotee_gateway-0.0.6/riotee_gateway/cli.py` & `riotee_gateway-0.0.7/riotee_gateway/cli.py`

 * *Files identical despite different names*

### Comparing `riotee_gateway-0.0.6/riotee_gateway/client.py` & `riotee_gateway-0.0.7/riotee_gateway/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import numpy as np
 import base64
 
 from riotee_gateway.packet_model import PacketApiSend
 
 
 def decode_dev_id(dev_id_b64: str):
-    return np.frombuffer(base64.b64decode(dev_id_b64), dtype=np.uint16)[0]
+    return np.frombuffer(base64.urlsafe_b64decode(dev_id_b64), dtype=np.uint16)[0]
 
 
 def encode_data(data):
-    return str(base64.b64encode(data), "utf-8")
+    return str(base64.urlsafe_b64encode(data), "utf-8")
 
 
 class GatewayClient(object):
     def __init__(self, host: str = "localhost", port: int = 8000):
         self.__url = f"http://{host}:{port}"
 
     def convert_dev_id(fn_called):
```

### Comparing `riotee_gateway-0.0.6/riotee_gateway/packet_model.py` & `riotee_gateway-0.0.7/riotee_gateway/packet_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             return val
 
 
 class PacketApiSend(PacketBase):
     """Packet sent to the Gateway server via API to be forwarded to a device."""
 
     @classmethod
-    def from_binary(cls, data: bytes, pkt_id: int = None):
+    def from_binary(cls, data: bytes, pkt_id: np.int16 = None):
         data_enc = base64.urlsafe_b64encode(data)
         return cls(data=data_enc, pkt_id=pkt_id)
 
 
 class PacketTransceiverSend(PacketBase):
     """Packet sent to the transceiver via USB CDC ACM."""
 
@@ -57,57 +57,55 @@
         else:
             pkt_id = pkt.pkt_id
 
         return cls(pkt_id=pkt_id, data=pkt.data, dev_id=dev_id)
 
     def to_uart(self):
         """Returns a string ready to be sent to the gateway transceiver."""
-        dev_id_bytes = base64.urlsafe_b64decode(self.dev_id)
-        dev_id_enc = str(base64.b64encode(dev_id_bytes), "utf-8")
-        pkt_id_enc = str(base64.b64encode(np.uint16(self.pkt_id)), "utf-8")
-        data_bytes = base64.urlsafe_b64decode(self.data)
-        data_enc = str(base64.b64encode(data_bytes), "utf-8")
+        dev_id_enc = str(self.dev_id, "utf-8")
+        data_enc = str(self.data, "utf-8")
+        pkt_id_enc = str(base64.urlsafe_b64encode(np.uint16(self.pkt_id)), "utf-8")
         return bytes(f"[{dev_id_enc}\0{pkt_id_enc}\0{data_enc}\0]", encoding="utf-8")
 
 
 class PacketApiReceive(PacketBase):
     """Packet received by the Gateway server from a device to be retrieved via the API."""
 
     dev_id: bytes
     pkt_id: int
     ack_id: int
     timestamp: datetime
 
     @staticmethod
-    def base64_to_bytes(pkt_str: bytes):
+    def base64_extract(pkt_str: bytes):
         """Extracts a null-terminated base64 string from pkt_str and converts it to utf-8."""
         term_idx = pkt_str.find(b"\0")
         if term_idx < 0:
             raise Exception("Could not find terminating character")
-        return base64.b64decode(pkt_str[:term_idx], validate=True), term_idx
+        return pkt_str[:term_idx], term_idx
+
+    @staticmethod
+    def base64_to_bytes(pkt_str: bytes):
+        """Extracts a null-terminated base64 string from pkt_str and converts it to utf-8."""
+        pkt_str_cut, term_idx = PacketApiReceive.base64_extract(pkt_str)
+        return base64.urlsafe_b64decode(pkt_str_cut), term_idx
 
     @staticmethod
     def base64_to_bin(pkt_str: bytes, dtype):
         """Extracts a null-terminated base64 string from pkt_str and converts it to specified type."""
         binbytes, term_idx = PacketApiReceive.base64_to_bytes(pkt_str)
         return np.frombuffer(binbytes, dtype)[0], term_idx
 
     @classmethod
     def from_uart(cls, pkt_str: str, timestamp: datetime):
         """Populates class from a pkt_str received from the gateway transceiver."""
-        # Re-encode as URL safe base64
-        dev_id, term_idx = cls.base64_to_bytes(pkt_str)
-        dev_id = base64.urlsafe_b64encode(dev_id)
+        dev_id, term_idx = cls.base64_extract(pkt_str)
         pkt_str = pkt_str[term_idx + 1 :]
 
         pkt_id, term_idx = cls.base64_to_bin(pkt_str, np.uint16)
         pkt_str = pkt_str[term_idx + 1 :]
 
         ack_id, term_idx = cls.base64_to_bin(pkt_str, np.uint16)
 
-        pkt_str = pkt_str[term_idx + 1 :]
-
-        # Re-encode as URL safe base64
-        data, _ = cls.base64_to_bytes(pkt_str)
-        data = base64.urlsafe_b64encode(data)
+        data = pkt_str[term_idx + 1 :]
 
         return cls(dev_id=dev_id, pkt_id=pkt_id, ack_id=ack_id, data=data, timestamp=timestamp)
```

### Comparing `riotee_gateway-0.0.6/riotee_gateway/server.py` & `riotee_gateway-0.0.7/riotee_gateway/server.py`

 * *Files identical despite different names*

### Comparing `riotee_gateway-0.0.6/riotee_gateway/transceiver.py` & `riotee_gateway-0.0.7/riotee_gateway/transceiver.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,9 +47,10 @@
 
     async def read_packet(self):
         await self.__reader.readuntil(b"[")
         pkt_str = await self.__reader.readuntil(b"]")
         return PacketApiReceive.from_uart(pkt_str, datetime.now())
 
     def send_packet(self, pkt: PacketTransceiverSend):
+        print(pkt.to_uart())
         self.__writer.write(pkt.to_uart())
         logging.debug(pkt.to_uart())
```

