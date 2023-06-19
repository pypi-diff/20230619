# Comparing `tmp/nobuco-0.5.0.tar.gz` & `tmp/nobuco-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.5.0.tar", last modified: Sun Jun 18 11:29:57 2023, max compression
+gzip compressed data, was "nobuco-0.5.1.tar", last modified: Mon Jun 19 11:22:45 2023, max compression
```

## Comparing `nobuco-0.5.0.tar` & `nobuco-0.5.1.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-18 11:29:57.491739 nobuco-0.5.0/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.5.0/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)    22522 2023-06-18 11:29:57.491739 nobuco-0.5.0/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    20688 2023-06-18 11:15:01.000000 nobuco-0.5.0/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-18 11:29:57.487739 nobuco-0.5.0/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    13696 2023-06-09 15:12:04.000000 nobuco-0.5.0/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-18 11:29:57.487739 nobuco-0.5.0/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-06-02 13:56:50.000000 nobuco-0.5.0/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-02 12:03:42.000000 nobuco-0.5.0/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4064 2023-06-06 20:42:12.000000 nobuco-0.5.0/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-18 11:29:57.487739 nobuco-0.5.0/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-05-17 10:49:40.000000 nobuco-0.5.0/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-18 11:29:57.487739 nobuco-0.5.0/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4419 2023-06-17 09:52:53.000000 nobuco-0.5.0/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1069 2023-06-06 15:58:09.000000 nobuco-0.5.0/nobuco/layers/weight.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-18 11:29:57.487739 nobuco-0.5.0/nobuco/locate/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/locate/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/locate/link.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/locate/locate.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-18 11:29:57.491739 nobuco-0.5.0/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     6967 2023-06-15 13:23:44.000000 nobuco-0.5.0/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1165 2023-06-16 16:26:28.000000 nobuco-0.5.0/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-06-01 14:17:46.000000 nobuco-0.5.0/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-05-03 16:03:42.000000 nobuco-0.5.0/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/node_converters/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1533 2023-06-06 20:30:38.000000 nobuco-0.5.0/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     5086 2023-05-01 12:01:37.000000 nobuco-0.5.0/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13838 2023-06-06 20:13:59.000000 nobuco-0.5.0/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-05-16 10:06:23.000000 nobuco-0.5.0/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1638 2023-05-17 15:16:26.000000 nobuco-0.5.0/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-06-07 02:32:02.000000 nobuco-0.5.0/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2879 2023-05-17 15:16:26.000000 nobuco-0.5.0/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9372 2023-06-17 10:31:40.000000 nobuco-0.5.0/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-05-17 10:46:04.000000 nobuco-0.5.0/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5969 2023-06-07 02:44:23.000000 nobuco-0.5.0/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11126 2023-06-06 20:13:14.000000 nobuco-0.5.0/nobuco/node_converters/tensor_manipulation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-06-06 21:33:32.000000 nobuco-0.5.0/nobuco/node_converters/tensor_shape.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-18 11:29:57.491739 nobuco-0.5.0/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-06-06 19:21:15.000000 nobuco-0.5.0/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10039 2023-06-09 15:11:00.000000 nobuco-0.5.0/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-18 11:29:57.491739 nobuco-0.5.0/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-18 11:29:57.487739 nobuco-0.5.0/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    22522 2023-06-18 11:29:57.000000 nobuco-0.5.0/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1628 2023-06-18 11:29:57.000000 nobuco-0.5.0/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-18 11:29:57.000000 nobuco-0.5.0/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-06-18 11:29:57.000000 nobuco-0.5.0/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-06-18 11:29:57.000000 nobuco-0.5.0/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-06-18 11:27:44.000000 nobuco-0.5.0/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-18 11:29:57.491739 nobuco-0.5.0/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 11:22:45.145135 nobuco-0.5.1/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.5.1/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22244 2023-06-19 11:22:45.145135 nobuco-0.5.1/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20410 2023-06-19 11:19:36.000000 nobuco-0.5.1/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 11:22:45.137135 nobuco-0.5.1/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    13696 2023-06-09 15:12:04.000000 nobuco-0.5.1/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 11:22:45.141135 nobuco-0.5.1/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-06-02 13:56:50.000000 nobuco-0.5.1/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-02 12:03:42.000000 nobuco-0.5.1/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4064 2023-06-06 20:42:12.000000 nobuco-0.5.1/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 11:22:45.141135 nobuco-0.5.1/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-05-17 10:49:40.000000 nobuco-0.5.1/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 11:22:45.141135 nobuco-0.5.1/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4419 2023-06-17 09:52:53.000000 nobuco-0.5.1/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1069 2023-06-06 15:58:09.000000 nobuco-0.5.1/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 11:22:45.141135 nobuco-0.5.1/nobuco/locate/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/locate/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/locate/link.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/locate/locate.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 11:22:45.145135 nobuco-0.5.1/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     6967 2023-06-15 13:23:44.000000 nobuco-0.5.1/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2225 2023-06-19 11:09:59.000000 nobuco-0.5.1/nobuco/node_converters/attention.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1165 2023-06-16 16:26:28.000000 nobuco-0.5.1/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-06-01 14:17:46.000000 nobuco-0.5.1/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-05-03 16:03:42.000000 nobuco-0.5.1/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1533 2023-06-06 20:30:38.000000 nobuco-0.5.1/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     5086 2023-05-01 12:01:37.000000 nobuco-0.5.1/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13838 2023-06-06 20:13:59.000000 nobuco-0.5.1/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-05-16 10:06:23.000000 nobuco-0.5.1/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1638 2023-05-17 15:16:26.000000 nobuco-0.5.1/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-06-07 02:32:02.000000 nobuco-0.5.1/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2879 2023-05-17 15:16:26.000000 nobuco-0.5.1/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9372 2023-06-17 10:31:40.000000 nobuco-0.5.1/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-05-17 10:46:04.000000 nobuco-0.5.1/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5969 2023-06-07 02:44:23.000000 nobuco-0.5.1/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11143 2023-06-18 12:05:46.000000 nobuco-0.5.1/nobuco/node_converters/tensor_manipulation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-06-06 21:33:32.000000 nobuco-0.5.1/nobuco/node_converters/tensor_shape.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 11:22:45.145135 nobuco-0.5.1/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-06-06 19:21:15.000000 nobuco-0.5.1/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10039 2023-06-09 15:11:00.000000 nobuco-0.5.1/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 11:22:45.145135 nobuco-0.5.1/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 11:22:45.137135 nobuco-0.5.1/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22244 2023-06-19 11:22:45.000000 nobuco-0.5.1/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1664 2023-06-19 11:22:45.000000 nobuco-0.5.1/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-19 11:22:45.000000 nobuco-0.5.1/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-06-19 11:22:45.000000 nobuco-0.5.1/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-06-19 11:22:45.000000 nobuco-0.5.1/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-06-19 11:19:56.000000 nobuco-0.5.1/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-19 11:22:45.145135 nobuco-0.5.1/setup.cfg
```

### Comparing `nobuco-0.5.0/LICENSE` & `nobuco-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/PKG-INFO` & `nobuco-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.5.0
+Version: 0.5.1
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -483,54 +483,42 @@
 
 As we've learned, Nobuco gets confused when in-place operation is applied to a slice.
 There's a way to fix that, but let's not do it now.
 Instead, we'll use it as an excuse to explain the concept of nested converters.
 So, for this module, conversion will give us incorrect result:
 
 ```python
-class MyModule(nn.Module):
-    def __init__(self):
-        super().__init__()
-        self.conv = nn.Conv2d(3, 3, kernel_size=(3, 3), padding=(1, 1))
-
+class SliceReLU(nn.Module):
     def forward(self, x):
-        x = self.conv(x)
         # Gives incorrect result after conversion
         torch.relu_(x[:, 1:2, 16:25, 8::2])
         # That's the recommended approach, but we're not going for it now
         # x[:, 1:2, 16:25, 8::2] = torch.relu_(x[:, 1:2, 16:25, 8::2])
         return x
-```
-
-<img src="docs/converter_inside_converter1.svg" width="100%">
-
-In the previous section, we've seen it's possible to invoke a Nobuco converter inside another Nobuco converter.
-Can we embed some third-party converter? You bet! Why? Because it might just do what we need.
-Let's consider the standard route: pytorch -> onnx -> tensorflow, with the latter step done with [onnx-tf](https://github.com/onnx/onnx-tensorflow).
-This library likes transposing stuff so much, converting the whole graph with it may introduce intolerable inference overhead. Nonetheless, it does the job.
-A sensible tradeoff would be to wrap the problematic operation into its own `nn.Module` and give it a special treat, while handling everything else with Nobuco.
-
-```python
-class SliceReLU(nn.Module):
-    def forward(self, x):
-        torch.relu_(x[:, 1:2, 16:25, 8::2])
-        return x
 
 
 class MyModule(nn.Module):
     def __init__(self):
         super().__init__()
         self.conv = nn.Conv2d(3, 3, kernel_size=(3, 3), padding=(1, 1))
 
     def forward(self, x):
         x = self.conv(x)
         SliceReLU()(x)
         return x
 ```
 
+<img src="docs/converter_inside_converter1.svg" width="100%">
+
+In the previous section, we've seen it's possible to invoke a Nobuco converter inside another Nobuco converter.
+Can we embed some third-party converter? You bet! Why? Because it might just do what we need.
+Let's consider the standard route: pytorch -> onnx -> tensorflow, with the latter step done with [onnx-tf](https://github.com/onnx/onnx-tensorflow).
+This library likes transposing stuff so much, converting the whole graph with it may introduce intolerable inference overhead. Nonetheless, it does the job.
+A sensible tradeoff would be to wrap the problematic operation into its own `nn.Module` and give it a special treat, while handling everything else with Nobuco.
+
 ```python
 import onnx
 from onnx_tf.backend import prepare
 
 
 @nobuco.converter(SliceReLU, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER, reusable=False)
 def converter_SliceReLU(self, x):
```

### Comparing `nobuco-0.5.0/README.md` & `nobuco-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -447,54 +447,42 @@
 
 As we've learned, Nobuco gets confused when in-place operation is applied to a slice.
 There's a way to fix that, but let's not do it now.
 Instead, we'll use it as an excuse to explain the concept of nested converters.
 So, for this module, conversion will give us incorrect result:
 
 ```python
-class MyModule(nn.Module):
-    def __init__(self):
-        super().__init__()
-        self.conv = nn.Conv2d(3, 3, kernel_size=(3, 3), padding=(1, 1))
-
+class SliceReLU(nn.Module):
     def forward(self, x):
-        x = self.conv(x)
         # Gives incorrect result after conversion
         torch.relu_(x[:, 1:2, 16:25, 8::2])
         # That's the recommended approach, but we're not going for it now
         # x[:, 1:2, 16:25, 8::2] = torch.relu_(x[:, 1:2, 16:25, 8::2])
         return x
-```
-
-<img src="docs/converter_inside_converter1.svg" width="100%">
-
-In the previous section, we've seen it's possible to invoke a Nobuco converter inside another Nobuco converter.
-Can we embed some third-party converter? You bet! Why? Because it might just do what we need.
-Let's consider the standard route: pytorch -> onnx -> tensorflow, with the latter step done with [onnx-tf](https://github.com/onnx/onnx-tensorflow).
-This library likes transposing stuff so much, converting the whole graph with it may introduce intolerable inference overhead. Nonetheless, it does the job.
-A sensible tradeoff would be to wrap the problematic operation into its own `nn.Module` and give it a special treat, while handling everything else with Nobuco.
-
-```python
-class SliceReLU(nn.Module):
-    def forward(self, x):
-        torch.relu_(x[:, 1:2, 16:25, 8::2])
-        return x
 
 
 class MyModule(nn.Module):
     def __init__(self):
         super().__init__()
         self.conv = nn.Conv2d(3, 3, kernel_size=(3, 3), padding=(1, 1))
 
     def forward(self, x):
         x = self.conv(x)
         SliceReLU()(x)
         return x
 ```
 
+<img src="docs/converter_inside_converter1.svg" width="100%">
+
+In the previous section, we've seen it's possible to invoke a Nobuco converter inside another Nobuco converter.
+Can we embed some third-party converter? You bet! Why? Because it might just do what we need.
+Let's consider the standard route: pytorch -> onnx -> tensorflow, with the latter step done with [onnx-tf](https://github.com/onnx/onnx-tensorflow).
+This library likes transposing stuff so much, converting the whole graph with it may introduce intolerable inference overhead. Nonetheless, it does the job.
+A sensible tradeoff would be to wrap the problematic operation into its own `nn.Module` and give it a special treat, while handling everything else with Nobuco.
+
 ```python
 import onnx
 from onnx_tf.backend import prepare
 
 
 @nobuco.converter(SliceReLU, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER, reusable=False)
 def converter_SliceReLU(self, x):
```

### Comparing `nobuco-0.5.0/nobuco/__init__.py` & `nobuco-0.5.1/nobuco/__init__.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/commons.py` & `nobuco-0.5.1/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/convert.py` & `nobuco-0.5.1/nobuco/convert.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/converters/channel_ordering.py` & `nobuco-0.5.1/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/converters/node_converter.py` & `nobuco-0.5.1/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/converters/tensor.py` & `nobuco-0.5.1/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/converters/type_cast.py` & `nobuco-0.5.1/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/converters/validation.py` & `nobuco-0.5.1/nobuco/converters/validation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/entity/keras.py` & `nobuco-0.5.1/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/entity/pytorch.py` & `nobuco-0.5.1/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/funcs.py` & `nobuco-0.5.1/nobuco/funcs.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/layers/channel_order.py` & `nobuco-0.5.1/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/layers/container.py` & `nobuco-0.5.1/nobuco/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/layers/weight.py` & `nobuco-0.5.1/nobuco/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/locate/link.py` & `nobuco-0.5.1/nobuco/locate/link.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/locate/locate.py` & `nobuco-0.5.1/nobuco/locate/locate.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/node_converters/activation.py` & `nobuco-0.5.1/nobuco/node_converters/activation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/node_converters/boolean.py` & `nobuco-0.5.1/nobuco/node_converters/boolean.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/node_converters/boolean_mask.py` & `nobuco-0.5.1/nobuco/node_converters/boolean_mask.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/node_converters/comparison.py` & `nobuco-0.5.1/nobuco/node_converters/comparison.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/node_converters/convolution.py` & `nobuco-0.5.1/nobuco/node_converters/convolution.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/node_converters/dropout.py` & `nobuco-0.5.1/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/node_converters/interpolation.py` & `nobuco-0.5.1/nobuco/node_converters/interpolation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/node_converters/linear.py` & `nobuco-0.5.1/nobuco/node_converters/linear.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/node_converters/math.py` & `nobuco-0.5.1/nobuco/node_converters/math.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/node_converters/misc.py` & `nobuco-0.5.1/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/node_converters/normalization.py` & `nobuco-0.5.1/nobuco/node_converters/normalization.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/node_converters/padding.py` & `nobuco-0.5.1/nobuco/node_converters/padding.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/node_converters/pooling.py` & `nobuco-0.5.1/nobuco/node_converters/pooling.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/node_converters/recurrent.py` & `nobuco-0.5.1/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/node_converters/slice.py` & `nobuco-0.5.1/nobuco/node_converters/slice.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/node_converters/tensor_cast.py` & `nobuco-0.5.1/nobuco/node_converters/tensor_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/node_converters/tensor_creation.py` & `nobuco-0.5.1/nobuco/node_converters/tensor_creation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.5.1/nobuco/node_converters/tensor_manipulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,16 +208,16 @@
 @converter(torch.Tensor.unbind, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
 def converter_unbind(self, dim=0):
     def func(self, dim=0):
         return tf.unstack(self, axis=dim)
     return func
 
 
-@converter(torch.Tensor.flatten, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
-def converter_flatten(self, start_dim=0, end_dim=-1):
+@converter(torch.Tensor.flatten, torch.flatten, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
+def converter_t_flatten(self, start_dim=0, end_dim=-1):
     def func(self, start_dim=0, end_dim=-1):
         start_shape = self.shape[:start_dim]
 
         n_dims = len(self.shape)
         end_dim = _dim_make_positive(end_dim, n_dims)
         if end_dim < n_dims-1:
             end_shape = self.shape[end_dim+1:]
```

### Comparing `nobuco-0.5.0/nobuco/trace/tensor_storage.py` & `nobuco-0.5.1/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/trace/trace.py` & `nobuco-0.5.1/nobuco/trace/trace.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/util.py` & `nobuco-0.5.1/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/vis/console_stylizer.py` & `nobuco-0.5.1/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco/vis/html_stylizer.py` & `nobuco-0.5.1/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.0/nobuco.egg-info/PKG-INFO` & `nobuco-0.5.1/nobuco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.5.0
+Version: 0.5.1
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -483,54 +483,42 @@
 
 As we've learned, Nobuco gets confused when in-place operation is applied to a slice.
 There's a way to fix that, but let's not do it now.
 Instead, we'll use it as an excuse to explain the concept of nested converters.
 So, for this module, conversion will give us incorrect result:
 
 ```python
-class MyModule(nn.Module):
-    def __init__(self):
-        super().__init__()
-        self.conv = nn.Conv2d(3, 3, kernel_size=(3, 3), padding=(1, 1))
-
+class SliceReLU(nn.Module):
     def forward(self, x):
-        x = self.conv(x)
         # Gives incorrect result after conversion
         torch.relu_(x[:, 1:2, 16:25, 8::2])
         # That's the recommended approach, but we're not going for it now
         # x[:, 1:2, 16:25, 8::2] = torch.relu_(x[:, 1:2, 16:25, 8::2])
         return x
-```
-
-<img src="docs/converter_inside_converter1.svg" width="100%">
-
-In the previous section, we've seen it's possible to invoke a Nobuco converter inside another Nobuco converter.
-Can we embed some third-party converter? You bet! Why? Because it might just do what we need.
-Let's consider the standard route: pytorch -> onnx -> tensorflow, with the latter step done with [onnx-tf](https://github.com/onnx/onnx-tensorflow).
-This library likes transposing stuff so much, converting the whole graph with it may introduce intolerable inference overhead. Nonetheless, it does the job.
-A sensible tradeoff would be to wrap the problematic operation into its own `nn.Module` and give it a special treat, while handling everything else with Nobuco.
-
-```python
-class SliceReLU(nn.Module):
-    def forward(self, x):
-        torch.relu_(x[:, 1:2, 16:25, 8::2])
-        return x
 
 
 class MyModule(nn.Module):
     def __init__(self):
         super().__init__()
         self.conv = nn.Conv2d(3, 3, kernel_size=(3, 3), padding=(1, 1))
 
     def forward(self, x):
         x = self.conv(x)
         SliceReLU()(x)
         return x
 ```
 
+<img src="docs/converter_inside_converter1.svg" width="100%">
+
+In the previous section, we've seen it's possible to invoke a Nobuco converter inside another Nobuco converter.
+Can we embed some third-party converter? You bet! Why? Because it might just do what we need.
+Let's consider the standard route: pytorch -> onnx -> tensorflow, with the latter step done with [onnx-tf](https://github.com/onnx/onnx-tensorflow).
+This library likes transposing stuff so much, converting the whole graph with it may introduce intolerable inference overhead. Nonetheless, it does the job.
+A sensible tradeoff would be to wrap the problematic operation into its own `nn.Module` and give it a special treat, while handling everything else with Nobuco.
+
 ```python
 import onnx
 from onnx_tf.backend import prepare
 
 
 @nobuco.converter(SliceReLU, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER, reusable=False)
 def converter_SliceReLU(self, x):
```

### Comparing `nobuco-0.5.0/nobuco.egg-info/SOURCES.txt` & `nobuco-0.5.1/nobuco.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 nobuco/layers/stub.py
 nobuco/layers/weight.py
 nobuco/locate/__init__.py
 nobuco/locate/link.py
 nobuco/locate/locate.py
 nobuco/node_converters/__init__.py
 nobuco/node_converters/activation.py
+nobuco/node_converters/attention.py
 nobuco/node_converters/boolean.py
 nobuco/node_converters/boolean_mask.py
 nobuco/node_converters/comparison.py
 nobuco/node_converters/convolution.py
 nobuco/node_converters/dropout.py
 nobuco/node_converters/interpolation.py
 nobuco/node_converters/linear.py
```

### Comparing `nobuco-0.5.0/pyproject.toml` & `nobuco-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.5.0"
+version = "0.5.1"
 description = "Pytorch to Tensorflow conversion made somewhat easy"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

