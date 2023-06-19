# Comparing `tmp/tonpay-0.0.1.tar.gz` & `tmp/tonpay-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonpay-0.0.1.tar", last modified: Fri Jun 16 11:39:33 2023, max compression
+gzip compressed data, was "tonpay-0.0.2.tar", last modified: Mon Jun 19 06:36:50 2023, max compression
```

## Comparing `tonpay-0.0.1.tar` & `tonpay-0.0.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-16 11:39:33.980601 tonpay-0.0.1/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1063 2023-05-27 08:05:57.000000 tonpay-0.0.1/LICENSE
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     2051 2023-06-16 11:39:33.980601 tonpay-0.0.1/PKG-INFO
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)       42 2023-05-27 08:05:57.000000 tonpay-0.0.1/README.md
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)      956 2023-06-16 11:28:16.000000 tonpay-0.0.1/pyproject.toml
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)       38 2023-06-16 11:39:33.980601 tonpay-0.0.1/setup.cfg
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-16 11:39:33.963934 tonpay-0.0.1/tonpay/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1195 2023-06-15 14:58:44.000000 tonpay-0.0.1/tonpay/__init__.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)       84 2023-06-07 15:00:17.000000 tonpay-0.0.1/tonpay/constants.py
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-16 11:39:33.967267 tonpay-0.0.1/tonpay/contracts/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)        0 2023-06-06 12:43:24.000000 tonpay-0.0.1/tonpay/contracts/__init__.py
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-16 11:39:33.970601 tonpay-0.0.1/tonpay/contracts/invoice/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)      274 2023-06-15 12:09:13.000000 tonpay-0.0.1/tonpay/contracts/invoice/__init__.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     6838 2023-06-15 14:52:29.000000 tonpay-0.0.1/tonpay/contracts/invoice/_code.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     6284 2023-06-16 11:06:03.000000 tonpay-0.0.1/tonpay/contracts/invoice/_contract.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1293 2023-06-15 13:39:25.000000 tonpay-0.0.1/tonpay/contracts/invoice/_deeplink.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     8046 2023-06-15 13:40:48.000000 tonpay-0.0.1/tonpay/contracts/invoice/_invoice.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     3015 2023-06-15 15:33:09.000000 tonpay-0.0.1/tonpay/contracts/invoice/_messages.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)      187 2023-06-11 10:38:34.000000 tonpay-0.0.1/tonpay/contracts/invoice/_opcodes.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     2044 2023-06-15 05:17:34.000000 tonpay-0.0.1/tonpay/contracts/invoice/_types.py
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-16 11:39:33.970601 tonpay-0.0.1/tonpay/contracts/jetton_wallet/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)       92 2023-06-15 11:50:22.000000 tonpay-0.0.1/tonpay/contracts/jetton_wallet/__init__.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)      901 2023-06-16 09:20:10.000000 tonpay-0.0.1/tonpay/contracts/jetton_wallet/_messages.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)       98 2023-06-14 10:54:19.000000 tonpay-0.0.1/tonpay/contracts/jetton_wallet/_opcodes.py
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-16 11:39:33.977267 tonpay-0.0.1/tonpay/contracts/store/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)      270 2023-06-15 12:10:13.000000 tonpay-0.0.1/tonpay/contracts/store/__init__.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     4333 2023-06-15 14:27:18.000000 tonpay-0.0.1/tonpay/contracts/store/_code.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     3879 2023-06-15 15:35:38.000000 tonpay-0.0.1/tonpay/contracts/store/_contract.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     2790 2023-06-15 13:40:04.000000 tonpay-0.0.1/tonpay/contracts/store/_deeplink.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     4872 2023-06-15 15:32:36.000000 tonpay-0.0.1/tonpay/contracts/store/_messages.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)      354 2023-06-14 14:44:53.000000 tonpay-0.0.1/tonpay/contracts/store/_opcodes.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)    12114 2023-06-16 11:14:24.000000 tonpay-0.0.1/tonpay/contracts/store/_store.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     2074 2023-06-15 12:09:13.000000 tonpay-0.0.1/tonpay/contracts/store/_types.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     9071 2023-06-16 10:46:08.000000 tonpay-0.0.1/tonpay/currency.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)      179 2023-06-16 10:09:37.000000 tonpay-0.0.1/tonpay/enums.py
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-16 11:39:33.977267 tonpay-0.0.1/tonpay/network/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)       28 2023-06-15 11:39:34.000000 tonpay-0.0.1/tonpay/network/__init__.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)      433 2023-06-12 09:43:21.000000 tonpay-0.0.1/tonpay/network/_sender.py
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-16 11:39:33.977267 tonpay-0.0.1/tonpay/utils/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)       72 2023-06-15 15:29:32.000000 tonpay-0.0.1/tonpay/utils/__init__.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1536 2023-06-15 15:29:32.000000 tonpay-0.0.1/tonpay/utils/_strings.py
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-16 11:39:33.977267 tonpay-0.0.1/tonpay/utils/deeplink/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)      130 2023-06-15 13:40:48.000000 tonpay-0.0.1/tonpay/utils/deeplink/__init__.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1410 2023-06-15 15:17:59.000000 tonpay-0.0.1/tonpay/utils/deeplink/_ton.py
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-16 11:39:33.980601 tonpay-0.0.1/tonpay/utils/ton_access/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)       61 2023-06-15 10:23:52.000000 tonpay-0.0.1/tonpay/utils/ton_access/__init__.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     3518 2023-06-15 14:25:21.000000 tonpay-0.0.1/tonpay/utils/ton_access/_access.py
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1563 2023-06-15 14:12:45.000000 tonpay-0.0.1/tonpay/utils/ton_access/_node.py
-drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-16 11:39:33.967267 tonpay-0.0.1/tonpay.egg-info/
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     2051 2023-06-16 11:39:33.000000 tonpay-0.0.1/tonpay.egg-info/PKG-INFO
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1226 2023-06-16 11:39:33.000000 tonpay-0.0.1/tonpay.egg-info/SOURCES.txt
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)        1 2023-06-16 11:39:33.000000 tonpay-0.0.1/tonpay.egg-info/dependency_links.txt
--rw-r--r--   0 arterialist  (1000) arterialist  (1000)        7 2023-06-16 11:39:33.000000 tonpay-0.0.1/tonpay.egg-info/top_level.txt
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.348395 tonpay-0.0.2/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1063 2023-05-27 08:05:57.000000 tonpay-0.0.2/LICENSE
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     2051 2023-06-19 06:36:50.348395 tonpay-0.0.2/PKG-INFO
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)       42 2023-05-27 08:05:57.000000 tonpay-0.0.2/README.md
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)      956 2023-06-19 06:36:08.000000 tonpay-0.0.2/pyproject.toml
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)       38 2023-06-19 06:36:50.348395 tonpay-0.0.2/setup.cfg
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.338395 tonpay-0.0.2/tonpay/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1195 2023-06-15 14:58:44.000000 tonpay-0.0.2/tonpay/__init__.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)       84 2023-06-07 15:00:17.000000 tonpay-0.0.2/tonpay/constants.py
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.341729 tonpay-0.0.2/tonpay/contracts/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)        0 2023-06-06 12:43:24.000000 tonpay-0.0.2/tonpay/contracts/__init__.py
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.341729 tonpay-0.0.2/tonpay/contracts/invoice/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)      274 2023-06-15 12:09:13.000000 tonpay-0.0.2/tonpay/contracts/invoice/__init__.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     6838 2023-06-15 14:52:29.000000 tonpay-0.0.2/tonpay/contracts/invoice/_code.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     6284 2023-06-16 11:06:03.000000 tonpay-0.0.2/tonpay/contracts/invoice/_contract.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1293 2023-06-15 13:39:25.000000 tonpay-0.0.2/tonpay/contracts/invoice/_deeplink.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     8046 2023-06-15 13:40:48.000000 tonpay-0.0.2/tonpay/contracts/invoice/_invoice.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     3015 2023-06-15 15:33:09.000000 tonpay-0.0.2/tonpay/contracts/invoice/_messages.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)      187 2023-06-11 10:38:34.000000 tonpay-0.0.2/tonpay/contracts/invoice/_opcodes.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     2044 2023-06-15 05:17:34.000000 tonpay-0.0.2/tonpay/contracts/invoice/_types.py
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.341729 tonpay-0.0.2/tonpay/contracts/jetton_wallet/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)       92 2023-06-15 11:50:22.000000 tonpay-0.0.2/tonpay/contracts/jetton_wallet/__init__.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)      901 2023-06-16 09:20:10.000000 tonpay-0.0.2/tonpay/contracts/jetton_wallet/_messages.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)       98 2023-06-14 10:54:19.000000 tonpay-0.0.2/tonpay/contracts/jetton_wallet/_opcodes.py
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.345062 tonpay-0.0.2/tonpay/contracts/store/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)      270 2023-06-15 12:10:13.000000 tonpay-0.0.2/tonpay/contracts/store/__init__.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     4333 2023-06-15 14:27:18.000000 tonpay-0.0.2/tonpay/contracts/store/_code.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     3879 2023-06-15 15:35:38.000000 tonpay-0.0.2/tonpay/contracts/store/_contract.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     2790 2023-06-15 13:40:04.000000 tonpay-0.0.2/tonpay/contracts/store/_deeplink.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     4872 2023-06-15 15:32:36.000000 tonpay-0.0.2/tonpay/contracts/store/_messages.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)      354 2023-06-14 14:44:53.000000 tonpay-0.0.2/tonpay/contracts/store/_opcodes.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)    12108 2023-06-19 06:35:34.000000 tonpay-0.0.2/tonpay/contracts/store/_store.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     2074 2023-06-15 12:09:13.000000 tonpay-0.0.2/tonpay/contracts/store/_types.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     9021 2023-06-17 09:28:12.000000 tonpay-0.0.2/tonpay/currency.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)      179 2023-06-16 10:09:37.000000 tonpay-0.0.2/tonpay/enums.py
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.345062 tonpay-0.0.2/tonpay/network/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)       28 2023-06-15 11:39:34.000000 tonpay-0.0.2/tonpay/network/__init__.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)      433 2023-06-12 09:43:21.000000 tonpay-0.0.2/tonpay/network/_sender.py
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.345062 tonpay-0.0.2/tonpay/utils/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)       72 2023-06-15 15:29:32.000000 tonpay-0.0.2/tonpay/utils/__init__.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1536 2023-06-15 15:29:32.000000 tonpay-0.0.2/tonpay/utils/_strings.py
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.345062 tonpay-0.0.2/tonpay/utils/deeplink/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)      130 2023-06-15 13:40:48.000000 tonpay-0.0.2/tonpay/utils/deeplink/__init__.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1410 2023-06-15 15:17:59.000000 tonpay-0.0.2/tonpay/utils/deeplink/_ton.py
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.348395 tonpay-0.0.2/tonpay/utils/ton_access/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)       61 2023-06-15 10:23:52.000000 tonpay-0.0.2/tonpay/utils/ton_access/__init__.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     3518 2023-06-15 14:25:21.000000 tonpay-0.0.2/tonpay/utils/ton_access/_access.py
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1563 2023-06-15 14:12:45.000000 tonpay-0.0.2/tonpay/utils/ton_access/_node.py
+drwxr-xr-x   0 arterialist  (1000) arterialist  (1000)        0 2023-06-19 06:36:50.341729 tonpay-0.0.2/tonpay.egg-info/
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     2051 2023-06-19 06:36:50.000000 tonpay-0.0.2/tonpay.egg-info/PKG-INFO
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)     1226 2023-06-19 06:36:50.000000 tonpay-0.0.2/tonpay.egg-info/SOURCES.txt
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)        1 2023-06-19 06:36:50.000000 tonpay-0.0.2/tonpay.egg-info/dependency_links.txt
+-rw-r--r--   0 arterialist  (1000) arterialist  (1000)        7 2023-06-19 06:36:50.000000 tonpay-0.0.2/tonpay.egg-info/top_level.txt
```

### Comparing `tonpay-0.0.1/LICENSE` & `tonpay-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.1/PKG-INFO` & `tonpay-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonpay
-Version: 0.0.1
+Version: 0.0.2
 Summary: SDK for crypto payment system Tonpay
 Author-email: Arterialist <arterialist@thetonpay.app>
 License: MIT License
         
         Copyright (c) 2023 Tonpay
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tonpay-0.0.1/pyproject.toml` & `tonpay-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "tonpay"
 description = "SDK for crypto payment system Tonpay"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "Arterialist", email = "arterialist@thetonpay.app" }
 ]
 dependencies = []
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `tonpay-0.0.1/tonpay/__init__.py` & `tonpay-0.0.2/tonpay/__init__.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.1/tonpay/contracts/invoice/_code.py` & `tonpay-0.0.2/tonpay/contracts/invoice/_code.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.1/tonpay/contracts/invoice/_contract.py` & `tonpay-0.0.2/tonpay/contracts/invoice/_contract.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.1/tonpay/contracts/invoice/_deeplink.py` & `tonpay-0.0.2/tonpay/contracts/invoice/_deeplink.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.1/tonpay/contracts/invoice/_invoice.py` & `tonpay-0.0.2/tonpay/contracts/invoice/_invoice.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.1/tonpay/contracts/invoice/_messages.py` & `tonpay-0.0.2/tonpay/contracts/invoice/_messages.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.1/tonpay/contracts/invoice/_types.py` & `tonpay-0.0.2/tonpay/contracts/invoice/_types.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.1/tonpay/contracts/jetton_wallet/_messages.py` & `tonpay-0.0.2/tonpay/contracts/jetton_wallet/_messages.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.1/tonpay/contracts/store/_code.py` & `tonpay-0.0.2/tonpay/contracts/store/_code.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.1/tonpay/contracts/store/_contract.py` & `tonpay-0.0.2/tonpay/contracts/store/_contract.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.1/tonpay/contracts/store/_deeplink.py` & `tonpay-0.0.2/tonpay/contracts/store/_deeplink.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.1/tonpay/contracts/store/_messages.py` & `tonpay-0.0.2/tonpay/contracts/store/_messages.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.1/tonpay/contracts/store/_store.py` & `tonpay-0.0.2/tonpay/contracts/store/_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         self._sender = sender
         self._client = client
         self._wrapper = StoreContract(address=address, client=client)
 
     def get_address(self):
         return self.address
 
-    async def edit_store(self, name: str, description: str, image: str, webhook: str, mcc_code: int):
+    async def edit(self, name: str, description: str, image: str, webhook: str, mcc_code: int):
         """
         This method edits the store data
 
         :param name: New store name
         :param description: New store description
         :param image: New store image URL
         :param webhook: New store webhook URL
```

### Comparing `tonpay-0.0.1/tonpay/contracts/store/_types.py` & `tonpay-0.0.2/tonpay/contracts/store/_types.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.1/tonpay/currency.py` & `tonpay-0.0.2/tonpay/currency.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-import base64
-
-from tonsdk.boc import begin_cell
-
 from tonpay.constants import ZERO_ADDRESS
 
 BRIDGE_WALLET = "te6cckECEwEAA4UAART/APSkE/S88sgLAQIBYgIDAgLLBAUAG6D2BdqJofQB9IH0gamjAgHOBgcCAVgKCwL3CDHAJJfBOAB0NMDAXGwlRNfA/Ad4PpA+kAx+gAxcdch+gAx+gAwc6m0AALTHwHbPFsyNDQ0JIIQD4p+pbqaMGwiNl4xECPwGuAkghAXjUUZupswbCJeMhAkQwDwG+A3WzaCEFlfB7y6nwJxsPLSwFAjuvLixgHwHOBfBYAgJABE+kQwwADy4U2AAXIBP+DMgbpUwgLH4M94gbvLSmtDTBzHT/9P/9ATTB9Qw0PoA+gD6APoA+gD6ADAACIQP8vACAVgMDQIBSBESAfcBdM/AQH6APpAIfAB7UTQ+gD6QPpA1NFRNqFSLMcF8uLBKsL/8uLCVDRCcFQgE1QUA8hQBPoCWM8WAc8WzMkiyMsBEvQA9ADLAMkgcAH5AHTIywISygfL/8nQBPpA9AQx+gAg10nCAPLixMiAGAHLBVAHzxZw+gJ3ActrgDgLzO1E0PoA+kD6QNTRCtM/AQH6AFFRoAX6QPpAU13HBVRzb3BUIBNUFAPIUAT6AljPFgHPFszJIsjLARL0APQAywDJcAH5AHTIywISygfL/8nQUA/HBR6x8uLDDPoAUcqhKbYIGaFQB6AYoSaSbFXjDSXXCwHDACHCALCAPEACqE8zIghAXjUUZWAoCyx/LP1AH+gIizxZQBs8WJfoCUAPPFslQBcwjkXKRceJQB6gToAiqAFAEoBegFLzy4sUByYBA+wBDAMhQBPoCWM8WAc8WzMntVAByUmmgGKHIghBzYtCcKQLLH8s/UAf6AlAEzxZQB88WyciAEAHLBSfPFlAE+gJxActqE8zJcfsAUEITAHSOI8iAEAHLBVAGzxZQBfoCcAHLaoIQ1TJ221gFAssfyz/JcvsAklsz4kADyFAE+gJYzxYBzxbMye1UAOs7UTQ+gD6QPpA1NEF0z8BAfoAIcIA8uLC+kD0BAHQ05/RAdFRYqFSWMcF8uLBJsL/8uLCyIIQe92X3lgEAssfyz8B+gIjzxYBzxYTy5/JyIAYAcsFI88WcPoCcQHLaszJgED7AEATyFAE+gJYzxYBzxbMye1UgAIcgCDXIe1E0PoA+kD6QNTRBNMfAYQPIYIQF41FGboCghB73ZfeuhKx8vTTPwEw+gAwE6BQI8hQBPoCWM8WAc8WzMntVINjFu1o=";
 
 BOLT_WALLET = "te6cckECEQEAAxcAART/APSkE/S88sgLAQIBYgIDAgLMBAUAG6D2BdqJofQB9IH0gahhAgEgBgcCASAICQC30QY4B5IADoaYGAuNhKia+B+AZwfSB9IBj9ABi465D9ABj9ABgBaY/BCAfFP1KpEF1KmJos+ATwQQgLxqKMqRBdSxiZoBn4BXAawQgsr4PeXUms+AXwL4JCB/l4QAEWvpEMHC68uFNgIBIAoLAIPUAQa5D2omh9AH0gfSBqGAJpj8EIC8aijKkQXUEIPe7L7wndCVj5cWLpn5j9ABgJ0CgR5CgCfQEsZ4sA54tmZPaqQB9VA9M/+gD6QCHwBu1E0PoA+kD6QNQwUTahUirHBfLiwSjC//LiwlQ0QnBUIBNUFAPIUAT6AljPFgHPFszJIsjLARL0APQAywDJIPkAcHTIywLKB8v/ydAE+kD0BDH6AHeAGMjLBVAIzxZw+gIXy2sTzIIQF41FGcjLHxmAwCASANDgCOyz9QB/oCIs8WUAbPFiX6AlADzxbJUAXMB6oAE6CCCJiWgKoAggiYloCgoBS88uLFBMmAQPsAECPIUAT6AljPFgHPFszJ7VQC8TtRND6APpA+kDUMAfTP/oAUVGgBfpA+kBTWscFVHNscFQgE1QUA8hQBPoCWM8WAc8WzMkiyMsBEvQA9ADLAMn5AHB0yMsCygfL/8nQUAzHBRux8uLDCfoAggiYloCCCJiWgKAaoSGVEEk4XwTjDSXXCwHDACTCALCAPEADbO1E0PoA+kD6QNQwB9M/+gD6QDBRUaFSSccF8uLBJ8L/8uLCggiYloCqABagFrzy4sOCEHvdl97Iyx8Vyz9QA/oCIs8WAc8WyXGAEMjLBSTPFnD6AstqzMmAQPsAQBPIUAT6AljPFgHPFszJ7VSAAbFIZoBihghBzYtCcyMsfUkDLP1AD+gIBzxZQB88WyXGAGMjLBSXPFlAH+gIWy2oVzMlx+wAQNACCjiqCCJiWgHL7AoIQ1TJ223CAEMjLBVAIzxZQBfoCFstqE8sfE8s/yXL7AFiSbDPiVQLIUAT6AljPFgHPFszJ7VSoVpbw";
 
 DEFAULT_WALLET = "te6cckECEQEAAyMAART/APSkE/S88sgLAQIBYgIDAgLMBAUAG6D2BdqJofQB9IH0gahhAgHUBgcCASAICQDDCDHAJJfBOAB0NMDAXGwlRNfA/AM4PpA+kAx+gAxcdch+gAx+gAwc6m0AALTH4IQD4p+pVIgupUxNFnwCeCCEBeNRRlSILqWMUREA/AK4DWCEFlfB7y6k1nwC+BfBIQP8vCAAET6RDBwuvLhTYAIBIAoLAIPUAQa5D2omh9AH0gfSBqGAJpj8EIC8aijKkQXUEIPe7L7wndCVj5cWLpn5j9ABgJ0CgR5CgCfQEsZ4sA54tmZPaqQB8VA9M/+gD6QCHwAe1E0PoA+kD6QNQwUTahUirHBfLiwSjC//LiwlQ0QnBUIBNUFAPIUAT6AljPFgHPFszJIsjLARL0APQAywDJIPkAcHTIywLKB8v/ydAE+kD0BDH6ACDXScIA8uLEd4AYyMsFUAjPFnD6AhfLaxPMgMAgEgDQ4AnoIQF41FGcjLHxnLP1AH+gIizxZQBs8WJfoCUAPPFslQBcwjkXKRceJQCKgToIIJycOAoBS88uLFBMmAQPsAECPIUAT6AljPFgHPFszJ7VQC9ztRND6APpA+kDUMAjTP/oAUVGgBfpA+kBTW8cFVHNtcFQgE1QUA8hQBPoCWM8WAc8WzMkiyMsBEvQA9ADLAMn5AHB0yMsCygfL/8nQUA3HBRyx8uLDCvoAUaihggiYloBmtgihggiYloCgGKEnlxBJEDg3XwTjDSXXCwGAPEADXO1E0PoA+kD6QNQwB9M/+gD6QDBRUaFSSccF8uLBJ8L/8uLCBYIJMS0AoBa88uLDghB73ZfeyMsfFcs/UAP6AiLPFgHPFslxgBjIywUkzxZw+gLLaszJgED7AEATyFAE+gJYzxYBzxbMye1UgAHBSeaAYoYIQc2LQnMjLH1Iwyz9Y+gJQB88WUAfPFslxgBDIywUkzxZQBvoCFctqFMzJcfsAECQQIwB8wwAjwgCwjiGCENUydttwgBDIywVQCM8WUAT6AhbLahLLHxLLP8ly+wCTNWwh4gPIUAT6AljPFgHPFszJ7VSV6u3X";
```

### Comparing `tonpay-0.0.1/tonpay/utils/_strings.py` & `tonpay-0.0.2/tonpay/utils/_strings.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.1/tonpay/utils/deeplink/_ton.py` & `tonpay-0.0.2/tonpay/utils/deeplink/_ton.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.1/tonpay/utils/ton_access/_access.py` & `tonpay-0.0.2/tonpay/utils/ton_access/_access.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.1/tonpay/utils/ton_access/_node.py` & `tonpay-0.0.2/tonpay/utils/ton_access/_node.py`

 * *Files identical despite different names*

### Comparing `tonpay-0.0.1/tonpay.egg-info/PKG-INFO` & `tonpay-0.0.2/tonpay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonpay
-Version: 0.0.1
+Version: 0.0.2
 Summary: SDK for crypto payment system Tonpay
 Author-email: Arterialist <arterialist@thetonpay.app>
 License: MIT License
         
         Copyright (c) 2023 Tonpay
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tonpay-0.0.1/tonpay.egg-info/SOURCES.txt` & `tonpay-0.0.2/tonpay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

