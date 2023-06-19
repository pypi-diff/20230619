# Comparing `tmp/quao-0.2.7.tar.gz` & `tmp/quao-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quao-0.2.7.tar", last modified: Mon Jun 19 01:50:44 2023, max compression
+gzip compressed data, was "quao-0.2.8.tar", last modified: Mon Jun 19 02:14:36 2023, max compression
```

## Comparing `quao-0.2.7.tar` & `quao-0.2.8.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 01:50:44.048615 quao-0.2.7/
--rw-rw-rw-   0        0        0     1111 2023-05-26 04:30:40.000000 quao-0.2.7/LICENSE
--rw-rw-rw-   0        0        0     2839 2023-06-19 01:50:44.043616 quao-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2023-05-26 04:30:40.000000 quao-0.2.7/README.md
--rw-rw-rw-   0        0        0      939 2023-06-19 01:50:26.000000 quao-0.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-19 01:50:44.054616 quao-0.2.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.806584 quao-0.2.7/src/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.2.7/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.811585 quao-0.2.7/src/quao/
--rw-rw-rw-   0        0        0      203 2023-06-19 01:50:26.000000 quao-0.2.7/src/quao/__init__.py
--rw-rw-rw-   0        0        0     6636 2023-06-19 01:49:45.000000 quao-0.2.7/src/quao/backend.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.833584 quao-0.2.7/src/quao/config/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.2.7/src/quao/config/__init__.py
--rw-rw-rw-   0        0        0      193 2023-06-15 04:25:14.000000 quao-0.2.7/src/quao/config/logging_config.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.849582 quao-0.2.7/src/quao/data/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.870584 quao-0.2.7/src/quao/data/job/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/data/job/__init__.py
--rw-rw-rw-   0        0        0      942 2023-06-19 01:49:45.000000 quao-0.2.7/src/quao/data/job/job_response.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.877585 quao-0.2.7/src/quao/data/request/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/data/request/__init__.py
--rw-rw-rw-   0        0        0      680 2023-06-16 07:14:53.000000 quao-0.2.7/src/quao/data/request/request_data.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.917617 quao-0.2.7/src/quao/enum/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/enum/__init__.py
--rw-rw-rw-   0        0        0      185 2023-06-15 04:16:49.000000 quao-0.2.7/src/quao/enum/http_header.py
--rw-rw-rw-   0        0        0      212 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/enum/http_status.py
--rw-rw-rw-   0        0        0      213 2023-06-02 10:41:04.000000 quao-0.2.7/src/quao/enum/job_status.py
--rw-rw-rw-   0        0        0      258 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/enum/media_type.py
--rw-rw-rw-   0        0        0      205 2023-06-13 03:37:41.000000 quao-0.2.7/src/quao/enum/processing_unit.py
--rw-rw-rw-   0        0        0      297 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/enum/provider_type.py
--rw-rw-rw-   0        0        0      179 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/enum/sdk.py
--rw-rw-rw-   0        0        0      169 2023-06-16 09:12:10.000000 quao-0.2.7/src/quao/enum/token_type.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.924618 quao-0.2.7/src/quao/factory/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/factory/__init__.py
--rw-rw-rw-   0        0        0     1555 2023-06-02 10:41:04.000000 quao-0.2.7/src/quao/factory/device_factory.py
--rw-rw-rw-   0        0        0     1351 2023-06-02 10:41:04.000000 quao-0.2.7/src/quao/factory/provider_factory.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.927618 quao-0.2.7/src/quao/model/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.982615 quao-0.2.7/src/quao/model/device/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/model/device/__init__.py
--rw-rw-rw-   0        0        0     1541 2023-06-15 04:25:14.000000 quao-0.2.7/src/quao/model/device/aws_braket_device.py
--rw-rw-rw-   0        0        0     3164 2023-06-15 04:25:14.000000 quao-0.2.7/src/quao/model/device/device.py
--rw-rw-rw-   0        0        0     1015 2023-06-15 04:25:14.000000 quao-0.2.7/src/quao/model/device/ibm_cloud_device.py
--rw-rw-rw-   0        0        0      795 2023-06-15 04:25:14.000000 quao-0.2.7/src/quao/model/device/ibm_quantum_device.py
--rw-rw-rw-   0        0        0      779 2023-06-15 04:25:14.000000 quao-0.2.7/src/quao/model/device/qiskit_device.py
--rw-rw-rw-   0        0        0     2637 2023-06-15 04:25:14.000000 quao-0.2.7/src/quao/model/device/quao_device.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.987617 quao-0.2.7/src/quao/model/job/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/model/job/__init__.py
--rw-rw-rw-   0        0        0     2693 2023-06-02 10:41:04.000000 quao-0.2.7/src/quao/model/job/qiskit_status.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:50:44.016616 quao-0.2.7/src/quao/model/provider/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/model/provider/__init__.py
--rw-rw-rw-   0        0        0     1258 2023-06-15 04:25:14.000000 quao-0.2.7/src/quao/model/provider/aws_braket_provider.py
--rw-rw-rw-   0        0        0     1011 2023-06-15 04:25:14.000000 quao-0.2.7/src/quao/model/provider/ibm_cloud_provider.py
--rw-rw-rw-   0        0        0      881 2023-06-15 04:25:14.000000 quao-0.2.7/src/quao/model/provider/ibm_quantum_provider.py
--rw-rw-rw-   0        0        0      589 2023-06-02 10:41:04.000000 quao-0.2.7/src/quao/model/provider/provider.py
--rw-rw-rw-   0        0        0     1456 2023-06-16 07:07:16.000000 quao-0.2.7/src/quao/model/provider/quao_provider.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:50:44.036622 quao-0.2.7/src/quao/util/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.7/src/quao/util/__init__.py
--rw-rw-rw-   0        0        0     2047 2023-06-02 10:41:04.000000 quao-0.2.7/src/quao/util/json_parser_util.py
--rw-rw-rw-   0        0        0     1568 2023-06-19 01:49:45.000000 quao-0.2.7/src/quao/util/response_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:50:43.826589 quao-0.2.7/src/quao.egg-info/
--rw-rw-rw-   0        0        0     2839 2023-06-19 01:50:43.000000 quao-0.2.7/src/quao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1537 2023-06-19 01:50:43.000000 quao-0.2.7/src/quao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 01:50:43.000000 quao-0.2.7/src/quao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      181 2023-06-19 01:50:43.000000 quao-0.2.7/src/quao.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-19 01:50:43.000000 quao-0.2.7/src/quao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 02:14:36.289151 quao-0.2.8/
+-rw-rw-rw-   0        0        0     1111 2023-05-26 04:30:40.000000 quao-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0     2839 2023-06-19 02:14:36.288151 quao-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2023-05-26 04:30:40.000000 quao-0.2.8/README.md
+-rw-rw-rw-   0        0        0      939 2023-06-19 02:14:23.000000 quao-0.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 02:14:36.289151 quao-0.2.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-19 02:14:36.229150 quao-0.2.8/src/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.2.8/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:14:36.232176 quao-0.2.8/src/quao/
+-rw-rw-rw-   0        0        0      203 2023-06-19 02:14:23.000000 quao-0.2.8/src/quao/__init__.py
+-rw-rw-rw-   0        0        0     6636 2023-06-19 01:49:45.000000 quao-0.2.8/src/quao/backend.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:14:36.239150 quao-0.2.8/src/quao/config/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.2.8/src/quao/config/__init__.py
+-rw-rw-rw-   0        0        0      193 2023-06-15 04:25:14.000000 quao-0.2.8/src/quao/config/logging_config.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:14:36.240150 quao-0.2.8/src/quao/data/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.8/src/quao/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:14:36.242150 quao-0.2.8/src/quao/data/job/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.8/src/quao/data/job/__init__.py
+-rw-rw-rw-   0        0        0      942 2023-06-19 01:49:45.000000 quao-0.2.8/src/quao/data/job/job_response.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:14:36.245152 quao-0.2.8/src/quao/data/request/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.8/src/quao/data/request/__init__.py
+-rw-rw-rw-   0        0        0      680 2023-06-16 07:14:53.000000 quao-0.2.8/src/quao/data/request/request_data.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:14:36.256151 quao-0.2.8/src/quao/enum/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.8/src/quao/enum/__init__.py
+-rw-rw-rw-   0        0        0      185 2023-06-15 04:16:49.000000 quao-0.2.8/src/quao/enum/http_header.py
+-rw-rw-rw-   0        0        0      212 2023-06-02 01:59:38.000000 quao-0.2.8/src/quao/enum/http_status.py
+-rw-rw-rw-   0        0        0      213 2023-06-02 10:41:04.000000 quao-0.2.8/src/quao/enum/job_status.py
+-rw-rw-rw-   0        0        0      258 2023-06-02 01:59:38.000000 quao-0.2.8/src/quao/enum/media_type.py
+-rw-rw-rw-   0        0        0      205 2023-06-13 03:37:41.000000 quao-0.2.8/src/quao/enum/processing_unit.py
+-rw-rw-rw-   0        0        0      297 2023-06-02 01:59:38.000000 quao-0.2.8/src/quao/enum/provider_type.py
+-rw-rw-rw-   0        0        0      179 2023-06-02 01:59:38.000000 quao-0.2.8/src/quao/enum/sdk.py
+-rw-rw-rw-   0        0        0      169 2023-06-16 09:12:10.000000 quao-0.2.8/src/quao/enum/token_type.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:14:36.260151 quao-0.2.8/src/quao/factory/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.8/src/quao/factory/__init__.py
+-rw-rw-rw-   0        0        0     1555 2023-06-02 10:41:04.000000 quao-0.2.8/src/quao/factory/device_factory.py
+-rw-rw-rw-   0        0        0     1351 2023-06-02 10:41:04.000000 quao-0.2.8/src/quao/factory/provider_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:14:36.261151 quao-0.2.8/src/quao/model/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.8/src/quao/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:14:36.271151 quao-0.2.8/src/quao/model/device/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.8/src/quao/model/device/__init__.py
+-rw-rw-rw-   0        0        0     1612 2023-06-19 02:14:23.000000 quao-0.2.8/src/quao/model/device/aws_braket_device.py
+-rw-rw-rw-   0        0        0     3198 2023-06-19 02:14:23.000000 quao-0.2.8/src/quao/model/device/device.py
+-rw-rw-rw-   0        0        0     1015 2023-06-15 04:25:14.000000 quao-0.2.8/src/quao/model/device/ibm_cloud_device.py
+-rw-rw-rw-   0        0        0      795 2023-06-15 04:25:14.000000 quao-0.2.8/src/quao/model/device/ibm_quantum_device.py
+-rw-rw-rw-   0        0        0      876 2023-06-19 02:14:23.000000 quao-0.2.8/src/quao/model/device/qiskit_device.py
+-rw-rw-rw-   0        0        0     2734 2023-06-19 02:14:23.000000 quao-0.2.8/src/quao/model/device/quao_device.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:14:36.273151 quao-0.2.8/src/quao/model/job/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.8/src/quao/model/job/__init__.py
+-rw-rw-rw-   0        0        0     2693 2023-06-02 10:41:04.000000 quao-0.2.8/src/quao/model/job/qiskit_status.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:14:36.282152 quao-0.2.8/src/quao/model/provider/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.8/src/quao/model/provider/__init__.py
+-rw-rw-rw-   0        0        0     1258 2023-06-15 04:25:14.000000 quao-0.2.8/src/quao/model/provider/aws_braket_provider.py
+-rw-rw-rw-   0        0        0     1011 2023-06-15 04:25:14.000000 quao-0.2.8/src/quao/model/provider/ibm_cloud_provider.py
+-rw-rw-rw-   0        0        0      881 2023-06-15 04:25:14.000000 quao-0.2.8/src/quao/model/provider/ibm_quantum_provider.py
+-rw-rw-rw-   0        0        0      589 2023-06-02 10:41:04.000000 quao-0.2.8/src/quao/model/provider/provider.py
+-rw-rw-rw-   0        0        0     1456 2023-06-16 07:07:16.000000 quao-0.2.8/src/quao/model/provider/quao_provider.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:14:36.286150 quao-0.2.8/src/quao/util/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.8/src/quao/util/__init__.py
+-rw-rw-rw-   0        0        0     2047 2023-06-02 10:41:04.000000 quao-0.2.8/src/quao/util/json_parser_util.py
+-rw-rw-rw-   0        0        0     1568 2023-06-19 01:49:45.000000 quao-0.2.8/src/quao/util/response_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:14:36.237150 quao-0.2.8/src/quao.egg-info/
+-rw-rw-rw-   0        0        0     2839 2023-06-19 02:14:36.000000 quao-0.2.8/src/quao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1537 2023-06-19 02:14:36.000000 quao-0.2.8/src/quao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 02:14:36.000000 quao-0.2.8/src/quao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      181 2023-06-19 02:14:36.000000 quao-0.2.8/src/quao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-19 02:14:36.000000 quao-0.2.8/src/quao.egg-info/top_level.txt
```

### Comparing `quao-0.2.7/LICENSE` & `quao-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `quao-0.2.7/PKG-INFO` & `quao-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.2.7
+Version: 0.2.8
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.2.7/README.md` & `quao-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `quao-0.2.7/pyproject.toml` & `quao-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quao"
-version = "0.2.7"
+version = "0.2.8"
 description = "Quao Library supporting Quao Platform for Quantum Computing"
 readme = "README.md"
 authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `quao-0.2.7/src/quao/backend.py` & `quao-0.2.8/src/quao/backend.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.7/src/quao/data/job/job_response.py` & `quao-0.2.8/src/quao/data/job/job_response.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.7/src/quao/data/request/request_data.py` & `quao-0.2.8/src/quao/data/request/request_data.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.7/src/quao/factory/device_factory.py` & `quao-0.2.8/src/quao/factory/device_factory.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.7/src/quao/factory/provider_factory.py` & `quao-0.2.8/src/quao/factory/provider_factory.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.7/src/quao/model/device/aws_braket_device.py` & `quao-0.2.8/src/quao/model/device/aws_braket_device.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from ..provider.provider import Provider
 from ...enum.job_status import JobStatus
 from ...util.json_parser_util import JsonParserUtils
 from ...config.logging_config import logging
 
 
 class AwsBraketDevice(Device):
+    def _get_name(self) -> str:
+        return str(self.device.name)
 
     def __init__(self, provider: Provider,
                  device_specification: str,
                  s3_bucket_name: str,
                  s3_prefix: str):
         super().__init__(provider, device_specification)
         self.s3_folder = (s3_bucket_name, s3_prefix)
```

### Comparing `quao-0.2.7/src/quao/model/device/device.py` & `quao-0.2.8/src/quao/model/device/device.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,21 +43,19 @@
                 content_type = MediaType.APPLICATION_JSON.value
 
                 logging.debug('Producing histogram ....')
                 job_histogram = self._produce_histogram_data(job_result)
                 logging.debug('Producing histogram completed!')
 
         except Exception as exception:
-            device_name = str(self.device.configuration().backend_name)
-
             logging.debug('Exception when invoke job on device {0}: {1}'
-                         .format(device_name, str(exception)))
+                          .format(self._get_name(), str(exception)))
 
             job_result_dictionary = {
-                "error": "Exception when invoke job on device: " + device_name,
+                "error": "Exception when invoke job on device: " + self._get_name(),
                 "exception": str(exception)
             }
 
             job_status = JobStatus.ERROR.value
 
         return JobResponse(
             provider_job_id=provider_job_id,
@@ -107,7 +105,14 @@
 
     @abstractmethod
     def _parse_job_result(self, job_result) -> dict:
         """
 
         """
         pass
+
+    @abstractmethod
+    def _get_name(self) -> str:
+        """
+
+        """
+        pass
```

### Comparing `quao-0.2.7/src/quao/model/device/ibm_cloud_device.py` & `quao-0.2.8/src/quao/model/device/ibm_cloud_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.7/src/quao/model/device/ibm_quantum_device.py` & `quao-0.2.8/src/quao/model/device/ibm_quantum_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.7/src/quao/model/device/qiskit_device.py` & `quao-0.2.8/src/quao/model/device/qiskit_device.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,7 +21,10 @@
         return histogram_data
 
     def _get_provider_job_id(self, job) -> str:
         return job.job_id()
 
     def _get_job_status(self, job) -> str:
         return job.status().name
+
+    def _get_name(self) -> str:
+        return str(self.device.configuration().backend_name)
```

### Comparing `quao-0.2.7/src/quao/model/device/quao_device.py` & `quao-0.2.8/src/quao/model/device/quao_device.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 from ...enum.sdk import Sdk
 from ..device.device import Device
 from ..provider.provider import Provider
 from ...config.logging_config import logging
 
 
 class QuaoDevice(Device):
+    def _get_name(self) -> str:
+        return str(self.device.configuration().backend_name)
+
     def __init__(self, provider: Provider, device_specification: str, sdk: str):
         super().__init__(provider, device_specification)
         self.sdk = sdk
 
     def _create_job(self, circuit, shots):
         logging.debug('Create Quao job with {0} shots'.format(shots))
         if Sdk.QISKIT.value.__eq__(self.sdk):
```

### Comparing `quao-0.2.7/src/quao/model/job/qiskit_status.py` & `quao-0.2.8/src/quao/model/job/qiskit_status.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.7/src/quao/model/provider/aws_braket_provider.py` & `quao-0.2.8/src/quao/model/provider/aws_braket_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.7/src/quao/model/provider/ibm_cloud_provider.py` & `quao-0.2.8/src/quao/model/provider/ibm_cloud_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.7/src/quao/model/provider/ibm_quantum_provider.py` & `quao-0.2.8/src/quao/model/provider/ibm_quantum_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.7/src/quao/model/provider/provider.py` & `quao-0.2.8/src/quao/model/provider/provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.7/src/quao/model/provider/quao_provider.py` & `quao-0.2.8/src/quao/model/provider/quao_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.7/src/quao/util/json_parser_util.py` & `quao-0.2.8/src/quao/util/json_parser_util.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.7/src/quao/util/response_utils.py` & `quao-0.2.8/src/quao/util/response_utils.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.7/src/quao.egg-info/PKG-INFO` & `quao-0.2.8/src/quao.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.2.7
+Version: 0.2.8
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.2.7/src/quao.egg-info/SOURCES.txt` & `quao-0.2.8/src/quao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

