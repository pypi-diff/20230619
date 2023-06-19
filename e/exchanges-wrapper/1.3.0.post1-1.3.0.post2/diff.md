# Comparing `tmp/exchanges-wrapper-1.3.0.post1.tar.gz` & `tmp/exchanges-wrapper-1.3.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchanges-wrapper-1.3.0.post1.tar", last modified: Sat Jun  3 20:49:19 2023, max compression
+gzip compressed data, was "exchanges-wrapper-1.3.0.post2.tar", last modified: Mon Jun 19 18:52:52 2023, max compression
```

## Comparing `exchanges-wrapper-1.3.0.post1.tar` & `exchanges-wrapper-1.3.0.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      165 2022-06-06 16:51:29.613842 exchanges-wrapper-1.3.0.post1/.deepsource.toml
--rw-r--r--   0        0        0       78 2022-09-23 15:45:46.921324 exchanges-wrapper-1.3.0.post1/.dockerignore
--rw-r--r--   0        0        0       71 2022-06-07 10:33:14.780369 exchanges-wrapper-1.3.0.post1/.github/FUNDING.yml
--rw-r--r--   0        0        0      502 2022-09-23 19:36:49.587213 exchanges-wrapper-1.3.0.post1/.github/dependabot.yml
--rwxr-xr-x   0        0        0     5996 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0.post1/CHANGELOG.md
--rw-r--r--   0        0        0      641 2022-09-23 17:33:34.192514 exchanges-wrapper-1.3.0.post1/Dockerfile
--rw-r--r--   0        0        0     1114 2022-05-29 08:10:10.422624 exchanges-wrapper-1.3.0.post1/LICENSE.md
--rw-r--r--   0        0        0     6698 2023-02-22 15:25:52.460883 exchanges-wrapper-1.3.0.post1/README.md
--rw-r--r--   0        0        0    15398 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0.post1/example/exch_client.py
--rwxr-xr-x   0        0        0      159 2023-02-22 15:25:52.460883 exchanges-wrapper-1.3.0.post1/example/ms_cfg.toml
--rw-r--r--   0        0        0     1289 2023-06-03 20:48:25.969282 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/__init__.py
--rw-r--r--   0        0        0    45215 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/api_pb2.py
--rw-r--r--   0        0        0    44445 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/api_pb2_grpc.py
--rw-r--r--   0        0        0    19618 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/bitfinex_parser.py
--rw-r--r--   0        0        0     6048 2023-04-01 15:08:34.303021 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/c_structures.py
--rw-r--r--   0        0        0    61936 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/client.py
--rw-r--r--   0        0        0     2601 2023-02-04 15:12:03.490966 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/definitions.py
--rw-r--r--   0        0        0      796 2023-02-04 15:12:03.490966 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/errors.py
--rw-r--r--   0        0        0    12494 2023-02-24 16:57:17.581054 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/events.py
--rwxr-xr-x   0        0        0    43798 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/exch_srv.py
--rw-r--r--   0        0        0     4189 2023-02-22 15:25:52.464921 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/exch_srv_cfg.toml.template
--rw-r--r--   0        0        0    10270 2023-05-23 10:25:45.286853 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/http_client.py
--rw-r--r--   0        0        0    15723 2023-02-04 15:12:03.494948 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/huobi_parser.py
--rw-r--r--   0        0        0    16098 2023-03-02 12:37:56.947270 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/okx_parser.py
--rw-r--r--   0        0        0    12097 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/proto/exchanges_wrapper/api.proto
--rw-r--r--   0        0        0    22294 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/web_sockets.py
--rw-r--r--   0        0        0      986 2023-06-03 20:48:25.969282 exchanges-wrapper-1.3.0.post1/pyproject.toml
--rw-r--r--   0        0        0      105 2023-06-03 20:46:47.277312 exchanges-wrapper-1.3.0.post1/requirements.txt
--rw-r--r--   0        0        0     7583 1970-01-01 00:00:00.000000 exchanges-wrapper-1.3.0.post1/PKG-INFO
+-rw-r--r--   0        0        0      165 2022-06-06 16:51:29.613842 exchanges-wrapper-1.3.0.post2/.deepsource.toml
+-rw-r--r--   0        0        0       78 2022-09-23 15:45:46.921324 exchanges-wrapper-1.3.0.post2/.dockerignore
+-rw-r--r--   0        0        0       71 2022-06-07 10:33:14.780369 exchanges-wrapper-1.3.0.post2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      502 2022-09-23 19:36:49.587213 exchanges-wrapper-1.3.0.post2/.github/dependabot.yml
+-rwxr-xr-x   0        0        0     6058 2023-06-19 18:46:26.434468 exchanges-wrapper-1.3.0.post2/CHANGELOG.md
+-rw-r--r--   0        0        0      641 2022-09-23 17:33:34.192514 exchanges-wrapper-1.3.0.post2/Dockerfile
+-rw-r--r--   0        0        0     1114 2022-05-29 08:10:10.422624 exchanges-wrapper-1.3.0.post2/LICENSE.md
+-rw-r--r--   0        0        0     6698 2023-02-22 15:25:52.460883 exchanges-wrapper-1.3.0.post2/README.md
+-rw-r--r--   0        0        0    15398 2023-06-19 18:46:17.287114 exchanges-wrapper-1.3.0.post2/example/exch_client.py
+-rwxr-xr-x   0        0        0      159 2023-02-22 15:25:52.460883 exchanges-wrapper-1.3.0.post2/example/ms_cfg.toml
+-rw-r--r--   0        0        0     1289 2023-06-19 18:46:26.434468 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/__init__.py
+-rw-r--r--   0        0        0    45215 2023-06-19 18:46:17.287114 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/api_pb2.py
+-rw-r--r--   0        0        0    44445 2023-06-19 18:46:17.287114 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/api_pb2_grpc.py
+-rw-r--r--   0        0        0    19618 2023-06-19 18:46:17.287114 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/bitfinex_parser.py
+-rw-r--r--   0        0        0     6048 2023-06-13 17:51:56.390756 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/c_structures.py
+-rw-r--r--   0        0        0    61936 2023-06-19 18:46:17.287114 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/client.py
+-rw-r--r--   0        0        0     2601 2023-06-14 12:41:55.572680 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/definitions.py
+-rw-r--r--   0        0        0      796 2023-06-14 12:41:55.572680 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/errors.py
+-rw-r--r--   0        0        0    12494 2023-06-14 12:41:55.572680 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/events.py
+-rwxr-xr-x   0        0        0    43798 2023-06-19 18:46:26.434468 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/exch_srv.py
+-rw-r--r--   0        0        0     4189 2023-02-22 15:25:52.464921 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/exch_srv_cfg.toml.template
+-rw-r--r--   0        0        0    10270 2023-06-19 18:46:17.287114 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/http_client.py
+-rw-r--r--   0        0        0    15723 2023-02-04 15:12:03.494948 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/huobi_parser.py
+-rw-r--r--   0        0        0    16098 2023-03-02 12:37:56.947270 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/okx_parser.py
+-rw-r--r--   0        0        0    12097 2023-06-19 18:46:17.287114 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/proto/exchanges_wrapper/api.proto
+-rw-r--r--   0        0        0    22384 2023-06-19 18:46:26.434468 exchanges-wrapper-1.3.0.post2/exchanges_wrapper/web_sockets.py
+-rw-r--r--   0        0        0      986 2023-06-19 18:46:17.291107 exchanges-wrapper-1.3.0.post2/pyproject.toml
+-rw-r--r--   0        0        0      105 2023-06-19 18:46:17.291107 exchanges-wrapper-1.3.0.post2/requirements.txt
+-rw-r--r--   0        0        0     7583 1970-01-01 00:00:00.000000 exchanges-wrapper-1.3.0.post2/PKG-INFO
```

### Comparing `exchanges-wrapper-1.3.0.post1/CHANGELOG.md` & `exchanges-wrapper-1.3.0.post2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## v1.3.0-2 - 2023-06-19
+### Update
+* Binance: keepalive WSS
+
 ## v1.3.0 - 2023-06-01
 ### Fix
 * exchanges_wrapper.client.Client.cancel_all_orders() set correct 'status' for cancelled orders
 
 ### Update
 * protobuf format for CancelAllOrders() and OnOrderUpdate(). Now simple use ```result = eval(json.loads(res.result))```
 for unpack incoming message. **Not compatible with earlier versions**
```

### Comparing `exchanges-wrapper-1.3.0.post1/Dockerfile` & `exchanges-wrapper-1.3.0.post2/Dockerfile`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post1/LICENSE.md` & `exchanges-wrapper-1.3.0.post2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post1/README.md` & `exchanges-wrapper-1.3.0.post2/README.md`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post1/example/exch_client.py` & `exchanges-wrapper-1.3.0.post2/example/exch_client.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/__init__.py` & `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 __authors__ = ["Th0rgal", "Jerry Fedorenko"]
 __license__ = "MIT"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 __email__ = "jerry.fedorenko@yahoo.com"
 __credits__ = ["https://github.com/DanyaSWorlD"]
-__version__ = "1.3.0-1"
+__version__ = "1.3.0-2"
 
 from pathlib import Path
 import shutil
 #
 import platform
 print(f"Python {platform.python_version()}")
 #
```

### Comparing `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/api_pb2.py` & `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/api_pb2.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/api_pb2_grpc.py` & `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/bitfinex_parser.py` & `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/bitfinex_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/c_structures.py` & `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/c_structures.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/client.py` & `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/definitions.py` & `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/definitions.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/errors.py` & `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/errors.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/events.py` & `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/events.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/exch_srv.py` & `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/exch_srv.py`

 * *Files 0% similar despite different names*

```diff
@@ -789,15 +789,15 @@
 
     async def CheckStream(self, request: api_pb2.MarketRequest,
                           _context: grpc.aio.ServicerContext) -> api_pb2.SimpleResponse:
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
         response = api_pb2.SimpleResponse()
         response.success = bool(client.data_streams.get(request.trade_id))
-        logger.debug(f"CheckStream request for {request.symbol} on {client.exchange} passed: {response.success}")
+        logger.debug(f"CheckStream request passed: {response.success} for {request.symbol} on {client.exchange}")
         return response
 
 
 async def stop_stream(client, trade_id):
     await client.stop_events_listener(trade_id)
     client.events.unregister(client.exchange, trade_id)
     [await _queue.put(trade_id) for _queue in client.stream_queue.get(trade_id, [])]
```

### Comparing `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/exch_srv_cfg.toml.template` & `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/exch_srv_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/http_client.py` & `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/http_client.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/huobi_parser.py` & `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/huobi_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/okx_parser.py` & `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/okx_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/proto/exchanges_wrapper/api.proto` & `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/proto/exchanges_wrapper/api.proto`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/web_sockets.py` & `exchanges-wrapper-1.3.0.post2/exchanges_wrapper/web_sockets.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,16 @@
         self.candles_max_time = None
 
     async def start_wss(self):
         logger.info(f"Start market WSS {self.channel if self.channel else ''} for {self.exchange}")
         registered_streams = self.client.events.registered_streams.get(self.exchange, {}).get(self.trade_id, set())
         if self.exchange == 'binance':
             combined_streams = "/".join(registered_streams)
-            self.web_socket = await self.session.ws_connect(f"{self.endpoint}/stream?streams={combined_streams}")
+            self.web_socket = await self.session.ws_connect(url=f"{self.endpoint}/stream?streams={combined_streams}",
+                                                            receive_timeout=100)
             logger.info(f"Combined events stream started: {combined_streams}")
             await self._handle_messages(self.web_socket)
         else:
             symbol = self.channel.split('@')[0]
             ch_type = self.channel.split('@')[1]
             request = {}
             if self.exchange == 'okx':
@@ -438,15 +439,15 @@
         # https://github.com/binance-exchange/binance-official-api-docs/blob/master/user-data-stream.md#pingkeep-alive-a-listenkey
         while True:
             await asyncio.sleep(interval)
             await self.client.keep_alive_listen_key(listen_key)
 
     async def start_wss(self):
         listen_key = (await self.client.create_listen_key())["listenKey"]
-        self.web_socket = await self.session.ws_connect(f"{self.endpoint}/ws/{listen_key}", heartbeat=15)
+        self.web_socket = await self.session.ws_connect(url=f"{self.endpoint}/ws/{listen_key}", heartbeat=500)
         _task = asyncio.ensure_future(self._heartbeat(listen_key))
         try:
             await self._handle_messages(self.web_socket)
         finally:
             _task.cancel()
 
     async def _handle_event(self, content):
```

### Comparing `exchanges-wrapper-1.3.0.post1/pyproject.toml` & `exchanges-wrapper-1.3.0.post2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0.post1/PKG-INFO` & `exchanges-wrapper-1.3.0.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchanges-wrapper
-Version: 1.3.0.post1
+Version: 1.3.0.post2
 Summary: REST API and WebSocket asyncio wrapper with grpc powered multiplexer server
 Author-email: Thomas Marchand <thomas.marchand@tuta.io>, Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: exchanges-wrapper Version: 1.3.0.post1 Summary:
+Metadata-Version: 2.1 Name: exchanges-wrapper Version: 1.3.0.post2 Summary:
 REST API and WebSocket asyncio wrapper with grpc powered multiplexer server
 Author-email: Thomas Marchand
 marchand@tuta.io>, Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
```

