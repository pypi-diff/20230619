# Comparing `tmp/nobuco-0.5.1.tar.gz` & `tmp/nobuco-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.5.1.tar", last modified: Mon Jun 19 11:22:45 2023, max compression
+gzip compressed data, was "nobuco-0.5.2.tar", last modified: Mon Jun 19 20:17:02 2023, max compression
```

## Comparing `nobuco-0.5.1.tar` & `nobuco-0.5.2.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 11:22:45.145135 nobuco-0.5.1/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.5.1/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)    22244 2023-06-19 11:22:45.145135 nobuco-0.5.1/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    20410 2023-06-19 11:19:36.000000 nobuco-0.5.1/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 11:22:45.137135 nobuco-0.5.1/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    13696 2023-06-09 15:12:04.000000 nobuco-0.5.1/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 11:22:45.141135 nobuco-0.5.1/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-06-02 13:56:50.000000 nobuco-0.5.1/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-02 12:03:42.000000 nobuco-0.5.1/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4064 2023-06-06 20:42:12.000000 nobuco-0.5.1/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 11:22:45.141135 nobuco-0.5.1/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-05-17 10:49:40.000000 nobuco-0.5.1/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 11:22:45.141135 nobuco-0.5.1/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4419 2023-06-17 09:52:53.000000 nobuco-0.5.1/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1069 2023-06-06 15:58:09.000000 nobuco-0.5.1/nobuco/layers/weight.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 11:22:45.141135 nobuco-0.5.1/nobuco/locate/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/locate/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/locate/link.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/locate/locate.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 11:22:45.145135 nobuco-0.5.1/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     6967 2023-06-15 13:23:44.000000 nobuco-0.5.1/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2225 2023-06-19 11:09:59.000000 nobuco-0.5.1/nobuco/node_converters/attention.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1165 2023-06-16 16:26:28.000000 nobuco-0.5.1/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-06-01 14:17:46.000000 nobuco-0.5.1/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-05-03 16:03:42.000000 nobuco-0.5.1/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/node_converters/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1533 2023-06-06 20:30:38.000000 nobuco-0.5.1/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     5086 2023-05-01 12:01:37.000000 nobuco-0.5.1/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13838 2023-06-06 20:13:59.000000 nobuco-0.5.1/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-05-16 10:06:23.000000 nobuco-0.5.1/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1638 2023-05-17 15:16:26.000000 nobuco-0.5.1/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-06-07 02:32:02.000000 nobuco-0.5.1/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2879 2023-05-17 15:16:26.000000 nobuco-0.5.1/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9372 2023-06-17 10:31:40.000000 nobuco-0.5.1/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-05-17 10:46:04.000000 nobuco-0.5.1/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5969 2023-06-07 02:44:23.000000 nobuco-0.5.1/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11143 2023-06-18 12:05:46.000000 nobuco-0.5.1/nobuco/node_converters/tensor_manipulation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-06-06 21:33:32.000000 nobuco-0.5.1/nobuco/node_converters/tensor_shape.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 11:22:45.145135 nobuco-0.5.1/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-06-06 19:21:15.000000 nobuco-0.5.1/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10039 2023-06-09 15:11:00.000000 nobuco-0.5.1/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 11:22:45.145135 nobuco-0.5.1/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.5.1/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 11:22:45.137135 nobuco-0.5.1/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    22244 2023-06-19 11:22:45.000000 nobuco-0.5.1/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1664 2023-06-19 11:22:45.000000 nobuco-0.5.1/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-19 11:22:45.000000 nobuco-0.5.1/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-06-19 11:22:45.000000 nobuco-0.5.1/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-06-19 11:22:45.000000 nobuco-0.5.1/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-06-19 11:19:56.000000 nobuco-0.5.1/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-19 11:22:45.145135 nobuco-0.5.1/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 20:17:02.816937 nobuco-0.5.2/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.5.2/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22244 2023-06-19 20:17:02.816937 nobuco-0.5.2/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20410 2023-06-19 11:19:36.000000 nobuco-0.5.2/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 20:17:02.808937 nobuco-0.5.2/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    13970 2023-06-19 19:46:46.000000 nobuco-0.5.2/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 20:17:02.808937 nobuco-0.5.2/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-06-02 13:56:50.000000 nobuco-0.5.2/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-19 20:03:57.000000 nobuco-0.5.2/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4048 2023-06-19 19:40:14.000000 nobuco-0.5.2/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 20:17:02.808937 nobuco-0.5.2/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-05-17 10:49:40.000000 nobuco-0.5.2/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 20:17:02.808937 nobuco-0.5.2/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4419 2023-06-17 09:52:53.000000 nobuco-0.5.2/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1069 2023-06-06 15:58:09.000000 nobuco-0.5.2/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 20:17:02.812937 nobuco-0.5.2/nobuco/locate/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/locate/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/locate/link.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/locate/locate.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 20:17:02.812937 nobuco-0.5.2/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     6967 2023-06-15 13:23:44.000000 nobuco-0.5.2/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2225 2023-06-19 11:09:59.000000 nobuco-0.5.2/nobuco/node_converters/attention.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1169 2023-06-19 13:20:31.000000 nobuco-0.5.2/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1165 2023-06-16 16:26:28.000000 nobuco-0.5.2/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-06-01 14:17:46.000000 nobuco-0.5.2/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-05-03 16:03:42.000000 nobuco-0.5.2/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1533 2023-06-06 20:30:38.000000 nobuco-0.5.2/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     5152 2023-06-19 13:27:23.000000 nobuco-0.5.2/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13838 2023-06-06 20:13:59.000000 nobuco-0.5.2/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-05-16 10:06:23.000000 nobuco-0.5.2/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1638 2023-05-17 15:16:26.000000 nobuco-0.5.2/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-06-07 02:32:02.000000 nobuco-0.5.2/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2879 2023-05-17 15:16:26.000000 nobuco-0.5.2/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9538 2023-06-19 13:43:03.000000 nobuco-0.5.2/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-05-17 10:46:04.000000 nobuco-0.5.2/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6244 2023-06-19 13:24:40.000000 nobuco-0.5.2/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11297 2023-06-19 20:07:28.000000 nobuco-0.5.2/nobuco/node_converters/tensor_manipulation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-06-06 21:33:32.000000 nobuco-0.5.2/nobuco/node_converters/tensor_shape.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      452 2023-06-19 20:13:01.000000 nobuco-0.5.2/nobuco/node_converters/torchvision.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 20:17:02.812937 nobuco-0.5.2/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-06-06 19:21:15.000000 nobuco-0.5.2/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10039 2023-06-09 15:11:00.000000 nobuco-0.5.2/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 20:17:02.816937 nobuco-0.5.2/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 20:17:02.808937 nobuco-0.5.2/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22244 2023-06-19 20:17:02.000000 nobuco-0.5.2/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1702 2023-06-19 20:17:02.000000 nobuco-0.5.2/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-19 20:17:02.000000 nobuco-0.5.2/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-06-19 20:17:02.000000 nobuco-0.5.2/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-06-19 20:17:02.000000 nobuco-0.5.2/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-06-19 20:10:11.000000 nobuco-0.5.2/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-19 20:17:02.816937 nobuco-0.5.2/setup.cfg
```

### Comparing `nobuco-0.5.1/LICENSE` & `nobuco-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/PKG-INFO` & `nobuco-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.5.1
+Version: 0.5.2
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nobuco-0.5.1/README.md` & `nobuco-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/__init__.py` & `nobuco-0.5.2/nobuco/__init__.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/commons.py` & `nobuco-0.5.2/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/convert.py` & `nobuco-0.5.2/nobuco/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+import traceback
 import warnings
 from typing import Callable, Dict, Collection, Optional, List, Union, Tuple
 
 import torch
 from nobuco.converters.tensor import permute_pytorch2keras
 from torch import nn
 import tensorflow as tf
@@ -133,16 +134,21 @@
         keras_op, children_converted_nodes = converted_op_dict.get(node.get_op(), (None, []))
         node_is_reusable = False
         if reuse_layers and keras_op is not None:
             conversion_result = ConversionResult(converted_manually=False, is_duplicate=True, converter=converter)
         elif has_converter(node, converter_dict):
             children_converted_nodes = []
             node_converter: Pytorch2KerasNodeConverter = converter_dict.get(node.get_type(), None)
-            node_is_reusable = node_converter.reusable
-            keras_op = convert_node(node, node_converter)
+            try:
+                keras_op = convert_node(node, node_converter)
+                node_is_reusable = node_converter.reusable
+            except Exception as e:
+                warnings.warn(f"Conversion exception on node '{node.get_type().__name__}': {e}")
+                traceback.print_exc()
+                keras_op = UnimplementedOpStub(node.get_op())
             conversion_result = ConversionResult(converted_manually=True, converter=converter)
         elif len(children) > 0:
             children_converted_nodes = [convert(child, converted_op_dict, reuse_layers, full_validation, depth + 1) for child in children]
             keras_op = convert_container(node, children, children_converted_nodes, input_names, output_names, node.output_tensors, constants_to_variables=constants_to_variables)
 
             connectivity_status = keras_op.get_connectivity_status()
             if not connectivity_status.is_connected():
```

### Comparing `nobuco-0.5.1/nobuco/converters/channel_ordering.py` & `nobuco-0.5.2/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/converters/node_converter.py` & `nobuco-0.5.2/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/converters/tensor.py` & `nobuco-0.5.2/nobuco/converters/tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         return iterable[0]
     else:
         return iterable
 
 
 def _ensure_iterable(iterable):
     if isinstance(iterable, (list, tuple)):
-        if isinstance(iterable[0], (list, tuple)) and len(iterable) == 1:
+        if len(iterable) == 1 and isinstance(iterable[0], (list, tuple)):
             return iterable[0]
         return iterable
     else:
         return [iterable]
 
 
 def _ensure_tuple(iterable):
```

### Comparing `nobuco-0.5.1/nobuco/converters/type_cast.py` & `nobuco-0.5.2/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/converters/validation.py` & `nobuco-0.5.2/nobuco/converters/validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,16 +56,16 @@
             diff = 0
 
         if diff > tolerance or math.isnan(diff):
             return diff, ValidationStatus.INACCURATE
         else:
             return diff, ValidationStatus.SUCCESS
     except Exception as e:
-        # raise Exception("Validation exception on node '{}'".format(op_type.__name__), e)
-        warnings.warn("Validation exception on node '{}': {}".format(op_type.__name__, e))
+        # raise Exception(f"Validation exception on node '{op_type.__name__}': {e}")
+        warnings.warn(f"Validation exception on node '{op_type.__name__}': {e}")
         return None, ValidationStatus.FAIL
 
 
 def validate_diff_default(keras_op, pytorch_op, args_pt, kwargs_pt, outputs_pt, is_training=False):
     args_tf = pytorch2keras_recursively(args_pt, channel_order=ChannelOrder.TENSORFLOW)
     kwargs_tf = pytorch2keras_recursively(kwargs_pt, channel_order=ChannelOrder.TENSORFLOW)
```

### Comparing `nobuco-0.5.1/nobuco/entity/keras.py` & `nobuco-0.5.2/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/entity/pytorch.py` & `nobuco-0.5.2/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/funcs.py` & `nobuco-0.5.2/nobuco/funcs.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/layers/channel_order.py` & `nobuco-0.5.2/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/layers/container.py` & `nobuco-0.5.2/nobuco/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/layers/weight.py` & `nobuco-0.5.2/nobuco/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/locate/link.py` & `nobuco-0.5.2/nobuco/locate/link.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/locate/locate.py` & `nobuco-0.5.2/nobuco/locate/locate.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/node_converters/activation.py` & `nobuco-0.5.2/nobuco/node_converters/activation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/node_converters/attention.py` & `nobuco-0.5.2/nobuco/node_converters/attention.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/node_converters/boolean.py` & `nobuco-0.5.2/nobuco/node_converters/boolean.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,7 +22,15 @@
 
 
 @converter(torch.Tensor.__invert__, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def converter_invert(input: Tensor):
     def func(input):
         return tf.math.logical_not(input)
     return func
+
+
+@converter(torch.Tensor.__ne__, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_ne(self, *args, **kwargs):
+    def func(self, *args, **kwargs):
+        val = args[0]
+        return tf.math.not_equal(self, val)
+    return func
```

### Comparing `nobuco-0.5.1/nobuco/node_converters/boolean_mask.py` & `nobuco-0.5.2/nobuco/node_converters/boolean_mask.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/node_converters/comparison.py` & `nobuco-0.5.2/nobuco/node_converters/comparison.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/node_converters/convolution.py` & `nobuco-0.5.2/nobuco/node_converters/convolution.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/node_converters/dropout.py` & `nobuco-0.5.2/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/node_converters/interpolation.py` & `nobuco-0.5.2/nobuco/node_converters/interpolation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/node_converters/linear.py` & `nobuco-0.5.2/nobuco/node_converters/linear.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,36 +19,37 @@
 
 @converter(nn.Linear, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
 def converter_Linear(self, input: Tensor):
     out_filters, in_filters = self.weight.shape
     weights = self.weight.detach().numpy()
     weights = weights.transpose(1, 0)
 
-    biases = self.bias
-    if biases is not None:
+    use_bias = self.bias is not None
+    if use_bias:
         biases = self.bias.detach().numpy()
         params = [weights, biases]
     else:
         params = [weights]
-    return keras.layers.Dense(out_filters, weights=params)
+    return keras.layers.Dense(out_filters, use_bias=use_bias, weights=params)
 
 
 @converter(torch.nn.functional.linear, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
 def converter_linear(input, weight, bias, out=None):
     out_filters, in_filters = weight.shape
     weights = weight.detach().numpy()
     weights = weights.transpose(1, 0)
 
-    if bias is not None:
+    use_bias = bias is not None
+    if use_bias:
         biases = bias.detach().numpy()
         params = [weights, biases]
     else:
         params = [weights]
 
-    layer = keras.layers.Dense(out_filters, weights=params)
+    layer = keras.layers.Dense(out_filters, use_bias=use_bias, weights=params)
 
     def func(input, weight, bias, out=None):
         return layer(input)
     return func
 
 
 @converter(torch.matmul, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
```

### Comparing `nobuco-0.5.1/nobuco/node_converters/math.py` & `nobuco-0.5.2/nobuco/node_converters/math.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/node_converters/misc.py` & `nobuco-0.5.2/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/node_converters/normalization.py` & `nobuco-0.5.2/nobuco/node_converters/normalization.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/node_converters/padding.py` & `nobuco-0.5.2/nobuco/node_converters/padding.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/node_converters/pooling.py` & `nobuco-0.5.2/nobuco/node_converters/pooling.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/node_converters/recurrent.py` & `nobuco-0.5.2/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/node_converters/slice.py` & `nobuco-0.5.2/nobuco/node_converters/slice.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,19 @@
                 if start is None:
                     start = 0
                 if stop is None:
                     stop = shape[real_index]
                 if step is None:
                     step = 1
 
+                if start < 0:
+                    start = shape[real_index] + start
+                if stop < 0:
+                    stop = shape[real_index] + stop
+
                 corresponding_range = tf.cast(tf.range(start, stop, step), dtype=tf.int32)
             else:
                 slice_spec = tf.convert_to_tensor(slice_spec)
                 corresponding_range = tf.cast(slice_spec, dtype=tf.int32)
                 n_indexed_dims += 1
 
             corresponding_ranges.append(corresponding_range)
```

### Comparing `nobuco-0.5.1/nobuco/node_converters/tensor_cast.py` & `nobuco-0.5.2/nobuco/node_converters/tensor_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/node_converters/tensor_creation.py` & `nobuco-0.5.2/nobuco/node_converters/tensor_creation.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,21 @@
 def converter_zeros_like(input: Tensor, *, memory_format=None, dtype=None, layout=None, device=None, pin_memory=False, requires_grad=False):
     def func(input: Tensor, *, memory_format=None, dtype=None, layout=None, device=None, pin_memory=False, requires_grad=False):
         tf_type = dtype_pytorch2keras(dtype)
         return tf.zeros_like(input, dtype=tf_type)
     return func
 
 
+@converter(torch.Tensor.new_zeros, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
+def converter_new_zeros(self, size, *args, **kwargs):
+    def func(self, size, *args, **kwargs):
+        return tf.zeros(shape=size, dtype=self.dtype)
+    return func
+
+
 @converter(torch.Tensor.new_empty, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
 def converter_new_empty(self, size, dtype=None, device=None, requires_grad=False, layout=torch.strided, pin_memory=False):
     def func(self, size, dtype=None, device=None, requires_grad=False, layout=torch.strided, pin_memory=False):
         if dtype is not None:
             dtype = dtype_pytorch2keras(dtype)
         else:
             dtype = self.dtype
```

### Comparing `nobuco-0.5.1/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.5.2/nobuco/node_converters/tensor_manipulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy as np
 
 from nobuco.commons import ChannelOrder, ChannelOrderingStrategy
 from nobuco.converters.channel_ordering import set_channel_order, get_channel_order
 from nobuco.converters.node_converter import converter
 from nobuco.converters.tensor import dims_pytorch2keras, perm_keras2pytorch, \
     _dim_make_positive, dim_pytorch2keras, _permute, _flatten, perm_pytorch2keras, perm_compose, \
-    is_identity_perm, permute_pytorch2keras, perm_identity
+    is_identity_perm, permute_pytorch2keras, perm_identity, _ensure_iterable
 
 
 def _permute_inner(perm_original, allow_lazy=True):
     def func(x):
         input_channel_order = get_channel_order(x)
 
         if allow_lazy:
@@ -191,21 +191,28 @@
         broadcast_shape = get_broadcast_shape(other.shape, self.shape)
         return tf.broadcast_to(self, broadcast_shape)
     return func
 
 
 @converter(torch.roll, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def converter_roll(input: Tensor, shifts: Union[_int, _size], dims: Union[_int, _size]=()):
-    assert isinstance(shifts, _int) and isinstance(dims, _int)
+    assert dims != (), 'Assertion error'
     n_dims = input.dim()
 
     def func(input, shifts, dims=()):
+        shifts = _ensure_iterable(shifts)
+        dims = _ensure_iterable(dims)
+
         if get_channel_order(input) == ChannelOrder.TENSORFLOW:
-            dims = dim_pytorch2keras(dims, n_dims)
-        return tf.roll(input, shift=shifts, axis=dims)
+            dims = dims_pytorch2keras(dims, n_dims)
+
+        x = input
+        for shift, dim in zip(shifts, dims):
+            x = tf.roll(x, shift=shift, axis=dim)
+        return x
     return func
 
 
 @converter(torch.Tensor.unbind, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
 def converter_unbind(self, dim=0):
     def func(self, dim=0):
         return tf.unstack(self, axis=dim)
```

### Comparing `nobuco-0.5.1/nobuco/trace/tensor_storage.py` & `nobuco-0.5.2/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/trace/trace.py` & `nobuco-0.5.2/nobuco/trace/trace.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/util.py` & `nobuco-0.5.2/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/vis/console_stylizer.py` & `nobuco-0.5.2/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco/vis/html_stylizer.py` & `nobuco-0.5.2/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.1/nobuco.egg-info/PKG-INFO` & `nobuco-0.5.2/nobuco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.5.1
+Version: 0.5.2
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nobuco-0.5.1/nobuco.egg-info/SOURCES.txt` & `nobuco-0.5.2/nobuco.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -45,13 +45,14 @@
 nobuco/node_converters/pooling.py
 nobuco/node_converters/recurrent.py
 nobuco/node_converters/slice.py
 nobuco/node_converters/tensor_cast.py
 nobuco/node_converters/tensor_creation.py
 nobuco/node_converters/tensor_manipulation.py
 nobuco/node_converters/tensor_shape.py
+nobuco/node_converters/torchvision.py
 nobuco/trace/__init__.py
 nobuco/trace/tensor_storage.py
 nobuco/trace/trace.py
 nobuco/vis/__init__.py
 nobuco/vis/console_stylizer.py
 nobuco/vis/html_stylizer.py
```

### Comparing `nobuco-0.5.1/pyproject.toml` & `nobuco-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.5.1"
+version = "0.5.2"
 description = "Pytorch to Tensorflow conversion made somewhat easy"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

