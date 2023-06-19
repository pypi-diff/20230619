# Comparing `tmp/nobuco-0.5.2.tar.gz` & `tmp/nobuco-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.5.2.tar", last modified: Mon Jun 19 20:17:02 2023, max compression
+gzip compressed data, was "nobuco-0.5.3.tar", last modified: Mon Jun 19 21:45:24 2023, max compression
```

## Comparing `nobuco-0.5.2.tar` & `nobuco-0.5.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 20:17:02.816937 nobuco-0.5.2/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.5.2/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)    22244 2023-06-19 20:17:02.816937 nobuco-0.5.2/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    20410 2023-06-19 11:19:36.000000 nobuco-0.5.2/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 20:17:02.808937 nobuco-0.5.2/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    13970 2023-06-19 19:46:46.000000 nobuco-0.5.2/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 20:17:02.808937 nobuco-0.5.2/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-06-02 13:56:50.000000 nobuco-0.5.2/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-19 20:03:57.000000 nobuco-0.5.2/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4048 2023-06-19 19:40:14.000000 nobuco-0.5.2/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 20:17:02.808937 nobuco-0.5.2/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-05-17 10:49:40.000000 nobuco-0.5.2/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 20:17:02.808937 nobuco-0.5.2/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4419 2023-06-17 09:52:53.000000 nobuco-0.5.2/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1069 2023-06-06 15:58:09.000000 nobuco-0.5.2/nobuco/layers/weight.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 20:17:02.812937 nobuco-0.5.2/nobuco/locate/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/locate/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/locate/link.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/locate/locate.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 20:17:02.812937 nobuco-0.5.2/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     6967 2023-06-15 13:23:44.000000 nobuco-0.5.2/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2225 2023-06-19 11:09:59.000000 nobuco-0.5.2/nobuco/node_converters/attention.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1169 2023-06-19 13:20:31.000000 nobuco-0.5.2/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1165 2023-06-16 16:26:28.000000 nobuco-0.5.2/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-06-01 14:17:46.000000 nobuco-0.5.2/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-05-03 16:03:42.000000 nobuco-0.5.2/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/node_converters/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1533 2023-06-06 20:30:38.000000 nobuco-0.5.2/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     5152 2023-06-19 13:27:23.000000 nobuco-0.5.2/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13838 2023-06-06 20:13:59.000000 nobuco-0.5.2/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-05-16 10:06:23.000000 nobuco-0.5.2/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1638 2023-05-17 15:16:26.000000 nobuco-0.5.2/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-06-07 02:32:02.000000 nobuco-0.5.2/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2879 2023-05-17 15:16:26.000000 nobuco-0.5.2/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9538 2023-06-19 13:43:03.000000 nobuco-0.5.2/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-05-17 10:46:04.000000 nobuco-0.5.2/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6244 2023-06-19 13:24:40.000000 nobuco-0.5.2/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11297 2023-06-19 20:07:28.000000 nobuco-0.5.2/nobuco/node_converters/tensor_manipulation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-06-06 21:33:32.000000 nobuco-0.5.2/nobuco/node_converters/tensor_shape.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      452 2023-06-19 20:13:01.000000 nobuco-0.5.2/nobuco/node_converters/torchvision.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 20:17:02.812937 nobuco-0.5.2/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-06-06 19:21:15.000000 nobuco-0.5.2/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10039 2023-06-09 15:11:00.000000 nobuco-0.5.2/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 20:17:02.816937 nobuco-0.5.2/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.5.2/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 20:17:02.808937 nobuco-0.5.2/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    22244 2023-06-19 20:17:02.000000 nobuco-0.5.2/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1702 2023-06-19 20:17:02.000000 nobuco-0.5.2/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-19 20:17:02.000000 nobuco-0.5.2/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-06-19 20:17:02.000000 nobuco-0.5.2/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-06-19 20:17:02.000000 nobuco-0.5.2/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-06-19 20:10:11.000000 nobuco-0.5.2/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-19 20:17:02.816937 nobuco-0.5.2/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 21:45:24.893394 nobuco-0.5.3/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.5.3/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22244 2023-06-19 21:45:24.893394 nobuco-0.5.3/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20410 2023-06-19 11:19:36.000000 nobuco-0.5.3/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 21:45:24.885394 nobuco-0.5.3/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    13970 2023-06-19 19:46:46.000000 nobuco-0.5.3/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 21:45:24.885394 nobuco-0.5.3/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-06-02 13:56:50.000000 nobuco-0.5.3/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-19 20:03:57.000000 nobuco-0.5.3/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4095 2023-06-19 20:43:10.000000 nobuco-0.5.3/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 21:45:24.885394 nobuco-0.5.3/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-05-17 10:49:40.000000 nobuco-0.5.3/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 21:45:24.885394 nobuco-0.5.3/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4419 2023-06-17 09:52:53.000000 nobuco-0.5.3/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1069 2023-06-06 15:58:09.000000 nobuco-0.5.3/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 21:45:24.889394 nobuco-0.5.3/nobuco/locate/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/locate/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/locate/link.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/locate/locate.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 21:45:24.893394 nobuco-0.5.3/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     6967 2023-06-15 13:23:44.000000 nobuco-0.5.3/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2225 2023-06-19 11:09:59.000000 nobuco-0.5.3/nobuco/node_converters/attention.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1169 2023-06-19 13:20:31.000000 nobuco-0.5.3/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1165 2023-06-16 16:26:28.000000 nobuco-0.5.3/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-06-01 14:17:46.000000 nobuco-0.5.3/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-05-03 16:03:42.000000 nobuco-0.5.3/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1533 2023-06-06 20:30:38.000000 nobuco-0.5.3/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     5152 2023-06-19 13:27:23.000000 nobuco-0.5.3/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13838 2023-06-06 20:13:59.000000 nobuco-0.5.3/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-05-16 10:06:23.000000 nobuco-0.5.3/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1662 2023-06-19 20:57:04.000000 nobuco-0.5.3/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-06-07 02:32:02.000000 nobuco-0.5.3/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2934 2023-06-19 21:15:29.000000 nobuco-0.5.3/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9538 2023-06-19 13:43:03.000000 nobuco-0.5.3/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-05-17 10:46:04.000000 nobuco-0.5.3/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6244 2023-06-19 13:24:40.000000 nobuco-0.5.3/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11297 2023-06-19 20:07:28.000000 nobuco-0.5.3/nobuco/node_converters/tensor_manipulation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-06-06 21:33:32.000000 nobuco-0.5.3/nobuco/node_converters/tensor_shape.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      452 2023-06-19 20:13:01.000000 nobuco-0.5.3/nobuco/node_converters/torchvision.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 21:45:24.893394 nobuco-0.5.3/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-06-06 19:21:15.000000 nobuco-0.5.3/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10039 2023-06-09 15:11:00.000000 nobuco-0.5.3/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 21:45:24.893394 nobuco-0.5.3/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 21:45:24.885394 nobuco-0.5.3/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22244 2023-06-19 21:45:24.000000 nobuco-0.5.3/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1702 2023-06-19 21:45:24.000000 nobuco-0.5.3/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-19 21:45:24.000000 nobuco-0.5.3/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-06-19 21:45:24.000000 nobuco-0.5.3/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-06-19 21:45:24.000000 nobuco-0.5.3/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-06-19 21:44:16.000000 nobuco-0.5.3/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-19 21:45:24.893394 nobuco-0.5.3/setup.cfg
```

### Comparing `nobuco-0.5.2/LICENSE` & `nobuco-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/PKG-INFO` & `nobuco-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.5.2
+Version: 0.5.3
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nobuco-0.5.2/README.md` & `nobuco-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/__init__.py` & `nobuco-0.5.3/nobuco/__init__.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/commons.py` & `nobuco-0.5.3/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/convert.py` & `nobuco-0.5.3/nobuco/convert.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/converters/channel_ordering.py` & `nobuco-0.5.3/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/converters/node_converter.py` & `nobuco-0.5.3/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/converters/tensor.py` & `nobuco-0.5.3/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/converters/type_cast.py` & `nobuco-0.5.3/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/converters/validation.py` & `nobuco-0.5.3/nobuco/converters/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import traceback
 import warnings
 from enum import Enum
 import math
 
 import torch
 
 from nobuco.commons import ChannelOrder, TF_TENSOR_CLASSES
@@ -58,14 +59,15 @@
         if diff > tolerance or math.isnan(diff):
             return diff, ValidationStatus.INACCURATE
         else:
             return diff, ValidationStatus.SUCCESS
     except Exception as e:
         # raise Exception(f"Validation exception on node '{op_type.__name__}': {e}")
         warnings.warn(f"Validation exception on node '{op_type.__name__}': {e}")
+        traceback.print_exc()
         return None, ValidationStatus.FAIL
 
 
 def validate_diff_default(keras_op, pytorch_op, args_pt, kwargs_pt, outputs_pt, is_training=False):
     args_tf = pytorch2keras_recursively(args_pt, channel_order=ChannelOrder.TENSORFLOW)
     kwargs_tf = pytorch2keras_recursively(kwargs_pt, channel_order=ChannelOrder.TENSORFLOW)
```

### Comparing `nobuco-0.5.2/nobuco/entity/keras.py` & `nobuco-0.5.3/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/entity/pytorch.py` & `nobuco-0.5.3/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/funcs.py` & `nobuco-0.5.3/nobuco/funcs.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/layers/channel_order.py` & `nobuco-0.5.3/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/layers/container.py` & `nobuco-0.5.3/nobuco/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/layers/weight.py` & `nobuco-0.5.3/nobuco/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/locate/link.py` & `nobuco-0.5.3/nobuco/locate/link.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/locate/locate.py` & `nobuco-0.5.3/nobuco/locate/locate.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/node_converters/activation.py` & `nobuco-0.5.3/nobuco/node_converters/activation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/node_converters/attention.py` & `nobuco-0.5.3/nobuco/node_converters/attention.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/node_converters/boolean.py` & `nobuco-0.5.3/nobuco/node_converters/boolean.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/node_converters/boolean_mask.py` & `nobuco-0.5.3/nobuco/node_converters/boolean_mask.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/node_converters/comparison.py` & `nobuco-0.5.3/nobuco/node_converters/comparison.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/node_converters/convolution.py` & `nobuco-0.5.3/nobuco/node_converters/convolution.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/node_converters/dropout.py` & `nobuco-0.5.3/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/node_converters/interpolation.py` & `nobuco-0.5.3/nobuco/node_converters/interpolation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/node_converters/linear.py` & `nobuco-0.5.3/nobuco/node_converters/linear.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/node_converters/math.py` & `nobuco-0.5.3/nobuco/node_converters/math.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/node_converters/misc.py` & `nobuco-0.5.3/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/node_converters/normalization.py` & `nobuco-0.5.3/nobuco/node_converters/normalization.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional, Union, List, Tuple, Sequence, Any
 
 from torch import Tensor
 
+import tensorflow as tf
 from tensorflow import keras
 import torch
 import torch.nn.functional as F
 from torch import nn
 
 from nobuco.commons import ChannelOrder, ChannelOrderingStrategy
 from nobuco.converters.node_converter import converter
```

### Comparing `nobuco-0.5.2/nobuco/node_converters/padding.py` & `nobuco-0.5.3/nobuco/node_converters/padding.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/node_converters/pooling.py` & `nobuco-0.5.3/nobuco/node_converters/pooling.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,20 +58,21 @@
         return keras.layers.AvgPool2D(pool_size=kernel_size, strides=stride)(input)
     return func
 
 
 @converter(F.adaptive_avg_pool2d)
 def converter_adaptiveAvgPool2D(input: Tensor, output_size):
     if output_size == (1, 1) or output_size == 1:
-        pool_size = input.shape[2:]
         def func(input, output_size):
-            return keras.layers.AvgPool2D(pool_size=pool_size)(input)
-        return func
+            return keras.layers.GlobalAvgPool2D(keepdims=True)(input)
     else:
-        raise Exception('Unsupported parameters for adaptive_avg_pool2d')
+        def func(input, output_size):
+            import tensorflow_addons as tfa
+            return tfa.layers.AdaptiveAveragePooling2D(output_size=output_size)(input)
+    return func
 
 
 @converter(F.pixel_shuffle)
 def converter_pixel_shuffle(input: Tensor, upscale_factor: _int):
     def func(input, upscale_factor):
         x = input
         x = tf.concat([x[..., i::upscale_factor**2] for i in range(upscale_factor**2)], axis=-1)
```

### Comparing `nobuco-0.5.2/nobuco/node_converters/recurrent.py` & `nobuco-0.5.3/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/node_converters/slice.py` & `nobuco-0.5.3/nobuco/node_converters/slice.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/node_converters/tensor_cast.py` & `nobuco-0.5.3/nobuco/node_converters/tensor_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/node_converters/tensor_creation.py` & `nobuco-0.5.3/nobuco/node_converters/tensor_creation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.5.3/nobuco/node_converters/tensor_manipulation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/trace/tensor_storage.py` & `nobuco-0.5.3/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/trace/trace.py` & `nobuco-0.5.3/nobuco/trace/trace.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/util.py` & `nobuco-0.5.3/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/vis/console_stylizer.py` & `nobuco-0.5.3/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco/vis/html_stylizer.py` & `nobuco-0.5.3/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/nobuco.egg-info/PKG-INFO` & `nobuco-0.5.3/nobuco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.5.2
+Version: 0.5.3
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nobuco-0.5.2/nobuco.egg-info/SOURCES.txt` & `nobuco-0.5.3/nobuco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.2/pyproject.toml` & `nobuco-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.5.2"
+version = "0.5.3"
 description = "Pytorch to Tensorflow conversion made somewhat easy"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

