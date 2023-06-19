# Comparing `tmp/pyln_grpc_proto-0.1.0.tar.gz` & `tmp/pyln_grpc_proto-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyln_grpc_proto-0.1.0.tar", max compression
+gzip compressed data, was "pyln_grpc_proto-0.1.1.tar", max compression
```

## Comparing `pyln_grpc_proto-0.1.0.tar` & `pyln_grpc_proto-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      228 2023-06-19 16:35:27.846317 pyln_grpc_proto-0.1.0/README.md
--rw-r--r--   0        0        0    99911 2023-06-19 16:52:30.080318 pyln_grpc_proto-0.1.0/pyln/grpc/node_pb2.py
--rw-r--r--   0        0        0    82309 2023-06-19 16:52:30.080318 pyln_grpc_proto-0.1.0/pyln/grpc/node_pb2_grpc.py
--rw-r--r--   0        0        0     4685 2023-06-19 16:52:30.068318 pyln_grpc_proto-0.1.0/pyln/grpc/primitives_pb2.py
--rw-r--r--   0        0        0      159 2023-06-19 16:47:01.133051 pyln_grpc_proto-0.1.0/pyln/grpc/primitives_pb2_grpc.py
--rw-r--r--   0        0        0      459 2023-06-19 16:56:37.758769 pyln_grpc_proto-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 pyln_grpc_proto-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      228 2023-06-19 16:35:27.846317 pyln_grpc_proto-0.1.1/README.md
+-rw-r--r--   0        0        0      110 2023-06-19 17:12:22.176058 pyln_grpc_proto-0.1.1/pyln/grpc/__init__.py
+-rw-r--r--   0        0        0    99911 2023-06-19 16:52:30.080318 pyln_grpc_proto-0.1.1/pyln/grpc/node_pb2.py
+-rw-r--r--   0        0        0    82309 2023-06-19 16:52:30.080318 pyln_grpc_proto-0.1.1/pyln/grpc/node_pb2_grpc.py
+-rw-r--r--   0        0        0     4685 2023-06-19 16:52:30.068318 pyln_grpc_proto-0.1.1/pyln/grpc/primitives_pb2.py
+-rw-r--r--   0        0        0      159 2023-06-19 16:47:01.133051 pyln_grpc_proto-0.1.1/pyln/grpc/primitives_pb2_grpc.py
+-rw-r--r--   0        0        0      476 2023-06-19 17:55:53.404211 pyln_grpc_proto-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 pyln_grpc_proto-0.1.1/PKG-INFO
```

### Comparing `pyln_grpc_proto-0.1.0/pyln/grpc/node_pb2.py` & `pyln_grpc_proto-0.1.1/pyln/grpc/node_pb2.py`

 * *Files identical despite different names*

### Comparing `pyln_grpc_proto-0.1.0/pyln/grpc/node_pb2_grpc.py` & `pyln_grpc_proto-0.1.1/pyln/grpc/node_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pyln_grpc_proto-0.1.0/pyln/grpc/primitives_pb2.py` & `pyln_grpc_proto-0.1.1/pyln/grpc/primitives_pb2.py`

 * *Files identical despite different names*

### Comparing `pyln_grpc_proto-0.1.0/PKG-INFO` & `pyln_grpc_proto-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyln-grpc-proto
-Version: 0.1.0
+Version: 0.1.1
 Summary: The compiled GRPC proto for CLN
 License: MIT
 Author: Christian Decker
 Author-email: decker@blockstream.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

