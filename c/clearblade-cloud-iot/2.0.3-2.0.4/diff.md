# Comparing `tmp/clearblade-cloud-iot-2.0.3.tar.gz` & `tmp/clearblade-cloud-iot-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clearblade-cloud-iot-2.0.3.tar", last modified: Tue Jun  6 17:38:15 2023, max compression
+gzip compressed data, was "dist/clearblade-cloud-iot-2.0.4.tar", last modified: Mon Jun 19 12:05:52 2023, max compression
```

## Comparing `clearblade-cloud-iot-2.0.3.tar` & `clearblade-cloud-iot-2.0.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/clearblade/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/
--rw-rw-r--   0 root         (0) root         (0)    22605 2023-06-06 17:32:57.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/device_types.py
--rw-rw-r--   0 root         (0) root         (0)    13659 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/developer_tests.py
--rw-rw-r--   0 root         (0) root         (0)     6471 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/resources.py
--rw-rw-r--   0 root         (0) root         (0)     9331 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/registry.py
--rw-rw-r--   0 root         (0) root         (0)     7497 2023-05-20 17:29:53.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/config_manager.py
--rw-rw-r--   0 root         (0) root         (0)     8201 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/registry_types.py
--rw-rw-r--   0 root         (0) root         (0)     3742 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8386 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/http_client.py
--rw-rw-r--   0 root         (0) root         (0)     2942 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/config.py
--rw-rw-r--   0 root         (0) root         (0)    22724 2023-05-23 13:52:19.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/devices.py
--rw-rw-r--   0 root         (0) root         (0)    10305 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/client.py
--rw-rw-r--   0 root         (0) root         (0)     7622 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/pagers.py
--rw-rw-r--   0 root         (0) root         (0)     3255 2023-05-26 17:20:22.000000 clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/utils.py
--rw-rw-r--   0 root         (0) root         (0)    11358 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.3/LICENSE
--rw-rw-r--   0 root         (0) root         (0)     1442 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.3/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)     5090 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/google/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/google/cloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/google/cloud/iot/
--rw-rw-r--   0 root         (0) root         (0)       77 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.3/google/cloud/iot/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/google/cloud/iot_v1/
--rw-rw-r--   0 root         (0) root         (0)       77 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.3/google/cloud/iot_v1/py.typed
--rw-rw-r--   0 root         (0) root         (0)     5506 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.3/google/cloud/iot_v1/gapic_metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/tests/unit/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/tests/unit/gapic/
--rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.3/tests/unit/gapic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/tests/unit/gapic/iot_v1/
--rw-rw-r--   0 root         (0) root         (0)   235456 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.3/tests/unit/gapic/iot_v1/test_device_manager.py
--rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.3/tests/unit/gapic/iot_v1/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.3/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/tests/system/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/tests/system/gapic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/tests/system/gapic/v1/
--rw-rw-r--   0 root         (0) root         (0)     1557 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.3/tests/system/gapic/v1/test_system_device_manager_v1.py
--rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.3/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       67 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2835 2023-06-06 17:34:52.000000 clearblade-cloud-iot-2.0.3/setup.py
--rw-r--r--   0 root         (0) root         (0)     7002 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/clearblade_cloud_iot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1152 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/clearblade_cloud_iot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/clearblade_cloud_iot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/clearblade_cloud_iot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/clearblade_cloud_iot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     7002 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/clearblade_cloud_iot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-13 22:31:57.000000 clearblade-cloud-iot-2.0.3/clearblade_cloud_iot.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       28 2023-06-06 17:38:15.000000 clearblade-cloud-iot-2.0.3/clearblade_cloud_iot.egg-info/namespace_packages.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/clearblade/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/clearblade/cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/
+-rw-rw-r--   0 root         (0) root         (0)    22604 2023-06-19 11:47:15.000000 clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/device_types.py
+-rw-rw-r--   0 root         (0) root         (0)    13659 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/developer_tests.py
+-rw-rw-r--   0 root         (0) root         (0)     6471 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/resources.py
+-rw-rw-r--   0 root         (0) root         (0)     9331 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/registry.py
+-rw-rw-r--   0 root         (0) root         (0)     8728 2023-06-19 11:47:15.000000 clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/config_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     8201 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/registry_types.py
+-rw-rw-r--   0 root         (0) root         (0)     3742 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8386 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/http_client.py
+-rw-rw-r--   0 root         (0) root         (0)     2942 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/config.py
+-rw-rw-r--   0 root         (0) root         (0)    22723 2023-06-19 11:47:15.000000 clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/devices.py
+-rw-rw-r--   0 root         (0) root         (0)    10305 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/client.py
+-rw-rw-r--   0 root         (0) root         (0)     7622 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/pagers.py
+-rw-rw-r--   0 root         (0) root         (0)     3255 2023-05-26 17:20:22.000000 clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/utils.py
+-rw-rw-r--   0 root         (0) root         (0)    11358 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.4/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)     1442 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.4/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)     4525 2023-06-19 12:01:14.000000 clearblade-cloud-iot-2.0.4/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/google/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/google/cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/google/cloud/iot/
+-rw-rw-r--   0 root         (0) root         (0)       77 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.4/google/cloud/iot/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/google/cloud/iot_v1/
+-rw-rw-r--   0 root         (0) root         (0)       77 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.4/google/cloud/iot_v1/py.typed
+-rw-rw-r--   0 root         (0) root         (0)     5506 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.4/google/cloud/iot_v1/gapic_metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/tests/unit/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/tests/unit/gapic/
+-rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.4/tests/unit/gapic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/tests/unit/gapic/iot_v1/
+-rw-rw-r--   0 root         (0) root         (0)   235456 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.4/tests/unit/gapic/iot_v1/test_device_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.4/tests/unit/gapic/iot_v1/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.4/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/tests/system/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/tests/system/gapic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/tests/system/gapic/v1/
+-rw-rw-r--   0 root         (0) root         (0)     1557 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.4/tests/system/gapic/v1/test_system_device_manager_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.4/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2835 2023-06-19 12:03:17.000000 clearblade-cloud-iot-2.0.4/setup.py
+-rw-r--r--   0 root         (0) root         (0)     6309 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/clearblade_cloud_iot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/clearblade_cloud_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/clearblade_cloud_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/clearblade_cloud_iot.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/clearblade_cloud_iot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     6309 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/clearblade_cloud_iot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-13 22:31:57.000000 clearblade-cloud-iot-2.0.4/clearblade_cloud_iot.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-19 12:05:52.000000 clearblade-cloud-iot-2.0.4/clearblade_cloud_iot.egg-info/namespace_packages.txt
```

### Comparing `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/device_types.py` & `clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/device_types.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -630,8 +630,8 @@
             for device_json in devices_json:
                 device = Device.from_json(device_json)
                 devices.append(device)
 
         if 'nextPageToken' in devices_list_json:
             next_page_token = devices_list_json['nextPageToken']
 
-        return ListDevicesResponse(devices=devices, next_page_token=next_page_token)
+        return ListDevicesResponse(devices=devices, next_page_token=next_page_token)
```

### Comparing `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/developer_tests.py` & `clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/developer_tests.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/resources.py` & `clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/resources.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/registry.py` & `clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/registry.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/config_manager.py` & `clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/config_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,14 +78,19 @@
         auth_token = service_account_data['token']
         api_url = service_account_data['url']
         project = service_account_data['project']
 
         self._admin_config = ClearBladeConfig(system_key=system_key, auth_token=auth_token,
                                                  api_url=api_url, project=project)
 
+    def _create_regional_config_from_env(self, systemKey:str = None, serviceAccountToken:str = None, url:str = None, region:str = None)-> ClearBladeConfig :
+        return ClearBladeConfig(system_key=systemKey, auth_token=serviceAccountToken, api_url=url,
+                                region=region, project=self._admin_config.project)
+
+    
     def _create_regional_config(self, regional_json: json = None)-> ClearBladeConfig :
         system_key = regional_json['systemKey']
         auth_token = regional_json['serviceAccountToken']
         api_url = regional_json['url']
         region = regional_json['region']
 
         return ClearBladeConfig(system_key=system_key, auth_token=auth_token, api_url=api_url,
@@ -98,53 +103,62 @@
             region = self.region_name
 
         if not registry:
             registry = self.registry_name
 
         if not region or not registry:
             raise Exception("Either location or registry name is not provided")
-
-        sync_client = SyncClient(clearblade_config=self._admin_config)
-        request_body = {'region':region,'registry':registry, 'project':self._admin_config.project}
-        response = sync_client.post(api_name="getRegistryCredentials", is_webhook_folder=False,
-                                    request_body=request_body)
-
-        if response.status_code != 200:
-            raise Exception(
-                f"\n\nRegistry Information not found! Please check if the given registry exists\nProject: {self._admin_config.project}\nRegistry: {registry}\nRegion: {region}"
-                )
-
-        response_json = response.json()
-        response_json['region'] = region
-        self._regional_config = self._create_regional_config(regional_json=response_json)
+        
+        system_key = os.environ.get("REGISTRY_SYSKEY")
+        registry_token = os.environ.get("REGISTRY_TOKEN")
+        url = os.environ.get("REGISTRY_URL")
+        if (system_key and registry_token and url) :
+            self._regional_config = self._create_regional_config_from_env(systemKey=system_key , serviceAccountToken = registry_token, url = url, region = region)
+        else :
+            request_body = {'region':region,'registry':registry, 'project':self._admin_config.project}
+            sync_client = SyncClient(clearblade_config=self._admin_config)
+            response = sync_client.post(api_name="getRegistryCredentials", is_webhook_folder=False,
+                                        request_body=request_body)
+            if response.status_code != 200:
+                raise Exception(
+                    f"\n\nRegistry Information not found! Please check if the given registry exists\nProject: {self._admin_config.project}\nRegistry: {registry}\nRegion: {region}"
+                    )
+            response_json = response.json()
+            response_json['region'] = region
+            self._regional_config = self._create_regional_config(regional_json=response_json) 
+            
 
     async def _set_regional_config_async(self, region:str = None, registry:str = None):
 
         self._set_admin_clearblade_config()
 
         if not region:
             region = self._region_name
 
         if not registry:
             registry = self.registry_name
-
-        async_client = AsyncClient(clearblade_config=self._admin_config)
-        request_body = {'region':region,'registry':registry, 'project':self._admin_config.project}
-        response = await async_client.post(api_name="getRegistryCredentials",
-                                           is_webhook_folder=False,
-                                           request_body=request_body)
-
-        if response.status_code != 200:
-            raise Exception(
-                f"\n\nRegistry Information not found! Please check if the given registry exists\nProject: {self._admin_config.project}\nRegistry: {registry}\nRegion: {region}"
-                )
-
-        response_json = response.json()
-        response_json['region'] = region
-        self._regional_config = self._create_regional_config(regional_json=response_json)
+        system_key = os.environ.get("REGISTRY_SYSKEY")
+        registry_token = os.environ.get("REGISTRY_TOKEN")
+        url = os.environ.get("REGISTRY_URL")
+        if (system_key and registry_token) :
+            self._regional_config = self._create_regional_config_from_env(systemKey=system_key , serviceAccountToken = registry_token, url = url, region = region)
+        else :            
+            async_client = AsyncClient(clearblade_config=self._admin_config)
+            request_body = {'region':region,'registry':registry, 'project':self._admin_config.project}
+            response = await async_client.post(api_name="getRegistryCredentials",
+                                            is_webhook_folder=False,
+                                            request_body=request_body)
+
+            if response.status_code != 200:
+                raise Exception(
+                    f"\n\nRegistry Information not found! Please check if the given registry exists\nProject: {self._admin_config.project}\nRegistry: {registry}\nRegion: {region}"
+                    )
+            response_json = response.json()
+            response_json['region'] = region
+            self._regional_config = self._create_regional_config(regional_json=response_json)
 
 
     @property
     def admin_config(self):
         if not self._admin_config:
             self._set_admin_clearblade_config()
```

### Comparing `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/registry_types.py` & `clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/registry_types.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/__init__.py` & `clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/http_client.py` & `clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/http_client.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/config.py` & `clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/config.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/devices.py` & `clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/devices.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -486,8 +486,8 @@
         params = {'name':request.parent, 'numVersions':request.numVersions}
         clearblade_config = await self._config_manager.regional_config_async(request.parent)
         async_client = AsyncClient(clearblade_config=clearblade_config)
         response = await async_client.get(api_name="cloudiot_devices_configVersions", request_params=params)
 
         if response.status_code == 200:
             return ListDeviceConfigVersionsResponse.from_json(response.json())
-        return response
+        return response
```

### Comparing `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/client.py` & `clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/client.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/pagers.py` & `clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/pagers.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.3/clearblade/cloud/iot_v1/utils.py` & `clearblade-cloud-iot-2.0.4/clearblade/cloud/iot_v1/utils.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.3/LICENSE` & `clearblade-cloud-iot-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.3/MANIFEST.in` & `clearblade-cloud-iot-2.0.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.3/README.rst` & `clearblade-cloud-iot-2.0.4/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,52 @@
-.. Copyright 2023 ClearBlade Inc.
-    Licensed under the Apache License, Version 2.0 (the "License");
-    you may not use this file except in compliance with the License.
-    You may obtain a copy of the License at
-        http://www.apache.org/licenses/LICENSE-2.0
-    Unless required by applicable law or agreed to in writing, software
-    distributed under the License is distributed on an "AS IS" BASIS,
-    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-    See the License for the specific language governing permissions and
-    limitations under the License.
-    Copyright 2022 Google LLC
-    Licensed under the Apache License, Version 2.0 (the "License");
-    you may not use this file except in compliance with the License.
-    You may obtain a copy of the License at
-        http://www.apache.org/licenses/LICENSE-2.0
-    Unless required by applicable law or agreed to in writing, software
-    distributed under the License is distributed on an "AS IS" BASIS,
-    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-    See the License for the specific language governing permissions and
-    limitations under the License.
- 
-Python Client for ClearBlade Internet of Things (IoT) Core API
+Python Client for ClearBlade IoT Core API
 ================================================================
 
-Quick Start
+Quick start
 -----------
 
-In order to use this library, you first need to go through the following steps:
+To use this library, you first need to go through the following steps:
 
 1. Install pip package - ```pip install clearblade-cloud-iot```
 
-
-2. Set an environment variable **CLEARBLADE_CONFIGURATION** which should point to your clearblade service account json file.
+2. Set an environment variable **CLEARBLADE_CONFIGURATION**, pointing to your ClearBlade service account JSON file.
 
 3. Optionally set an environment variable **BINARYDATA_AND_TIME_GOOGLE_FORMAT** to True. Look at **Note about types of times and binaryData** below for details. 
 
 Installation
 ~~~~~~~~~~~~
 
-Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
-create isolated Python environments. The basic problem it addresses is one of
-dependencies and versions, and indirectly permissions.
-
-With `virtualenv`_, it's possible to install this library without needing system
-install permissions, and without clashing with the installed system
-dependencies.
+Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to create isolated Python environments. It addresses dependencies and versions and, indirectly, permissions.
+
+With `virtualenv`_, it's possible to install this library without system install permissions and clashing with the installed system dependencies.
 
 .. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
 
 
 Code samples and snippets
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Code samples and snippets live in the `samples/clearblade` folder.
+Code samples and snippets live in the samples/clearblade folder.
 
 
-Supported Python Versions
+Supported Python versions
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 Our client libraries are compatible with all current `active`_ and `maintenance`_ versions of
 Python.
 
 Python >= 3.7
 
 .. _active: https://devguide.python.org/devcycle/#in-development-main-branch
 .. _maintenance: https://devguide.python.org/devcycle/#maintenance-branches
 
-Unsupported Python Versions
+Unsupported Python versions
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^
 Python <= 3.6
 
-If you are using an `end-of-life`_
-version of Python, we recommend that you update as soon as possible to an actively supported version.
+If you are using an `end-of-life`_ version of Python, we recommend you update it to an actively supported version as soon as possible.
 
 .. _end-of-life: https://devguide.python.org/devcycle/#end-of-life-branches
 
 Mac/Linux
 ^^^^^^^^^
 
 .. code-block:: console
@@ -88,48 +61,58 @@
 
 .. code-block:: console
 
     pip install virtualenv
     virtualenv <your-env>
     <your-env>\Scripts\activate
 
-Next Steps
+Next steps
 ~~~~~~~~~~
 
-- clone the github repository.
+- Clone the GitHub repository.
 
-- and execute the setup.py file like , python setup.py install.
+- Execute the setup.py file like Python setup.py install.
 
-- mostly if you change you imports from from google.cloud to clearblade.cloud everything else should work.
+- Everything else should work if you change your imports from google.cloud to clearblade.cloud.
 
 Note about types of times and binaryData
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-- By default the following parameters are returned as the shown types:
+- By default, the following parameters are returned as the shown types:
 
 1. All time parameters (e.g. **cloudUpdateTime**, **deviceAckTime**, **updateTime**): **RFC3339** strings (e.g. "2023-01-12T23:38:07.732Z")
 2. **CONFIG binaryData**: **base64-encoded string**
 3. **STATE binaryData**: **NON-base64-encoded string**
 
 
 - To return these parameters using the same types used by the **Google IoTCore Python SDK**, set environment variable **BINARYDATA_AND_TIME_GOOGLE_FORMAT** to **True** (case-insensitive string). This will ensure the following parameters are returned as the shown types:
 
 1. All times: **DatetimeWithNanoseconds** (defined in the **proto.datetime_helpers** module)
 2. All **binaryData** (CONFIG, STATE etc.): **BYTE ARRAYS**
 
-- If this environment variable is not set, or is set to any unexpeced values, then the default types listed previously are used.
+- If this environment variable is not set, or is set to any unexpected values, then the default types listed previously are used.
+
+Note about performance:
+~~~~~~~~~~~~~~~~~~~~~~~
+
+- By default calls to some SDK functions cause a REST request to be sent to acquire the Registry API Keys found on the IoTCore UI Registry Details page. Those keys are cached for subsequent operations in order to improve performance. However these caches do not persist if the application is stopped and restarted as would be the case with typical serverless functions (e.g. Google Cloud Functions, AWS Lambda etc.). In order to improve the performance of those functions, the REST call can be prevented by passing the API Keys as environment variables:
+
+1. **REGISTRY_URL**: **string**
+2. **REGISTRY_SYSKEY**: **string**
+3. **REGISTRY_TOKEN**: **string**
+
+Note about running from the source instead of the PyPi (pip) module:
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Note about running from source instead of PyPi (pip) module:
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-- To temporarily use the source code in this repo. instead of the installed PyPi (pip) module do the following:
+- To temporarily use the source code in this repo instead of the installed PyPi (pip) module, do the following:
 
 1. Clone this repo.
-2. Checkout the desired branch using **git checkout <branch>**.
+2. Check out the desired branch using **git checkout <branch>**.
 3. In your code find where **clearblade** or **clearblade.cloud** is being imported.
-4. Precede that line with **import sys** and **sys.path.insert(0, <path_to_python-iot>)**. The path must end with "python-iot". So for example:
+4. Precede that line with **import sys** and **sys.path.insert(0, <path_to_python-iot>)**. The path must end with python-iot. For example:
 
 .. code-block:: console
 
     import sys
     sys.path.insert(0, "path/to/python-iot")
 
-    from clearblade.cloud import iot_v1
+    from clearblade.cloud import iot_v1
```

### Comparing `clearblade-cloud-iot-2.0.3/google/cloud/iot_v1/gapic_metadata.json` & `clearblade-cloud-iot-2.0.4/google/cloud/iot_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.3/tests/unit/gapic/__init__.py` & `clearblade-cloud-iot-2.0.4/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.3/tests/unit/gapic/iot_v1/test_device_manager.py` & `clearblade-cloud-iot-2.0.4/tests/unit/gapic/iot_v1/test_device_manager.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.3/tests/unit/gapic/iot_v1/__init__.py` & `clearblade-cloud-iot-2.0.4/tests/unit/gapic/iot_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.3/tests/unit/__init__.py` & `clearblade-cloud-iot-2.0.4/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.3/tests/system/gapic/v1/test_system_device_manager_v1.py` & `clearblade-cloud-iot-2.0.4/tests/system/gapic/v1/test_system_device_manager_v1.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.3/tests/__init__.py` & `clearblade-cloud-iot-2.0.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.3/setup.py` & `clearblade-cloud-iot-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import io
 import os
 
 import setuptools
 
 name = "clearblade-cloud-iot"
 description = "Cloud IoT API client library"
-version = "2.0.3"
+version = "2.0.4"
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = ["httpx", "proto-plus"]
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
```

### Comparing `clearblade-cloud-iot-2.0.3/PKG-INFO` & `clearblade-cloud-iot-2.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,60 @@
 Metadata-Version: 1.2
 Name: clearblade-cloud-iot
-Version: 2.0.3
+Version: 2.0.4
 Summary: Cloud IoT API client library
 Home-page: https://github.com/clearblade/python-iot
 Author: Clearblade
 Author-email: googleapis-packages@oogle.com
 License: Apache 2.0
-Description: .. Copyright 2023 ClearBlade Inc.
-            Licensed under the Apache License, Version 2.0 (the "License");
-            you may not use this file except in compliance with the License.
-            You may obtain a copy of the License at
-                http://www.apache.org/licenses/LICENSE-2.0
-            Unless required by applicable law or agreed to in writing, software
-            distributed under the License is distributed on an "AS IS" BASIS,
-            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-            See the License for the specific language governing permissions and
-            limitations under the License.
-            Copyright 2022 Google LLC
-            Licensed under the Apache License, Version 2.0 (the "License");
-            you may not use this file except in compliance with the License.
-            You may obtain a copy of the License at
-                http://www.apache.org/licenses/LICENSE-2.0
-            Unless required by applicable law or agreed to in writing, software
-            distributed under the License is distributed on an "AS IS" BASIS,
-            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-            See the License for the specific language governing permissions and
-            limitations under the License.
-         
-        Python Client for ClearBlade Internet of Things (IoT) Core API
+Description: Python Client for ClearBlade IoT Core API
         ================================================================
         
-        Quick Start
+        Quick start
         -----------
         
-        In order to use this library, you first need to go through the following steps:
+        To use this library, you first need to go through the following steps:
         
         1. Install pip package - ```pip install clearblade-cloud-iot```
         
-        
-        2. Set an environment variable **CLEARBLADE_CONFIGURATION** which should point to your clearblade service account json file.
+        2. Set an environment variable **CLEARBLADE_CONFIGURATION**, pointing to your ClearBlade service account JSON file.
         
         3. Optionally set an environment variable **BINARYDATA_AND_TIME_GOOGLE_FORMAT** to True. Look at **Note about types of times and binaryData** below for details. 
         
         Installation
         ~~~~~~~~~~~~
         
-        Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
-        create isolated Python environments. The basic problem it addresses is one of
-        dependencies and versions, and indirectly permissions.
-        
-        With `virtualenv`_, it's possible to install this library without needing system
-        install permissions, and without clashing with the installed system
-        dependencies.
+        Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to create isolated Python environments. It addresses dependencies and versions and, indirectly, permissions.
+        
+        With `virtualenv`_, it's possible to install this library without system install permissions and clashing with the installed system dependencies.
         
         .. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
         
         
         Code samples and snippets
         ~~~~~~~~~~~~~~~~~~~~~~~~~
         
-        Code samples and snippets live in the `samples/clearblade` folder.
+        Code samples and snippets live in the samples/clearblade folder.
         
         
-        Supported Python Versions
+        Supported Python versions
         ^^^^^^^^^^^^^^^^^^^^^^^^^
         Our client libraries are compatible with all current `active`_ and `maintenance`_ versions of
         Python.
         
         Python >= 3.7
         
         .. _active: https://devguide.python.org/devcycle/#in-development-main-branch
         .. _maintenance: https://devguide.python.org/devcycle/#maintenance-branches
         
-        Unsupported Python Versions
+        Unsupported Python versions
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^
         Python <= 3.6
         
-        If you are using an `end-of-life`_
-        version of Python, we recommend that you update as soon as possible to an actively supported version.
+        If you are using an `end-of-life`_ version of Python, we recommend you update it to an actively supported version as soon as possible.
         
         .. _end-of-life: https://devguide.python.org/devcycle/#end-of-life-branches
         
         Mac/Linux
         ^^^^^^^^^
         
         .. code-block:: console
@@ -96,55 +69,66 @@
         
         .. code-block:: console
         
             pip install virtualenv
             virtualenv <your-env>
             <your-env>\Scripts\activate
         
-        Next Steps
+        Next steps
         ~~~~~~~~~~
         
-        - clone the github repository.
+        - Clone the GitHub repository.
         
-        - and execute the setup.py file like , python setup.py install.
+        - Execute the setup.py file like Python setup.py install.
         
-        - mostly if you change you imports from from google.cloud to clearblade.cloud everything else should work.
+        - Everything else should work if you change your imports from google.cloud to clearblade.cloud.
         
         Note about types of times and binaryData
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
-        - By default the following parameters are returned as the shown types:
+        - By default, the following parameters are returned as the shown types:
         
         1. All time parameters (e.g. **cloudUpdateTime**, **deviceAckTime**, **updateTime**): **RFC3339** strings (e.g. "2023-01-12T23:38:07.732Z")
         2. **CONFIG binaryData**: **base64-encoded string**
         3. **STATE binaryData**: **NON-base64-encoded string**
         
         
         - To return these parameters using the same types used by the **Google IoTCore Python SDK**, set environment variable **BINARYDATA_AND_TIME_GOOGLE_FORMAT** to **True** (case-insensitive string). This will ensure the following parameters are returned as the shown types:
         
         1. All times: **DatetimeWithNanoseconds** (defined in the **proto.datetime_helpers** module)
         2. All **binaryData** (CONFIG, STATE etc.): **BYTE ARRAYS**
         
-        - If this environment variable is not set, or is set to any unexpeced values, then the default types listed previously are used.
+        - If this environment variable is not set, or is set to any unexpected values, then the default types listed previously are used.
+        
+        Note about performance:
+        ~~~~~~~~~~~~~~~~~~~~~~~
+        
+        - By default calls to some SDK functions cause a REST request to be sent to acquire the Registry API Keys found on the IoTCore UI Registry Details page. Those keys are cached for subsequent operations in order to improve performance. However these caches do not persist if the application is stopped and restarted as would be the case with typical serverless functions (e.g. Google Cloud Functions, AWS Lambda etc.). In order to improve the performance of those functions, the REST call can be prevented by passing the API Keys as environment variables:
         
-        Note about running from source instead of PyPi (pip) module:
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        - To temporarily use the source code in this repo. instead of the installed PyPi (pip) module do the following:
+        1. **REGISTRY_URL**: **string**
+        2. **REGISTRY_SYSKEY**: **string**
+        3. **REGISTRY_TOKEN**: **string**
+        
+        Note about running from the source instead of the PyPi (pip) module:
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        - To temporarily use the source code in this repo instead of the installed PyPi (pip) module, do the following:
         
         1. Clone this repo.
-        2. Checkout the desired branch using **git checkout <branch>**.
+        2. Check out the desired branch using **git checkout <branch>**.
         3. In your code find where **clearblade** or **clearblade.cloud** is being imported.
-        4. Precede that line with **import sys** and **sys.path.insert(0, <path_to_python-iot>)**. The path must end with "python-iot". So for example:
+        4. Precede that line with **import sys** and **sys.path.insert(0, <path_to_python-iot>)**. The path must end with python-iot. For example:
         
         .. code-block:: console
         
             import sys
             sys.path.insert(0, "path/to/python-iot")
         
             from clearblade.cloud import iot_v1
+        
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `clearblade-cloud-iot-2.0.3/clearblade_cloud_iot.egg-info/SOURCES.txt` & `clearblade-cloud-iot-2.0.4/clearblade_cloud_iot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.3/clearblade_cloud_iot.egg-info/PKG-INFO` & `clearblade-cloud-iot-2.0.4/clearblade_cloud_iot.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,60 @@
 Metadata-Version: 1.2
 Name: clearblade-cloud-iot
-Version: 2.0.3
+Version: 2.0.4
 Summary: Cloud IoT API client library
 Home-page: https://github.com/clearblade/python-iot
 Author: Clearblade
 Author-email: googleapis-packages@oogle.com
 License: Apache 2.0
-Description: .. Copyright 2023 ClearBlade Inc.
-            Licensed under the Apache License, Version 2.0 (the "License");
-            you may not use this file except in compliance with the License.
-            You may obtain a copy of the License at
-                http://www.apache.org/licenses/LICENSE-2.0
-            Unless required by applicable law or agreed to in writing, software
-            distributed under the License is distributed on an "AS IS" BASIS,
-            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-            See the License for the specific language governing permissions and
-            limitations under the License.
-            Copyright 2022 Google LLC
-            Licensed under the Apache License, Version 2.0 (the "License");
-            you may not use this file except in compliance with the License.
-            You may obtain a copy of the License at
-                http://www.apache.org/licenses/LICENSE-2.0
-            Unless required by applicable law or agreed to in writing, software
-            distributed under the License is distributed on an "AS IS" BASIS,
-            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-            See the License for the specific language governing permissions and
-            limitations under the License.
-         
-        Python Client for ClearBlade Internet of Things (IoT) Core API
+Description: Python Client for ClearBlade IoT Core API
         ================================================================
         
-        Quick Start
+        Quick start
         -----------
         
-        In order to use this library, you first need to go through the following steps:
+        To use this library, you first need to go through the following steps:
         
         1. Install pip package - ```pip install clearblade-cloud-iot```
         
-        
-        2. Set an environment variable **CLEARBLADE_CONFIGURATION** which should point to your clearblade service account json file.
+        2. Set an environment variable **CLEARBLADE_CONFIGURATION**, pointing to your ClearBlade service account JSON file.
         
         3. Optionally set an environment variable **BINARYDATA_AND_TIME_GOOGLE_FORMAT** to True. Look at **Note about types of times and binaryData** below for details. 
         
         Installation
         ~~~~~~~~~~~~
         
-        Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
-        create isolated Python environments. The basic problem it addresses is one of
-        dependencies and versions, and indirectly permissions.
-        
-        With `virtualenv`_, it's possible to install this library without needing system
-        install permissions, and without clashing with the installed system
-        dependencies.
+        Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to create isolated Python environments. It addresses dependencies and versions and, indirectly, permissions.
+        
+        With `virtualenv`_, it's possible to install this library without system install permissions and clashing with the installed system dependencies.
         
         .. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
         
         
         Code samples and snippets
         ~~~~~~~~~~~~~~~~~~~~~~~~~
         
-        Code samples and snippets live in the `samples/clearblade` folder.
+        Code samples and snippets live in the samples/clearblade folder.
         
         
-        Supported Python Versions
+        Supported Python versions
         ^^^^^^^^^^^^^^^^^^^^^^^^^
         Our client libraries are compatible with all current `active`_ and `maintenance`_ versions of
         Python.
         
         Python >= 3.7
         
         .. _active: https://devguide.python.org/devcycle/#in-development-main-branch
         .. _maintenance: https://devguide.python.org/devcycle/#maintenance-branches
         
-        Unsupported Python Versions
+        Unsupported Python versions
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^
         Python <= 3.6
         
-        If you are using an `end-of-life`_
-        version of Python, we recommend that you update as soon as possible to an actively supported version.
+        If you are using an `end-of-life`_ version of Python, we recommend you update it to an actively supported version as soon as possible.
         
         .. _end-of-life: https://devguide.python.org/devcycle/#end-of-life-branches
         
         Mac/Linux
         ^^^^^^^^^
         
         .. code-block:: console
@@ -96,55 +69,66 @@
         
         .. code-block:: console
         
             pip install virtualenv
             virtualenv <your-env>
             <your-env>\Scripts\activate
         
-        Next Steps
+        Next steps
         ~~~~~~~~~~
         
-        - clone the github repository.
+        - Clone the GitHub repository.
         
-        - and execute the setup.py file like , python setup.py install.
+        - Execute the setup.py file like Python setup.py install.
         
-        - mostly if you change you imports from from google.cloud to clearblade.cloud everything else should work.
+        - Everything else should work if you change your imports from google.cloud to clearblade.cloud.
         
         Note about types of times and binaryData
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
-        - By default the following parameters are returned as the shown types:
+        - By default, the following parameters are returned as the shown types:
         
         1. All time parameters (e.g. **cloudUpdateTime**, **deviceAckTime**, **updateTime**): **RFC3339** strings (e.g. "2023-01-12T23:38:07.732Z")
         2. **CONFIG binaryData**: **base64-encoded string**
         3. **STATE binaryData**: **NON-base64-encoded string**
         
         
         - To return these parameters using the same types used by the **Google IoTCore Python SDK**, set environment variable **BINARYDATA_AND_TIME_GOOGLE_FORMAT** to **True** (case-insensitive string). This will ensure the following parameters are returned as the shown types:
         
         1. All times: **DatetimeWithNanoseconds** (defined in the **proto.datetime_helpers** module)
         2. All **binaryData** (CONFIG, STATE etc.): **BYTE ARRAYS**
         
-        - If this environment variable is not set, or is set to any unexpeced values, then the default types listed previously are used.
+        - If this environment variable is not set, or is set to any unexpected values, then the default types listed previously are used.
+        
+        Note about performance:
+        ~~~~~~~~~~~~~~~~~~~~~~~
+        
+        - By default calls to some SDK functions cause a REST request to be sent to acquire the Registry API Keys found on the IoTCore UI Registry Details page. Those keys are cached for subsequent operations in order to improve performance. However these caches do not persist if the application is stopped and restarted as would be the case with typical serverless functions (e.g. Google Cloud Functions, AWS Lambda etc.). In order to improve the performance of those functions, the REST call can be prevented by passing the API Keys as environment variables:
         
-        Note about running from source instead of PyPi (pip) module:
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        - To temporarily use the source code in this repo. instead of the installed PyPi (pip) module do the following:
+        1. **REGISTRY_URL**: **string**
+        2. **REGISTRY_SYSKEY**: **string**
+        3. **REGISTRY_TOKEN**: **string**
+        
+        Note about running from the source instead of the PyPi (pip) module:
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        - To temporarily use the source code in this repo instead of the installed PyPi (pip) module, do the following:
         
         1. Clone this repo.
-        2. Checkout the desired branch using **git checkout <branch>**.
+        2. Check out the desired branch using **git checkout <branch>**.
         3. In your code find where **clearblade** or **clearblade.cloud** is being imported.
-        4. Precede that line with **import sys** and **sys.path.insert(0, <path_to_python-iot>)**. The path must end with "python-iot". So for example:
+        4. Precede that line with **import sys** and **sys.path.insert(0, <path_to_python-iot>)**. The path must end with python-iot. For example:
         
         .. code-block:: console
         
             import sys
             sys.path.insert(0, "path/to/python-iot")
         
             from clearblade.cloud import iot_v1
+        
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

