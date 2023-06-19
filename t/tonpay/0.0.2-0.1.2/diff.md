# Comparing `tmp/tonpay-0.0.2.tar.gz` & `tmp/tonpay-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonpay-0.0.2.tar", last modified: Mon Jun 19 06:36:50 2023, max compression
+gzip compressed data, was "tonpay-0.1.2.tar", last modified: Mon Jun 19 10:29:17 2023, max compression
```

## Comparing `tonpay-0.0.2.tar` & `tonpay-0.1.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.348395 tonpay-0.0.2/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1063 2023-05-27 08:05:57.000000 tonpay-0.0.2/LICENSE
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     2051 2023-06-19 06:36:50.348395 tonpay-0.0.2/PKG-INFO
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)       42 2023-05-27 08:05:57.000000 tonpay-0.0.2/README.md
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)      956 2023-06-19 06:36:08.000000 tonpay-0.0.2/pyproject.toml
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)       38 2023-06-19 06:36:50.348395 tonpay-0.0.2/setup.cfg
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.338395 tonpay-0.0.2/tonpay/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1195 2023-06-15 14:58:44.000000 tonpay-0.0.2/tonpay/__init__.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)       84 2023-06-07 15:00:17.000000 tonpay-0.0.2/tonpay/constants.py
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.341729 tonpay-0.0.2/tonpay/contracts/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)        0 2023-06-06 12:43:24.000000 tonpay-0.0.2/tonpay/contracts/__init__.py
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.341729 tonpay-0.0.2/tonpay/contracts/invoice/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)      274 2023-06-15 12:09:13.000000 tonpay-0.0.2/tonpay/contracts/invoice/__init__.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     6838 2023-06-15 14:52:29.000000 tonpay-0.0.2/tonpay/contracts/invoice/_code.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     6284 2023-06-16 11:06:03.000000 tonpay-0.0.2/tonpay/contracts/invoice/_contract.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1293 2023-06-15 13:39:25.000000 tonpay-0.0.2/tonpay/contracts/invoice/_deeplink.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     8046 2023-06-15 13:40:48.000000 tonpay-0.0.2/tonpay/contracts/invoice/_invoice.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     3015 2023-06-15 15:33:09.000000 tonpay-0.0.2/tonpay/contracts/invoice/_messages.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)      187 2023-06-11 10:38:34.000000 tonpay-0.0.2/tonpay/contracts/invoice/_opcodes.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     2044 2023-06-15 05:17:34.000000 tonpay-0.0.2/tonpay/contracts/invoice/_types.py
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.341729 tonpay-0.0.2/tonpay/contracts/jetton_wallet/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)       92 2023-06-15 11:50:22.000000 tonpay-0.0.2/tonpay/contracts/jetton_wallet/__init__.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)      901 2023-06-16 09:20:10.000000 tonpay-0.0.2/tonpay/contracts/jetton_wallet/_messages.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)       98 2023-06-14 10:54:19.000000 tonpay-0.0.2/tonpay/contracts/jetton_wallet/_opcodes.py
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.345062 tonpay-0.0.2/tonpay/contracts/store/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)      270 2023-06-15 12:10:13.000000 tonpay-0.0.2/tonpay/contracts/store/__init__.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     4333 2023-06-15 14:27:18.000000 tonpay-0.0.2/tonpay/contracts/store/_code.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     3879 2023-06-15 15:35:38.000000 tonpay-0.0.2/tonpay/contracts/store/_contract.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     2790 2023-06-15 13:40:04.000000 tonpay-0.0.2/tonpay/contracts/store/_deeplink.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     4872 2023-06-15 15:32:36.000000 tonpay-0.0.2/tonpay/contracts/store/_messages.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)      354 2023-06-14 14:44:53.000000 tonpay-0.0.2/tonpay/contracts/store/_opcodes.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)    12108 2023-06-19 06:35:34.000000 tonpay-0.0.2/tonpay/contracts/store/_store.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     2074 2023-06-15 12:09:13.000000 tonpay-0.0.2/tonpay/contracts/store/_types.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     9021 2023-06-17 09:28:12.000000 tonpay-0.0.2/tonpay/currency.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)      179 2023-06-16 10:09:37.000000 tonpay-0.0.2/tonpay/enums.py
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.345062 tonpay-0.0.2/tonpay/network/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)       28 2023-06-15 11:39:34.000000 tonpay-0.0.2/tonpay/network/__init__.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)      433 2023-06-12 09:43:21.000000 tonpay-0.0.2/tonpay/network/_sender.py
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.345062 tonpay-0.0.2/tonpay/utils/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)       72 2023-06-15 15:29:32.000000 tonpay-0.0.2/tonpay/utils/__init__.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1536 2023-06-15 15:29:32.000000 tonpay-0.0.2/tonpay/utils/_strings.py
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.345062 tonpay-0.0.2/tonpay/utils/deeplink/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)      130 2023-06-15 13:40:48.000000 tonpay-0.0.2/tonpay/utils/deeplink/__init__.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1410 2023-06-15 15:17:59.000000 tonpay-0.0.2/tonpay/utils/deeplink/_ton.py
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.348395 tonpay-0.0.2/tonpay/utils/ton_access/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)       61 2023-06-15 10:23:52.000000 tonpay-0.0.2/tonpay/utils/ton_access/__init__.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     3518 2023-06-15 14:25:21.000000 tonpay-0.0.2/tonpay/utils/ton_access/_access.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1563 2023-06-15 14:12:45.000000 tonpay-0.0.2/tonpay/utils/ton_access/_node.py
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.341729 tonpay-0.0.2/tonpay.egg-info/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     2051 2023-06-19 06:36:50.000000 tonpay-0.0.2/tonpay.egg-info/PKG-INFO
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1226 2023-06-19 06:36:50.000000 tonpay-0.0.2/tonpay.egg-info/SOURCES.txt
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)        1 2023-06-19 06:36:50.000000 tonpay-0.0.2/tonpay.egg-info/dependency_links.txt
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)        7 2023-06-19 06:36:50.000000 tonpay-0.0.2/tonpay.egg-info/top_level.txt
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 10:29:17.189149 tonpay-0.1.2/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1063 2023-05-27 08:05:57.000000 tonpay-0.1.2/LICENSE
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     2051 2023-06-19 10:29:17.189149 tonpay-0.1.2/PKG-INFO
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)       42 2023-05-27 08:05:57.000000 tonpay-0.1.2/README.md
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)      956 2023-06-19 10:28:49.000000 tonpay-0.1.2/pyproject.toml
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)       38 2023-06-19 10:29:17.189149 tonpay-0.1.2/setup.cfg
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 10:29:17.179149 tonpay-0.1.2/tonpay/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1195 2023-06-15 14:58:44.000000 tonpay-0.1.2/tonpay/__init__.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)       84 2023-06-07 15:00:17.000000 tonpay-0.1.2/tonpay/constants.py
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 10:29:17.182482 tonpay-0.1.2/tonpay/contracts/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)        0 2023-06-06 12:43:24.000000 tonpay-0.1.2/tonpay/contracts/__init__.py
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 10:29:17.182482 tonpay-0.1.2/tonpay/contracts/invoice/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)      274 2023-06-15 12:09:13.000000 tonpay-0.1.2/tonpay/contracts/invoice/__init__.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     6838 2023-06-15 14:52:29.000000 tonpay-0.1.2/tonpay/contracts/invoice/_code.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     6284 2023-06-16 11:06:03.000000 tonpay-0.1.2/tonpay/contracts/invoice/_contract.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1293 2023-06-15 13:39:25.000000 tonpay-0.1.2/tonpay/contracts/invoice/_deeplink.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     8046 2023-06-15 13:40:48.000000 tonpay-0.1.2/tonpay/contracts/invoice/_invoice.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     3015 2023-06-15 15:33:09.000000 tonpay-0.1.2/tonpay/contracts/invoice/_messages.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)      187 2023-06-11 10:38:34.000000 tonpay-0.1.2/tonpay/contracts/invoice/_opcodes.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     2044 2023-06-15 05:17:34.000000 tonpay-0.1.2/tonpay/contracts/invoice/_types.py
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 10:29:17.185815 tonpay-0.1.2/tonpay/contracts/jetton_wallet/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)       92 2023-06-15 11:50:22.000000 tonpay-0.1.2/tonpay/contracts/jetton_wallet/__init__.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)      901 2023-06-16 09:20:10.000000 tonpay-0.1.2/tonpay/contracts/jetton_wallet/_messages.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)       98 2023-06-14 10:54:19.000000 tonpay-0.1.2/tonpay/contracts/jetton_wallet/_opcodes.py
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 10:29:17.185815 tonpay-0.1.2/tonpay/contracts/store/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)      270 2023-06-15 12:10:13.000000 tonpay-0.1.2/tonpay/contracts/store/__init__.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     4333 2023-06-15 14:27:18.000000 tonpay-0.1.2/tonpay/contracts/store/_code.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     3879 2023-06-15 15:35:38.000000 tonpay-0.1.2/tonpay/contracts/store/_contract.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     2790 2023-06-15 13:40:04.000000 tonpay-0.1.2/tonpay/contracts/store/_deeplink.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     4872 2023-06-15 15:32:36.000000 tonpay-0.1.2/tonpay/contracts/store/_messages.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)      354 2023-06-14 14:44:53.000000 tonpay-0.1.2/tonpay/contracts/store/_opcodes.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)    13503 2023-06-19 08:01:37.000000 tonpay-0.1.2/tonpay/contracts/store/_store.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     2074 2023-06-15 12:09:13.000000 tonpay-0.1.2/tonpay/contracts/store/_types.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     9021 2023-06-17 09:28:12.000000 tonpay-0.1.2/tonpay/currency.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)      179 2023-06-16 10:09:37.000000 tonpay-0.1.2/tonpay/enums.py
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 10:29:17.189149 tonpay-0.1.2/tonpay/network/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)       28 2023-06-15 11:39:34.000000 tonpay-0.1.2/tonpay/network/__init__.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)      433 2023-06-12 09:43:21.000000 tonpay-0.1.2/tonpay/network/_sender.py
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 10:29:17.189149 tonpay-0.1.2/tonpay/utils/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)       72 2023-06-15 15:29:32.000000 tonpay-0.1.2/tonpay/utils/__init__.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1536 2023-06-15 15:29:32.000000 tonpay-0.1.2/tonpay/utils/_strings.py
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 10:29:17.189149 tonpay-0.1.2/tonpay/utils/deeplink/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)      130 2023-06-15 13:40:48.000000 tonpay-0.1.2/tonpay/utils/deeplink/__init__.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1410 2023-06-15 15:17:59.000000 tonpay-0.1.2/tonpay/utils/deeplink/_ton.py
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 10:29:17.189149 tonpay-0.1.2/tonpay/utils/ton_access/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)       61 2023-06-15 10:23:52.000000 tonpay-0.1.2/tonpay/utils/ton_access/__init__.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     3518 2023-06-15 14:25:21.000000 tonpay-0.1.2/tonpay/utils/ton_access/_access.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1563 2023-06-15 14:12:45.000000 tonpay-0.1.2/tonpay/utils/ton_access/_node.py
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 10:29:17.179149 tonpay-0.1.2/tonpay.egg-info/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     2051 2023-06-19 10:29:17.000000 tonpay-0.1.2/tonpay.egg-info/PKG-INFO
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1226 2023-06-19 10:29:17.000000 tonpay-0.1.2/tonpay.egg-info/SOURCES.txt
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)        1 2023-06-19 10:29:17.000000 tonpay-0.1.2/tonpay.egg-info/dependency_links.txt
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)        7 2023-06-19 10:29:17.000000 tonpay-0.1.2/tonpay.egg-info/top_level.txt
```

### Comparing `tonpay-0.0.2/LICENSE` & `tonpay-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.2/PKG-INFO` & `tonpay-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonpay
-Version: 0.0.2
+Version: 0.1.2
 Summary: SDK for crypto payment system Tonpay
 Author-email: Arterialist <arterialist@thetonpay.app>
 License: MIT License
         
         Copyright (c) 2023 Tonpay
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tonpay-0.0.2/pyproject.toml` & `tonpay-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "tonpay"
 description = "SDK for crypto payment system Tonpay"
-version = "0.0.2"
+version = "0.1.2"
 authors = [
     { name = "Arterialist", email = "arterialist@thetonpay.app" }
 ]
 dependencies = []
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `tonpay-0.0.2/tonpay/__init__.py` & `tonpay-0.1.2/tonpay/__init__.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.2/tonpay/contracts/invoice/_code.py` & `tonpay-0.1.2/tonpay/contracts/invoice/_code.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.2/tonpay/contracts/invoice/_contract.py` & `tonpay-0.1.2/tonpay/contracts/invoice/_contract.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.2/tonpay/contracts/invoice/_deeplink.py` & `tonpay-0.1.2/tonpay/contracts/invoice/_deeplink.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.2/tonpay/contracts/invoice/_invoice.py` & `tonpay-0.1.2/tonpay/contracts/invoice/_invoice.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.2/tonpay/contracts/invoice/_messages.py` & `tonpay-0.1.2/tonpay/contracts/invoice/_messages.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.2/tonpay/contracts/invoice/_types.py` & `tonpay-0.1.2/tonpay/contracts/invoice/_types.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.2/tonpay/contracts/jetton_wallet/_messages.py` & `tonpay-0.1.2/tonpay/contracts/jetton_wallet/_messages.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.2/tonpay/contracts/store/_code.py` & `tonpay-0.1.2/tonpay/contracts/store/_code.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.2/tonpay/contracts/store/_contract.py` & `tonpay-0.1.2/tonpay/contracts/store/_contract.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.2/tonpay/contracts/store/_deeplink.py` & `tonpay-0.1.2/tonpay/contracts/store/_deeplink.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.2/tonpay/contracts/store/_messages.py` & `tonpay-0.1.2/tonpay/contracts/store/_messages.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.2/tonpay/contracts/store/_store.py` & `tonpay-0.1.2/tonpay/contracts/store/_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,14 +261,48 @@
             invoice.amount,
             invoice.invoice_id,
             invoice.metadata,
             StoreFees.REQUEST_PURCHASE_JETTON,
             url_format
         )
 
+    async def get_purchase_request_invoice(self, invoice: PurchaseRequestInvoice):
+        if not invoice.invoice_id:
+            raise ValueError("Invoice ID is required")
+
+        if len(invoice.invoice_id) > 120:
+            raise ValueError("Invoice ID must not be longer than 120 characters")
+
+        if invoice.metadata and len(invoice.metadata) > 500:
+            raise ValueError("Metadata must not be longer than 500 characters")
+
+        if invoice.amount < 0:
+            raise ValueError("Amount must be greater than 0")
+
+        merchant_address = await self.get_owner()
+        return Invoice(
+            address=InvoiceContract(None, self._client, config=InvoiceConfig(
+                self.address,
+                merchant_address.to_string(True, True, True),
+                "EQD2wz8Rq5QDj9iK2Z_leGQu-Rup__y-Z4wo8Lm7-tSD6Iz2",
+                False,
+                Address(ZERO_ADDRESS).to_string(True, True, True),
+                invoice.invoice_id,
+                invoice.metadata,
+                invoice.amount * pow(10, invoice.currency.decimals),
+                False,
+                True,
+                True,
+                invoice.currency.address,
+                Cell.one_from_boc(base64.b64decode(invoice.currency.wallet_code))
+            )).address.to_string(True, True, True),
+            sender=self._sender,
+            client=self._client
+        )
+
     async def apply_update(self, new_data: Optional[Cell] = None):
         if not self._sender:
             raise Exception("This store is read-only. Pass the sender to the constructor to make changes.")
 
         await self._sender.send(
             StoreFees.FULL_UPGRADE,
             Address(self.address),
```

### Comparing `tonpay-0.0.2/tonpay/contracts/store/_types.py` & `tonpay-0.1.2/tonpay/contracts/store/_types.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.2/tonpay/currency.py` & `tonpay-0.1.2/tonpay/currency.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.2/tonpay/utils/_strings.py` & `tonpay-0.1.2/tonpay/utils/_strings.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.2/tonpay/utils/deeplink/_ton.py` & `tonpay-0.1.2/tonpay/utils/deeplink/_ton.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.2/tonpay/utils/ton_access/_access.py` & `tonpay-0.1.2/tonpay/utils/ton_access/_access.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.2/tonpay/utils/ton_access/_node.py` & `tonpay-0.1.2/tonpay/utils/ton_access/_node.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.2/tonpay.egg-info/PKG-INFO` & `tonpay-0.1.2/tonpay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonpay
-Version: 0.0.2
+Version: 0.1.2
 Summary: SDK for crypto payment system Tonpay
 Author-email: Arterialist <arterialist@thetonpay.app>
 License: MIT License
         
         Copyright (c) 2023 Tonpay
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tonpay-0.0.2/tonpay.egg-info/SOURCES.txt` & `tonpay-0.1.2/tonpay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

