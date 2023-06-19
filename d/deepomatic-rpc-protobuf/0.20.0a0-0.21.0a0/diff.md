# Comparing `tmp/deepomatic-rpc-protobuf-0.20.0a0.tar.gz` & `tmp/deepomatic-rpc-protobuf-0.21.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepomatic-rpc-protobuf-0.20.0a0.tar", last modified: Mon Jun 19 12:51:41 2023, max compression
+gzip compressed data, was "deepomatic-rpc-protobuf-0.21.0a0.tar", last modified: Fri Jun 16 07:58:10 2023, max compression
```

## Comparing `deepomatic-rpc-protobuf-0.20.0a0.tar` & `deepomatic-rpc-protobuf-0.21.0a0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-19 12:51:41.838881 deepomatic-rpc-protobuf-0.20.0a0/
--rw-rw-r--   0 dude      (1000) dude      (1000)       44 2023-06-12 10:38:48.000000 deepomatic-rpc-protobuf-0.20.0a0/LICENCE
--rw-r--r--   0 dude      (1000) dude      (1000)     9869 2023-06-19 12:51:41.838881 deepomatic-rpc-protobuf-0.20.0a0/PKG-INFO
--rw-rw-r--   0 dude      (1000) dude      (1000)     9353 2023-06-15 10:08:49.000000 deepomatic-rpc-protobuf-0.20.0a0/README.md
--rw-rw-r--   0 dude      (1000) dude      (1000)      675 2023-06-19 09:31:56.000000 deepomatic-rpc-protobuf-0.20.0a0/pyproject.toml
--rw-r--r--   0 dude      (1000) dude      (1000)       38 2023-06-19 12:51:41.838881 deepomatic-rpc-protobuf-0.20.0a0/setup.cfg
-drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-19 12:51:41.830881 deepomatic-rpc-protobuf-0.20.0a0/src/
-drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-19 12:51:41.830881 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/
-drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-19 12:51:41.830881 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/
-drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-19 12:51:41.834881 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/
--rw-r--r--   0 dude      (1000) dude      (1000)        0 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/__init__.py
-drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-19 12:51:41.834881 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/
--rw-r--r--   0 dude      (1000) dude      (1000)        0 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/__init__.py
-drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-19 12:51:41.834881 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/cli/
--r-xr-xr-x   0 dude      (1000) dude      (1000)     1672 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/cli/Message_pb2.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/cli/Message_pb2_grpc.py
--rw-r--r--   0 dude      (1000) dude      (1000)        0 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/cli/__init__.py
-drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-19 12:51:41.834881 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/common/
--r-xr-xr-x   0 dude      (1000) dude      (1000)     1101 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/common/Error_pb2.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/common/Error_pb2_grpc.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)     1419 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/common/Image_pb2.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/common/Image_pb2_grpc.py
--rw-r--r--   0 dude      (1000) dude      (1000)        0 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/common/__init__.py
-drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-19 12:51:41.834881 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/
--r-xr-xr-x   0 dude      (1000) dude      (1000)     2639 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Command_pb2.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Command_pb2_grpc.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)     1439 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Message_pb2.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Message_pb2_grpc.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)     7611 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Postprocessing_pb2.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Postprocessing_pb2_grpc.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)     4018 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Preprocessing_pb2.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Preprocessing_pb2_grpc.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)     1583 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Result_pb2.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Result_pb2_grpc.py
--rw-r--r--   0 dude      (1000) dude      (1000)        0 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/__init__.py
-drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-19 12:51:41.834881 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/frameworks/
--r-xr-xr-x   0 dude      (1000) dude      (1000)     2303 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/frameworks/Caffe_pb2.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/frameworks/Caffe_pb2_grpc.py
--rw-r--r--   0 dude      (1000) dude      (1000)        0 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/frameworks/__init__.py
-drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-19 12:51:41.838881 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/
--r-xr-xr-x   0 dude      (1000) dude      (1000)     1312 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Commands_pb2.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Commands_pb2_grpc.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)     1784 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Inputs_pb2.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Inputs_pb2_grpc.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)     3502 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Results_pb2.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Results_pb2_grpc.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)     2441 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Workflows_pb2.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Workflows_pb2_grpc.py
--rw-r--r--   0 dude      (1000) dude      (1000)        0 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/__init__.py
-drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-19 12:51:41.838881 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/workflows/
--r-xr-xr-x   0 dude      (1000) dude      (1000)     3649 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/workflows/WorkflowExecution_pb2.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)     4941 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/workflows/WorkflowExecution_pb2_grpc.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)     4343 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/workflows/Workflow_pb2.py
--r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/workflows/Workflow_pb2_grpc.py
--rw-r--r--   0 dude      (1000) dude      (1000)        0 2023-06-19 12:51:36.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/workflows/__init__.py
-drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-19 12:51:41.838881 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic_rpc_protobuf.egg-info/
--rw-r--r--   0 dude      (1000) dude      (1000)     9869 2023-06-19 12:51:41.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic_rpc_protobuf.egg-info/PKG-INFO
--rw-r--r--   0 dude      (1000) dude      (1000)     2539 2023-06-19 12:51:41.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic_rpc_protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 dude      (1000) dude      (1000)        1 2023-06-19 12:51:41.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic_rpc_protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 dude      (1000) dude      (1000)       15 2023-06-19 12:51:41.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic_rpc_protobuf.egg-info/requires.txt
--rw-r--r--   0 dude      (1000) dude      (1000)       11 2023-06-19 12:51:41.000000 deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic_rpc_protobuf.egg-info/top_level.txt
+drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-16 07:58:10.444887 deepomatic-rpc-protobuf-0.21.0a0/
+-rw-rw-r--   0 dude      (1000) dude      (1000)       44 2023-06-12 10:38:48.000000 deepomatic-rpc-protobuf-0.21.0a0/LICENCE
+-rw-r--r--   0 dude      (1000) dude      (1000)     9869 2023-06-16 07:58:10.440886 deepomatic-rpc-protobuf-0.21.0a0/PKG-INFO
+-rw-rw-r--   0 dude      (1000) dude      (1000)     9353 2023-06-15 10:08:49.000000 deepomatic-rpc-protobuf-0.21.0a0/README.md
+-rw-rw-r--   0 dude      (1000) dude      (1000)      675 2023-06-16 07:57:43.000000 deepomatic-rpc-protobuf-0.21.0a0/pyproject.toml
+-rw-r--r--   0 dude      (1000) dude      (1000)       38 2023-06-16 07:58:10.444887 deepomatic-rpc-protobuf-0.21.0a0/setup.cfg
+drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-16 07:58:10.440886 deepomatic-rpc-protobuf-0.21.0a0/src/
+drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-16 07:58:10.440886 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/
+drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-16 07:58:10.440886 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/
+drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-16 07:58:10.440886 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/
+-rw-r--r--   0 dude      (1000) dude      (1000)        0 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/__init__.py
+drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-16 07:58:10.440886 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/
+-rw-r--r--   0 dude      (1000) dude      (1000)        0 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/__init__.py
+drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-16 07:58:10.440886 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/cli/
+-r-xr-xr-x   0 dude      (1000) dude      (1000)     1672 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/cli/Message_pb2.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/cli/Message_pb2_grpc.py
+-rw-r--r--   0 dude      (1000) dude      (1000)        0 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/cli/__init__.py
+drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-16 07:58:10.440886 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/common/
+-r-xr-xr-x   0 dude      (1000) dude      (1000)     1101 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/common/Error_pb2.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/common/Error_pb2_grpc.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)     1419 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/common/Image_pb2.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/common/Image_pb2_grpc.py
+-rw-r--r--   0 dude      (1000) dude      (1000)        0 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/common/__init__.py
+drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-16 07:58:10.440886 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/
+-r-xr-xr-x   0 dude      (1000) dude      (1000)     2639 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Command_pb2.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Command_pb2_grpc.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)     1439 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Message_pb2.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Message_pb2_grpc.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)     7611 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Postprocessing_pb2.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Postprocessing_pb2_grpc.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)     4018 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Preprocessing_pb2.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Preprocessing_pb2_grpc.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)     1583 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Result_pb2.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Result_pb2_grpc.py
+-rw-r--r--   0 dude      (1000) dude      (1000)        0 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/__init__.py
+drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-16 07:58:10.440886 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/frameworks/
+-r-xr-xr-x   0 dude      (1000) dude      (1000)     2303 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/frameworks/Caffe_pb2.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/frameworks/Caffe_pb2_grpc.py
+-rw-r--r--   0 dude      (1000) dude      (1000)        0 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/frameworks/__init__.py
+drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-16 07:58:10.440886 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/
+-r-xr-xr-x   0 dude      (1000) dude      (1000)     1312 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Commands_pb2.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Commands_pb2_grpc.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)     1784 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Inputs_pb2.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Inputs_pb2_grpc.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)     3502 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Results_pb2.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Results_pb2_grpc.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)     2441 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Workflows_pb2.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Workflows_pb2_grpc.py
+-rw-r--r--   0 dude      (1000) dude      (1000)        0 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/__init__.py
+drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-16 07:58:10.440886 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/workflows/
+-r-xr-xr-x   0 dude      (1000) dude      (1000)     3649 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/workflows/WorkflowExecution_pb2.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)     4941 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/workflows/WorkflowExecution_pb2_grpc.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)     4343 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/workflows/Workflow_pb2.py
+-r-xr-xr-x   0 dude      (1000) dude      (1000)      159 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/workflows/Workflow_pb2_grpc.py
+-rw-r--r--   0 dude      (1000) dude      (1000)        0 2023-06-13 15:06:37.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/workflows/__init__.py
+drwxr-xr-x   0 dude      (1000) dude      (1000)        0 2023-06-16 07:58:10.440886 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic_rpc_protobuf.egg-info/
+-rw-r--r--   0 dude      (1000) dude      (1000)     9869 2023-06-16 07:58:10.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic_rpc_protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 dude      (1000) dude      (1000)     2539 2023-06-16 07:58:10.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic_rpc_protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 dude      (1000) dude      (1000)        1 2023-06-16 07:58:10.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic_rpc_protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 dude      (1000) dude      (1000)       15 2023-06-16 07:58:10.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic_rpc_protobuf.egg-info/requires.txt
+-rw-r--r--   0 dude      (1000) dude      (1000)       11 2023-06-16 07:58:10.000000 deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic_rpc_protobuf.egg-info/top_level.txt
```

### Comparing `deepomatic-rpc-protobuf-0.20.0a0/PKG-INFO` & `deepomatic-rpc-protobuf-0.21.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepomatic-rpc-protobuf
-Version: 0.20.0a0
+Version: 0.21.0a0
 Summary: Generated protobufs for deepomatic-rpc
 Author-email: deepomatic <support@deepomatic.com>
 Project-URL: Homepage, https://github.com/Deepomatic/deepomatic-rpc
 Project-URL: Company, https://www.deepomatic.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `deepomatic-rpc-protobuf-0.20.0a0/README.md` & `deepomatic-rpc-protobuf-0.21.0a0/README.md`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/cli/Message_pb2.py` & `deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/cli/Message_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/common/Error_pb2.py` & `deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/common/Error_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/common/Image_pb2.py` & `deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/common/Image_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Command_pb2.py` & `deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Command_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Message_pb2.py` & `deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Message_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Postprocessing_pb2.py` & `deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Postprocessing_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Preprocessing_pb2.py` & `deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Preprocessing_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Result_pb2.py` & `deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/Result_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/frameworks/Caffe_pb2.py` & `deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/frameworks/Caffe_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Commands_pb2.py` & `deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Commands_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Inputs_pb2.py` & `deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Inputs_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Results_pb2.py` & `deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Results_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Workflows_pb2.py` & `deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/nn/v07/Workflows_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/workflows/WorkflowExecution_pb2.py` & `deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/workflows/WorkflowExecution_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/workflows/WorkflowExecution_pb2_grpc.py` & `deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/workflows/WorkflowExecution_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic/rpc/buffers/protobuf/workflows/Workflow_pb2.py` & `deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic/rpc/buffers/protobuf/workflows/Workflow_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic_rpc_protobuf.egg-info/PKG-INFO` & `deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic_rpc_protobuf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepomatic-rpc-protobuf
-Version: 0.20.0a0
+Version: 0.21.0a0
 Summary: Generated protobufs for deepomatic-rpc
 Author-email: deepomatic <support@deepomatic.com>
 Project-URL: Homepage, https://github.com/Deepomatic/deepomatic-rpc
 Project-URL: Company, https://www.deepomatic.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `deepomatic-rpc-protobuf-0.20.0a0/src/deepomatic_rpc_protobuf.egg-info/SOURCES.txt` & `deepomatic-rpc-protobuf-0.21.0a0/src/deepomatic_rpc_protobuf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

