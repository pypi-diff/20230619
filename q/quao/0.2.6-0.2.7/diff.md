# Comparing `tmp/quao-0.2.6.tar.gz` & `tmp/quao-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quao-0.2.6.tar", last modified: Fri Jun 16 09:14:00 2023, max compression
+gzip compressed data, was "quao-0.2.7.tar", last modified: Mon Jun 19 01:50:44 2023, max compression
```

## Comparing `quao-0.2.6.tar` & `quao-0.2.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 09:14:00.275891 quao-0.2.6/
--rw-rw-rw-   0        0        0     1111 2023-05-26 04:30:40.000000 quao-0.2.6/LICENSE
--rw-rw-rw-   0        0        0     2839 2023-06-16 09:14:00.274891 quao-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2023-05-26 04:30:40.000000 quao-0.2.6/README.md
--rw-rw-rw-   0        0        0      939 2023-06-16 09:13:47.000000 quao-0.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-16 09:14:00.275891 quao-0.2.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-16 09:14:00.218891 quao-0.2.6/src/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.2.6/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 09:14:00.221947 quao-0.2.6/src/quao/
--rw-rw-rw-   0        0        0      203 2023-06-16 09:13:47.000000 quao-0.2.6/src/quao/__init__.py
--rw-rw-rw-   0        0        0     6520 2023-06-16 09:13:47.000000 quao-0.2.6/src/quao/backend.py
-drwxrwxrwx   0        0        0        0 2023-06-16 09:14:00.229892 quao-0.2.6/src/quao/config/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.2.6/src/quao/config/__init__.py
--rw-rw-rw-   0        0        0      193 2023-06-15 04:25:14.000000 quao-0.2.6/src/quao/config/logging_config.py
-drwxrwxrwx   0        0        0        0 2023-06-16 09:14:00.230903 quao-0.2.6/src/quao/data/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.6/src/quao/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 09:14:00.232891 quao-0.2.6/src/quao/data/job/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.6/src/quao/data/job/__init__.py
--rw-rw-rw-   0        0        0      876 2023-06-16 07:14:53.000000 quao-0.2.6/src/quao/data/job/job_response.py
-drwxrwxrwx   0        0        0        0 2023-06-16 09:14:00.235891 quao-0.2.6/src/quao/data/request/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.6/src/quao/data/request/__init__.py
--rw-rw-rw-   0        0        0      680 2023-06-16 07:14:53.000000 quao-0.2.6/src/quao/data/request/request_data.py
-drwxrwxrwx   0        0        0        0 2023-06-16 09:14:00.245892 quao-0.2.6/src/quao/enum/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.6/src/quao/enum/__init__.py
--rw-rw-rw-   0        0        0      185 2023-06-15 04:16:49.000000 quao-0.2.6/src/quao/enum/http_header.py
--rw-rw-rw-   0        0        0      212 2023-06-02 01:59:38.000000 quao-0.2.6/src/quao/enum/http_status.py
--rw-rw-rw-   0        0        0      213 2023-06-02 10:41:04.000000 quao-0.2.6/src/quao/enum/job_status.py
--rw-rw-rw-   0        0        0      258 2023-06-02 01:59:38.000000 quao-0.2.6/src/quao/enum/media_type.py
--rw-rw-rw-   0        0        0      205 2023-06-13 03:37:41.000000 quao-0.2.6/src/quao/enum/processing_unit.py
--rw-rw-rw-   0        0        0      297 2023-06-02 01:59:38.000000 quao-0.2.6/src/quao/enum/provider_type.py
--rw-rw-rw-   0        0        0      179 2023-06-02 01:59:38.000000 quao-0.2.6/src/quao/enum/sdk.py
--rw-rw-rw-   0        0        0      169 2023-06-16 09:12:10.000000 quao-0.2.6/src/quao/enum/token_type.py
-drwxrwxrwx   0        0        0        0 2023-06-16 09:14:00.248890 quao-0.2.6/src/quao/factory/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.6/src/quao/factory/__init__.py
--rw-rw-rw-   0        0        0     1555 2023-06-02 10:41:04.000000 quao-0.2.6/src/quao/factory/device_factory.py
--rw-rw-rw-   0        0        0     1351 2023-06-02 10:41:04.000000 quao-0.2.6/src/quao/factory/provider_factory.py
-drwxrwxrwx   0        0        0        0 2023-06-16 09:14:00.250891 quao-0.2.6/src/quao/model/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.6/src/quao/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 09:14:00.260891 quao-0.2.6/src/quao/model/device/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.6/src/quao/model/device/__init__.py
--rw-rw-rw-   0        0        0     1541 2023-06-15 04:25:14.000000 quao-0.2.6/src/quao/model/device/aws_braket_device.py
--rw-rw-rw-   0        0        0     3164 2023-06-15 04:25:14.000000 quao-0.2.6/src/quao/model/device/device.py
--rw-rw-rw-   0        0        0     1015 2023-06-15 04:25:14.000000 quao-0.2.6/src/quao/model/device/ibm_cloud_device.py
--rw-rw-rw-   0        0        0      795 2023-06-15 04:25:14.000000 quao-0.2.6/src/quao/model/device/ibm_quantum_device.py
--rw-rw-rw-   0        0        0      779 2023-06-15 04:25:14.000000 quao-0.2.6/src/quao/model/device/qiskit_device.py
--rw-rw-rw-   0        0        0     2637 2023-06-15 04:25:14.000000 quao-0.2.6/src/quao/model/device/quao_device.py
-drwxrwxrwx   0        0        0        0 2023-06-16 09:14:00.263891 quao-0.2.6/src/quao/model/job/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.6/src/quao/model/job/__init__.py
--rw-rw-rw-   0        0        0     2693 2023-06-02 10:41:04.000000 quao-0.2.6/src/quao/model/job/qiskit_status.py
-drwxrwxrwx   0        0        0        0 2023-06-16 09:14:00.270891 quao-0.2.6/src/quao/model/provider/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.6/src/quao/model/provider/__init__.py
--rw-rw-rw-   0        0        0     1258 2023-06-15 04:25:14.000000 quao-0.2.6/src/quao/model/provider/aws_braket_provider.py
--rw-rw-rw-   0        0        0     1011 2023-06-15 04:25:14.000000 quao-0.2.6/src/quao/model/provider/ibm_cloud_provider.py
--rw-rw-rw-   0        0        0      881 2023-06-15 04:25:14.000000 quao-0.2.6/src/quao/model/provider/ibm_quantum_provider.py
--rw-rw-rw-   0        0        0      589 2023-06-02 10:41:04.000000 quao-0.2.6/src/quao/model/provider/provider.py
--rw-rw-rw-   0        0        0     1456 2023-06-16 07:07:16.000000 quao-0.2.6/src/quao/model/provider/quao_provider.py
-drwxrwxrwx   0        0        0        0 2023-06-16 09:14:00.273891 quao-0.2.6/src/quao/util/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.6/src/quao/util/__init__.py
--rw-rw-rw-   0        0        0     2047 2023-06-02 10:41:04.000000 quao-0.2.6/src/quao/util/json_parser_util.py
--rw-rw-rw-   0        0        0     1458 2023-06-16 07:14:53.000000 quao-0.2.6/src/quao/util/response_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-16 09:14:00.226891 quao-0.2.6/src/quao.egg-info/
--rw-rw-rw-   0        0        0     2839 2023-06-16 09:14:00.000000 quao-0.2.6/src/quao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1537 2023-06-16 09:14:00.000000 quao-0.2.6/src/quao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 09:14:00.000000 quao-0.2.6/src/quao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      181 2023-06-16 09:14:00.000000 quao-0.2.6/src/quao.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-16 09:14:00.000000 quao-0.2.6/src/quao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 01:50:44.048615 quao-0.2.7/
+-rw-rw-rw-   0        0        0     1111 2023-05-26 04:30:40.000000 quao-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0     2839 2023-06-19 01:50:44.043616 quao-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2023-05-26 04:30:40.000000 quao-0.2.7/README.md
+-rw-rw-rw-   0        0        0      939 2023-06-19 01:50:26.000000 quao-0.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 01:50:44.054616 quao-0.2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.806584 quao-0.2.7/src/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.2.7/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.811585 quao-0.2.7/src/quao/
+-rw-rw-rw-   0        0        0      203 2023-06-19 01:50:26.000000 quao-0.2.7/src/quao/__init__.py
+-rw-rw-rw-   0        0        0     6636 2023-06-19 01:49:45.000000 quao-0.2.7/src/quao/backend.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.833584 quao-0.2.7/src/quao/config/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.2.7/src/quao/config/__init__.py
+-rw-rw-rw-   0        0        0      193 2023-06-15 04:25:14.000000 quao-0.2.7/src/quao/config/logging_config.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.849582 quao-0.2.7/src/quao/data/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.870584 quao-0.2.7/src/quao/data/job/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/data/job/__init__.py
+-rw-rw-rw-   0        0        0      942 2023-06-19 01:49:45.000000 quao-0.2.7/src/quao/data/job/job_response.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.877585 quao-0.2.7/src/quao/data/request/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/data/request/__init__.py
+-rw-rw-rw-   0        0        0      680 2023-06-16 07:14:53.000000 quao-0.2.7/src/quao/data/request/request_data.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.917617 quao-0.2.7/src/quao/enum/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/enum/__init__.py
+-rw-rw-rw-   0        0        0      185 2023-06-15 04:16:49.000000 quao-0.2.7/src/quao/enum/http_header.py
+-rw-rw-rw-   0        0        0      212 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/enum/http_status.py
+-rw-rw-rw-   0        0        0      213 2023-06-02 10:41:04.000000 quao-0.2.7/src/quao/enum/job_status.py
+-rw-rw-rw-   0        0        0      258 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/enum/media_type.py
+-rw-rw-rw-   0        0        0      205 2023-06-13 03:37:41.000000 quao-0.2.7/src/quao/enum/processing_unit.py
+-rw-rw-rw-   0        0        0      297 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/enum/provider_type.py
+-rw-rw-rw-   0        0        0      179 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/enum/sdk.py
+-rw-rw-rw-   0        0        0      169 2023-06-16 09:12:10.000000 quao-0.2.7/src/quao/enum/token_type.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.924618 quao-0.2.7/src/quao/factory/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/factory/__init__.py
+-rw-rw-rw-   0        0        0     1555 2023-06-02 10:41:04.000000 quao-0.2.7/src/quao/factory/device_factory.py
+-rw-rw-rw-   0        0        0     1351 2023-06-02 10:41:04.000000 quao-0.2.7/src/quao/factory/provider_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.927618 quao-0.2.7/src/quao/model/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.982615 quao-0.2.7/src/quao/model/device/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/model/device/__init__.py
+-rw-rw-rw-   0        0        0     1541 2023-06-15 04:25:14.000000 quao-0.2.7/src/quao/model/device/aws_braket_device.py
+-rw-rw-rw-   0        0        0     3164 2023-06-15 04:25:14.000000 quao-0.2.7/src/quao/model/device/device.py
+-rw-rw-rw-   0        0        0     1015 2023-06-15 04:25:14.000000 quao-0.2.7/src/quao/model/device/ibm_cloud_device.py
+-rw-rw-rw-   0        0        0      795 2023-06-15 04:25:14.000000 quao-0.2.7/src/quao/model/device/ibm_quantum_device.py
+-rw-rw-rw-   0        0        0      779 2023-06-15 04:25:14.000000 quao-0.2.7/src/quao/model/device/qiskit_device.py
+-rw-rw-rw-   0        0        0     2637 2023-06-15 04:25:14.000000 quao-0.2.7/src/quao/model/device/quao_device.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.987617 quao-0.2.7/src/quao/model/job/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/model/job/__init__.py
+-rw-rw-rw-   0        0        0     2693 2023-06-02 10:41:04.000000 quao-0.2.7/src/quao/model/job/qiskit_status.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:50:44.016616 quao-0.2.7/src/quao/model/provider/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/model/provider/__init__.py
+-rw-rw-rw-   0        0        0     1258 2023-06-15 04:25:14.000000 quao-0.2.7/src/quao/model/provider/aws_braket_provider.py
+-rw-rw-rw-   0        0        0     1011 2023-06-15 04:25:14.000000 quao-0.2.7/src/quao/model/provider/ibm_cloud_provider.py
+-rw-rw-rw-   0        0        0      881 2023-06-15 04:25:14.000000 quao-0.2.7/src/quao/model/provider/ibm_quantum_provider.py
+-rw-rw-rw-   0        0        0      589 2023-06-02 10:41:04.000000 quao-0.2.7/src/quao/model/provider/provider.py
+-rw-rw-rw-   0        0        0     1456 2023-06-16 07:07:16.000000 quao-0.2.7/src/quao/model/provider/quao_provider.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:50:44.036622 quao-0.2.7/src/quao/util/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/util/__init__.py
+-rw-rw-rw-   0        0        0     2047 2023-06-02 10:41:04.000000 quao-0.2.7/src/quao/util/json_parser_util.py
+-rw-rw-rw-   0        0        0     1568 2023-06-19 01:49:45.000000 quao-0.2.7/src/quao/util/response_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.826589 quao-0.2.7/src/quao.egg-info/
+-rw-rw-rw-   0        0        0     2839 2023-06-19 01:50:43.000000 quao-0.2.7/src/quao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1537 2023-06-19 01:50:43.000000 quao-0.2.7/src/quao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 01:50:43.000000 quao-0.2.7/src/quao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      181 2023-06-19 01:50:43.000000 quao-0.2.7/src/quao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-19 01:50:43.000000 quao-0.2.7/src/quao.egg-info/top_level.txt
```

### Comparing `quao-0.2.6/LICENSE` & `quao-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `quao-0.2.6/PKG-INFO` & `quao-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.2.6
+Version: 0.2.7
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.2.6/README.md` & `quao-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `quao-0.2.6/pyproject.toml` & `quao-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quao"
-version = "0.2.6"
+version = "0.2.7"
 description = "Quao Library supporting Quao Platform for Quantum Computing"
 readme = "README.md"
 authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `quao-0.2.6/src/quao/backend.py` & `quao-0.2.7/src/quao/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,15 @@
         @param circuit:
         @return:
         """
 
         error_job_response = JobResponse()
         error_job_response.job_status = JobStatus.ERROR.value
         error_job_response.user_identity = self.user_identity
+        error_job_response.user_token = self.user_token
 
         shots = self.shots
 
         if circuit and self.backend_data:
             device_name = self.backend_data.get("deviceName")
             provider_tag = self.backend_data.get("providerTag")
             authentication = self.backend_data.get("authentication")
@@ -151,14 +152,15 @@
 
                 logging.debug('Execute job with device name: {0}'.format(device_name))
                 device = DeviceFactory().create_device(provider, device_name, authentication,
                                                        self.sdk)
 
                 job_response = device.run_circuit(circuit=circuit, shots=shots)
                 job_response.user_identity = self.user_identity
+                job_response.user_token = self.user_token
 
                 return job_response
 
             except Exception as exception:
                 error_job_response.job_result = {"error": str(exception)}
 
         elif self.backend_data is None:
```

### Comparing `quao-0.2.6/src/quao/data/job/job_response.py` & `quao-0.2.7/src/quao/data/job/job_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,17 @@
     def __init__(
             self,
             provider_job_id: str = "",
             job_status: str = "",
             job_result=None,
             content_type=None,
             job_histogram=None,
-            user_identity=""
+            user_identity="",
+            user_token=""
     ):
         self.provider_job_id = provider_job_id if provider_job_id else ""
         self.job_status = job_status if job_status else JobStatus.ERROR.value
         self.job_result = job_result if job_result else None
         self.content_type = content_type if content_type else MediaType.ALL_TYPE.value
         self.job_histogram = job_histogram if job_histogram else None
         self.user_identity = user_identity
+        self.user_token = user_token
```

### Comparing `quao-0.2.6/src/quao/data/request/request_data.py` & `quao-0.2.7/src/quao/data/request/request_data.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.6/src/quao/factory/device_factory.py` & `quao-0.2.7/src/quao/factory/device_factory.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.6/src/quao/factory/provider_factory.py` & `quao-0.2.7/src/quao/factory/provider_factory.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.6/src/quao/model/device/aws_braket_device.py` & `quao-0.2.7/src/quao/model/device/aws_braket_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.6/src/quao/model/device/device.py` & `quao-0.2.7/src/quao/model/device/device.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.6/src/quao/model/device/ibm_cloud_device.py` & `quao-0.2.7/src/quao/model/device/ibm_cloud_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.6/src/quao/model/device/ibm_quantum_device.py` & `quao-0.2.7/src/quao/model/device/ibm_quantum_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.6/src/quao/model/device/qiskit_device.py` & `quao-0.2.7/src/quao/model/device/qiskit_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.6/src/quao/model/device/quao_device.py` & `quao-0.2.7/src/quao/model/device/quao_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.6/src/quao/model/job/qiskit_status.py` & `quao-0.2.7/src/quao/model/job/qiskit_status.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.6/src/quao/model/provider/aws_braket_provider.py` & `quao-0.2.7/src/quao/model/provider/aws_braket_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.6/src/quao/model/provider/ibm_cloud_provider.py` & `quao-0.2.7/src/quao/model/provider/ibm_cloud_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.6/src/quao/model/provider/ibm_quantum_provider.py` & `quao-0.2.7/src/quao/model/provider/ibm_quantum_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.6/src/quao/model/provider/provider.py` & `quao-0.2.7/src/quao/model/provider/provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.6/src/quao/model/provider/quao_provider.py` & `quao-0.2.7/src/quao/model/provider/quao_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.6/src/quao/util/json_parser_util.py` & `quao-0.2.7/src/quao/util/json_parser_util.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.6/src/quao/util/response_utils.py` & `quao-0.2.7/src/quao/util/response_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,18 @@
                 "contentType": job_response.content_type,
                 "histogram": job_response.job_histogram
             }
 
             response = {
                 "statusCode": status_code,
                 "body": job_dict,
-                "userIdentity": job_response.user_identity
+                "userIdentity": job_response.user_identity,
+                "userToken": job_response.user_token
             }
         else:
             response = {
                 "statusCode": 500,
                 "body": "Error in function code. Please contact the developer.",
-                "userIdentity": job_response.user_identity
+                "userIdentity": job_response.user_identity,
+                "userToken": job_response.user_token
             }
         return response
```

### Comparing `quao-0.2.6/src/quao.egg-info/PKG-INFO` & `quao-0.2.7/src/quao.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.2.6
+Version: 0.2.7
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.2.6/src/quao.egg-info/SOURCES.txt` & `quao-0.2.7/src/quao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

