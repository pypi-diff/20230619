# Comparing `tmp/pasqal-cloud-0.2.7.tar.gz` & `tmp/pasqal-cloud-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasqal-cloud-0.2.7.tar", last modified: Thu Jun  8 09:25:09 2023, max compression
+gzip compressed data, was "pasqal-cloud-0.2.8.tar", last modified: Mon Jun 19 16:12:46 2023, max compression
```

## Comparing `pasqal-cloud-0.2.7.tar` & `pasqal-cloud-0.2.8.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.791922 pasqal-cloud-0.2.7/pasqal_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/pasqal_cloud/device/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/pasqal_cloud/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/device/configuration/base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/device/configuration/emu_free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/device/configuration/emu_tn.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/device/emulator_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/job.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/pasqal_cloud/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/utils/jsend.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/utils/strenum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/pasqal_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-06-08 09:25:09.000000 pasqal-cloud-0.2.7/pasqal_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-08 09:25:09.000000 pasqal-cloud-0.2.7/pasqal_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:25:09.000000 pasqal-cloud-0.2.7/pasqal_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-08 09:25:09.000000 pasqal-cloud-0.2.7/pasqal_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 09:25:09.000000 pasqal-cloud-0.2.7/pasqal_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/sdk/device/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/sdk/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/sdk/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/sdk/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/sdk/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/test_cloud_sdk_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/test_device_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/tests/test_doubles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/test_doubles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/test_doubles/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/test_project_renaming_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.840451 pasqal-cloud-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-19 16:12:46.840451 pasqal-cloud-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.836451 pasqal-cloud-0.2.8/pasqal_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.836451 pasqal-cloud-0.2.8/pasqal_cloud/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.836451 pasqal-cloud-0.2.8/pasqal_cloud/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/device/configuration/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/device/configuration/emu_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/device/configuration/emu_tn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/device/emulator_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.840451 pasqal-cloud-0.2.8/pasqal_cloud/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/utils/jsend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/utils/strenum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.836451 pasqal-cloud-0.2.8/pasqal_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-19 16:12:46.000000 pasqal-cloud-0.2.8/pasqal_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-19 16:12:46.000000 pasqal-cloud-0.2.8/pasqal_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:12:46.000000 pasqal-cloud-0.2.8/pasqal_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-19 16:12:46.000000 pasqal-cloud-0.2.8/pasqal_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-19 16:12:46.000000 pasqal-cloud-0.2.8/pasqal_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.840451 pasqal-cloud-0.2.8/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.840451 pasqal-cloud-0.2.8/sdk/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/sdk/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.840451 pasqal-cloud-0.2.8/sdk/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/sdk/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/sdk/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.840451 pasqal-cloud-0.2.8/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-19 16:12:46.840451 pasqal-cloud-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.840451 pasqal-cloud-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/test_cloud_sdk_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/test_device_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.840451 pasqal-cloud-0.2.8/tests/test_doubles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/test_doubles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/test_doubles/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/test_project_renaming_compatibility.py
```

### Comparing `pasqal-cloud-0.2.7/LICENSE` & `pasqal-cloud-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.7/PKG-INFO` & `pasqal-cloud-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.2.7
+Version: 0.2.8
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -98,15 +98,16 @@
 ### Authentication
 
 There are several ways to provide a correct authentication using the SDK.
 
 ```python
 from pasqal_cloud import SDK
 
-project_id="your_project_id" # Replace this value by your project_id on the PASQAL platform.
+project_id="your_project_id" # Replace this value by your project_id. It can be found on the user portal under the name "group_id". "Groups" have recently been renamed to "projects" and frontend is currently being updated accordingly.
+
 username="your_username" # Replace this value by your username or email on the PASQAL platform.
 password="your_password" # Replace this value by your password on the PASQAL platform.
 # Ideally, do not write this password in a script but provide in through the command-line or as a secret environment variable.
 
 """ Method 1: Username + Password
     If you know your credentials, you can pass them to the SDK instance on creation.
 """
@@ -165,15 +166,15 @@
 ### List of supported device specifications
 
 The SDK provides a method to retrieve the devices specs currently defined on PASQAL's cloud platform.
 They define the physical constraints of our QPUs and these constraints enforce some rules on
 the pulser sequence that can be run on QPUs (e.g. max amount of atoms, available pulse channels, ...)
 
 ```python
-sdk.get_device_specs_list()
+sdk.get_device_specs_dict()
 ```
 
 The method returns a dict object mapping a device type to a serialized device specs. These specs can be used
 to instantiate a `Device` instance in the `Pulser` library.
 
 
 ### Target different API endpoints
@@ -183,13 +184,13 @@
 
 To target a specific environment (`prod`, `preprod` or `dev`), instantiate the SDK class using 
 `PASQAL_ENDPOINTS['env']` for the parameter `endpoints` and `AUTH0_CONFIG['env']` for 
 `auth0` with env being the environment you want to target.
 
 Example:
 ```python
-from pasqal_cloud import SDK
+from pasqal_cloud import AUTH0_CONFIG, SDK, PASQAL_ENDPOINTS
 
-sdk = SDK(..., endpoints=PASQAL_ENDPOINTS['preprod'], auth0=AUTH_CONFIG['preprod'])
+sdk = SDK(..., endpoints=PASQAL_ENDPOINTS['preprod'], auth0=AUTH0_CONFIG['preprod'])
 ```
 
 By default, the targeted environment for `endpoints` and `auth0` is `prod`.
```

### Comparing `pasqal-cloud-0.2.7/README.md` & `pasqal-cloud-0.2.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,16 @@
 ### Authentication
 
 There are several ways to provide a correct authentication using the SDK.
 
 ```python
 from pasqal_cloud import SDK
 
-project_id="your_project_id" # Replace this value by your project_id on the PASQAL platform.
+project_id="your_project_id" # Replace this value by your project_id. It can be found on the user portal under the name "group_id". "Groups" have recently been renamed to "projects" and frontend is currently being updated accordingly.
+
 username="your_username" # Replace this value by your username or email on the PASQAL platform.
 password="your_password" # Replace this value by your password on the PASQAL platform.
 # Ideally, do not write this password in a script but provide in through the command-line or as a secret environment variable.
 
 """ Method 1: Username + Password
     If you know your credentials, you can pass them to the SDK instance on creation.
 """
@@ -150,15 +151,15 @@
 ### List of supported device specifications
 
 The SDK provides a method to retrieve the devices specs currently defined on PASQAL's cloud platform.
 They define the physical constraints of our QPUs and these constraints enforce some rules on
 the pulser sequence that can be run on QPUs (e.g. max amount of atoms, available pulse channels, ...)
 
 ```python
-sdk.get_device_specs_list()
+sdk.get_device_specs_dict()
 ```
 
 The method returns a dict object mapping a device type to a serialized device specs. These specs can be used
 to instantiate a `Device` instance in the `Pulser` library.
 
 
 ### Target different API endpoints
@@ -168,13 +169,13 @@
 
 To target a specific environment (`prod`, `preprod` or `dev`), instantiate the SDK class using 
 `PASQAL_ENDPOINTS['env']` for the parameter `endpoints` and `AUTH0_CONFIG['env']` for 
 `auth0` with env being the environment you want to target.
 
 Example:
 ```python
-from pasqal_cloud import SDK
+from pasqal_cloud import AUTH0_CONFIG, SDK, PASQAL_ENDPOINTS
 
-sdk = SDK(..., endpoints=PASQAL_ENDPOINTS['preprod'], auth0=AUTH_CONFIG['preprod'])
+sdk = SDK(..., endpoints=PASQAL_ENDPOINTS['preprod'], auth0=AUTH0_CONFIG['preprod'])
 ```
 
 By default, the targeted environment for `endpoints` and `auth0` is `prod`.
```

### Comparing `pasqal-cloud-0.2.7/pasqal_cloud/__init__.py` & `pasqal-cloud-0.2.8/pasqal_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.7/pasqal_cloud/_version.py` & `pasqal-cloud-0.2.8/pasqal_cloud/_version.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.7"
+__version__ = "0.2.8"
```

### Comparing `pasqal-cloud-0.2.7/pasqal_cloud/authentication.py` & `pasqal-cloud-0.2.8/pasqal_cloud/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.7/pasqal_cloud/batch.py` & `pasqal-cloud-0.2.8/pasqal_cloud/batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     complete: bool
     created_at: str
     updated_at: str
     device_type: str
     project_id: str
     id: str
-    user_id: int
+    user_id: str
     priority: int
     status: str
     webhook: Optional[str]
     _client: Client
     sequence_builder: str
     start_datetime: Optional[str]
     end_datetime: Optional[str]
```

### Comparing `pasqal-cloud-0.2.7/pasqal_cloud/client.py` & `pasqal-cloud-0.2.8/pasqal_cloud/client.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.7/pasqal_cloud/device/configuration/base_config.py` & `pasqal-cloud-0.2.8/pasqal_cloud/device/configuration/base_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.7/pasqal_cloud/device/configuration/emu_tn.py` & `pasqal-cloud-0.2.8/pasqal_cloud/device/configuration/emu_tn.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.7/pasqal_cloud/endpoints.py` & `pasqal-cloud-0.2.8/pasqal_cloud/endpoints.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.7/pasqal_cloud/errors.py` & `pasqal-cloud-0.2.8/pasqal_cloud/errors.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.7/pasqal_cloud/job.py` & `pasqal-cloud-0.2.8/pasqal_cloud/job.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.7/pasqal_cloud/utils/jsend.py` & `pasqal-cloud-0.2.8/pasqal_cloud/utils/jsend.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.7/pasqal_cloud.egg-info/PKG-INFO` & `pasqal-cloud-0.2.8/pasqal_cloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.2.7
+Version: 0.2.8
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -98,15 +98,16 @@
 ### Authentication
 
 There are several ways to provide a correct authentication using the SDK.
 
 ```python
 from pasqal_cloud import SDK
 
-project_id="your_project_id" # Replace this value by your project_id on the PASQAL platform.
+project_id="your_project_id" # Replace this value by your project_id. It can be found on the user portal under the name "group_id". "Groups" have recently been renamed to "projects" and frontend is currently being updated accordingly.
+
 username="your_username" # Replace this value by your username or email on the PASQAL platform.
 password="your_password" # Replace this value by your password on the PASQAL platform.
 # Ideally, do not write this password in a script but provide in through the command-line or as a secret environment variable.
 
 """ Method 1: Username + Password
     If you know your credentials, you can pass them to the SDK instance on creation.
 """
@@ -165,15 +166,15 @@
 ### List of supported device specifications
 
 The SDK provides a method to retrieve the devices specs currently defined on PASQAL's cloud platform.
 They define the physical constraints of our QPUs and these constraints enforce some rules on
 the pulser sequence that can be run on QPUs (e.g. max amount of atoms, available pulse channels, ...)
 
 ```python
-sdk.get_device_specs_list()
+sdk.get_device_specs_dict()
 ```
 
 The method returns a dict object mapping a device type to a serialized device specs. These specs can be used
 to instantiate a `Device` instance in the `Pulser` library.
 
 
 ### Target different API endpoints
@@ -183,13 +184,13 @@
 
 To target a specific environment (`prod`, `preprod` or `dev`), instantiate the SDK class using 
 `PASQAL_ENDPOINTS['env']` for the parameter `endpoints` and `AUTH0_CONFIG['env']` for 
 `auth0` with env being the environment you want to target.
 
 Example:
 ```python
-from pasqal_cloud import SDK
+from pasqal_cloud import AUTH0_CONFIG, SDK, PASQAL_ENDPOINTS
 
-sdk = SDK(..., endpoints=PASQAL_ENDPOINTS['preprod'], auth0=AUTH_CONFIG['preprod'])
+sdk = SDK(..., endpoints=PASQAL_ENDPOINTS['preprod'], auth0=AUTH0_CONFIG['preprod'])
 ```
 
 By default, the targeted environment for `endpoints` and `auth0` is `prod`.
```

### Comparing `pasqal-cloud-0.2.7/pasqal_cloud.egg-info/SOURCES.txt` & `pasqal-cloud-0.2.8/pasqal_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.7/sdk/setup.py` & `pasqal-cloud-0.2.8/sdk/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.7/setup.py` & `pasqal-cloud-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.7/tests/conftest.py` & `pasqal-cloud-0.2.8/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     batch_data = {
         "complete": False,
         "created_at": "2022-12-31T23:59:59.999Z",
         "updated_at": "2023-01-01T00:00:00.000Z",
         "device_type": "qpu",
         "project_id": "00000000-0000-0000-0000-000000000002",
         "id": "00000000-0000-0000-0000-000000000001",
-        "user_id": 1,
+        "user_id": "EQZj1ZQE",
         "priority": 0,
         "status": "PENDING",
         "webhook": "https://example.com/webhook",
         "_client": pasqal_client_mock,
         "sequence_builder": "pulser",
         "start_datetime": "2023-01-01T00:00:00.000Z",
         "end_datetime": None,
```

### Comparing `pasqal-cloud-0.2.7/tests/test_batch.py` & `pasqal-cloud-0.2.8/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.7/tests/test_client.py` & `pasqal-cloud-0.2.8/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.7/tests/test_cloud_sdk_import.py` & `pasqal-cloud-0.2.8/tests/test_cloud_sdk_import.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.7/tests/test_config.py` & `pasqal-cloud-0.2.8/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.7/tests/test_device_specs.py` & `pasqal-cloud-0.2.8/tests/test_device_specs.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.7/tests/test_doubles/authentication.py` & `pasqal-cloud-0.2.8/tests/test_doubles/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.7/tests/test_job.py` & `pasqal-cloud-0.2.8/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.7/tests/test_project_renaming_compatibility.py` & `pasqal-cloud-0.2.8/tests/test_project_renaming_compatibility.py`

 * *Files identical despite different names*

